# Comparing `tmp/trytond_account_dunning-7.2.0.tar.gz` & `tmp/trytond_account_dunning-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_dunning-7.2.0.tar", last modified: Mon Apr 29 15:32:34 2024, max compression
+gzip compressed data, was "trytond_account_dunning-7.2.1.tar", last modified: Wed May  1 12:24:26 2024, max compression
```

## Comparing `trytond_account_dunning-7.2.0.tar` & `trytond_account_dunning-7.2.1.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:32:34.351770 trytond_account_dunning-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     2146 2024-04-29 15:13:22.000000 trytond_account_dunning-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-04-29 15:13:21.000000 trytond_account_dunning-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_dunning-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_dunning-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3597 2024-04-29 15:32:34.351770 trytond_account_dunning-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1033 2023-01-16 14:00:20.000000 trytond_account_dunning-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      784 2023-04-15 07:12:15.000000 trytond_account_dunning-7.2.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1341 2023-04-15 07:12:14.000000 trytond_account_dunning-7.2.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)      900 2024-04-27 16:30:39.000000 trytond_account_dunning-7.2.0/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:32:34.345104 trytond_account_dunning-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3078 2024-04-27 16:30:39.000000 trytond_account_dunning-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1033 2023-01-16 14:00:20.000000 trytond_account_dunning-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:36:52.000000 trytond_account_dunning-7.2.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)    12757 2024-01-27 09:58:52.000000 trytond_account_dunning-7.2.0/dunning.py
--rw-r--r--   0 ced       (1000) ced       (1000)    14153 2024-04-27 16:30:39.000000 trytond_account_dunning-7.2.0/dunning.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:32:34.348437 trytond_account_dunning-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     7436 2024-04-27 16:43:20.000000 trytond_account_dunning-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7968 2024-04-27 16:43:20.000000 trytond_account_dunning-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6852 2024-04-27 16:43:20.000000 trytond_account_dunning-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7762 2024-04-27 16:43:20.000000 trytond_account_dunning-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8040 2024-04-27 16:43:20.000000 trytond_account_dunning-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7158 2024-04-27 16:43:20.000000 trytond_account_dunning-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7702 2024-04-27 16:43:20.000000 trytond_account_dunning-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8263 2024-04-27 16:43:20.000000 trytond_account_dunning-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6839 2024-04-27 16:43:20.000000 trytond_account_dunning-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7899 2024-04-27 16:43:20.000000 trytond_account_dunning-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8205 2024-04-27 16:43:20.000000 trytond_account_dunning-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6706 2024-04-27 16:43:20.000000 trytond_account_dunning-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7417 2024-04-27 16:43:20.000000 trytond_account_dunning-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8681 2024-04-27 16:43:20.000000 trytond_account_dunning-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6967 2024-04-27 16:43:20.000000 trytond_account_dunning-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7909 2024-04-27 16:43:20.000000 trytond_account_dunning-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6981 2024-04-27 16:43:20.000000 trytond_account_dunning-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7515 2024-04-27 16:43:20.000000 trytond_account_dunning-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7250 2024-04-29 13:17:17.000000 trytond_account_dunning-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7437 2024-04-27 16:43:20.000000 trytond_account_dunning-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7344 2024-04-27 16:43:20.000000 trytond_account_dunning-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7234 2024-04-27 16:43:20.000000 trytond_account_dunning-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6493 2024-04-27 16:43:20.000000 trytond_account_dunning-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6998 2024-04-27 16:43:20.000000 trytond_account_dunning-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      386 2023-04-15 07:12:15.000000 trytond_account_dunning-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1197 2024-04-22 12:14:36.000000 trytond_account_dunning-7.2.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)      454 2023-01-16 14:00:20.000000 trytond_account_dunning-7.2.0/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:32:34.351770 trytond_account_dunning-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4436 2024-03-17 11:01:36.000000 trytond_account_dunning-7.2.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:32:34.348437 trytond_account_dunning-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_dunning-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8257 2024-04-22 12:14:36.000000 trytond_account_dunning-7.2.0/tests/scenario_account_dunning.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2950 2024-04-22 12:14:36.000000 trytond_account_dunning-7.2.0/tests/scenario_account_dunning_final.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      408 2023-04-15 07:12:14.000000 trytond_account_dunning-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_dunning-7.2.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:36:52.000000 trytond_account_dunning-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      148 2024-04-29 15:13:17.000000 trytond_account_dunning-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:32:34.348437 trytond_account_dunning-7.2.0/trytond_account_dunning.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3597 2024-04-29 15:32:33.000000 trytond_account_dunning-7.2.0/trytond_account_dunning.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2300 2024-04-29 15:32:34.000000 trytond_account_dunning-7.2.0/trytond_account_dunning.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:32:33.000000 trytond_account_dunning-7.2.0/trytond_account_dunning.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       68 2024-04-29 15:32:33.000000 trytond_account_dunning-7.2.0/trytond_account_dunning.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:03.000000 trytond_account_dunning-7.2.0/trytond_account_dunning.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      136 2024-04-29 15:32:33.000000 trytond_account_dunning-7.2.0/trytond_account_dunning.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:32:33.000000 trytond_account_dunning-7.2.0/trytond_account_dunning.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:32:34.348437 trytond_account_dunning-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      424 2023-01-16 14:00:20.000000 trytond_account_dunning-7.2.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      405 2023-04-15 07:12:15.000000 trytond_account_dunning-7.2.0/view/dunning_create_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      808 2023-04-15 07:12:15.000000 trytond_account_dunning-7.2.0/view/dunning_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      378 2023-04-15 07:12:14.000000 trytond_account_dunning-7.2.0/view/dunning_level_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      266 2023-01-16 14:00:20.000000 trytond_account_dunning-7.2.0/view/dunning_level_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      286 2023-01-16 14:00:20.000000 trytond_account_dunning-7.2.0/view/dunning_level_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      548 2023-04-15 07:12:15.000000 trytond_account_dunning-7.2.0/view/dunning_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      343 2023-01-16 14:00:20.000000 trytond_account_dunning-7.2.0/view/dunning_procedure_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-01-16 14:00:20.000000 trytond_account_dunning-7.2.0/view/dunning_procedure_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      349 2023-04-15 07:12:15.000000 trytond_account_dunning-7.2.0/view/dunning_process_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      481 2023-01-16 14:00:20.000000 trytond_account_dunning-7.2.0/view/party_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:24:26.604729 trytond_account_dunning-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2247 2024-05-01 12:24:23.000000 trytond_account_dunning-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-05-01 12:24:23.000000 trytond_account_dunning-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:20:59.000000 trytond_account_dunning-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:20:59.000000 trytond_account_dunning-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3597 2024-05-01 12:24:26.604729 trytond_account_dunning-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1033 2024-04-30 17:20:59.000000 trytond_account_dunning-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      784 2024-04-30 17:20:59.000000 trytond_account_dunning-7.2.1/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1341 2024-04-30 17:20:59.000000 trytond_account_dunning-7.2.1/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      900 2024-04-30 17:20:59.000000 trytond_account_dunning-7.2.1/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:24:26.601396 trytond_account_dunning-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3078 2024-04-30 17:20:59.000000 trytond_account_dunning-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1033 2024-04-30 17:20:59.000000 trytond_account_dunning-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:20:59.000000 trytond_account_dunning-7.2.1/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)    12757 2024-04-30 17:20:59.000000 trytond_account_dunning-7.2.1/dunning.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    14153 2024-04-30 17:20:59.000000 trytond_account_dunning-7.2.1/dunning.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:24:26.601396 trytond_account_dunning-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     7436 2024-04-30 17:20:59.000000 trytond_account_dunning-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7976 2024-04-30 17:21:59.000000 trytond_account_dunning-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6852 2024-04-30 17:20:59.000000 trytond_account_dunning-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7762 2024-04-30 17:21:59.000000 trytond_account_dunning-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8043 2024-04-30 17:21:59.000000 trytond_account_dunning-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7158 2024-04-30 17:20:59.000000 trytond_account_dunning-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7702 2024-04-30 17:20:59.000000 trytond_account_dunning-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8263 2024-04-30 17:20:59.000000 trytond_account_dunning-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6839 2024-04-30 17:20:59.000000 trytond_account_dunning-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7899 2024-04-30 17:20:59.000000 trytond_account_dunning-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8205 2024-04-30 17:20:59.000000 trytond_account_dunning-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6706 2024-04-30 17:20:59.000000 trytond_account_dunning-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7417 2024-04-30 17:20:59.000000 trytond_account_dunning-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8681 2024-04-30 17:20:59.000000 trytond_account_dunning-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6967 2024-04-30 17:20:59.000000 trytond_account_dunning-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7909 2024-04-30 17:20:59.000000 trytond_account_dunning-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6981 2024-04-30 17:20:59.000000 trytond_account_dunning-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7515 2024-04-30 17:20:59.000000 trytond_account_dunning-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7250 2024-04-30 17:20:59.000000 trytond_account_dunning-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7437 2024-04-30 17:20:59.000000 trytond_account_dunning-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7344 2024-04-30 17:20:59.000000 trytond_account_dunning-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7234 2024-04-30 17:20:59.000000 trytond_account_dunning-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6493 2024-04-30 17:20:59.000000 trytond_account_dunning-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6998 2024-04-30 17:20:59.000000 trytond_account_dunning-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      386 2024-04-30 17:20:59.000000 trytond_account_dunning-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1197 2024-04-30 17:20:59.000000 trytond_account_dunning-7.2.1/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      454 2024-04-30 17:20:59.000000 trytond_account_dunning-7.2.1/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 12:24:26.604729 trytond_account_dunning-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4436 2024-04-30 17:20:59.000000 trytond_account_dunning-7.2.1/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:24:26.604729 trytond_account_dunning-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:20:59.000000 trytond_account_dunning-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8257 2024-04-30 17:20:59.000000 trytond_account_dunning-7.2.1/tests/scenario_account_dunning.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2950 2024-04-30 17:20:59.000000 trytond_account_dunning-7.2.1/tests/scenario_account_dunning_final.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      408 2024-04-30 17:20:59.000000 trytond_account_dunning-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:20:59.000000 trytond_account_dunning-7.2.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:20:59.000000 trytond_account_dunning-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      148 2024-04-30 17:21:06.000000 trytond_account_dunning-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:24:26.604729 trytond_account_dunning-7.2.1/trytond_account_dunning.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3597 2024-05-01 12:24:26.000000 trytond_account_dunning-7.2.1/trytond_account_dunning.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2300 2024-05-01 12:24:26.000000 trytond_account_dunning-7.2.1/trytond_account_dunning.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:24:26.000000 trytond_account_dunning-7.2.1/trytond_account_dunning.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       68 2024-05-01 12:24:26.000000 trytond_account_dunning-7.2.1/trytond_account_dunning.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:24:26.000000 trytond_account_dunning-7.2.1/trytond_account_dunning.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      136 2024-05-01 12:24:26.000000 trytond_account_dunning-7.2.1/trytond_account_dunning.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 12:24:26.000000 trytond_account_dunning-7.2.1/trytond_account_dunning.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:24:26.604729 trytond_account_dunning-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      424 2024-04-30 17:20:59.000000 trytond_account_dunning-7.2.1/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      405 2024-04-30 17:20:59.000000 trytond_account_dunning-7.2.1/view/dunning_create_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      808 2024-04-30 17:20:59.000000 trytond_account_dunning-7.2.1/view/dunning_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      378 2024-04-30 17:20:59.000000 trytond_account_dunning-7.2.1/view/dunning_level_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      266 2024-04-30 17:20:59.000000 trytond_account_dunning-7.2.1/view/dunning_level_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      286 2024-04-30 17:20:59.000000 trytond_account_dunning-7.2.1/view/dunning_level_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      548 2024-04-30 17:20:59.000000 trytond_account_dunning-7.2.1/view/dunning_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      343 2024-04-30 17:20:59.000000 trytond_account_dunning-7.2.1/view/dunning_procedure_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2024-04-30 17:20:59.000000 trytond_account_dunning-7.2.1/view/dunning_procedure_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      349 2024-04-30 17:20:59.000000 trytond_account_dunning-7.2.1/view/dunning_process_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      481 2024-04-30 17:20:59.000000 trytond_account_dunning-7.2.1/view/party_form.xml
```

### Comparing `trytond_account_dunning-7.2.0/CHANGELOG` & `trytond_account_dunning-7.2.1/CHANGELOG`

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

### Comparing `trytond_account_dunning-7.2.0/COPYRIGHT` & `trytond_account_dunning-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.2.0/LICENSE` & `trytond_account_dunning-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.2.0/PKG-INFO` & `trytond_account_dunning-7.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_account_dunning
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module for account dunning
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account_dunning-7.2.0/README.rst` & `trytond_account_dunning-7.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.2.0/__init__.py` & `trytond_account_dunning-7.2.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.2.0/account.py` & `trytond_account_dunning-7.2.1/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.2.0/account.xml` & `trytond_account_dunning-7.2.1/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.2.0/doc/conf.py` & `trytond_account_dunning-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.2.0/doc/index.rst` & `trytond_account_dunning-7.2.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.2.0/dunning.py` & `trytond_account_dunning-7.2.1/dunning.py`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.2.0/dunning.xml` & `trytond_account_dunning-7.2.1/dunning.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.2.0/locale/bg.po` & `trytond_account_dunning-7.2.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.2.0/locale/ca.po` & `trytond_account_dunning-7.2.1/locale/ca.po`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 msgctxt "field:account.dunning,amount:"
 msgid "Amount"
 msgstr "Import"
 
 msgctxt "field:account.dunning,amount_second_currency:"
 msgid "Amount Second Currency"
