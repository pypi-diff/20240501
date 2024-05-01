# Comparing `tmp/trytond_stock_product_location-7.0.2.tar.gz` & `tmp/trytond_stock_product_location-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_stock_product_location-7.0.2.tar", last modified: Wed May  1 09:55:44 2024, max compression
+gzip compressed data, was "trytond_stock_product_location-7.2.0.tar", last modified: Mon Apr 29 15:52:26 2024, max compression
```

## Comparing `trytond_stock_product_location-7.0.2.tar` & `trytond_stock_product_location-7.2.0.tar`

### file list

```diff
@@ -1,66 +1,69 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:55:44.675848 trytond_stock_product_location-7.0.2/
--rw-r--r--   0 ced       (1000) ced       (1000)     2836 2024-05-01 09:55:41.000000 trytond_stock_product_location-7.0.2/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      728 2024-05-01 09:55:41.000000 trytond_stock_product_location-7.0.2/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_stock_product_location-7.0.2/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_stock_product_location-7.0.2/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2907 2024-05-01 09:55:44.675848 trytond_stock_product_location-7.0.2/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      347 2024-02-05 16:24:27.000000 trytond_stock_product_location-7.0.2/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      624 2023-10-30 17:06:38.000000 trytond_stock_product_location-7.0.2/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:55:44.669182 trytond_stock_product_location-7.0.2/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2801 2024-03-03 16:24:20.000000 trytond_stock_product_location-7.0.2/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      347 2024-02-05 16:24:27.000000 trytond_stock_product_location-7.0.2/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_stock_product_location-7.0.2/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:55:44.672515 trytond_stock_product_location-7.0.2/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      887 2023-10-30 17:06:38.000000 trytond_stock_product_location-7.0.2/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)      737 2023-10-30 17:06:38.000000 trytond_stock_product_location-7.0.2/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      619 2023-10-30 17:06:38.000000 trytond_stock_product_location-7.0.2/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)      708 2023-10-30 17:06:38.000000 trytond_stock_product_location-7.0.2/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)      729 2023-10-30 17:06:38.000000 trytond_stock_product_location-7.0.2/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      690 2023-10-30 17:06:38.000000 trytond_stock_product_location-7.0.2/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      712 2023-10-30 17:06:38.000000 trytond_stock_product_location-7.0.2/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)      749 2023-10-30 17:06:38.000000 trytond_stock_product_location-7.0.2/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      619 2023-10-30 17:06:38.000000 trytond_stock_product_location-7.0.2/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)      733 2023-10-30 17:06:38.000000 trytond_stock_product_location-7.0.2/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      742 2023-10-30 17:06:38.000000 trytond_stock_product_location-7.0.2/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      676 2023-10-30 17:06:38.000000 trytond_stock_product_location-7.0.2/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)      724 2023-10-30 17:06:38.000000 trytond_stock_product_location-7.0.2/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)      886 2023-10-30 17:06:38.000000 trytond_stock_product_location-7.0.2/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      619 2023-10-30 17:06:38.000000 trytond_stock_product_location-7.0.2/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      704 2023-10-30 17:06:38.000000 trytond_stock_product_location-7.0.2/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      713 2023-10-30 17:06:38.000000 trytond_stock_product_location-7.0.2/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      754 2023-10-30 17:06:38.000000 trytond_stock_product_location-7.0.2/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      713 2023-10-30 17:06:38.000000 trytond_stock_product_location-7.0.2/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      837 2023-10-30 17:06:38.000000 trytond_stock_product_location-7.0.2/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      713 2023-10-30 17:06:38.000000 trytond_stock_product_location-7.0.2/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      688 2023-10-30 17:06:38.000000 trytond_stock_product_location-7.0.2/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      619 2023-10-30 17:06:38.000000 trytond_stock_product_location-7.0.2/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      619 2023-10-30 17:06:38.000000 trytond_stock_product_location-7.0.2/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3381 2024-04-27 05:19:49.000000 trytond_stock_product_location-7.0.2/location.py
--rw-r--r--   0 ced       (1000) ced       (1000)      721 2024-02-05 16:24:27.000000 trytond_stock_product_location-7.0.2/location.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2902 2023-10-30 17:06:38.000000 trytond_stock_product_location-7.0.2/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      469 2023-10-30 17:06:38.000000 trytond_stock_product_location-7.0.2/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      585 2023-10-30 17:06:38.000000 trytond_stock_product_location-7.0.2/production.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 09:55:44.675848 trytond_stock_product_location-7.0.2/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4604 2024-03-03 16:47:02.000000 trytond_stock_product_location-7.0.2/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:55:44.672515 trytond_stock_product_location-7.0.2/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_stock_product_location-7.0.2/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1966 2024-02-05 16:24:27.000000 trytond_stock_product_location-7.0.2/tests/scenario_product_copy_locations.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3725 2024-02-05 16:24:27.000000 trytond_stock_product_location-7.0.2/tests/scenario_stock_product_location.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4520 2024-02-05 16:24:27.000000 trytond_stock_product_location-7.0.2/tests/scenario_stock_product_location_production.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3733 2024-02-05 16:24:27.000000 trytond_stock_product_location-7.0.2/tests/scenario_stock_product_location_template.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      378 2023-10-30 17:06:38.000000 trytond_stock_product_location-7.0.2/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-10-30 17:06:38.000000 trytond_stock_product_location-7.0.2/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_stock_product_location-7.0.2/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      129 2024-02-05 16:24:27.000000 trytond_stock_product_location-7.0.2/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:55:44.672515 trytond_stock_product_location-7.0.2/trytond_stock_product_location.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2907 2024-05-01 09:55:44.000000 trytond_stock_product_location-7.0.2/trytond_stock_product_location.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2055 2024-05-01 09:55:44.000000 trytond_stock_product_location-7.0.2/trytond_stock_product_location.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 09:55:44.000000 trytond_stock_product_location-7.0.2/trytond_stock_product_location.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       82 2024-05-01 09:55:44.000000 trytond_stock_product_location-7.0.2/trytond_stock_product_location.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:08:16.000000 trytond_stock_product_location-7.0.2/trytond_stock_product_location.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      139 2024-05-01 09:55:44.000000 trytond_stock_product_location-7.0.2/trytond_stock_product_location.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 09:55:44.000000 trytond_stock_product_location-7.0.2/trytond_stock_product_location.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:55:44.672515 trytond_stock_product_location-7.0.2/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      349 2023-10-30 17:06:38.000000 trytond_stock_product_location-7.0.2/view/product_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      508 2023-10-30 17:06:38.000000 trytond_stock_product_location-7.0.2/view/product_location_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      346 2023-10-30 17:06:38.000000 trytond_stock_product_location-7.0.2/view/product_location_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:52:26.670586 trytond_stock_product_location-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3465 2024-04-29 15:28:40.000000 trytond_stock_product_location-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      728 2024-04-29 15:28:40.000000 trytond_stock_product_location-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_stock_product_location-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_stock_product_location-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2719 2024-04-29 15:52:26.670586 trytond_stock_product_location-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      211 2024-04-22 12:14:36.000000 trytond_stock_product_location-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      624 2023-04-15 07:12:15.000000 trytond_stock_product_location-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:52:26.667253 trytond_stock_product_location-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3085 2024-04-27 16:30:39.000000 trytond_stock_product_location-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      537 2024-04-22 12:14:36.000000 trytond_stock_product_location-7.2.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      211 2024-04-22 12:14:36.000000 trytond_stock_product_location-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-22 12:14:36.000000 trytond_stock_product_location-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:35.000000 trytond_stock_product_location-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:52:26.667253 trytond_stock_product_location-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)      887 2024-04-27 16:43:28.000000 trytond_stock_product_location-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      737 2024-04-27 16:43:28.000000 trytond_stock_product_location-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      619 2024-04-27 16:43:28.000000 trytond_stock_product_location-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      708 2024-04-27 16:43:28.000000 trytond_stock_product_location-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      729 2024-04-27 16:43:28.000000 trytond_stock_product_location-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      690 2024-04-27 16:43:28.000000 trytond_stock_product_location-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      712 2024-04-27 16:43:28.000000 trytond_stock_product_location-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      749 2024-04-27 16:43:28.000000 trytond_stock_product_location-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      619 2024-04-27 16:43:28.000000 trytond_stock_product_location-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      733 2024-04-27 16:43:28.000000 trytond_stock_product_location-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      742 2024-04-27 16:43:28.000000 trytond_stock_product_location-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      676 2024-04-27 16:43:28.000000 trytond_stock_product_location-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      724 2024-04-27 16:43:28.000000 trytond_stock_product_location-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      886 2024-04-27 16:43:28.000000 trytond_stock_product_location-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      619 2024-04-27 16:43:28.000000 trytond_stock_product_location-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      704 2024-04-27 16:43:28.000000 trytond_stock_product_location-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      713 2024-04-27 16:43:28.000000 trytond_stock_product_location-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      754 2024-04-27 16:43:28.000000 trytond_stock_product_location-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      713 2024-04-27 16:43:28.000000 trytond_stock_product_location-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      837 2024-04-27 16:43:28.000000 trytond_stock_product_location-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      713 2024-04-27 16:43:28.000000 trytond_stock_product_location-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      688 2024-04-27 16:43:28.000000 trytond_stock_product_location-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      619 2024-04-27 16:43:28.000000 trytond_stock_product_location-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      619 2024-04-27 16:43:28.000000 trytond_stock_product_location-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3942 2024-04-27 16:30:39.000000 trytond_stock_product_location-7.2.0/location.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1526 2024-04-27 16:30:39.000000 trytond_stock_product_location-7.2.0/location.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2902 2023-04-15 07:12:15.000000 trytond_stock_product_location-7.2.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      469 2023-04-15 07:12:15.000000 trytond_stock_product_location-7.2.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      569 2024-04-27 16:30:39.000000 trytond_stock_product_location-7.2.0/production.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:52:26.670586 trytond_stock_product_location-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4717 2024-04-27 16:30:39.000000 trytond_stock_product_location-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:52:26.667253 trytond_stock_product_location-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_stock_product_location-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1968 2024-04-22 12:14:37.000000 trytond_stock_product_location-7.2.0/tests/scenario_product_copy_locations.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3721 2024-04-22 12:14:36.000000 trytond_stock_product_location-7.2.0/tests/scenario_stock_product_location.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2199 2024-04-22 12:14:36.000000 trytond_stock_product_location-7.2.0/tests/scenario_stock_product_location_consumable.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4485 2024-04-22 12:14:36.000000 trytond_stock_product_location-7.2.0/tests/scenario_stock_product_location_production.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3729 2024-04-22 12:14:36.000000 trytond_stock_product_location-7.2.0/tests/scenario_stock_product_location_template.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      378 2023-04-15 07:12:15.000000 trytond_stock_product_location-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_stock_product_location-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:35.000000 trytond_stock_product_location-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      129 2024-04-29 15:28:36.000000 trytond_stock_product_location-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:52:26.670586 trytond_stock_product_location-7.2.0/trytond_stock_product_location.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2719 2024-04-29 15:52:26.000000 trytond_stock_product_location-7.2.0/trytond_stock_product_location.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2195 2024-04-29 15:52:26.000000 trytond_stock_product_location-7.2.0/trytond_stock_product_location.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:52:26.000000 trytond_stock_product_location-7.2.0/trytond_stock_product_location.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       82 2024-04-29 15:52:26.000000 trytond_stock_product_location-7.2.0/trytond_stock_product_location.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:03.000000 trytond_stock_product_location-7.2.0/trytond_stock_product_location.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      139 2024-04-29 15:52:26.000000 trytond_stock_product_location-7.2.0/trytond_stock_product_location.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:52:26.000000 trytond_stock_product_location-7.2.0/trytond_stock_product_location.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:52:26.670586 trytond_stock_product_location-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      349 2023-01-16 14:00:21.000000 trytond_stock_product_location-7.2.0/view/product_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      508 2023-04-15 07:12:15.000000 trytond_stock_product_location-7.2.0/view/product_location_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      346 2023-04-15 07:12:15.000000 trytond_stock_product_location-7.2.0/view/product_location_tree.xml
```

### Comparing `trytond_stock_product_location-7.0.2/CHANGELOG` & `trytond_stock_product_location-7.2.0/CHANGELOG`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,9 @@
 
-Version 7.0.2 - 2024-05-01
---------------------------
-* Bug fixes (see mercurial logs for details)
-
-
-Version 7.0.1 - 2023-12-01
+Version 7.2.0 - 2024-04-29
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 
 Version 7.0.0 - 2023-10-30
 --------------------------
 * Bug fixes (see mercurial logs for details)
@@ -21,94 +16,122 @@
 * Add support for Python 3.11
 
 Version 6.6.0 - 2022-10-31
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 6.4.0 - 2022-05-02
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Add support for Python 3.10
 * Remove support for Python 3.6
 
 Version 6.2.0 - 2021-11-01
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 6.0.0 - 2021-05-03
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 5.8.0 - 2020-11-02
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Remove support for Python 3.5
 * Add default locations on templates
 
 Version 5.6.0 - 2020-05-04
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 5.4.0 - 2019-11-04
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 5.2.0 - 2019-05-06
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 5.0.0 - 2018-10-01
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Remove support for Python 2.7
 
 Version 4.8.0 - 2018-04-23
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 4.6.0 - 2017-10-30
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 4.4.0 - 2017-05-01
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Use MatchMixin for ProductLocation
 
 Version 4.2.0 - 2016-11-28
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Use product default location for production outputs
 
 Version 4.0.0 - 2016-05-02
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Add Python3 support
 
 Version 3.8.0 - 2015-11-02
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 3.6.0 - 2015-04-20
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Add support for PyPy
+
 Version 3.4.0 - 2014-10-20
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 3.2.0 - 2014-04-21
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 3.0.0 - 2013-10-21
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 2.8.0 - 2013-04-22
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 2.6.0 - 2012-10-22
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 2.4.0 - 2012-04-24
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 2.2.0 - 2011-10-25
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 2.0.0 - 2011-04-27
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 1.8.0 - 2010-11-01
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 1.6.0 - 2010-05-12
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 1.4.0 - 2009-10-19
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 1.2.0 - 2009-07-31
+--------------------------
 * Initial release
```

