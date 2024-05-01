# Comparing `tmp/trytond_purchase_request-7.2.0.tar.gz` & `tmp/trytond_purchase_request-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_purchase_request-7.2.0.tar", last modified: Mon Apr 29 15:46:12 2024, max compression
+gzip compressed data, was "trytond_purchase_request-7.2.1.tar", last modified: Wed May  1 11:35:57 2024, max compression
```

## Comparing `trytond_purchase_request-7.2.0.tar` & `trytond_purchase_request-7.2.1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:12.513705 trytond_purchase_request-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     2229 2024-04-29 15:24:00.000000 trytond_purchase_request-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      802 2024-04-29 15:24:00.000000 trytond_purchase_request-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_purchase_request-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_purchase_request-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3673 2024-04-29 15:46:12.513705 trytond_purchase_request-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1175 2023-04-15 07:12:15.000000 trytond_purchase_request-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      715 2023-04-15 07:12:15.000000 trytond_purchase_request-7.2.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:12.507039 trytond_purchase_request-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3079 2024-04-27 16:30:39.000000 trytond_purchase_request-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1175 2023-04-15 07:12:15.000000 trytond_purchase_request-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:21.000000 trytond_purchase_request-7.2.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      244 2023-04-15 07:12:15.000000 trytond_purchase_request-7.2.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:12.510372 trytond_purchase_request-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     6930 2024-04-27 16:43:26.000000 trytond_purchase_request-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7361 2024-04-27 16:43:26.000000 trytond_purchase_request-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6200 2024-04-27 16:43:26.000000 trytond_purchase_request-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7439 2024-04-27 16:43:26.000000 trytond_purchase_request-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7326 2024-04-27 16:43:26.000000 trytond_purchase_request-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6246 2024-04-27 16:43:26.000000 trytond_purchase_request-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6482 2024-04-27 16:43:26.000000 trytond_purchase_request-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7783 2024-04-27 16:43:26.000000 trytond_purchase_request-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6200 2024-04-27 16:43:26.000000 trytond_purchase_request-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7321 2024-04-27 16:43:26.000000 trytond_purchase_request-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6883 2024-04-27 16:43:26.000000 trytond_purchase_request-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6225 2024-04-27 16:43:26.000000 trytond_purchase_request-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7286 2024-04-27 16:43:26.000000 trytond_purchase_request-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6898 2024-04-27 16:43:26.000000 trytond_purchase_request-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6236 2024-04-27 16:43:26.000000 trytond_purchase_request-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7289 2024-04-27 16:43:26.000000 trytond_purchase_request-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6479 2024-04-27 16:43:26.000000 trytond_purchase_request-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7029 2024-04-27 16:43:26.000000 trytond_purchase_request-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7393 2024-04-29 13:17:17.000000 trytond_purchase_request-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7053 2024-04-27 16:43:26.000000 trytond_purchase_request-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6951 2024-04-27 16:43:26.000000 trytond_purchase_request-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6200 2024-04-27 16:43:26.000000 trytond_purchase_request-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5929 2024-04-27 16:43:26.000000 trytond_purchase_request-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6954 2024-04-27 16:43:26.000000 trytond_purchase_request-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1093 2023-04-15 07:12:15.000000 trytond_purchase_request-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      400 2023-04-15 07:12:15.000000 trytond_purchase_request-7.2.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3855 2024-04-22 12:14:36.000000 trytond_purchase_request-7.2.0/purchase.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1086 2024-02-04 18:51:26.000000 trytond_purchase_request-7.2.0/purchase.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    19606 2024-04-22 12:14:36.000000 trytond_purchase_request-7.2.0/purchase_request.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9229 2024-04-27 16:30:39.000000 trytond_purchase_request-7.2.0/purchase_request.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:46:12.513705 trytond_purchase_request-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4454 2024-03-17 11:01:36.000000 trytond_purchase_request-7.2.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:12.510372 trytond_purchase_request-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_purchase_request-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8378 2024-04-22 12:14:36.000000 trytond_purchase_request-7.2.0/tests/scenario_purchase_request.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      335 2024-01-29 09:46:02.000000 trytond_purchase_request-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_purchase_request-7.2.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:21.000000 trytond_purchase_request-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      127 2024-04-29 15:23:55.000000 trytond_purchase_request-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:12.513705 trytond_purchase_request-7.2.0/trytond_purchase_request.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3673 2024-04-29 15:46:12.000000 trytond_purchase_request-7.2.0/trytond_purchase_request.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2013 2024-04-29 15:46:12.000000 trytond_purchase_request-7.2.0/trytond_purchase_request.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:46:12.000000 trytond_purchase_request-7.2.0/trytond_purchase_request.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       70 2024-04-29 15:46:12.000000 trytond_purchase_request-7.2.0/trytond_purchase_request.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:00.000000 trytond_purchase_request-7.2.0/trytond_purchase_request.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      128 2024-04-29 15:46:12.000000 trytond_purchase_request-7.2.0/trytond_purchase_request.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:46:12.000000 trytond_purchase_request-7.2.0/trytond_purchase_request.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:12.513705 trytond_purchase_request-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      385 2023-04-15 07:12:15.000000 trytond_purchase_request-7.2.0/view/handle_purchase_cancellation_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      335 2023-01-16 14:00:21.000000 trytond_purchase_request-7.2.0/view/purchase_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      449 2023-01-16 14:00:21.000000 trytond_purchase_request-7.2.0/view/purchase_request_create_purchase_ask_party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1817 2024-02-04 18:51:26.000000 trytond_purchase_request-7.2.0/view/purchase_request_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      602 2024-03-17 13:11:55.000000 trytond_purchase_request-7.2.0/view/purchase_request_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:35:57.163672 trytond_purchase_request-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2330 2024-05-01 11:35:53.000000 trytond_purchase_request-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      802 2024-05-01 11:35:53.000000 trytond_purchase_request-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3673 2024-05-01 11:35:57.160339 trytond_purchase_request-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1175 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      715 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:35:57.157006 trytond_purchase_request-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3079 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1175 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      244 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:35:57.160339 trytond_purchase_request-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     6930 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7361 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6200 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7439 2024-04-30 17:21:59.000000 trytond_purchase_request-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7326 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6246 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6482 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7783 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6200 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7341 2024-04-30 17:21:59.000000 trytond_purchase_request-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6883 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6225 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7286 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6898 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6236 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7289 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6479 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7029 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7393 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7053 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6951 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6200 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5929 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6954 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1093 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      400 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3855 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/purchase.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1086 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/purchase.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    19606 2024-04-30 17:21:06.000000 trytond_purchase_request-7.2.1/purchase_request.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9229 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/purchase_request.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 11:35:57.163672 trytond_purchase_request-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4454 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:35:57.160339 trytond_purchase_request-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8378 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/tests/scenario_purchase_request.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      335 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      127 2024-04-30 17:21:06.000000 trytond_purchase_request-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:35:57.160339 trytond_purchase_request-7.2.1/trytond_purchase_request.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3673 2024-05-01 11:35:56.000000 trytond_purchase_request-7.2.1/trytond_purchase_request.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2013 2024-05-01 11:35:57.000000 trytond_purchase_request-7.2.1/trytond_purchase_request.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:35:56.000000 trytond_purchase_request-7.2.1/trytond_purchase_request.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       70 2024-05-01 11:35:56.000000 trytond_purchase_request-7.2.1/trytond_purchase_request.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:35:56.000000 trytond_purchase_request-7.2.1/trytond_purchase_request.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      128 2024-05-01 11:35:56.000000 trytond_purchase_request-7.2.1/trytond_purchase_request.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 11:35:56.000000 trytond_purchase_request-7.2.1/trytond_purchase_request.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:35:57.160339 trytond_purchase_request-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      385 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/view/handle_purchase_cancellation_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      335 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/view/purchase_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      449 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/view/purchase_request_create_purchase_ask_party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1817 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/view/purchase_request_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      602 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/view/purchase_request_tree.xml
```

### Comparing `trytond_purchase_request-7.2.0/CHANGELOG` & `trytond_purchase_request-7.2.1/CHANGELOG`

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
 
 Open purchases created from requests
 
 Version 7.0.0 - 2023-10-30
```