-msgstr "Import segona moneda"
+msgstr "Import moneda secundaria"
 
 msgctxt "field:account.dunning,blocked:"
 msgid "Blocked"
 msgstr "Bloquejada"
 
 msgctxt "field:account.dunning,company:"
 msgid "Company"
@@ -61,15 +61,15 @@
 
 msgctxt "field:account.dunning,procedure:"
 msgid "Procedure"
 msgstr "Procediment"
 
 msgctxt "field:account.dunning,second_currency:"
 msgid "Second Currency"
-msgstr "Segona moneda"
+msgstr "Moneda secundaria"
 
 msgctxt "field:account.dunning,state:"
 msgid "State"
 msgstr "Estat"
 
 msgctxt "field:account.dunning.create.start,date:"
 msgid "Date"
```

### Comparing `trytond_account_dunning-7.2.0/locale/cs.po` & `trytond_account_dunning-7.2.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.2.0/locale/de.po` & `trytond_account_dunning-7.2.1/locale/de.po`

 * *Files 0% similar despite different names*

```diff
@@ -224,15 +224,15 @@
 
 msgctxt "model:ir.model.button,string:dunning_reschedule_button"
 msgid "Reschedule"
 msgstr "Neu terminieren"
 
 msgctxt "model:ir.rule.group,name:rule_group_dunning_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.ui.menu,name:menu_dunning_configuration"
 msgid "Dunnings"
 msgstr "Mahnungen"
 
 msgctxt "model:ir.ui.menu,name:menu_dunning_create"
 msgid "Create Dunnings"
