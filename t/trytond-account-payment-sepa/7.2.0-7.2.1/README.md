# Comparing `tmp/trytond_account_payment_sepa-7.2.0.tar.gz` & `tmp/trytond_account_payment_sepa-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_payment_sepa-7.2.0.tar", last modified: Mon Apr 29 15:35:01 2024, max compression
+gzip compressed data, was "trytond_account_payment_sepa-7.2.1.tar", last modified: Wed May  1 12:20:05 2024, max compression
```

## Comparing `trytond_account_payment_sepa-7.2.0.tar` & `trytond_account_payment_sepa-7.2.1.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:01.204596 trytond_account_payment_sepa-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     2919 2024-04-29 15:15:19.000000 trytond_account_payment_sepa-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-04-29 15:15:18.000000 trytond_account_payment_sepa-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_payment_sepa-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     4558 2024-04-29 15:35:01.204596 trytond_account_payment_sepa-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1915 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      803 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.2.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1256 2024-01-27 09:58:52.000000 trytond_account_payment_sepa-7.2.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1056 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.2.0/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:01.197930 trytond_account_payment_sepa-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3083 2024-04-27 16:30:39.000000 trytond_account_payment_sepa-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1915 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:36:57.000000 trytond_account_payment_sepa-7.2.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      240 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.2.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:01.201263 trytond_account_payment_sepa-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    14910 2024-04-27 16:43:21.000000 trytond_account_payment_sepa-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16985 2024-04-27 16:43:21.000000 trytond_account_payment_sepa-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14377 2024-04-27 16:43:21.000000 trytond_account_payment_sepa-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17220 2024-04-27 16:43:21.000000 trytond_account_payment_sepa-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16868 2024-04-27 16:43:21.000000 trytond_account_payment_sepa-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13739 2024-04-27 16:43:21.000000 trytond_account_payment_sepa-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16064 2024-04-27 16:43:21.000000 trytond_account_payment_sepa-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17244 2024-04-27 16:43:21.000000 trytond_account_payment_sepa-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14360 2024-04-27 16:43:21.000000 trytond_account_payment_sepa-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17008 2024-04-27 16:43:21.000000 trytond_account_payment_sepa-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14691 2024-04-27 16:43:21.000000 trytond_account_payment_sepa-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14237 2024-04-27 16:43:21.000000 trytond_account_payment_sepa-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16454 2024-04-27 16:43:21.000000 trytond_account_payment_sepa-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15217 2024-04-27 16:43:21.000000 trytond_account_payment_sepa-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14491 2024-04-27 16:43:21.000000 trytond_account_payment_sepa-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16936 2024-04-27 16:43:21.000000 trytond_account_payment_sepa-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14648 2024-04-27 16:43:21.000000 trytond_account_payment_sepa-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16059 2024-04-27 16:43:21.000000 trytond_account_payment_sepa-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13893 2024-04-29 13:17:17.000000 trytond_account_payment_sepa-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14999 2024-04-27 16:43:21.000000 trytond_account_payment_sepa-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15931 2024-04-27 16:43:21.000000 trytond_account_payment_sepa-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14360 2024-04-27 16:43:21.000000 trytond_account_payment_sepa-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13739 2024-04-27 16:43:21.000000 trytond_account_payment_sepa-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14512 2024-04-27 16:43:21.000000 trytond_account_payment_sepa-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)    81526 2024-04-29 13:17:17.000000 trytond_account_payment_sepa-7.2.0/mandate.fodt
--rw-r--r--   0 ced       (1000) ced       (1000)     1891 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3817 2024-02-04 18:51:26.000000 trytond_account_payment_sepa-7.2.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2048 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.2.0/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    33864 2024-03-17 11:01:36.000000 trytond_account_payment_sepa-7.2.0/payment.py
--rw-r--r--   0 ced       (1000) ced       (1000)    14944 2024-04-27 16:30:39.000000 trytond_account_payment_sepa-7.2.0/payment.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4236 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.2.0/sepa_handler.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:35:01.204596 trytond_account_payment_sepa-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4585 2024-03-17 11:01:36.000000 trytond_account_payment_sepa-7.2.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:01.201263 trytond_account_payment_sepa-7.2.0/template/
--rw-r--r--   0 ced       (1000) ced       (1000)     4112 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.2.0/template/base.003.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4330 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.2.0/template/base.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4970 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.2.0/template/pain.001.001.03.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4356 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.2.0/template/pain.001.001.05.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3590 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.2.0/template/pain.001.003.03.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     5513 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.2.0/template/pain.008.001.02.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4824 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.2.0/template/pain.008.001.04.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4286 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.2.0/template/pain.008.003.02.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:01.201263 trytond_account_payment_sepa-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      213 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1543 2023-01-16 14:00:20.000000 trytond_account_payment_sepa-7.2.0/tests/camt.054.001.01.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    54208 2024-02-04 18:51:26.000000 trytond_account_payment_sepa-7.2.0/tests/camt.054.001.01.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     1394 2023-01-16 14:00:20.000000 trytond_account_payment_sepa-7.2.0/tests/camt.054.001.02.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    63527 2024-02-04 18:51:26.000000 trytond_account_payment_sepa-7.2.0/tests/camt.054.001.02.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     2090 2023-01-16 14:00:20.000000 trytond_account_payment_sepa-7.2.0/tests/camt.054.001.03.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    88220 2024-02-04 18:51:26.000000 trytond_account_payment_sepa-7.2.0/tests/camt.054.001.03.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     2159 2023-01-16 14:00:20.000000 trytond_account_payment_sepa-7.2.0/tests/camt.054.001.04.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    87039 2024-02-04 18:51:26.000000 trytond_account_payment_sepa-7.2.0/tests/camt.054.001.04.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)    45054 2024-02-04 18:51:26.000000 trytond_account_payment_sepa-7.2.0/tests/pain.001.001.03.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)    46028 2024-02-04 18:51:26.000000 trytond_account_payment_sepa-7.2.0/tests/pain.001.001.05.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)    19631 2024-02-04 18:51:26.000000 trytond_account_payment_sepa-7.2.0/tests/pain.001.003.03.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)    43289 2024-02-04 18:51:26.000000 trytond_account_payment_sepa-7.2.0/tests/pain.008.001.02.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)    44237 2024-02-04 18:51:26.000000 trytond_account_payment_sepa-7.2.0/tests/pain.008.001.04.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)    26052 2024-02-04 18:51:26.000000 trytond_account_payment_sepa-7.2.0/tests/pain.008.003.02.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)    15710 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:36:57.000000 trytond_account_payment_sepa-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      201 2024-04-29 15:15:14.000000 trytond_account_payment_sepa-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:01.204596 trytond_account_payment_sepa-7.2.0/trytond_account_payment_sepa.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     4558 2024-04-29 15:35:00.000000 trytond_account_payment_sepa-7.2.0/trytond_account_payment_sepa.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     3425 2024-04-29 15:35:01.000000 trytond_account_payment_sepa-7.2.0/trytond_account_payment_sepa.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:35:00.000000 trytond_account_payment_sepa-7.2.0/trytond_account_payment_sepa.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       78 2024-04-29 15:35:00.000000 trytond_account_payment_sepa-7.2.0/trytond_account_payment_sepa.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:04.000000 trytond_account_payment_sepa-7.2.0/trytond_account_payment_sepa.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      180 2024-04-29 15:35:00.000000 trytond_account_payment_sepa-7.2.0/trytond_account_payment_sepa.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:35:00.000000 trytond_account_payment_sepa-7.2.0/trytond_account_payment_sepa.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:01.204596 trytond_account_payment_sepa-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      418 2023-01-16 14:00:20.000000 trytond_account_payment_sepa-7.2.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1044 2023-01-16 14:00:20.000000 trytond_account_payment_sepa-7.2.0/view/mandate_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      366 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.2.0/view/mandate_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      788 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.2.0/view/message_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      401 2023-01-16 14:00:20.000000 trytond_account_payment_sepa-7.2.0/view/message_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      335 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.2.0/view/party_identifier_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      354 2024-03-08 19:04:12.000000 trytond_account_payment_sepa-7.2.0/view/party_reception_direct_debit_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      776 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.2.0/view/payment_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      446 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.2.0/view/payment_group_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      317 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.2.0/view/payment_group_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1027 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.2.0/view/payment_journal_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      323 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.2.0/view/payment_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:20:05.258231 trytond_account_payment_sepa-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3020 2024-05-01 12:20:02.000000 trytond_account_payment_sepa-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-05-01 12:20:01.000000 trytond_account_payment_sepa-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     4558 2024-05-01 12:20:05.258231 trytond_account_payment_sepa-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1915 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      803 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1256 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1056 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:20:05.251565 trytond_account_payment_sepa-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3083 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1915 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      240 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:20:05.254898 trytond_account_payment_sepa-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    14910 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16985 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14377 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17247 2024-04-30 17:21:59.000000 trytond_account_payment_sepa-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16868 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13739 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16064 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17244 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14360 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17008 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14691 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14237 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16454 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15217 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14491 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16936 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14648 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16059 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13893 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14999 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15931 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14360 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13739 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14512 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    81526 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/mandate.fodt
+-rw-r--r--   0 ced       (1000) ced       (1000)     1891 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3817 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2048 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    33864 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/payment.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    14944 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/payment.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4236 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/sepa_handler.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 12:20:05.258231 trytond_account_payment_sepa-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4585 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:20:05.254898 trytond_account_payment_sepa-7.2.1/template/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4112 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/template/base.003.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4330 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/template/base.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4970 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/template/pain.001.001.03.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4356 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/template/pain.001.001.05.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3590 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/template/pain.001.003.03.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     5513 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/template/pain.008.001.02.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4824 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/template/pain.008.001.04.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4286 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/template/pain.008.003.02.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:20:05.258231 trytond_account_payment_sepa-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      213 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1543 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/tests/camt.054.001.01.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    54208 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/tests/camt.054.001.01.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     1394 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/tests/camt.054.001.02.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    63527 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/tests/camt.054.001.02.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     2090 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/tests/camt.054.001.03.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    88220 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/tests/camt.054.001.03.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     2159 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/tests/camt.054.001.04.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    87039 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/tests/camt.054.001.04.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)    45054 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/tests/pain.001.001.03.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)    46028 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/tests/pain.001.001.05.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)    19631 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/tests/pain.001.003.03.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)    43289 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/tests/pain.008.001.02.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)    44237 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/tests/pain.008.001.04.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)    26052 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/tests/pain.008.003.02.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)    15710 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      201 2024-04-30 17:21:06.000000 trytond_account_payment_sepa-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:20:05.258231 trytond_account_payment_sepa-7.2.1/trytond_account_payment_sepa.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4558 2024-05-01 12:20:04.000000 trytond_account_payment_sepa-7.2.1/trytond_account_payment_sepa.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     3425 2024-05-01 12:20:05.000000 trytond_account_payment_sepa-7.2.1/trytond_account_payment_sepa.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:20:04.000000 trytond_account_payment_sepa-7.2.1/trytond_account_payment_sepa.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       78 2024-05-01 12:20:04.000000 trytond_account_payment_sepa-7.2.1/trytond_account_payment_sepa.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:20:04.000000 trytond_account_payment_sepa-7.2.1/trytond_account_payment_sepa.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      180 2024-05-01 12:20:04.000000 trytond_account_payment_sepa-7.2.1/trytond_account_payment_sepa.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 12:20:04.000000 trytond_account_payment_sepa-7.2.1/trytond_account_payment_sepa.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:20:05.258231 trytond_account_payment_sepa-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      418 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1044 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/view/mandate_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      366 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/view/mandate_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      788 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/view/message_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      401 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/view/message_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      335 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/view/party_identifier_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      354 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/view/party_reception_direct_debit_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      776 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/view/payment_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      446 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/view/payment_group_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      317 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/view/payment_group_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1027 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/view/payment_journal_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      323 2024-04-30 17:20:59.000000 trytond_account_payment_sepa-7.2.1/view/payment_list.xml
```

### Comparing `trytond_account_payment_sepa-7.2.0/CHANGELOG` & `trytond_account_payment_sepa-7.2.1/CHANGELOG`

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

### Comparing `trytond_account_payment_sepa-7.2.0/COPYRIGHT` & `trytond_account_payment_sepa-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/LICENSE` & `trytond_account_payment_sepa-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/PKG-INFO` & `trytond_account_payment_sepa-7.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_account_payment_sepa
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module for SEPA payment
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account_payment_sepa-7.2.0/README.rst` & `trytond_account_payment_sepa-7.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/__init__.py` & `trytond_account_payment_sepa-7.2.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/account.py` & `trytond_account_payment_sepa-7.2.1/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/account.xml` & `trytond_account_payment_sepa-7.2.1/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/doc/conf.py` & `trytond_account_payment_sepa-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/doc/index.rst` & `trytond_account_payment_sepa-7.2.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/locale/bg.po` & `trytond_account_payment_sepa-7.2.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/locale/ca.po` & `trytond_account_payment_sepa-7.2.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/locale/cs.po` & `trytond_account_payment_sepa-7.2.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/locale/de.po` & `trytond_account_payment_sepa-7.2.1/locale/de.po`

 * *Files 2% similar despite different names*

```diff
@@ -65,27 +65,27 @@
 
 msgctxt "field:account.payment.journal,sepa_charge_bearer:"
 msgid "Charge Bearer"
 msgstr "Gebührenträger"
 
 msgctxt "field:account.payment.journal,sepa_payable_flavor:"
 msgid "Payable Flavor"
