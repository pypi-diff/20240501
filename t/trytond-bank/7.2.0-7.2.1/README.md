# Comparing `tmp/trytond_bank-7.2.0.tar.gz` & `tmp/trytond_bank-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_bank-7.2.0.tar", last modified: Mon Apr 29 15:38:29 2024, max compression
+gzip compressed data, was "trytond_bank-7.2.1.tar", last modified: Wed May  1 12:04:16 2024, max compression
```

## Comparing `trytond_bank-7.2.0.tar` & `trytond_bank-7.2.1.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:38:29.219156 trytond_bank-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     2437 2024-04-29 15:18:15.000000 trytond_bank-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-04-29 15:18:14.000000 trytond_bank-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_bank-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_bank-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3206 2024-04-29 15:38:29.219156 trytond_bank-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      635 2023-01-16 14:00:20.000000 trytond_bank-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      475 2023-04-15 07:12:15.000000 trytond_bank-7.2.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10477 2024-03-17 11:01:36.000000 trytond_bank-7.2.0/bank.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5803 2024-04-27 16:30:39.000000 trytond_bank-7.2.0/bank.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:38:29.212489 trytond_bank-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3067 2024-04-27 16:30:39.000000 trytond_bank-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      635 2023-01-16 14:00:20.000000 trytond_bank-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:05.000000 trytond_bank-7.2.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      357 2023-04-15 07:12:15.000000 trytond_bank-7.2.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:38:29.212489 trytond_bank-7.2.0/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_bank-7.2.0/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      375 2023-01-16 14:00:20.000000 trytond_bank-7.2.0/icons/tryton-bank.svg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:38:29.215822 trytond_bank-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     3294 2024-04-27 16:43:22.000000 trytond_bank-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3503 2024-04-27 16:43:22.000000 trytond_bank-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3011 2024-04-27 16:43:22.000000 trytond_bank-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3518 2024-04-27 16:43:22.000000 trytond_bank-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3533 2024-04-27 16:43:22.000000 trytond_bank-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2942 2024-04-27 16:43:22.000000 trytond_bank-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3337 2024-04-27 16:43:22.000000 trytond_bank-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3675 2024-04-27 16:43:22.000000 trytond_bank-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3011 2024-04-27 16:43:22.000000 trytond_bank-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3553 2024-04-27 16:43:22.000000 trytond_bank-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3278 2024-04-27 16:43:22.000000 trytond_bank-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3108 2024-04-27 16:43:22.000000 trytond_bank-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3525 2024-04-27 16:43:22.000000 trytond_bank-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3904 2024-04-27 16:43:22.000000 trytond_bank-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3206 2024-04-27 16:43:22.000000 trytond_bank-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3513 2024-04-27 16:43:22.000000 trytond_bank-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3372 2024-04-27 16:43:22.000000 trytond_bank-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3498 2024-04-27 16:43:22.000000 trytond_bank-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3464 2024-04-27 16:43:22.000000 trytond_bank-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3278 2024-04-27 16:43:22.000000 trytond_bank-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3536 2024-04-27 16:43:22.000000 trytond_bank-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3011 2024-04-27 16:43:22.000000 trytond_bank-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2881 2024-04-27 16:43:22.000000 trytond_bank-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3026 2024-04-27 16:43:22.000000 trytond_bank-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1009 2023-04-15 07:12:15.000000 trytond_bank-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1530 2024-01-27 09:58:52.000000 trytond_bank-7.2.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1354 2024-04-27 16:30:39.000000 trytond_bank-7.2.0/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:38:29.219156 trytond_bank-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4361 2024-03-17 11:01:36.000000 trytond_bank-7.2.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:38:29.215822 trytond_bank-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_bank-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7283 2023-04-15 07:12:15.000000 trytond_bank-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:05.000000 trytond_bank-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      110 2024-04-29 15:18:10.000000 trytond_bank-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:38:29.219156 trytond_bank-7.2.0/trytond_bank.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3206 2024-04-29 15:38:28.000000 trytond_bank-7.2.0/trytond_bank.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1847 2024-04-29 15:38:29.000000 trytond_bank-7.2.0/trytond_bank.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:38:28.000000 trytond_bank-7.2.0/trytond_bank.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2024-04-29 15:38:28.000000 trytond_bank-7.2.0/trytond_bank.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:59.000000 trytond_bank-7.2.0/trytond_bank.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      145 2024-04-29 15:38:28.000000 trytond_bank-7.2.0/trytond_bank.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:38:28.000000 trytond_bank-7.2.0/trytond_bank.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:38:29.219156 trytond_bank-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      515 2023-01-16 14:00:20.000000 trytond_bank-7.2.0/view/bank_account_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      333 2023-04-15 07:12:15.000000 trytond_bank-7.2.0/view/bank_account_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      576 2024-01-27 09:58:52.000000 trytond_bank-7.2.0/view/bank_account_number_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      288 2023-04-15 07:12:15.000000 trytond_bank-7.2.0/view/bank_account_number_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      308 2023-04-15 07:12:15.000000 trytond_bank-7.2.0/view/bank_account_number_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      286 2023-01-16 14:00:20.000000 trytond_bank-7.2.0/view/bank_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      258 2023-04-15 07:12:15.000000 trytond_bank-7.2.0/view/bank_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      384 2023-01-16 14:00:20.000000 trytond_bank-7.2.0/view/party_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:04:16.692556 trytond_bank-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2538 2024-05-01 12:04:13.000000 trytond_bank-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-05-01 12:04:13.000000 trytond_bank-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:20:59.000000 trytond_bank-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:20:59.000000 trytond_bank-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3206 2024-05-01 12:04:16.692556 trytond_bank-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      635 2024-04-30 17:20:59.000000 trytond_bank-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      475 2024-04-30 17:20:59.000000 trytond_bank-7.2.1/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10477 2024-04-30 17:20:59.000000 trytond_bank-7.2.1/bank.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5803 2024-04-30 17:20:59.000000 trytond_bank-7.2.1/bank.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:04:16.689222 trytond_bank-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3067 2024-04-30 17:20:59.000000 trytond_bank-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      635 2024-04-30 17:20:59.000000 trytond_bank-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:20:59.000000 trytond_bank-7.2.1/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      357 2024-04-30 17:20:59.000000 trytond_bank-7.2.1/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:04:16.689222 trytond_bank-7.2.1/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2024-04-30 17:20:59.000000 trytond_bank-7.2.1/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      375 2024-04-30 17:20:59.000000 trytond_bank-7.2.1/icons/tryton-bank.svg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:04:16.689222 trytond_bank-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3294 2024-04-30 17:20:59.000000 trytond_bank-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3503 2024-04-30 17:20:59.000000 trytond_bank-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3011 2024-04-30 17:20:59.000000 trytond_bank-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3514 2024-04-30 17:21:59.000000 trytond_bank-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3533 2024-04-30 17:20:59.000000 trytond_bank-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2942 2024-04-30 17:20:59.000000 trytond_bank-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3337 2024-04-30 17:20:59.000000 trytond_bank-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3675 2024-04-30 17:20:59.000000 trytond_bank-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3011 2024-04-30 17:20:59.000000 trytond_bank-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3553 2024-04-30 17:20:59.000000 trytond_bank-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3278 2024-04-30 17:20:59.000000 trytond_bank-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3108 2024-04-30 17:20:59.000000 trytond_bank-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3525 2024-04-30 17:20:59.000000 trytond_bank-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3904 2024-04-30 17:20:59.000000 trytond_bank-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3206 2024-04-30 17:20:59.000000 trytond_bank-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3513 2024-04-30 17:20:59.000000 trytond_bank-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3492 2024-04-30 17:21:59.000000 trytond_bank-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3498 2024-04-30 17:20:59.000000 trytond_bank-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3464 2024-04-30 17:20:59.000000 trytond_bank-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3278 2024-04-30 17:20:59.000000 trytond_bank-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3536 2024-04-30 17:20:59.000000 trytond_bank-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3011 2024-04-30 17:20:59.000000 trytond_bank-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2881 2024-04-30 17:20:59.000000 trytond_bank-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3026 2024-04-30 17:20:59.000000 trytond_bank-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1009 2024-04-30 17:20:59.000000 trytond_bank-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1530 2024-04-30 17:20:59.000000 trytond_bank-7.2.1/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1354 2024-04-30 17:20:59.000000 trytond_bank-7.2.1/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 12:04:16.692556 trytond_bank-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4361 2024-04-30 17:20:59.000000 trytond_bank-7.2.1/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:04:16.689222 trytond_bank-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:20:59.000000 trytond_bank-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7283 2024-04-30 17:20:59.000000 trytond_bank-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:20:59.000000 trytond_bank-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      110 2024-04-30 17:21:06.000000 trytond_bank-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:04:16.692556 trytond_bank-7.2.1/trytond_bank.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3206 2024-05-01 12:04:16.000000 trytond_bank-7.2.1/trytond_bank.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1847 2024-05-01 12:04:16.000000 trytond_bank-7.2.1/trytond_bank.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:04:16.000000 trytond_bank-7.2.1/trytond_bank.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       46 2024-05-01 12:04:16.000000 trytond_bank-7.2.1/trytond_bank.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:04:16.000000 trytond_bank-7.2.1/trytond_bank.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      145 2024-05-01 12:04:16.000000 trytond_bank-7.2.1/trytond_bank.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 12:04:16.000000 trytond_bank-7.2.1/trytond_bank.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:04:16.692556 trytond_bank-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      515 2024-04-30 17:20:59.000000 trytond_bank-7.2.1/view/bank_account_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      333 2024-04-30 17:20:59.000000 trytond_bank-7.2.1/view/bank_account_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      576 2024-04-30 17:20:59.000000 trytond_bank-7.2.1/view/bank_account_number_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      288 2024-04-30 17:20:59.000000 trytond_bank-7.2.1/view/bank_account_number_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      308 2024-04-30 17:20:59.000000 trytond_bank-7.2.1/view/bank_account_number_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      286 2024-04-30 17:20:59.000000 trytond_bank-7.2.1/view/bank_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      258 2024-04-30 17:20:59.000000 trytond_bank-7.2.1/view/bank_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      384 2024-04-30 17:20:59.000000 trytond_bank-7.2.1/view/party_form.xml
```

### Comparing `trytond_bank-7.2.0/CHANGELOG` & `trytond_bank-7.2.1/CHANGELOG`

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

### Comparing `trytond_bank-7.2.0/COPYRIGHT` & `trytond_bank-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.2.0/LICENSE` & `trytond_bank-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.2.0/PKG-INFO` & `trytond_bank-7.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_bank
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module with banks
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_bank-7.2.0/README.rst` & `trytond_bank-7.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.2.0/bank.py` & `trytond_bank-7.2.1/bank.py`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.2.0/bank.xml` & `trytond_bank-7.2.1/bank.xml`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.2.0/doc/conf.py` & `trytond_bank-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.2.0/doc/index.rst` & `trytond_bank-7.2.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.2.0/icons/LICENSE` & `trytond_bank-7.2.1/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.2.0/locale/bg.po` & `trytond_bank-7.2.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.2.0/locale/ca.po` & `trytond_bank-7.2.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.2.0/locale/cs.po` & `trytond_bank-7.2.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.2.0/locale/de.po` & `trytond_bank-7.2.1/locale/de.po`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,15 @@
 
 msgctxt "model:ir.message,text:msg_account_iban_unique"
 msgid "Account can have only one IBAN."
 msgstr "Für das Bankkonto kann nur eine IBAN erfasst werden."
 
 msgctxt "model:ir.message,text:msg_invalid_bic"
 msgid "The BIC \"%(bic)s\" is not valid."
-msgstr "Die IBAN \"%(number)s\" ist ungültig."
+msgstr "Die BIC \"%(bic)s\" ist ungültig."
 
 msgctxt "model:ir.message,text:msg_invalid_iban"
 msgid "IBAN \"%(number)s\" is not valid."
 msgstr "Die IBAN \"%(number)s\" ist ungültig."
 
 msgctxt "model:ir.message,text:msg_number_iban_unique"
 msgid "IBAN must be unique."
```

