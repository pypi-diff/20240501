# Comparing `tmp/trytond_party-7.2.0.tar.gz` & `tmp/trytond_party-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_party-7.2.0.tar", last modified: Mon Apr 29 15:41:54 2024, max compression
+gzip compressed data, was "trytond_party-7.2.1.tar", last modified: Wed May  1 11:57:09 2024, max compression
```

## Comparing `trytond_party-7.2.0.tar` & `trytond_party-7.2.1.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:54.547119 trytond_party-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     7035 2024-04-29 15:20:52.000000 trytond_party-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      884 2024-04-29 15:20:52.000000 trytond_party-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_party-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_party-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3003 2024-04-29 15:41:54.547119 trytond_party-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      361 2023-04-15 07:12:15.000000 trytond_party-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1062 2023-04-15 07:12:15.000000 trytond_party-7.2.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    16172 2024-02-04 18:51:26.000000 trytond_party-7.2.0/address.py
--rw-r--r--   0 ced       (1000) ced       (1000)    25150 2024-04-27 16:30:39.000000 trytond_party-7.2.0/address.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1173 2024-01-27 09:58:52.000000 trytond_party-7.2.0/category.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3612 2024-04-27 16:30:39.000000 trytond_party-7.2.0/category.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4042 2024-02-04 18:51:26.000000 trytond_party-7.2.0/configuration.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2205 2024-04-27 16:30:39.000000 trytond_party-7.2.0/configuration.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    13151 2024-02-04 18:51:26.000000 trytond_party-7.2.0/contact_mechanism.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2097 2023-04-15 07:12:15.000000 trytond_party-7.2.0/contact_mechanism.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      658 2023-04-15 07:12:15.000000 trytond_party-7.2.0/country.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:54.540452 trytond_party-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3068 2024-04-27 16:30:39.000000 trytond_party-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6349 2023-04-15 07:12:15.000000 trytond_party-7.2.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      361 2023-04-15 07:12:15.000000 trytond_party-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_party-7.2.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:13.000000 trytond_party-7.2.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     4129 2023-04-15 07:12:15.000000 trytond_party-7.2.0/doc/usage.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      599 2024-02-04 18:51:26.000000 trytond_party-7.2.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:54.540452 trytond_party-7.2.0/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_party-7.2.0/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      259 2023-01-16 14:00:20.000000 trytond_party-7.2.0/icons/tryton-party.svg
--rw-r--r--   0 ced       (1000) ced       (1000)     3841 2023-04-15 07:12:15.000000 trytond_party-7.2.0/ir.py
--rw-r--r--   0 ced       (1000) ced       (1000)      484 2023-04-15 07:12:15.000000 trytond_party-7.2.0/ir.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    31778 2023-01-16 14:00:20.000000 trytond_party-7.2.0/label.fodt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:54.543785 trytond_party-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    34600 2024-04-27 16:43:24.000000 trytond_party-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    41677 2024-04-27 16:43:24.000000 trytond_party-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    33245 2024-04-27 16:43:24.000000 trytond_party-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    43389 2024-04-27 16:43:24.000000 trytond_party-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    42097 2024-04-27 16:43:24.000000 trytond_party-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    33184 2024-04-27 16:43:24.000000 trytond_party-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    38928 2024-04-27 16:43:24.000000 trytond_party-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    38349 2024-04-27 16:43:24.000000 trytond_party-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    33030 2024-04-27 16:43:24.000000 trytond_party-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    41643 2024-04-27 16:43:24.000000 trytond_party-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    35922 2024-04-27 16:43:24.000000 trytond_party-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    33899 2024-04-27 16:43:24.000000 trytond_party-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    36283 2024-04-27 16:43:24.000000 trytond_party-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    37727 2024-04-27 16:43:24.000000 trytond_party-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    39999 2024-04-27 16:43:24.000000 trytond_party-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    41340 2024-04-27 16:43:24.000000 trytond_party-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    40052 2024-04-27 16:43:24.000000 trytond_party-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    36259 2024-04-27 16:43:24.000000 trytond_party-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    40658 2024-04-29 13:17:17.000000 trytond_party-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    35113 2024-04-27 16:43:24.000000 trytond_party-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    41421 2024-04-27 16:43:24.000000 trytond_party-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    33030 2024-04-27 16:43:24.000000 trytond_party-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    49356 2024-04-27 16:43:24.000000 trytond_party-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    35733 2024-04-27 16:43:24.000000 trytond_party-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3240 2024-02-04 18:51:26.000000 trytond_party-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    42600 2024-04-27 16:30:39.000000 trytond_party-7.2.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8099 2023-04-15 07:12:15.000000 trytond_party-7.2.0/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:41:54.547119 trytond_party-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4638 2024-04-27 16:30:39.000000 trytond_party-7.2.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:54.543785 trytond_party-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      227 2023-04-15 07:12:15.000000 trytond_party-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1618 2024-04-22 12:14:36.000000 trytond_party-7.2.0/tests/scenario_party_erase.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      868 2024-01-27 09:58:52.000000 trytond_party-7.2.0/tests/scenario_party_identifier_notifications.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1101 2024-04-22 12:14:36.000000 trytond_party-7.2.0/tests/scenario_party_phone_number.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1407 2024-04-22 12:14:36.000000 trytond_party-7.2.0/tests/scenario_party_replace.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    19513 2024-04-01 21:57:37.000000 trytond_party-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_party-7.2.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:13.000000 trytond_party-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      186 2024-04-29 15:20:48.000000 trytond_party-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:54.547119 trytond_party-7.2.0/trytond_party.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3003 2024-04-29 15:41:54.000000 trytond_party-7.2.0/trytond_party.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     3500 2024-04-29 15:41:54.000000 trytond_party-7.2.0/trytond_party.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:41:54.000000 trytond_party-7.2.0/trytond_party.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       48 2024-04-29 15:41:54.000000 trytond_party-7.2.0/trytond_party.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-02-14 15:56:20.000000 trytond_party-7.2.0/trytond_party.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      176 2024-04-29 15:41:54.000000 trytond_party-7.2.0/trytond_party.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:41:54.000000 trytond_party-7.2.0/trytond_party.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:54.547119 trytond_party-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)     1579 2024-03-17 11:01:36.000000 trytond_party-7.2.0/view/address_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1022 2024-03-17 11:01:36.000000 trytond_party-7.2.0/view/address_form_simple.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      317 2023-04-15 07:12:15.000000 trytond_party-7.2.0/view/address_format_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      104 2023-04-15 07:12:15.000000 trytond_party-7.2.0/view/address_format_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      386 2023-04-15 07:12:15.000000 trytond_party-7.2.0/view/address_subdivision_type_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      256 2023-04-15 07:12:15.000000 trytond_party-7.2.0/view/address_subdivision_type_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      498 2023-04-15 07:12:15.000000 trytond_party-7.2.0/view/address_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      518 2023-04-15 07:12:15.000000 trytond_party-7.2.0/view/address_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      383 2023-01-16 14:00:20.000000 trytond_party-7.2.0/view/category_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      226 2023-01-16 14:00:20.000000 trytond_party-7.2.0/view/category_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      239 2023-04-15 07:12:15.000000 trytond_party-7.2.0/view/category_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      265 2023-01-16 14:00:20.000000 trytond_party-7.2.0/view/check_vies_result.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      453 2024-04-22 12:14:36.000000 trytond_party-7.2.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1195 2023-04-15 07:12:15.000000 trytond_party-7.2.0/view/contact_mechanism_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      460 2023-04-15 07:12:15.000000 trytond_party-7.2.0/view/contact_mechanism_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      530 2023-04-15 07:12:15.000000 trytond_party-7.2.0/view/contact_mechanism_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      357 2024-04-27 16:30:39.000000 trytond_party-7.2.0/view/email_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      238 2023-01-16 14:00:20.000000 trytond_party-7.2.0/view/erase_ask_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      599 2024-01-27 09:58:52.000000 trytond_party-7.2.0/view/identifier_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      334 2023-04-15 07:12:15.000000 trytond_party-7.2.0/view/identifier_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-04-15 07:12:15.000000 trytond_party-7.2.0/view/identifier_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1593 2024-03-17 11:01:36.000000 trytond_party-7.2.0/view/party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      333 2023-04-15 07:12:15.000000 trytond_party-7.2.0/view/party_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      190 2023-01-16 14:00:20.000000 trytond_party-7.2.0/view/replace_ask_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:57:09.800387 trytond_party-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     7136 2024-05-01 11:57:06.000000 trytond_party-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      884 2024-05-01 11:57:06.000000 trytond_party-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:20:59.000000 trytond_party-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:20:59.000000 trytond_party-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3003 2024-05-01 11:57:09.800387 trytond_party-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      361 2024-04-30 17:20:59.000000 trytond_party-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1062 2024-04-30 17:20:59.000000 trytond_party-7.2.1/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    16172 2024-04-30 17:20:59.000000 trytond_party-7.2.1/address.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    25150 2024-04-30 17:20:59.000000 trytond_party-7.2.1/address.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1173 2024-04-30 17:20:59.000000 trytond_party-7.2.1/category.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3612 2024-04-30 17:20:59.000000 trytond_party-7.2.1/category.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4042 2024-04-30 17:20:59.000000 trytond_party-7.2.1/configuration.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2205 2024-04-30 17:20:59.000000 trytond_party-7.2.1/configuration.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    13151 2024-04-30 17:20:59.000000 trytond_party-7.2.1/contact_mechanism.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2097 2024-04-30 17:20:59.000000 trytond_party-7.2.1/contact_mechanism.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      658 2024-04-30 17:20:59.000000 trytond_party-7.2.1/country.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:57:09.793721 trytond_party-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3068 2024-04-30 17:20:59.000000 trytond_party-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6349 2024-04-30 17:20:59.000000 trytond_party-7.2.1/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      361 2024-04-30 17:20:59.000000 trytond_party-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-30 17:20:59.000000 trytond_party-7.2.1/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:20:59.000000 trytond_party-7.2.1/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     4129 2024-04-30 17:20:59.000000 trytond_party-7.2.1/doc/usage.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      599 2024-04-30 17:20:59.000000 trytond_party-7.2.1/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:57:09.793721 trytond_party-7.2.1/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2024-04-30 17:20:59.000000 trytond_party-7.2.1/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      259 2024-04-30 17:20:59.000000 trytond_party-7.2.1/icons/tryton-party.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)     3841 2024-04-30 17:20:59.000000 trytond_party-7.2.1/ir.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      484 2024-04-30 17:20:59.000000 trytond_party-7.2.1/ir.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    31778 2024-04-30 17:20:59.000000 trytond_party-7.2.1/label.fodt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:57:09.797054 trytond_party-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    34600 2024-04-30 17:20:59.000000 trytond_party-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    41677 2024-04-30 17:20:59.000000 trytond_party-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    33245 2024-04-30 17:20:59.000000 trytond_party-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    43399 2024-04-30 17:21:59.000000 trytond_party-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    42097 2024-04-30 17:20:59.000000 trytond_party-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    33184 2024-04-30 17:20:59.000000 trytond_party-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    38928 2024-04-30 17:20:59.000000 trytond_party-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    38349 2024-04-30 17:20:59.000000 trytond_party-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    33030 2024-04-30 17:20:59.000000 trytond_party-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    41643 2024-04-30 17:20:59.000000 trytond_party-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    35922 2024-04-30 17:20:59.000000 trytond_party-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    33899 2024-04-30 17:20:59.000000 trytond_party-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    36283 2024-04-30 17:20:59.000000 trytond_party-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37727 2024-04-30 17:20:59.000000 trytond_party-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    39999 2024-04-30 17:20:59.000000 trytond_party-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    41340 2024-04-30 17:20:59.000000 trytond_party-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    40334 2024-04-30 17:21:59.000000 trytond_party-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    36259 2024-04-30 17:20:59.000000 trytond_party-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    40658 2024-04-30 17:20:59.000000 trytond_party-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    35113 2024-04-30 17:20:59.000000 trytond_party-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    41421 2024-04-30 17:20:59.000000 trytond_party-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    33030 2024-04-30 17:20:59.000000 trytond_party-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    49356 2024-04-30 17:20:59.000000 trytond_party-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    35733 2024-04-30 17:20:59.000000 trytond_party-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3240 2024-04-30 17:20:59.000000 trytond_party-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    42600 2024-04-30 17:20:59.000000 trytond_party-7.2.1/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8099 2024-04-30 17:20:59.000000 trytond_party-7.2.1/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 11:57:09.800387 trytond_party-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4638 2024-04-30 17:20:59.000000 trytond_party-7.2.1/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:57:09.797054 trytond_party-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      227 2024-04-30 17:20:59.000000 trytond_party-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1618 2024-04-30 17:20:59.000000 trytond_party-7.2.1/tests/scenario_party_erase.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      868 2024-04-30 17:20:59.000000 trytond_party-7.2.1/tests/scenario_party_identifier_notifications.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1101 2024-04-30 17:20:59.000000 trytond_party-7.2.1/tests/scenario_party_phone_number.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1407 2024-04-30 17:20:59.000000 trytond_party-7.2.1/tests/scenario_party_replace.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    19513 2024-04-30 17:20:59.000000 trytond_party-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:20:59.000000 trytond_party-7.2.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:20:59.000000 trytond_party-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      186 2024-04-30 17:21:06.000000 trytond_party-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:57:09.800387 trytond_party-7.2.1/trytond_party.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3003 2024-05-01 11:57:09.000000 trytond_party-7.2.1/trytond_party.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     3500 2024-05-01 11:57:09.000000 trytond_party-7.2.1/trytond_party.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:57:09.000000 trytond_party-7.2.1/trytond_party.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       48 2024-05-01 11:57:09.000000 trytond_party-7.2.1/trytond_party.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:57:09.000000 trytond_party-7.2.1/trytond_party.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      176 2024-05-01 11:57:09.000000 trytond_party-7.2.1/trytond_party.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 11:57:09.000000 trytond_party-7.2.1/trytond_party.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:57:09.800387 trytond_party-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1579 2024-04-30 17:20:59.000000 trytond_party-7.2.1/view/address_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1022 2024-04-30 17:20:59.000000 trytond_party-7.2.1/view/address_form_simple.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      317 2024-04-30 17:20:59.000000 trytond_party-7.2.1/view/address_format_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      104 2024-04-30 17:20:59.000000 trytond_party-7.2.1/view/address_format_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      386 2024-04-30 17:20:59.000000 trytond_party-7.2.1/view/address_subdivision_type_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      256 2024-04-30 17:20:59.000000 trytond_party-7.2.1/view/address_subdivision_type_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      498 2024-04-30 17:20:59.000000 trytond_party-7.2.1/view/address_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      518 2024-04-30 17:20:59.000000 trytond_party-7.2.1/view/address_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      383 2024-04-30 17:20:59.000000 trytond_party-7.2.1/view/category_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      226 2024-04-30 17:20:59.000000 trytond_party-7.2.1/view/category_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      239 2024-04-30 17:20:59.000000 trytond_party-7.2.1/view/category_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      265 2024-04-30 17:20:59.000000 trytond_party-7.2.1/view/check_vies_result.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      453 2024-04-30 17:20:59.000000 trytond_party-7.2.1/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1195 2024-04-30 17:20:59.000000 trytond_party-7.2.1/view/contact_mechanism_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      460 2024-04-30 17:20:59.000000 trytond_party-7.2.1/view/contact_mechanism_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      530 2024-04-30 17:20:59.000000 trytond_party-7.2.1/view/contact_mechanism_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      357 2024-04-30 17:20:59.000000 trytond_party-7.2.1/view/email_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      238 2024-04-30 17:20:59.000000 trytond_party-7.2.1/view/erase_ask_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      599 2024-04-30 17:20:59.000000 trytond_party-7.2.1/view/identifier_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      334 2024-04-30 17:20:59.000000 trytond_party-7.2.1/view/identifier_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      354 2024-04-30 17:20:59.000000 trytond_party-7.2.1/view/identifier_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1593 2024-04-30 17:20:59.000000 trytond_party-7.2.1/view/party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      333 2024-04-30 17:20:59.000000 trytond_party-7.2.1/view/party_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      190 2024-04-30 17:20:59.000000 trytond_party-7.2.1/view/replace_ask_form.xml
```

### Comparing `trytond_party-7.2.0/CHANGELOG` & `trytond_party-7.2.1/CHANGELOG`

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
 * Use usage from context for default contact mechanism on party
 
 Version 7.0.0 - 2023-10-30
 --------------------------
```