### Comparing `trytond_purchase_request-7.2.0/COPYRIGHT` & `trytond_purchase_request-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.0/LICENSE` & `trytond_purchase_request-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.0/PKG-INFO` & `trytond_purchase_request-7.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_purchase_request
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module for purchase requests
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_purchase_request-7.2.0/README.rst` & `trytond_purchase_request-7.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.0/__init__.py` & `trytond_purchase_request-7.2.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.0/doc/conf.py` & `trytond_purchase_request-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.0/doc/index.rst` & `trytond_purchase_request-7.2.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.0/locale/bg.po` & `trytond_purchase_request-7.2.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.0/locale/ca.po` & `trytond_purchase_request-7.2.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.0/locale/cs.po` & `trytond_purchase_request-7.2.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.0/locale/de.po` & `trytond_purchase_request-7.2.1/locale/de.po`

 * *Files 1% similar despite different names*

```diff
@@ -186,15 +186,15 @@
 msgctxt ""
 "model:ir.model.button,string:purchase_hande_purchase_cancellation_exception_button"
 msgid "Handle Purchase Cancellation"
 msgstr "Einkaufsannullierung bearbeiten"
 
 msgctxt "model:ir.rule.group,name:rule_group_purchase_request_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.ui.menu,name:menu_purchase_request_form"
 msgid "Purchase Requests"
 msgstr "Bestellvorschläge"
 
 msgctxt "model:purchase.request,name:"
 msgid "Purchase Request"