### Comparing `trytond_bank-7.2.0/locale/es.po` & `trytond_bank-7.2.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.2.0/locale/es_419.po` & `trytond_bank-7.2.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.2.0/locale/et.po` & `trytond_bank-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.2.0/locale/fa.po` & `trytond_bank-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.2.0/locale/fi.po` & `trytond_bank-7.2.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.2.0/locale/fr.po` & `trytond_bank-7.2.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.2.0/locale/hu.po` & `trytond_bank-7.2.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.2.0/locale/id.po` & `trytond_bank-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.2.0/locale/it.po` & `trytond_bank-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.2.0/locale/lo.po` & `trytond_bank-7.2.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.2.0/locale/lt.po` & `trytond_bank-7.2.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.2.0/locale/nl.po` & `trytond_bank-7.2.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.2.0/locale/pl.po` & `trytond_bank-7.2.1/locale/ro.po`

 * *Files 8% similar despite different names*

```diff
@@ -4,145 +4,144 @@
 
 msgctxt "field:bank,bic:"
 msgid "BIC"
 msgstr "BIC"
 
 msgctxt "field:bank,party:"
 msgid "Party"
-msgstr "Strona"
+msgstr "Parte"
 
 msgctxt "field:bank.account,bank:"
 msgid "Bank"
-msgstr "Bank"
+msgstr "Banca"
 
 msgctxt "field:bank.account,currency:"
 msgid "Currency"
-msgstr "Waluta"
+msgstr "Moneda"
 
 msgctxt "field:bank.account,numbers:"
 msgid "Numbers"
-msgstr "Numery kont"
+msgstr "Numere"
 
 msgctxt "field:bank.account,owners:"
 msgid "Owners"
-msgstr "Właściciele"
+msgstr "Proprietari"
 
 msgctxt "field:bank.account-party.party,account:"
 msgid "Account"
-msgstr "Konto"
+msgstr "Cont"
 
 msgctxt "field:bank.account-party.party,owner:"
 msgid "Owner"
-msgstr "Właściciel"
+msgstr "Proprietar"
 
 msgctxt "field:bank.account.number,account:"
 msgid "Account"
-msgstr "Konto"
+msgstr "Cont"
 
 msgctxt "field:bank.account.number,number:"
 msgid "Number"
-msgstr "Numer"
+msgstr "Număr"
 
 msgctxt "field:bank.account.number,number_compact:"
 msgid "Number Compact"
-msgstr "Numer kompaktowy"
+msgstr "Număr Compact"
 
 msgctxt "field:bank.account.number,type:"
 msgid "Type"
-msgstr "Typ"
+msgstr "Tip"
 
 msgctxt "field:party.party,bank_accounts:"
 msgid "Bank Accounts"
-msgstr "Konta bankowe"
+msgstr "Conturi Bancare"
 
 msgctxt "help:bank,bic:"
 msgid "Bank/Business Identifier Code."
-msgstr "Bankowy/biznesowy kod identyfikacyjny."
+msgstr "Banca/Cod Identificare Companie."
 
 msgctxt "help:bank.account,bank:"
 msgid "The bank where the account is open."
-msgstr "Bank, w którym otworzono konto."
+msgstr "Banca la care este deschis contul."
 
 msgctxt "help:bank.account,numbers:"
 msgid "Add the numbers which identify the bank account."
-msgstr "Dodaj cyfry identyfikujące konto w banku."
+msgstr "Adăugaţi numerele care identifică contul bancar."
 
 msgctxt "help:bank.account.number,account:"
 msgid "The bank account which is identified by the number."
-msgstr "Konto bankowe identyfikowane przez numer."
+msgstr "Contul bancar care este identificat de numărul."
 
 msgctxt "model:bank,name:"
 msgid "Bank"
-msgstr "Bank"
+msgstr "Banca"
 
 msgctxt "model:bank.account,name:"
 msgid "Bank Account"
-msgstr "Konto bankowe"
+msgstr "Cont Bancar"
 
 msgctxt "model:bank.account-party.party,name:"
 msgid "Bank Account - Party"
-msgstr "Konto bankowe - Strona"
+msgstr "Cont Bancar - Parte"
 
 msgctxt "model:bank.account.number,name:"
 msgid "Bank Account Number"
-msgstr "Numer konta bankowego"
+msgstr "Cont Bancar"
 
 msgctxt "model:ir.action,name:act_bank_account_form"
 msgid "Accounts"
-msgstr "Konta"
+msgstr "Conturi"
 
 msgctxt "model:ir.action,name:act_bank_form"
 msgid "Banks"
-msgstr "Banki"
+msgstr "Bănci"
 
 msgctxt "model:ir.message,text:msg_account_iban_invalid_bic"
 msgid "The BIC of \"%(account)s\" is not valid with the \"%(bic)s\" from IBAN."
-msgstr ""
+msgstr "BIC-ul contului \"%(account)s\" nu corespunde cu \"%(bic)s\"-ul de la IBAN."
 
 msgctxt "model:ir.message,text:msg_account_iban_unique"
 msgid "Account can have only one IBAN."
-msgstr ""
+msgstr "Contul poate avea un singur IBAN."
 
 msgctxt "model:ir.message,text:msg_invalid_bic"
 msgid "The BIC \"%(bic)s\" is not valid."
-msgstr "Kod BIC \"%(bic)s\" jest niepoprawny."
+msgstr "Codul BIC \"%(bic)s\" nu este valid."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_invalid_iban"
 msgid "IBAN \"%(number)s\" is not valid."
-msgstr "Numer IBAN \"%(number)s\" jest niepoprawny."
+msgstr "Codul IBAN \"%(number)s\" nu este valid."
 
 msgctxt "model:ir.message,text:msg_number_iban_unique"
 msgid "IBAN must be unique."
-msgstr ""
+msgstr "IBAN-ul trebuie să fie unic."
 
 msgctxt "model:ir.ui.menu,name:menu_bank_account_form"
 msgid "Accounts"
-msgstr "Konta"
+msgstr "Conturi"
 
 msgctxt "model:ir.ui.menu,name:menu_bank_form"
 msgid "Banks"
-msgstr "Banki"
+msgstr "Bănci"
 
 msgctxt "model:ir.ui.menu,name:menu_banking"
 msgid "Banking"
-msgstr "Bankowość"
+msgstr "Bancar"
 
 msgctxt "model:res.group,name:group_bank_admin"
 msgid "Bank Administration"
-msgstr "Administracja ustawieniami banku"
+msgstr "Gestiune Bănci"
 
 msgctxt "selection:bank.account.number,type:"
 msgid "IBAN"
 msgstr "IBAN"
 
 msgctxt "selection:bank.account.number,type:"
 msgid "Other"
-msgstr "Inne"
+msgstr "Alte"
 
 msgctxt "view:bank.account:"
 msgid "Number"
-msgstr "Numer"
+msgstr "Număr"
 
 msgctxt "view:party.party:"
 msgid "Banking"
-msgstr "Bankowość"
+msgstr "Bancar"
```

