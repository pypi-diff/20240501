# Comparing `tmp/trytond_stock_forecast-7.2.0.tar.gz` & `tmp/trytond_stock_forecast-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_stock_forecast-7.2.0.tar", last modified: Mon Apr 29 15:50:56 2024, max compression
+gzip compressed data, was "trytond_stock_forecast-7.2.1.tar", last modified: Wed May  1 10:05:03 2024, max compression
```

## Comparing `trytond_stock_forecast-7.2.0.tar` & `trytond_stock_forecast-7.2.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:50:56.839602 trytond_stock_forecast-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     3749 2024-04-29 15:27:34.000000 trytond_stock_forecast-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      728 2024-04-29 15:27:33.000000 trytond_stock_forecast-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_stock_forecast-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_stock_forecast-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2746 2024-04-29 15:50:56.836269 trytond_stock_forecast-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      261 2024-04-27 16:30:39.000000 trytond_stock_forecast-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      518 2024-01-27 09:58:52.000000 trytond_stock_forecast-7.2.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:50:56.832936 trytond_stock_forecast-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3077 2024-04-27 16:30:39.000000 trytond_stock_forecast-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1135 2024-04-27 16:30:39.000000 trytond_stock_forecast-7.2.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      261 2024-04-27 16:30:39.000000 trytond_stock_forecast-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-27 16:30:39.000000 trytond_stock_forecast-7.2.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:32.000000 trytond_stock_forecast-7.2.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      257 2023-04-15 07:12:15.000000 trytond_stock_forecast-7.2.0/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)    22210 2024-04-27 16:30:39.000000 trytond_stock_forecast-7.2.0/forecast.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6201 2024-04-27 16:30:39.000000 trytond_stock_forecast-7.2.0/forecast.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:50:56.836269 trytond_stock_forecast-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     5450 2024-04-27 16:43:27.000000 trytond_stock_forecast-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5330 2024-04-27 16:43:27.000000 trytond_stock_forecast-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4635 2024-04-27 16:43:27.000000 trytond_stock_forecast-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5465 2024-04-27 16:43:27.000000 trytond_stock_forecast-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5327 2024-04-27 16:43:27.000000 trytond_stock_forecast-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4513 2024-04-27 16:43:27.000000 trytond_stock_forecast-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4884 2024-04-27 16:43:27.000000 trytond_stock_forecast-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5610 2024-04-27 16:43:27.000000 trytond_stock_forecast-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4635 2024-04-27 16:43:27.000000 trytond_stock_forecast-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5373 2024-04-27 16:43:27.000000 trytond_stock_forecast-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4908 2024-04-27 16:43:27.000000 trytond_stock_forecast-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4605 2024-04-27 16:43:27.000000 trytond_stock_forecast-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4895 2024-04-27 16:43:27.000000 trytond_stock_forecast-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5294 2024-04-27 16:43:27.000000 trytond_stock_forecast-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4668 2024-04-27 16:43:27.000000 trytond_stock_forecast-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5281 2024-04-27 16:43:27.000000 trytond_stock_forecast-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4853 2024-04-27 16:43:27.000000 trytond_stock_forecast-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5134 2024-04-27 16:43:27.000000 trytond_stock_forecast-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4460 2024-04-27 16:43:27.000000 trytond_stock_forecast-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5638 2024-04-27 16:43:27.000000 trytond_stock_forecast-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5041 2024-04-27 16:43:27.000000 trytond_stock_forecast-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4635 2024-04-27 16:43:27.000000 trytond_stock_forecast-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4406 2024-04-27 16:43:27.000000 trytond_stock_forecast-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4690 2024-04-27 16:43:27.000000 trytond_stock_forecast-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      777 2023-04-15 07:12:15.000000 trytond_stock_forecast-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      507 2024-01-27 09:58:52.000000 trytond_stock_forecast-7.2.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:50:56.839602 trytond_stock_forecast-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4462 2024-04-27 16:30:39.000000 trytond_stock_forecast-7.2.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:50:56.836269 trytond_stock_forecast-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_stock_forecast-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    14575 2024-04-22 12:14:37.000000 trytond_stock_forecast-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:32.000000 trytond_stock_forecast-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      135 2024-04-29 15:27:29.000000 trytond_stock_forecast-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:50:56.836269 trytond_stock_forecast-7.2.0/trytond_stock_forecast.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2746 2024-04-29 15:50:56.000000 trytond_stock_forecast-7.2.0/trytond_stock_forecast.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1777 2024-04-29 15:50:56.000000 trytond_stock_forecast-7.2.0/trytond_stock_forecast.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:50:56.000000 trytond_stock_forecast-7.2.0/trytond_stock_forecast.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       66 2024-04-29 15:50:56.000000 trytond_stock_forecast-7.2.0/trytond_stock_forecast.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:02.000000 trytond_stock_forecast-7.2.0/trytond_stock_forecast.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      126 2024-04-29 15:50:56.000000 trytond_stock_forecast-7.2.0/trytond_stock_forecast.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:50:56.000000 trytond_stock_forecast-7.2.0/trytond_stock_forecast.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:50:56.836269 trytond_stock_forecast-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      522 2024-01-27 09:58:52.000000 trytond_stock_forecast-7.2.0/view/forecast_complete_ask_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      915 2023-04-15 07:12:15.000000 trytond_stock_forecast-7.2.0/view/forecast_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      619 2024-02-04 18:51:26.000000 trytond_stock_forecast-7.2.0/view/forecast_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      407 2024-02-04 18:51:26.000000 trytond_stock_forecast-7.2.0/view/forecast_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      432 2024-01-27 09:58:52.000000 trytond_stock_forecast-7.2.0/view/forecast_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      310 2024-01-27 09:58:52.000000 trytond_stock_forecast-7.2.0/view/product_list_forecast.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 10:05:03.434568 trytond_stock_forecast-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3850 2024-05-01 10:05:00.000000 trytond_stock_forecast-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      728 2024-05-01 10:05:00.000000 trytond_stock_forecast-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:21:00.000000 trytond_stock_forecast-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:21:00.000000 trytond_stock_forecast-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2746 2024-05-01 10:05:03.434568 trytond_stock_forecast-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      261 2024-04-30 17:21:00.000000 trytond_stock_forecast-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      518 2024-04-30 17:21:00.000000 trytond_stock_forecast-7.2.1/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 10:05:03.431234 trytond_stock_forecast-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3077 2024-04-30 17:21:00.000000 trytond_stock_forecast-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1135 2024-04-30 17:21:00.000000 trytond_stock_forecast-7.2.1/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      261 2024-04-30 17:21:00.000000 trytond_stock_forecast-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-30 17:21:00.000000 trytond_stock_forecast-7.2.1/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:21:00.000000 trytond_stock_forecast-7.2.1/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      257 2024-04-30 17:21:00.000000 trytond_stock_forecast-7.2.1/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    22210 2024-04-30 17:21:00.000000 trytond_stock_forecast-7.2.1/forecast.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6201 2024-04-30 17:21:00.000000 trytond_stock_forecast-7.2.1/forecast.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 10:05:03.434568 trytond_stock_forecast-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     5450 2024-04-30 17:21:00.000000 trytond_stock_forecast-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5330 2024-04-30 17:21:00.000000 trytond_stock_forecast-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4635 2024-04-30 17:21:00.000000 trytond_stock_forecast-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5465 2024-04-30 17:21:59.000000 trytond_stock_forecast-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5327 2024-04-30 17:21:00.000000 trytond_stock_forecast-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4513 2024-04-30 17:21:00.000000 trytond_stock_forecast-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4884 2024-04-30 17:21:00.000000 trytond_stock_forecast-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5610 2024-04-30 17:21:00.000000 trytond_stock_forecast-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4635 2024-04-30 17:21:00.000000 trytond_stock_forecast-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5373 2024-04-30 17:21:00.000000 trytond_stock_forecast-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4908 2024-04-30 17:21:00.000000 trytond_stock_forecast-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4605 2024-04-30 17:21:00.000000 trytond_stock_forecast-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4895 2024-04-30 17:21:00.000000 trytond_stock_forecast-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5294 2024-04-30 17:21:00.000000 trytond_stock_forecast-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4668 2024-04-30 17:21:00.000000 trytond_stock_forecast-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5281 2024-04-30 17:21:00.000000 trytond_stock_forecast-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4853 2024-04-30 17:21:00.000000 trytond_stock_forecast-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5134 2024-04-30 17:21:00.000000 trytond_stock_forecast-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4460 2024-04-30 17:21:00.000000 trytond_stock_forecast-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5638 2024-04-30 17:21:00.000000 trytond_stock_forecast-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5041 2024-04-30 17:21:00.000000 trytond_stock_forecast-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4635 2024-04-30 17:21:00.000000 trytond_stock_forecast-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4406 2024-04-30 17:21:00.000000 trytond_stock_forecast-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4690 2024-04-30 17:21:00.000000 trytond_stock_forecast-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      777 2024-04-30 17:21:00.000000 trytond_stock_forecast-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      507 2024-04-30 17:21:00.000000 trytond_stock_forecast-7.2.1/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 10:05:03.434568 trytond_stock_forecast-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4462 2024-04-30 17:21:00.000000 trytond_stock_forecast-7.2.1/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 10:05:03.434568 trytond_stock_forecast-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:21:00.000000 trytond_stock_forecast-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    14575 2024-04-30 17:21:00.000000 trytond_stock_forecast-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:21:00.000000 trytond_stock_forecast-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      135 2024-04-30 17:21:06.000000 trytond_stock_forecast-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 10:05:03.434568 trytond_stock_forecast-7.2.1/trytond_stock_forecast.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2746 2024-05-01 10:05:02.000000 trytond_stock_forecast-7.2.1/trytond_stock_forecast.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1777 2024-05-01 10:05:03.000000 trytond_stock_forecast-7.2.1/trytond_stock_forecast.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 10:05:02.000000 trytond_stock_forecast-7.2.1/trytond_stock_forecast.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       66 2024-05-01 10:05:02.000000 trytond_stock_forecast-7.2.1/trytond_stock_forecast.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 10:05:02.000000 trytond_stock_forecast-7.2.1/trytond_stock_forecast.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      126 2024-05-01 10:05:02.000000 trytond_stock_forecast-7.2.1/trytond_stock_forecast.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 10:05:02.000000 trytond_stock_forecast-7.2.1/trytond_stock_forecast.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 10:05:03.434568 trytond_stock_forecast-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      522 2024-04-30 17:21:00.000000 trytond_stock_forecast-7.2.1/view/forecast_complete_ask_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      915 2024-04-30 17:21:00.000000 trytond_stock_forecast-7.2.1/view/forecast_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      619 2024-04-30 17:21:00.000000 trytond_stock_forecast-7.2.1/view/forecast_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      407 2024-04-30 17:21:00.000000 trytond_stock_forecast-7.2.1/view/forecast_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      432 2024-04-30 17:21:00.000000 trytond_stock_forecast-7.2.1/view/forecast_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      310 2024-04-30 17:21:00.000000 trytond_stock_forecast-7.2.1/view/product_list_forecast.xml
```

### Comparing `trytond_stock_forecast-7.2.0/CHANGELOG` & `trytond_stock_forecast-7.2.1/CHANGELOG`

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

### Comparing `trytond_stock_forecast-7.2.0/COPYRIGHT` & `trytond_stock_forecast-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.2.0/LICENSE` & `trytond_stock_forecast-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.2.0/PKG-INFO` & `trytond_stock_forecast-7.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_stock_forecast
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module with stock forecasts
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_stock_forecast-7.2.0/__init__.py` & `trytond_stock_forecast-7.2.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.2.0/doc/conf.py` & `trytond_stock_forecast-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.2.0/doc/design.rst` & `trytond_stock_forecast-7.2.1/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.2.0/forecast.py` & `trytond_stock_forecast-7.2.1/forecast.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.2.0/forecast.xml` & `trytond_stock_forecast-7.2.1/forecast.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.2.0/locale/bg.po` & `trytond_stock_forecast-7.2.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.2.0/locale/ca.po` & `trytond_stock_forecast-7.2.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.2.0/locale/cs.po` & `trytond_stock_forecast-7.2.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.2.0/locale/de.po` & `trytond_stock_forecast-7.2.1/locale/de.po`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,15 @@
 
 msgctxt "model:ir.model.button,string:forecast_draft_button"
 msgid "Draft"
 msgstr "Entwurf"
 
 msgctxt "model:ir.rule.group,name:rule_group_forecast_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.ui.menu,name:menu_forecast_form"
 msgid "Forecasts"
 msgstr "Bedarfsprognosen"
 
 msgctxt "model:res.group,name:group_stock_forecast"
 msgid "Stock Forecast"
```