```

### Comparing `trytond_purchase_request-7.2.0/locale/es.po` & `trytond_purchase_request-7.2.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.0/locale/es_419.po` & `trytond_purchase_request-7.2.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.0/locale/et.po` & `trytond_purchase_request-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.0/locale/fa.po` & `trytond_purchase_request-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.0/locale/fi.po` & `trytond_purchase_request-7.2.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.0/locale/fr.po` & `trytond_purchase_request-7.2.1/locale/fr.po`

 * *Files 0% similar despite different names*

```diff
@@ -164,16 +164,16 @@
 msgctxt "model:ir.message,text:msg_purchase_request_warehouse"
 msgid ""
 "Warehouse \"%(purchase_warehouse)s\" on purchase \"%(purchase)s\" is "
 "different to warehouse \"%(request_warehouse)s\" on linked purchase request "
 "\"%(request)s\"."
 msgstr ""
 "L'entrepôt « %(purchase_warehouse)s » de l'achat « %(purchase)s » est "
-"différent de l'entrepôt « %(request_warehouse)s » de la demande d'achat "
-"liée."
+"différent de l'entrepôt « %(request_warehouse)s » de la demande d'achat liée"
+" « %(request)s »."
 
 msgctxt "model:ir.message,text:msg_request_delete_purchased"
 msgid ""
 "You cannot delete purchase request \"%(request)s\" because it is purchased."
 msgstr ""
 "Vous ne pouvez pas supprimer la demande d'achat « %(request)s » car elle est"
 " achetée."
```

### Comparing `trytond_purchase_request-7.2.0/locale/hu.po` & `trytond_purchase_request-7.2.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.0/locale/id.po` & `trytond_purchase_request-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.0/locale/it.po` & `trytond_purchase_request-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.0/locale/lo.po` & `trytond_purchase_request-7.2.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.0/locale/lt.po` & `trytond_purchase_request-7.2.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.0/locale/nl.po` & `trytond_purchase_request-7.2.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.0/locale/pl.po` & `trytond_purchase_request-7.2.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.0/locale/pt.po` & `trytond_purchase_request-7.2.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.0/locale/ro.po` & `trytond_purchase_request-7.2.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.0/locale/ru.po` & `trytond_purchase_request-7.2.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.0/locale/sl.po` & `trytond_purchase_request-7.2.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.0/locale/tr.po` & `trytond_purchase_request-7.2.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.0/locale/uk.po` & `trytond_purchase_request-7.2.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.0/locale/zh_CN.po` & `trytond_purchase_request-7.2.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.0/message.xml` & `trytond_purchase_request-7.2.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.0/purchase.py` & `trytond_purchase_request-7.2.1/purchase.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.0/purchase.xml` & `trytond_purchase_request-7.2.1/purchase.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.0/purchase_request.py` & `trytond_purchase_request-7.2.1/purchase_request.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.0/purchase_request.xml` & `trytond_purchase_request-7.2.1/purchase_request.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.0/setup.py` & `trytond_purchase_request-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.0/tests/scenario_purchase_request.rst` & `trytond_purchase_request-7.2.1/tests/scenario_purchase_request.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.0/tox.ini` & `trytond_purchase_request-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.0/trytond_purchase_request.egg-info/PKG-INFO` & `trytond_purchase_request-7.2.1/trytond_purchase_request.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_purchase_request
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module for purchase requests
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_purchase_request-7.2.0/trytond_purchase_request.egg-info/SOURCES.txt` & `trytond_purchase_request-7.2.1/trytond_purchase_request.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.0/view/purchase_request_form.xml` & `trytond_purchase_request-7.2.1/view/purchase_request_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.0/view/purchase_request_tree.xml` & `trytond_purchase_request-7.2.1/view/purchase_request_tree.xml`

 * *Files identical despite different names*

