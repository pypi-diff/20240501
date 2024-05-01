# Comparing `tmp/trytond_account_payment_stripe-7.2.0.tar.gz` & `tmp/trytond_account_payment_stripe-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_payment_stripe-7.2.0.tar", last modified: Mon Apr 29 15:35:15 2024, max compression
+gzip compressed data, was "trytond_account_payment_stripe-7.2.1.tar", last modified: Wed May  1 12:19:43 2024, max compression
```

## Comparing `trytond_account_payment_stripe-7.2.0.tar` & `trytond_account_payment_stripe-7.2.1.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:15.390892 trytond_account_payment_stripe-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     2134 2024-04-29 15:15:29.000000 trytond_account_payment_stripe-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:15:29.000000 trytond_account_payment_stripe-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_payment_stripe-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     5117 2024-04-29 15:35:15.390892 trytond_account_payment_stripe-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2533 2024-02-04 18:51:26.000000 trytond_account_payment_stripe-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      953 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-7.2.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5183 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-7.2.0/checkout.html
--rw-r--r--   0 ced       (1000) ced       (1000)     5064 2024-01-27 09:58:52.000000 trytond_account_payment_stripe-7.2.0/common.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:15.387559 trytond_account_payment_stripe-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3085 2024-04-27 16:30:39.000000 trytond_account_payment_stripe-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2533 2024-02-04 18:51:26.000000 trytond_account_payment_stripe-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:36:58.000000 trytond_account_payment_stripe-7.2.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     1274 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-7.2.0/email_checkout.html
--rw-r--r--   0 ced       (1000) ced       (1000)     1091 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-7.2.0/ir.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:15.387559 trytond_account_payment_stripe-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    16196 2024-04-27 16:43:21.000000 trytond_account_payment_stripe-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17701 2024-04-27 16:43:21.000000 trytond_account_payment_stripe-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16196 2024-04-27 16:43:21.000000 trytond_account_payment_stripe-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17557 2024-04-27 16:43:21.000000 trytond_account_payment_stripe-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17713 2024-04-27 16:43:21.000000 trytond_account_payment_stripe-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14745 2024-04-27 16:43:21.000000 trytond_account_payment_stripe-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14708 2024-04-27 16:43:21.000000 trytond_account_payment_stripe-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17994 2024-04-27 16:43:21.000000 trytond_account_payment_stripe-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16196 2024-04-27 16:43:21.000000 trytond_account_payment_stripe-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17665 2024-04-27 16:43:21.000000 trytond_account_payment_stripe-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16196 2024-04-27 16:43:21.000000 trytond_account_payment_stripe-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14826 2024-04-27 16:43:21.000000 trytond_account_payment_stripe-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16182 2024-04-27 16:43:21.000000 trytond_account_payment_stripe-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16196 2024-04-27 16:43:21.000000 trytond_account_payment_stripe-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16208 2024-04-27 16:43:21.000000 trytond_account_payment_stripe-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17330 2024-04-27 16:43:21.000000 trytond_account_payment_stripe-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16207 2024-04-27 16:43:21.000000 trytond_account_payment_stripe-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16909 2024-04-27 16:43:21.000000 trytond_account_payment_stripe-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14891 2024-04-29 13:17:17.000000 trytond_account_payment_stripe-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16196 2024-04-27 16:43:21.000000 trytond_account_payment_stripe-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16624 2024-04-27 16:43:21.000000 trytond_account_payment_stripe-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16196 2024-04-27 16:43:21.000000 trytond_account_payment_stripe-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14625 2024-04-27 16:43:21.000000 trytond_account_payment_stripe-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16196 2024-04-27 16:43:21.000000 trytond_account_payment_stripe-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      780 2024-03-25 13:26:54.000000 trytond_account_payment_stripe-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2285 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-7.2.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)      556 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-7.2.0/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    70679 2024-04-27 16:30:39.000000 trytond_account_payment_stripe-7.2.0/payment.py
--rw-r--r--   0 ced       (1000) ced       (1000)    17311 2024-04-27 16:30:39.000000 trytond_account_payment_stripe-7.2.0/payment.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2861 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-7.2.0/routes.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:35:15.390892 trytond_account_payment_stripe-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4553 2024-03-17 11:01:36.000000 trytond_account_payment_stripe-7.2.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:15.387559 trytond_account_payment_stripe-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10754 2024-04-27 16:30:39.000000 trytond_account_payment_stripe-7.2.0/tests/scenario_account_payment_stripe.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     8914 2024-04-27 16:30:39.000000 trytond_account_payment_stripe-7.2.0/tests/scenario_account_payment_stripe_dispute.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3149 2024-04-22 12:14:36.000000 trytond_account_payment_stripe-7.2.0/tests/scenario_account_payment_stripe_identical.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5531 2024-04-27 16:30:39.000000 trytond_account_payment_stripe-7.2.0/tests/scenario_account_payment_stripe_intent.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      352 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      399 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-7.2.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:36:58.000000 trytond_account_payment_stripe-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      132 2024-04-29 15:15:24.000000 trytond_account_payment_stripe-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:15.390892 trytond_account_payment_stripe-7.2.0/trytond_account_payment_stripe.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     5117 2024-04-29 15:35:14.000000 trytond_account_payment_stripe-7.2.0/trytond_account_payment_stripe.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2607 2024-04-29 15:35:15.000000 trytond_account_payment_stripe-7.2.0/trytond_account_payment_stripe.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:35:14.000000 trytond_account_payment_stripe-7.2.0/trytond_account_payment_stripe.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       82 2024-04-29 15:35:14.000000 trytond_account_payment_stripe-7.2.0/trytond_account_payment_stripe.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:02.000000 trytond_account_payment_stripe-7.2.0/trytond_account_payment_stripe.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      143 2024-04-29 15:35:14.000000 trytond_account_payment_stripe-7.2.0/trytond_account_payment_stripe.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:35:14.000000 trytond_account_payment_stripe-7.2.0/trytond_account_payment_stripe.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:15.390892 trytond_account_payment_stripe-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      717 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-7.2.0/view/account_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-01-16 14:00:20.000000 trytond_account_payment_stripe-7.2.0/view/account_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      938 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-7.2.0/view/customer_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      378 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-7.2.0/view/customer_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-7.2.0/view/customer_source_detach_ask_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      871 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-7.2.0/view/party_reception_direct_debit_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2519 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-7.2.0/view/payment_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      439 2023-01-16 14:00:20.000000 trytond_account_payment_stripe-7.2.0/view/payment_journal_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      349 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-7.2.0/view/payment_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1039 2024-03-17 11:01:36.000000 trytond_account_payment_stripe-7.2.0/view/refund_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      384 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-7.2.0/view/refund_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:19:43.278806 trytond_account_payment_stripe-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2235 2024-05-01 12:19:39.000000 trytond_account_payment_stripe-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-05-01 12:19:39.000000 trytond_account_payment_stripe-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:20:59.000000 trytond_account_payment_stripe-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:20:59.000000 trytond_account_payment_stripe-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     5117 2024-05-01 12:19:43.278806 trytond_account_payment_stripe-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2533 2024-04-30 17:20:59.000000 trytond_account_payment_stripe-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      953 2024-04-30 17:20:59.000000 trytond_account_payment_stripe-7.2.1/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5183 2024-04-30 17:20:59.000000 trytond_account_payment_stripe-7.2.1/checkout.html
+-rw-r--r--   0 ced       (1000) ced       (1000)     5064 2024-04-30 17:20:59.000000 trytond_account_payment_stripe-7.2.1/common.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:19:43.268806 trytond_account_payment_stripe-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3085 2024-04-30 17:20:59.000000 trytond_account_payment_stripe-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2533 2024-04-30 17:20:59.000000 trytond_account_payment_stripe-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:20:59.000000 trytond_account_payment_stripe-7.2.1/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     1274 2024-04-30 17:20:59.000000 trytond_account_payment_stripe-7.2.1/email_checkout.html
+-rw-r--r--   0 ced       (1000) ced       (1000)     1091 2024-04-30 17:20:59.000000 trytond_account_payment_stripe-7.2.1/ir.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:19:43.272139 trytond_account_payment_stripe-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    16196 2024-04-30 17:20:59.000000 trytond_account_payment_stripe-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17701 2024-04-30 17:20:59.000000 trytond_account_payment_stripe-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16196 2024-04-30 17:20:59.000000 trytond_account_payment_stripe-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17557 2024-04-30 17:21:59.000000 trytond_account_payment_stripe-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17713 2024-04-30 17:20:59.000000 trytond_account_payment_stripe-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14745 2024-04-30 17:20:59.000000 trytond_account_payment_stripe-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14708 2024-04-30 17:20:59.000000 trytond_account_payment_stripe-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17994 2024-04-30 17:20:59.000000 trytond_account_payment_stripe-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16196 2024-04-30 17:20:59.000000 trytond_account_payment_stripe-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17665 2024-04-30 17:20:59.000000 trytond_account_payment_stripe-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16196 2024-04-30 17:20:59.000000 trytond_account_payment_stripe-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14826 2024-04-30 17:20:59.000000 trytond_account_payment_stripe-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16182 2024-04-30 17:20:59.000000 trytond_account_payment_stripe-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16196 2024-04-30 17:20:59.000000 trytond_account_payment_stripe-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16208 2024-04-30 17:20:59.000000 trytond_account_payment_stripe-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17330 2024-04-30 17:20:59.000000 trytond_account_payment_stripe-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16207 2024-04-30 17:20:59.000000 trytond_account_payment_stripe-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16909 2024-04-30 17:20:59.000000 trytond_account_payment_stripe-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14891 2024-04-30 17:20:59.000000 trytond_account_payment_stripe-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16196 2024-04-30 17:20:59.000000 trytond_account_payment_stripe-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16624 2024-04-30 17:20:59.000000 trytond_account_payment_stripe-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16196 2024-04-30 17:20:59.000000 trytond_account_payment_stripe-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14625 2024-04-30 17:20:59.000000 trytond_account_payment_stripe-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16196 2024-04-30 17:20:59.000000 trytond_account_payment_stripe-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      780 2024-04-30 17:20:59.000000 trytond_account_payment_stripe-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2285 2024-04-30 17:20:59.000000 trytond_account_payment_stripe-7.2.1/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      556 2024-04-30 17:20:59.000000 trytond_account_payment_stripe-7.2.1/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    70679 2024-04-30 17:20:59.000000 trytond_account_payment_stripe-7.2.1/payment.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    17311 2024-04-30 17:20:59.000000 trytond_account_payment_stripe-7.2.1/payment.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2861 2024-04-30 17:20:59.000000 trytond_account_payment_stripe-7.2.1/routes.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 12:19:43.278806 trytond_account_payment_stripe-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4553 2024-04-30 17:20:59.000000 trytond_account_payment_stripe-7.2.1/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:19:43.275473 trytond_account_payment_stripe-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:20:59.000000 trytond_account_payment_stripe-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10754 2024-04-30 17:20:59.000000 trytond_account_payment_stripe-7.2.1/tests/scenario_account_payment_stripe.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     8914 2024-04-30 17:20:59.000000 trytond_account_payment_stripe-7.2.1/tests/scenario_account_payment_stripe_dispute.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3149 2024-04-30 17:20:59.000000 trytond_account_payment_stripe-7.2.1/tests/scenario_account_payment_stripe_identical.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5531 2024-04-30 17:20:59.000000 trytond_account_payment_stripe-7.2.1/tests/scenario_account_payment_stripe_intent.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      352 2024-04-30 17:20:59.000000 trytond_account_payment_stripe-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      399 2024-04-30 17:20:59.000000 trytond_account_payment_stripe-7.2.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:20:59.000000 trytond_account_payment_stripe-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      132 2024-04-30 17:21:06.000000 trytond_account_payment_stripe-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:19:43.275473 trytond_account_payment_stripe-7.2.1/trytond_account_payment_stripe.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     5117 2024-05-01 12:19:42.000000 trytond_account_payment_stripe-7.2.1/trytond_account_payment_stripe.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2607 2024-05-01 12:19:43.000000 trytond_account_payment_stripe-7.2.1/trytond_account_payment_stripe.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:19:42.000000 trytond_account_payment_stripe-7.2.1/trytond_account_payment_stripe.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       82 2024-05-01 12:19:42.000000 trytond_account_payment_stripe-7.2.1/trytond_account_payment_stripe.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:19:42.000000 trytond_account_payment_stripe-7.2.1/trytond_account_payment_stripe.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      143 2024-05-01 12:19:42.000000 trytond_account_payment_stripe-7.2.1/trytond_account_payment_stripe.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 12:19:42.000000 trytond_account_payment_stripe-7.2.1/trytond_account_payment_stripe.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:19:43.275473 trytond_account_payment_stripe-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      717 2024-04-30 17:20:59.000000 trytond_account_payment_stripe-7.2.1/view/account_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2024-04-30 17:20:59.000000 trytond_account_payment_stripe-7.2.1/view/account_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      938 2024-04-30 17:20:59.000000 trytond_account_payment_stripe-7.2.1/view/customer_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      378 2024-04-30 17:20:59.000000 trytond_account_payment_stripe-7.2.1/view/customer_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      306 2024-04-30 17:20:59.000000 trytond_account_payment_stripe-7.2.1/view/customer_source_detach_ask_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      871 2024-04-30 17:20:59.000000 trytond_account_payment_stripe-7.2.1/view/party_reception_direct_debit_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2519 2024-04-30 17:20:59.000000 trytond_account_payment_stripe-7.2.1/view/payment_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      439 2024-04-30 17:20:59.000000 trytond_account_payment_stripe-7.2.1/view/payment_journal_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      349 2024-04-30 17:20:59.000000 trytond_account_payment_stripe-7.2.1/view/payment_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1039 2024-04-30 17:20:59.000000 trytond_account_payment_stripe-7.2.1/view/refund_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      384 2024-04-30 17:20:59.000000 trytond_account_payment_stripe-7.2.1/view/refund_list.xml
```

### Comparing `trytond_account_payment_stripe-7.2.0/CHANGELOG` & `trytond_account_payment_stripe-7.2.1/CHANGELOG`

 * *Files 4% similar despite different names*

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

### Comparing `trytond_account_payment_stripe-7.2.0/COPYRIGHT` & `trytond_account_payment_stripe-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.2.0/LICENSE` & `trytond_account_payment_stripe-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.2.0/PKG-INFO` & `trytond_account_payment_stripe-7.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_account_payment_stripe
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module for Stripe payment
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account_payment_stripe-7.2.0/README.rst` & `trytond_account_payment_stripe-7.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.2.0/__init__.py` & `trytond_account_payment_stripe-7.2.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.2.0/checkout.html` & `trytond_account_payment_stripe-7.2.1/checkout.html`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.2.0/common.py` & `trytond_account_payment_stripe-7.2.1/common.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.2.0/doc/conf.py` & `trytond_account_payment_stripe-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.2.0/doc/index.rst` & `trytond_account_payment_stripe-7.2.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.2.0/email_checkout.html` & `trytond_account_payment_stripe-7.2.1/email_checkout.html`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.2.0/ir.py` & `trytond_account_payment_stripe-7.2.1/ir.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.2.0/locale/bg.po` & `trytond_account_payment_stripe-7.2.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.2.0/locale/ca.po` & `trytond_account_payment_stripe-7.2.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.2.0/locale/cs.po` & `trytond_account_payment_stripe-7.2.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.2.0/locale/de.po` & `trytond_account_payment_stripe-7.2.1/locale/de.po`

 * *Files 0% similar despite different names*

```diff
@@ -404,15 +404,15 @@
 msgstr ""
 "Um Zahlung \"%(payment)s\" ausführen zu können, muss ein Stripe Token oder "
 "ein Kunde erfasst werden."
 
 msgctxt "model:ir.message,text:msg_stripe_receivable"
 msgid "To pay \"%(payment)s\", you cannot use a stripe journal \"%(journal)s\"."
 msgstr ""