### Comparing `trytond_bank-7.2.0/locale/pt.po` & `trytond_bank-7.2.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.2.0/locale/ro.po` & `trytond_bank-7.2.1/locale/pl.po`

 * *Files 8% similar despite different names*

```diff
@@ -4,144 +4,144 @@
 
 msgctxt "field:bank,bic:"
 msgid "BIC"
 msgstr "BIC"
 
 msgctxt "field:bank,party:"
 msgid "Party"
-msgstr "Parte"
+msgstr "Strona"
 
 msgctxt "field:bank.account,bank:"
 msgid "Bank"
-msgstr "Banca"
+msgstr "Bank"
 
 msgctxt "field:bank.account,currency:"
 msgid "Currency"
-msgstr "Moneda"
+msgstr "Waluta"
 
 msgctxt "field:bank.account,numbers:"
 msgid "Numbers"
-msgstr "Numere"
+msgstr "Numery kont"
 
 msgctxt "field:bank.account,owners:"
 msgid "Owners"
-msgstr "Proprietari"
+msgstr "Właściciele"
 
 msgctxt "field:bank.account-party.party,account:"
 msgid "Account"
-msgstr "Cont"
+msgstr "Konto"
 
 msgctxt "field:bank.account-party.party,owner:"
 msgid "Owner"
-msgstr "Proprietar"
+msgstr "Właściciel"
 
 msgctxt "field:bank.account.number,account:"
 msgid "Account"
-msgstr "Cont"
+msgstr "Konto"
 
 msgctxt "field:bank.account.number,number:"
 msgid "Number"
-msgstr "Număr"
+msgstr "Numer"
 
 msgctxt "field:bank.account.number,number_compact:"
 msgid "Number Compact"
-msgstr "Număr Compact"
+msgstr "Numer kompaktowy"
 
 msgctxt "field:bank.account.number,type:"
 msgid "Type"
-msgstr "Tip"
+msgstr "Typ"
 
 msgctxt "field:party.party,bank_accounts:"
 msgid "Bank Accounts"
-msgstr "Conturi Bancare"
+msgstr "Konta bankowe"
 
 msgctxt "help:bank,bic:"
 msgid "Bank/Business Identifier Code."
-msgstr "Banca/Cod Identificare Companie."
+msgstr "Bankowy/biznesowy kod identyfikacyjny."
 
 msgctxt "help:bank.account,bank:"
 msgid "The bank where the account is open."
-msgstr "Banca la care este deschis contul."
+msgstr "Bank, w którym otworzono konto."
 
 msgctxt "help:bank.account,numbers:"
 msgid "Add the numbers which identify the bank account."
-msgstr "Adăugaţi numerele care identifică contul bancar."
+msgstr "Dodaj cyfry identyfikujące konto w banku."
 
 msgctxt "help:bank.account.number,account:"
 msgid "The bank account which is identified by the number."
-msgstr "Contul bancar care este identificat de numărul."
+msgstr "Konto bankowe identyfikowane przez numer."
 
 msgctxt "model:bank,name:"
 msgid "Bank"
-msgstr "Banca"
+msgstr "Bank"
 
 msgctxt "model:bank.account,name:"
 msgid "Bank Account"
-msgstr "Cont Bancar"
+msgstr "Konto bankowe"
 
 msgctxt "model:bank.account-party.party,name:"
 msgid "Bank Account - Party"
-msgstr "Cont Bancar - Parte"
+msgstr "Konto bankowe - Strona"
 
 msgctxt "model:bank.account.number,name:"
 msgid "Bank Account Number"
-msgstr "Cont Bancar"
+msgstr "Numer konta bankowego"
 
 msgctxt "model:ir.action,name:act_bank_account_form"
 msgid "Accounts"
-msgstr "Conturi"
+msgstr "Konta"
 
 msgctxt "model:ir.action,name:act_bank_form"
 msgid "Banks"
-msgstr "Bănci"
+msgstr "Banki"
 
 msgctxt "model:ir.message,text:msg_account_iban_invalid_bic"
 msgid "The BIC of \"%(account)s\" is not valid with the \"%(bic)s\" from IBAN."
-msgstr "BIC-ul contului \"%(account)s\" nu corespunde cu \"%(bic)s\"-ul de la IBAN."
+msgstr "BIC \"%(account)s\" nie jest ważny z \"%(bic)s\" z IBAN."
 
 msgctxt "model:ir.message,text:msg_account_iban_unique"
 msgid "Account can have only one IBAN."
-msgstr "Contul poate avea un singur IBAN."
+msgstr "Konto może mieć tylko jeden numer IBAN."
 
 msgctxt "model:ir.message,text:msg_invalid_bic"
 msgid "The BIC \"%(bic)s\" is not valid."
-msgstr "Codul BIC \"%(bic)s\" nu este valid."
+msgstr "Kod BIC \"%(bic)s\" jest niepoprawny."
 
 msgctxt "model:ir.message,text:msg_invalid_iban"
 msgid "IBAN \"%(number)s\" is not valid."
-msgstr "Codul IBAN \"%(number)s\" nu este valid."
+msgstr "Numer IBAN \"%(number)s\" jest niepoprawny."
 
 msgctxt "model:ir.message,text:msg_number_iban_unique"
 msgid "IBAN must be unique."
-msgstr "IBAN-ul trebuie să fie unic."
+msgstr "Numer IBAN musi być unikatowy."
 
 msgctxt "model:ir.ui.menu,name:menu_bank_account_form"
 msgid "Accounts"
-msgstr "Conturi"
+msgstr "Konta"
 
 msgctxt "model:ir.ui.menu,name:menu_bank_form"
 msgid "Banks"
-msgstr "Bănci"
+msgstr "Banki"
 
 msgctxt "model:ir.ui.menu,name:menu_banking"
 msgid "Banking"
-msgstr "Bancar"
+msgstr "Bankowość"
 
 msgctxt "model:res.group,name:group_bank_admin"
 msgid "Bank Administration"
-msgstr "Gestiune Bănci"
+msgstr "Administracja ustawieniami banku"
 
 msgctxt "selection:bank.account.number,type:"
 msgid "IBAN"
 msgstr "IBAN"
 
 msgctxt "selection:bank.account.number,type:"
 msgid "Other"
-msgstr "Alte"
+msgstr "Inne"
 
 msgctxt "view:bank.account:"
 msgid "Number"
-msgstr "Număr"
+msgstr "Numer"
 
 msgctxt "view:party.party:"
 msgid "Banking"
-msgstr "Bancar"
+msgstr "Bankowość"
```