### Comparing `trytond_stock_product_location-7.0.2/COPYRIGHT` & `trytond_stock_product_location-7.2.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location-7.0.2/LICENSE` & `trytond_stock_product_location-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location-7.0.2/PKG-INFO` & `trytond_stock_product_location-7.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_stock_product_location
-Version: 7.0.2
+Version: 7.2.0
 Summary: Tryton module to add default location on product
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/modules-stock-product-location
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
@@ -48,22 +48,20 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql>=0.4
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_production<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_production<7.3,>=7.2; extra == "test"
 
 Stock Product Location Module
 #############################
 
-The Stock Product Location Module adds on the product form a list of
-preferred location by warehouse. This list is used when a supplier
-shipment is received: the auto-generated Inventory Moves will use as
-default destination the preferred locations associated to the current
-warehouse.
+The *Stock Product Location Module* adds a list of preferred locations by
+warehouse and product.
+
```

### Comparing `trytond_stock_product_location-7.0.2/__init__.py` & `trytond_stock_product_location-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location-7.0.2/doc/conf.py` & `trytond_stock_product_location-7.2.0/doc/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,22 +67,33 @@
     }
 html_title = info['description']
 master_doc = 'index'
 project = info['name']
 release = version = info['series']
 default_role = 'ref'
 highlight_language = 'none'