```

### Comparing `trytond_account_dunning-7.2.0/locale/es.po` & `trytond_account_dunning-7.2.1/locale/es.po`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 msgctxt "field:account.dunning,amount:"
 msgid "Amount"
 msgstr "Importe"
 
 msgctxt "field:account.dunning,amount_second_currency:"
 msgid "Amount Second Currency"
-msgstr "Importe segunda moneda"
+msgstr "Importe moneda secundaria"
 
 msgctxt "field:account.dunning,blocked:"
 msgid "Blocked"
 msgstr "Bloqueada"
 
 msgctxt "field:account.dunning,company:"
 msgid "Company"
```

### Comparing `trytond_account_dunning-7.2.0/locale/es_419.po` & `trytond_account_dunning-7.2.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.2.0/locale/et.po` & `trytond_account_dunning-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.2.0/locale/fa.po` & `trytond_account_dunning-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.2.0/locale/fi.po` & `trytond_account_dunning-7.2.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.2.0/locale/fr.po` & `trytond_account_dunning-7.2.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.2.0/locale/hu.po` & `trytond_account_dunning-7.2.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.2.0/locale/id.po` & `trytond_account_dunning-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.2.0/locale/it.po` & `trytond_account_dunning-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.2.0/locale/lo.po` & `trytond_account_dunning-7.2.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.2.0/locale/lt.po` & `trytond_account_dunning-7.2.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.2.0/locale/nl.po` & `trytond_account_dunning-7.2.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.2.0/locale/pl.po` & `trytond_account_dunning-7.2.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.2.0/locale/pt.po` & `trytond_account_dunning-7.2.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.2.0/locale/ro.po` & `trytond_account_dunning-7.2.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.2.0/locale/ru.po` & `trytond_account_dunning-7.2.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.2.0/locale/sl.po` & `trytond_account_dunning-7.2.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.2.0/locale/tr.po` & `trytond_account_dunning-7.2.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.2.0/locale/uk.po` & `trytond_account_dunning-7.2.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.2.0/locale/zh_CN.po` & `trytond_account_dunning-7.2.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.2.0/party.py` & `trytond_account_dunning-7.2.1/party.py`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.2.0/setup.py` & `trytond_account_dunning-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.2.0/tests/scenario_account_dunning.rst` & `trytond_account_dunning-7.2.1/tests/scenario_account_dunning.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.2.0/tests/scenario_account_dunning_final.rst` & `trytond_account_dunning-7.2.1/tests/scenario_account_dunning_final.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.2.0/tox.ini` & `trytond_account_dunning-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.2.0/trytond_account_dunning.egg-info/PKG-INFO` & `trytond_account_dunning-7.2.1/trytond_account_dunning.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_account_dunning
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module for account dunning
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account_dunning-7.2.0/trytond_account_dunning.egg-info/SOURCES.txt` & `trytond_account_dunning-7.2.1/trytond_account_dunning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.2.0/view/dunning_form.xml` & `trytond_account_dunning-7.2.1/view/dunning_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.2.0/view/dunning_list.xml` & `trytond_account_dunning-7.2.1/view/dunning_list.xml`

 * *Files identical despite different names*