-msgstr "SEPA-Typ Verbindlichkeiten"
+msgstr "Nachrichtenformat für Überweisungen"
 
 msgctxt "field:account.payment.journal,sepa_payable_initiator_id:"
 msgid "SEPA Payable Initiator Identifier"
-msgstr "SEPA Identifikator Auftraggeber Überweisung"
+msgstr "Identifikator als Überweisungsauftraggeber"
 
 msgctxt "field:account.payment.journal,sepa_receivable_flavor:"
 msgid "Receivable Flavor"
-msgstr "SEPA-Typ Forderungen"
+msgstr "Nachrichtenformat für Lastschriften"
 
 msgctxt "field:account.payment.journal,sepa_receivable_initiator_id:"
 msgid "SEPA Receivable Initiator Identifier"
-msgstr "SEPA Identifikator Einreicher Lastschrift"
+msgstr "Identifikator als Lastschrifteinreicher"
 
 msgctxt "field:account.payment.sepa.mandate,account_number:"
 msgid "Account Number"
 msgstr "Kontonummer"
 
 msgctxt "field:account.payment.sepa.mandate,company:"
 msgid "Company"
@@ -358,19 +358,19 @@
 
 msgctxt "model:ir.model.button,string:message_wait_button"
 msgid "Wait"
 msgstr "Warten"
 
 msgctxt "model:ir.rule.group,name:rule_group_mandate_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.rule.group,name:rule_group_message_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.sequence.type,name:sequence_type_mandate"
 msgid "SEPA Mandate"
 msgstr "SEPA-Mandat"
 
 msgctxt "model:ir.ui.menu,name:menu_mandate_form"
 msgid "SEPA Mandates"