### Comparing `trytond_party-7.2.0/COPYRIGHT` & `trytond_party-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_party-7.2.0/LICENSE` & `trytond_party-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_party-7.2.0/PKG-INFO` & `trytond_party-7.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_party
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module with parties and addresses
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_party-7.2.0/__init__.py` & `trytond_party-7.2.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_party-7.2.0/address.py` & `trytond_party-7.2.1/address.py`

 * *Files identical despite different names*

### Comparing `trytond_party-7.2.0/address.xml` & `trytond_party-7.2.1/address.xml`

 * *Files identical despite different names*

### Comparing `trytond_party-7.2.0/category.py` & `trytond_party-7.2.1/category.py`

 * *Files identical despite different names*

### Comparing `trytond_party-7.2.0/category.xml` & `trytond_party-7.2.1/category.xml`

 * *Files identical despite different names*

### Comparing `trytond_party-7.2.0/configuration.py` & `trytond_party-7.2.1/configuration.py`

 * *Files identical despite different names*

### Comparing `trytond_party-7.2.0/configuration.xml` & `trytond_party-7.2.1/configuration.xml`

 * *Files identical despite different names*

### Comparing `trytond_party-7.2.0/contact_mechanism.py` & `trytond_party-7.2.1/contact_mechanism.py`

 * *Files identical despite different names*

### Comparing `trytond_party-7.2.0/contact_mechanism.xml` & `trytond_party-7.2.1/contact_mechanism.xml`

 * *Files identical despite different names*

### Comparing `trytond_party-7.2.0/country.py` & `trytond_party-7.2.1/country.py`

 * *Files identical despite different names*

### Comparing `trytond_party-7.2.0/doc/conf.py` & `trytond_party-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_party-7.2.0/doc/design.rst` & `trytond_party-7.2.1/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_party-7.2.0/doc/usage.rst` & `trytond_party-7.2.1/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `trytond_party-7.2.0/exceptions.py` & `trytond_party-7.2.1/exceptions.py`

 * *Files identical despite different names*

