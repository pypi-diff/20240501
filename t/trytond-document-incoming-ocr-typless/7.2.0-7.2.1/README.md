# Comparing `tmp/trytond_document_incoming_ocr_typless-7.2.0.tar.gz` & `tmp/trytond_document_incoming_ocr_typless-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_document_incoming_ocr_typless-7.2.0.tar", last modified: Mon Apr 29 15:40:35 2024, max compression
+gzip compressed data, was "trytond_document_incoming_ocr_typless-7.2.1.tar", last modified: Wed May  1 11:58:55 2024, max compression
```

## Comparing `trytond_document_incoming_ocr_typless-7.2.0.tar` & `trytond_document_incoming_ocr_typless-7.2.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:35.355857 trytond_document_incoming_ocr_typless-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      172 2024-04-29 15:19:51.000000 trytond_document_incoming_ocr_typless-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:19:51.000000 trytond_document_incoming_ocr_typless-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-02-04 18:51:26.000000 trytond_document_incoming_ocr_typless-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-02-04 18:51:26.000000 trytond_document_incoming_ocr_typless-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2956 2024-04-29 15:40:35.355857 trytond_document_incoming_ocr_typless-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      277 2024-02-04 18:51:26.000000 trytond_document_incoming_ocr_typless-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      360 2024-02-04 18:51:26.000000 trytond_document_incoming_ocr_typless-7.2.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:35.352523 trytond_document_incoming_ocr_typless-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3092 2024-04-27 16:30:39.000000 trytond_document_incoming_ocr_typless-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      277 2024-02-04 18:51:26.000000 trytond_document_incoming_ocr_typless-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-02-04 18:51:26.000000 trytond_document_incoming_ocr_typless-7.2.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:10.000000 trytond_document_incoming_ocr_typless-7.2.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     2357 2024-02-04 18:51:26.000000 trytond_document_incoming_ocr_typless-7.2.0/doc/setup.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    11741 2024-03-25 13:26:54.000000 trytond_document_incoming_ocr_typless-7.2.0/document.py
--rw-r--r--   0 ced       (1000) ced       (1000)      560 2024-02-04 18:51:26.000000 trytond_document_incoming_ocr_typless-7.2.0/document.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      228 2024-03-25 13:26:54.000000 trytond_document_incoming_ocr_typless-7.2.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:35.352523 trytond_document_incoming_ocr_typless-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      757 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr_typless-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)      977 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr_typless-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      757 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr_typless-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)      973 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr_typless-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)      994 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr_typless-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      757 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr_typless-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      757 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr_typless-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)      757 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr_typless-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      757 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr_typless-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)      986 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr_typless-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      757 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr_typless-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      757 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr_typless-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)      950 2024-04-29 13:17:17.000000 trytond_document_incoming_ocr_typless-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)      757 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr_typless-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      757 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr_typless-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      988 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr_typless-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      757 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr_typless-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      757 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr_typless-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      757 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr_typless-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      757 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr_typless-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      799 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr_typless-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      757 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr_typless-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      757 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr_typless-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      757 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr_typless-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      428 2024-03-25 13:26:54.000000 trytond_document_incoming_ocr_typless-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:40:35.355857 trytond_document_incoming_ocr_typless-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4852 2024-04-27 16:30:39.000000 trytond_document_incoming_ocr_typless-7.2.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:35.352523 trytond_document_incoming_ocr_typless-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-02-04 18:51:26.000000 trytond_document_incoming_ocr_typless-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4017 2024-04-22 12:14:36.000000 trytond_document_incoming_ocr_typless-7.2.0/tests/scenario_document_incoming_ocr_typless.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    24399 2024-02-04 18:51:26.000000 trytond_document_incoming_ocr_typless-7.2.0/tests/supplier-invoice-sample.pdf
--rw-r--r--   0 ced       (1000) ced       (1000)     1091 2024-02-04 18:51:26.000000 trytond_document_incoming_ocr_typless-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      396 2024-02-04 18:51:26.000000 trytond_document_incoming_ocr_typless-7.2.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:10.000000 trytond_document_incoming_ocr_typless-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      193 2024-04-29 15:19:47.000000 trytond_document_incoming_ocr_typless-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:35.355857 trytond_document_incoming_ocr_typless-7.2.0/trytond_document_incoming_ocr_typless.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2956 2024-04-29 15:40:34.000000 trytond_document_incoming_ocr_typless-7.2.0/trytond_document_incoming_ocr_typless.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1813 2024-04-29 15:40:35.000000 trytond_document_incoming_ocr_typless-7.2.0/trytond_document_incoming_ocr_typless.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:40:34.000000 trytond_document_incoming_ocr_typless-7.2.0/trytond_document_incoming_ocr_typless.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       96 2024-04-29 15:40:34.000000 trytond_document_incoming_ocr_typless-7.2.0/trytond_document_incoming_ocr_typless.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:30:04.000000 trytond_document_incoming_ocr_typless-7.2.0/trytond_document_incoming_ocr_typless.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      224 2024-04-29 15:40:34.000000 trytond_document_incoming_ocr_typless-7.2.0/trytond_document_incoming_ocr_typless.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:40:34.000000 trytond_document_incoming_ocr_typless-7.2.0/trytond_document_incoming_ocr_typless.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:35.355857 trytond_document_incoming_ocr_typless-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      492 2024-02-04 18:51:26.000000 trytond_document_incoming_ocr_typless-7.2.0/view/document_incoming_ocr_service_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:58:55.630953 trytond_document_incoming_ocr_typless-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)      273 2024-05-01 11:58:52.000000 trytond_document_incoming_ocr_typless-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-05-01 11:58:52.000000 trytond_document_incoming_ocr_typless-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr_typless-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr_typless-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2956 2024-05-01 11:58:55.630953 trytond_document_incoming_ocr_typless-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      277 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr_typless-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      360 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr_typless-7.2.1/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:58:55.624286 trytond_document_incoming_ocr_typless-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3092 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr_typless-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      277 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr_typless-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr_typless-7.2.1/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr_typless-7.2.1/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     2357 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr_typless-7.2.1/doc/setup.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    11741 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr_typless-7.2.1/document.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      560 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr_typless-7.2.1/document.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      228 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr_typless-7.2.1/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:58:55.627620 trytond_document_incoming_ocr_typless-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)      757 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr_typless-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      977 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr_typless-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      757 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr_typless-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      973 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr_typless-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      994 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr_typless-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      757 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr_typless-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      757 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr_typless-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      757 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr_typless-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      757 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr_typless-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      976 2024-04-30 17:21:59.000000 trytond_document_incoming_ocr_typless-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      757 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr_typless-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      757 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr_typless-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      950 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr_typless-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      757 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr_typless-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      757 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr_typless-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      988 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr_typless-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      757 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr_typless-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      757 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr_typless-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      757 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr_typless-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      757 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr_typless-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      799 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr_typless-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      757 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr_typless-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      757 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr_typless-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      757 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr_typless-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      428 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr_typless-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 11:58:55.630953 trytond_document_incoming_ocr_typless-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4852 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr_typless-7.2.1/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:58:55.627620 trytond_document_incoming_ocr_typless-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr_typless-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4017 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr_typless-7.2.1/tests/scenario_document_incoming_ocr_typless.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    24399 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr_typless-7.2.1/tests/supplier-invoice-sample.pdf
+-rw-r--r--   0 ced       (1000) ced       (1000)     1091 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr_typless-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      396 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr_typless-7.2.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr_typless-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      193 2024-04-30 17:21:06.000000 trytond_document_incoming_ocr_typless-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:58:55.627620 trytond_document_incoming_ocr_typless-7.2.1/trytond_document_incoming_ocr_typless.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2956 2024-05-01 11:58:55.000000 trytond_document_incoming_ocr_typless-7.2.1/trytond_document_incoming_ocr_typless.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1813 2024-05-01 11:58:55.000000 trytond_document_incoming_ocr_typless-7.2.1/trytond_document_incoming_ocr_typless.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:58:55.000000 trytond_document_incoming_ocr_typless-7.2.1/trytond_document_incoming_ocr_typless.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       96 2024-05-01 11:58:55.000000 trytond_document_incoming_ocr_typless-7.2.1/trytond_document_incoming_ocr_typless.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:58:55.000000 trytond_document_incoming_ocr_typless-7.2.1/trytond_document_incoming_ocr_typless.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      224 2024-05-01 11:58:55.000000 trytond_document_incoming_ocr_typless-7.2.1/trytond_document_incoming_ocr_typless.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 11:58:55.000000 trytond_document_incoming_ocr_typless-7.2.1/trytond_document_incoming_ocr_typless.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:58:55.627620 trytond_document_incoming_ocr_typless-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      492 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr_typless-7.2.1/view/document_incoming_ocr_service_form.xml
```

### Comparing `trytond_document_incoming_ocr_typless-7.2.0/COPYRIGHT` & `trytond_document_incoming_ocr_typless-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr_typless-7.2.0/LICENSE` & `trytond_document_incoming_ocr_typless-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr_typless-7.2.0/PKG-INFO` & `trytond_document_incoming_ocr_typless-7.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_document_incoming_ocr_typless
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module that integrates Typless OCR for incoming document
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_document_incoming_ocr_typless-7.2.0/doc/conf.py` & `trytond_document_incoming_ocr_typless-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr_typless-7.2.0/doc/setup.rst` & `trytond_document_incoming_ocr_typless-7.2.1/doc/setup.rst`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr_typless-7.2.0/document.py` & `trytond_document_incoming_ocr_typless-7.2.1/document.py`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr_typless-7.2.0/document.xml` & `trytond_document_incoming_ocr_typless-7.2.1/document.xml`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr_typless-7.2.0/locale/bg.po` & `trytond_document_incoming_ocr_typless-7.2.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr_typless-7.2.0/locale/ca.po` & `trytond_document_incoming_ocr_typless-7.2.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr_typless-7.2.0/locale/cs.po` & `trytond_document_incoming_ocr_typless-7.2.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr_typless-7.2.0/locale/de.po` & `trytond_document_incoming_ocr_typless-7.2.1/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr_typless-7.2.0/locale/es.po` & `trytond_document_incoming_ocr_typless-7.2.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr_typless-7.2.0/locale/es_419.po` & `trytond_document_incoming_ocr_typless-7.2.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr_typless-7.2.0/locale/et.po` & `trytond_document_incoming_ocr_typless-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr_typless-7.2.0/locale/fa.po` & `trytond_document_incoming_ocr_typless-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr_typless-7.2.0/locale/fi.po` & `trytond_document_incoming_ocr_typless-7.2.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr_typless-7.2.0/locale/fr.po` & `trytond_document_incoming_ocr_typless-7.2.1/locale/fr.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #
-#, fuzzy
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:document.incoming.ocr.service,typless_api_key:"
 msgid "API Key"
 msgstr "Clé API"
 
@@ -21,12 +20,12 @@
 
 msgctxt "model:ir.message,text:msg_typless_webserver_error"
 msgid ""
 "Typless webservice call failed with the following error message:\n"
 "%(message)s"
 msgstr ""
 "L'appel au service Web Typless a échoué avec le message d'erreur suivant :\n"
-"%(messages)s"
+"%(message)s"
 
 msgctxt "selection:document.incoming.ocr.service,type:"
 msgid "Typless"
 msgstr "Typless"
```