@@ -524,19 +524,19 @@
 
 msgctxt "selection:account.payment.journal,sepa_receivable_initiator_id:"
 msgid "Spanish VAT Number"
 msgstr "Spanische Steuernummer (NIF)"
 
 msgctxt "selection:account.payment.sepa.mandate,scheme:"
 msgid "Business to Business"
-msgstr "B2B-Schema (SEPA B2B)"
+msgstr "Firmenlastschrift (B2B)"
 
 msgctxt "selection:account.payment.sepa.mandate,scheme:"
 msgid "Core"
-msgstr "B2C-Schema (SEPA CORE)"
+msgstr "Basislastschrift (Core)"
 
 msgctxt "selection:account.payment.sepa.mandate,state:"
 msgid "Cancelled"
 msgstr "Annulliert"
 
 msgctxt "selection:account.payment.sepa.mandate,state:"
 msgid "Draft"
```

### Comparing `trytond_account_payment_sepa-7.2.0/locale/es.po` & `trytond_account_payment_sepa-7.2.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/locale/es_419.po` & `trytond_account_payment_sepa-7.2.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/locale/et.po` & `trytond_account_payment_sepa-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/locale/fa.po` & `trytond_account_payment_sepa-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/locale/fi.po` & `trytond_account_payment_sepa-7.2.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/locale/fr.po` & `trytond_account_payment_sepa-7.2.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/locale/hu.po` & `trytond_account_payment_sepa-7.2.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/locale/id.po` & `trytond_account_payment_sepa-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/locale/it.po` & `trytond_account_payment_sepa-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/locale/lo.po` & `trytond_account_payment_sepa-7.2.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/locale/lt.po` & `trytond_account_payment_sepa-7.2.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/locale/nl.po` & `trytond_account_payment_sepa-7.2.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/locale/pl.po` & `trytond_account_payment_sepa-7.2.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/locale/pt.po` & `trytond_account_payment_sepa-7.2.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/locale/ro.po` & `trytond_account_payment_sepa-7.2.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/locale/ru.po` & `trytond_account_payment_sepa-7.2.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/locale/sl.po` & `trytond_account_payment_sepa-7.2.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/locale/tr.po` & `trytond_account_payment_sepa-7.2.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/locale/uk.po` & `trytond_account_payment_sepa-7.2.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/locale/zh_CN.po` & `trytond_account_payment_sepa-7.2.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/mandate.fodt` & `trytond_account_payment_sepa-7.2.1/mandate.fodt`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/message.xml` & `trytond_account_payment_sepa-7.2.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/party.py` & `trytond_account_payment_sepa-7.2.1/party.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/party.xml` & `trytond_account_payment_sepa-7.2.1/party.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/payment.py` & `trytond_account_payment_sepa-7.2.1/payment.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/payment.xml` & `trytond_account_payment_sepa-7.2.1/payment.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/sepa_handler.py` & `trytond_account_payment_sepa-7.2.1/sepa_handler.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/setup.py` & `trytond_account_payment_sepa-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/template/base.003.xml` & `trytond_account_payment_sepa-7.2.1/template/base.003.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/template/base.xml` & `trytond_account_payment_sepa-7.2.1/template/base.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/template/pain.001.001.03.xml` & `trytond_account_payment_sepa-7.2.1/template/pain.001.001.03.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/template/pain.001.001.05.xml` & `trytond_account_payment_sepa-7.2.1/template/pain.001.001.05.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/template/pain.001.003.03.xml` & `trytond_account_payment_sepa-7.2.1/template/pain.001.003.03.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/template/pain.008.001.02.xml` & `trytond_account_payment_sepa-7.2.1/template/pain.008.001.02.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/template/pain.008.001.04.xml` & `trytond_account_payment_sepa-7.2.1/template/pain.008.001.04.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/template/pain.008.003.02.xml` & `trytond_account_payment_sepa-7.2.1/template/pain.008.003.02.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/tests/camt.054.001.01.xml` & `trytond_account_payment_sepa-7.2.1/tests/camt.054.001.01.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/tests/camt.054.001.01.xsd` & `trytond_account_payment_sepa-7.2.1/tests/camt.054.001.01.xsd`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/tests/camt.054.001.02.xml` & `trytond_account_payment_sepa-7.2.1/tests/camt.054.001.02.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/tests/camt.054.001.02.xsd` & `trytond_account_payment_sepa-7.2.1/tests/camt.054.001.02.xsd`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/tests/camt.054.001.03.xml` & `trytond_account_payment_sepa-7.2.1/tests/camt.054.001.03.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/tests/camt.054.001.03.xsd` & `trytond_account_payment_sepa-7.2.1/tests/camt.054.001.03.xsd`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/tests/camt.054.001.04.xml` & `trytond_account_payment_sepa-7.2.1/tests/camt.054.001.04.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/tests/camt.054.001.04.xsd` & `trytond_account_payment_sepa-7.2.1/tests/camt.054.001.04.xsd`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/tests/pain.001.001.03.xsd` & `trytond_account_payment_sepa-7.2.1/tests/pain.001.001.03.xsd`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/tests/pain.001.001.05.xsd` & `trytond_account_payment_sepa-7.2.1/tests/pain.001.001.05.xsd`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/tests/pain.001.003.03.xsd` & `trytond_account_payment_sepa-7.2.1/tests/pain.001.003.03.xsd`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/tests/pain.008.001.02.xsd` & `trytond_account_payment_sepa-7.2.1/tests/pain.008.001.02.xsd`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/tests/pain.008.001.04.xsd` & `trytond_account_payment_sepa-7.2.1/tests/pain.008.001.04.xsd`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/tests/pain.008.003.02.xsd` & `trytond_account_payment_sepa-7.2.1/tests/pain.008.003.02.xsd`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/tests/test_module.py` & `trytond_account_payment_sepa-7.2.1/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/tox.ini` & `trytond_account_payment_sepa-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/trytond_account_payment_sepa.egg-info/PKG-INFO` & `trytond_account_payment_sepa-7.2.1/trytond_account_payment_sepa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_account_payment_sepa
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module for SEPA payment
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account_payment_sepa-7.2.0/trytond_account_payment_sepa.egg-info/SOURCES.txt` & `trytond_account_payment_sepa-7.2.1/trytond_account_payment_sepa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/view/mandate_form.xml` & `trytond_account_payment_sepa-7.2.1/view/mandate_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/view/message_form.xml` & `trytond_account_payment_sepa-7.2.1/view/message_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/view/payment_form.xml` & `trytond_account_payment_sepa-7.2.1/view/payment_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.2.0/view/payment_journal_form.xml` & `trytond_account_payment_sepa-7.2.1/view/payment_journal_form.xml`

 * *Files identical despite different names*