### Comparing `trytond_party-7.2.0/icons/LICENSE` & `trytond_party-7.2.1/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_party-7.2.0/ir.py` & `trytond_party-7.2.1/ir.py`

 * *Files identical despite different names*

### Comparing `trytond_party-7.2.0/label.fodt` & `trytond_party-7.2.1/label.fodt`

 * *Files identical despite different names*

### Comparing `trytond_party-7.2.0/locale/bg.po` & `trytond_party-7.2.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_party-7.2.0/locale/ca.po` & `trytond_party-7.2.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_party-7.2.0/locale/cs.po` & `trytond_party-7.2.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_party-7.2.0/locale/de.po` & `trytond_party-7.2.1/locale/de.po`

 * *Files 1% similar despite different names*

```diff
@@ -220,15 +220,15 @@
 
 msgctxt "field:party.party,code:"
 msgid "Code"
 msgstr "Code Partei"
 
 msgctxt "field:party.party,code_readonly:"
 msgid "Code Readonly"
-msgstr "Code (nur lesbar)"
+msgstr "Code ist nur lesbar"
 
 msgctxt "field:party.party,contact_mechanisms:"
 msgid "Contact Mechanisms"
 msgstr "Kontaktinformationen"
 
 msgctxt "field:party.party,distance:"
 msgid "Distance"
@@ -1160,15 +1160,15 @@
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Russian Tax identifier"
 msgstr "Russischer Steueridentifikator"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "SEPA Identifier of the Creditor (AT-02)"
-msgstr "SEPA Kreditorenidentifikation (AT-02)"
+msgstr "SEPA Gläubiger-Identifikationsnummer (AT-02)"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "San Marino National Tax Number"
 msgstr "San-marinesische Steuernummer (COE)"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Serbian Tax Identification"
```