+exclude_patterns = ['**/*.inc.rst']
 extensions = [
     'sphinx_copybutton',
     'sphinx.ext.intersphinx',
     ]
 intersphinx_mapping = {
     'trytond': (trytond_url.format(series=version), None),
     }
 intersphinx_mapping.update({
         m: (modules_url.format(
                 module=m.replace('_', '-'), series=version), None)
         for m in info['modules']
         })
 linkcheck_ignore = [r'/.*', r'https://demo.tryton.org/*']
 
+try:
+    with open(os.path.join(
+                os.path.dirname(__file__),
+                'linkcheck_ignore.json'), 'r') as f:
+        import json
+        linkcheck_ignore.extend(json.load(f))
+        del json
+except FileNotFoundError:
+    pass
+
 del get_info, info, base_url, modules_url, trytond_url
```

### Comparing `trytond_stock_product_location-7.0.2/locale/bg.po` & `trytond_stock_product_location-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location-7.0.2/locale/ca.po` & `trytond_stock_product_location-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location-7.0.2/locale/cs.po` & `trytond_stock_product_location-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location-7.0.2/locale/de.po` & `trytond_stock_product_location-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location-7.0.2/locale/es.po` & `trytond_stock_product_location-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location-7.0.2/locale/es_419.po` & `trytond_stock_product_location-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location-7.0.2/locale/et.po` & `trytond_stock_product_location-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location-7.0.2/locale/fa.po` & `trytond_stock_product_location-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location-7.0.2/locale/fi.po` & `trytond_stock_product_location-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location-7.0.2/locale/fr.po` & `trytond_stock_product_location-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location-7.0.2/locale/hu.po` & `trytond_stock_product_location-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location-7.0.2/locale/id.po` & `trytond_stock_product_location-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location-7.0.2/locale/it.po` & `trytond_stock_product_location-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location-7.0.2/locale/lo.po` & `trytond_stock_product_location-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location-7.0.2/locale/lt.po` & `trytond_stock_product_location-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location-7.0.2/locale/nl.po` & `trytond_stock_product_location-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location-7.0.2/locale/pl.po` & `trytond_stock_product_location-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location-7.0.2/locale/pt.po` & `trytond_stock_product_location-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location-7.0.2/locale/ro.po` & `trytond_stock_product_location-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location-7.0.2/locale/ru.po` & `trytond_stock_product_location-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location-7.0.2/locale/sl.po` & `trytond_stock_product_location-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location-7.0.2/locale/tr.po` & `trytond_stock_product_location-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location-7.0.2/locale/uk.po` & `trytond_stock_product_location-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location-7.0.2/locale/zh_CN.po` & `trytond_stock_product_location-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location-7.0.2/location.py` & `trytond_stock_product_location-7.2.0/location.py`

 * *Files 15% similar despite different names*

```diff
@@ -52,30 +52,45 @@
             self.template = self.product.template
 
 
 class Move(metaclass=PoolMeta):
     __name__ = 'stock.move'
 
     def set_product_location(self, field='to_location', **pattern):
