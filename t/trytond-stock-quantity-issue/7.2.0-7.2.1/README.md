# Comparing `tmp/trytond_stock_quantity_issue-7.2.0.tar.gz` & `tmp/trytond_stock_quantity_issue-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_stock_quantity_issue-7.2.0.tar", last modified: Mon Apr 29 15:52:42 2024, max compression
+gzip compressed data, was "trytond_stock_quantity_issue-7.2.1.tar", last modified: Wed May  1 09:54:32 2024, max compression
```

## Comparing `trytond_stock_quantity_issue-7.2.0.tar` & `trytond_stock_quantity_issue-7.2.1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:52:42.310177 trytond_stock_quantity_issue-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      828 2024-04-29 15:28:50.000000 trytond_stock_quantity_issue-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      651 2024-04-29 15:28:50.000000 trytond_stock_quantity_issue-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_stock_quantity_issue-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_stock_quantity_issue-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2811 2024-04-29 15:52:42.310177 trytond_stock_quantity_issue-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      220 2023-04-15 07:12:15.000000 trytond_stock_quantity_issue-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      686 2023-04-15 07:12:15.000000 trytond_stock_quantity_issue-7.2.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:52:42.306844 trytond_stock_quantity_issue-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3083 2024-04-27 16:30:39.000000 trytond_stock_quantity_issue-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1555 2023-04-15 07:12:15.000000 trytond_stock_quantity_issue-7.2.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      220 2023-04-15 07:12:15.000000 trytond_stock_quantity_issue-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_stock_quantity_issue-7.2.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:35.000000 trytond_stock_quantity_issue-7.2.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      331 2023-04-15 07:12:15.000000 trytond_stock_quantity_issue-7.2.0/doc/usage.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      233 2023-04-15 07:12:15.000000 trytond_stock_quantity_issue-7.2.0/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)      476 2023-04-15 07:12:15.000000 trytond_stock_quantity_issue-7.2.0/ir.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:52:42.310177 trytond_stock_quantity_issue-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     4142 2024-04-27 16:43:28.000000 trytond_stock_quantity_issue-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5075 2024-04-27 16:43:28.000000 trytond_stock_quantity_issue-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4142 2024-04-27 16:43:28.000000 trytond_stock_quantity_issue-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5086 2024-04-27 16:43:28.000000 trytond_stock_quantity_issue-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5098 2024-04-27 16:43:28.000000 trytond_stock_quantity_issue-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4142 2024-04-27 16:43:28.000000 trytond_stock_quantity_issue-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4142 2024-04-27 16:43:28.000000 trytond_stock_quantity_issue-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4142 2024-04-27 16:43:28.000000 trytond_stock_quantity_issue-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4142 2024-04-27 16:43:28.000000 trytond_stock_quantity_issue-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5158 2024-04-27 16:43:28.000000 trytond_stock_quantity_issue-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4142 2024-04-27 16:43:28.000000 trytond_stock_quantity_issue-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4188 2024-04-27 16:43:28.000000 trytond_stock_quantity_issue-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4167 2024-04-27 16:43:28.000000 trytond_stock_quantity_issue-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4142 2024-04-27 16:43:28.000000 trytond_stock_quantity_issue-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4142 2024-04-27 16:43:28.000000 trytond_stock_quantity_issue-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5158 2024-04-27 16:43:28.000000 trytond_stock_quantity_issue-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4142 2024-04-27 16:43:28.000000 trytond_stock_quantity_issue-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4142 2024-04-27 16:43:28.000000 trytond_stock_quantity_issue-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4142 2024-04-27 16:43:28.000000 trytond_stock_quantity_issue-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4142 2024-04-27 16:43:28.000000 trytond_stock_quantity_issue-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4154 2024-04-27 16:43:28.000000 trytond_stock_quantity_issue-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4142 2024-04-27 16:43:28.000000 trytond_stock_quantity_issue-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4142 2024-04-27 16:43:28.000000 trytond_stock_quantity_issue-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4142 2024-04-27 16:43:28.000000 trytond_stock_quantity_issue-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      480 2023-04-15 07:12:15.000000 trytond_stock_quantity_issue-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      489 2023-04-15 07:12:15.000000 trytond_stock_quantity_issue-7.2.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:52:42.310177 trytond_stock_quantity_issue-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4758 2024-04-27 16:30:39.000000 trytond_stock_quantity_issue-7.2.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)    14852 2024-01-27 09:58:52.000000 trytond_stock_quantity_issue-7.2.0/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6381 2024-04-27 16:30:39.000000 trytond_stock_quantity_issue-7.2.0/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:52:42.310177 trytond_stock_quantity_issue-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_stock_quantity_issue-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4325 2024-04-22 12:14:36.000000 trytond_stock_quantity_issue-7.2.0/tests/scenario_stock_quantity_issue.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      451 2023-04-15 07:12:15.000000 trytond_stock_quantity_issue-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_stock_quantity_issue-7.2.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:35.000000 trytond_stock_quantity_issue-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      154 2024-04-29 15:28:46.000000 trytond_stock_quantity_issue-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:52:42.310177 trytond_stock_quantity_issue-7.2.0/trytond_stock_quantity_issue.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2811 2024-04-29 15:52:41.000000 trytond_stock_quantity_issue-7.2.0/trytond_stock_quantity_issue.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1871 2024-04-29 15:52:42.000000 trytond_stock_quantity_issue-7.2.0/trytond_stock_quantity_issue.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:52:41.000000 trytond_stock_quantity_issue-7.2.0/trytond_stock_quantity_issue.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       78 2024-04-29 15:52:41.000000 trytond_stock_quantity_issue-7.2.0/trytond_stock_quantity_issue.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:05.000000 trytond_stock_quantity_issue-7.2.0/trytond_stock_quantity_issue.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      149 2024-04-29 15:52:41.000000 trytond_stock_quantity_issue-7.2.0/trytond_stock_quantity_issue.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:52:41.000000 trytond_stock_quantity_issue-7.2.0/trytond_stock_quantity_issue.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:52:42.310177 trytond_stock_quantity_issue-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      367 2023-04-15 07:12:15.000000 trytond_stock_quantity_issue-7.2.0/view/product_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1349 2023-04-15 07:12:15.000000 trytond_stock_quantity_issue-7.2.0/view/quantity_issue_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      407 2023-04-15 07:12:15.000000 trytond_stock_quantity_issue-7.2.0/view/quantity_issue_generate_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      335 2023-04-15 07:12:15.000000 trytond_stock_quantity_issue-7.2.0/view/quantity_issue_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:54:32.881060 trytond_stock_quantity_issue-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)      929 2024-05-01 09:54:29.000000 trytond_stock_quantity_issue-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      651 2024-05-01 09:54:29.000000 trytond_stock_quantity_issue-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:21:00.000000 trytond_stock_quantity_issue-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:21:00.000000 trytond_stock_quantity_issue-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2811 2024-05-01 09:54:32.881060 trytond_stock_quantity_issue-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      220 2024-04-30 17:21:00.000000 trytond_stock_quantity_issue-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      686 2024-04-30 17:21:00.000000 trytond_stock_quantity_issue-7.2.1/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:54:32.874393 trytond_stock_quantity_issue-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3083 2024-04-30 17:21:00.000000 trytond_stock_quantity_issue-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1555 2024-04-30 17:21:00.000000 trytond_stock_quantity_issue-7.2.1/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      220 2024-04-30 17:21:00.000000 trytond_stock_quantity_issue-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-30 17:21:00.000000 trytond_stock_quantity_issue-7.2.1/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:21:00.000000 trytond_stock_quantity_issue-7.2.1/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      331 2024-04-30 17:21:00.000000 trytond_stock_quantity_issue-7.2.1/doc/usage.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      233 2024-04-30 17:21:00.000000 trytond_stock_quantity_issue-7.2.1/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      476 2024-04-30 17:21:00.000000 trytond_stock_quantity_issue-7.2.1/ir.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:54:32.874393 trytond_stock_quantity_issue-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4142 2024-04-30 17:21:00.000000 trytond_stock_quantity_issue-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5075 2024-04-30 17:21:00.000000 trytond_stock_quantity_issue-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4142 2024-04-30 17:21:00.000000 trytond_stock_quantity_issue-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5086 2024-04-30 17:21:59.000000 trytond_stock_quantity_issue-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5098 2024-04-30 17:21:00.000000 trytond_stock_quantity_issue-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4142 2024-04-30 17:21:00.000000 trytond_stock_quantity_issue-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4142 2024-04-30 17:21:00.000000 trytond_stock_quantity_issue-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4142 2024-04-30 17:21:00.000000 trytond_stock_quantity_issue-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4142 2024-04-30 17:21:00.000000 trytond_stock_quantity_issue-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5158 2024-04-30 17:21:00.000000 trytond_stock_quantity_issue-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4142 2024-04-30 17:21:00.000000 trytond_stock_quantity_issue-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4188 2024-04-30 17:21:00.000000 trytond_stock_quantity_issue-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4167 2024-04-30 17:21:00.000000 trytond_stock_quantity_issue-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4142 2024-04-30 17:21:00.000000 trytond_stock_quantity_issue-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4142 2024-04-30 17:21:00.000000 trytond_stock_quantity_issue-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5158 2024-04-30 17:21:00.000000 trytond_stock_quantity_issue-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4142 2024-04-30 17:21:00.000000 trytond_stock_quantity_issue-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4142 2024-04-30 17:21:00.000000 trytond_stock_quantity_issue-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4142 2024-04-30 17:21:00.000000 trytond_stock_quantity_issue-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4142 2024-04-30 17:21:00.000000 trytond_stock_quantity_issue-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4154 2024-04-30 17:21:00.000000 trytond_stock_quantity_issue-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4142 2024-04-30 17:21:00.000000 trytond_stock_quantity_issue-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4142 2024-04-30 17:21:00.000000 trytond_stock_quantity_issue-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4142 2024-04-30 17:21:00.000000 trytond_stock_quantity_issue-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      480 2024-04-30 17:21:00.000000 trytond_stock_quantity_issue-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      489 2024-04-30 17:21:00.000000 trytond_stock_quantity_issue-7.2.1/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 09:54:32.881060 trytond_stock_quantity_issue-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4758 2024-04-30 17:21:00.000000 trytond_stock_quantity_issue-7.2.1/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    14852 2024-04-30 17:21:00.000000 trytond_stock_quantity_issue-7.2.1/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6381 2024-04-30 17:21:00.000000 trytond_stock_quantity_issue-7.2.1/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:54:32.874393 trytond_stock_quantity_issue-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:21:00.000000 trytond_stock_quantity_issue-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4325 2024-04-30 17:21:00.000000 trytond_stock_quantity_issue-7.2.1/tests/scenario_stock_quantity_issue.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      451 2024-04-30 17:21:00.000000 trytond_stock_quantity_issue-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:21:00.000000 trytond_stock_quantity_issue-7.2.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:21:00.000000 trytond_stock_quantity_issue-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      154 2024-04-30 17:21:06.000000 trytond_stock_quantity_issue-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:54:32.874393 trytond_stock_quantity_issue-7.2.1/trytond_stock_quantity_issue.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2811 2024-05-01 09:54:32.000000 trytond_stock_quantity_issue-7.2.1/trytond_stock_quantity_issue.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1871 2024-05-01 09:54:32.000000 trytond_stock_quantity_issue-7.2.1/trytond_stock_quantity_issue.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 09:54:32.000000 trytond_stock_quantity_issue-7.2.1/trytond_stock_quantity_issue.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       78 2024-05-01 09:54:32.000000 trytond_stock_quantity_issue-7.2.1/trytond_stock_quantity_issue.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 09:54:32.000000 trytond_stock_quantity_issue-7.2.1/trytond_stock_quantity_issue.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      149 2024-05-01 09:54:32.000000 trytond_stock_quantity_issue-7.2.1/trytond_stock_quantity_issue.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 09:54:32.000000 trytond_stock_quantity_issue-7.2.1/trytond_stock_quantity_issue.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:54:32.874393 trytond_stock_quantity_issue-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      367 2024-04-30 17:21:00.000000 trytond_stock_quantity_issue-7.2.1/view/product_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1349 2024-04-30 17:21:00.000000 trytond_stock_quantity_issue-7.2.1/view/quantity_issue_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      407 2024-04-30 17:21:00.000000 trytond_stock_quantity_issue-7.2.1/view/quantity_issue_generate_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      335 2024-04-30 17:21:00.000000 trytond_stock_quantity_issue-7.2.1/view/quantity_issue_list.xml
```

### Comparing `trytond_stock_quantity_issue-7.2.0/CHANGELOG` & `trytond_stock_quantity_issue-7.2.1/CHANGELOG`

 * *Files 7% similar despite different names*

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

### Comparing `trytond_stock_quantity_issue-7.2.0/COPYRIGHT` & `trytond_stock_quantity_issue-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_issue-7.2.0/LICENSE` & `trytond_stock_quantity_issue-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_issue-7.2.0/PKG-INFO` & `trytond_stock_quantity_issue-7.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_stock_quantity_issue
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module to manage quantity issue with stock
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_stock_quantity_issue-7.2.0/__init__.py` & `trytond_stock_quantity_issue-7.2.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_issue-7.2.0/doc/conf.py` & `trytond_stock_quantity_issue-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_issue-7.2.0/doc/design.rst` & `trytond_stock_quantity_issue-7.2.1/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_issue-7.2.0/locale/bg.po` & `trytond_stock_quantity_issue-7.2.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_issue-7.2.0/locale/ca.po` & `trytond_stock_quantity_issue-7.2.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_issue-7.2.0/locale/cs.po` & `trytond_stock_quantity_issue-7.2.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_issue-7.2.0/locale/de.po` & `trytond_stock_quantity_issue-7.2.1/locale/de.po`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,15 @@
 
 msgctxt "model:ir.model.button,string:quantity_issue_solve_button"
 msgid "Solve"
 msgstr "Beheben"
 
 msgctxt "model:ir.rule.group,name:rule_group_quantity_issue_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.ui.menu,name:menu_quantity_issue_form"
 msgid "Quantity Issues"
 msgstr "Verfügbarkeitsprobleme"
 
 msgctxt "model:ir.ui.menu,name:menu_quantity_issue_generate"
 msgid "Generate Stock Quantity Issues"
```