### Comparing `trytond_party-7.2.0/locale/es.po` & `trytond_party-7.2.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_party-7.2.0/locale/es_419.po` & `trytond_party-7.2.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_party-7.2.0/locale/et.po` & `trytond_party-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_party-7.2.0/locale/fa.po` & `trytond_party-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_party-7.2.0/locale/fi.po` & `trytond_party-7.2.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_party-7.2.0/locale/fr.po` & `trytond_party-7.2.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_party-7.2.0/locale/hu.po` & `trytond_party-7.2.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_party-7.2.0/locale/id.po` & `trytond_party-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_party-7.2.0/locale/it.po` & `trytond_party-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_party-7.2.0/locale/lo.po` & `trytond_party-7.2.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_party-7.2.0/locale/lt.po` & `trytond_party-7.2.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_party-7.2.0/locale/nl.po` & `trytond_party-7.2.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_party-7.2.0/locale/pl.po` & `trytond_party-7.2.1/locale/pl.po`

 * *Files 6% similar despite different names*

```diff
@@ -512,18 +512,17 @@
 msgid ""
 "Parties have different tax identifiers: \"%(source_code)s\" vs "
 "\"%(destination_code)s\"."
 msgstr ""
 "Strony mają różny identyfikator podatkowy: \"%(source_code)s\" różni się od "
 "\"%(destination_code)s\"."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_email_invalid"
 msgid "The email address \"%(email)s\" for party \"%(party)s\" is not valid."
-msgstr "Typ %(type)s \"%(code)s\" strony \"%(party)s\" jest niepoprawny."
+msgstr "Adres e-mail \"%(email)s\" strony \"%(party)s\" jest nieprawidłowy."
 
 msgctxt "model:ir.message,text:msg_erase_active_party"
 msgid "Party \"%(party)s\" cannot be erased because they are still active."
 msgstr ""
 "Strona \"%(party)s\" nie może zostać usunięta, ponieważ nadal jest aktywna."
 
 msgctxt "model:ir.message,text:msg_identifier_type_remove"
@@ -548,15 +547,15 @@
 
 msgctxt "model:ir.message,text:msg_party_code_unique"
 msgid "The code on party must be unique."
 msgstr "Kod strony musi być unikatowy."
 
 msgctxt "model:ir.message,text:msg_party_identifier_duplicate"
 msgid "The party \"%(party)s\" has the same %(type)s \"%(code)s\"."
-msgstr ""
+msgstr "Strona \"%(party)s\" ma ten sam %(type)s \"%(code)s\"."
 
 msgctxt "model:ir.message,text:msg_party_set_contact_mechanism"
 msgid ""
 "To change the \"%(field)s\" for party \"%(party)s\", you must edit their "
 "contact mechanisms."
 msgstr ""
 "Aby zmienić pole \"%(field)s\" strony \"%(party)s\" należy zmodyfikować "
@@ -682,18 +681,17 @@
 msgid "Party Administration"
 msgstr "Administracja ustawieniami strony"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Albanian VAT Number"
 msgstr "Albański numer VAT"
 
-#, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Algerian Tax Number"
-msgstr "Numer podatkowy w Andorze"
+msgstr "Algierski Numer Podatkowy"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Andorra Tax Number"
 msgstr "Numer podatkowy w Andorze"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Argentinian National Identity Number"
@@ -723,36 +721,33 @@
 msgid "Austrian Social Security Number"
 msgstr "Australijski numer przedsiębiorstwa"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Austrian Tax Identification"
 msgstr "Austriacka identyfikacja podatkowa"
 
-#, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Austrian Umsatzsteuer-Identifikationsnummer"
-msgstr "Austriacka identyfikacja podatkowa"
+msgstr "Austriacki Umsatzsteuer-Identifikations-Nummer"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Belarus VAT Number"
 msgstr "Białoruski numer VAT"
 
-#, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Belgian BIS Number"
-msgstr "Bułgarski numer VAT"
+msgstr "Belgijski numer BIS"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Belgian Enterprise Number"
 msgstr "Belgijski numer przedsiębiorstw"
 
-#, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Belgian National Number"
-msgstr "Chilijski numer podatkowy"
+msgstr "Belgijski numer krajowy"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Brazillian Company Identifier"
 msgstr "Brazylijski identyfikator przedsiębiorstw"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Brazillian National Identifier"
@@ -866,18 +861,17 @@
 msgid "Ecuadorian Personal Identity Code"
 msgstr "Ekwadorski osobisty kod identyfikacyjny"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Ecuadorian Tax Identification"
 msgstr "Ekwadorska identyfikacja podatkowa"
 
-#, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Egyptian Tax Registration Number"
-msgstr "PESEL"
+msgstr "Egipski numer rejestracji podatkowej"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "English Unique Pupil Number"
 msgstr "Angielski indywidualny numer ucznia (UPN)"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Estonian Organisation Registration Code"
@@ -893,235 +887,195 @@
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "European VAT Number"
 msgstr "VAT-UE"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "European VAT on e-Commerce - One Stop Shop"
-msgstr ""
+msgstr "Europejski VAT od handlu elektronicznego - One Stop Shop"
 
-#, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Faroese Tax Number"
-msgstr "NIP"
+msgstr "Numer podatkowy Wysp Owczych"
 
-#, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Finnish Association Identifier"
-msgstr "Brazylijski Identyfikator Narodowy"
+msgstr "Identyfikator fińskiego stowarzyszenia"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Finnish Business Identifier"
-msgstr ""
+msgstr "Fiński identyfikator biznesowy"
 
-#, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Finnish Individual Tax Number"
-msgstr "Nr podatkowy w Argentynie"
+msgstr "Fiński indywidualny numer podatkowy"
 
-#, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Finnish Personal Identity Code"
-msgstr "Bułgarskie Kody Tożsamości"
+msgstr "Fiński osobisty kod identyfikacyjny"
 
-#, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Finnish VAT Number"
-msgstr "NIP"
+msgstr "Fiński numer VAT"
 
-#, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "French Company Establishment Identification Number"
-msgstr "PESEL"
+msgstr "Francuski numer SIRET"
 
-#, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "French Company Identification Number"
-msgstr "PESEL"
+msgstr "Francuski numer SIREN"
 
-#, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "French Personal Identification Number"
-msgstr "PESEL"
+msgstr "Francuski osobisty numer identyfikacyjny"
 
-#, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "French Tax Identification Number"
-msgstr "PESEL"
+msgstr "Francuski numer identyfikacji podatkowej"
 
-#, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "French VAT Number"
-msgstr "VAT-UE"
+msgstr "Francuski numer VAT"
 
-#, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "German Company Register Number"
-msgstr "Austryjacki Rejestr Przedsiębiorstw"
+msgstr "Niemiecki numer rejestracyjny firmy"
 
-#, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "German Personal Tax Number"
-msgstr "Numer podatkowy w Andorze"
+msgstr "Niemiecki numer identyfikacji podatkowej"
 
-#, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "German Tax Number"
-msgstr "Numer podatkowy w Andorze"
+msgstr "Niemiecki numer podatkowy"
 
-#, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "German VAT Number"
-msgstr "VAT-UE"
+msgstr "Niemiecki numer VAT"
 
-#, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Ghanaian Taxpayer Identification Number"
-msgstr "PESEL"
+msgstr "Numer identyfikacyjny podatnika w Ghanie"
 
-#, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Greek Social Security Number"
-msgstr "Australijski Numer Przedsiębiorstwa"
+msgstr "Grecki numer ubezpieczenia społecznego"
 
-#, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Greek VAT Number"
-msgstr "VAT-UE"
+msgstr "Grecki numer VAT"
 
-#, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Guatemala Tax Number"
-msgstr "Australijski Numer Podatkowy"
+msgstr "Numer podatkowy w Gwatemali"
 
-#, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Guinean Tax Number"
-msgstr "Numer podatkowy w Andorze"
+msgstr "Numer podatkowy w Gwinei"
 
-#, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Hungarian VAT Number"
-msgstr "Bułgarski Numer VAT"
+msgstr "Węgierski numer VAT"
 
-#, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Icelandic Personal and Organisation Identity Code"
-msgstr "Bułgarskie Kody Tożsamości"
+msgstr "Islandzki kod identyfikacyjny osoby i organizacji"
 
-#, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Icelandic VAT Number"
-msgstr "Numer VAT w Albanii"
+msgstr "Numer VAT w Islandii"
 
-#, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Indian Digital Resident Personal Identity Number"
-msgstr "Brazylijski Identyfikator Narodowy"
+msgstr "Cyfrowy numer identyfikacyjny indyjskiego rezydenta"
 
-#, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Indian Income Tax Identifier"
-msgstr "Identyfikator podatkowy"
+msgstr "Identyfikator podatku dochodowego w Indiach"
 
-#, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Indian VAT number"
-msgstr "Numer VAT w Albanii"
+msgstr "Numer VAT w Indiach"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Indian Voter ID"
-msgstr ""
+msgstr "Indyjski identyfikator wyborcy"
 
-#, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Indonesian VAT Number"
-msgstr "Numer VAT w Albanii"
+msgstr "Numer VAT w Indonezji"
 
-#, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Irish Personal Number"
-msgstr "Australijski Numer Przedsiębiorstwa"
+msgstr "Irlandzki numer osobisty"
 
-#, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Irish VAT Number"
-msgstr "NIP"
+msgstr "Numer VAT w Irlandii"
 
-#, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Israeli Company Number"
-msgstr "Australijski Numer Przedsiębiorstwa"
+msgstr "Izraelski numer firmy"
 
-#, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Israeli Identity Number"
-msgstr "Australijski Numer Przedsiębiorstwa"
+msgstr "Izraelski numer identyfikacyjny"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Italian Tax Code for Individuals"
-msgstr ""
+msgstr "Włoski numer podatkowy dla osób fizycznych"
 
-#, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Italian VAT Number"
-msgstr "Numer VAT w Albanii"
+msgstr "Numer VAT we Włoszech"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Japanese Corporate Number"
-msgstr ""
+msgstr "Japoński numer przedsiębiorstwa"
 
-#, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Latvian VAT Number"
-msgstr "Numer VAT w Albanii"
+msgstr "Łotewski numer VAT"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Lithuanian Personal Number"
-msgstr ""
+msgstr "Litewski numer osobisty"
 
-#, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Lithuanian VAT Number"
-msgstr "Numer VAT w Albanii"
+msgstr "Litewski numer VAT"
 
-#, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Luxembourgian VAT Number"
-msgstr "Bułgarski Numer VAT"
+msgstr "Luksemburski numer VAT"
 
-#, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Macedonian Tax Number"
-msgstr "Nr podatkowy w Argentynie"
+msgstr "Macedoński numer podatkowy"
 
-#, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Malaysian National Registration Identity Card Number"
-msgstr "Brazylijski Identyfikator Narodowy"
+msgstr "Numer dowodu osobistego w malezyjskim rejestrze krajowym"
 
-#, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Maltese VAT Number"
-msgstr "NIP"
+msgstr "Maltański numer VAT"
 
-#, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Mauritian National Identifier"
-msgstr "Brazylijski Identyfikator Narodowy"
+msgstr "Identyfikator narodowy Mauritiusa"
 
-#, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Mexican Tax Number"
-msgstr "Nr podatkowy w Argentynie"
+msgstr "Meksykański numer podatkowy"
 
-#, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Moldavian Company Identification Number"
-msgstr "PESEL"
+msgstr "Numer identyfikacyjny mołdawskiego przedsiębiorstwa"
 
 #, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Monacan VAT Number"
 msgstr "Numer VAT w Albanii"
 
 #, fuzzy
@@ -1435,15 +1389,14 @@
 msgid "Skype"
 msgstr "Skype"
 
 msgctxt "selection:party.contact_mechanism,type:"
 msgid "Website"
 msgstr "Strona WWW"
 
-#, fuzzy
 msgctxt "view:party.address:"
 msgid "General"
 msgstr "Ogólne"
 
 msgctxt "view:party.party:"
 msgid "General"
 msgstr "Ogólne"
```