+        "Set the product location on the field"
         assert field in {'from_location', 'to_location'}
+        location = self.get_product_location(**pattern)
+        if location:
+            setattr(self, field, location)
+
+    def get_product_location(self, **pattern):
+        "Return the product location for the move"
         if (getattr(self, 'shipment', None)
                 and getattr(self.shipment, 'warehouse', None)):
             pattern.setdefault('warehouse', self.shipment.warehouse.id)
         elif getattr(self, 'production', None):
             pattern.setdefault('warehouse', self.production.warehouse.id)
 
         if self.product:
             pattern.setdefault('template', self.product.template.id)
             pattern.setdefault('product', self.product.id)
 
         locations = self.product.locations + self.product.template.locations
         for product_location in locations:
             if product_location.match(pattern):
-                setattr(self, field, product_location.location)
-                break
+                return product_location.location
+
+    @property
+    def _default_pick_location(self):
+        location = super()._default_pick_location
+        if self.product.consumable:
+            if ((product_location := self.get_product_location())
+                    and product_location.type != 'view'):
+                location = product_location
+        return location
 
 
 class ShipmentIn(metaclass=PoolMeta):
     __name__ = 'stock.shipment.in'
 
     def _get_inventory_move(self, incoming_move):
         move = super()._get_inventory_move(incoming_move)