### Comparing `trytond_stock_quantity_issue-7.2.0/locale/es.po` & `trytond_stock_quantity_issue-7.2.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_issue-7.2.0/locale/es_419.po` & `trytond_stock_quantity_issue-7.2.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_issue-7.2.0/locale/et.po` & `trytond_stock_quantity_issue-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_issue-7.2.0/locale/fa.po` & `trytond_stock_quantity_issue-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_issue-7.2.0/locale/fi.po` & `trytond_stock_quantity_issue-7.2.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_issue-7.2.0/locale/fr.po` & `trytond_stock_quantity_issue-7.2.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_issue-7.2.0/locale/hu.po` & `trytond_stock_quantity_issue-7.2.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_issue-7.2.0/locale/id.po` & `trytond_stock_quantity_issue-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_issue-7.2.0/locale/it.po` & `trytond_stock_quantity_issue-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_issue-7.2.0/locale/lo.po` & `trytond_stock_quantity_issue-7.2.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_issue-7.2.0/locale/lt.po` & `trytond_stock_quantity_issue-7.2.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_issue-7.2.0/locale/nl.po` & `trytond_stock_quantity_issue-7.2.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_issue-7.2.0/locale/pl.po` & `trytond_stock_quantity_issue-7.2.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_issue-7.2.0/locale/pt.po` & `trytond_stock_quantity_issue-7.2.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_issue-7.2.0/locale/ro.po` & `trytond_stock_quantity_issue-7.2.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_issue-7.2.0/locale/ru.po` & `trytond_stock_quantity_issue-7.2.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_issue-7.2.0/locale/sl.po` & `trytond_stock_quantity_issue-7.2.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_issue-7.2.0/locale/tr.po` & `trytond_stock_quantity_issue-7.2.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_issue-7.2.0/locale/uk.po` & `trytond_stock_quantity_issue-7.2.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_issue-7.2.0/locale/zh_CN.po` & `trytond_stock_quantity_issue-7.2.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_issue-7.2.0/setup.py` & `trytond_stock_quantity_issue-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_issue-7.2.0/stock.py` & `trytond_stock_quantity_issue-7.2.1/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_issue-7.2.0/stock.xml` & `trytond_stock_quantity_issue-7.2.1/stock.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_issue-7.2.0/tests/scenario_stock_quantity_issue.rst` & `trytond_stock_quantity_issue-7.2.1/tests/scenario_stock_quantity_issue.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_issue-7.2.0/tox.ini` & `trytond_stock_quantity_issue-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_issue-7.2.0/trytond_stock_quantity_issue.egg-info/PKG-INFO` & `trytond_stock_quantity_issue-7.2.1/trytond_stock_quantity_issue.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_stock_quantity_issue
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module to manage quantity issue with stock
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_stock_quantity_issue-7.2.0/trytond_stock_quantity_issue.egg-info/SOURCES.txt` & `trytond_stock_quantity_issue-7.2.1/trytond_stock_quantity_issue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_issue-7.2.0/view/quantity_issue_form.xml` & `trytond_stock_quantity_issue-7.2.1/view/quantity_issue_form.xml`

 * *Files identical despite different names*