### Comparing `trytond_document_incoming_ocr_typless-7.2.0/locale/hu.po` & `trytond_document_incoming_ocr_typless-7.2.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr_typless-7.2.0/locale/id.po` & `trytond_document_incoming_ocr_typless-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr_typless-7.2.0/locale/it.po` & `trytond_document_incoming_ocr_typless-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr_typless-7.2.0/locale/lo.po` & `trytond_document_incoming_ocr_typless-7.2.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr_typless-7.2.0/locale/lt.po` & `trytond_document_incoming_ocr_typless-7.2.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr_typless-7.2.0/locale/nl.po` & `trytond_document_incoming_ocr_typless-7.2.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr_typless-7.2.0/locale/pl.po` & `trytond_document_incoming_ocr_typless-7.2.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr_typless-7.2.0/locale/pt.po` & `trytond_document_incoming_ocr_typless-7.2.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr_typless-7.2.0/locale/ro.po` & `trytond_document_incoming_ocr_typless-7.2.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr_typless-7.2.0/locale/ru.po` & `trytond_document_incoming_ocr_typless-7.2.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr_typless-7.2.0/locale/sl.po` & `trytond_document_incoming_ocr_typless-7.2.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr_typless-7.2.0/locale/tr.po` & `trytond_document_incoming_ocr_typless-7.2.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr_typless-7.2.0/locale/uk.po` & `trytond_document_incoming_ocr_typless-7.2.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr_typless-7.2.0/locale/zh_CN.po` & `trytond_document_incoming_ocr_typless-7.2.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr_typless-7.2.0/setup.py` & `trytond_document_incoming_ocr_typless-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr_typless-7.2.0/tests/scenario_document_incoming_ocr_typless.rst` & `trytond_document_incoming_ocr_typless-7.2.1/tests/scenario_document_incoming_ocr_typless.rst`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr_typless-7.2.0/tests/supplier-invoice-sample.pdf` & `trytond_document_incoming_ocr_typless-7.2.1/tests/supplier-invoice-sample.pdf`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr_typless-7.2.0/tests/test_module.py` & `trytond_document_incoming_ocr_typless-7.2.1/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr_typless-7.2.0/tox.ini` & `trytond_document_incoming_ocr_typless-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr_typless-7.2.0/trytond_document_incoming_ocr_typless.egg-info/PKG-INFO` & `trytond_document_incoming_ocr_typless-7.2.1/trytond_document_incoming_ocr_typless.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_document_incoming_ocr_typless
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module that integrates Typless OCR for incoming document
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_document_incoming_ocr_typless-7.2.0/trytond_document_incoming_ocr_typless.egg-info/SOURCES.txt` & `trytond_document_incoming_ocr_typless-7.2.1/trytond_document_incoming_ocr_typless.egg-info/SOURCES.txt`

 * *Files identical despite different names*