### Comparing `trytond_party-7.2.0/locale/pt.po` & `trytond_party-7.2.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_party-7.2.0/locale/ro.po` & `trytond_party-7.2.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_party-7.2.0/locale/ru.po` & `trytond_party-7.2.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_party-7.2.0/locale/sl.po` & `trytond_party-7.2.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_party-7.2.0/locale/tr.po` & `trytond_party-7.2.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_party-7.2.0/locale/uk.po` & `trytond_party-7.2.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_party-7.2.0/locale/zh_CN.po` & `trytond_party-7.2.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_party-7.2.0/message.xml` & `trytond_party-7.2.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_party-7.2.0/party.py` & `trytond_party-7.2.1/party.py`

 * *Files identical despite different names*

### Comparing `trytond_party-7.2.0/party.xml` & `trytond_party-7.2.1/party.xml`

 * *Files identical despite different names*

### Comparing `trytond_party-7.2.0/setup.py` & `trytond_party-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_party-7.2.0/tests/scenario_party_erase.rst` & `trytond_party-7.2.1/tests/scenario_party_erase.rst`

 * *Files identical despite different names*

### Comparing `trytond_party-7.2.0/tests/scenario_party_identifier_notifications.rst` & `trytond_party-7.2.1/tests/scenario_party_identifier_notifications.rst`

 * *Files identical despite different names*