### Comparing `trytond_stock_forecast-7.2.0/locale/es.po` & `trytond_stock_forecast-7.2.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.2.0/locale/es_419.po` & `trytond_stock_forecast-7.2.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.2.0/locale/et.po` & `trytond_stock_forecast-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.2.0/locale/fa.po` & `trytond_stock_forecast-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.2.0/locale/fi.po` & `trytond_stock_forecast-7.2.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.2.0/locale/fr.po` & `trytond_stock_forecast-7.2.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.2.0/locale/hu.po` & `trytond_stock_forecast-7.2.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.2.0/locale/id.po` & `trytond_stock_forecast-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.2.0/locale/it.po` & `trytond_stock_forecast-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.2.0/locale/lo.po` & `trytond_stock_forecast-7.2.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.2.0/locale/lt.po` & `trytond_stock_forecast-7.2.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.2.0/locale/nl.po` & `trytond_stock_forecast-7.2.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.2.0/locale/pl.po` & `trytond_stock_forecast-7.2.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.2.0/locale/pt.po` & `trytond_stock_forecast-7.2.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.2.0/locale/ro.po` & `trytond_stock_forecast-7.2.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.2.0/locale/ru.po` & `trytond_stock_forecast-7.2.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.2.0/locale/sl.po` & `trytond_stock_forecast-7.2.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.2.0/locale/tr.po` & `trytond_stock_forecast-7.2.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.2.0/locale/uk.po` & `trytond_stock_forecast-7.2.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.2.0/locale/zh_CN.po` & `trytond_stock_forecast-7.2.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.2.0/message.xml` & `trytond_stock_forecast-7.2.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.2.0/setup.py` & `trytond_stock_forecast-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.2.0/tests/test_module.py` & `trytond_stock_forecast-7.2.1/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.2.0/tox.ini` & `trytond_stock_forecast-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.2.0/trytond_stock_forecast.egg-info/PKG-INFO` & `trytond_stock_forecast-7.2.1/trytond_stock_forecast.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_stock_forecast
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module with stock forecasts
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_stock_forecast-7.2.0/trytond_stock_forecast.egg-info/SOURCES.txt` & `trytond_stock_forecast-7.2.1/trytond_stock_forecast.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.2.0/view/forecast_complete_ask_form.xml` & `trytond_stock_forecast-7.2.1/view/forecast_complete_ask_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.2.0/view/forecast_form.xml` & `trytond_stock_forecast-7.2.1/view/forecast_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.2.0/view/forecast_line_form.xml` & `trytond_stock_forecast-7.2.1/view/forecast_line_form.xml`

 * *Files identical despite different names*