### Comparing `trytond_bank-7.2.0/locale/ru.po` & `trytond_bank-7.2.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.2.0/locale/sl.po` & `trytond_bank-7.2.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.2.0/locale/tr.po` & `trytond_bank-7.2.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.2.0/locale/uk.po` & `trytond_bank-7.2.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.2.0/locale/zh_CN.po` & `trytond_bank-7.2.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.2.0/message.xml` & `trytond_bank-7.2.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.2.0/party.py` & `trytond_bank-7.2.1/party.py`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.2.0/party.xml` & `trytond_bank-7.2.1/party.xml`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.2.0/setup.py` & `trytond_bank-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.2.0/tests/test_module.py` & `trytond_bank-7.2.1/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.2.0/tox.ini` & `trytond_bank-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.2.0/trytond_bank.egg-info/PKG-INFO` & `trytond_bank-7.2.1/trytond_bank.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_bank
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module with banks
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_bank-7.2.0/trytond_bank.egg-info/SOURCES.txt` & `trytond_bank-7.2.1/trytond_bank.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.2.0/view/bank_account_form.xml` & `trytond_bank-7.2.1/view/bank_account_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.2.0/view/bank_account_number_form.xml` & `trytond_bank-7.2.1/view/bank_account_number_form.xml`

 * *Files identical despite different names*