```

### Comparing `trytond_stock_product_location-7.0.2/product.py` & `trytond_stock_product_location-7.2.0/product.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location-7.0.2/setup.py` & `trytond_stock_product_location-7.2.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,17 +7,20 @@
 import re
 from configparser import ConfigParser
 
 from setuptools import find_packages, setup
 
 
 def read(fname):
-    return io.open(
+    content = io.open(
         os.path.join(os.path.dirname(__file__), fname),
         'r', encoding='utf-8').read()
+    content = re.sub(
+        r'(?m)^\.\. toctree::\r?\n((^$|^\s.*$)\r?\n)*', '', content)
+    return content
 
 
 def get_require_version(name):
     require = '%s >= %s.%s, < %s.%s'
     require %= (name, major_version, minor_version,
         major_version, minor_version + 1)
     return require
```

### Comparing `trytond_stock_product_location-7.0.2/tests/scenario_product_copy_locations.rst` & `trytond_stock_product_location-7.2.0/tests/scenario_product_copy_locations.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 =============================
 Product Copy Locaton Scenario
 =============================
 
 Imports::
 
     >>> from decimal import Decimal
+
     >>> from proteus import Model
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
 Activate modules::
 
     >>> config = activate_modules('stock_product_location')
 
 Create company::
 
@@ -49,16 +49,15 @@
     >>> template_location.warehouse = warehouse_loc
     >>> template_location.location = child_loc
     >>> template.save()
     >>> product, = template.products
     >>> product_location = product.locations.new()
     >>> product_location.warehouse = warehouse_loc
     >>> product_location.location = child_loc
-    >>> product_location.template == template
-    True
+    >>> assertEqual(product_location.template, template)
     >>> product.save()
 
 Location is copied when copying the template::
 
     >>> template_copy, = template.duplicate()
     >>> product_copy, = template_copy.products
     >>> len(template_copy.locations)
```

### Comparing `trytond_stock_product_location-7.0.2/tests/scenario_stock_product_location.rst` & `trytond_stock_product_location-7.2.0/tests/scenario_stock_product_location.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 Stock Product Locations Scenario
 ================================
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
+
+    >>> from proteus import Model
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
     >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('stock_product_location')
 
@@ -92,36 +92,34 @@
     >>> move.currency = company.currency
     >>> shipment_in.save()
 
 Test that to_location is child location on reception::
 
     >>> shipment_in.click('receive')
     >>> move, = shipment_in.inventory_moves
-    >>> move.to_location == child_loc
-    True
+    >>> assertEqual(move.to_location, child_loc)
 
 Create return shipment out::
 
     >>> Shipment_out_Return = Model.get('stock.shipment.out.return')
     >>> shipment_out_return = Shipment_out_Return()
     >>> shipment_out_return.customer = customer
     >>> shipment_out_return.save()
 
 Add one shipment return line::
 
     >>> move = shipment_out_return.incoming_moves.new()
     >>> move.product = product
-    >>> move.unit =unit
+    >>> move.unit = unit
     >>> move.quantity = 1
     >>> move.from_location = customer_loc
-    >>> move.to_location =  input_loc
+    >>> move.to_location = input_loc
     >>> move.company = company
     >>> move.unit_price = Decimal('1')
     >>> move.currency = company.currency
     >>> shipment_out_return.save()
 
 Test that to_location is child location on reception::
 
     >>> shipment_out_return.click('receive')
     >>> move, = shipment_out_return.inventory_moves
-    >>> move.to_location == child_loc
-    True
+    >>> assertEqual(move.to_location, child_loc)
```

### Comparing `trytond_stock_product_location-7.0.2/tests/scenario_stock_product_location_production.rst` & `trytond_stock_product_location-7.2.0/tests/scenario_stock_product_location_production.rst`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 Stock Product Locations Production Scenario
 ===========================================
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
+
     >>> from proteus import Model
-    >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
     >>> today = dt.date.today()
 
 Activate modules::
 
     >>> _ = activate_modules(['stock_product_location', 'production'])
 
@@ -125,26 +126,20 @@
     >>> production.planned_date = today
     >>> production.product = product
     >>> production.bom = bom
     >>> production.quantity = 2
 
 Test storage location of the warehouse::
 
-    >> warehouse_loc.storage_location == storage_loc
-    True
+    >> assertEqual(warehouse_loc.storage_location, storage_loc)
 
 Test locations of the production inputs::
 
-    >>> all([input_.from_location == storage_loc for \
-    ...      input_ in production.inputs])
-    True
-    >>> all([input_.to_location == production_loc for \
-    ...      input_ in production.inputs])
-    True
+    >>> for input_ in production.inputs:
+    ...     assertEqual(input_.from_location, storage_loc)
+    ...     assertEqual(input_.to_location, production_loc)
 
 Test location of the production output::
 
     >>> output, = production.outputs
-    >>> output.from_location == production_loc
-    True
-    >>> output.to_location == child_loc
-    True
+    >>> assertEqual(output.from_location, production_loc)
+    >>> assertEqual(output.to_location, child_loc)
```

### Comparing `trytond_stock_product_location-7.0.2/tests/scenario_stock_product_location_template.rst` & `trytond_stock_product_location-7.2.0/tests/scenario_stock_product_location_template.rst`

 * *Files 6% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 Stock Product Locations Template Scenario
 =========================================
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
+
+    >>> from proteus import Model
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
     >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('stock_product_location')
 
@@ -91,36 +91,34 @@
     >>> move.currency = company.currency
     >>> shipment_in.save()
 
 Test that to_location is child location on reception::
 
     >>> shipment_in.click('receive')
     >>> move, = shipment_in.inventory_moves
-    >>> move.to_location == child_loc
-    True
+    >>> assertEqual(move.to_location, child_loc)
 
 Create return shipment out::
 
     >>> Shipment_out_Return = Model.get('stock.shipment.out.return')
     >>> shipment_out_return = Shipment_out_Return()
     >>> shipment_out_return.customer = customer
     >>> shipment_out_return.save()
 
 Add one shipment return line::
 
     >>> move = shipment_out_return.incoming_moves.new()
     >>> move.product = product
-    >>> move.unit =unit
+    >>> move.unit = unit
     >>> move.quantity = 1
     >>> move.from_location = customer_loc
-    >>> move.to_location =  input_loc
+    >>> move.to_location = input_loc
     >>> move.company = company
     >>> move.unit_price = Decimal('1')
     >>> move.currency = company.currency
     >>> shipment_out_return.save()
 
 Test that to_location is child location on reception::
 
     >>> shipment_out_return.click('receive')
     >>> move, = shipment_out_return.inventory_moves
-    >>> move.to_location == child_loc
-    True
+    >>> assertEqual(move.to_location, child_loc)
```

### Comparing `trytond_stock_product_location-7.0.2/tox.ini` & `trytond_stock_product_location-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location-7.0.2/trytond_stock_product_location.egg-info/PKG-INFO` & `trytond_stock_product_location-7.2.0/trytond_stock_product_location.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_stock_product_location
-Version: 7.0.2
+Version: 7.2.0
 Summary: Tryton module to add default location on product
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/modules-stock-product-location
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
@@ -48,22 +48,20 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql>=0.4
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_production<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_production<7.3,>=7.2; extra == "test"
 
 Stock Product Location Module
 #############################
 
-The Stock Product Location Module adds on the product form a list of
-preferred location by warehouse. This list is used when a supplier
-shipment is received: the auto-generated Inventory Moves will use as
-default destination the preferred locations associated to the current
-warehouse.
+The *Stock Product Location Module* adds a list of preferred locations by
+warehouse and product.
+
```

### Comparing `trytond_stock_product_location-7.0.2/trytond_stock_product_location.egg-info/SOURCES.txt` & `trytond_stock_product_location-7.2.0/trytond_stock_product_location.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -42,23 +42,26 @@
 ./locale/sl.po
 ./locale/tr.po
 ./locale/uk.po
 ./locale/zh_CN.po
 ./tests/__init__.py
 ./tests/scenario_product_copy_locations.rst
 ./tests/scenario_stock_product_location.rst
+./tests/scenario_stock_product_location_consumable.rst
 ./tests/scenario_stock_product_location_production.rst
 ./tests/scenario_stock_product_location_template.rst
 ./tests/test_module.py
 ./tests/test_scenario.py
 ./view/product_form.xml
 ./view/product_location_form.xml
 ./view/product_location_tree.xml
 doc/conf.py
+doc/design.rst
 doc/index.rst
+doc/releases.rst
 doc/requirements-doc.txt
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
@@ -79,14 +82,15 @@
 locale/sl.po
 locale/tr.po
 locale/uk.po
 locale/zh_CN.po
 tests/__init__.py
 tests/scenario_product_copy_locations.rst
 tests/scenario_stock_product_location.rst
+tests/scenario_stock_product_location_consumable.rst
 tests/scenario_stock_product_location_production.rst
 tests/scenario_stock_product_location_template.rst
 tests/test_module.py
 tests/test_scenario.py
 trytond_stock_product_location.egg-info/PKG-INFO
 trytond_stock_product_location.egg-info/SOURCES.txt
 trytond_stock_product_location.egg-info/dependency_links.txt
```