### Comparing `trytond_party-7.2.0/tests/scenario_party_phone_number.rst` & `trytond_party-7.2.1/tests/scenario_party_phone_number.rst`

 * *Files identical despite different names*

### Comparing `trytond_party-7.2.0/tests/scenario_party_replace.rst` & `trytond_party-7.2.1/tests/scenario_party_replace.rst`

 * *Files identical despite different names*

### Comparing `trytond_party-7.2.0/tests/test_module.py` & `trytond_party-7.2.1/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_party-7.2.0/tox.ini` & `trytond_party-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_party-7.2.0/trytond_party.egg-info/PKG-INFO` & `trytond_party-7.2.1/trytond_party.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_party
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module with parties and addresses
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_party-7.2.0/trytond_party.egg-info/SOURCES.txt` & `trytond_party-7.2.1/trytond_party.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_party-7.2.0/view/address_form.xml` & `trytond_party-7.2.1/view/address_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_party-7.2.0/view/address_form_simple.xml` & `trytond_party-7.2.1/view/address_form_simple.xml`

 * *Files identical despite different names*

### Comparing `trytond_party-7.2.0/view/address_tree_sequence.xml` & `trytond_party-7.2.1/view/address_tree_sequence.xml`

 * *Files identical despite different names*

### Comparing `trytond_party-7.2.0/view/contact_mechanism_form.xml` & `trytond_party-7.2.1/view/contact_mechanism_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_party-7.2.0/view/contact_mechanism_tree_sequence.xml` & `trytond_party-7.2.1/view/contact_mechanism_tree_sequence.xml`

 * *Files identical despite different names*

### Comparing `trytond_party-7.2.0/view/identifier_form.xml` & `trytond_party-7.2.1/view/identifier_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_party-7.2.0/view/party_form.xml` & `trytond_party-7.2.1/view/party_form.xml`

 * *Files identical despite different names*