-"\"(%payment)s\" kann nicht über das Stripe Journal \"%(journal)s\" bezahlt "
+"\"%(payment)s\" kann nicht über das Stripe Journal \"%(journal)s\" bezahlt "
 "werden."
 
 msgctxt "model:ir.model.button,confirm:account_new_identifier_button"
 msgid ""
 "This action will make the previous URL unusable. Do you want to continue?"
 msgstr ""
 "Diese Aktion macht die vorherige URL unbrauchbar. Möchten Sie fortsetzen?"
```

### Comparing `trytond_account_payment_stripe-7.2.0/locale/es.po` & `trytond_account_payment_stripe-7.2.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.2.0/locale/es_419.po` & `trytond_account_payment_stripe-7.2.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.2.0/locale/et.po` & `trytond_account_payment_stripe-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.2.0/locale/fa.po` & `trytond_account_payment_stripe-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.2.0/locale/fi.po` & `trytond_account_payment_stripe-7.2.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.2.0/locale/fr.po` & `trytond_account_payment_stripe-7.2.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.2.0/locale/hu.po` & `trytond_account_payment_stripe-7.2.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.2.0/locale/id.po` & `trytond_account_payment_stripe-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.2.0/locale/it.po` & `trytond_account_payment_stripe-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.2.0/locale/lo.po` & `trytond_account_payment_stripe-7.2.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.2.0/locale/lt.po` & `trytond_account_payment_stripe-7.2.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.2.0/locale/nl.po` & `trytond_account_payment_stripe-7.2.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.2.0/locale/pl.po` & `trytond_account_payment_stripe-7.2.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.2.0/locale/pt.po` & `trytond_account_payment_stripe-7.2.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.2.0/locale/ro.po` & `trytond_account_payment_stripe-7.2.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.2.0/locale/ru.po` & `trytond_account_payment_stripe-7.2.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.2.0/locale/sl.po` & `trytond_account_payment_stripe-7.2.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.2.0/locale/tr.po` & `trytond_account_payment_stripe-7.2.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.2.0/locale/uk.po` & `trytond_account_payment_stripe-7.2.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.2.0/locale/zh_CN.po` & `trytond_account_payment_stripe-7.2.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.2.0/message.xml` & `trytond_account_payment_stripe-7.2.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.2.0/party.py` & `trytond_account_payment_stripe-7.2.1/party.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.2.0/party.xml` & `trytond_account_payment_stripe-7.2.1/party.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.2.0/payment.py` & `trytond_account_payment_stripe-7.2.1/payment.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.2.0/payment.xml` & `trytond_account_payment_stripe-7.2.1/payment.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.2.0/routes.py` & `trytond_account_payment_stripe-7.2.1/routes.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.2.0/setup.py` & `trytond_account_payment_stripe-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.2.0/tests/scenario_account_payment_stripe.rst` & `trytond_account_payment_stripe-7.2.1/tests/scenario_account_payment_stripe.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.2.0/tests/scenario_account_payment_stripe_dispute.rst` & `trytond_account_payment_stripe-7.2.1/tests/scenario_account_payment_stripe_dispute.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.2.0/tests/scenario_account_payment_stripe_identical.rst` & `trytond_account_payment_stripe-7.2.1/tests/scenario_account_payment_stripe_identical.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.2.0/tests/scenario_account_payment_stripe_intent.rst` & `trytond_account_payment_stripe-7.2.1/tests/scenario_account_payment_stripe_intent.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.2.0/tox.ini` & `trytond_account_payment_stripe-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.2.0/trytond_account_payment_stripe.egg-info/PKG-INFO` & `trytond_account_payment_stripe-7.2.1/trytond_account_payment_stripe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_account_payment_stripe
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module for Stripe payment
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account_payment_stripe-7.2.0/trytond_account_payment_stripe.egg-info/SOURCES.txt` & `trytond_account_payment_stripe-7.2.1/trytond_account_payment_stripe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.2.0/view/account_form.xml` & `trytond_account_payment_stripe-7.2.1/view/account_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.2.0/view/customer_form.xml` & `trytond_account_payment_stripe-7.2.1/view/customer_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.2.0/view/party_reception_direct_debit_form.xml` & `trytond_account_payment_stripe-7.2.1/view/party_reception_direct_debit_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.2.0/view/payment_form.xml` & `trytond_account_payment_stripe-7.2.1/view/payment_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.2.0/view/refund_form.xml` & `trytond_account_payment_stripe-7.2.1/view/refund_form.xml`

 * *Files identical despite different names*

