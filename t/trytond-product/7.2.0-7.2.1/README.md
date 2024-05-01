# Comparing `tmp/trytond_product-7.2.0.tar.gz` & `tmp/trytond_product-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_product-7.2.0.tar", last modified: Mon Apr 29 15:42:21 2024, max compression
+gzip compressed data, was "trytond_product-7.2.1.tar", last modified: Wed May  1 11:55:51 2024, max compression
```

## Comparing `trytond_product-7.2.0.tar` & `trytond_product-7.2.1.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:21.546413 trytond_product-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     5565 2024-04-29 15:21:14.000000 trytond_product-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      763 2024-04-29 15:21:13.000000 trytond_product-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_product-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_product-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2822 2024-04-29 15:42:21.546413 trytond_product-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      369 2024-04-27 16:30:39.000000 trytond_product-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1087 2024-04-27 16:30:39.000000 trytond_product-7.2.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3875 2024-04-27 16:30:39.000000 trytond_product-7.2.0/category.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5393 2024-04-27 16:30:39.000000 trytond_product-7.2.0/category.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2310 2024-04-27 16:30:39.000000 trytond_product-7.2.0/configuration.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2512 2024-04-27 16:30:39.000000 trytond_product-7.2.0/configuration.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:21.539746 trytond_product-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3070 2024-04-27 16:30:39.000000 trytond_product-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1230 2023-04-15 07:12:15.000000 trytond_product-7.2.0/doc/configuration.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5486 2024-01-27 09:58:52.000000 trytond_product-7.2.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      369 2024-04-27 16:30:39.000000 trytond_product-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1011 2024-04-27 16:30:39.000000 trytond_product-7.2.0/doc/reference.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_product-7.2.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:14.000000 trytond_product-7.2.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     2539 2023-04-15 07:12:15.000000 trytond_product-7.2.0/doc/usage.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      493 2023-04-15 07:12:15.000000 trytond_product-7.2.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:21.543079 trytond_product-7.2.0/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_product-7.2.0/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      244 2023-01-16 14:00:20.000000 trytond_product-7.2.0/icons/tryton-product.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      898 2023-04-15 07:12:15.000000 trytond_product-7.2.0/ir.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:21.543079 trytond_product-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    24996 2024-04-27 16:43:24.000000 trytond_product-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    26388 2024-04-27 16:43:24.000000 trytond_product-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    22448 2024-04-27 16:43:24.000000 trytond_product-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    26809 2024-04-27 16:43:24.000000 trytond_product-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    26635 2024-04-27 16:43:24.000000 trytond_product-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    22475 2024-04-27 16:43:24.000000 trytond_product-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    23000 2024-04-27 16:43:24.000000 trytond_product-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    24422 2024-04-27 16:43:24.000000 trytond_product-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    22383 2024-04-27 16:43:24.000000 trytond_product-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    26611 2024-04-27 16:43:24.000000 trytond_product-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    25122 2024-04-27 16:43:24.000000 trytond_product-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    22098 2024-04-27 16:43:24.000000 trytond_product-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    23216 2024-04-27 16:43:24.000000 trytond_product-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    25465 2024-04-27 16:43:24.000000 trytond_product-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    24117 2024-04-27 16:43:24.000000 trytond_product-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    26440 2024-04-27 16:43:24.000000 trytond_product-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    26272 2024-04-27 16:43:24.000000 trytond_product-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    23582 2024-04-27 16:43:24.000000 trytond_product-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    25936 2024-04-29 13:17:17.000000 trytond_product-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    25236 2024-04-27 16:43:24.000000 trytond_product-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    23581 2024-04-27 16:43:24.000000 trytond_product-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    23677 2024-04-27 16:43:24.000000 trytond_product-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    21311 2024-04-27 16:43:24.000000 trytond_product-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    24924 2024-04-27 16:43:24.000000 trytond_product-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2072 2024-04-27 16:30:39.000000 trytond_product-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    30204 2024-04-27 16:30:39.000000 trytond_product-7.2.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10469 2024-04-27 16:30:39.000000 trytond_product-7.2.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:42:21.546413 trytond_product-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4575 2024-04-27 16:30:39.000000 trytond_product-7.2.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:21.543079 trytond_product-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_product-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1182 2024-04-22 12:14:36.000000 trytond_product-7.2.0/tests/scenario_product_identifier.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2124 2024-04-22 12:14:36.000000 trytond_product-7.2.0/tests/scenario_product_variant.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    22022 2024-01-27 09:58:52.000000 trytond_product-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_product-7.2.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:14.000000 trytond_product-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      147 2024-04-29 15:21:09.000000 trytond_product-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:21.546413 trytond_product-7.2.0/trytond_product.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2822 2024-04-29 15:42:21.000000 trytond_product-7.2.0/trytond_product.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2778 2024-04-29 15:42:21.000000 trytond_product-7.2.0/trytond_product.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:42:21.000000 trytond_product-7.2.0/trytond_product.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       52 2024-04-29 15:42:21.000000 trytond_product-7.2.0/trytond_product.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:03.000000 trytond_product-7.2.0/trytond_product.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      122 2024-04-29 15:42:21.000000 trytond_product-7.2.0/trytond_product.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:42:21.000000 trytond_product-7.2.0/trytond_product.egg-info/top_level.txt
--rw-r--r--   0 ced       (1000) ced       (1000)    10730 2024-02-04 18:51:26.000000 trytond_product-7.2.0/uom.py
--rw-r--r--   0 ced       (1000) ced       (1000)    16944 2024-04-27 16:30:39.000000 trytond_product-7.2.0/uom.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:21.546413 trytond_product-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      661 2024-04-27 16:30:39.000000 trytond_product-7.2.0/view/category_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      319 2024-04-27 16:30:39.000000 trytond_product-7.2.0/view/category_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      307 2024-04-27 16:30:39.000000 trytond_product-7.2.0/view/category_product_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      380 2024-04-27 16:30:39.000000 trytond_product-7.2.0/view/category_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-27 16:30:39.000000 trytond_product-7.2.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      400 2023-04-15 07:12:15.000000 trytond_product-7.2.0/view/identifier_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      275 2023-04-15 07:12:15.000000 trytond_product-7.2.0/view/identifier_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      295 2023-04-15 07:12:15.000000 trytond_product-7.2.0/view/identifier_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1133 2023-04-15 07:12:15.000000 trytond_product-7.2.0/view/product_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      730 2023-04-15 07:12:15.000000 trytond_product-7.2.0/view/product_form_simple.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      263 2023-04-15 07:12:15.000000 trytond_product-7.2.0/view/product_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      226 2023-04-15 07:12:15.000000 trytond_product-7.2.0/view/product_tree_simple.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1416 2024-04-27 16:30:39.000000 trytond_product-7.2.0/view/template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      471 2023-04-15 07:12:15.000000 trytond_product-7.2.0/view/template_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      244 2023-01-16 14:00:20.000000 trytond_product-7.2.0/view/uom_category_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-04-15 07:12:15.000000 trytond_product-7.2.0/view/uom_category_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      626 2023-01-16 14:00:20.000000 trytond_product-7.2.0/view/uom_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      435 2023-04-15 07:12:15.000000 trytond_product-7.2.0/view/uom_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:55:51.852426 trytond_product-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     5666 2024-05-01 11:55:48.000000 trytond_product-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      763 2024-05-01 11:55:48.000000 trytond_product-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:20:59.000000 trytond_product-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:20:59.000000 trytond_product-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2822 2024-05-01 11:55:51.852426 trytond_product-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      369 2024-04-30 17:20:59.000000 trytond_product-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1087 2024-04-30 17:20:59.000000 trytond_product-7.2.1/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3875 2024-04-30 17:20:59.000000 trytond_product-7.2.1/category.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5393 2024-04-30 17:20:59.000000 trytond_product-7.2.1/category.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2310 2024-04-30 17:20:59.000000 trytond_product-7.2.1/configuration.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2512 2024-04-30 17:20:59.000000 trytond_product-7.2.1/configuration.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:55:51.845759 trytond_product-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3070 2024-04-30 17:20:59.000000 trytond_product-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1230 2024-04-30 17:20:59.000000 trytond_product-7.2.1/doc/configuration.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5486 2024-04-30 17:20:59.000000 trytond_product-7.2.1/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      369 2024-04-30 17:20:59.000000 trytond_product-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1011 2024-04-30 17:20:59.000000 trytond_product-7.2.1/doc/reference.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-30 17:20:59.000000 trytond_product-7.2.1/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:20:59.000000 trytond_product-7.2.1/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     2539 2024-04-30 17:20:59.000000 trytond_product-7.2.1/doc/usage.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      493 2024-04-30 17:20:59.000000 trytond_product-7.2.1/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:55:51.845759 trytond_product-7.2.1/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2024-04-30 17:20:59.000000 trytond_product-7.2.1/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      244 2024-04-30 17:20:59.000000 trytond_product-7.2.1/icons/tryton-product.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      898 2024-04-30 17:20:59.000000 trytond_product-7.2.1/ir.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:55:51.849093 trytond_product-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    25797 2024-04-30 17:21:59.000000 trytond_product-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    27299 2024-04-30 17:21:59.000000 trytond_product-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    23213 2024-04-30 17:21:59.000000 trytond_product-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    27743 2024-04-30 17:21:59.000000 trytond_product-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    27559 2024-04-30 17:21:59.000000 trytond_product-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    23248 2024-04-30 17:21:59.000000 trytond_product-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    23769 2024-04-30 17:21:59.000000 trytond_product-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    25214 2024-04-30 17:21:59.000000 trytond_product-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    23148 2024-04-30 17:21:59.000000 trytond_product-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    27525 2024-04-30 17:21:59.000000 trytond_product-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    25999 2024-04-30 17:21:59.000000 trytond_product-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    22868 2024-04-30 17:21:59.000000 trytond_product-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    23992 2024-04-30 17:21:59.000000 trytond_product-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    26291 2024-04-30 17:21:59.000000 trytond_product-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    24887 2024-04-30 17:21:59.000000 trytond_product-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    27324 2024-04-30 17:21:59.000000 trytond_product-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    27129 2024-04-30 17:21:59.000000 trytond_product-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    24360 2024-04-30 17:21:59.000000 trytond_product-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    26847 2024-04-30 17:21:59.000000 trytond_product-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    26034 2024-04-30 17:21:59.000000 trytond_product-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    24371 2024-04-30 17:21:59.000000 trytond_product-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    24448 2024-04-30 17:21:59.000000 trytond_product-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    22056 2024-04-30 17:21:59.000000 trytond_product-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    25818 2024-04-30 17:21:59.000000 trytond_product-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2072 2024-04-30 17:20:59.000000 trytond_product-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    30204 2024-04-30 17:20:59.000000 trytond_product-7.2.1/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10469 2024-04-30 17:20:59.000000 trytond_product-7.2.1/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 11:55:51.852426 trytond_product-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4575 2024-04-30 17:20:59.000000 trytond_product-7.2.1/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:55:51.849093 trytond_product-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:20:59.000000 trytond_product-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1182 2024-04-30 17:20:59.000000 trytond_product-7.2.1/tests/scenario_product_identifier.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2124 2024-04-30 17:20:59.000000 trytond_product-7.2.1/tests/scenario_product_variant.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    22022 2024-04-30 17:20:59.000000 trytond_product-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:20:59.000000 trytond_product-7.2.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:20:59.000000 trytond_product-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      147 2024-04-30 17:21:06.000000 trytond_product-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:55:51.852426 trytond_product-7.2.1/trytond_product.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2822 2024-05-01 11:55:51.000000 trytond_product-7.2.1/trytond_product.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2778 2024-05-01 11:55:51.000000 trytond_product-7.2.1/trytond_product.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:55:51.000000 trytond_product-7.2.1/trytond_product.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       52 2024-05-01 11:55:51.000000 trytond_product-7.2.1/trytond_product.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:55:51.000000 trytond_product-7.2.1/trytond_product.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      122 2024-05-01 11:55:51.000000 trytond_product-7.2.1/trytond_product.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 11:55:51.000000 trytond_product-7.2.1/trytond_product.egg-info/top_level.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)    10730 2024-04-30 17:20:59.000000 trytond_product-7.2.1/uom.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    16944 2024-04-30 17:20:59.000000 trytond_product-7.2.1/uom.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:55:51.852426 trytond_product-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      661 2024-04-30 17:20:59.000000 trytond_product-7.2.1/view/category_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      319 2024-04-30 17:20:59.000000 trytond_product-7.2.1/view/category_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      307 2024-04-30 17:20:59.000000 trytond_product-7.2.1/view/category_product_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      380 2024-04-30 17:20:59.000000 trytond_product-7.2.1/view/category_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:20:59.000000 trytond_product-7.2.1/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      400 2024-04-30 17:20:59.000000 trytond_product-7.2.1/view/identifier_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      275 2024-04-30 17:20:59.000000 trytond_product-7.2.1/view/identifier_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      295 2024-04-30 17:20:59.000000 trytond_product-7.2.1/view/identifier_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1133 2024-04-30 17:20:59.000000 trytond_product-7.2.1/view/product_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      730 2024-04-30 17:20:59.000000 trytond_product-7.2.1/view/product_form_simple.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      263 2024-04-30 17:20:59.000000 trytond_product-7.2.1/view/product_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      226 2024-04-30 17:20:59.000000 trytond_product-7.2.1/view/product_tree_simple.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1416 2024-04-30 17:20:59.000000 trytond_product-7.2.1/view/template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      471 2024-04-30 17:20:59.000000 trytond_product-7.2.1/view/template_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      244 2024-04-30 17:20:59.000000 trytond_product-7.2.1/view/uom_category_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2024-04-30 17:20:59.000000 trytond_product-7.2.1/view/uom_category_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      626 2024-04-30 17:20:59.000000 trytond_product-7.2.1/view/uom_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      435 2024-04-30 17:20:59.000000 trytond_product-7.2.1/view/uom_tree.xml
```

### Comparing `trytond_product-7.2.0/CHANGELOG` & `trytond_product-7.2.1/CHANGELOG`

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
 * Add Manufacturer Part Number product identifier
 * Add brand product identifier
 * Support generate barcode of different type
 * Add code on product category
```

### Comparing `trytond_product-7.2.0/COPYRIGHT` & `trytond_product-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_product-7.2.0/LICENSE` & `trytond_product-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_product-7.2.0/PKG-INFO` & `trytond_product-7.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_product
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module with products
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_product-7.2.0/__init__.py` & `trytond_product-7.2.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_product-7.2.0/category.py` & `trytond_product-7.2.1/category.py`

 * *Files identical despite different names*

### Comparing `trytond_product-7.2.0/category.xml` & `trytond_product-7.2.1/category.xml`

 * *Files identical despite different names*

### Comparing `trytond_product-7.2.0/configuration.py` & `trytond_product-7.2.1/configuration.py`

 * *Files identical despite different names*

### Comparing `trytond_product-7.2.0/configuration.xml` & `trytond_product-7.2.1/configuration.xml`

 * *Files identical despite different names*

### Comparing `trytond_product-7.2.0/doc/conf.py` & `trytond_product-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_product-7.2.0/doc/configuration.rst` & `trytond_product-7.2.1/doc/configuration.rst`

 * *Files identical despite different names*

### Comparing `trytond_product-7.2.0/doc/design.rst` & `trytond_product-7.2.1/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_product-7.2.0/doc/reference.rst` & `trytond_product-7.2.1/doc/reference.rst`

 * *Files identical despite different names*

### Comparing `trytond_product-7.2.0/doc/usage.rst` & `trytond_product-7.2.1/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `trytond_product-7.2.0/icons/LICENSE` & `trytond_product-7.2.1/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_product-7.2.0/ir.py` & `trytond_product-7.2.1/ir.py`

 * *Files identical despite different names*

### Comparing `trytond_product-7.2.0/locale/bg.po` & `trytond_product-7.2.1/locale/ru.po`

 * *Files 3% similar despite different names*

```diff
@@ -1,65 +1,79 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 #, fuzzy
 msgctxt "field:ir.configuration,product_price_decimal:"
 msgid "Product Price Decimal"
-msgstr "Продукт"
+msgstr "Вид продукта"
 
 msgctxt "field:product.category,childs:"
 msgid "Children"
-msgstr "Наследници"
+msgstr "Подчиненные"
+
+#, fuzzy
+msgctxt "field:product.category,code:"
+msgid "Code"
+msgstr "Код"
+
+msgctxt "field:product.category,code_readonly:"
+msgid "Code Readonly"
+msgstr ""
 
 msgctxt "field:product.category,name:"
 msgid "Name"
-msgstr "Име"
+msgstr "Наименование"
 
 msgctxt "field:product.category,parent:"
 msgid "Parent"
-msgstr "Родител"
+msgstr "Предок"
 
 #, fuzzy
 msgctxt "field:product.category,templates:"
 msgid "Products"
-msgstr "Продукти по местонахождения"
+msgstr "Products"
+
+#, fuzzy
+msgctxt "field:product.configuration,category_sequence:"
+msgid "Category Sequence"
+msgstr "Шаблон продукта"
 
 msgctxt "field:product.configuration,default_cost_price_method:"
 msgid "Default Cost Method"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:product.configuration,product_sequence:"
 msgid "Variant Sequence"
-msgstr "Щаблон за продукт"
+msgstr "Шаблон продукта"
 
 #, fuzzy
 msgctxt "field:product.configuration,template_sequence:"
 msgid "Product Sequence"
-msgstr "Щаблон за продукт"
+msgstr "Шаблон продукта"
 
 msgctxt ""
 "field:product.configuration.default_cost_price_method,default_cost_price_method:"
 msgid "Default Cost Method"
 msgstr ""
 
 msgctxt "field:product.cost_price,company:"
 msgid "Company"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:product.cost_price,cost_price:"
 msgid "Cost Price"
-msgstr "Фабрична цена"
+msgstr "Себестоимость"
 
 #, fuzzy
 msgctxt "field:product.cost_price,product:"
 msgid "Product"
-msgstr "Продукт"
+msgstr "Продукция"
 
 msgctxt "field:product.cost_price_method,company:"
 msgid "Company"
 msgstr ""
 
 msgctxt "field:product.cost_price_method,cost_price_method:"
 msgid "Cost Price Method"
@@ -74,29 +88,29 @@
 msgctxt "field:product.identifier,code:"
 msgid "Code"
 msgstr "Код"
 
 #, fuzzy
 msgctxt "field:product.identifier,product:"
 msgid "Product"
-msgstr "Продукт"
+msgstr "Продукция"
 
 #, fuzzy
 msgctxt "field:product.identifier,type:"
 msgid "Type"
-msgstr "Вид"
+msgstr "Тип"
 
 msgctxt "field:product.list_price,company:"
 msgid "Company"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:product.list_price,list_price:"
 msgid "List Price"
-msgstr "Каталожна цена"
+msgstr "Цена"
 
 #, fuzzy
 msgctxt "field:product.list_price,template:"
 msgid "Template"
 msgstr "Шаблон"
 
 #, fuzzy
@@ -116,93 +130,90 @@
 msgctxt "field:product.product,code_readonly:"
 msgid "Code Readonly"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:product.product,consumable:"
 msgid "Consumable"
-msgstr "Консуматив"
+msgstr "Потребляемый"
 
 #, fuzzy
 msgctxt "field:product.product,cost_price:"
 msgid "Cost Price"
-msgstr "Фабрична цена"
+msgstr "Себестоимость"
 
 msgctxt "field:product.product,cost_price_method:"
 msgid "Cost Price Method"
 msgstr ""
 
 msgctxt "field:product.product,cost_price_methods:"
 msgid "Cost Price Methods"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:product.product,cost_price_uom:"
 msgid "Cost Price"
-msgstr "Фабрична цена"
+msgstr "Себестоимость"
 
 #, fuzzy
 msgctxt "field:product.product,cost_prices:"
 msgid "Cost Prices"
-msgstr "Фабрична цена"
+msgstr "Себестоимость"
 
 #, fuzzy
 msgctxt "field:product.product,default_uom:"
 msgid "Default UoM"
-msgstr "Мер. ед. по подрабиране"
+msgstr "Ед.измерения по умолчанию"
 
 #, fuzzy
 msgctxt "field:product.product,default_uom_category:"
 msgid "Default UoM Category"
-msgstr "Категория мер. ед. по подразбиране"
+msgstr "Категория ед.измерения по умолчанию"
 
 msgctxt "field:product.product,description:"
 msgid "Description"
 msgstr "Описание"
 
 msgctxt "field:product.product,identifiers:"
 msgid "Identifiers"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:product.product,list_price:"
 msgid "List Price"
-msgstr "Каталожна цена"
+msgstr "Цена"
 
-#, fuzzy
 msgctxt "field:product.product,list_price_uom:"
 msgid "List Price"
-msgstr "Каталожна цена"
+msgstr "Цена"
 
 #, fuzzy
 msgctxt "field:product.product,list_prices:"
 msgid "List Prices"
-msgstr "Каталожна цена"
+msgstr "Цена"
 
 #, fuzzy
 msgctxt "field:product.product,name:"
 msgid "Name"
-msgstr "Име"
+msgstr "Наименование"
 
 msgctxt "field:product.product,prefix_code:"
 msgid "Prefix Code"
 msgstr ""
 
 msgctxt "field:product.product,suffix_code:"
 msgid "Suffix Code"
 msgstr ""
 
 msgctxt "field:product.product,template:"
 msgid "Product Template"
-msgstr "Щаблон за продукт"
+msgstr "Шаблон продукта"
 
-#, fuzzy
 msgctxt "field:product.product,type:"
 msgid "Type"
-msgstr "Вид"
+msgstr "Тип"
 
 #, fuzzy
 msgctxt "field:product.template,categories:"
 msgid "Categories"
 msgstr "Категории"
 
 #, fuzzy
@@ -217,59 +228,58 @@
 
 msgctxt "field:product.template,code_readonly:"
 msgid "Code Readonly"
 msgstr ""
 
 msgctxt "field:product.template,consumable:"
 msgid "Consumable"
-msgstr "Консуматив"
+msgstr "Потребляемый"
 
 msgctxt "field:product.template,cost_price:"
 msgid "Cost Price"
-msgstr "Фабрична цена"
+msgstr "Себестоимость"
 
 msgctxt "field:product.template,cost_price_method:"
 msgid "Cost Price Method"
 msgstr ""
 
 msgctxt "field:product.template,cost_price_methods:"
 msgid "Cost Price Methods"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:product.template,default_uom:"
 msgid "Default UoM"
-msgstr "Мер. ед. по подрабиране"
+msgstr "Ед.измерения по умолчанию"
 
 #, fuzzy
 msgctxt "field:product.template,default_uom_category:"
 msgid "Default UoM Category"
-msgstr "Категория мер. ед. по подразбиране"
+msgstr "Категория ед.измерения по умолчанию"
 
 msgctxt "field:product.template,list_price:"
 msgid "List Price"
-msgstr "Каталожна цена"
+msgstr "Цена"
 
 #, fuzzy
 msgctxt "field:product.template,list_prices:"
 msgid "List Prices"
-msgstr "Каталожна цена"
+msgstr "Цена"
 
 msgctxt "field:product.template,name:"
 msgid "Name"
-msgstr "Име"
+msgstr "Наименование"
 
-#, fuzzy
 msgctxt "field:product.template,products:"
 msgid "Variants"
-msgstr "Продукти"
+msgstr "Разновидности"
 
 msgctxt "field:product.template,type:"
 msgid "Type"
-msgstr "Вид"
+msgstr "Тип"
 
 #, fuzzy
 msgctxt "field:product.template-product.category,category:"
 msgid "Category"
 msgstr "Категория"
 
 #, fuzzy
@@ -286,57 +296,61 @@
 msgctxt "field:product.template-product.category.all,template:"
 msgid "Template"
 msgstr "Шаблон"
 
 #, fuzzy
 msgctxt "field:product.uom,category:"
 msgid "Category"
-msgstr "Категория мер. ед."
+msgstr "Категория ед. измерения"
 
 msgctxt "field:product.uom,digits:"
 msgid "Display Digits"
-msgstr "Цифри за показване"
+msgstr "Кол-во знаков после запятой"
 
 msgctxt "field:product.uom,factor:"
 msgid "Factor"
-msgstr "Коефициент"
+msgstr "Коэффициент к основной единице"
 
 msgctxt "field:product.uom,name:"
 msgid "Name"
-msgstr "Име"
+msgstr "Наименование"
 
 msgctxt "field:product.uom,rate:"
 msgid "Rate"
-msgstr "Отношение"
+msgstr "Коэфициент основной единицы"
 
 msgctxt "field:product.uom,rounding:"
 msgid "Rounding Precision"
-msgstr "Точност на закръгление"
+msgstr "Точность округления"
 
 msgctxt "field:product.uom,symbol:"
 msgid "Symbol"
-msgstr "Символ"
+msgstr "Условное обозначение"
 
 msgctxt "field:product.uom.category,name:"
 msgid "Name"
-msgstr "Име"
+msgstr "Наименование"
 
 #, fuzzy
 msgctxt "field:product.uom.category,uoms:"
 msgid "Units of Measure"
 msgstr "Units of Measure"
 
 msgctxt "help:product.category,childs:"
 msgid "Used to add structure below the category."
 msgstr ""
 
 msgctxt "help:product.category,parent:"
 msgid "Used to add structure above the category."
 msgstr ""
 
+msgctxt "help:product.configuration,category_sequence:"
+msgid "Used to generate the category code."
+msgstr ""
+
 msgctxt "help:product.configuration,default_cost_price_method:"
 msgid "The default cost price method for new products."
 msgstr ""
 
 msgctxt "help:product.configuration,product_sequence:"
 msgid "Used to generate the last part of the product code."
 msgstr ""
@@ -383,15 +397,15 @@
 "The standard Unit of Measure for the product.\n"
 "Used internally when calculating the stock levels of goods and assets."
 msgstr ""
 
 #, fuzzy
 msgctxt "help:product.product,default_uom_category:"
 msgid "The category of the default Unit of Measure."
-msgstr "Категория мерни единици"
+msgstr "Категория ед.измерения"
 
 msgctxt "help:product.product,identifiers:"
 msgid "Other identifiers associated with the variant."
 msgstr ""
 
 msgctxt "help:product.product,list_price:"
 msgid "The standard price the product is sold at."
@@ -431,15 +445,15 @@
 "The standard Unit of Measure for the product.\n"
 "Used internally when calculating the stock levels of goods and assets."
 msgstr ""
 
 #, fuzzy
 msgctxt "help:product.template,default_uom_category:"
 msgid "The category of the default Unit of Measure."
-msgstr "Категория мерни единици"
+msgstr "Категория ед.измерения"
 
 msgctxt "help:product.template,list_price:"
 msgid "The standard price the product is sold at."
 msgstr ""
 
 msgctxt "help:product.template,products:"
 msgid "The different variants the product comes in."
@@ -457,24 +471,24 @@
 
 #, fuzzy
 msgctxt "help:product.uom,factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "coefficient (base unit) = 1 (this unit)"
 msgstr ""
-"Коефициент в тази формула:\n"
-"1 (баз. единица) = коеф. (тази единица)"
+"Коэффициент по формуле:\n"
+"коэффициент в этом поле (базовая единица) = 1 (этой ед. измерения)"
 
 msgctxt "help:product.uom,rate:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (base unit) = coef (this unit)"
 msgstr ""
-"Коефициент в тази формула:\n"
-"1 (баз. единица) = коеф. (тази единица)"
+"Коэффициент по формуле:\n"
+"1 (базовая единица) = коэффициенту (этой ед.измерения)"
 
 msgctxt "help:product.uom,rounding:"
 msgid "The accuracy to which values are rounded."
 msgstr ""
 
 msgctxt "help:product.uom,symbol:"
 msgid "The symbol that represents the unit of measure."
@@ -484,56 +498,60 @@
 msgctxt "model:ir.action,name:act_category_list"
 msgid "Categories"
 msgstr "Categories"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_category_product"
 msgid "Add products"
-msgstr "Продукти по местонахождения"
+msgstr "Products"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_category_tree"
 msgid "Categories"
 msgstr "Categories"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_product_configuration_form"
 msgid "Configuration"
-msgstr "Настройки"
+msgstr "Конфигурация"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_product_form"
 msgid "Variants"
-msgstr "Продукти"
+msgstr "Variants"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_product_from_template"
 msgid "Variants"
-msgstr "Продукти"
+msgstr "Разновидности"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_template_by_category"
 msgid "Product by Category"
-msgstr "Категория на продукт"
+msgstr "Product by Category"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_template_form"
 msgid "Products"
-msgstr "Продукти по местонахождения"
+msgstr "Products"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_uom_category_form"
 msgid "Categories"
 msgstr "Категории"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_uom_form"
 msgid "Units of Measure"
 msgstr "Units of Measure"
 
+msgctxt "model:ir.message,text:msg_category_code_unique"
+msgid "The code on product category must be unique."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_invalid_code"
 msgid "The %(type)s \"%(code)s\" for product \"%(product)s\" is not valid."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_product_code_unique"
 msgid "Code of active product must be unique."
 msgstr ""
@@ -567,78 +585,83 @@
 msgctxt "model:ir.message,text:msg_uom_no_zero_factor_rate"
 msgid "Rate and factor can not be both equal to zero."
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.model.button,string:category_add_products_button"
 msgid "Add products"
-msgstr "Продукти по местонахождения"
+msgstr "Products"
+
+#, fuzzy
+msgctxt "model:ir.sequence.type,name:sequence_type_category"
+msgid "Category"
+msgstr "Категория"
 
 #, fuzzy
 msgctxt "model:ir.sequence.type,name:sequence_type_product"
 msgid "Variant"
-msgstr "Продукти"
+msgstr "Разновидности"
 
 #, fuzzy
 msgctxt "model:ir.sequence.type,name:sequence_type_template"
 msgid "Product"
-msgstr "Продукт"
+msgstr "Продукция"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_category_list"
 msgid "Categories"
 msgstr "Categories"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_category_tree"
 msgid "Categories"
 msgstr "Categories"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_configuration"
 msgid "Configuration"
-msgstr "Настройки"
+msgstr "Конфигурация"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_main_product"
 msgid "Products"
-msgstr "Продукти по местонахождения"
+msgstr "Products"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_product"
 msgid "Variants"
-msgstr "Продукти"
+msgstr "Variants"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_product_configuration"
 msgid "Configuration"
-msgstr "Настройки"
+msgstr "Конфигурация"
 
 msgctxt "model:ir.ui.menu,name:menu_reporting"
 msgid "Reporting"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_template"
 msgid "Products"
-msgstr "Продукти по местонахождения"
+msgstr "Products"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_uom_category_form"
 msgid "Categories"
 msgstr "Categories"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_uom_form"
 msgid "Units of Measure"
 msgstr "Units of Measure"
 
 msgctxt "model:product.category,name:"
 msgid "Product Category"
-msgstr "Категория на продукт"
+msgstr "Категория продукции"
 
 #, fuzzy
 msgctxt "model:product.configuration,name:"
 msgid "Product Configuration"
 msgstr "Product Configuration"
 
 msgctxt "model:product.configuration.default_cost_price_method,name:"
@@ -652,41 +675,40 @@
 msgctxt "model:product.cost_price_method,name:"
 msgid "Product Cost Price Method"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:product.identifier,name:"
 msgid "Product Identifier"
-msgstr "Щаблон за продукт"
+msgstr "Шаблон продукта"
 
 msgctxt "model:product.list_price,name:"
 msgid "Product List Price"
 msgstr ""
 
-#, fuzzy
 msgctxt "model:product.product,name:"
 msgid "Product Variant"
-msgstr "Продукт"
+msgstr "Вид продукта"
 
 msgctxt "model:product.template,name:"
 msgid "Product Template"
-msgstr "Щаблон за продукт"
+msgstr "Шаблон продукта"
 
 msgctxt "model:product.template-product.category,name:"
 msgid "Template - Category"
 msgstr ""
 
 msgctxt "model:product.template-product.category.all,name:"
 msgid "Template - Category All"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:product.uom,name:"
 msgid "Unit of Measure"
-msgstr "Мерни единици"
+msgstr "Единица измерения"
 
 #, fuzzy
 msgctxt "model:product.uom,name:uom_are"
 msgid "Are"
 msgstr "Are"
 
 #, fuzzy
@@ -851,42 +873,50 @@
 msgstr "Unit"
 
 #, fuzzy
 msgctxt "model:product.uom,name:uom_yard"
 msgid "Yard"
 msgstr "Yard"
 
+#, fuzzy
 msgctxt "model:product.uom,symbol:uom_are"
 msgid "a"
 msgstr "a"
 
+#, fuzzy
 msgctxt "model:product.uom,symbol:uom_carat"
 msgid "c"
 msgstr "c"
 
+#, fuzzy
 msgctxt "model:product.uom,symbol:uom_centimeter"
 msgid "cm"
 msgstr "cm"
 
+#, fuzzy
 msgctxt "model:product.uom,symbol:uom_cubic_centimeter"
 msgid "cm³"
 msgstr "cm³"
 
+#, fuzzy
 msgctxt "model:product.uom,symbol:uom_cubic_foot"
 msgid "ft³"
 msgstr "ft³"
 
+#, fuzzy
 msgctxt "model:product.uom,symbol:uom_cubic_inch"
 msgid "in³"
 msgstr "in³"
 
+#, fuzzy
 msgctxt "model:product.uom,symbol:uom_cubic_meter"
 msgid "m³"
 msgstr "m³"
 
+#, fuzzy
 msgctxt "model:product.uom,symbol:uom_day"
 msgid "d"
 msgstr "d"
 
 msgctxt "model:product.uom,symbol:uom_energy_joule"
 msgid "J"
 msgstr ""
@@ -899,111 +929,133 @@
 msgid "MJ"
 msgstr ""
 
 msgctxt "model:product.uom,symbol:uom_energy_mwh"
 msgid "MW⋅h"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:product.uom,symbol:uom_foot"
 msgid "ft"
 msgstr "ft"
 
+#, fuzzy
 msgctxt "model:product.uom,symbol:uom_gallon"
 msgid "gal"
 msgstr "gal"
 
+#, fuzzy
 msgctxt "model:product.uom,symbol:uom_gram"
 msgid "g"
 msgstr "g"
 
+#, fuzzy
 msgctxt "model:product.uom,symbol:uom_hectare"
 msgid "ha"
 msgstr "ha"
 
+#, fuzzy
 msgctxt "model:product.uom,symbol:uom_hour"
 msgid "h"
 msgstr "h"
 
+#, fuzzy
 msgctxt "model:product.uom,symbol:uom_inch"
 msgid "in"
 msgstr "in"
 
+#, fuzzy
 msgctxt "model:product.uom,symbol:uom_kilogram"
 msgid "kg"
 msgstr "kg"
 
+#, fuzzy
 msgctxt "model:product.uom,symbol:uom_kilometer"
 msgid "km"
 msgstr "km"
 
+#, fuzzy
 msgctxt "model:product.uom,symbol:uom_liter"
 msgid "l"
 msgstr "l"
 
+#, fuzzy
 msgctxt "model:product.uom,symbol:uom_meter"
 msgid "m"
 msgstr "m"
 
+#, fuzzy
 msgctxt "model:product.uom,symbol:uom_mile"
 msgid "mi"
 msgstr "mi"
 
+#, fuzzy
 msgctxt "model:product.uom,symbol:uom_millimeter"
 msgid "mm"
 msgstr "mm"
 
+#, fuzzy
 msgctxt "model:product.uom,symbol:uom_minute"
 msgid "min"
 msgstr "min"
 
+#, fuzzy
 msgctxt "model:product.uom,symbol:uom_ounce"
 msgid "oz"
 msgstr "oz"
 
 #, fuzzy
 msgctxt "model:product.uom,symbol:uom_pound"
 msgid "lb"
-msgstr "lbs"
+msgstr "фунт"
 
+#, fuzzy
 msgctxt "model:product.uom,symbol:uom_second"
 msgid "s"
 msgstr "s"
 
+#, fuzzy
 msgctxt "model:product.uom,symbol:uom_square_centimeter"
 msgid "cm²"
 msgstr "cm²"
 
+#, fuzzy
 msgctxt "model:product.uom,symbol:uom_square_foot"
 msgid "ft²"
 msgstr "ft²"
 
+#, fuzzy
 msgctxt "model:product.uom,symbol:uom_square_inch"
 msgid "in²"
 msgstr "in²"
 
+#, fuzzy
 msgctxt "model:product.uom,symbol:uom_square_meter"
 msgid "m²"
 msgstr "m²"
 
+#, fuzzy
 msgctxt "model:product.uom,symbol:uom_square_yard"
 msgid "yd²"
 msgstr "yd²"
 
+#, fuzzy
 msgctxt "model:product.uom,symbol:uom_unit"
 msgid "u"
 msgstr "u"
 
+#, fuzzy
 msgctxt "model:product.uom,symbol:uom_yard"
 msgid "yd"
 msgstr "yd"
 
 #, fuzzy
 msgctxt "model:product.uom.category,name:"
 msgid "Unit of Measure Category"
-msgstr "Мерни единици"
+msgstr "Единица измерения"
 
 msgctxt "model:product.uom.category,name:uom_cat_energy"
 msgid "Energy"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:product.uom.category,name:uom_cat_length"
@@ -1037,14 +1089,18 @@
 
 #, fuzzy
 msgctxt "model:res.group,name:group_product_admin"
 msgid "Product Administration"
 msgstr "Product Administration"
 
 msgctxt "selection:product.identifier,type:"
+msgid "Brand"
+msgstr ""
+
+msgctxt "selection:product.identifier,type:"
 msgid "International Article Number"
 msgstr ""
 
 msgctxt "selection:product.identifier,type:"
 msgid "International Securities Identification Number"
 msgstr ""
 
@@ -1060,64 +1116,65 @@
 msgid "International Standard Identifier for Libraries"
 msgstr ""
 
 msgctxt "selection:product.identifier,type:"
 msgid "International Standard Music Number"
 msgstr ""
 
+msgctxt "selection:product.identifier,type:"
+msgid "Manufacturer Part Number"
+msgstr ""
+
 #, fuzzy
 msgctxt "selection:product.product,cost_price_method:"
 msgid "Average"
-msgstr "Средна"
+msgstr "Средняя цена"
 
 #, fuzzy
 msgctxt "selection:product.product,cost_price_method:"
 msgid "Fixed"
-msgstr "Фиксирана"
+msgstr "Фиксированная цена"
 
-#, fuzzy
 msgctxt "selection:product.product,type:"
 msgid "Assets"
-msgstr "Активи"
+msgstr "Активы"
 
-#, fuzzy
 msgctxt "selection:product.product,type:"
 msgid "Goods"
-msgstr "Стока"
+msgstr "Товары"
 
-#, fuzzy
 msgctxt "selection:product.product,type:"
 msgid "Service"
-msgstr "Услуга"
+msgstr "Услуги"
 
 msgctxt "selection:product.template,cost_price_method:"
 msgid "Average"
-msgstr "Средна"
+msgstr "Средняя цена"
 
 msgctxt "selection:product.template,cost_price_method:"
 msgid "Fixed"
-msgstr "Фиксирана"
+msgstr "Фиксированная цена"
 
 msgctxt "selection:product.template,type:"
 msgid "Assets"
-msgstr "Активи"
+msgstr "Активы"
 
 msgctxt "selection:product.template,type:"
 msgid "Goods"
-msgstr "Стока"
+msgstr "Товары"
 
 msgctxt "selection:product.template,type:"
 msgid "Service"
-msgstr "Услуга"
+msgstr "Услуги"
 
 msgctxt "view:product.category:"
 msgid "Children"
-msgstr "Наследници"
+msgstr "Подчиненные"
 
 #, fuzzy
 msgctxt "view:product.configuration:"
 msgid "Sequences"
-msgstr "Щаблон за продукт"
+msgstr "Шаблон продукта"
 
 msgctxt "view:product.template:"
 msgid "General"
-msgstr "Основен"
+msgstr "Основные"
```

### Comparing `trytond_product-7.2.0/locale/ca.po` & `trytond_product-7.2.1/locale/ca.po`

 * *Files 2% similar despite different names*

```diff
@@ -6,26 +6,38 @@
 msgid "Product Price Decimal"
 msgstr "Decimals del preu de cost del producte"
 
 msgctxt "field:product.category,childs:"
 msgid "Children"
 msgstr "Fills"
 
+msgctxt "field:product.category,code:"
+msgid "Code"
+msgstr "Codi"
+
+msgctxt "field:product.category,code_readonly:"
+msgid "Code Readonly"
+msgstr "Codi només lectura"
+
 msgctxt "field:product.category,name:"
 msgid "Name"
 msgstr "Nom"
 
 msgctxt "field:product.category,parent:"
 msgid "Parent"
 msgstr "Pare"
 
 msgctxt "field:product.category,templates:"
 msgid "Products"
 msgstr "Productes"
 
+msgctxt "field:product.configuration,category_sequence:"
+msgid "Category Sequence"
+msgstr "Seqüència de la categoria"
+
 msgctxt "field:product.configuration,default_cost_price_method:"
 msgid "Default Cost Method"
 msgstr "Mètode de cost per defecte"
 
 msgctxt "field:product.configuration,product_sequence:"
 msgid "Variant Sequence"
 msgstr "Seqüencia de la variant"
@@ -185,15 +197,15 @@
 
 msgctxt "field:product.template,code:"
 msgid "Code"
 msgstr "Codi"
 
 msgctxt "field:product.template,code_readonly:"
 msgid "Code Readonly"
-msgstr "Code només lectura"
+msgstr "Codi només lectura"
 
 msgctxt "field:product.template,consumable:"
 msgid "Consumable"
 msgstr "Consumible"
 
 msgctxt "field:product.template,cost_price:"
 msgid "Cost Price"
@@ -291,14 +303,18 @@
 msgid "Used to add structure below the category."
 msgstr "Utilitzat per afegir una estructura per sota la categoria."
 
 msgctxt "help:product.category,parent:"
 msgid "Used to add structure above the category."
 msgstr "Utilitzat per afegir una estructura per sobre la categoria."
 
+msgctxt "help:product.configuration,category_sequence:"
+msgid "Used to generate the category code."
+msgstr "Utilitzada per generar el codi de la categoria."
+
 msgctxt "help:product.configuration,default_cost_price_method:"
 msgid "The default cost price method for new products."
 msgstr "El mètode de cost per defecte per als nous productes."
 
 msgctxt "help:product.configuration,product_sequence:"
 msgid "Used to generate the last part of the product code."
 msgstr "Utilitzada per generar la part final del codi del producte."
@@ -492,14 +508,18 @@
 msgid "Categories"
 msgstr "Categories"
 
 msgctxt "model:ir.action,name:act_uom_form"
 msgid "Units of Measure"
 msgstr "Unitats de mesura"
 
+msgctxt "model:ir.message,text:msg_category_code_unique"
+msgid "The code on product category must be unique."
+msgstr "El codi de la categoria de producte ha de ser únic."
+
 msgctxt "model:ir.message,text:msg_invalid_code"
 msgid "The %(type)s \"%(code)s\" for product \"%(product)s\" is not valid."
 msgstr "El \"%(type)s\" \"%(code)s\" del producte \"%(product)s\" no és vàlid."
 
 msgctxt "model:ir.message,text:msg_product_code_unique"
 msgid "Code of active product must be unique."
 msgstr "El codi dels productes actius ha de ser únic."
@@ -536,14 +556,18 @@
 msgid "Rate and factor can not be both equal to zero."
 msgstr "El rati i el factor no poden ser els dos igual a zero."
 
 msgctxt "model:ir.model.button,string:category_add_products_button"
 msgid "Add products"
 msgstr "Afegeix productes"
 
+msgctxt "model:ir.sequence.type,name:sequence_type_category"
+msgid "Category"
+msgstr "Categoria"
+
 msgctxt "model:ir.sequence.type,name:sequence_type_product"
 msgid "Variant"
 msgstr "Variant"
 
 msgctxt "model:ir.sequence.type,name:sequence_type_template"
 msgid "Product"
 msgstr "Producte"
@@ -949,14 +973,18 @@
 msgstr "Pes"
 
 msgctxt "model:res.group,name:group_product_admin"
 msgid "Product Administration"
 msgstr "Administració de productes"
 
 msgctxt "selection:product.identifier,type:"
+msgid "Brand"
+msgstr "Marca"
+
+msgctxt "selection:product.identifier,type:"
 msgid "International Article Number"
 msgstr "Número d'article internacional (EAN)"
 
 msgctxt "selection:product.identifier,type:"
 msgid "International Securities Identification Number"
 msgstr "Número Internacional d'itenficador de Valors (ISIN)"
 
@@ -972,14 +1000,18 @@
 msgid "International Standard Identifier for Libraries"
 msgstr "Número estàndard Internacional del Lllibreries (ISIL)"
 
 msgctxt "selection:product.identifier,type:"
 msgid "International Standard Music Number"
 msgstr "Número estàndard Internacional de Música (ISMN)"
 
+msgctxt "selection:product.identifier,type:"
+msgid "Manufacturer Part Number"
+msgstr "Número de peça del fabricant"
+
 msgctxt "selection:product.product,cost_price_method:"
 msgid "Average"
 msgstr "Mitjana"
 
 msgctxt "selection:product.product,cost_price_method:"
 msgid "Fixed"
 msgstr "Fix"
```

### Comparing `trytond_product-7.2.0/locale/cs.po` & `trytond_product-7.2.1/locale/fi.po`

 * *Files 2% similar despite different names*

```diff
@@ -6,28 +6,40 @@
 msgid "Product Price Decimal"
 msgstr ""
 
 msgctxt "field:product.category,childs:"
 msgid "Children"
 msgstr ""
 
-#, fuzzy
+msgctxt "field:product.category,code:"
+msgid "Code"
+msgstr ""
+
+msgctxt "field:product.category,code_readonly:"
+msgid "Code Readonly"
+msgstr ""
+
 msgctxt "field:product.category,name:"
 msgid "Name"
-msgstr "Namu"
+msgstr ""
 
 msgctxt "field:product.category,parent:"
 msgid "Parent"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:product.category,templates:"
 msgid "Products"
 msgstr "Products"
 
+#, fuzzy
+msgctxt "field:product.configuration,category_sequence:"
+msgid "Category Sequence"
+msgstr "Product by Category"
+
 msgctxt "field:product.configuration,default_cost_price_method:"
 msgid "Default Cost Method"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:product.configuration,product_sequence:"
 msgid "Variant Sequence"
@@ -160,18 +172,17 @@
 msgid "List Price"
 msgstr ""
 
 msgctxt "field:product.product,list_prices:"
 msgid "List Prices"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:product.product,name:"
 msgid "Name"
-msgstr "Namu"
+msgstr ""
 
 msgctxt "field:product.product,prefix_code:"
 msgid "Prefix Code"
 msgstr ""
 
 msgctxt "field:product.product,suffix_code:"
 msgid "Suffix Code"
@@ -232,18 +243,17 @@
 msgid "List Price"
 msgstr ""
 
 msgctxt "field:product.template,list_prices:"
 msgid "List Prices"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:product.template,name:"
 msgid "Name"
-msgstr "Namu"
+msgstr ""
 
 #, fuzzy
 msgctxt "field:product.template,products:"
 msgid "Variants"
 msgstr "Variants"
 
 msgctxt "field:product.template,type:"
@@ -274,49 +284,51 @@
 msgid "Display Digits"
 msgstr ""
 
 msgctxt "field:product.uom,factor:"
 msgid "Factor"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:product.uom,name:"
 msgid "Name"
-msgstr "Namu"
+msgstr ""
 
 msgctxt "field:product.uom,rate:"
 msgid "Rate"
 msgstr ""
 
 msgctxt "field:product.uom,rounding:"
 msgid "Rounding Precision"
 msgstr ""
 
 msgctxt "field:product.uom,symbol:"
 msgid "Symbol"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:product.uom.category,name:"
 msgid "Name"
-msgstr "Namu"
+msgstr ""
 
 #, fuzzy
 msgctxt "field:product.uom.category,uoms:"
 msgid "Units of Measure"
 msgstr "Units of Measure"
 
 msgctxt "help:product.category,childs:"
 msgid "Used to add structure below the category."
 msgstr ""
 
 msgctxt "help:product.category,parent:"
 msgid "Used to add structure above the category."
 msgstr ""
 
+msgctxt "help:product.configuration,category_sequence:"
+msgid "Used to generate the category code."
+msgstr ""
+
 msgctxt "help:product.configuration,default_cost_price_method:"
 msgid "The default cost price method for new products."
 msgstr ""
 
 msgctxt "help:product.configuration,product_sequence:"
 msgid "Used to generate the last part of the product code."
 msgstr ""
@@ -494,14 +506,18 @@
 msgid "Categories"
 msgstr "Categories"
 
 msgctxt "model:ir.action,name:act_uom_form"
 msgid "Units of Measure"
 msgstr "Units of Measure"
 
+msgctxt "model:ir.message,text:msg_category_code_unique"
+msgid "The code on product category must be unique."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_invalid_code"
 msgid "The %(type)s \"%(code)s\" for product \"%(product)s\" is not valid."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_product_code_unique"
 msgid "Code of active product must be unique."
 msgstr ""
@@ -538,14 +554,19 @@
 
 #, fuzzy
 msgctxt "model:ir.model.button,string:category_add_products_button"
 msgid "Add products"
 msgstr "Products"
 
 #, fuzzy
+msgctxt "model:ir.sequence.type,name:sequence_type_category"
+msgid "Category"
+msgstr "Categories"
+
+#, fuzzy
 msgctxt "model:ir.sequence.type,name:sequence_type_product"
 msgid "Variant"
 msgstr "Variants"
 
 #, fuzzy
 msgctxt "model:ir.sequence.type,name:sequence_type_template"
 msgid "Product"
@@ -960,14 +981,18 @@
 msgstr "Weight"
 
 msgctxt "model:res.group,name:group_product_admin"
 msgid "Product Administration"
 msgstr "Product Administration"
 
 msgctxt "selection:product.identifier,type:"
+msgid "Brand"
+msgstr ""
+
+msgctxt "selection:product.identifier,type:"
 msgid "International Article Number"
 msgstr ""
 
 msgctxt "selection:product.identifier,type:"
 msgid "International Securities Identification Number"
 msgstr ""
 
@@ -983,14 +1008,18 @@
 msgid "International Standard Identifier for Libraries"
 msgstr ""
 
 msgctxt "selection:product.identifier,type:"
 msgid "International Standard Music Number"
 msgstr ""
 
+msgctxt "selection:product.identifier,type:"
+msgid "Manufacturer Part Number"
+msgstr ""
+
 msgctxt "selection:product.product,cost_price_method:"
 msgid "Average"
 msgstr ""
 
 msgctxt "selection:product.product,cost_price_method:"
 msgid "Fixed"
 msgstr ""
```

### Comparing `trytond_product-7.2.0/locale/de.po` & `trytond_product-7.2.1/locale/de.po`

 * *Files 2% similar despite different names*

```diff
@@ -6,26 +6,38 @@
 msgid "Product Price Decimal"
 msgstr "Nachkommastellen Artikelpreis"
 
 msgctxt "field:product.category,childs:"
 msgid "Children"
 msgstr "Untergeordnet (Kategorien)"
 
+msgctxt "field:product.category,code:"
+msgid "Code"
+msgstr "Code"
+
+msgctxt "field:product.category,code_readonly:"
+msgid "Code Readonly"
+msgstr "Code ist nur lesbar"
+
 msgctxt "field:product.category,name:"
 msgid "Name"
 msgstr "Name"
 
 msgctxt "field:product.category,parent:"
 msgid "Parent"
 msgstr "Übergeordnet (Kategorie)"
 
 msgctxt "field:product.category,templates:"
 msgid "Products"
 msgstr "Artikel"
 
+msgctxt "field:product.configuration,category_sequence:"
+msgid "Category Sequence"
+msgstr "Nummernkreis Artikelkategorie"
+
 msgctxt "field:product.configuration,default_cost_price_method:"
 msgid "Default Cost Method"
 msgstr "Standardbestandsbewertungsmethode"
 
 msgctxt "field:product.configuration,product_sequence:"
 msgid "Variant Sequence"
 msgstr "Nummernkreis Variante"
@@ -291,14 +303,18 @@
 msgid "Used to add structure below the category."
 msgstr "Erlaubt den Aufbau einer Struktur unterhalb dieser Kategorie."
 
 msgctxt "help:product.category,parent:"
 msgid "Used to add structure above the category."
 msgstr "Erlaubt den Aufbau einer Struktur oberhalb dieser Kategorie."
 
+msgctxt "help:product.configuration,category_sequence:"
+msgid "Used to generate the category code."
+msgstr "Wird zum Generieren des Artikelkategoriecodes genutzt."
+
 msgctxt "help:product.configuration,default_cost_price_method:"
 msgid "The default cost price method for new products."
 msgstr "Die Standardbestandsbewertungsmethode für neue Artikel."
 
 msgctxt "help:product.configuration,product_sequence:"
 msgid "Used to generate the last part of the product code."
 msgstr "Wird zum Generieren des hinteren Teils der Artikelnummer genutzt."
@@ -495,14 +511,18 @@
 msgid "Categories"
 msgstr "Kategorien"
 
 msgctxt "model:ir.action,name:act_uom_form"
 msgid "Units of Measure"
 msgstr "Maßeinheiten"
 
+msgctxt "model:ir.message,text:msg_category_code_unique"
+msgid "The code on product category must be unique."
+msgstr "Der Code für eine Artikelkategorie kann nur einmal vergeben werden."
+
 msgctxt "model:ir.message,text:msg_invalid_code"
 msgid "The %(type)s \"%(code)s\" for product \"%(product)s\" is not valid."
 msgstr ""
 "Der Wert \"%(code)s\" für den Identifikator %(type)s von Artikel "
 "\"%(product)s\" ist ungültig."
 
 msgctxt "model:ir.message,text:msg_product_code_unique"
@@ -545,14 +565,18 @@
 msgid "Rate and factor can not be both equal to zero."
 msgstr "Faktor und Kehrwert können nicht beide Null sein."
 
 msgctxt "model:ir.model.button,string:category_add_products_button"
 msgid "Add products"
 msgstr "Artikel hinzufügen"
 
+msgctxt "model:ir.sequence.type,name:sequence_type_category"
+msgid "Category"
+msgstr "Artikelkategorie"
+
 msgctxt "model:ir.sequence.type,name:sequence_type_product"
 msgid "Variant"
 msgstr "Variante"
 
 msgctxt "model:ir.sequence.type,name:sequence_type_template"
 msgid "Product"
 msgstr "Artikel"
@@ -958,14 +982,18 @@
 msgstr "Gewicht"
 
 msgctxt "model:res.group,name:group_product_admin"
 msgid "Product Administration"
 msgstr "Artikel Administration"
 
 msgctxt "selection:product.identifier,type:"
+msgid "Brand"
+msgstr "Marke"
+
+msgctxt "selection:product.identifier,type:"
 msgid "International Article Number"
 msgstr "Internationale Artikelnummer (IAN/EAN)"
 
 msgctxt "selection:product.identifier,type:"
 msgid "International Securities Identification Number"
 msgstr "Internationale Wertpapierkennnummer (ISIN)"
 
@@ -981,14 +1009,18 @@
 msgid "International Standard Identifier for Libraries"
 msgstr "International Standard Identifier for Libraries (ISIL)"
 
 msgctxt "selection:product.identifier,type:"
 msgid "International Standard Music Number"
 msgstr "Internationale Standardmusiknummer (ISMN)"
 
+msgctxt "selection:product.identifier,type:"
+msgid "Manufacturer Part Number"
+msgstr "Herstellerteilenummer"
+
 msgctxt "selection:product.product,cost_price_method:"
 msgid "Average"
 msgstr "Gleitender Durchschnitt"
 
 msgctxt "selection:product.product,cost_price_method:"
 msgid "Fixed"
 msgstr "Festwert"
```

### Comparing `trytond_product-7.2.0/locale/es.po` & `trytond_product-7.2.1/locale/es.po`

 * *Files 2% similar despite different names*

```diff
@@ -6,26 +6,38 @@
 msgid "Product Price Decimal"
 msgstr "Decimales del precio del producto"
 
 msgctxt "field:product.category,childs:"
 msgid "Children"
 msgstr "Hijos"
 
+msgctxt "field:product.category,code:"
+msgid "Code"
+msgstr "Código"
+
+msgctxt "field:product.category,code_readonly:"
+msgid "Code Readonly"
+msgstr "Código solo lectura"
+
 msgctxt "field:product.category,name:"
 msgid "Name"
 msgstr "Nombre"
 
 msgctxt "field:product.category,parent:"
 msgid "Parent"
 msgstr "Padre"
 
 msgctxt "field:product.category,templates:"
 msgid "Products"
 msgstr "Productos"
 
+msgctxt "field:product.configuration,category_sequence:"
+msgid "Category Sequence"
+msgstr "Secuencia de la categoría"
+
 msgctxt "field:product.configuration,default_cost_price_method:"
 msgid "Default Cost Method"
 msgstr "Método de coste por defecto"
 
 msgctxt "field:product.configuration,product_sequence:"
 msgid "Variant Sequence"
 msgstr "Secuencia de la variante"
@@ -291,14 +303,18 @@
 msgid "Used to add structure below the category."
 msgstr "Utilizado para añadir una estructura por debajo de la categoría."
 
 msgctxt "help:product.category,parent:"
 msgid "Used to add structure above the category."
 msgstr "Utilizado para añadir una estructura por encima de la categoría."
 
+msgctxt "help:product.configuration,category_sequence:"
+msgid "Used to generate the category code."
+msgstr "Utilizado para generar el código de la categoría."
+
 msgctxt "help:product.configuration,default_cost_price_method:"
 msgid "The default cost price method for new products."
 msgstr "El método de coste por defecto para los nuevos productos."
 
 msgctxt "help:product.configuration,product_sequence:"
 msgid "Used to generate the last part of the product code."
 msgstr "Utilizado para generar la parte final del código del producto."
@@ -492,14 +508,18 @@
 msgid "Categories"
 msgstr "Categorías"
 
 msgctxt "model:ir.action,name:act_uom_form"
 msgid "Units of Measure"
 msgstr "Unidades de medida"
 
+msgctxt "model:ir.message,text:msg_category_code_unique"
+msgid "The code on product category must be unique."
+msgstr "El código de la categoría de producto debe ser único."
+
 msgctxt "model:ir.message,text:msg_invalid_code"
 msgid "The %(type)s \"%(code)s\" for product \"%(product)s\" is not valid."
 msgstr "El \"%(type)s\" \"%(code)s\" del producto \"%(product)s\" no es valido."
 
 msgctxt "model:ir.message,text:msg_product_code_unique"
 msgid "Code of active product must be unique."
 msgstr "El código de los productos activos debe ser único."
@@ -537,14 +557,18 @@
 msgid "Rate and factor can not be both equal to zero."
 msgstr "El ratio i el factor no pueden ser a la vez zero."
 
 msgctxt "model:ir.model.button,string:category_add_products_button"
 msgid "Add products"
 msgstr "Añadir productos"
 
+msgctxt "model:ir.sequence.type,name:sequence_type_category"
+msgid "Category"
+msgstr "Categoría"
+
 msgctxt "model:ir.sequence.type,name:sequence_type_product"
 msgid "Variant"
 msgstr "Variante"
 
 msgctxt "model:ir.sequence.type,name:sequence_type_template"
 msgid "Product"
 msgstr "Producto"
@@ -950,14 +974,18 @@
 msgstr "Peso"
 
 msgctxt "model:res.group,name:group_product_admin"
 msgid "Product Administration"
 msgstr "Administración de productos"
 
 msgctxt "selection:product.identifier,type:"
+msgid "Brand"
+msgstr "Marca"
+
+msgctxt "selection:product.identifier,type:"
 msgid "International Article Number"
 msgstr "Número de articulo internacional (EAN)"
 
 msgctxt "selection:product.identifier,type:"
 msgid "International Securities Identification Number"
 msgstr "Numero Internacional de Identificación de Valores (ISIN)"
 
@@ -973,14 +1001,18 @@
 msgid "International Standard Identifier for Libraries"
 msgstr "Número Estándar Internacional de Librerias (ISIL)"
 
 msgctxt "selection:product.identifier,type:"
 msgid "International Standard Music Number"
 msgstr "Número Estándar Internacional de Música (ISMN)"
 
+msgctxt "selection:product.identifier,type:"
+msgid "Manufacturer Part Number"
+msgstr "Número de pieza del fabricante"
+
 msgctxt "selection:product.product,cost_price_method:"
 msgid "Average"
 msgstr "Promedio"
 
 msgctxt "selection:product.product,cost_price_method:"
 msgid "Fixed"
 msgstr "Fijo"
```

### Comparing `trytond_product-7.2.0/locale/es_419.po` & `trytond_product-7.2.1/locale/es_419.po`

 * *Files 1% similar despite different names*

```diff
@@ -6,27 +6,40 @@
 msgid "Product Price Decimal"
 msgstr ""
 
 msgctxt "field:product.category,childs:"
 msgid "Children"
 msgstr ""
 
+msgctxt "field:product.category,code:"
+msgid "Code"
+msgstr ""
+
+msgctxt "field:product.category,code_readonly:"
+msgid "Code Readonly"
+msgstr ""
+
 msgctxt "field:product.category,name:"
 msgid "Name"
 msgstr ""
 
 msgctxt "field:product.category,parent:"
 msgid "Parent"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:product.category,templates:"
 msgid "Products"
 msgstr "Configuración de producto"
 
+#, fuzzy
+msgctxt "field:product.configuration,category_sequence:"
+msgid "Category Sequence"
+msgstr "Configuración de producto"
+
 msgctxt "field:product.configuration,default_cost_price_method:"
 msgid "Default Cost Method"
 msgstr "Método de costo por defecto"
 
 #, fuzzy
 msgctxt "field:product.configuration,product_sequence:"
 msgid "Variant Sequence"
@@ -312,14 +325,18 @@
 msgid "Used to add structure below the category."
 msgstr ""
 
 msgctxt "help:product.category,parent:"
 msgid "Used to add structure above the category."
 msgstr ""
 
+msgctxt "help:product.configuration,category_sequence:"
+msgid "Used to generate the category code."
+msgstr ""
+
 msgctxt "help:product.configuration,default_cost_price_method:"
 msgid "The default cost price method for new products."
 msgstr ""
 
 msgctxt "help:product.configuration,product_sequence:"
 msgid "Used to generate the last part of the product code."
 msgstr ""
@@ -499,14 +516,18 @@
 msgid "Categories"
 msgstr "Categorías"
 
 msgctxt "model:ir.action,name:act_uom_form"
 msgid "Units of Measure"
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_category_code_unique"
+msgid "The code on product category must be unique."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_invalid_code"
 msgid "The %(type)s \"%(code)s\" for product \"%(product)s\" is not valid."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_product_code_unique"
 msgid "Code of active product must be unique."
 msgstr ""
@@ -543,14 +564,19 @@
 
 #, fuzzy
 msgctxt "model:ir.model.button,string:category_add_products_button"
 msgid "Add products"
 msgstr "Configuración de producto"
 
 #, fuzzy
+msgctxt "model:ir.sequence.type,name:sequence_type_category"
+msgid "Category"
+msgstr "Categorías"
+
+#, fuzzy
 msgctxt "model:ir.sequence.type,name:sequence_type_product"
 msgid "Variant"
 msgstr "Variantes"
 
 #, fuzzy
 msgctxt "model:ir.sequence.type,name:sequence_type_template"
 msgid "Product"
@@ -966,14 +992,18 @@
 msgstr ""
 
 msgctxt "model:res.group,name:group_product_admin"
 msgid "Product Administration"
 msgstr ""
 
 msgctxt "selection:product.identifier,type:"
+msgid "Brand"
+msgstr ""
+
+msgctxt "selection:product.identifier,type:"
 msgid "International Article Number"
 msgstr ""
 
 msgctxt "selection:product.identifier,type:"
 msgid "International Securities Identification Number"
 msgstr ""
 
@@ -989,14 +1019,18 @@
 msgid "International Standard Identifier for Libraries"
 msgstr ""
 
 msgctxt "selection:product.identifier,type:"
 msgid "International Standard Music Number"
 msgstr ""
 
+msgctxt "selection:product.identifier,type:"
+msgid "Manufacturer Part Number"
+msgstr ""
+
 msgctxt "selection:product.product,cost_price_method:"
 msgid "Average"
 msgstr ""
 
 msgctxt "selection:product.product,cost_price_method:"
 msgid "Fixed"
 msgstr ""
```

### Comparing `trytond_product-7.2.0/locale/et.po` & `trytond_product-7.2.1/locale/et.po`

 * *Files 2% similar despite different names*

```diff
@@ -7,26 +7,40 @@
 msgid "Product Price Decimal"
 msgstr "Toote omahind"
 
 msgctxt "field:product.category,childs:"
 msgid "Children"
 msgstr "Alam"
 
+#, fuzzy
+msgctxt "field:product.category,code:"
+msgid "Code"
+msgstr "Kood"
+
+msgctxt "field:product.category,code_readonly:"
+msgid "Code Readonly"
+msgstr ""
+
 msgctxt "field:product.category,name:"
 msgid "Name"
 msgstr "Nimi"
 
 msgctxt "field:product.category,parent:"
 msgid "Parent"
 msgstr "Ülem"
 
 msgctxt "field:product.category,templates:"
 msgid "Products"
 msgstr "Tooted"
 
+#, fuzzy
+msgctxt "field:product.configuration,category_sequence:"
+msgid "Category Sequence"
+msgstr "Kauba mall"
+
 msgctxt "field:product.configuration,default_cost_price_method:"
 msgid "Default Cost Method"
 msgstr "Vaikimisi kulumeetod"
 
 #, fuzzy
 msgctxt "field:product.configuration,product_sequence:"
 msgid "Variant Sequence"
@@ -303,14 +317,18 @@
 msgid "Used to add structure below the category."
 msgstr ""
 
 msgctxt "help:product.category,parent:"
 msgid "Used to add structure above the category."
 msgstr ""
 
+msgctxt "help:product.configuration,category_sequence:"
+msgid "Used to generate the category code."
+msgstr ""
+
 msgctxt "help:product.configuration,default_cost_price_method:"
 msgid "The default cost price method for new products."
 msgstr ""
 
 msgctxt "help:product.configuration,product_sequence:"
 msgid "Used to generate the last part of the product code."
 msgstr ""
@@ -487,14 +505,18 @@
 msgid "Categories"
 msgstr "Kategooriad"
 
 msgctxt "model:ir.action,name:act_uom_form"
 msgid "Units of Measure"
 msgstr "Mõõtühik"
 
+msgctxt "model:ir.message,text:msg_category_code_unique"
+msgid "The code on product category must be unique."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_invalid_code"
 msgid "The %(type)s \"%(code)s\" for product \"%(product)s\" is not valid."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_product_code_unique"
 msgid "Code of active product must be unique."
 msgstr ""
@@ -531,14 +553,19 @@
 
 #, fuzzy
 msgctxt "model:ir.model.button,string:category_add_products_button"
 msgid "Add products"
 msgstr "Tooted"
 
 #, fuzzy
+msgctxt "model:ir.sequence.type,name:sequence_type_category"
+msgid "Category"
+msgstr "Kategooria"
+
+#, fuzzy
 msgctxt "model:ir.sequence.type,name:sequence_type_product"
 msgid "Variant"
 msgstr "Variandid"
 
 #, fuzzy
 msgctxt "model:ir.sequence.type,name:sequence_type_template"
 msgid "Product"
@@ -950,14 +977,18 @@
 msgstr "Kaal"
 
 msgctxt "model:res.group,name:group_product_admin"
 msgid "Product Administration"
 msgstr "Toote administreerimine"
 
 msgctxt "selection:product.identifier,type:"
+msgid "Brand"
+msgstr ""
+
+msgctxt "selection:product.identifier,type:"
 msgid "International Article Number"
 msgstr ""
 
 msgctxt "selection:product.identifier,type:"
 msgid "International Securities Identification Number"
 msgstr ""
 
@@ -973,14 +1004,18 @@
 msgid "International Standard Identifier for Libraries"
 msgstr ""
 
 msgctxt "selection:product.identifier,type:"
 msgid "International Standard Music Number"
 msgstr ""
 
+msgctxt "selection:product.identifier,type:"
+msgid "Manufacturer Part Number"
+msgstr ""
+
 msgctxt "selection:product.product,cost_price_method:"
 msgid "Average"
 msgstr "Keskmine"
 
 msgctxt "selection:product.product,cost_price_method:"
 msgid "Fixed"
 msgstr "Fikseeritud"
```

### Comparing `trytond_product-7.2.0/locale/fa.po` & `trytond_product-7.2.1/locale/fa.po`

 * *Files 1% similar despite different names*

```diff
@@ -7,27 +7,41 @@
 msgid "Product Price Decimal"
 msgstr "ارزش بها محصول"
 
 msgctxt "field:product.category,childs:"
 msgid "Children"
 msgstr "زیر مجموعه"
 
+#, fuzzy
+msgctxt "field:product.category,code:"
+msgid "Code"
+msgstr "کد"
+
+msgctxt "field:product.category,code_readonly:"
+msgid "Code Readonly"
+msgstr ""
+
 msgctxt "field:product.category,name:"
 msgid "Name"
 msgstr "نام"
 
 msgctxt "field:product.category,parent:"
 msgid "Parent"
 msgstr "منبع"
 
 #, fuzzy
 msgctxt "field:product.category,templates:"
 msgid "Products"
 msgstr "محصولات"
 
+#, fuzzy
+msgctxt "field:product.configuration,category_sequence:"
+msgid "Category Sequence"
+msgstr "الگوی محصول"
+
 msgctxt "field:product.configuration,default_cost_price_method:"
 msgid "Default Cost Method"
 msgstr "روش هزینه پیش فرض"
 
 #, fuzzy
 msgctxt "field:product.configuration,product_sequence:"
 msgid "Variant Sequence"
@@ -304,14 +318,18 @@
 msgid "Used to add structure below the category."
 msgstr ""
 
 msgctxt "help:product.category,parent:"
 msgid "Used to add structure above the category."
 msgstr ""
 
+msgctxt "help:product.configuration,category_sequence:"
+msgid "Used to generate the category code."
+msgstr ""
+
 msgctxt "help:product.configuration,default_cost_price_method:"
 msgid "The default cost price method for new products."
 msgstr ""
 
 msgctxt "help:product.configuration,product_sequence:"
 msgid "Used to generate the last part of the product code."
 msgstr ""
@@ -494,14 +512,18 @@
 msgid "Categories"
 msgstr "دسته بندی ها"
 
 msgctxt "model:ir.action,name:act_uom_form"
 msgid "Units of Measure"
 msgstr "واحدهای اندازه گیری"
 
+msgctxt "model:ir.message,text:msg_category_code_unique"
+msgid "The code on product category must be unique."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_invalid_code"
 msgid "The %(type)s \"%(code)s\" for product \"%(product)s\" is not valid."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_product_code_unique"
 msgid "Code of active product must be unique."
 msgstr ""
@@ -538,14 +560,19 @@
 
 #, fuzzy
 msgctxt "model:ir.model.button,string:category_add_products_button"
 msgid "Add products"
 msgstr "محصولات"
 
 #, fuzzy
+msgctxt "model:ir.sequence.type,name:sequence_type_category"
+msgid "Category"
+msgstr "دسته‌بندی‌"
+
+#, fuzzy
 msgctxt "model:ir.sequence.type,name:sequence_type_product"
 msgid "Variant"
 msgstr "متغیرها"
 
 #, fuzzy
 msgctxt "model:ir.sequence.type,name:sequence_type_template"
 msgid "Product"
@@ -958,14 +985,18 @@
 msgstr "وزن"
 
 msgctxt "model:res.group,name:group_product_admin"
 msgid "Product Administration"
 msgstr "مدیریت محصول"
 
 msgctxt "selection:product.identifier,type:"
+msgid "Brand"
+msgstr ""
+
+msgctxt "selection:product.identifier,type:"
 msgid "International Article Number"
 msgstr ""
 
 msgctxt "selection:product.identifier,type:"
 msgid "International Securities Identification Number"
 msgstr ""
 
@@ -981,14 +1012,18 @@
 msgid "International Standard Identifier for Libraries"
 msgstr ""
 
 msgctxt "selection:product.identifier,type:"
 msgid "International Standard Music Number"
 msgstr ""
 
+msgctxt "selection:product.identifier,type:"
+msgid "Manufacturer Part Number"
+msgstr ""
+
 msgctxt "selection:product.product,cost_price_method:"
 msgid "Average"
 msgstr "متوسط"
 
 msgctxt "selection:product.product,cost_price_method:"
 msgid "Fixed"
 msgstr "درست شد"
```

### Comparing `trytond_product-7.2.0/locale/fi.po` & `trytond_product-7.2.1/locale/id.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,111 +4,120 @@
 
 msgctxt "field:ir.configuration,product_price_decimal:"
 msgid "Product Price Decimal"
 msgstr ""
 
 msgctxt "field:product.category,childs:"
 msgid "Children"
+msgstr "Cabang"
+
+#, fuzzy
+msgctxt "field:product.category,code:"
+msgid "Code"
+msgstr "Kode"
+
+msgctxt "field:product.category,code_readonly:"
+msgid "Code Readonly"
 msgstr ""
 
 msgctxt "field:product.category,name:"
 msgid "Name"
-msgstr ""
+msgstr "Nama"
 
 msgctxt "field:product.category,parent:"
 msgid "Parent"
-msgstr ""
+msgstr "Induk"
 
-#, fuzzy
 msgctxt "field:product.category,templates:"
 msgid "Products"
-msgstr "Products"
+msgstr "Produk-produk"
+
+#, fuzzy
+msgctxt "field:product.configuration,category_sequence:"
+msgid "Category Sequence"
+msgstr "Urutan Produk"
 
 msgctxt "field:product.configuration,default_cost_price_method:"
 msgid "Default Cost Method"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:product.configuration,product_sequence:"
 msgid "Variant Sequence"
-msgstr "Product by Category"
+msgstr "Urutan Produk"
 
 #, fuzzy
 msgctxt "field:product.configuration,template_sequence:"
 msgid "Product Sequence"
-msgstr "Product by Category"
+msgstr "Urutan Produk"
 
 msgctxt ""
 "field:product.configuration.default_cost_price_method,default_cost_price_method:"
 msgid "Default Cost Method"
 msgstr ""
 
 msgctxt "field:product.cost_price,company:"
 msgid "Company"
-msgstr ""
+msgstr "Perusahaan"
 
 msgctxt "field:product.cost_price,cost_price:"
 msgid "Cost Price"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:product.cost_price,product:"
 msgid "Product"
-msgstr "Product"
+msgstr "Produk"
 
 msgctxt "field:product.cost_price_method,company:"
 msgid "Company"
-msgstr ""
+msgstr "Perusahaan"
 
 msgctxt "field:product.cost_price_method,cost_price_method:"
 msgid "Cost Price Method"
 msgstr ""
 
 msgctxt "field:product.cost_price_method,template:"
 msgid "Template"
-msgstr ""
+msgstr "Templat"
 
 msgctxt "field:product.identifier,code:"
 msgid "Code"
-msgstr ""
+msgstr "Kode"
 
-#, fuzzy
 msgctxt "field:product.identifier,product:"
 msgid "Product"
-msgstr "Product"
+msgstr "Produk"
 
 msgctxt "field:product.identifier,type:"
 msgid "Type"
 msgstr ""
 
 msgctxt "field:product.list_price,company:"
 msgid "Company"
-msgstr ""
+msgstr "Perusahaan"
 
 msgctxt "field:product.list_price,list_price:"
 msgid "List Price"
 msgstr ""
 
 msgctxt "field:product.list_price,template:"
 msgid "Template"
-msgstr ""
+msgstr "Templat"
 
-#, fuzzy
 msgctxt "field:product.product,categories:"
 msgid "Categories"
-msgstr "Categories"
+msgstr "Kategori"
 
-#, fuzzy
 msgctxt "field:product.product,categories_all:"
 msgid "Categories"
-msgstr "Categories"
+msgstr "Kategori"
 
 msgctxt "field:product.product,code:"
 msgid "Code"
-msgstr ""
+msgstr "Kode"
 
 msgctxt "field:product.product,code_readonly:"
 msgid "Code Readonly"
 msgstr ""
 
 msgctxt "field:product.product,consumable:"
 msgid "Consumable"
@@ -137,39 +146,39 @@
 msgctxt "field:product.product,default_uom:"
 msgid "Default UoM"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:product.product,default_uom_category:"
 msgid "Default UoM Category"
-msgstr "Product by Category"
+msgstr "Kategori Produk"
 
 msgctxt "field:product.product,description:"
 msgid "Description"
-msgstr ""
+msgstr "Deskripsi"
 
 msgctxt "field:product.product,identifiers:"
 msgid "Identifiers"
 msgstr ""
 
 msgctxt "field:product.product,list_price:"
 msgid "List Price"
-msgstr ""
+msgstr "Daftar Harga"
 
 msgctxt "field:product.product,list_price_uom:"
 msgid "List Price"
-msgstr ""
+msgstr "Daftar Harga"
 
 msgctxt "field:product.product,list_prices:"
 msgid "List Prices"
 msgstr ""
 
 msgctxt "field:product.product,name:"
 msgid "Name"
-msgstr ""
+msgstr "Nama"
 
 msgctxt "field:product.product,prefix_code:"
 msgid "Prefix Code"
 msgstr ""
 
 msgctxt "field:product.product,suffix_code:"
 msgid "Suffix Code"
@@ -179,27 +188,25 @@
 msgid "Product Template"
 msgstr ""
 
 msgctxt "field:product.product,type:"
 msgid "Type"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:product.template,categories:"
 msgid "Categories"
-msgstr "Categories"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:product.template,categories_all:"
 msgid "Categories"
-msgstr "Categories"
+msgstr ""
 
 msgctxt "field:product.template,code:"
 msgid "Code"
-msgstr ""
+msgstr "Kode"
 
 msgctxt "field:product.template,code_readonly:"
 msgid "Code Readonly"
 msgstr ""
 
 msgctxt "field:product.template,consumable:"
 msgid "Consumable"
@@ -220,68 +227,67 @@
 msgctxt "field:product.template,default_uom:"
 msgid "Default UoM"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:product.template,default_uom_category:"
 msgid "Default UoM Category"
-msgstr "Product by Category"
+msgstr "Kategori Produk"
 
 msgctxt "field:product.template,list_price:"
 msgid "List Price"
-msgstr ""
+msgstr "Daftar Harga"
 
 msgctxt "field:product.template,list_prices:"
 msgid "List Prices"
 msgstr ""
 
 msgctxt "field:product.template,name:"
 msgid "Name"
-msgstr ""
+msgstr "Nama"
 
-#, fuzzy
 msgctxt "field:product.template,products:"
 msgid "Variants"
-msgstr "Variants"
+msgstr ""
 
 msgctxt "field:product.template,type:"
 msgid "Type"
 msgstr ""
 
 msgctxt "field:product.template-product.category,category:"
 msgid "Category"
-msgstr ""
+msgstr "Kategori"
 
 msgctxt "field:product.template-product.category,template:"
 msgid "Template"
-msgstr ""
+msgstr "Templat"
 
 msgctxt "field:product.template-product.category.all,category:"
 msgid "Category"
-msgstr ""
+msgstr "Kategori"
 
 msgctxt "field:product.template-product.category.all,template:"
 msgid "Template"
-msgstr ""
+msgstr "Templat"
 
 msgctxt "field:product.uom,category:"
 msgid "Category"
-msgstr ""
+msgstr "Kategori"
 
 msgctxt "field:product.uom,digits:"
 msgid "Display Digits"
 msgstr ""
 
 msgctxt "field:product.uom,factor:"
 msgid "Factor"
 msgstr ""
 
 msgctxt "field:product.uom,name:"
 msgid "Name"
-msgstr ""
+msgstr "Nama"
 
 msgctxt "field:product.uom,rate:"
 msgid "Rate"
 msgstr ""
 
 msgctxt "field:product.uom,rounding:"
 msgid "Rounding Precision"
@@ -289,29 +295,32 @@
 
 msgctxt "field:product.uom,symbol:"
 msgid "Symbol"
 msgstr ""
 
 msgctxt "field:product.uom.category,name:"
 msgid "Name"
-msgstr ""
+msgstr "Nama"
 
-#, fuzzy
 msgctxt "field:product.uom.category,uoms:"
 msgid "Units of Measure"
-msgstr "Units of Measure"
+msgstr "Satuan Ukuran"
 
 msgctxt "help:product.category,childs:"
 msgid "Used to add structure below the category."
 msgstr ""
 
 msgctxt "help:product.category,parent:"
 msgid "Used to add structure above the category."
 msgstr ""
 
+msgctxt "help:product.configuration,category_sequence:"
+msgid "Used to generate the category code."
+msgstr ""
+
 msgctxt "help:product.configuration,default_cost_price_method:"
 msgid "The default cost price method for new products."
 msgstr ""
 
 msgctxt "help:product.configuration,product_sequence:"
 msgid "Used to generate the last part of the product code."
 msgstr ""
@@ -355,18 +364,17 @@
 
 msgctxt "help:product.product,default_uom:"
 msgid ""
 "The standard Unit of Measure for the product.\n"
 "Used internally when calculating the stock levels of goods and assets."
 msgstr ""
 
-#, fuzzy
 msgctxt "help:product.product,default_uom_category:"
 msgid "The category of the default Unit of Measure."
-msgstr "Categories of Unit of Measure"
+msgstr ""
 
 msgctxt "help:product.product,identifiers:"
 msgid "Other identifiers associated with the variant."
 msgstr ""
 
 msgctxt "help:product.product,list_price:"
 msgid "The standard price the product is sold at."
@@ -403,18 +411,17 @@
 
 msgctxt "help:product.template,default_uom:"
 msgid ""
 "The standard Unit of Measure for the product.\n"
 "Used internally when calculating the stock levels of goods and assets."
 msgstr ""
 
-#, fuzzy
 msgctxt "help:product.template,default_uom_category:"
 msgid "The category of the default Unit of Measure."
-msgstr "Categories of Unit of Measure"
+msgstr ""
 
 msgctxt "help:product.template,list_price:"
 msgid "The standard price the product is sold at."
 msgstr ""
 
 msgctxt "help:product.template,products:"
 msgid "The different variants the product comes in."
@@ -448,54 +455,57 @@
 
 msgctxt "help:product.uom,symbol:"
 msgid "The symbol that represents the unit of measure."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_category_list"
 msgid "Categories"
-msgstr "Categories"
+msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_category_product"
 msgid "Add products"
-msgstr "Products"
+msgstr "Produk"
 
 msgctxt "model:ir.action,name:act_category_tree"
 msgid "Categories"
-msgstr "Categories"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_product_configuration_form"
 msgid "Configuration"
-msgstr "Configuration"
+msgstr "Konfigurasi"
 
 msgctxt "model:ir.action,name:act_product_form"
 msgid "Variants"
-msgstr "Variants"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_product_from_template"
 msgid "Variants"
-msgstr "Variants"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_template_by_category"
 msgid "Product by Category"
-msgstr "Product by Category"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_template_form"
 msgid "Products"
-msgstr "Products"
+msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_uom_category_form"
 msgid "Categories"
-msgstr "Categories"
+msgstr "Kategori"
 
 msgctxt "model:ir.action,name:act_uom_form"
 msgid "Units of Measure"
-msgstr "Units of Measure"
+msgstr "Satuan Ukuran"
+
+msgctxt "model:ir.message,text:msg_category_code_unique"
+msgid "The code on product category must be unique."
+msgstr ""
 
 msgctxt "model:ir.message,text:msg_invalid_code"
 msgid "The %(type)s \"%(code)s\" for product \"%(product)s\" is not valid."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_product_code_unique"
 msgid "Code of active product must be unique."
@@ -527,97 +537,95 @@
 msgid "You cannot modify the rate of the unit of measure\"%(uom)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_uom_no_zero_factor_rate"
 msgid "Rate and factor can not be both equal to zero."
 msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.model.button,string:category_add_products_button"
 msgid "Add products"
-msgstr "Products"
+msgstr "Tambah produk"
 
 #, fuzzy
+msgctxt "model:ir.sequence.type,name:sequence_type_category"
+msgid "Category"
+msgstr "Kategori"
+
 msgctxt "model:ir.sequence.type,name:sequence_type_product"
 msgid "Variant"
-msgstr "Variants"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.sequence.type,name:sequence_type_template"
 msgid "Product"
-msgstr "Product"
+msgstr "Produk"
 
 msgctxt "model:ir.ui.menu,name:menu_category_list"
 msgid "Categories"
-msgstr "Categories"
+msgstr "Kategori-Kategori"
 
 msgctxt "model:ir.ui.menu,name:menu_category_tree"
 msgid "Categories"
-msgstr "Categories"
+msgstr "Kategori-Kategori"
 
 msgctxt "model:ir.ui.menu,name:menu_configuration"
 msgid "Configuration"
-msgstr "Configuration"
+msgstr "Konfigurasi"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_main_product"
 msgid "Products"
-msgstr "Products"
+msgstr "Produk-produk"
 
 msgctxt "model:ir.ui.menu,name:menu_product"
 msgid "Variants"
-msgstr "Variants"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_product_configuration"
 msgid "Configuration"
-msgstr "Configuration"
+msgstr "Konfigurasi"
 
 msgctxt "model:ir.ui.menu,name:menu_reporting"
 msgid "Reporting"
-msgstr ""
+msgstr "Pelaporan"
 
 msgctxt "model:ir.ui.menu,name:menu_template"
 msgid "Products"
-msgstr "Products"
+msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_uom_category_form"
 msgid "Categories"
-msgstr "Categories"
+msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_uom_form"
 msgid "Units of Measure"
-msgstr "Units of Measure"
+msgstr "Satuan Ukuran"
 
-#, fuzzy
 msgctxt "model:product.category,name:"
 msgid "Product Category"
-msgstr "Product by Category"
+msgstr "Kategori Produk"
 
-#, fuzzy
 msgctxt "model:product.configuration,name:"
 msgid "Product Configuration"
-msgstr "Product Configuration"
+msgstr "Konfigurasi Produk"
 
 msgctxt "model:product.configuration.default_cost_price_method,name:"
 msgid "Product Configuration Default Cost Price Method"
 msgstr ""
 
 msgctxt "model:product.cost_price,name:"
 msgid "Product Cost Price"
 msgstr ""
 
 msgctxt "model:product.cost_price_method,name:"
 msgid "Product Cost Price Method"
 msgstr ""
 
-#, fuzzy
 msgctxt "model:product.identifier,name:"
 msgid "Product Identifier"
-msgstr "Product by Category"
+msgstr "Pengenal Produk"
 
 msgctxt "model:product.list_price,name:"
 msgid "Product List Price"
 msgstr ""
 
 msgctxt "model:product.product,name:"
 msgid "Product Variant"
@@ -631,51 +639,50 @@
 msgid "Template - Category"
 msgstr ""
 
 msgctxt "model:product.template-product.category.all,name:"
 msgid "Template - Category All"
 msgstr ""
 
-#, fuzzy
 msgctxt "model:product.uom,name:"
 msgid "Unit of Measure"
-msgstr "Units of Measure"
+msgstr "Satuan Ukuran"
 
 msgctxt "model:product.uom,name:uom_are"
 msgid "Are"
 msgstr "Are"
 
 msgctxt "model:product.uom,name:uom_carat"
 msgid "Carat"
-msgstr "Carat"
+msgstr "Karat"
 
 #, fuzzy
 msgctxt "model:product.uom,name:uom_centimeter"
 msgid "Centimeter"
-msgstr "centimeter"
+msgstr "sentimeter"
 
 msgctxt "model:product.uom,name:uom_cubic_centimeter"
 msgid "Cubic centimeter"
-msgstr "Cubic centimeter"
+msgstr "Centimeter kubik"
 
 msgctxt "model:product.uom,name:uom_cubic_foot"
 msgid "Cubic foot"
-msgstr "Cubic foot"
+msgstr "Kaki kubik"
 
 msgctxt "model:product.uom,name:uom_cubic_inch"
 msgid "Cubic inch"
-msgstr "Cubic inch"
+msgstr "Inci kubik"
 
 msgctxt "model:product.uom,name:uom_cubic_meter"
 msgid "Cubic meter"
-msgstr "Cubic meter"
+msgstr "Meter kubik"
 
 msgctxt "model:product.uom,name:uom_day"
 msgid "Day"
-msgstr "Day"
+msgstr "Hari"
 
 msgctxt "model:product.uom,name:uom_energy_joule"
 msgid "Joule"
 msgstr ""
 
 msgctxt "model:product.uom,name:uom_energy_kwh"
 msgid "Kilowatt-hour"
@@ -687,35 +694,35 @@
 
 msgctxt "model:product.uom,name:uom_energy_mwh"
 msgid "Megawatt-hour"
 msgstr ""
 
 msgctxt "model:product.uom,name:uom_foot"
 msgid "Foot"
-msgstr "Foot"
+msgstr "Kaki"
 
 msgctxt "model:product.uom,name:uom_gallon"
 msgid "Gallon"
-msgstr "Gallon"
+msgstr "Galon"
 
 msgctxt "model:product.uom,name:uom_gram"
 msgid "Gram"
 msgstr "Gram"
 
 msgctxt "model:product.uom,name:uom_hectare"
 msgid "Hectare"
-msgstr "Hectare"
+msgstr "Hektar"
 
 msgctxt "model:product.uom,name:uom_hour"
 msgid "Hour"
-msgstr "Hour"
+msgstr "Jam"
 
 msgctxt "model:product.uom,name:uom_inch"
 msgid "Inch"
-msgstr "Inch"
+msgstr "Inci"
 
 msgctxt "model:product.uom,name:uom_kilogram"
 msgid "Kilogram"
 msgstr "Kilogram"
 
 msgctxt "model:product.uom,name:uom_kilometer"
 msgid "Kilometer"
@@ -727,71 +734,71 @@
 
 msgctxt "model:product.uom,name:uom_meter"
 msgid "Meter"
 msgstr "Meter"
 
 msgctxt "model:product.uom,name:uom_mile"
 msgid "Mile"
-msgstr "Mile"
+msgstr ""
 
 msgctxt "model:product.uom,name:uom_millimeter"
 msgid "Millimeter"
 msgstr "Millimeter"
 
 msgctxt "model:product.uom,name:uom_minute"
 msgid "Minute"
-msgstr "Minute"
+msgstr "Menit"
 
 msgctxt "model:product.uom,name:uom_ounce"
 msgid "Ounce"
-msgstr "Ounce"
+msgstr "Ons"
 
 msgctxt "model:product.uom,name:uom_pound"
 msgid "Pound"
-msgstr "Pound"
+msgstr ""
 
 msgctxt "model:product.uom,name:uom_second"
 msgid "Second"
-msgstr "Second"
+msgstr "Detik"
 
 msgctxt "model:product.uom,name:uom_square_centimeter"
 msgid "Square centimeter"
-msgstr "Square centimeter"
+msgstr "Centimeter persegi"
 
 msgctxt "model:product.uom,name:uom_square_foot"
 msgid "Square foot"
-msgstr "Square foot"
+msgstr "Kaki persegi"
 
 msgctxt "model:product.uom,name:uom_square_inch"
 msgid "Square inch"
-msgstr "Square inch"
+msgstr "Inci persegi"
 
 msgctxt "model:product.uom,name:uom_square_meter"
 msgid "Square meter"
-msgstr "Square meter"
+msgstr "Meter persegi"
 
 msgctxt "model:product.uom,name:uom_square_yard"
 msgid "Square yard"
-msgstr "Square yard"
+msgstr "Yard persegi"
 
 msgctxt "model:product.uom,name:uom_unit"
 msgid "Unit"
-msgstr "Unit"
+msgstr ""
 
 msgctxt "model:product.uom,name:uom_yard"
 msgid "Yard"
-msgstr "Yard"
+msgstr ""
 
 msgctxt "model:product.uom,symbol:uom_are"
 msgid "a"
-msgstr "a"
+msgstr ""
 
 msgctxt "model:product.uom,symbol:uom_carat"
 msgid "c"
-msgstr "c"
+msgstr ""
 
 msgctxt "model:product.uom,symbol:uom_centimeter"
 msgid "cm"
 msgstr "cm"
 
 msgctxt "model:product.uom,symbol:uom_cubic_centimeter"
 msgid "cm³"
@@ -799,23 +806,23 @@
 
 msgctxt "model:product.uom,symbol:uom_cubic_foot"
 msgid "ft³"
 msgstr "ft³"
 
 msgctxt "model:product.uom,symbol:uom_cubic_inch"
 msgid "in³"
-msgstr "in³"
+msgstr ""
 
 msgctxt "model:product.uom,symbol:uom_cubic_meter"
 msgid "m³"
 msgstr "m³"
 
 msgctxt "model:product.uom,symbol:uom_day"
 msgid "d"
-msgstr "d"
+msgstr ""
 
 msgctxt "model:product.uom,symbol:uom_energy_joule"
 msgid "J"
 msgstr ""
 
 msgctxt "model:product.uom,symbol:uom_energy_kwh"
 msgid "kW⋅h"
@@ -827,35 +834,35 @@
 
 msgctxt "model:product.uom,symbol:uom_energy_mwh"
 msgid "MW⋅h"
 msgstr ""
 
 msgctxt "model:product.uom,symbol:uom_foot"
 msgid "ft"
-msgstr "ft"
+msgstr ""
 
 msgctxt "model:product.uom,symbol:uom_gallon"
 msgid "gal"
-msgstr "gal"
+msgstr ""
 
 msgctxt "model:product.uom,symbol:uom_gram"
 msgid "g"
-msgstr "g"
+msgstr ""
 
 msgctxt "model:product.uom,symbol:uom_hectare"
 msgid "ha"
-msgstr "ha"
+msgstr ""
 
 msgctxt "model:product.uom,symbol:uom_hour"
 msgid "h"
-msgstr "h"
+msgstr ""
 
 msgctxt "model:product.uom,symbol:uom_inch"
 msgid "in"
-msgstr "in"
+msgstr ""
 
 msgctxt "model:product.uom,symbol:uom_kilogram"
 msgid "kg"
 msgstr "kg"
 
 msgctxt "model:product.uom,symbol:uom_kilometer"
 msgid "km"
@@ -867,100 +874,103 @@
 
 msgctxt "model:product.uom,symbol:uom_meter"
 msgid "m"
 msgstr "m"
 
 msgctxt "model:product.uom,symbol:uom_mile"
 msgid "mi"
-msgstr "mi"
+msgstr ""
 
 msgctxt "model:product.uom,symbol:uom_millimeter"
 msgid "mm"
 msgstr "mm"
 
 msgctxt "model:product.uom,symbol:uom_minute"
 msgid "min"
-msgstr "min"
+msgstr ""
 
 msgctxt "model:product.uom,symbol:uom_ounce"
 msgid "oz"
-msgstr "oz"
+msgstr ""
 
 msgctxt "model:product.uom,symbol:uom_pound"
 msgid "lb"
-msgstr "lb"
+msgstr ""
 
 msgctxt "model:product.uom,symbol:uom_second"
 msgid "s"
-msgstr "s"
+msgstr ""
 
 msgctxt "model:product.uom,symbol:uom_square_centimeter"
 msgid "cm²"
 msgstr "cm²"
 
 msgctxt "model:product.uom,symbol:uom_square_foot"
 msgid "ft²"
-msgstr "ft²"
+msgstr ""
 
 msgctxt "model:product.uom,symbol:uom_square_inch"
 msgid "in²"
-msgstr "in²"
+msgstr ""
 
 msgctxt "model:product.uom,symbol:uom_square_meter"
 msgid "m²"
 msgstr "m²"
 
 msgctxt "model:product.uom,symbol:uom_square_yard"
 msgid "yd²"
-msgstr "yd²"
+msgstr ""
 
 msgctxt "model:product.uom,symbol:uom_unit"
 msgid "u"
-msgstr "u"
+msgstr ""
 
 msgctxt "model:product.uom,symbol:uom_yard"
 msgid "yd"
-msgstr "yd"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:product.uom.category,name:"
 msgid "Unit of Measure Category"
-msgstr "Units of Measure"
+msgstr "Kategori Satuan Ukuran"
 
 msgctxt "model:product.uom.category,name:uom_cat_energy"
 msgid "Energy"
 msgstr ""
 
 msgctxt "model:product.uom.category,name:uom_cat_length"
 msgid "Length"
-msgstr "Length"
+msgstr "Panjang"
 
 msgctxt "model:product.uom.category,name:uom_cat_surface"
 msgid "Surface"
-msgstr "Surface"
+msgstr ""
 
 msgctxt "model:product.uom.category,name:uom_cat_time"
 msgid "Time"
-msgstr "Time"
+msgstr "Waktu"
 
 msgctxt "model:product.uom.category,name:uom_cat_unit"
 msgid "Units"
-msgstr "Units"
+msgstr ""
 
 msgctxt "model:product.uom.category,name:uom_cat_volume"
 msgid "Volume"
-msgstr "Volume"
+msgstr ""
 
 msgctxt "model:product.uom.category,name:uom_cat_weight"
 msgid "Weight"
-msgstr "Weight"
+msgstr "Berat"
 
 msgctxt "model:res.group,name:group_product_admin"
 msgid "Product Administration"
-msgstr "Product Administration"
+msgstr ""
+
+msgctxt "selection:product.identifier,type:"
+msgid "Brand"
+msgstr ""
 
 msgctxt "selection:product.identifier,type:"
 msgid "International Article Number"
 msgstr ""
 
 msgctxt "selection:product.identifier,type:"
 msgid "International Securities Identification Number"
@@ -978,59 +988,62 @@
 msgid "International Standard Identifier for Libraries"
 msgstr ""
 
 msgctxt "selection:product.identifier,type:"
 msgid "International Standard Music Number"
 msgstr ""
 
+msgctxt "selection:product.identifier,type:"
+msgid "Manufacturer Part Number"
+msgstr ""
+
 msgctxt "selection:product.product,cost_price_method:"
 msgid "Average"
 msgstr ""
 
 msgctxt "selection:product.product,cost_price_method:"
 msgid "Fixed"
 msgstr ""
 
 msgctxt "selection:product.product,type:"
 msgid "Assets"
-msgstr ""
+msgstr "Aset-Aset"
 
 msgctxt "selection:product.product,type:"
 msgid "Goods"
-msgstr ""
+msgstr "Barang"
 
 msgctxt "selection:product.product,type:"
 msgid "Service"
-msgstr ""
+msgstr "Jasa"
 
 msgctxt "selection:product.template,cost_price_method:"
 msgid "Average"
 msgstr ""
 
 msgctxt "selection:product.template,cost_price_method:"
 msgid "Fixed"
 msgstr ""
 
 msgctxt "selection:product.template,type:"
 msgid "Assets"
-msgstr ""
+msgstr "Aset-Aset"
 
 msgctxt "selection:product.template,type:"
 msgid "Goods"
-msgstr ""
+msgstr "Barang"
 
 msgctxt "selection:product.template,type:"
 msgid "Service"
-msgstr ""
+msgstr "Jasa"
 
 msgctxt "view:product.category:"
 msgid "Children"
-msgstr ""
+msgstr "Cabang"
 
-#, fuzzy
 msgctxt "view:product.configuration:"
 msgid "Sequences"
-msgstr "Product by Category"
+msgstr "Urutan-Urutan"
 
 msgctxt "view:product.template:"
 msgid "General"
-msgstr ""
+msgstr "Umum"
```

### Comparing `trytond_product-7.2.0/locale/fr.po` & `trytond_product-7.2.1/locale/fr.po`

 * *Files 1% similar despite different names*

```diff
@@ -6,26 +6,38 @@
 msgid "Product Price Decimal"
 msgstr "Décimal de prix de revient de produit"
 
 msgctxt "field:product.category,childs:"
 msgid "Children"
 msgstr "Enfants"
 
+msgctxt "field:product.category,code:"
+msgid "Code"
+msgstr "Code"
+
+msgctxt "field:product.category,code_readonly:"
+msgid "Code Readonly"
+msgstr "Code en lecture seule"
+
 msgctxt "field:product.category,name:"
 msgid "Name"
 msgstr "Nom"
 
 msgctxt "field:product.category,parent:"
 msgid "Parent"
 msgstr "Parent"
 
 msgctxt "field:product.category,templates:"
 msgid "Products"
 msgstr "Produits"
 
+msgctxt "field:product.configuration,category_sequence:"
+msgid "Category Sequence"
+msgstr "Séquence de catégories"
+
 msgctxt "field:product.configuration,default_cost_price_method:"
 msgid "Default Cost Method"
 msgstr "Méthode de coût par défaut"
 
 msgctxt "field:product.configuration,product_sequence:"
 msgid "Variant Sequence"
 msgstr "Séquence de variantes"
@@ -291,14 +303,18 @@
 msgid "Used to add structure below the category."
 msgstr "Utilisé pour ajouter une structure sous la catégorie."
 
 msgctxt "help:product.category,parent:"
 msgid "Used to add structure above the category."
 msgstr "Utilisé pour ajouter une structure au-dessus de la catégorie."
 
+msgctxt "help:product.configuration,category_sequence:"
+msgid "Used to generate the category code."
+msgstr "Utilisé pour générer le code de catégorie."
+
 msgctxt "help:product.configuration,default_cost_price_method:"
 msgid "The default cost price method for new products."
 msgstr "La méthode du prix de revient par défaut pour les nouveaux produits."
 
 msgctxt "help:product.configuration,product_sequence:"
 msgid "Used to generate the last part of the product code."
 msgstr "Utilisé pour générer la dernière partie du code produit."
@@ -494,14 +510,18 @@
 msgid "Categories"
 msgstr "Catégories"
 
 msgctxt "model:ir.action,name:act_uom_form"
 msgid "Units of Measure"
 msgstr "Unités de mesure"
 
+msgctxt "model:ir.message,text:msg_category_code_unique"
+msgid "The code on product category must be unique."
+msgstr "Le code sur la catégorie de produit doit être unique."
+
 msgctxt "model:ir.message,text:msg_invalid_code"
 msgid "The %(type)s \"%(code)s\" for product \"%(product)s\" is not valid."
 msgstr "Le %(type)s « %(code)s » du produit « %(product)s » n'est pas valide."
 
 msgctxt "model:ir.message,text:msg_product_code_unique"
 msgid "Code of active product must be unique."
 msgstr "Le code des produits actifs doit être unique."
@@ -543,14 +563,18 @@
 msgid "Rate and factor can not be both equal to zero."
 msgstr "Le taux et le facteur ne peuvent pas être tous deux égaux à zéro."
 
 msgctxt "model:ir.model.button,string:category_add_products_button"
 msgid "Add products"
 msgstr "Ajouter des produits"
 
+msgctxt "model:ir.sequence.type,name:sequence_type_category"
+msgid "Category"
+msgstr "Catégorie"
+
 msgctxt "model:ir.sequence.type,name:sequence_type_product"
 msgid "Variant"
 msgstr "Variante"
 
 msgctxt "model:ir.sequence.type,name:sequence_type_template"
 msgid "Product"
 msgstr "Produit"
@@ -956,14 +980,18 @@
 msgstr "Poids"
 
 msgctxt "model:res.group,name:group_product_admin"
 msgid "Product Administration"
 msgstr "Administration des produits"
 
 msgctxt "selection:product.identifier,type:"
+msgid "Brand"
+msgstr "Marque"
+
+msgctxt "selection:product.identifier,type:"
 msgid "International Article Number"
 msgstr "Numéro d'article international"
 
 msgctxt "selection:product.identifier,type:"
 msgid "International Securities Identification Number"
 msgstr "Numéro international d'identification de titres"
 
@@ -979,14 +1007,18 @@
 msgid "International Standard Identifier for Libraries"
 msgstr "Identifiant international standard pour les bibliothèques"
 
 msgctxt "selection:product.identifier,type:"
 msgid "International Standard Music Number"
 msgstr "Numéro international normalisé de musique"
 
+msgctxt "selection:product.identifier,type:"
+msgid "Manufacturer Part Number"
+msgstr "Numéro de pièce du fabricant"
+
 msgctxt "selection:product.product,cost_price_method:"
 msgid "Average"
 msgstr "Moyenne"
 
 msgctxt "selection:product.product,cost_price_method:"
 msgid "Fixed"
 msgstr "Fixe"
```

### Comparing `trytond_product-7.2.0/locale/hu.po` & `trytond_product-7.2.1/locale/hu.po`

 * *Files 2% similar despite different names*

```diff
@@ -7,26 +7,41 @@
 msgid "Product Price Decimal"
 msgstr "Cikk változat"
 
 msgctxt "field:product.category,childs:"
 msgid "Children"
 msgstr "Alkategóriák"
 
+#, fuzzy
+msgctxt "field:product.category,code:"
+msgid "Code"
+msgstr "Kód"
+
+#, fuzzy
+msgctxt "field:product.category,code_readonly:"
+msgid "Code Readonly"
+msgstr "Szám csak olvasható"
+
 msgctxt "field:product.category,name:"
 msgid "Name"
 msgstr "Név"
 
 msgctxt "field:product.category,parent:"
 msgid "Parent"
 msgstr "Fölérendelt"
 
 msgctxt "field:product.category,templates:"
 msgid "Products"
 msgstr "Termékek"
 
+#, fuzzy
+msgctxt "field:product.configuration,category_sequence:"
+msgid "Category Sequence"
+msgstr "Változatok sorszámozása"
+
 msgctxt "field:product.configuration,default_cost_price_method:"
 msgid "Default Cost Method"
 msgstr "Alapértelmezett költségár számítási mód"
 
 msgctxt "field:product.configuration,product_sequence:"
 msgid "Variant Sequence"
 msgstr "Változatok sorszámozása"
@@ -297,14 +312,19 @@
 msgid "Used to add structure below the category."
 msgstr "Itt egyből megadhatja az alkategóriákat."
 
 msgctxt "help:product.category,parent:"
 msgid "Used to add structure above the category."
 msgstr "Itt megadhatja vagy létrehozhatja a főkategóriát."
 
+#, fuzzy
+msgctxt "help:product.configuration,category_sequence:"
+msgid "Used to generate the category code."
+msgstr "Itt megadhatja vagy létrehozhatja a főkategóriát."
+
 msgctxt "help:product.configuration,default_cost_price_method:"
 msgid "The default cost price method for new products."
 msgstr ""
 
 msgctxt "help:product.configuration,product_sequence:"
 msgid "Used to generate the last part of the product code."
 msgstr ""
@@ -504,14 +524,18 @@
 msgid "Categories"
 msgstr "Kategóriák"
 
 msgctxt "model:ir.action,name:act_uom_form"
 msgid "Units of Measure"
 msgstr "Mértékegységek"
 
+msgctxt "model:ir.message,text:msg_category_code_unique"
+msgid "The code on product category must be unique."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_invalid_code"
 msgid "The %(type)s \"%(code)s\" for product \"%(product)s\" is not valid."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_product_code_unique"
 msgid "Code of active product must be unique."
 msgstr ""
@@ -546,14 +570,19 @@
 msgid "Rate and factor can not be both equal to zero."
 msgstr ""
 
 msgctxt "model:ir.model.button,string:category_add_products_button"
 msgid "Add products"
 msgstr "Termékek hozzáadása"
 
+#, fuzzy
+msgctxt "model:ir.sequence.type,name:sequence_type_category"
+msgid "Category"
+msgstr "Kategória"
+
 msgctxt "model:ir.sequence.type,name:sequence_type_product"
 msgid "Variant"
 msgstr "Változat"
 
 msgctxt "model:ir.sequence.type,name:sequence_type_template"
 msgid "Product"
 msgstr "Termék"
@@ -965,14 +994,18 @@
 
 #, fuzzy
 msgctxt "model:res.group,name:group_product_admin"
 msgid "Product Administration"
 msgstr "Product Administration"
 
 msgctxt "selection:product.identifier,type:"
+msgid "Brand"
+msgstr ""
+
+msgctxt "selection:product.identifier,type:"
 msgid "International Article Number"
 msgstr "Globális Kereskedelmi Áruazonosító Szám (GTIN)"
 
 msgctxt "selection:product.identifier,type:"
 msgid "International Securities Identification Number"
 msgstr ""
 
@@ -988,14 +1021,18 @@
 msgid "International Standard Identifier for Libraries"
 msgstr ""
 
 msgctxt "selection:product.identifier,type:"
 msgid "International Standard Music Number"
 msgstr "Nemzetközi Szabványos Kottaazonosító (ISMN)"
 
+msgctxt "selection:product.identifier,type:"
+msgid "Manufacturer Part Number"
+msgstr ""
+
 msgctxt "selection:product.product,cost_price_method:"
 msgid "Average"
 msgstr "Átlag"
 
 msgctxt "selection:product.product,cost_price_method:"
 msgid "Fixed"
 msgstr "Fix"
```

### Comparing `trytond_product-7.2.0/locale/id.po` & `trytond_product-7.2.1/locale/it.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,308 +1,336 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+#, fuzzy
 msgctxt "field:ir.configuration,product_price_decimal:"
 msgid "Product Price Decimal"
-msgstr ""
+msgstr "Prezzo del prodotto"
 
 msgctxt "field:product.category,childs:"
 msgid "Children"
-msgstr "Cabang"
+msgstr "Figlio"
+
+#, fuzzy
+msgctxt "field:product.category,code:"
+msgid "Code"
+msgstr "Codice"
+
+msgctxt "field:product.category,code_readonly:"
+msgid "Code Readonly"
+msgstr ""
 
 msgctxt "field:product.category,name:"
 msgid "Name"
-msgstr "Nama"
+msgstr "Nome"
 
 msgctxt "field:product.category,parent:"
 msgid "Parent"
-msgstr "Induk"
+msgstr "Padre"
 
+#, fuzzy
 msgctxt "field:product.category,templates:"
 msgid "Products"
-msgstr "Produk-produk"
+msgstr "Prodotti"
+
+#, fuzzy
+msgctxt "field:product.configuration,category_sequence:"
+msgid "Category Sequence"
+msgstr "Modello prodotto"
 
 msgctxt "field:product.configuration,default_cost_price_method:"
 msgid "Default Cost Method"
-msgstr ""
+msgstr "Metodo di costo predefinito"
 
 #, fuzzy
 msgctxt "field:product.configuration,product_sequence:"
 msgid "Variant Sequence"
-msgstr "Urutan Produk"
+msgstr "Modello prodotto"
 
 #, fuzzy
 msgctxt "field:product.configuration,template_sequence:"
 msgid "Product Sequence"
-msgstr "Urutan Produk"
+msgstr "Modello prodotto"
 
+#, fuzzy
 msgctxt ""
 "field:product.configuration.default_cost_price_method,default_cost_price_method:"
 msgid "Default Cost Method"
-msgstr ""
+msgstr "Metodo di costo predefinito"
 
 msgctxt "field:product.cost_price,company:"
 msgid "Company"
-msgstr "Perusahaan"
+msgstr "Azienda"
 
 msgctxt "field:product.cost_price,cost_price:"
 msgid "Cost Price"
-msgstr ""
+msgstr "Prezzo di costo"
 
 msgctxt "field:product.cost_price,product:"
 msgid "Product"
-msgstr "Produk"
+msgstr "Prodotto"
 
 msgctxt "field:product.cost_price_method,company:"
 msgid "Company"
-msgstr "Perusahaan"
+msgstr "Azienda"
 
 msgctxt "field:product.cost_price_method,cost_price_method:"
 msgid "Cost Price Method"
 msgstr ""
 
 msgctxt "field:product.cost_price_method,template:"
 msgid "Template"
-msgstr "Templat"
+msgstr "Modello"
 
+#, fuzzy
 msgctxt "field:product.identifier,code:"
 msgid "Code"
-msgstr "Kode"
+msgstr "Codice"
 
 msgctxt "field:product.identifier,product:"
 msgid "Product"
-msgstr "Produk"
+msgstr "Prodotto"
 
+#, fuzzy
 msgctxt "field:product.identifier,type:"
 msgid "Type"
-msgstr ""
+msgstr "Tipo"
 
 msgctxt "field:product.list_price,company:"
 msgid "Company"
-msgstr "Perusahaan"
+msgstr "Azienda"
 
 msgctxt "field:product.list_price,list_price:"
 msgid "List Price"
-msgstr ""
+msgstr "Listino prezzi"
 
 msgctxt "field:product.list_price,template:"
 msgid "Template"
-msgstr "Templat"
+msgstr "Modello"
 
 msgctxt "field:product.product,categories:"
 msgid "Categories"
-msgstr "Kategori"
+msgstr "Categorie"
 
 msgctxt "field:product.product,categories_all:"
 msgid "Categories"
-msgstr "Kategori"
+msgstr "Categorie"
 
 msgctxt "field:product.product,code:"
 msgid "Code"
-msgstr "Kode"
+msgstr "Codice"
 
 msgctxt "field:product.product,code_readonly:"
 msgid "Code Readonly"
 msgstr ""
 
 msgctxt "field:product.product,consumable:"
 msgid "Consumable"
-msgstr ""
+msgstr "Consumabile"
 
 msgctxt "field:product.product,cost_price:"
 msgid "Cost Price"
-msgstr ""
+msgstr "Prezzo di costo"
 
 msgctxt "field:product.product,cost_price_method:"
 msgid "Cost Price Method"
 msgstr ""
 
 msgctxt "field:product.product,cost_price_methods:"
 msgid "Cost Price Methods"
 msgstr ""
 
 msgctxt "field:product.product,cost_price_uom:"
 msgid "Cost Price"
-msgstr ""
+msgstr "Prezzo di costo"
 
 msgctxt "field:product.product,cost_prices:"
 msgid "Cost Prices"
-msgstr ""
+msgstr "Costi"
 
+#, fuzzy
 msgctxt "field:product.product,default_uom:"
 msgid "Default UoM"
-msgstr ""
+msgstr "UdM predefinita"
 
 #, fuzzy
 msgctxt "field:product.product,default_uom_category:"
 msgid "Default UoM Category"
-msgstr "Kategori Produk"
+msgstr "UdM predefinita"
 
 msgctxt "field:product.product,description:"
 msgid "Description"
-msgstr "Deskripsi"
+msgstr "Descrizione"
 
 msgctxt "field:product.product,identifiers:"
 msgid "Identifiers"
 msgstr ""
 
 msgctxt "field:product.product,list_price:"
 msgid "List Price"
-msgstr "Daftar Harga"
+msgstr "Listino prezzi"
 
 msgctxt "field:product.product,list_price_uom:"
 msgid "List Price"
-msgstr "Daftar Harga"
+msgstr "Listino prezzi"
 
 msgctxt "field:product.product,list_prices:"
 msgid "List Prices"
-msgstr ""
+msgstr "Listino prezzi"
 
 msgctxt "field:product.product,name:"
 msgid "Name"
-msgstr "Nama"
+msgstr "Nome"
 
 msgctxt "field:product.product,prefix_code:"
 msgid "Prefix Code"
 msgstr ""
 
 msgctxt "field:product.product,suffix_code:"
 msgid "Suffix Code"
 msgstr ""
 
 msgctxt "field:product.product,template:"
 msgid "Product Template"
-msgstr ""
+msgstr "Modello prodotto"
 
 msgctxt "field:product.product,type:"
 msgid "Type"
-msgstr ""
+msgstr "Tipo"
 
 msgctxt "field:product.template,categories:"
 msgid "Categories"
-msgstr ""
+msgstr "Categorie"
 
 msgctxt "field:product.template,categories_all:"
 msgid "Categories"
-msgstr ""
+msgstr "Categorie"
 
+#, fuzzy
 msgctxt "field:product.template,code:"
 msgid "Code"
-msgstr "Kode"
+msgstr "Codice"
 
 msgctxt "field:product.template,code_readonly:"
 msgid "Code Readonly"
 msgstr ""
 
 msgctxt "field:product.template,consumable:"
 msgid "Consumable"
-msgstr ""
+msgstr "Consumabile"
 
 msgctxt "field:product.template,cost_price:"
 msgid "Cost Price"
-msgstr ""
+msgstr "Prezzo di costo"
 
 msgctxt "field:product.template,cost_price_method:"
 msgid "Cost Price Method"
 msgstr ""
 
 msgctxt "field:product.template,cost_price_methods:"
 msgid "Cost Price Methods"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:product.template,default_uom:"
 msgid "Default UoM"
-msgstr ""
+msgstr "UdM predefinita"
 
 #, fuzzy
 msgctxt "field:product.template,default_uom_category:"
 msgid "Default UoM Category"
-msgstr "Kategori Produk"
+msgstr "UdM predefinita"
 
 msgctxt "field:product.template,list_price:"
 msgid "List Price"
-msgstr "Daftar Harga"
+msgstr "Listino prezzi"
 
 msgctxt "field:product.template,list_prices:"
 msgid "List Prices"
-msgstr ""
+msgstr "Listino prezzi"
 
 msgctxt "field:product.template,name:"
 msgid "Name"
-msgstr "Nama"
+msgstr "Nome"
 
 msgctxt "field:product.template,products:"
 msgid "Variants"
-msgstr ""
+msgstr "Varianti"
 
 msgctxt "field:product.template,type:"
 msgid "Type"
-msgstr ""
+msgstr "Tipo"
 
 msgctxt "field:product.template-product.category,category:"
 msgid "Category"
-msgstr "Kategori"
+msgstr "Categoria"
 
 msgctxt "field:product.template-product.category,template:"
 msgid "Template"
-msgstr "Templat"
+msgstr "Modello"
 
 msgctxt "field:product.template-product.category.all,category:"
 msgid "Category"
-msgstr "Kategori"
+msgstr "Categoria"
 
 msgctxt "field:product.template-product.category.all,template:"
 msgid "Template"
-msgstr "Templat"
+msgstr "Modello"
 
 msgctxt "field:product.uom,category:"
 msgid "Category"
-msgstr "Kategori"
+msgstr "Categoria"
 
+#, fuzzy
 msgctxt "field:product.uom,digits:"
 msgid "Display Digits"
-msgstr ""
+msgstr "Posizioni"
 
 msgctxt "field:product.uom,factor:"
 msgid "Factor"
-msgstr ""
+msgstr "Fattore"
 
 msgctxt "field:product.uom,name:"
 msgid "Name"
-msgstr "Nama"
+msgstr "Nome"
 
 msgctxt "field:product.uom,rate:"
 msgid "Rate"
-msgstr ""
+msgstr "Cambio"
 
 msgctxt "field:product.uom,rounding:"
 msgid "Rounding Precision"
-msgstr ""
+msgstr "Precisione di arrotondamento"
 
 msgctxt "field:product.uom,symbol:"
 msgid "Symbol"
-msgstr ""
+msgstr "Simbolo"
 
 msgctxt "field:product.uom.category,name:"
 msgid "Name"
-msgstr "Nama"
+msgstr "Nome"
 
+#, fuzzy
 msgctxt "field:product.uom.category,uoms:"
 msgid "Units of Measure"
-msgstr "Satuan Ukuran"
+msgstr "Units of Measure"
 
 msgctxt "help:product.category,childs:"
 msgid "Used to add structure below the category."
 msgstr ""
 
 msgctxt "help:product.category,parent:"
 msgid "Used to add structure above the category."
 msgstr ""
 
+msgctxt "help:product.configuration,category_sequence:"
+msgid "Used to generate the category code."
+msgstr ""
+
 msgctxt "help:product.configuration,default_cost_price_method:"
 msgid "The default cost price method for new products."
 msgstr ""
 
 msgctxt "help:product.configuration,product_sequence:"
 msgid "Used to generate the last part of the product code."
 msgstr ""
@@ -346,17 +374,18 @@
 
 msgctxt "help:product.product,default_uom:"
 msgid ""
 "The standard Unit of Measure for the product.\n"
 "Used internally when calculating the stock levels of goods and assets."
 msgstr ""
 
+#, fuzzy
 msgctxt "help:product.product,default_uom_category:"
 msgid "The category of the default Unit of Measure."
-msgstr ""
+msgstr "Categories of Unit of Measure"
 
 msgctxt "help:product.product,identifiers:"
 msgid "Other identifiers associated with the variant."
 msgstr ""
 
 msgctxt "help:product.product,list_price:"
 msgid "The standard price the product is sold at."
@@ -393,17 +422,18 @@
 
 msgctxt "help:product.template,default_uom:"
 msgid ""
 "The standard Unit of Measure for the product.\n"
 "Used internally when calculating the stock levels of goods and assets."
 msgstr ""
 
+#, fuzzy
 msgctxt "help:product.template,default_uom_category:"
 msgid "The category of the default Unit of Measure."
-msgstr ""
+msgstr "Categories of Unit of Measure"
 
 msgctxt "help:product.template,list_price:"
 msgid "The standard price the product is sold at."
 msgstr ""
 
 msgctxt "help:product.template,products:"
 msgid "The different variants the product comes in."
@@ -415,75 +445,85 @@
 "Conversions between different units of measure can be done if they are in the same category."
 msgstr ""
 
 msgctxt "help:product.uom,digits:"
 msgid "The number of digits to display after the decimal separator."
 msgstr ""
 
+#, fuzzy
 msgctxt "help:product.uom,factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "coefficient (base unit) = 1 (this unit)"
 msgstr ""
+"Il coefficiente per la formula:\n"
+"coef (unità base) = 1 (questa unità)"
 
 msgctxt "help:product.uom,rate:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (base unit) = coef (this unit)"
 msgstr ""
+"Il coefficiente per la formula:\n"
+"1 (unità base) = coef (questa unità)"
 
 msgctxt "help:product.uom,rounding:"
 msgid "The accuracy to which values are rounded."
 msgstr ""
 
 msgctxt "help:product.uom,symbol:"
 msgid "The symbol that represents the unit of measure."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_category_list"
 msgid "Categories"
-msgstr ""
+msgstr "Categorie"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_category_product"
 msgid "Add products"
-msgstr "Produk"
+msgstr "Prodotti"
 
 msgctxt "model:ir.action,name:act_category_tree"
 msgid "Categories"
-msgstr ""
+msgstr "Categorie"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_product_configuration_form"
 msgid "Configuration"
-msgstr "Konfigurasi"
+msgstr "Configurazione"
 
 msgctxt "model:ir.action,name:act_product_form"
 msgid "Variants"
-msgstr ""
+msgstr "Variants"
 
 msgctxt "model:ir.action,name:act_product_from_template"
 msgid "Variants"
-msgstr ""
+msgstr "Variants"
 
 msgctxt "model:ir.action,name:act_template_by_category"
 msgid "Product by Category"
-msgstr ""
+msgstr "Product by Category"
 
 msgctxt "model:ir.action,name:act_template_form"
 msgid "Products"
-msgstr ""
+msgstr "Prodotti"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_uom_category_form"
 msgid "Categories"
-msgstr "Kategori"
+msgstr "Categorie"
 
 msgctxt "model:ir.action,name:act_uom_form"
 msgid "Units of Measure"
-msgstr "Satuan Ukuran"
+msgstr "Units of Measure"
+
+msgctxt "model:ir.message,text:msg_category_code_unique"
+msgid "The code on product category must be unique."
+msgstr ""
 
 msgctxt "model:ir.message,text:msg_invalid_code"
 msgid "The %(type)s \"%(code)s\" for product \"%(product)s\" is not valid."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_product_code_unique"
 msgid "Code of active product must be unique."
@@ -515,147 +555,159 @@
 msgid "You cannot modify the rate of the unit of measure\"%(uom)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_uom_no_zero_factor_rate"
 msgid "Rate and factor can not be both equal to zero."
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.model.button,string:category_add_products_button"
 msgid "Add products"
-msgstr "Tambah produk"
+msgstr "Prodotti"
+
+#, fuzzy
+msgctxt "model:ir.sequence.type,name:sequence_type_category"
+msgid "Category"
+msgstr "Categoria"
 
+#, fuzzy
 msgctxt "model:ir.sequence.type,name:sequence_type_product"
 msgid "Variant"
-msgstr ""
+msgstr "Varianti"
 
+#, fuzzy
 msgctxt "model:ir.sequence.type,name:sequence_type_template"
 msgid "Product"
-msgstr "Produk"
+msgstr "Prodotto"
 
 msgctxt "model:ir.ui.menu,name:menu_category_list"
 msgid "Categories"
-msgstr "Kategori-Kategori"
+msgstr "Categorie"
 
 msgctxt "model:ir.ui.menu,name:menu_category_tree"
 msgid "Categories"
-msgstr "Kategori-Kategori"
+msgstr "Categorie"
 
 msgctxt "model:ir.ui.menu,name:menu_configuration"
 msgid "Configuration"
-msgstr "Konfigurasi"
+msgstr "Configurazione"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_main_product"
 msgid "Products"
-msgstr "Produk-produk"
+msgstr "Prodotti"
 
 msgctxt "model:ir.ui.menu,name:menu_product"
 msgid "Variants"
-msgstr ""
+msgstr "Variants"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_product_configuration"
 msgid "Configuration"
-msgstr "Konfigurasi"
+msgstr "Configurazione"
 
 msgctxt "model:ir.ui.menu,name:menu_reporting"
 msgid "Reporting"
-msgstr "Pelaporan"
+msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_template"
 msgid "Products"
-msgstr ""
+msgstr "Prodotti"
 
 msgctxt "model:ir.ui.menu,name:menu_uom_category_form"
 msgid "Categories"
-msgstr ""
+msgstr "Categorie"
 
 msgctxt "model:ir.ui.menu,name:menu_uom_form"
 msgid "Units of Measure"
-msgstr "Satuan Ukuran"
+msgstr "Units of Measure"
 
 msgctxt "model:product.category,name:"
 msgid "Product Category"
-msgstr "Kategori Produk"
+msgstr "Categoria Prodotto"
 
+#, fuzzy
 msgctxt "model:product.configuration,name:"
 msgid "Product Configuration"
-msgstr "Konfigurasi Produk"
+msgstr "Product Configuration"
 
 msgctxt "model:product.configuration.default_cost_price_method,name:"
 msgid "Product Configuration Default Cost Price Method"
 msgstr ""
 
 msgctxt "model:product.cost_price,name:"
 msgid "Product Cost Price"
-msgstr ""
+msgstr "Prezzo del prodotto"
 
 msgctxt "model:product.cost_price_method,name:"
 msgid "Product Cost Price Method"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:product.identifier,name:"
 msgid "Product Identifier"
-msgstr "Pengenal Produk"
+msgstr "Modello prodotto"
 
 msgctxt "model:product.list_price,name:"
 msgid "Product List Price"
-msgstr ""
+msgstr "Prezzo di listino dei prodotti"
 
 msgctxt "model:product.product,name:"
 msgid "Product Variant"
-msgstr ""
+msgstr "Variante prodotto"
 
 msgctxt "model:product.template,name:"
 msgid "Product Template"
-msgstr ""
+msgstr "Modello prodotto"
 
 msgctxt "model:product.template-product.category,name:"
 msgid "Template - Category"
 msgstr ""
 
 msgctxt "model:product.template-product.category.all,name:"
 msgid "Template - Category All"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:product.uom,name:"
 msgid "Unit of Measure"
-msgstr "Satuan Ukuran"
+msgstr "Unità di misura"
 
 msgctxt "model:product.uom,name:uom_are"
 msgid "Are"
 msgstr "Are"
 
 msgctxt "model:product.uom,name:uom_carat"
 msgid "Carat"
-msgstr "Karat"
+msgstr "Carat"
 
 #, fuzzy
 msgctxt "model:product.uom,name:uom_centimeter"
 msgid "Centimeter"
-msgstr "sentimeter"
+msgstr "centimeter"
 
 msgctxt "model:product.uom,name:uom_cubic_centimeter"
 msgid "Cubic centimeter"
-msgstr "Centimeter kubik"
+msgstr "Cubic centimeter"
 
 msgctxt "model:product.uom,name:uom_cubic_foot"
 msgid "Cubic foot"
-msgstr "Kaki kubik"
+msgstr "Cubic foot"
 
 msgctxt "model:product.uom,name:uom_cubic_inch"
 msgid "Cubic inch"
-msgstr "Inci kubik"
+msgstr "Cubic inch"
 
 msgctxt "model:product.uom,name:uom_cubic_meter"
 msgid "Cubic meter"
-msgstr "Meter kubik"
+msgstr "Cubic meter"
 
 msgctxt "model:product.uom,name:uom_day"
 msgid "Day"
-msgstr "Hari"
+msgstr "Giorno"
 
 msgctxt "model:product.uom,name:uom_energy_joule"
 msgid "Joule"
 msgstr ""
 
 msgctxt "model:product.uom,name:uom_energy_kwh"
 msgid "Kilowatt-hour"
@@ -667,35 +719,35 @@
 
 msgctxt "model:product.uom,name:uom_energy_mwh"
 msgid "Megawatt-hour"
 msgstr ""
 
 msgctxt "model:product.uom,name:uom_foot"
 msgid "Foot"
-msgstr "Kaki"
+msgstr "Foot"
 
 msgctxt "model:product.uom,name:uom_gallon"
 msgid "Gallon"
-msgstr "Galon"
+msgstr "Gallon"
 
 msgctxt "model:product.uom,name:uom_gram"
 msgid "Gram"
 msgstr "Gram"
 
 msgctxt "model:product.uom,name:uom_hectare"
 msgid "Hectare"
-msgstr "Hektar"
+msgstr "Hectare"
 
 msgctxt "model:product.uom,name:uom_hour"
 msgid "Hour"
-msgstr "Jam"
+msgstr "Hour"
 
 msgctxt "model:product.uom,name:uom_inch"
 msgid "Inch"
-msgstr "Inci"
+msgstr "Inch"
 
 msgctxt "model:product.uom,name:uom_kilogram"
 msgid "Kilogram"
 msgstr "Kilogram"
 
 msgctxt "model:product.uom,name:uom_kilometer"
 msgid "Kilometer"
@@ -707,71 +759,71 @@
 
 msgctxt "model:product.uom,name:uom_meter"
 msgid "Meter"
 msgstr "Meter"
 
 msgctxt "model:product.uom,name:uom_mile"
 msgid "Mile"
-msgstr ""
+msgstr "Mile"
 
 msgctxt "model:product.uom,name:uom_millimeter"
 msgid "Millimeter"
 msgstr "Millimeter"
 
 msgctxt "model:product.uom,name:uom_minute"
 msgid "Minute"
-msgstr "Menit"
+msgstr "Minute"
 
 msgctxt "model:product.uom,name:uom_ounce"
 msgid "Ounce"
-msgstr "Ons"
+msgstr "Ounce"
 
 msgctxt "model:product.uom,name:uom_pound"
 msgid "Pound"
-msgstr ""
+msgstr "Pound"
 
 msgctxt "model:product.uom,name:uom_second"
 msgid "Second"
-msgstr "Detik"
+msgstr "Second"
 
 msgctxt "model:product.uom,name:uom_square_centimeter"
 msgid "Square centimeter"
-msgstr "Centimeter persegi"
+msgstr "Square centimeter"
 
 msgctxt "model:product.uom,name:uom_square_foot"
 msgid "Square foot"
-msgstr "Kaki persegi"
+msgstr "Square foot"
 
 msgctxt "model:product.uom,name:uom_square_inch"
 msgid "Square inch"
-msgstr "Inci persegi"
+msgstr "Square inch"
 
 msgctxt "model:product.uom,name:uom_square_meter"
 msgid "Square meter"
-msgstr "Meter persegi"
+msgstr "Square meter"
 
 msgctxt "model:product.uom,name:uom_square_yard"
 msgid "Square yard"
-msgstr "Yard persegi"
+msgstr "Square yard"
 
 msgctxt "model:product.uom,name:uom_unit"
 msgid "Unit"
-msgstr ""
+msgstr "Unità"
 
 msgctxt "model:product.uom,name:uom_yard"
 msgid "Yard"
-msgstr ""
+msgstr "Yard"
 
 msgctxt "model:product.uom,symbol:uom_are"
 msgid "a"
-msgstr ""
+msgstr "a"
 
 msgctxt "model:product.uom,symbol:uom_carat"
 msgid "c"
-msgstr ""
+msgstr "c"
 
 msgctxt "model:product.uom,symbol:uom_centimeter"
 msgid "cm"
 msgstr "cm"
 
 msgctxt "model:product.uom,symbol:uom_cubic_centimeter"
 msgid "cm³"
@@ -779,23 +831,23 @@
 
 msgctxt "model:product.uom,symbol:uom_cubic_foot"
 msgid "ft³"
 msgstr "ft³"
 
 msgctxt "model:product.uom,symbol:uom_cubic_inch"
 msgid "in³"
-msgstr ""
+msgstr "in³"
 
 msgctxt "model:product.uom,symbol:uom_cubic_meter"
 msgid "m³"
 msgstr "m³"
 
 msgctxt "model:product.uom,symbol:uom_day"
 msgid "d"
-msgstr ""
+msgstr "d"
 
 msgctxt "model:product.uom,symbol:uom_energy_joule"
 msgid "J"
 msgstr ""
 
 msgctxt "model:product.uom,symbol:uom_energy_kwh"
 msgid "kW⋅h"
@@ -807,35 +859,35 @@
 
 msgctxt "model:product.uom,symbol:uom_energy_mwh"
 msgid "MW⋅h"
 msgstr ""
 
 msgctxt "model:product.uom,symbol:uom_foot"
 msgid "ft"
-msgstr ""
+msgstr "ft"
 
 msgctxt "model:product.uom,symbol:uom_gallon"
 msgid "gal"
-msgstr ""
+msgstr "gal"
 
 msgctxt "model:product.uom,symbol:uom_gram"
 msgid "g"
-msgstr ""
+msgstr "g"
 
 msgctxt "model:product.uom,symbol:uom_hectare"
 msgid "ha"
-msgstr ""
+msgstr "ha"
 
 msgctxt "model:product.uom,symbol:uom_hour"
 msgid "h"
-msgstr ""
+msgstr "h"
 
 msgctxt "model:product.uom,symbol:uom_inch"
 msgid "in"
-msgstr ""
+msgstr "in"
 
 msgctxt "model:product.uom,symbol:uom_kilogram"
 msgid "kg"
 msgstr "kg"
 
 msgctxt "model:product.uom,symbol:uom_kilometer"
 msgid "km"
@@ -847,98 +899,103 @@
 
 msgctxt "model:product.uom,symbol:uom_meter"
 msgid "m"
 msgstr "m"
 
 msgctxt "model:product.uom,symbol:uom_mile"
 msgid "mi"
-msgstr ""
+msgstr "mi"
 
 msgctxt "model:product.uom,symbol:uom_millimeter"
 msgid "mm"
 msgstr "mm"
 
 msgctxt "model:product.uom,symbol:uom_minute"
 msgid "min"
-msgstr ""
+msgstr "min"
 
 msgctxt "model:product.uom,symbol:uom_ounce"
 msgid "oz"
-msgstr ""
+msgstr "oz"
 
 msgctxt "model:product.uom,symbol:uom_pound"
 msgid "lb"
-msgstr ""
+msgstr "lb"
 
 msgctxt "model:product.uom,symbol:uom_second"
 msgid "s"
-msgstr ""
+msgstr "s"
 
 msgctxt "model:product.uom,symbol:uom_square_centimeter"
 msgid "cm²"
 msgstr "cm²"
 
 msgctxt "model:product.uom,symbol:uom_square_foot"
 msgid "ft²"
-msgstr ""
+msgstr "ft²"
 
 msgctxt "model:product.uom,symbol:uom_square_inch"
 msgid "in²"
-msgstr ""
+msgstr "in²"
 
 msgctxt "model:product.uom,symbol:uom_square_meter"
 msgid "m²"
 msgstr "m²"
 
 msgctxt "model:product.uom,symbol:uom_square_yard"
 msgid "yd²"
-msgstr ""
+msgstr "yd²"
 
 msgctxt "model:product.uom,symbol:uom_unit"
 msgid "u"
-msgstr ""
+msgstr "u"
 
 msgctxt "model:product.uom,symbol:uom_yard"
 msgid "yd"
-msgstr ""
+msgstr "yd"
 
+#, fuzzy
 msgctxt "model:product.uom.category,name:"
 msgid "Unit of Measure Category"
-msgstr "Kategori Satuan Ukuran"
+msgstr "Unità di misura"
 
 msgctxt "model:product.uom.category,name:uom_cat_energy"
 msgid "Energy"
 msgstr ""
 
 msgctxt "model:product.uom.category,name:uom_cat_length"
 msgid "Length"
-msgstr "Panjang"
+msgstr "Lunghezza"
 
 msgctxt "model:product.uom.category,name:uom_cat_surface"
 msgid "Surface"
-msgstr ""
+msgstr "Surface"
 
 msgctxt "model:product.uom.category,name:uom_cat_time"
 msgid "Time"
-msgstr "Waktu"
+msgstr "Tempo"
 
 msgctxt "model:product.uom.category,name:uom_cat_unit"
 msgid "Units"
-msgstr ""
+msgstr "Unità"
 
 msgctxt "model:product.uom.category,name:uom_cat_volume"
 msgid "Volume"
-msgstr ""
+msgstr "Volume"
 
 msgctxt "model:product.uom.category,name:uom_cat_weight"
 msgid "Weight"
-msgstr "Berat"
+msgstr "Peso"
 
 msgctxt "model:res.group,name:group_product_admin"
 msgid "Product Administration"
+msgstr "Amministrazione prodotto"
+
+msgctxt "selection:product.identifier,type:"
+msgid "Brand"
 msgstr ""
 
 msgctxt "selection:product.identifier,type:"
 msgid "International Article Number"
 msgstr ""
 
 msgctxt "selection:product.identifier,type:"
@@ -957,58 +1014,65 @@
 msgid "International Standard Identifier for Libraries"
 msgstr ""
 
 msgctxt "selection:product.identifier,type:"
 msgid "International Standard Music Number"
 msgstr ""
 
+msgctxt "selection:product.identifier,type:"
+msgid "Manufacturer Part Number"
+msgstr ""
+
 msgctxt "selection:product.product,cost_price_method:"
 msgid "Average"
-msgstr ""
+msgstr "Media"
 
 msgctxt "selection:product.product,cost_price_method:"
 msgid "Fixed"
-msgstr ""
+msgstr "Fissa"
 
+#, fuzzy
 msgctxt "selection:product.product,type:"
 msgid "Assets"
-msgstr "Aset-Aset"
+msgstr "Immobilizzazioni"
 
 msgctxt "selection:product.product,type:"
 msgid "Goods"
-msgstr "Barang"
+msgstr "Beni"
 
 msgctxt "selection:product.product,type:"
 msgid "Service"
-msgstr "Jasa"
+msgstr "Servizio"
 
 msgctxt "selection:product.template,cost_price_method:"
 msgid "Average"
-msgstr ""
+msgstr "Media"
 
 msgctxt "selection:product.template,cost_price_method:"
 msgid "Fixed"
-msgstr ""
+msgstr "Fissa"
 
+#, fuzzy
 msgctxt "selection:product.template,type:"
 msgid "Assets"
-msgstr "Aset-Aset"
+msgstr "Immobilizzazioni"
 
 msgctxt "selection:product.template,type:"
 msgid "Goods"
-msgstr "Barang"
+msgstr "Beni"
 
 msgctxt "selection:product.template,type:"
 msgid "Service"
-msgstr "Jasa"
+msgstr "Servizio"
 
 msgctxt "view:product.category:"
 msgid "Children"
-msgstr "Cabang"
+msgstr "Figlio"
 
+#, fuzzy
 msgctxt "view:product.configuration:"
 msgid "Sequences"
-msgstr "Urutan-Urutan"
+msgstr "Modello prodotto"
 
 msgctxt "view:product.template:"
 msgid "General"
-msgstr "Umum"
+msgstr "Generale"
```

### Comparing `trytond_product-7.2.0/locale/it.po` & `trytond_product-7.2.1/locale/cs.po`

 * *Files 3% similar despite different names*

```diff
@@ -1,318 +1,339 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
-#, fuzzy
 msgctxt "field:ir.configuration,product_price_decimal:"
 msgid "Product Price Decimal"
-msgstr "Prezzo del prodotto"
+msgstr ""
 
 msgctxt "field:product.category,childs:"
 msgid "Children"
-msgstr "Figlio"
+msgstr ""
+
+msgctxt "field:product.category,code:"
+msgid "Code"
+msgstr ""
 
+msgctxt "field:product.category,code_readonly:"
+msgid "Code Readonly"
+msgstr ""
+
+#, fuzzy
 msgctxt "field:product.category,name:"
 msgid "Name"
-msgstr "Nome"
+msgstr "Namu"
 
 msgctxt "field:product.category,parent:"
 msgid "Parent"
-msgstr "Padre"
+msgstr ""
 
 #, fuzzy
 msgctxt "field:product.category,templates:"
 msgid "Products"
-msgstr "Prodotti"
+msgstr "Products"
+
+#, fuzzy
+msgctxt "field:product.configuration,category_sequence:"
+msgid "Category Sequence"
+msgstr "Product by Category"
 
 msgctxt "field:product.configuration,default_cost_price_method:"
 msgid "Default Cost Method"
-msgstr "Metodo di costo predefinito"
+msgstr ""
 
 #, fuzzy
 msgctxt "field:product.configuration,product_sequence:"
 msgid "Variant Sequence"
-msgstr "Modello prodotto"
+msgstr "Product by Category"
 
 #, fuzzy
 msgctxt "field:product.configuration,template_sequence:"
 msgid "Product Sequence"
-msgstr "Modello prodotto"
+msgstr "Product by Category"
 
-#, fuzzy
 msgctxt ""
 "field:product.configuration.default_cost_price_method,default_cost_price_method:"
 msgid "Default Cost Method"
-msgstr "Metodo di costo predefinito"
+msgstr ""
 
 msgctxt "field:product.cost_price,company:"
 msgid "Company"
-msgstr "Azienda"
+msgstr ""
 
 msgctxt "field:product.cost_price,cost_price:"
 msgid "Cost Price"
-msgstr "Prezzo di costo"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:product.cost_price,product:"
 msgid "Product"
-msgstr "Prodotto"
+msgstr "Product"
 
 msgctxt "field:product.cost_price_method,company:"
 msgid "Company"
-msgstr "Azienda"
+msgstr ""
 
 msgctxt "field:product.cost_price_method,cost_price_method:"
 msgid "Cost Price Method"
 msgstr ""
 
 msgctxt "field:product.cost_price_method,template:"
 msgid "Template"
-msgstr "Modello"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:product.identifier,code:"
 msgid "Code"
-msgstr "Codice"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:product.identifier,product:"
 msgid "Product"
-msgstr "Prodotto"
+msgstr "Product"
 
-#, fuzzy
 msgctxt "field:product.identifier,type:"
 msgid "Type"
-msgstr "Tipo"
+msgstr ""
 
 msgctxt "field:product.list_price,company:"
 msgid "Company"
-msgstr "Azienda"
+msgstr ""
 
 msgctxt "field:product.list_price,list_price:"
 msgid "List Price"
-msgstr "Listino prezzi"
+msgstr ""
 
 msgctxt "field:product.list_price,template:"
 msgid "Template"
-msgstr "Modello"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:product.product,categories:"
 msgid "Categories"
-msgstr "Categorie"
+msgstr "Categories"
 
+#, fuzzy
 msgctxt "field:product.product,categories_all:"
 msgid "Categories"
-msgstr "Categorie"
+msgstr "Categories"
 
 msgctxt "field:product.product,code:"
 msgid "Code"
-msgstr "Codice"
+msgstr ""
 
 msgctxt "field:product.product,code_readonly:"
 msgid "Code Readonly"
 msgstr ""
 
 msgctxt "field:product.product,consumable:"
 msgid "Consumable"
-msgstr "Consumabile"
+msgstr ""
 
 msgctxt "field:product.product,cost_price:"
 msgid "Cost Price"
-msgstr "Prezzo di costo"
+msgstr ""
 
 msgctxt "field:product.product,cost_price_method:"
 msgid "Cost Price Method"
 msgstr ""
 
 msgctxt "field:product.product,cost_price_methods:"
 msgid "Cost Price Methods"
 msgstr ""
 
 msgctxt "field:product.product,cost_price_uom:"
 msgid "Cost Price"
-msgstr "Prezzo di costo"
+msgstr ""
 
 msgctxt "field:product.product,cost_prices:"
 msgid "Cost Prices"
-msgstr "Costi"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:product.product,default_uom:"
 msgid "Default UoM"
-msgstr "UdM predefinita"
+msgstr ""
 
 #, fuzzy
 msgctxt "field:product.product,default_uom_category:"
 msgid "Default UoM Category"
-msgstr "UdM predefinita"
+msgstr "Product by Category"
 
 msgctxt "field:product.product,description:"
 msgid "Description"
-msgstr "Descrizione"
+msgstr ""
 
 msgctxt "field:product.product,identifiers:"
 msgid "Identifiers"
 msgstr ""
 
 msgctxt "field:product.product,list_price:"
 msgid "List Price"
-msgstr "Listino prezzi"
+msgstr ""
 
 msgctxt "field:product.product,list_price_uom:"
 msgid "List Price"
-msgstr "Listino prezzi"
+msgstr ""
 
 msgctxt "field:product.product,list_prices:"
 msgid "List Prices"
-msgstr "Listino prezzi"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:product.product,name:"
 msgid "Name"
-msgstr "Nome"
+msgstr "Namu"
 
 msgctxt "field:product.product,prefix_code:"
 msgid "Prefix Code"
 msgstr ""
 
 msgctxt "field:product.product,suffix_code:"
 msgid "Suffix Code"
 msgstr ""
 
 msgctxt "field:product.product,template:"
 msgid "Product Template"
-msgstr "Modello prodotto"
+msgstr ""
 
 msgctxt "field:product.product,type:"
 msgid "Type"
-msgstr "Tipo"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:product.template,categories:"
 msgid "Categories"
-msgstr "Categorie"
+msgstr "Categories"
 
+#, fuzzy
 msgctxt "field:product.template,categories_all:"
 msgid "Categories"
-msgstr "Categorie"
+msgstr "Categories"
 
-#, fuzzy
 msgctxt "field:product.template,code:"
 msgid "Code"
-msgstr "Codice"
+msgstr ""
 
 msgctxt "field:product.template,code_readonly:"
 msgid "Code Readonly"
 msgstr ""
 
 msgctxt "field:product.template,consumable:"
 msgid "Consumable"
-msgstr "Consumabile"
+msgstr ""
 
 msgctxt "field:product.template,cost_price:"
 msgid "Cost Price"
-msgstr "Prezzo di costo"
+msgstr ""
 
 msgctxt "field:product.template,cost_price_method:"
 msgid "Cost Price Method"
 msgstr ""
 
 msgctxt "field:product.template,cost_price_methods:"
 msgid "Cost Price Methods"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:product.template,default_uom:"
 msgid "Default UoM"
-msgstr "UdM predefinita"
+msgstr ""
 
 #, fuzzy
 msgctxt "field:product.template,default_uom_category:"
 msgid "Default UoM Category"
-msgstr "UdM predefinita"
+msgstr "Product by Category"
 
 msgctxt "field:product.template,list_price:"
 msgid "List Price"
-msgstr "Listino prezzi"
+msgstr ""
 
 msgctxt "field:product.template,list_prices:"
 msgid "List Prices"
-msgstr "Listino prezzi"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:product.template,name:"
 msgid "Name"
-msgstr "Nome"
+msgstr "Namu"
 
+#, fuzzy
 msgctxt "field:product.template,products:"
 msgid "Variants"
-msgstr "Varianti"
+msgstr "Variants"
 
 msgctxt "field:product.template,type:"
 msgid "Type"
-msgstr "Tipo"
+msgstr ""
 
 msgctxt "field:product.template-product.category,category:"
 msgid "Category"
-msgstr "Categoria"
+msgstr ""
 
 msgctxt "field:product.template-product.category,template:"
 msgid "Template"
-msgstr "Modello"
+msgstr ""
 
 msgctxt "field:product.template-product.category.all,category:"
 msgid "Category"
-msgstr "Categoria"
+msgstr ""
 
 msgctxt "field:product.template-product.category.all,template:"
 msgid "Template"
-msgstr "Modello"
+msgstr ""
 
 msgctxt "field:product.uom,category:"
 msgid "Category"
-msgstr "Categoria"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:product.uom,digits:"
 msgid "Display Digits"
-msgstr "Posizioni"
+msgstr ""
 
 msgctxt "field:product.uom,factor:"
 msgid "Factor"
-msgstr "Fattore"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:product.uom,name:"
 msgid "Name"
-msgstr "Nome"
+msgstr "Namu"
 
 msgctxt "field:product.uom,rate:"
 msgid "Rate"
-msgstr "Cambio"
+msgstr ""
 
 msgctxt "field:product.uom,rounding:"
 msgid "Rounding Precision"
-msgstr "Precisione di arrotondamento"
+msgstr ""
 
 msgctxt "field:product.uom,symbol:"
 msgid "Symbol"
-msgstr "Simbolo"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:product.uom.category,name:"
 msgid "Name"
-msgstr "Nome"
+msgstr "Namu"
 
 #, fuzzy
 msgctxt "field:product.uom.category,uoms:"
 msgid "Units of Measure"
 msgstr "Units of Measure"
 
 msgctxt "help:product.category,childs:"
 msgid "Used to add structure below the category."
 msgstr ""
 
 msgctxt "help:product.category,parent:"
 msgid "Used to add structure above the category."
 msgstr ""
 
+msgctxt "help:product.configuration,category_sequence:"
+msgid "Used to generate the category code."
+msgstr ""
+
 msgctxt "help:product.configuration,default_cost_price_method:"
 msgid "The default cost price method for new products."
 msgstr ""
 
 msgctxt "help:product.configuration,product_sequence:"
 msgid "Used to generate the last part of the product code."
 msgstr ""
@@ -427,56 +448,51 @@
 "Conversions between different units of measure can be done if they are in the same category."
 msgstr ""
 
 msgctxt "help:product.uom,digits:"
 msgid "The number of digits to display after the decimal separator."
 msgstr ""
 
-#, fuzzy
 msgctxt "help:product.uom,factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "coefficient (base unit) = 1 (this unit)"
 msgstr ""
-"Il coefficiente per la formula:\n"
-"coef (unità base) = 1 (questa unità)"
 
 msgctxt "help:product.uom,rate:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (base unit) = coef (this unit)"
 msgstr ""
-"Il coefficiente per la formula:\n"
-"1 (unità base) = coef (questa unità)"
 
 msgctxt "help:product.uom,rounding:"
 msgid "The accuracy to which values are rounded."
 msgstr ""
 
 msgctxt "help:product.uom,symbol:"
 msgid "The symbol that represents the unit of measure."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_category_list"
 msgid "Categories"
-msgstr "Categorie"
+msgstr "Categories"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_category_product"
 msgid "Add products"
-msgstr "Prodotti"
+msgstr "Products"
 
 msgctxt "model:ir.action,name:act_category_tree"
 msgid "Categories"
-msgstr "Categorie"
+msgstr "Categories"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_product_configuration_form"
 msgid "Configuration"
-msgstr "Configurazione"
+msgstr "Configuration"
 
 msgctxt "model:ir.action,name:act_product_form"
 msgid "Variants"
 msgstr "Variants"
 
 msgctxt "model:ir.action,name:act_product_from_template"
 msgid "Variants"
@@ -484,25 +500,29 @@
 
 msgctxt "model:ir.action,name:act_template_by_category"
 msgid "Product by Category"
 msgstr "Product by Category"
 
 msgctxt "model:ir.action,name:act_template_form"
 msgid "Products"
-msgstr "Prodotti"
+msgstr "Products"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_uom_category_form"
 msgid "Categories"
-msgstr "Categorie"
+msgstr "Categories"
 
 msgctxt "model:ir.action,name:act_uom_form"
 msgid "Units of Measure"
 msgstr "Units of Measure"
 
+msgctxt "model:ir.message,text:msg_category_code_unique"
+msgid "The code on product category must be unique."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_invalid_code"
 msgid "The %(type)s \"%(code)s\" for product \"%(product)s\" is not valid."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_product_code_unique"
 msgid "Code of active product must be unique."
 msgstr ""
@@ -536,118 +556,124 @@
 msgctxt "model:ir.message,text:msg_uom_no_zero_factor_rate"
 msgid "Rate and factor can not be both equal to zero."
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.model.button,string:category_add_products_button"
 msgid "Add products"
-msgstr "Prodotti"
+msgstr "Products"
+
+#, fuzzy
+msgctxt "model:ir.sequence.type,name:sequence_type_category"
+msgid "Category"
+msgstr "Categories"
 
 #, fuzzy
 msgctxt "model:ir.sequence.type,name:sequence_type_product"
 msgid "Variant"
-msgstr "Varianti"
+msgstr "Variants"
 
 #, fuzzy
 msgctxt "model:ir.sequence.type,name:sequence_type_template"
 msgid "Product"
-msgstr "Prodotto"
+msgstr "Product"
 
 msgctxt "model:ir.ui.menu,name:menu_category_list"
 msgid "Categories"
-msgstr "Categorie"
+msgstr "Categories"
 
 msgctxt "model:ir.ui.menu,name:menu_category_tree"
 msgid "Categories"
-msgstr "Categorie"
+msgstr "Categories"
 
 msgctxt "model:ir.ui.menu,name:menu_configuration"
 msgid "Configuration"
-msgstr "Configurazione"
+msgstr "Configuration"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_main_product"
 msgid "Products"
-msgstr "Prodotti"
+msgstr "Products"
 
 msgctxt "model:ir.ui.menu,name:menu_product"
 msgid "Variants"
 msgstr "Variants"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_product_configuration"
 msgid "Configuration"
-msgstr "Configurazione"
+msgstr "Configuration"
 
 msgctxt "model:ir.ui.menu,name:menu_reporting"
 msgid "Reporting"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_template"
 msgid "Products"
-msgstr "Prodotti"
+msgstr "Products"
 
 msgctxt "model:ir.ui.menu,name:menu_uom_category_form"
 msgid "Categories"
-msgstr "Categorie"
+msgstr "Categories"
 
 msgctxt "model:ir.ui.menu,name:menu_uom_form"
 msgid "Units of Measure"
 msgstr "Units of Measure"
 
+#, fuzzy
 msgctxt "model:product.category,name:"
 msgid "Product Category"
-msgstr "Categoria Prodotto"
+msgstr "Product by Category"
 
 #, fuzzy
 msgctxt "model:product.configuration,name:"
 msgid "Product Configuration"
 msgstr "Product Configuration"
 
 msgctxt "model:product.configuration.default_cost_price_method,name:"
 msgid "Product Configuration Default Cost Price Method"
 msgstr ""
 
 msgctxt "model:product.cost_price,name:"
 msgid "Product Cost Price"
-msgstr "Prezzo del prodotto"
+msgstr ""
 
 msgctxt "model:product.cost_price_method,name:"
 msgid "Product Cost Price Method"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:product.identifier,name:"
 msgid "Product Identifier"
-msgstr "Modello prodotto"
+msgstr "Product by Category"
 
 msgctxt "model:product.list_price,name:"
 msgid "Product List Price"
-msgstr "Prezzo di listino dei prodotti"
+msgstr ""
 
 msgctxt "model:product.product,name:"
 msgid "Product Variant"
-msgstr "Variante prodotto"
+msgstr ""
 
 msgctxt "model:product.template,name:"
 msgid "Product Template"
-msgstr "Modello prodotto"
+msgstr ""
 
 msgctxt "model:product.template-product.category,name:"
 msgid "Template - Category"
 msgstr ""
 
 msgctxt "model:product.template-product.category.all,name:"
 msgid "Template - Category All"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:product.uom,name:"
 msgid "Unit of Measure"
-msgstr "Unità di misura"
+msgstr "Units of Measure"
 
 msgctxt "model:product.uom,name:uom_are"
 msgid "Are"
 msgstr "Are"
 
 msgctxt "model:product.uom,name:uom_carat"
 msgid "Carat"
@@ -672,15 +698,15 @@
 
 msgctxt "model:product.uom,name:uom_cubic_meter"
 msgid "Cubic meter"
 msgstr "Cubic meter"
 
 msgctxt "model:product.uom,name:uom_day"
 msgid "Day"
-msgstr "Giorno"
+msgstr "Day"
 
 msgctxt "model:product.uom,name:uom_energy_joule"
 msgid "Joule"
 msgstr ""
 
 msgctxt "model:product.uom,name:uom_energy_kwh"
 msgid "Kilowatt-hour"
@@ -776,15 +802,15 @@
 
 msgctxt "model:product.uom,name:uom_square_yard"
 msgid "Square yard"
 msgstr "Square yard"
 
 msgctxt "model:product.uom,name:uom_unit"
 msgid "Unit"
-msgstr "Unità"
+msgstr "Unit"
 
 msgctxt "model:product.uom,name:uom_yard"
 msgid "Yard"
 msgstr "Yard"
 
 msgctxt "model:product.uom,symbol:uom_are"
 msgid "a"
@@ -925,47 +951,51 @@
 msgctxt "model:product.uom,symbol:uom_yard"
 msgid "yd"
 msgstr "yd"
 
 #, fuzzy
 msgctxt "model:product.uom.category,name:"
 msgid "Unit of Measure Category"
-msgstr "Unità di misura"
+msgstr "Units of Measure"
 
 msgctxt "model:product.uom.category,name:uom_cat_energy"
 msgid "Energy"
 msgstr ""
 
 msgctxt "model:product.uom.category,name:uom_cat_length"
 msgid "Length"
-msgstr "Lunghezza"
+msgstr "Length"
 
 msgctxt "model:product.uom.category,name:uom_cat_surface"
 msgid "Surface"
 msgstr "Surface"
 
 msgctxt "model:product.uom.category,name:uom_cat_time"
 msgid "Time"
-msgstr "Tempo"
+msgstr "Time"
 
 msgctxt "model:product.uom.category,name:uom_cat_unit"
 msgid "Units"
-msgstr "Unità"
+msgstr "Units"
 
 msgctxt "model:product.uom.category,name:uom_cat_volume"
 msgid "Volume"
 msgstr "Volume"
 
 msgctxt "model:product.uom.category,name:uom_cat_weight"
 msgid "Weight"
-msgstr "Peso"
+msgstr "Weight"
 
 msgctxt "model:res.group,name:group_product_admin"
 msgid "Product Administration"
-msgstr "Amministrazione prodotto"
+msgstr "Product Administration"
+
+msgctxt "selection:product.identifier,type:"
+msgid "Brand"
+msgstr ""
 
 msgctxt "selection:product.identifier,type:"
 msgid "International Article Number"
 msgstr ""
 
 msgctxt "selection:product.identifier,type:"
 msgid "International Securities Identification Number"
@@ -983,61 +1013,63 @@
 msgid "International Standard Identifier for Libraries"
 msgstr ""
 
 msgctxt "selection:product.identifier,type:"
 msgid "International Standard Music Number"
 msgstr ""
 
+msgctxt "selection:product.identifier,type:"
+msgid "Manufacturer Part Number"
+msgstr ""
+
 msgctxt "selection:product.product,cost_price_method:"
 msgid "Average"
-msgstr "Media"
+msgstr ""
 
 msgctxt "selection:product.product,cost_price_method:"
 msgid "Fixed"
-msgstr "Fissa"
+msgstr ""
 
-#, fuzzy
 msgctxt "selection:product.product,type:"
 msgid "Assets"
-msgstr "Immobilizzazioni"
+msgstr ""
 
 msgctxt "selection:product.product,type:"
 msgid "Goods"
-msgstr "Beni"
+msgstr ""
 
 msgctxt "selection:product.product,type:"
 msgid "Service"
-msgstr "Servizio"
+msgstr ""
 
 msgctxt "selection:product.template,cost_price_method:"
 msgid "Average"
-msgstr "Media"
+msgstr ""
 
 msgctxt "selection:product.template,cost_price_method:"
 msgid "Fixed"
-msgstr "Fissa"
+msgstr ""
 
-#, fuzzy
 msgctxt "selection:product.template,type:"
 msgid "Assets"
-msgstr "Immobilizzazioni"
+msgstr ""
 
 msgctxt "selection:product.template,type:"
 msgid "Goods"
-msgstr "Beni"
+msgstr ""
 
 msgctxt "selection:product.template,type:"
 msgid "Service"
-msgstr "Servizio"
+msgstr ""
 
 msgctxt "view:product.category:"
 msgid "Children"
-msgstr "Figlio"
+msgstr ""
 
 #, fuzzy
 msgctxt "view:product.configuration:"
 msgid "Sequences"
-msgstr "Modello prodotto"
+msgstr "Product by Category"
 
 msgctxt "view:product.template:"
 msgid "General"
-msgstr "Generale"
+msgstr ""
```

### Comparing `trytond_product-7.2.0/locale/lo.po` & `trytond_product-7.2.1/locale/lo.po`

 * *Files 1% similar despite different names*

```diff
@@ -7,27 +7,41 @@
 msgid "Product Price Decimal"
 msgstr "ຜະລິດຕະພັນຍ່ອຍ"
 
 msgctxt "field:product.category,childs:"
 msgid "Children"
 msgstr "ໝວດຍ່ອຍ"
 
+#, fuzzy
+msgctxt "field:product.category,code:"
+msgid "Code"
+msgstr "ລະຫັດ"
+
+msgctxt "field:product.category,code_readonly:"
+msgid "Code Readonly"
+msgstr ""
+
 msgctxt "field:product.category,name:"
 msgid "Name"
 msgstr "ຊື່"
 
 msgctxt "field:product.category,parent:"
 msgid "Parent"
 msgstr "ບັນຊີແມ່"
 
 #, fuzzy
 msgctxt "field:product.category,templates:"
 msgid "Products"
 msgstr "Products"
 
+#, fuzzy
+msgctxt "field:product.configuration,category_sequence:"
+msgid "Category Sequence"
+msgstr "ຮ່າງແບບຜະລິດຕະພັນ"
+
 msgctxt "field:product.configuration,default_cost_price_method:"
 msgid "Default Cost Method"
 msgstr "ວິທີຄິດໄລ່ລາຄາເດີມ"
 
 #, fuzzy
 msgctxt "field:product.configuration,product_sequence:"
 msgid "Variant Sequence"
@@ -317,14 +331,18 @@
 msgid "Used to add structure below the category."
 msgstr ""
 
 msgctxt "help:product.category,parent:"
 msgid "Used to add structure above the category."
 msgstr ""
 
+msgctxt "help:product.configuration,category_sequence:"
+msgid "Used to generate the category code."
+msgstr ""
+
 msgctxt "help:product.configuration,default_cost_price_method:"
 msgid "The default cost price method for new products."
 msgstr ""
 
 msgctxt "help:product.configuration,product_sequence:"
 msgid "Used to generate the last part of the product code."
 msgstr ""
@@ -514,14 +532,18 @@
 msgstr "ປະເພດ"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_uom_form"
 msgid "Units of Measure"
 msgstr "Units of Measure"
 
+msgctxt "model:ir.message,text:msg_category_code_unique"
+msgid "The code on product category must be unique."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_invalid_code"
 msgid "The %(type)s \"%(code)s\" for product \"%(product)s\" is not valid."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_product_code_unique"
 msgid "Code of active product must be unique."
 msgstr ""
@@ -558,14 +580,19 @@
 
 #, fuzzy
 msgctxt "model:ir.model.button,string:category_add_products_button"
 msgid "Add products"
 msgstr "Products"
 
 #, fuzzy
+msgctxt "model:ir.sequence.type,name:sequence_type_category"
+msgid "Category"
+msgstr "ປະເພດ"
+
+#, fuzzy
 msgctxt "model:ir.sequence.type,name:sequence_type_product"
 msgid "Variant"
 msgstr "ຜະລິດຕະພັນຍ່ອຍ"
 
 #, fuzzy
 msgctxt "model:ir.sequence.type,name:sequence_type_template"
 msgid "Product"
@@ -1053,14 +1080,18 @@
 
 #, fuzzy
 msgctxt "model:res.group,name:group_product_admin"
 msgid "Product Administration"
 msgstr "Product Administration"
 
 msgctxt "selection:product.identifier,type:"
+msgid "Brand"
+msgstr ""
+
+msgctxt "selection:product.identifier,type:"
 msgid "International Article Number"
 msgstr ""
 
 msgctxt "selection:product.identifier,type:"
 msgid "International Securities Identification Number"
 msgstr ""
 
@@ -1076,14 +1107,18 @@
 msgid "International Standard Identifier for Libraries"
 msgstr ""
 
 msgctxt "selection:product.identifier,type:"
 msgid "International Standard Music Number"
 msgstr ""
 
+msgctxt "selection:product.identifier,type:"
+msgid "Manufacturer Part Number"
+msgstr ""
+
 msgctxt "selection:product.product,cost_price_method:"
 msgid "Average"
 msgstr "ສະເລັ່ຍ"
 
 msgctxt "selection:product.product,cost_price_method:"
 msgid "Fixed"
 msgstr "ຄົງທີ່"
```

### Comparing `trytond_product-7.2.0/locale/lt.po` & `trytond_product-7.2.1/locale/lt.po`

 * *Files 3% similar despite different names*

```diff
@@ -7,27 +7,41 @@
 msgid "Product Price Decimal"
 msgstr "Prekės savikaina"
 
 msgctxt "field:product.category,childs:"
 msgid "Children"
 msgstr "Dukterinės"
 
+#, fuzzy
+msgctxt "field:product.category,code:"
+msgid "Code"
+msgstr "Kodas"
+
+msgctxt "field:product.category,code_readonly:"
+msgid "Code Readonly"
+msgstr ""
+
 msgctxt "field:product.category,name:"
 msgid "Name"
 msgstr "Pavadinimas"
 
 msgctxt "field:product.category,parent:"
 msgid "Parent"
 msgstr "Motininė"
 
 #, fuzzy
 msgctxt "field:product.category,templates:"
 msgid "Products"
 msgstr "Prekės"
 
+#, fuzzy
+msgctxt "field:product.configuration,category_sequence:"
+msgid "Category Sequence"
+msgstr "Numeruotė"
+
 msgctxt "field:product.configuration,default_cost_price_method:"
 msgid "Default Cost Method"
 msgstr "Numatytasis savikainos metodas"
 
 #, fuzzy
 msgctxt "field:product.configuration,product_sequence:"
 msgid "Variant Sequence"
@@ -301,14 +315,18 @@
 msgid "Used to add structure below the category."
 msgstr ""
 
 msgctxt "help:product.category,parent:"
 msgid "Used to add structure above the category."
 msgstr ""
 
+msgctxt "help:product.configuration,category_sequence:"
+msgid "Used to generate the category code."
+msgstr ""
+
 msgctxt "help:product.configuration,default_cost_price_method:"
 msgid "The default cost price method for new products."
 msgstr ""
 
 msgctxt "help:product.configuration,product_sequence:"
 msgid "Used to generate the last part of the product code."
 msgstr ""
@@ -494,14 +512,18 @@
 msgid "Categories"
 msgstr "Kategorijos"
 
 msgctxt "model:ir.action,name:act_uom_form"
 msgid "Units of Measure"
 msgstr "Mato vienetai"
 
+msgctxt "model:ir.message,text:msg_category_code_unique"
+msgid "The code on product category must be unique."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_invalid_code"
 msgid "The %(type)s \"%(code)s\" for product \"%(product)s\" is not valid."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_product_code_unique"
 msgid "Code of active product must be unique."
 msgstr ""
@@ -538,14 +560,19 @@
 
 #, fuzzy
 msgctxt "model:ir.model.button,string:category_add_products_button"
 msgid "Add products"
 msgstr "Prekės"
 
 #, fuzzy
+msgctxt "model:ir.sequence.type,name:sequence_type_category"
+msgid "Category"
+msgstr "Kategorija"
+
+#, fuzzy
 msgctxt "model:ir.sequence.type,name:sequence_type_product"
 msgid "Variant"
 msgstr "Variantai"
 
 #, fuzzy
 msgctxt "model:ir.sequence.type,name:sequence_type_template"
 msgid "Product"
@@ -957,14 +984,18 @@
 msgstr "Svoris"
 
 msgctxt "model:res.group,name:group_product_admin"
 msgid "Product Administration"
 msgstr "Prekių valdymas"
 
 msgctxt "selection:product.identifier,type:"
+msgid "Brand"
+msgstr ""
+
+msgctxt "selection:product.identifier,type:"
 msgid "International Article Number"
 msgstr "Tarptautinis artikulas"
 
 msgctxt "selection:product.identifier,type:"
 msgid "International Securities Identification Number"
 msgstr "Tarptautinis saugumo numeris"
 
@@ -980,14 +1011,18 @@
 msgid "International Standard Identifier for Libraries"
 msgstr "Tarptautinis standartinis bibliotekų identifikatorius"
 
 msgctxt "selection:product.identifier,type:"
 msgid "International Standard Music Number"
 msgstr "Tarptautinis standartinis muzikos numeris"
 
+msgctxt "selection:product.identifier,type:"
+msgid "Manufacturer Part Number"
+msgstr ""
+
 msgctxt "selection:product.product,cost_price_method:"
 msgid "Average"
 msgstr "Vidutinė"
 
 msgctxt "selection:product.product,cost_price_method:"
 msgid "Fixed"
 msgstr "Fiksuota"
```

### Comparing `trytond_product-7.2.0/locale/nl.po` & `trytond_product-7.2.1/locale/nl.po`

 * *Files 3% similar despite different names*

```diff
@@ -6,26 +6,38 @@
 msgid "Product Price Decimal"
 msgstr "Productprijs decimalen"
 
 msgctxt "field:product.category,childs:"
 msgid "Children"
 msgstr "Onderliggende niveaus"
 
+msgctxt "field:product.category,code:"
+msgid "Code"
+msgstr "Code"
+
+msgctxt "field:product.category,code_readonly:"
+msgid "Code Readonly"
+msgstr "Code Alleen lezen"
+
 msgctxt "field:product.category,name:"
 msgid "Name"
 msgstr "Naam"
 
 msgctxt "field:product.category,parent:"
 msgid "Parent"
 msgstr "Bovenliggend niveau"
 
 msgctxt "field:product.category,templates:"
 msgid "Products"
 msgstr "Producten"
 
+msgctxt "field:product.configuration,category_sequence:"
+msgid "Category Sequence"
+msgstr "Categorie reeks"
+
 msgctxt "field:product.configuration,default_cost_price_method:"
 msgid "Default Cost Method"
 msgstr "Standaard kostprijs methode"
 
 msgctxt "field:product.configuration,product_sequence:"
 msgid "Variant Sequence"
 msgstr "Variant reeks"
@@ -291,14 +303,18 @@
 msgid "Used to add structure below the category."
 msgstr "Wordt gebruikt om een structuur onder de categorie toe te voegen."
 
 msgctxt "help:product.category,parent:"
 msgid "Used to add structure above the category."
 msgstr "Wordt gebruikt om een structuur boven de categorie toe te voegen."
 
+msgctxt "help:product.configuration,category_sequence:"
+msgid "Used to generate the category code."
+msgstr "Wordt gebruikt de categorie code te genereren."
+
 msgctxt "help:product.configuration,default_cost_price_method:"
 msgid "The default cost price method for new products."
 msgstr "De standaard kostprijs methode voor nieuwe producten."
 
 msgctxt "help:product.configuration,product_sequence:"
 msgid "Used to generate the last part of the product code."
 msgstr "Wordt gebruikt om het laatste deel van de productcode te genereren."
@@ -495,14 +511,18 @@
 msgid "Categories"
 msgstr "Categorieën"
 
 msgctxt "model:ir.action,name:act_uom_form"
 msgid "Units of Measure"
 msgstr "Maateenheden"
 
+msgctxt "model:ir.message,text:msg_category_code_unique"
+msgid "The code on product category must be unique."
+msgstr "Code van het product categorie moet uniek zijn."
+
 msgctxt "model:ir.message,text:msg_invalid_code"
 msgid "The %(type)s \"%(code)s\" for product \"%(product)s\" is not valid."
 msgstr "Het %(type)s \"%(code)s\" voor product \"%(product)s\" is niet geldig."
 
 msgctxt "model:ir.message,text:msg_product_code_unique"
 msgid "Code of active product must be unique."
 msgstr "Code van actief product moet uniek zijn."
@@ -517,15 +537,15 @@
 
 msgctxt "model:ir.message,text:msg_uom_modify_category"
 msgid "You cannot modify the category of the unit of measure \"%(uom)s\"."
 msgstr "U kunt de categorie van maateenheid \"%(uom)s\" niet wijzigen."
 
 msgctxt "model:ir.message,text:msg_uom_modify_factor"
 msgid "You cannot modify the factor of the unit of measure \"%(uom)s\"."
-msgstr "U kunt de factor van maateenheid \"% (uom) s\" niet wijzigen."
+msgstr "U kunt de factor van maateenheid \"%(uom)s\" niet wijzigen."
 
 msgctxt "model:ir.message,text:msg_uom_modify_options"
 msgid ""
 "If the unit of measure is still not used, you can delete it otherwise you "
 "can deactivate it and create a new one."
 msgstr ""
 "Als de maateenheid nog niet wordt gebruikt, kunt u deze verwijderen, anders "
@@ -539,14 +559,18 @@
 msgid "Rate and factor can not be both equal to zero."
 msgstr "De verhouding en factor kunnen niet beiden gelijk zijn aan nul."
 
 msgctxt "model:ir.model.button,string:category_add_products_button"
 msgid "Add products"
 msgstr "Producten toevoegen"
 
+msgctxt "model:ir.sequence.type,name:sequence_type_category"
+msgid "Category"
+msgstr "Categorie"
+
 msgctxt "model:ir.sequence.type,name:sequence_type_product"
 msgid "Variant"
 msgstr "Variant"
 
 msgctxt "model:ir.sequence.type,name:sequence_type_template"
 msgid "Product"
 msgstr "Product"
@@ -952,14 +976,18 @@
 msgstr "Gewicht"
 
 msgctxt "model:res.group,name:group_product_admin"
 msgid "Product Administration"
 msgstr "Product administratie"
 
 msgctxt "selection:product.identifier,type:"
+msgid "Brand"
+msgstr "Merk"
+
+msgctxt "selection:product.identifier,type:"
 msgid "International Article Number"
 msgstr "Internationaal artikelnummer"
 
 msgctxt "selection:product.identifier,type:"
 msgid "International Securities Identification Number"
 msgstr "Internationaal veiligheids idendificatie nummer (ISIN)"
 
@@ -975,14 +1003,18 @@
 msgid "International Standard Identifier for Libraries"
 msgstr "Internationale standaardidentificatie voor bibliotheken"
 
 msgctxt "selection:product.identifier,type:"
 msgid "International Standard Music Number"
 msgstr "Internationaal standaard muzieknummer"
 
+msgctxt "selection:product.identifier,type:"
+msgid "Manufacturer Part Number"
+msgstr "Onderdeel nummer fabrikant"
+
 msgctxt "selection:product.product,cost_price_method:"
 msgid "Average"
 msgstr "Gemiddeld"
 
 msgctxt "selection:product.product,cost_price_method:"
 msgid "Fixed"
 msgstr "Vast"
```

### Comparing `trytond_product-7.2.0/locale/pl.po` & `trytond_product-7.2.1/locale/zh_CN.po`

 * *Files 5% similar despite different names*

```diff
@@ -1,806 +1,805 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:ir.configuration,product_price_decimal:"
 msgid "Product Price Decimal"
-msgstr "Cena produktu po przecinku"
+msgstr "产品价格小数"
 
 msgctxt "field:product.category,childs:"
 msgid "Children"
-msgstr "Kategorie podrzędne"
+msgstr "子类别"
+
+#, fuzzy
+msgctxt "field:product.category,code:"
+msgid "Code"
+msgstr "代码"
+
+#, fuzzy
+msgctxt "field:product.category,code_readonly:"
+msgid "Code Readonly"
+msgstr "只读代码"
 
 msgctxt "field:product.category,name:"
 msgid "Name"
-msgstr "Nazwa"
+msgstr "名称"
 
 msgctxt "field:product.category,parent:"
 msgid "Parent"
-msgstr "Kategoria nadrzędna"
+msgstr "父类别"
 
-#, fuzzy
 msgctxt "field:product.category,templates:"
 msgid "Products"
-msgstr "Produkty"
+msgstr "产品"
+
+#, fuzzy
+msgctxt "field:product.configuration,category_sequence:"
+msgid "Category Sequence"
+msgstr "产品变体序列"
 
 msgctxt "field:product.configuration,default_cost_price_method:"
 msgid "Default Cost Method"
-msgstr "Domyślna metoda kosztowa"
+msgstr "默认成本法"
 
 msgctxt "field:product.configuration,product_sequence:"
 msgid "Variant Sequence"
-msgstr "Sekwencja wariantu produktu"
+msgstr "产品变体序列"
 
 msgctxt "field:product.configuration,template_sequence:"
 msgid "Product Sequence"
-msgstr "Sekwencja produktu"
+msgstr "产品序列"
 
 msgctxt ""
 "field:product.configuration.default_cost_price_method,default_cost_price_method:"
 msgid "Default Cost Method"
-msgstr "Domyślna metoda kosztowa"
+msgstr "默认成本法"
 
 msgctxt "field:product.cost_price,company:"
 msgid "Company"
-msgstr "Firma"
+msgstr "公司"
 
 msgctxt "field:product.cost_price,cost_price:"
 msgid "Cost Price"
-msgstr "Cena kosztów"
+msgstr "成本价"
 
 msgctxt "field:product.cost_price,product:"
 msgid "Product"
-msgstr "Produkt"
+msgstr "产品"
 
 msgctxt "field:product.cost_price_method,company:"
 msgid "Company"
-msgstr "Firma"
+msgstr "公司"
 
 msgctxt "field:product.cost_price_method,cost_price_method:"
 msgid "Cost Price Method"
-msgstr "Metoda wyceny zapasów"
+msgstr "成本价法"
 
 msgctxt "field:product.cost_price_method,template:"
 msgid "Template"
-msgstr "Szablon"
+msgstr "模板"
 
 msgctxt "field:product.identifier,code:"
 msgid "Code"
-msgstr "Kod"
+msgstr "代码"
 
 msgctxt "field:product.identifier,product:"
 msgid "Product"
-msgstr "Produkt"
+msgstr "产品"
 
 msgctxt "field:product.identifier,type:"
 msgid "Type"
-msgstr "Typ"
+msgstr "类型"
 
 msgctxt "field:product.list_price,company:"
 msgid "Company"
-msgstr "Firma"
+msgstr "公司"
 
 msgctxt "field:product.list_price,list_price:"
 msgid "List Price"
-msgstr "Cena sprzedaży"
+msgstr "定价"
 
 msgctxt "field:product.list_price,template:"
 msgid "Template"
-msgstr "Szablon"
+msgstr "模板"
 
 msgctxt "field:product.product,categories:"
 msgid "Categories"
-msgstr "Kategorie"
+msgstr "类别"
 
 msgctxt "field:product.product,categories_all:"
 msgid "Categories"
-msgstr "Kategorie"
+msgstr "类别"
 
 msgctxt "field:product.product,code:"
 msgid "Code"
-msgstr "Kod"
+msgstr "代码"
 
 msgctxt "field:product.product,code_readonly:"
 msgid "Code Readonly"
-msgstr "Kod tylko do odczytu"
+msgstr "只读代码"
 
 msgctxt "field:product.product,consumable:"
 msgid "Consumable"
-msgstr "Artykuły konsumpcyjne"
+msgstr "消耗品"
 
 msgctxt "field:product.product,cost_price:"
 msgid "Cost Price"
-msgstr "Cena kosztów"
+msgstr "成本价"
 
 msgctxt "field:product.product,cost_price_method:"
 msgid "Cost Price Method"
-msgstr "Metoda wyceny zapasów"
+msgstr "成本价法"
 
 msgctxt "field:product.product,cost_price_methods:"
 msgid "Cost Price Methods"
-msgstr "Metody wyceny zapasów"
+msgstr "成本价法"
 
 msgctxt "field:product.product,cost_price_uom:"
 msgid "Cost Price"
-msgstr "Cena kosztów"
+msgstr "成本价"
 
 msgctxt "field:product.product,cost_prices:"
 msgid "Cost Prices"
-msgstr "Ceny kosztów"
+msgstr "成本价"
 
-#, fuzzy
 msgctxt "field:product.product,default_uom:"
 msgid "Default UoM"
-msgstr "Domyślna jm"
+msgstr "默认计量单位"
 
-#, fuzzy
 msgctxt "field:product.product,default_uom_category:"
 msgid "Default UoM Category"
-msgstr "Domyślna kategoria jm"
+msgstr "默认计量单位类别"
 
 msgctxt "field:product.product,description:"
 msgid "Description"
-msgstr "Opis"
+msgstr "描述"
 
 msgctxt "field:product.product,identifiers:"
 msgid "Identifiers"
-msgstr "Identyfikatory"
+msgstr "标识"
 
 msgctxt "field:product.product,list_price:"
 msgid "List Price"
-msgstr "Cena sprzedaży"
+msgstr "定价"
 
 msgctxt "field:product.product,list_price_uom:"
 msgid "List Price"
-msgstr "Cena sprzedaży"
+msgstr "定价"
 
 msgctxt "field:product.product,list_prices:"
 msgid "List Prices"
-msgstr "Ceny sprzedaży"
+msgstr "定价"
 
 msgctxt "field:product.product,name:"
 msgid "Name"
-msgstr "Nazwa"
+msgstr "名称"
 
 msgctxt "field:product.product,prefix_code:"
 msgid "Prefix Code"
-msgstr "Prefiks kodu"
+msgstr "前缀代码"
 
 msgctxt "field:product.product,suffix_code:"
 msgid "Suffix Code"
-msgstr "Sufiks kodu"
+msgstr "后缀代码"
 
 msgctxt "field:product.product,template:"
 msgid "Product Template"
-msgstr "Szablon produktu"
+msgstr "产品模板"
 
 msgctxt "field:product.product,type:"
 msgid "Type"
-msgstr "Typ"
+msgstr "类型"
 
 msgctxt "field:product.template,categories:"
 msgid "Categories"
-msgstr "Kategorie"
+msgstr "类别"
 
 msgctxt "field:product.template,categories_all:"
 msgid "Categories"
-msgstr "Kategorie"
+msgstr "类别"
 
 msgctxt "field:product.template,code:"
 msgid "Code"
-msgstr "Kod"
+msgstr "代码"
 
 msgctxt "field:product.template,code_readonly:"
 msgid "Code Readonly"
-msgstr "Kod tylko do odczytu"
+msgstr "代码（只读）"
 
 msgctxt "field:product.template,consumable:"
 msgid "Consumable"
-msgstr "Artykuły konsumpcyjne"
+msgstr "消耗品"
 
 msgctxt "field:product.template,cost_price:"
 msgid "Cost Price"
-msgstr "Cena kosztów"
+msgstr "成本价"
 
 msgctxt "field:product.template,cost_price_method:"
 msgid "Cost Price Method"
-msgstr "Metoda wyceny zapasów"
+msgstr "成本价法"
 
 msgctxt "field:product.template,cost_price_methods:"
 msgid "Cost Price Methods"
-msgstr "Metody wyceny zapasów"
+msgstr "成本价法"
 
-#, fuzzy
 msgctxt "field:product.template,default_uom:"
 msgid "Default UoM"
-msgstr "Domyślna jm"
+msgstr "默认计量单位"
 
-#, fuzzy
 msgctxt "field:product.template,default_uom_category:"
 msgid "Default UoM Category"
-msgstr "Domyślna kategoria jm"
+msgstr "默认计量单位类别"
 
 msgctxt "field:product.template,list_price:"
 msgid "List Price"
-msgstr "Cena sprzedaży"
+msgstr "定价"
 
 msgctxt "field:product.template,list_prices:"
 msgid "List Prices"
-msgstr "Ceny sprzedaży"
+msgstr "定价"
 
 msgctxt "field:product.template,name:"
 msgid "Name"
-msgstr "Nazwa"
+msgstr "名称"
 
 msgctxt "field:product.template,products:"
 msgid "Variants"
-msgstr "Warianty"
+msgstr "变体"
 
 msgctxt "field:product.template,type:"
 msgid "Type"
-msgstr "Typ"
+msgstr "类型"
 
 msgctxt "field:product.template-product.category,category:"
 msgid "Category"
-msgstr "Kategoria"
+msgstr "类别"
 
 msgctxt "field:product.template-product.category,template:"
 msgid "Template"
-msgstr "Szablon"
+msgstr "模板"
 
 msgctxt "field:product.template-product.category.all,category:"
 msgid "Category"
-msgstr "Kategoria"
+msgstr "类别"
 
 msgctxt "field:product.template-product.category.all,template:"
 msgid "Template"
-msgstr "Szablon"
+msgstr "模板"
 
 msgctxt "field:product.uom,category:"
 msgid "Category"
-msgstr "Kategoria"
+msgstr "类别"
 
 msgctxt "field:product.uom,digits:"
 msgid "Display Digits"
-msgstr "Cyfry wyświetlane"
+msgstr "显示数位"
 
 msgctxt "field:product.uom,factor:"
 msgid "Factor"
-msgstr "Współczynnik"
+msgstr "换算因子"
 
 msgctxt "field:product.uom,name:"
 msgid "Name"
-msgstr "Nazwa"
+msgstr "名称"
 
 msgctxt "field:product.uom,rate:"
 msgid "Rate"
-msgstr "Kurs"
+msgstr "换算率"
 
 msgctxt "field:product.uom,rounding:"
 msgid "Rounding Precision"
-msgstr "Dokładność"
+msgstr "舍入精度"
 
 msgctxt "field:product.uom,symbol:"
 msgid "Symbol"
-msgstr "Symbol"
+msgstr "符号"
 
 msgctxt "field:product.uom.category,name:"
 msgid "Name"
-msgstr "Nazwa"
+msgstr "名称"
 
 msgctxt "field:product.uom.category,uoms:"
 msgid "Units of Measure"
-msgstr "Jednostki miary"
+msgstr "计量单位"
 
 msgctxt "help:product.category,childs:"
 msgid "Used to add structure below the category."
-msgstr "Służy do dodawania struktury poniżej kategorii."
+msgstr "用于在类别下面添加结构."
 
 msgctxt "help:product.category,parent:"
 msgid "Used to add structure above the category."
-msgstr "Służy do dodawania struktury powyżej kategorii."
+msgstr "用于在类别上面添加结构."
+
+#, fuzzy
+msgctxt "help:product.configuration,category_sequence:"
+msgid "Used to generate the category code."
+msgstr "用于生成产品代码的最后一部分."
 
 msgctxt "help:product.configuration,default_cost_price_method:"
 msgid "The default cost price method for new products."
-msgstr "Domyślna metoda wyceny zapasów dla nowych produktów."
+msgstr "新产品默认使用的成本价格方法."
 
 msgctxt "help:product.configuration,product_sequence:"
 msgid "Used to generate the last part of the product code."
-msgstr "Służy do generowania końcowej części kodu produktu."
+msgstr "用于生成产品代码的最后一部分."
 
 msgctxt "help:product.configuration,template_sequence:"
 msgid "Used to generate the first part of the product code."
-msgstr "Służy do generowania początkowej części kodu produktu."
+msgstr "用于生成产品代码的第一部分."
 
 msgctxt ""
 "help:product.configuration.default_cost_price_method,default_cost_price_method:"
 msgid "The default cost price method for new products."
-msgstr "Domyślna metoda wyceny zapasów dla nowych produktów."
+msgstr "新产品默认使用的成本价格方法."
 
 msgctxt "help:product.identifier,product:"
 msgid "The product identified by the code."
-msgstr "Produkt identyfikowany kodem."
+msgstr "此代码标识的产品."
 
 msgctxt "help:product.product,categories:"
 msgid ""
 "The categories that the product is in.\n"
 "Used to group similar products together."
 msgstr ""
-"Kategorie, do których należy produkt.\n"
-"Służy do grupowania razem podobnych produktów."
+"产品所属类别.\n"
+"用于将类似的产品聚在一组."
 
 msgctxt "help:product.product,code:"
 msgid "A unique identifier for the variant."
-msgstr "Unikalny identyfikator wariantu."
+msgstr "变体的唯一标识符."
 
 msgctxt "help:product.product,consumable:"
 msgid "Check to allow stock moves to be assigned regardless of stock level."
-msgstr ""
-"Zaznacz, aby zezwolić na przenoszenie zapasów niezależnie od poziomu "
-"zapasów."
+msgstr "选中此项后，将允许不考虑库存水平的情况下，分配库存移动."
 
 msgctxt "help:product.product,cost_price:"
 msgid ""
 "The amount it costs to purchase or make the variant, or carry out the "
 "service."
-msgstr "Koszt zakupu, wykonania wariantu produktu lub wykonania usługi."
+msgstr "购买或制作产品变体或执行服务所需的费用."
 
 msgctxt "help:product.product,cost_price_method:"
 msgid "The method used to calculate the cost price."
-msgstr "Metoda użyta do obliczenia kosztu własnego."
+msgstr "用于计算成本价的方法."
 
-#, fuzzy
 msgctxt "help:product.product,default_uom:"
 msgid ""
 "The standard Unit of Measure for the product.\n"
 "Used internally when calculating the stock levels of goods and assets."
 msgstr ""
-"Standardowa jednostka miary dla produktu.\n"
-"Używane wewnętrznie przy obliczaniu stanów magazynowych towarów i aktywów."
+"产品的标准计量单位.\n"
+"在计算货物和资产的库存水平时内部使用."
 
-#, fuzzy
 msgctxt "help:product.product,default_uom_category:"
 msgid "The category of the default Unit of Measure."
-msgstr "Kategorie jednostek miary"
+msgstr "默认计量单位类别。"
 
 msgctxt "help:product.product,identifiers:"
 msgid "Other identifiers associated with the variant."
-msgstr "Inne identyfikatory powiązane z wariantem produktu."
+msgstr "其它标识符(产品变体相关)。"
 
 msgctxt "help:product.product,list_price:"
 msgid "The standard price the product is sold at."
-msgstr "Standardowa cena, za jaką sprzedawany jest produkt."
+msgstr "产品销售的标准价格."
 
 msgctxt "help:product.product,suffix_code:"
 msgid "The unique identifier for the product (aka SKU)."
-msgstr "Unikalny identyfikator produktu (znany również jako SKU)."
+msgstr "产品的唯一标识符（也称为SKU）."
 
 msgctxt "help:product.product,template:"
 msgid ""
 "The product that defines the common properties inherited by the variant."
-msgstr ""
-"Produkt, który definiuje typowe właściwości dziedziczone przez wariant "
-"produktu."
+msgstr "用来定义公共属性的产品，这些公共属性会被产品的变体继承."
 
 msgctxt "help:product.template,categories:"
 msgid ""
 "The categories that the product is in.\n"
 "Used to group similar products together."
 msgstr ""
-"Kategorie, do których należy produkt.\n"
-"Służy do grupowania razem podobnych produktów."
+"产品所属类别.\n"
+"用来将类似的产品分组."
 
 msgctxt "help:product.template,consumable:"
 msgid "Check to allow stock moves to be assigned regardless of stock level."
-msgstr ""
-"Zaznacz, aby zezwolić na przenoszenie zapasów niezależnie od poziomu "
-"zapasów."
+msgstr "选中此项后，将允许在不考虑库存水平的情况下，分配库存移动."
 
 msgctxt "help:product.template,cost_price:"
 msgid ""
 "The amount it costs to purchase or make the product, or carry out the "
 "service."
-msgstr "Koszt zakupu, wytworzenia produktu lub wykonania usługi."
+msgstr "购买或制造产品或提供服务所需的费用."
 
 msgctxt "help:product.template,cost_price_method:"
 msgid "The method used to calculate the cost price."
-msgstr "Metoda użyta do obliczenia kosztu własnego."
+msgstr "用于计算成本价的方法."
 
-#, fuzzy
 msgctxt "help:product.template,default_uom:"
 msgid ""
 "The standard Unit of Measure for the product.\n"
 "Used internally when calculating the stock levels of goods and assets."
 msgstr ""
-"Standardowa jednostka miary dla produktu.\n"
-"Używana przy obliczaniu stanów magazynowych towarów i aktywów."
+"产品标准计量单位.\n"
+"在计算货物和资产的库存水平时内部使用."
 
-#, fuzzy
 msgctxt "help:product.template,default_uom_category:"
 msgid "The category of the default Unit of Measure."
-msgstr "Kategorie jednostek miary"
+msgstr "默认计量单位类别。"
 
 msgctxt "help:product.template,list_price:"
 msgid "The standard price the product is sold at."
-msgstr "Standardowa cena, za jaką sprzedawany jest produkt."
+msgstr "产品销售的标准价格."
 
 msgctxt "help:product.template,products:"
 msgid "The different variants the product comes in."
-msgstr "Różne warianty produktu."
+msgstr "产品不同变体."
 
 msgctxt "help:product.uom,category:"
 msgid ""
 "The category that contains the unit of measure.\n"
 "Conversions between different units of measure can be done if they are in the same category."
 msgstr ""
-"Kategoria zawierająca jednostkę miary.\n"
-"Konwersje między różnymi jednostkami miary można dokonać, jeśli należą one do tej samej kategorii."
+"计量单位类别.\n"
+"属于同类别的计量单位之间可以相互转换."
 
 msgctxt "help:product.uom,digits:"
 msgid "The number of digits to display after the decimal separator."
-msgstr "Liczba cyfr po separatorze dziesiętnym."
+msgstr "小数点后显示的数字位数."
 
 msgctxt "help:product.uom,factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "coefficient (base unit) = 1 (this unit)"
 msgstr ""
-"Współczynnik dla wzoru:\n"
-"współczynnik (jednostka podstawowa) = 1 (ta jednostka)"
+"公式系数:\n"
+"系数 X 基本单位 = 1 X 当前单位"
 
 msgctxt "help:product.uom,rate:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (base unit) = coef (this unit)"
 msgstr ""
-"Współczynnik dla wzoru:\n"
-"1 (jednostka bazowa) = coef (ta jednostka)"
+"换算公式的系数：\n"
+"1 X 基本单位 = 系数 X 当前单位"
 
 msgctxt "help:product.uom,rounding:"
 msgid "The accuracy to which values are rounded."
-msgstr "Dokładność, z jaką wartości są zaokrąglane."
+msgstr "四舍五入精度."
 
 msgctxt "help:product.uom,symbol:"
 msgid "The symbol that represents the unit of measure."
-msgstr "Symbol reprezentujący jednostkę miary."
+msgstr "表示计量单位的符号."
 
 msgctxt "model:ir.action,name:act_category_list"
 msgid "Categories"
-msgstr "Kategorie"
+msgstr "类别"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_category_product"
 msgid "Add products"
-msgstr "Produkty"
+msgstr "添加产品"
 
 msgctxt "model:ir.action,name:act_category_tree"
 msgid "Categories"
-msgstr "Kategorie"
+msgstr "类别"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_product_configuration_form"
 msgid "Configuration"
-msgstr "Konfiguracja"
+msgstr "设置"
 
 msgctxt "model:ir.action,name:act_product_form"
 msgid "Variants"
-msgstr "Warianty"
+msgstr "变体"
 
 msgctxt "model:ir.action,name:act_product_from_template"
 msgid "Variants"
-msgstr "Warianty"
+msgstr "变体"
 
 msgctxt "model:ir.action,name:act_template_by_category"
 msgid "Product by Category"
-msgstr "Produkt wg kategorii"
+msgstr "按类别划分的产品"
 
 msgctxt "model:ir.action,name:act_template_form"
 msgid "Products"
-msgstr "Produkty"
+msgstr "产品"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_uom_category_form"
 msgid "Categories"
-msgstr "Kategorie"
+msgstr "类别"
 
 msgctxt "model:ir.action,name:act_uom_form"
 msgid "Units of Measure"
-msgstr "Jednostki miary"
+msgstr "计量单位"
+
+#, fuzzy
+msgctxt "model:ir.message,text:msg_category_code_unique"
+msgid "The code on product category must be unique."
+msgstr "已启用产品的代码不能重复."
 
 msgctxt "model:ir.message,text:msg_invalid_code"
 msgid "The %(type)s \"%(code)s\" for product \"%(product)s\" is not valid."
-msgstr "%(type) s \"% (code) s” dla produktu \"% (product) s” jest nieprawidłowy."
+msgstr "%(type)s \"%(code)s\" 对产品 \"%(product)s\" 是无效的."
 
 msgctxt "model:ir.message,text:msg_product_code_unique"
 msgid "Code of active product must be unique."
-msgstr "Kod aktywnego produktu musi być unikalny."
+msgstr "已启用产品的代码不能重复."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_uom_decrease_digits"
 msgid "You cannot decrease the digits of the unit of measure \"%(uom)s\"."
-msgstr "Nie można modyfikować stawki jednostki miary \"% (uom) s”."
+msgstr "不能减少计量单位 \"%(uom)s\" 的位数。"
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_uom_incompatible_factor_rate"
 msgid "Incompatible factor and rate values on unit of measure\"%(uom)s\"."
-msgstr ""
-"Niezgodne wartości współczynnika i stawki w jednostce miary „% (uom) s”."
+msgstr "与计量单位 \"%(uom)s\" 不兼容的换算因子和换算率."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_uom_modify_category"
 msgid "You cannot modify the category of the unit of measure \"%(uom)s\"."
-msgstr "Nie możesz modyfikować kategorii JM \"% (uom) s”."
+msgstr "不能改变计量单位 \"%(uom)s\" 的类别."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_uom_modify_factor"
 msgid "You cannot modify the factor of the unit of measure \"%(uom)s\"."
-msgstr "Nie możesz modyfikować kategorii JM \"% (uom) s”."
+msgstr "不能更改计量单位 \"%(uom)s\" 的换算因子."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_uom_modify_options"
 msgid ""
 "If the unit of measure is still not used, you can delete it otherwise you "
 "can deactivate it and create a new one."
-msgstr ""
-"Jeśli jednostka miary nadal nie jest używana, możesz ją usunąć, w przeciwnym"
-" razie możesz ją dezaktywować i utworzyć nową."
+msgstr "从未使用过的计量单位可以删除，否则只能停用后再新建。"
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_uom_modify_rate"
 msgid "You cannot modify the rate of the unit of measure\"%(uom)s\"."
-msgstr "Nie można modyfikować stawki jednostki miary \"% (uom) s”."
+msgstr "不能修改计量单位 \"%(uom)s\" 的换算率."
 
 msgctxt "model:ir.message,text:msg_uom_no_zero_factor_rate"
 msgid "Rate and factor can not be both equal to zero."
-msgstr "Stawka i współczynnik nie mogą być równe zeru."
+msgstr "换算率和换算因子不能同时为零."
 
-#, fuzzy
 msgctxt "model:ir.model.button,string:category_add_products_button"
 msgid "Add products"
-msgstr "Produkty"
+msgstr "添加产品"
+
+#, fuzzy
+msgctxt "model:ir.sequence.type,name:sequence_type_category"
+msgid "Category"
+msgstr "类别"
 
 msgctxt "model:ir.sequence.type,name:sequence_type_product"
 msgid "Variant"
-msgstr "Wariant"
+msgstr "变体"
 
 msgctxt "model:ir.sequence.type,name:sequence_type_template"
 msgid "Product"
-msgstr "Produkt"
+msgstr "产品"
 
 msgctxt "model:ir.ui.menu,name:menu_category_list"
 msgid "Categories"
-msgstr "Kategorie"
+msgstr "类别"
 
 msgctxt "model:ir.ui.menu,name:menu_category_tree"
 msgid "Categories"
-msgstr "Kategorie"
+msgstr "类别"
 
 msgctxt "model:ir.ui.menu,name:menu_configuration"
 msgid "Configuration"
-msgstr "Konfiguracja"
+msgstr "设置"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_main_product"
 msgid "Products"
-msgstr "Produkty"
+msgstr "产品"
 
 msgctxt "model:ir.ui.menu,name:menu_product"
 msgid "Variants"
-msgstr "Warianty"
+msgstr "变体"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_product_configuration"
 msgid "Configuration"
-msgstr "Konfiguracja"
+msgstr "设置"
 
 msgctxt "model:ir.ui.menu,name:menu_reporting"
 msgid "Reporting"
-msgstr ""
+msgstr "报告"
 
 msgctxt "model:ir.ui.menu,name:menu_template"
 msgid "Products"
-msgstr "Produkty"
+msgstr "产品设置"
 
 msgctxt "model:ir.ui.menu,name:menu_uom_category_form"
 msgid "Categories"
-msgstr "Kategorie"
+msgstr "类别"
 
 msgctxt "model:ir.ui.menu,name:menu_uom_form"
 msgid "Units of Measure"
-msgstr "Jednostki miary"
+msgstr "计量单位"
 
 msgctxt "model:product.category,name:"
 msgid "Product Category"
-msgstr "Produkt wg kategorii"
+msgstr "按类别划分的产品"
 
 msgctxt "model:product.configuration,name:"
 msgid "Product Configuration"
-msgstr "Konfiguracja produktu"
+msgstr "产品设置"
 
 msgctxt "model:product.configuration.default_cost_price_method,name:"
 msgid "Product Configuration Default Cost Price Method"
-msgstr "Konfiguracja domyślnej metody wyceny zapasów"
+msgstr "产品设置 - 默认的成本价法"
 
 msgctxt "model:product.cost_price,name:"
 msgid "Product Cost Price"
-msgstr "Cena kosztów produktu"
+msgstr "产品成本价"
 
 msgctxt "model:product.cost_price_method,name:"
 msgid "Product Cost Price Method"
-msgstr "Metoda wyceny zapasów produktów"
+msgstr "产品成本价法"
 
 msgctxt "model:product.identifier,name:"
 msgid "Product Identifier"
-msgstr "Identyfikator produktu"
+msgstr "产品标识"
 
 msgctxt "model:product.list_price,name:"
 msgid "Product List Price"
-msgstr "Cena sprzedaży produktu"
+msgstr "产品定价"
 
 msgctxt "model:product.product,name:"
 msgid "Product Variant"
-msgstr "Wariant produktu"
+msgstr "产品变体"
 
 msgctxt "model:product.template,name:"
 msgid "Product Template"
-msgstr "Szablon produktu"
+msgstr "产品模板"
 
 msgctxt "model:product.template-product.category,name:"
 msgid "Template - Category"
-msgstr "Szablon - Kategoria"
+msgstr "模板 - 类别"
 
 msgctxt "model:product.template-product.category.all,name:"
 msgid "Template - Category All"
-msgstr "Szablon - Wszystkie kategorie"
+msgstr "模板 -所有类别"
 
 msgctxt "model:product.uom,name:"
 msgid "Unit of Measure"
-msgstr "Jednostka miary"
+msgstr "计量单位"
 
 msgctxt "model:product.uom,name:uom_are"
 msgid "Are"
-msgstr "Ar"
+msgstr "公亩"
 
 msgctxt "model:product.uom,name:uom_carat"
 msgid "Carat"
-msgstr "Karat"
+msgstr "克拉"
 
-#, fuzzy
 msgctxt "model:product.uom,name:uom_centimeter"
 msgid "Centimeter"
-msgstr "centymetr"
+msgstr "厘米"
 
 msgctxt "model:product.uom,name:uom_cubic_centimeter"
 msgid "Cubic centimeter"
-msgstr "Centymetr sześcienny"
+msgstr "立方厘米"
 
 msgctxt "model:product.uom,name:uom_cubic_foot"
 msgid "Cubic foot"
-msgstr "Stopa sześcienna"
+msgstr "立方英尺"
 
 msgctxt "model:product.uom,name:uom_cubic_inch"
 msgid "Cubic inch"
-msgstr "Cal sześcienny"
+msgstr "立方英寸"
 
 msgctxt "model:product.uom,name:uom_cubic_meter"
 msgid "Cubic meter"
-msgstr "Metr sześcienny"
+msgstr "立方米"
 
 msgctxt "model:product.uom,name:uom_day"
 msgid "Day"
-msgstr "Dzień"
+msgstr "天"
 
 msgctxt "model:product.uom,name:uom_energy_joule"
 msgid "Joule"
-msgstr ""
+msgstr "焦耳"
 
 msgctxt "model:product.uom,name:uom_energy_kwh"
 msgid "Kilowatt-hour"
-msgstr ""
+msgstr "千瓦时"
 
 msgctxt "model:product.uom,name:uom_energy_megajoule"
 msgid "Megajoule"
-msgstr ""
+msgstr "兆焦耳"
 
 msgctxt "model:product.uom,name:uom_energy_mwh"
 msgid "Megawatt-hour"
-msgstr ""
+msgstr "兆瓦时"
 
 msgctxt "model:product.uom,name:uom_foot"
 msgid "Foot"
-msgstr "Stopa"
+msgstr "英尺"
 
 msgctxt "model:product.uom,name:uom_gallon"
 msgid "Gallon"
-msgstr "Galon"
+msgstr "加仑"
 
 msgctxt "model:product.uom,name:uom_gram"
 msgid "Gram"
-msgstr "Gram"
+msgstr "加仑"
 
 msgctxt "model:product.uom,name:uom_hectare"
 msgid "Hectare"
-msgstr "Hektar"
+msgstr "公顷"
 
 msgctxt "model:product.uom,name:uom_hour"
 msgid "Hour"
-msgstr "Godzina"
+msgstr "小时"
 
 msgctxt "model:product.uom,name:uom_inch"
 msgid "Inch"
-msgstr "Cal"
+msgstr "英寸"
 
 msgctxt "model:product.uom,name:uom_kilogram"
 msgid "Kilogram"
-msgstr "Kilogram"
+msgstr "千克"
 
 msgctxt "model:product.uom,name:uom_kilometer"
 msgid "Kilometer"
-msgstr "Kilometr"
+msgstr "千米"
 
 msgctxt "model:product.uom,name:uom_liter"
 msgid "Liter"
-msgstr "Litr"
+msgstr "公升"
 
 msgctxt "model:product.uom,name:uom_meter"
 msgid "Meter"
-msgstr "Metr"
+msgstr "米"
 
 msgctxt "model:product.uom,name:uom_mile"
 msgid "Mile"
-msgstr "Mila"
+msgstr "英里"
 
 msgctxt "model:product.uom,name:uom_millimeter"
 msgid "Millimeter"
-msgstr "Milimetr"
+msgstr "毫米"
 
 msgctxt "model:product.uom,name:uom_minute"
 msgid "Minute"
-msgstr "Minuta"
+msgstr "分钟"
 
 msgctxt "model:product.uom,name:uom_ounce"
 msgid "Ounce"
-msgstr "Uncja"
+msgstr "盎司"
 
 msgctxt "model:product.uom,name:uom_pound"
 msgid "Pound"
-msgstr "Funt"
+msgstr "英镑"
 
 msgctxt "model:product.uom,name:uom_second"
 msgid "Second"
-msgstr "Sekunda"
+msgstr "秒"
 
 msgctxt "model:product.uom,name:uom_square_centimeter"
 msgid "Square centimeter"
-msgstr "Centymetr kwadratowy"
+msgstr "平方厘米"
 
 msgctxt "model:product.uom,name:uom_square_foot"
 msgid "Square foot"
-msgstr "Stopa kwadratowa"
+msgstr "平方英尺"
 
 msgctxt "model:product.uom,name:uom_square_inch"
 msgid "Square inch"
-msgstr "Cal kwadratowy"
+msgstr "平方英寸"
 
 msgctxt "model:product.uom,name:uom_square_meter"
 msgid "Square meter"
-msgstr "Metr kwadratowy"
+msgstr "平方米"
 
 msgctxt "model:product.uom,name:uom_square_yard"
 msgid "Square yard"
-msgstr "Jard kwadratowy"
+msgstr "平方码"
 
 msgctxt "model:product.uom,name:uom_unit"
 msgid "Unit"
-msgstr "Jednostka"
+msgstr "单位"
 
 msgctxt "model:product.uom,name:uom_yard"
 msgid "Yard"
-msgstr "Jard"
+msgstr "码"
 
 msgctxt "model:product.uom,symbol:uom_are"
 msgid "a"
 msgstr "a"
 
 msgctxt "model:product.uom,symbol:uom_carat"
 msgid "c"
@@ -828,27 +827,27 @@
 
 msgctxt "model:product.uom,symbol:uom_day"
 msgid "d"
 msgstr "d"
 
 msgctxt "model:product.uom,symbol:uom_energy_joule"
 msgid "J"
-msgstr ""
+msgstr "J"
 
 msgctxt "model:product.uom,symbol:uom_energy_kwh"
 msgid "kW⋅h"
-msgstr ""
+msgstr "kW⋅h"
 
 msgctxt "model:product.uom,symbol:uom_energy_megajoule"
 msgid "MJ"
-msgstr ""
+msgstr "MJ"
 
 msgctxt "model:product.uom,symbol:uom_energy_mwh"
 msgid "MW⋅h"
-msgstr ""
+msgstr "MW⋅h"
 
 msgctxt "model:product.uom,symbol:uom_foot"
 msgid "ft"
 msgstr "ft"
 
 msgctxt "model:product.uom,symbol:uom_gallon"
 msgid "gal"
@@ -928,124 +927,132 @@
 
 msgctxt "model:product.uom,symbol:uom_square_yard"
 msgid "yd²"
 msgstr "yd²"
 
 msgctxt "model:product.uom,symbol:uom_unit"
 msgid "u"
-msgstr "szt."
+msgstr "u"
 
 msgctxt "model:product.uom,symbol:uom_yard"
 msgid "yd"
 msgstr "yd"
 
 msgctxt "model:product.uom.category,name:"
 msgid "Unit of Measure Category"
-msgstr "Kategoria jednostek miary"
+msgstr "计量单位类别"
 
 msgctxt "model:product.uom.category,name:uom_cat_energy"
 msgid "Energy"
-msgstr ""
+msgstr "能量"
 
 msgctxt "model:product.uom.category,name:uom_cat_length"
 msgid "Length"
-msgstr "Długość"
+msgstr "长度"
 
 msgctxt "model:product.uom.category,name:uom_cat_surface"
 msgid "Surface"
-msgstr "Powierzchnia"
+msgstr "面积"
 
 msgctxt "model:product.uom.category,name:uom_cat_time"
 msgid "Time"
-msgstr "Czas"
+msgstr "时间"
 
 msgctxt "model:product.uom.category,name:uom_cat_unit"
 msgid "Units"
-msgstr "Sztuki"
+msgstr "单位"
 
 msgctxt "model:product.uom.category,name:uom_cat_volume"
 msgid "Volume"
-msgstr "Objętość"
+msgstr "体积或容量"
 
 msgctxt "model:product.uom.category,name:uom_cat_weight"
 msgid "Weight"
-msgstr "Waga"
+msgstr "重量"
 
 msgctxt "model:res.group,name:group_product_admin"
 msgid "Product Administration"
-msgstr "Administracja ustawieniami produktu"
+msgstr "产品管理"
+
+msgctxt "selection:product.identifier,type:"
+msgid "Brand"
+msgstr ""
 
 msgctxt "selection:product.identifier,type:"
 msgid "International Article Number"
-msgstr "Międzynarodowy numer artykułu"
+msgstr "国际商品编码"
 
 msgctxt "selection:product.identifier,type:"
 msgid "International Securities Identification Number"
-msgstr "Międzynarodowy numer identyfikacyjny papierów wartościowych"
+msgstr "国际证券识别码"
 
 msgctxt "selection:product.identifier,type:"
 msgid "International Standard Audiovisual Number"
-msgstr "Międzynarodowy Standardowy Numer Audiowizualny"
+msgstr "国际标准音视频编号"
 
 msgctxt "selection:product.identifier,type:"
 msgid "International Standard Book Number"
-msgstr "Międzynarodowy standardowy numer książki"
+msgstr "国际标准书号"
 
 msgctxt "selection:product.identifier,type:"
 msgid "International Standard Identifier for Libraries"
-msgstr "Międzynarodowy identyfikator standardu dla bibliotek"
+msgstr "图书馆国际标准标识符"
 
 msgctxt "selection:product.identifier,type:"
 msgid "International Standard Music Number"
-msgstr "Międzynarodowy standardowy numer muzyczny"
+msgstr "国际标准乐谱号"
+
+msgctxt "selection:product.identifier,type:"
+msgid "Manufacturer Part Number"
+msgstr ""
 
 msgctxt "selection:product.product,cost_price_method:"
 msgid "Average"
-msgstr "Średnia"
+msgstr "平均成本价法"
 
 msgctxt "selection:product.product,cost_price_method:"
 msgid "Fixed"
-msgstr "Stała"
+msgstr "固定成本价法"
 
 msgctxt "selection:product.product,type:"
 msgid "Assets"
-msgstr "Majątek"
+msgstr "资产"
 
 msgctxt "selection:product.product,type:"
 msgid "Goods"
-msgstr "Towar"
+msgstr "货物"
 
 msgctxt "selection:product.product,type:"
 msgid "Service"
-msgstr "Usługa"
+msgstr "服务"
 
 msgctxt "selection:product.template,cost_price_method:"
 msgid "Average"
-msgstr "Średnia"
+msgstr "平均成本价法"
 
 msgctxt "selection:product.template,cost_price_method:"
 msgid "Fixed"
-msgstr "Stała"
+msgstr "固定成本价法"
 
 msgctxt "selection:product.template,type:"
 msgid "Assets"
-msgstr "Majątek"
+msgstr "资产"
 
 msgctxt "selection:product.template,type:"
 msgid "Goods"
-msgstr "Towar"
+msgstr "货物"
 
 msgctxt "selection:product.template,type:"
 msgid "Service"
-msgstr "Usługa"
+msgstr "服务"
 
 msgctxt "view:product.category:"
 msgid "Children"
-msgstr "Kategorie podrzędne"
+msgstr "子类别"
 
 msgctxt "view:product.configuration:"
 msgid "Sequences"
-msgstr "Sekwencje"
+msgstr "产品序列"
 
 msgctxt "view:product.template:"
 msgid "General"
-msgstr "Ogólne"
+msgstr "常规"
```

### Comparing `trytond_product-7.2.0/locale/pt.po` & `trytond_product-7.2.1/locale/pt.po`

 * *Files 1% similar despite different names*

```diff
@@ -7,27 +7,41 @@
 msgid "Product Price Decimal"
 msgstr "Preço de Custo do Produto"
 
 msgctxt "field:product.category,childs:"
 msgid "Children"
 msgstr "Filhos"
 
+#, fuzzy
+msgctxt "field:product.category,code:"
+msgid "Code"
+msgstr "Código"
+
+msgctxt "field:product.category,code_readonly:"
+msgid "Code Readonly"
+msgstr ""
+
 msgctxt "field:product.category,name:"
 msgid "Name"
 msgstr "Nome"
 
 msgctxt "field:product.category,parent:"
 msgid "Parent"
 msgstr "Pai"
 
 #, fuzzy
 msgctxt "field:product.category,templates:"
 msgid "Products"
 msgstr "Produtos"
 
+#, fuzzy
+msgctxt "field:product.configuration,category_sequence:"
+msgid "Category Sequence"
+msgstr "Modelo de produto"
+
 msgctxt "field:product.configuration,default_cost_price_method:"
 msgid "Default Cost Method"
 msgstr "Método de Custo Padrão"
 
 #, fuzzy
 msgctxt "field:product.configuration,product_sequence:"
 msgid "Variant Sequence"
@@ -304,14 +318,18 @@
 msgid "Used to add structure below the category."
 msgstr ""
 
 msgctxt "help:product.category,parent:"
 msgid "Used to add structure above the category."
 msgstr ""
 
+msgctxt "help:product.configuration,category_sequence:"
+msgid "Used to generate the category code."
+msgstr ""
+
 msgctxt "help:product.configuration,default_cost_price_method:"
 msgid "The default cost price method for new products."
 msgstr ""
 
 msgctxt "help:product.configuration,product_sequence:"
 msgid "Used to generate the last part of the product code."
 msgstr ""
@@ -494,14 +512,18 @@
 msgid "Categories"
 msgstr "Categorias"
 
 msgctxt "model:ir.action,name:act_uom_form"
 msgid "Units of Measure"
 msgstr "Unidades de Medida"
 
+msgctxt "model:ir.message,text:msg_category_code_unique"
+msgid "The code on product category must be unique."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_invalid_code"
 msgid "The %(type)s \"%(code)s\" for product \"%(product)s\" is not valid."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_product_code_unique"
 msgid "Code of active product must be unique."
 msgstr ""
@@ -538,14 +560,19 @@
 
 #, fuzzy
 msgctxt "model:ir.model.button,string:category_add_products_button"
 msgid "Add products"
 msgstr "Produtos"
 
 #, fuzzy
+msgctxt "model:ir.sequence.type,name:sequence_type_category"
+msgid "Category"
+msgstr "Categoria"
+
+#, fuzzy
 msgctxt "model:ir.sequence.type,name:sequence_type_product"
 msgid "Variant"
 msgstr "Variante"
 
 #, fuzzy
 msgctxt "model:ir.sequence.type,name:sequence_type_template"
 msgid "Product"
@@ -958,14 +985,18 @@
 msgstr "Peso"
 
 msgctxt "model:res.group,name:group_product_admin"
 msgid "Product Administration"
 msgstr "Administração de produtos"
 
 msgctxt "selection:product.identifier,type:"
+msgid "Brand"
+msgstr ""
+
+msgctxt "selection:product.identifier,type:"
 msgid "International Article Number"
 msgstr ""
 
 msgctxt "selection:product.identifier,type:"
 msgid "International Securities Identification Number"
 msgstr ""
 
@@ -981,14 +1012,18 @@
 msgid "International Standard Identifier for Libraries"
 msgstr ""
 
 msgctxt "selection:product.identifier,type:"
 msgid "International Standard Music Number"
 msgstr ""
 
+msgctxt "selection:product.identifier,type:"
+msgid "Manufacturer Part Number"
+msgstr ""
+
 msgctxt "selection:product.product,cost_price_method:"
 msgid "Average"
 msgstr "Média"
 
 msgctxt "selection:product.product,cost_price_method:"
 msgid "Fixed"
 msgstr "Fixo"
```

### Comparing `trytond_product-7.2.0/locale/ro.po` & `trytond_product-7.2.1/locale/ro.po`

 * *Files 2% similar despite different names*

```diff
@@ -6,26 +6,41 @@
 msgid "Product Price Decimal"
 msgstr "Zecimale Preț Produs"
 
 msgctxt "field:product.category,childs:"
 msgid "Children"
 msgstr "Copii"
 
+#, fuzzy
+msgctxt "field:product.category,code:"
+msgid "Code"
+msgstr "Cod"
+
+#, fuzzy
+msgctxt "field:product.category,code_readonly:"
+msgid "Code Readonly"
+msgstr "Cod numai pentru citit"
+
 msgctxt "field:product.category,name:"
 msgid "Name"
 msgstr "Denumire"
 
 msgctxt "field:product.category,parent:"
 msgid "Parent"
 msgstr "Părinte"
 
 msgctxt "field:product.category,templates:"
 msgid "Products"
 msgstr "Produse"
 
+#, fuzzy
+msgctxt "field:product.configuration,category_sequence:"
+msgid "Category Sequence"
+msgstr "Secvența produs"
+
 msgctxt "field:product.configuration,default_cost_price_method:"
 msgid "Default Cost Method"
 msgstr "Metoda cost implicit"
 
 msgctxt "field:product.configuration,product_sequence:"
 msgid "Variant Sequence"
 msgstr "Secvența produs"
@@ -291,14 +306,19 @@
 msgid "Used to add structure below the category."
 msgstr "Folosit pentru a adăuga structură sub categorie."
 
 msgctxt "help:product.category,parent:"
 msgid "Used to add structure above the category."
 msgstr "Folosit pentru a adăuga structură deasupra categoriei."
 
+#, fuzzy
+msgctxt "help:product.configuration,category_sequence:"
+msgid "Used to generate the category code."
+msgstr "Folosit pentru a genera codul produsului."
+
 msgctxt "help:product.configuration,default_cost_price_method:"
 msgid "The default cost price method for new products."
 msgstr "Metoda implicita pentru costul produselor noi."
 
 msgctxt "help:product.configuration,product_sequence:"
 msgid "Used to generate the last part of the product code."
 msgstr "Folosit pentru a genera codul produsului."
@@ -493,14 +513,19 @@
 msgid "Categories"
 msgstr "Categorii"
 
 msgctxt "model:ir.action,name:act_uom_form"
 msgid "Units of Measure"
 msgstr "Unități de Măsura"
 
+#, fuzzy
+msgctxt "model:ir.message,text:msg_category_code_unique"
+msgid "The code on product category must be unique."
+msgstr "Codul al unui produs activ trebuie să fie unic."
+
 msgctxt "model:ir.message,text:msg_invalid_code"
 msgid "The %(type)s \"%(code)s\" for product \"%(product)s\" is not valid."
 msgstr "%(type)s \"%(code)s\" nu este valabil pentru produsul \"%(product)s\"."
 
 msgctxt "model:ir.message,text:msg_product_code_unique"
 msgid "Code of active product must be unique."
 msgstr "Codul al unui produs activ trebuie să fie unic."
@@ -537,14 +562,19 @@
 msgid "Rate and factor can not be both equal to zero."
 msgstr "Rata şi factor nu pot ambele sa fii egale cu zero."
 
 msgctxt "model:ir.model.button,string:category_add_products_button"
 msgid "Add products"
 msgstr "Adăugare Produse"
 
+#, fuzzy
+msgctxt "model:ir.sequence.type,name:sequence_type_category"
+msgid "Category"
+msgstr "Categorie"
+
 msgctxt "model:ir.sequence.type,name:sequence_type_product"
 msgid "Variant"
 msgstr "Varianta"
 
 msgctxt "model:ir.sequence.type,name:sequence_type_template"
 msgid "Product"
 msgstr "Produs"
@@ -950,14 +980,18 @@
 msgstr "Greutate"
 
 msgctxt "model:res.group,name:group_product_admin"
 msgid "Product Administration"
 msgstr "Administrare Produs"
 
 msgctxt "selection:product.identifier,type:"
+msgid "Brand"
+msgstr ""
+
+msgctxt "selection:product.identifier,type:"
 msgid "International Article Number"
 msgstr "Cod International Articol"
 
 msgctxt "selection:product.identifier,type:"
 msgid "International Securities Identification Number"
 msgstr "Număr internațional de identificare a valorilor mobiliare"
 
@@ -973,14 +1007,18 @@
 msgid "International Standard Identifier for Libraries"
 msgstr "Identificator standard internațional pentru biblioteci"
 
 msgctxt "selection:product.identifier,type:"
 msgid "International Standard Music Number"
 msgstr "Numărul de muzică standard internațional"
 
+msgctxt "selection:product.identifier,type:"
+msgid "Manufacturer Part Number"
+msgstr ""
+
 msgctxt "selection:product.product,cost_price_method:"
 msgid "Average"
 msgstr "Mediu"
 
 msgctxt "selection:product.product,cost_price_method:"
 msgid "Fixed"
 msgstr "Fix"
```

### Comparing `trytond_product-7.2.0/locale/ru.po` & `trytond_product-7.2.1/locale/bg.po`

 * *Files 5% similar despite different names*

```diff
@@ -1,65 +1,79 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 #, fuzzy
 msgctxt "field:ir.configuration,product_price_decimal:"
 msgid "Product Price Decimal"
-msgstr "Вид продукта"
+msgstr "Продукт"
 
 msgctxt "field:product.category,childs:"
 msgid "Children"
-msgstr "Подчиненные"
+msgstr "Наследници"
+
+#, fuzzy
+msgctxt "field:product.category,code:"
+msgid "Code"
+msgstr "Код"
+
+msgctxt "field:product.category,code_readonly:"
+msgid "Code Readonly"
+msgstr ""
 
 msgctxt "field:product.category,name:"
 msgid "Name"
-msgstr "Наименование"
+msgstr "Име"
 
 msgctxt "field:product.category,parent:"
 msgid "Parent"
-msgstr "Предок"
+msgstr "Родител"
 
 #, fuzzy
 msgctxt "field:product.category,templates:"
 msgid "Products"
-msgstr "Products"
+msgstr "Продукти по местонахождения"
+
+#, fuzzy
+msgctxt "field:product.configuration,category_sequence:"
+msgid "Category Sequence"
+msgstr "Щаблон за продукт"
 
 msgctxt "field:product.configuration,default_cost_price_method:"
 msgid "Default Cost Method"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:product.configuration,product_sequence:"
 msgid "Variant Sequence"
-msgstr "Шаблон продукта"
+msgstr "Щаблон за продукт"
 
 #, fuzzy
 msgctxt "field:product.configuration,template_sequence:"
 msgid "Product Sequence"
-msgstr "Шаблон продукта"
+msgstr "Щаблон за продукт"
 
 msgctxt ""
 "field:product.configuration.default_cost_price_method,default_cost_price_method:"
 msgid "Default Cost Method"
 msgstr ""
 
 msgctxt "field:product.cost_price,company:"
 msgid "Company"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:product.cost_price,cost_price:"
 msgid "Cost Price"
-msgstr "Себестоимость"
+msgstr "Фабрична цена"
 
 #, fuzzy
 msgctxt "field:product.cost_price,product:"
 msgid "Product"
-msgstr "Продукция"
+msgstr "Продукт"
 
 msgctxt "field:product.cost_price_method,company:"
 msgid "Company"
 msgstr ""
 
 msgctxt "field:product.cost_price_method,cost_price_method:"
 msgid "Cost Price Method"
@@ -74,29 +88,29 @@
 msgctxt "field:product.identifier,code:"
 msgid "Code"
 msgstr "Код"
 
 #, fuzzy
 msgctxt "field:product.identifier,product:"
 msgid "Product"
-msgstr "Продукция"
+msgstr "Продукт"
 
 #, fuzzy
 msgctxt "field:product.identifier,type:"
 msgid "Type"
-msgstr "Тип"
+msgstr "Вид"
 
 msgctxt "field:product.list_price,company:"
 msgid "Company"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:product.list_price,list_price:"
 msgid "List Price"
-msgstr "Цена"
+msgstr "Каталожна цена"
 
 #, fuzzy
 msgctxt "field:product.list_price,template:"
 msgid "Template"
 msgstr "Шаблон"
 
 #, fuzzy
@@ -116,90 +130,93 @@
 msgctxt "field:product.product,code_readonly:"
 msgid "Code Readonly"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:product.product,consumable:"
 msgid "Consumable"
-msgstr "Потребляемый"
+msgstr "Консуматив"
 
 #, fuzzy
 msgctxt "field:product.product,cost_price:"
 msgid "Cost Price"
-msgstr "Себестоимость"
+msgstr "Фабрична цена"
 
 msgctxt "field:product.product,cost_price_method:"
 msgid "Cost Price Method"
 msgstr ""
 
 msgctxt "field:product.product,cost_price_methods:"
 msgid "Cost Price Methods"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:product.product,cost_price_uom:"
 msgid "Cost Price"
-msgstr "Себестоимость"
+msgstr "Фабрична цена"
 
 #, fuzzy
 msgctxt "field:product.product,cost_prices:"
 msgid "Cost Prices"
-msgstr "Себестоимость"
+msgstr "Фабрична цена"
 
 #, fuzzy
 msgctxt "field:product.product,default_uom:"
 msgid "Default UoM"
-msgstr "Ед.измерения по умолчанию"
+msgstr "Мер. ед. по подрабиране"
 
 #, fuzzy
 msgctxt "field:product.product,default_uom_category:"
 msgid "Default UoM Category"
-msgstr "Категория ед.измерения по умолчанию"
+msgstr "Категория мер. ед. по подразбиране"
 
 msgctxt "field:product.product,description:"
 msgid "Description"
 msgstr "Описание"
 
 msgctxt "field:product.product,identifiers:"
 msgid "Identifiers"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:product.product,list_price:"
 msgid "List Price"
-msgstr "Цена"
+msgstr "Каталожна цена"
 
+#, fuzzy
 msgctxt "field:product.product,list_price_uom:"
 msgid "List Price"
-msgstr "Цена"
+msgstr "Каталожна цена"
 
 #, fuzzy
 msgctxt "field:product.product,list_prices:"
 msgid "List Prices"
-msgstr "Цена"
+msgstr "Каталожна цена"
 
 #, fuzzy
 msgctxt "field:product.product,name:"
 msgid "Name"
-msgstr "Наименование"
+msgstr "Име"
 
 msgctxt "field:product.product,prefix_code:"
 msgid "Prefix Code"
 msgstr ""
 
 msgctxt "field:product.product,suffix_code:"
 msgid "Suffix Code"
 msgstr ""
 
 msgctxt "field:product.product,template:"
 msgid "Product Template"
-msgstr "Шаблон продукта"
+msgstr "Щаблон за продукт"
 
+#, fuzzy
 msgctxt "field:product.product,type:"
 msgid "Type"
-msgstr "Тип"
+msgstr "Вид"
 
 #, fuzzy
 msgctxt "field:product.template,categories:"
 msgid "Categories"
 msgstr "Категории"
 
 #, fuzzy
@@ -214,58 +231,59 @@
 
 msgctxt "field:product.template,code_readonly:"
 msgid "Code Readonly"
 msgstr ""
 
 msgctxt "field:product.template,consumable:"
 msgid "Consumable"
-msgstr "Потребляемый"
+msgstr "Консуматив"
 
 msgctxt "field:product.template,cost_price:"
 msgid "Cost Price"
-msgstr "Себестоимость"
+msgstr "Фабрична цена"
 
 msgctxt "field:product.template,cost_price_method:"
 msgid "Cost Price Method"
 msgstr ""
 
 msgctxt "field:product.template,cost_price_methods:"
 msgid "Cost Price Methods"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:product.template,default_uom:"
 msgid "Default UoM"
-msgstr "Ед.измерения по умолчанию"
+msgstr "Мер. ед. по подрабиране"
 
 #, fuzzy
 msgctxt "field:product.template,default_uom_category:"
 msgid "Default UoM Category"
-msgstr "Категория ед.измерения по умолчанию"
+msgstr "Категория мер. ед. по подразбиране"
 
 msgctxt "field:product.template,list_price:"
 msgid "List Price"
-msgstr "Цена"
+msgstr "Каталожна цена"
 
 #, fuzzy
 msgctxt "field:product.template,list_prices:"
 msgid "List Prices"
-msgstr "Цена"
+msgstr "Каталожна цена"
 
 msgctxt "field:product.template,name:"
 msgid "Name"
-msgstr "Наименование"
+msgstr "Име"
 
+#, fuzzy
 msgctxt "field:product.template,products:"
 msgid "Variants"
-msgstr "Разновидности"
+msgstr "Продукти"
 
 msgctxt "field:product.template,type:"
 msgid "Type"
-msgstr "Тип"
+msgstr "Вид"
 
 #, fuzzy
 msgctxt "field:product.template-product.category,category:"
 msgid "Category"
 msgstr "Категория"
 
 #, fuzzy
@@ -282,57 +300,61 @@
 msgctxt "field:product.template-product.category.all,template:"
 msgid "Template"
 msgstr "Шаблон"
 
 #, fuzzy
 msgctxt "field:product.uom,category:"
 msgid "Category"
-msgstr "Категория ед. измерения"
+msgstr "Категория мер. ед."
 
 msgctxt "field:product.uom,digits:"
 msgid "Display Digits"
-msgstr "Кол-во знаков после запятой"
+msgstr "Цифри за показване"
 
 msgctxt "field:product.uom,factor:"
 msgid "Factor"
-msgstr "Коэффициент к основной единице"
+msgstr "Коефициент"
 
 msgctxt "field:product.uom,name:"
 msgid "Name"
-msgstr "Наименование"
+msgstr "Име"
 
 msgctxt "field:product.uom,rate:"
 msgid "Rate"
-msgstr "Коэфициент основной единицы"
+msgstr "Отношение"
 
 msgctxt "field:product.uom,rounding:"
 msgid "Rounding Precision"
-msgstr "Точность округления"
+msgstr "Точност на закръгление"
 
 msgctxt "field:product.uom,symbol:"
 msgid "Symbol"
-msgstr "Условное обозначение"
+msgstr "Символ"
 
 msgctxt "field:product.uom.category,name:"
 msgid "Name"
-msgstr "Наименование"
+msgstr "Име"
 
 #, fuzzy
 msgctxt "field:product.uom.category,uoms:"
 msgid "Units of Measure"
 msgstr "Units of Measure"
 
 msgctxt "help:product.category,childs:"
 msgid "Used to add structure below the category."
 msgstr ""
 
 msgctxt "help:product.category,parent:"
 msgid "Used to add structure above the category."
 msgstr ""
 
+msgctxt "help:product.configuration,category_sequence:"
+msgid "Used to generate the category code."
+msgstr ""
+
 msgctxt "help:product.configuration,default_cost_price_method:"
 msgid "The default cost price method for new products."
 msgstr ""
 
 msgctxt "help:product.configuration,product_sequence:"
 msgid "Used to generate the last part of the product code."
 msgstr ""
@@ -379,15 +401,15 @@
 "The standard Unit of Measure for the product.\n"
 "Used internally when calculating the stock levels of goods and assets."
 msgstr ""
 
 #, fuzzy
 msgctxt "help:product.product,default_uom_category:"
 msgid "The category of the default Unit of Measure."
-msgstr "Категория ед.измерения"
+msgstr "Категория мерни единици"
 
 msgctxt "help:product.product,identifiers:"
 msgid "Other identifiers associated with the variant."
 msgstr ""
 
 msgctxt "help:product.product,list_price:"
 msgid "The standard price the product is sold at."
@@ -427,15 +449,15 @@
 "The standard Unit of Measure for the product.\n"
 "Used internally when calculating the stock levels of goods and assets."
 msgstr ""
 
 #, fuzzy
 msgctxt "help:product.template,default_uom_category:"
 msgid "The category of the default Unit of Measure."
-msgstr "Категория ед.измерения"
+msgstr "Категория мерни единици"
 
 msgctxt "help:product.template,list_price:"
 msgid "The standard price the product is sold at."
 msgstr ""
 
 msgctxt "help:product.template,products:"
 msgid "The different variants the product comes in."
@@ -453,24 +475,24 @@
 
 #, fuzzy
 msgctxt "help:product.uom,factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "coefficient (base unit) = 1 (this unit)"
 msgstr ""
-"Коэффициент по формуле:\n"
-"коэффициент в этом поле (базовая единица) = 1 (этой ед. измерения)"
+"Коефициент в тази формула:\n"
+"1 (баз. единица) = коеф. (тази единица)"
 
 msgctxt "help:product.uom,rate:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (base unit) = coef (this unit)"
 msgstr ""
-"Коэффициент по формуле:\n"
-"1 (базовая единица) = коэффициенту (этой ед.измерения)"
+"Коефициент в тази формула:\n"
+"1 (баз. единица) = коеф. (тази единица)"
 
 msgctxt "help:product.uom,rounding:"
 msgid "The accuracy to which values are rounded."
 msgstr ""
 
 msgctxt "help:product.uom,symbol:"
 msgid "The symbol that represents the unit of measure."
@@ -480,56 +502,60 @@
 msgctxt "model:ir.action,name:act_category_list"
 msgid "Categories"
 msgstr "Categories"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_category_product"
 msgid "Add products"
-msgstr "Products"
+msgstr "Продукти по местонахождения"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_category_tree"
 msgid "Categories"
 msgstr "Categories"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_product_configuration_form"
 msgid "Configuration"
-msgstr "Конфигурация"
+msgstr "Настройки"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_product_form"
 msgid "Variants"
-msgstr "Variants"
+msgstr "Продукти"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_product_from_template"
 msgid "Variants"
-msgstr "Разновидности"
+msgstr "Продукти"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_template_by_category"
 msgid "Product by Category"
-msgstr "Product by Category"
+msgstr "Категория на продукт"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_template_form"
 msgid "Products"
-msgstr "Products"
+msgstr "Продукти по местонахождения"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_uom_category_form"
 msgid "Categories"
 msgstr "Категории"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_uom_form"
 msgid "Units of Measure"
 msgstr "Units of Measure"
 
+msgctxt "model:ir.message,text:msg_category_code_unique"
+msgid "The code on product category must be unique."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_invalid_code"
 msgid "The %(type)s \"%(code)s\" for product \"%(product)s\" is not valid."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_product_code_unique"
 msgid "Code of active product must be unique."
 msgstr ""
@@ -563,78 +589,83 @@
 msgctxt "model:ir.message,text:msg_uom_no_zero_factor_rate"
 msgid "Rate and factor can not be both equal to zero."
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.model.button,string:category_add_products_button"
 msgid "Add products"
-msgstr "Products"
+msgstr "Продукти по местонахождения"
+
+#, fuzzy
+msgctxt "model:ir.sequence.type,name:sequence_type_category"
+msgid "Category"
+msgstr "Категория"
 
 #, fuzzy
 msgctxt "model:ir.sequence.type,name:sequence_type_product"
 msgid "Variant"
-msgstr "Разновидности"
+msgstr "Продукти"
 
 #, fuzzy
 msgctxt "model:ir.sequence.type,name:sequence_type_template"
 msgid "Product"
-msgstr "Продукция"
+msgstr "Продукт"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_category_list"
 msgid "Categories"
 msgstr "Categories"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_category_tree"
 msgid "Categories"
 msgstr "Categories"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_configuration"
 msgid "Configuration"
-msgstr "Конфигурация"
+msgstr "Настройки"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_main_product"
 msgid "Products"
-msgstr "Products"
+msgstr "Продукти по местонахождения"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_product"
 msgid "Variants"
-msgstr "Variants"
+msgstr "Продукти"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_product_configuration"
 msgid "Configuration"
-msgstr "Конфигурация"
+msgstr "Настройки"
 
 msgctxt "model:ir.ui.menu,name:menu_reporting"
 msgid "Reporting"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_template"
 msgid "Products"
-msgstr "Products"
+msgstr "Продукти по местонахождения"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_uom_category_form"
 msgid "Categories"
 msgstr "Categories"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_uom_form"
 msgid "Units of Measure"
 msgstr "Units of Measure"
 
 msgctxt "model:product.category,name:"
 msgid "Product Category"
-msgstr "Категория продукции"
+msgstr "Категория на продукт"
 
 #, fuzzy
 msgctxt "model:product.configuration,name:"
 msgid "Product Configuration"
 msgstr "Product Configuration"
 
 msgctxt "model:product.configuration.default_cost_price_method,name:"
@@ -648,40 +679,41 @@
 msgctxt "model:product.cost_price_method,name:"
 msgid "Product Cost Price Method"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:product.identifier,name:"
 msgid "Product Identifier"
-msgstr "Шаблон продукта"
+msgstr "Щаблон за продукт"
 
 msgctxt "model:product.list_price,name:"
 msgid "Product List Price"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:product.product,name:"
 msgid "Product Variant"
-msgstr "Вид продукта"
+msgstr "Продукт"
 
 msgctxt "model:product.template,name:"
 msgid "Product Template"
-msgstr "Шаблон продукта"
+msgstr "Щаблон за продукт"
 
 msgctxt "model:product.template-product.category,name:"
 msgid "Template - Category"
 msgstr ""
 
 msgctxt "model:product.template-product.category.all,name:"
 msgid "Template - Category All"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:product.uom,name:"
 msgid "Unit of Measure"
-msgstr "Единица измерения"
+msgstr "Мерни единици"
 
 #, fuzzy
 msgctxt "model:product.uom,name:uom_are"
 msgid "Are"
 msgstr "Are"
 
 #, fuzzy
@@ -846,50 +878,42 @@
 msgstr "Unit"
 
 #, fuzzy
 msgctxt "model:product.uom,name:uom_yard"
 msgid "Yard"
 msgstr "Yard"
 
-#, fuzzy
 msgctxt "model:product.uom,symbol:uom_are"
 msgid "a"
 msgstr "a"
 
-#, fuzzy
 msgctxt "model:product.uom,symbol:uom_carat"
 msgid "c"
 msgstr "c"
 
-#, fuzzy
 msgctxt "model:product.uom,symbol:uom_centimeter"
 msgid "cm"
 msgstr "cm"
 
-#, fuzzy
 msgctxt "model:product.uom,symbol:uom_cubic_centimeter"
 msgid "cm³"
 msgstr "cm³"
 
-#, fuzzy
 msgctxt "model:product.uom,symbol:uom_cubic_foot"
 msgid "ft³"
 msgstr "ft³"
 
-#, fuzzy
 msgctxt "model:product.uom,symbol:uom_cubic_inch"
 msgid "in³"
 msgstr "in³"
 
-#, fuzzy
 msgctxt "model:product.uom,symbol:uom_cubic_meter"
 msgid "m³"
 msgstr "m³"
 
-#, fuzzy
 msgctxt "model:product.uom,symbol:uom_day"
 msgid "d"
 msgstr "d"
 
 msgctxt "model:product.uom,symbol:uom_energy_joule"
 msgid "J"
 msgstr ""
@@ -902,133 +926,111 @@
 msgid "MJ"
 msgstr ""
 
 msgctxt "model:product.uom,symbol:uom_energy_mwh"
 msgid "MW⋅h"
 msgstr ""
 
-#, fuzzy
 msgctxt "model:product.uom,symbol:uom_foot"
 msgid "ft"
 msgstr "ft"
 
-#, fuzzy
 msgctxt "model:product.uom,symbol:uom_gallon"
 msgid "gal"
 msgstr "gal"
 
-#, fuzzy
 msgctxt "model:product.uom,symbol:uom_gram"
 msgid "g"
 msgstr "g"
 
-#, fuzzy
 msgctxt "model:product.uom,symbol:uom_hectare"
 msgid "ha"
 msgstr "ha"
 
-#, fuzzy
 msgctxt "model:product.uom,symbol:uom_hour"
 msgid "h"
 msgstr "h"
 
-#, fuzzy
 msgctxt "model:product.uom,symbol:uom_inch"
 msgid "in"
 msgstr "in"
 
-#, fuzzy
 msgctxt "model:product.uom,symbol:uom_kilogram"
 msgid "kg"
 msgstr "kg"
 
-#, fuzzy
 msgctxt "model:product.uom,symbol:uom_kilometer"
 msgid "km"
 msgstr "km"
 
-#, fuzzy
 msgctxt "model:product.uom,symbol:uom_liter"
 msgid "l"
 msgstr "l"
 
-#, fuzzy
 msgctxt "model:product.uom,symbol:uom_meter"
 msgid "m"
 msgstr "m"
 
-#, fuzzy
 msgctxt "model:product.uom,symbol:uom_mile"
 msgid "mi"
 msgstr "mi"
 
-#, fuzzy
 msgctxt "model:product.uom,symbol:uom_millimeter"
 msgid "mm"
 msgstr "mm"
 
-#, fuzzy
 msgctxt "model:product.uom,symbol:uom_minute"
 msgid "min"
 msgstr "min"
 
-#, fuzzy
 msgctxt "model:product.uom,symbol:uom_ounce"
 msgid "oz"
 msgstr "oz"
 
 #, fuzzy
 msgctxt "model:product.uom,symbol:uom_pound"
 msgid "lb"
-msgstr "фунт"
+msgstr "lbs"
 
-#, fuzzy
 msgctxt "model:product.uom,symbol:uom_second"
 msgid "s"
 msgstr "s"
 
-#, fuzzy
 msgctxt "model:product.uom,symbol:uom_square_centimeter"
 msgid "cm²"
 msgstr "cm²"
 
-#, fuzzy
 msgctxt "model:product.uom,symbol:uom_square_foot"
 msgid "ft²"
 msgstr "ft²"
 
-#, fuzzy
 msgctxt "model:product.uom,symbol:uom_square_inch"
 msgid "in²"
 msgstr "in²"
 
-#, fuzzy
 msgctxt "model:product.uom,symbol:uom_square_meter"
 msgid "m²"
 msgstr "m²"
 
-#, fuzzy
 msgctxt "model:product.uom,symbol:uom_square_yard"
 msgid "yd²"
 msgstr "yd²"
 
-#, fuzzy
 msgctxt "model:product.uom,symbol:uom_unit"
 msgid "u"
 msgstr "u"
 
-#, fuzzy
 msgctxt "model:product.uom,symbol:uom_yard"
 msgid "yd"
 msgstr "yd"
 
 #, fuzzy
 msgctxt "model:product.uom.category,name:"
 msgid "Unit of Measure Category"
-msgstr "Единица измерения"
+msgstr "Мерни единици"
 
 msgctxt "model:product.uom.category,name:uom_cat_energy"
 msgid "Energy"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:product.uom.category,name:uom_cat_length"
@@ -1062,14 +1064,18 @@
 
 #, fuzzy
 msgctxt "model:res.group,name:group_product_admin"
 msgid "Product Administration"
 msgstr "Product Administration"
 
 msgctxt "selection:product.identifier,type:"
+msgid "Brand"
+msgstr ""
+
+msgctxt "selection:product.identifier,type:"
 msgid "International Article Number"
 msgstr ""
 
 msgctxt "selection:product.identifier,type:"
 msgid "International Securities Identification Number"
 msgstr ""
 
@@ -1085,61 +1091,68 @@
 msgid "International Standard Identifier for Libraries"
 msgstr ""
 
 msgctxt "selection:product.identifier,type:"
 msgid "International Standard Music Number"
 msgstr ""
 
+msgctxt "selection:product.identifier,type:"
+msgid "Manufacturer Part Number"
+msgstr ""
+
 #, fuzzy
 msgctxt "selection:product.product,cost_price_method:"
 msgid "Average"
-msgstr "Средняя цена"
+msgstr "Средна"
 
 #, fuzzy
 msgctxt "selection:product.product,cost_price_method:"
 msgid "Fixed"
-msgstr "Фиксированная цена"
+msgstr "Фиксирана"
 
+#, fuzzy
 msgctxt "selection:product.product,type:"
 msgid "Assets"
-msgstr "Активы"
+msgstr "Активи"
 
+#, fuzzy
 msgctxt "selection:product.product,type:"
 msgid "Goods"
-msgstr "Товары"
+msgstr "Стока"
 
+#, fuzzy
 msgctxt "selection:product.product,type:"
 msgid "Service"
-msgstr "Услуги"
+msgstr "Услуга"
 
 msgctxt "selection:product.template,cost_price_method:"
 msgid "Average"
-msgstr "Средняя цена"
+msgstr "Средна"
 
 msgctxt "selection:product.template,cost_price_method:"
 msgid "Fixed"
-msgstr "Фиксированная цена"
+msgstr "Фиксирана"
 
 msgctxt "selection:product.template,type:"
 msgid "Assets"
-msgstr "Активы"
+msgstr "Активи"
 
 msgctxt "selection:product.template,type:"
 msgid "Goods"
-msgstr "Товары"
+msgstr "Стока"
 
 msgctxt "selection:product.template,type:"
 msgid "Service"
-msgstr "Услуги"
+msgstr "Услуга"
 
 msgctxt "view:product.category:"
 msgid "Children"
-msgstr "Подчиненные"
+msgstr "Наследници"
 
 #, fuzzy
 msgctxt "view:product.configuration:"
 msgid "Sequences"
-msgstr "Шаблон продукта"
+msgstr "Щаблон за продукт"
 
 msgctxt "view:product.template:"
 msgid "General"
-msgstr "Основные"
+msgstr "Основен"
```

### Comparing `trytond_product-7.2.0/locale/sl.po` & `trytond_product-7.2.1/locale/sl.po`

 * *Files 1% similar despite different names*

```diff
@@ -7,27 +7,41 @@
 msgid "Product Price Decimal"
 msgstr "Nabavna cena izdelka"
 
 msgctxt "field:product.category,childs:"
 msgid "Children"
 msgstr "Podkategorije"
 
+#, fuzzy
+msgctxt "field:product.category,code:"
+msgid "Code"
+msgstr "Šifra"
+
+msgctxt "field:product.category,code_readonly:"
+msgid "Code Readonly"
+msgstr ""
+
 msgctxt "field:product.category,name:"
 msgid "Name"
 msgstr "Naziv"
 
 msgctxt "field:product.category,parent:"
 msgid "Parent"
 msgstr "Matična kategorija"
 
 #, fuzzy
 msgctxt "field:product.category,templates:"
 msgid "Products"
 msgstr "Products"
 
+#, fuzzy
+msgctxt "field:product.configuration,category_sequence:"
+msgid "Category Sequence"
+msgstr "Številčna serija različice"
+
 msgctxt "field:product.configuration,default_cost_price_method:"
 msgid "Default Cost Method"
 msgstr "Privzeti obračun"
 
 msgctxt "field:product.configuration,product_sequence:"
 msgid "Variant Sequence"
 msgstr "Številčna serija različice"
@@ -310,14 +324,18 @@
 msgid "Used to add structure below the category."
 msgstr ""
 
 msgctxt "help:product.category,parent:"
 msgid "Used to add structure above the category."
 msgstr ""
 
+msgctxt "help:product.configuration,category_sequence:"
+msgid "Used to generate the category code."
+msgstr ""
+
 msgctxt "help:product.configuration,default_cost_price_method:"
 msgid "The default cost price method for new products."
 msgstr ""
 
 msgctxt "help:product.configuration,product_sequence:"
 msgid "Used to generate the last part of the product code."
 msgstr ""
@@ -504,14 +522,18 @@
 msgstr "Kategorije"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_uom_form"
 msgid "Units of Measure"
 msgstr "Units of Measure"
 
+msgctxt "model:ir.message,text:msg_category_code_unique"
+msgid "The code on product category must be unique."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_invalid_code"
 msgid "The %(type)s \"%(code)s\" for product \"%(product)s\" is not valid."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_product_code_unique"
 msgid "Code of active product must be unique."
 msgstr ""
@@ -548,14 +570,19 @@
 
 #, fuzzy
 msgctxt "model:ir.model.button,string:category_add_products_button"
 msgid "Add products"
 msgstr "Products"
 
 #, fuzzy
+msgctxt "model:ir.sequence.type,name:sequence_type_category"
+msgid "Category"
+msgstr "Kategorija"
+
+#, fuzzy
 msgctxt "model:ir.sequence.type,name:sequence_type_product"
 msgid "Variant"
 msgstr "Različice"
 
 #, fuzzy
 msgctxt "model:ir.sequence.type,name:sequence_type_template"
 msgid "Product"
@@ -994,14 +1021,18 @@
 
 #, fuzzy
 msgctxt "model:res.group,name:group_product_admin"
 msgid "Product Administration"
 msgstr "Product Administration"
 
 msgctxt "selection:product.identifier,type:"
+msgid "Brand"
+msgstr ""
+
+msgctxt "selection:product.identifier,type:"
 msgid "International Article Number"
 msgstr ""
 
 msgctxt "selection:product.identifier,type:"
 msgid "International Securities Identification Number"
 msgstr ""
 
@@ -1017,14 +1048,18 @@
 msgid "International Standard Identifier for Libraries"
 msgstr ""
 
 msgctxt "selection:product.identifier,type:"
 msgid "International Standard Music Number"
 msgstr ""
 
+msgctxt "selection:product.identifier,type:"
+msgid "Manufacturer Part Number"
+msgstr ""
+
 msgctxt "selection:product.product,cost_price_method:"
 msgid "Average"
 msgstr "Povprečna cena"
 
 msgctxt "selection:product.product,cost_price_method:"
 msgid "Fixed"
 msgstr "Fiksna"
```

### Comparing `trytond_product-7.2.0/locale/tr.po` & `trytond_product-7.2.1/locale/tr.po`

 * *Files 1% similar despite different names*

```diff
@@ -7,27 +7,41 @@
 msgid "Product Price Decimal"
 msgstr "Ürün Maliyet Fiyatı"
 
 msgctxt "field:product.category,childs:"
 msgid "Children"
 msgstr "Alt Öğe"
 
+#, fuzzy
+msgctxt "field:product.category,code:"
+msgid "Code"
+msgstr "Kod"
+
+msgctxt "field:product.category,code_readonly:"
+msgid "Code Readonly"
+msgstr ""
+
 msgctxt "field:product.category,name:"
 msgid "Name"
 msgstr "Ad"
 
 msgctxt "field:product.category,parent:"
 msgid "Parent"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:product.category,templates:"
 msgid "Products"
 msgstr "Products"
 
+#, fuzzy
+msgctxt "field:product.configuration,category_sequence:"
+msgid "Category Sequence"
+msgstr "Ürün Şablonu"
+
 msgctxt "field:product.configuration,default_cost_price_method:"
 msgid "Default Cost Method"
 msgstr "Varsayılan Maliyet Metodu"
 
 #, fuzzy
 msgctxt "field:product.configuration,product_sequence:"
 msgid "Variant Sequence"
@@ -304,14 +318,18 @@
 msgid "Used to add structure below the category."
 msgstr ""
 
 msgctxt "help:product.category,parent:"
 msgid "Used to add structure above the category."
 msgstr ""
 
+msgctxt "help:product.configuration,category_sequence:"
+msgid "Used to generate the category code."
+msgstr ""
+
 msgctxt "help:product.configuration,default_cost_price_method:"
 msgid "The default cost price method for new products."
 msgstr ""
 
 msgctxt "help:product.configuration,product_sequence:"
 msgid "Used to generate the last part of the product code."
 msgstr ""
@@ -496,14 +514,18 @@
 msgstr "Kategoriler"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_uom_form"
 msgid "Units of Measure"
 msgstr "Ölçü birimi"
 
+msgctxt "model:ir.message,text:msg_category_code_unique"
+msgid "The code on product category must be unique."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_invalid_code"
 msgid "The %(type)s \"%(code)s\" for product \"%(product)s\" is not valid."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_product_code_unique"
 msgid "Code of active product must be unique."
 msgstr ""
@@ -540,14 +562,19 @@
 
 #, fuzzy
 msgctxt "model:ir.model.button,string:category_add_products_button"
 msgid "Add products"
 msgstr "Products"
 
 #, fuzzy
+msgctxt "model:ir.sequence.type,name:sequence_type_category"
+msgid "Category"
+msgstr "Kategori"
+
+#, fuzzy
 msgctxt "model:ir.sequence.type,name:sequence_type_product"
 msgid "Variant"
 msgstr "Varyantlar"
 
 #, fuzzy
 msgctxt "model:ir.sequence.type,name:sequence_type_template"
 msgid "Product"
@@ -1005,14 +1032,18 @@
 
 #, fuzzy
 msgctxt "model:res.group,name:group_product_admin"
 msgid "Product Administration"
 msgstr "Product Administration"
 
 msgctxt "selection:product.identifier,type:"
+msgid "Brand"
+msgstr ""
+
+msgctxt "selection:product.identifier,type:"
 msgid "International Article Number"
 msgstr ""
 
 msgctxt "selection:product.identifier,type:"
 msgid "International Securities Identification Number"
 msgstr ""
 
@@ -1028,14 +1059,18 @@
 msgid "International Standard Identifier for Libraries"
 msgstr ""
 
 msgctxt "selection:product.identifier,type:"
 msgid "International Standard Music Number"
 msgstr ""
 
+msgctxt "selection:product.identifier,type:"
+msgid "Manufacturer Part Number"
+msgstr ""
+
 msgctxt "selection:product.product,cost_price_method:"
 msgid "Average"
 msgstr "Ortalama"
 
 msgctxt "selection:product.product,cost_price_method:"
 msgid "Fixed"
 msgstr "Sabitlenmiş"
```

### Comparing `trytond_product-7.2.0/locale/uk.po` & `trytond_product-7.2.1/locale/uk.po`

 * *Files 1% similar despite different names*

```diff
@@ -6,26 +6,38 @@
 msgid "Product Price Decimal"
 msgstr ""
 
 msgctxt "field:product.category,childs:"
 msgid "Children"
 msgstr ""
 
+msgctxt "field:product.category,code:"
+msgid "Code"
+msgstr ""
+
+msgctxt "field:product.category,code_readonly:"
+msgid "Code Readonly"
+msgstr ""
+
 msgctxt "field:product.category,name:"
 msgid "Name"
 msgstr ""
 
 msgctxt "field:product.category,parent:"
 msgid "Parent"
 msgstr ""
 
 msgctxt "field:product.category,templates:"
 msgid "Products"
 msgstr ""
 
+msgctxt "field:product.configuration,category_sequence:"
+msgid "Category Sequence"
+msgstr ""
+
 msgctxt "field:product.configuration,default_cost_price_method:"
 msgid "Default Cost Method"
 msgstr ""
 
 msgctxt "field:product.configuration,product_sequence:"
 msgid "Variant Sequence"
 msgstr ""
@@ -291,14 +303,18 @@
 msgid "Used to add structure below the category."
 msgstr ""
 
 msgctxt "help:product.category,parent:"
 msgid "Used to add structure above the category."
 msgstr ""
 
+msgctxt "help:product.configuration,category_sequence:"
+msgid "Used to generate the category code."
+msgstr ""
+
 msgctxt "help:product.configuration,default_cost_price_method:"
 msgid "The default cost price method for new products."
 msgstr ""
 
 msgctxt "help:product.configuration,product_sequence:"
 msgid "Used to generate the last part of the product code."
 msgstr ""
@@ -471,14 +487,18 @@
 msgid "Categories"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_uom_form"
 msgid "Units of Measure"
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_category_code_unique"
+msgid "The code on product category must be unique."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_invalid_code"
 msgid "The %(type)s \"%(code)s\" for product \"%(product)s\" is not valid."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_product_code_unique"
 msgid "Code of active product must be unique."
 msgstr ""
@@ -513,14 +533,19 @@
 msgid "Rate and factor can not be both equal to zero."
 msgstr ""
 
 msgctxt "model:ir.model.button,string:category_add_products_button"
 msgid "Add products"
 msgstr ""
 
+#, fuzzy
+msgctxt "model:ir.sequence.type,name:sequence_type_category"
+msgid "Category"
+msgstr "Категорії"
+
 msgctxt "model:ir.sequence.type,name:sequence_type_product"
 msgid "Variant"
 msgstr ""
 
 msgctxt "model:ir.sequence.type,name:sequence_type_template"
 msgid "Product"
 msgstr ""
@@ -926,14 +951,18 @@
 msgstr ""
 
 msgctxt "model:res.group,name:group_product_admin"
 msgid "Product Administration"
 msgstr ""
 
 msgctxt "selection:product.identifier,type:"
+msgid "Brand"
+msgstr ""
+
+msgctxt "selection:product.identifier,type:"
 msgid "International Article Number"
 msgstr ""
 
 msgctxt "selection:product.identifier,type:"
 msgid "International Securities Identification Number"
 msgstr ""
 
@@ -949,14 +978,18 @@
 msgid "International Standard Identifier for Libraries"
 msgstr ""
 
 msgctxt "selection:product.identifier,type:"
 msgid "International Standard Music Number"
 msgstr ""
 
+msgctxt "selection:product.identifier,type:"
+msgid "Manufacturer Part Number"
+msgstr ""
+
 msgctxt "selection:product.product,cost_price_method:"
 msgid "Average"
 msgstr ""
 
 msgctxt "selection:product.product,cost_price_method:"
 msgid "Fixed"
 msgstr ""
```

### Comparing `trytond_product-7.2.0/locale/zh_CN.po` & `trytond_product-7.2.1/locale/pl.po`

 * *Files 8% similar despite different names*

```diff
@@ -1,775 +1,807 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:ir.configuration,product_price_decimal:"
 msgid "Product Price Decimal"
-msgstr "产品价格小数"
+msgstr "Cena produktu po przecinku"
 
 msgctxt "field:product.category,childs:"
 msgid "Children"
-msgstr "子类别"
+msgstr "Kategorie podrzędne"
+
+msgctxt "field:product.category,code:"
+msgid "Code"
+msgstr "Kod"
+
+msgctxt "field:product.category,code_readonly:"
+msgid "Code Readonly"
+msgstr "Kod tylko do odczytu"
 
 msgctxt "field:product.category,name:"
 msgid "Name"
-msgstr "名称"
+msgstr "Nazwa"
 
 msgctxt "field:product.category,parent:"
 msgid "Parent"
-msgstr "父类别"
+msgstr "Kategoria nadrzędna"
 
 msgctxt "field:product.category,templates:"
 msgid "Products"
-msgstr "产品"
+msgstr "Produkty"
+
+msgctxt "field:product.configuration,category_sequence:"
+msgid "Category Sequence"
+msgstr "Sekwencja kategorii"
 
 msgctxt "field:product.configuration,default_cost_price_method:"
 msgid "Default Cost Method"
-msgstr "默认成本法"
+msgstr "Domyślna metoda kosztowa"
 
 msgctxt "field:product.configuration,product_sequence:"
 msgid "Variant Sequence"
-msgstr "产品变体序列"
+msgstr "Sekwencja wariantu produktu"
 
 msgctxt "field:product.configuration,template_sequence:"
 msgid "Product Sequence"
-msgstr "产品序列"
+msgstr "Sekwencja produktu"
 
 msgctxt ""
 "field:product.configuration.default_cost_price_method,default_cost_price_method:"
 msgid "Default Cost Method"
-msgstr "默认成本法"
+msgstr "Domyślna metoda kosztowa"
 
 msgctxt "field:product.cost_price,company:"
 msgid "Company"
-msgstr "公司"
+msgstr "Firma"
 
 msgctxt "field:product.cost_price,cost_price:"
 msgid "Cost Price"
-msgstr "成本价"
+msgstr "Cena kosztów"
 
 msgctxt "field:product.cost_price,product:"
 msgid "Product"
-msgstr "产品"
+msgstr "Produkt"
 
 msgctxt "field:product.cost_price_method,company:"
 msgid "Company"
-msgstr "公司"
+msgstr "Firma"
 
 msgctxt "field:product.cost_price_method,cost_price_method:"
 msgid "Cost Price Method"
-msgstr "成本价法"
+msgstr "Metoda wyceny zapasów"
 
 msgctxt "field:product.cost_price_method,template:"
 msgid "Template"
-msgstr "模板"
+msgstr "Szablon"
 
 msgctxt "field:product.identifier,code:"
 msgid "Code"
-msgstr "代码"
+msgstr "Kod"
 
 msgctxt "field:product.identifier,product:"
 msgid "Product"
-msgstr "产品"
+msgstr "Produkt"
 
 msgctxt "field:product.identifier,type:"
 msgid "Type"
-msgstr "类型"
+msgstr "Typ"
 
 msgctxt "field:product.list_price,company:"
 msgid "Company"
-msgstr "公司"
+msgstr "Firma"
 
 msgctxt "field:product.list_price,list_price:"
 msgid "List Price"
-msgstr "定价"
+msgstr "Cena sprzedaży"
 
 msgctxt "field:product.list_price,template:"
 msgid "Template"
-msgstr "模板"
+msgstr "Szablon"
 
 msgctxt "field:product.product,categories:"
 msgid "Categories"
-msgstr "类别"
+msgstr "Kategorie"
 
 msgctxt "field:product.product,categories_all:"
 msgid "Categories"
-msgstr "类别"
+msgstr "Kategorie"
 
 msgctxt "field:product.product,code:"
 msgid "Code"
-msgstr "代码"
+msgstr "Kod"
 
 msgctxt "field:product.product,code_readonly:"
 msgid "Code Readonly"
-msgstr "只读代码"
+msgstr "Kod tylko do odczytu"
 
 msgctxt "field:product.product,consumable:"
 msgid "Consumable"
-msgstr "消耗品"
+msgstr "Artykuły konsumpcyjne"
 
 msgctxt "field:product.product,cost_price:"
 msgid "Cost Price"
-msgstr "成本价"
+msgstr "Cena kosztów"
 
 msgctxt "field:product.product,cost_price_method:"
 msgid "Cost Price Method"
-msgstr "成本价法"
+msgstr "Metoda wyceny zapasów"
 
 msgctxt "field:product.product,cost_price_methods:"
 msgid "Cost Price Methods"
-msgstr "成本价法"
+msgstr "Metody wyceny zapasów"
 
 msgctxt "field:product.product,cost_price_uom:"
 msgid "Cost Price"
-msgstr "成本价"
+msgstr "Cena kosztów"
 
 msgctxt "field:product.product,cost_prices:"
 msgid "Cost Prices"
-msgstr "成本价"
+msgstr "Ceny kosztów"
 
 msgctxt "field:product.product,default_uom:"
 msgid "Default UoM"
-msgstr "默认计量单位"
+msgstr "Domyślna jednostka miary"
 
 msgctxt "field:product.product,default_uom_category:"
 msgid "Default UoM Category"
-msgstr "默认计量单位类别"
+msgstr "Domyślna kategoria jednostki miary"
 
 msgctxt "field:product.product,description:"
 msgid "Description"
-msgstr "描述"
+msgstr "Opis"
 
 msgctxt "field:product.product,identifiers:"
 msgid "Identifiers"
-msgstr "标识"
+msgstr "Identyfikatory"
 
 msgctxt "field:product.product,list_price:"
 msgid "List Price"
-msgstr "定价"
+msgstr "Cena sprzedaży"
 
 msgctxt "field:product.product,list_price_uom:"
 msgid "List Price"
-msgstr "定价"
+msgstr "Cena sprzedaży"
 
 msgctxt "field:product.product,list_prices:"
 msgid "List Prices"
-msgstr "定价"
+msgstr "Ceny sprzedaży"
 
 msgctxt "field:product.product,name:"
 msgid "Name"
-msgstr "名称"
+msgstr "Nazwa"
 
 msgctxt "field:product.product,prefix_code:"
 msgid "Prefix Code"
-msgstr "前缀代码"
+msgstr "Prefiks kodu"
 
 msgctxt "field:product.product,suffix_code:"
 msgid "Suffix Code"
-msgstr "后缀代码"
+msgstr "Sufiks kodu"
 
 msgctxt "field:product.product,template:"
 msgid "Product Template"
-msgstr "产品模板"
+msgstr "Szablon produktu"
 
 msgctxt "field:product.product,type:"
 msgid "Type"
-msgstr "类型"
+msgstr "Typ"
 
 msgctxt "field:product.template,categories:"
 msgid "Categories"
-msgstr "类别"
+msgstr "Kategorie"
 
 msgctxt "field:product.template,categories_all:"
 msgid "Categories"
-msgstr "类别"
+msgstr "Kategorie"
 
 msgctxt "field:product.template,code:"
 msgid "Code"
-msgstr "代码"
+msgstr "Kod"
 
 msgctxt "field:product.template,code_readonly:"
 msgid "Code Readonly"
-msgstr "代码（只读）"
+msgstr "Kod tylko do odczytu"
 
 msgctxt "field:product.template,consumable:"
 msgid "Consumable"
-msgstr "消耗品"
+msgstr "Artykuły konsumpcyjne"
 
 msgctxt "field:product.template,cost_price:"
 msgid "Cost Price"
-msgstr "成本价"
+msgstr "Cena kosztów"
 
 msgctxt "field:product.template,cost_price_method:"
 msgid "Cost Price Method"
-msgstr "成本价法"
+msgstr "Metoda wyceny zapasów"
 
 msgctxt "field:product.template,cost_price_methods:"
 msgid "Cost Price Methods"
-msgstr "成本价法"
+msgstr "Metody wyceny zapasów"
 
 msgctxt "field:product.template,default_uom:"
 msgid "Default UoM"
-msgstr "默认计量单位"
+msgstr "Domyślna jednostka miary"
 
 msgctxt "field:product.template,default_uom_category:"
 msgid "Default UoM Category"
-msgstr "默认计量单位类别"
+msgstr "Domyślna kategoria jednostka miary"
 
 msgctxt "field:product.template,list_price:"
 msgid "List Price"
-msgstr "定价"
+msgstr "Cena sprzedaży"
 
 msgctxt "field:product.template,list_prices:"
 msgid "List Prices"
-msgstr "定价"
+msgstr "Ceny sprzedaży"
 
 msgctxt "field:product.template,name:"
 msgid "Name"
-msgstr "名称"
+msgstr "Nazwa"
 
 msgctxt "field:product.template,products:"
 msgid "Variants"
-msgstr "变体"
+msgstr "Warianty"
 
 msgctxt "field:product.template,type:"
 msgid "Type"
-msgstr "类型"
+msgstr "Typ"
 
 msgctxt "field:product.template-product.category,category:"
 msgid "Category"
-msgstr "类别"
+msgstr "Kategoria"
 
 msgctxt "field:product.template-product.category,template:"
 msgid "Template"
-msgstr "模板"
+msgstr "Szablon"
 
 msgctxt "field:product.template-product.category.all,category:"
 msgid "Category"
-msgstr "类别"
+msgstr "Kategoria"
 
 msgctxt "field:product.template-product.category.all,template:"
 msgid "Template"
-msgstr "模板"
+msgstr "Szablon"
 
 msgctxt "field:product.uom,category:"
 msgid "Category"
-msgstr "类别"
+msgstr "Kategoria"
 
 msgctxt "field:product.uom,digits:"
 msgid "Display Digits"
-msgstr "显示数位"
+msgstr "Cyfry wyświetlane"
 
 msgctxt "field:product.uom,factor:"
 msgid "Factor"
-msgstr "换算因子"
+msgstr "Współczynnik"
 
 msgctxt "field:product.uom,name:"
 msgid "Name"
-msgstr "名称"
+msgstr "Nazwa"
 
 msgctxt "field:product.uom,rate:"
 msgid "Rate"
-msgstr "换算率"
+msgstr "Kurs"
 
 msgctxt "field:product.uom,rounding:"
 msgid "Rounding Precision"
-msgstr "舍入精度"
+msgstr "Dokładność"
 
 msgctxt "field:product.uom,symbol:"
 msgid "Symbol"
-msgstr "符号"
+msgstr "Symbol"
 
 msgctxt "field:product.uom.category,name:"
 msgid "Name"
-msgstr "名称"
+msgstr "Nazwa"
 
 msgctxt "field:product.uom.category,uoms:"
 msgid "Units of Measure"
-msgstr "计量单位"
+msgstr "Jednostki miary"
 
 msgctxt "help:product.category,childs:"
 msgid "Used to add structure below the category."
-msgstr "用于在类别下面添加结构."
+msgstr "Służy do dodawania struktury poniżej kategorii."
 
 msgctxt "help:product.category,parent:"
 msgid "Used to add structure above the category."
-msgstr "用于在类别上面添加结构."
+msgstr "Służy do dodawania struktury powyżej kategorii."
+
+msgctxt "help:product.configuration,category_sequence:"
+msgid "Used to generate the category code."
+msgstr "Służy do generowania kodu kategorii."
 
 msgctxt "help:product.configuration,default_cost_price_method:"
 msgid "The default cost price method for new products."
-msgstr "新产品默认使用的成本价格方法."
+msgstr "Domyślna metoda wyceny zapasów dla nowych produktów."
 
 msgctxt "help:product.configuration,product_sequence:"
 msgid "Used to generate the last part of the product code."
-msgstr "用于生成产品代码的最后一部分."
+msgstr "Służy do generowania końcowej części kodu produktu."
 
 msgctxt "help:product.configuration,template_sequence:"
 msgid "Used to generate the first part of the product code."
-msgstr "用于生成产品代码的第一部分."
+msgstr "Służy do generowania początkowej części kodu produktu."
 
 msgctxt ""
 "help:product.configuration.default_cost_price_method,default_cost_price_method:"
 msgid "The default cost price method for new products."
-msgstr "新产品默认使用的成本价格方法."
+msgstr "Domyślna metoda wyceny zapasów dla nowych produktów."
 
 msgctxt "help:product.identifier,product:"
 msgid "The product identified by the code."
-msgstr "此代码标识的产品."
+msgstr "Produkt identyfikowany kodem."
 
 msgctxt "help:product.product,categories:"
 msgid ""
 "The categories that the product is in.\n"
 "Used to group similar products together."
 msgstr ""
-"产品所属类别.\n"
-"用于将类似的产品聚在一组."
+"Kategorie, do których należy produkt.\n"
+"Służy do grupowania razem podobnych produktów."
 
 msgctxt "help:product.product,code:"
 msgid "A unique identifier for the variant."
-msgstr "变体的唯一标识符."
+msgstr "Unikalny identyfikator wariantu."
 
 msgctxt "help:product.product,consumable:"
 msgid "Check to allow stock moves to be assigned regardless of stock level."
-msgstr "选中此项后，将允许不考虑库存水平的情况下，分配库存移动."
+msgstr ""
+"Zaznacz, aby zezwolić na przenoszenie zapasów niezależnie od poziomu "
+"zapasów."
 
 msgctxt "help:product.product,cost_price:"
 msgid ""
 "The amount it costs to purchase or make the variant, or carry out the "
 "service."
-msgstr "购买或制作产品变体或执行服务所需的费用."
+msgstr "Koszt zakupu, wykonania wariantu produktu lub wykonania usługi."
 
 msgctxt "help:product.product,cost_price_method:"
 msgid "The method used to calculate the cost price."
-msgstr "用于计算成本价的方法."
+msgstr "Metoda użyta do obliczenia kosztu własnego."
 
 msgctxt "help:product.product,default_uom:"
 msgid ""
 "The standard Unit of Measure for the product.\n"
 "Used internally when calculating the stock levels of goods and assets."
 msgstr ""
-"产品的标准计量单位.\n"
-"在计算货物和资产的库存水平时内部使用."
+"Standardowa jednostka miary dla produktu.\n"
+"Stosowana wewnętrznie przy obliczaniu poziomu zapasów towarów i aktywów."
 
 msgctxt "help:product.product,default_uom_category:"
 msgid "The category of the default Unit of Measure."
-msgstr "默认计量单位类别。"
+msgstr "Kategoria domyślnej jednostki miary."
 
 msgctxt "help:product.product,identifiers:"
 msgid "Other identifiers associated with the variant."
-msgstr "其它标识符(产品变体相关)。"
+msgstr "Inne identyfikatory powiązane z wariantem produktu."
 
 msgctxt "help:product.product,list_price:"
 msgid "The standard price the product is sold at."
-msgstr "产品销售的标准价格."
+msgstr "Standardowa cena, za jaką sprzedawany jest produkt."
 
 msgctxt "help:product.product,suffix_code:"
 msgid "The unique identifier for the product (aka SKU)."
-msgstr "产品的唯一标识符（也称为SKU）."
+msgstr "Unikalny identyfikator produktu (znany również jako SKU)."
 
 msgctxt "help:product.product,template:"
 msgid ""
 "The product that defines the common properties inherited by the variant."
-msgstr "用来定义公共属性的产品，这些公共属性会被产品的变体继承."
+msgstr ""
+"Produkt, który definiuje typowe właściwości dziedziczone przez wariant "
+"produktu."
 
 msgctxt "help:product.template,categories:"
 msgid ""
 "The categories that the product is in.\n"
 "Used to group similar products together."
 msgstr ""
-"产品所属类别.\n"
-"用来将类似的产品分组."
+"Kategorie, do których należy produkt.\n"
+"Służy do grupowania razem podobnych produktów."
 
 msgctxt "help:product.template,consumable:"
 msgid "Check to allow stock moves to be assigned regardless of stock level."
-msgstr "选中此项后，将允许在不考虑库存水平的情况下，分配库存移动."
+msgstr ""
+"Zaznacz, aby zezwolić na przenoszenie zapasów niezależnie od poziomu "
+"zapasów."
 
 msgctxt "help:product.template,cost_price:"
 msgid ""
 "The amount it costs to purchase or make the product, or carry out the "
 "service."
-msgstr "购买或制造产品或提供服务所需的费用."
+msgstr "Koszt zakupu, wytworzenia produktu lub wykonania usługi."
 
 msgctxt "help:product.template,cost_price_method:"
 msgid "The method used to calculate the cost price."
-msgstr "用于计算成本价的方法."
+msgstr "Metoda użyta do obliczenia kosztu własnego."
 
 msgctxt "help:product.template,default_uom:"
 msgid ""
 "The standard Unit of Measure for the product.\n"
 "Used internally when calculating the stock levels of goods and assets."
 msgstr ""
-"产品标准计量单位.\n"
-"在计算货物和资产的库存水平时内部使用."
+"Standardowa jednostka miary dla produktu.\n"
+"Stosowana wewnętrznie przy obliczaniu poziomu zapasów towarów i aktywów."
 
 msgctxt "help:product.template,default_uom_category:"
 msgid "The category of the default Unit of Measure."
-msgstr "默认计量单位类别。"
+msgstr "Kategoria domyślnej jednostki miary."
 
 msgctxt "help:product.template,list_price:"
 msgid "The standard price the product is sold at."
-msgstr "产品销售的标准价格."
+msgstr "Standardowa cena, za jaką sprzedawany jest produkt."
 
 msgctxt "help:product.template,products:"
 msgid "The different variants the product comes in."
-msgstr "产品不同变体."
+msgstr "Różne warianty produktu."
 
 msgctxt "help:product.uom,category:"
 msgid ""
 "The category that contains the unit of measure.\n"
 "Conversions between different units of measure can be done if they are in the same category."
 msgstr ""
-"计量单位类别.\n"
-"属于同类别的计量单位之间可以相互转换."
+"Kategoria zawierająca jednostkę miary.\n"
+"Konwersje między różnymi jednostkami miary można dokonać, jeśli należą one do tej samej kategorii."
 
 msgctxt "help:product.uom,digits:"
 msgid "The number of digits to display after the decimal separator."
-msgstr "小数点后显示的数字位数."
+msgstr "Liczba cyfr po separatorze dziesiętnym."
 
 msgctxt "help:product.uom,factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "coefficient (base unit) = 1 (this unit)"
 msgstr ""
-"公式系数:\n"
-"系数 X 基本单位 = 1 X 当前单位"
+"Współczynnik dla wzoru:\n"
+"współczynnik (jednostka podstawowa) = 1 (ta jednostka)"
 
 msgctxt "help:product.uom,rate:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (base unit) = coef (this unit)"
 msgstr ""
-"换算公式的系数：\n"
-"1 X 基本单位 = 系数 X 当前单位"
+"Współczynnik dla wzoru:\n"
+"1 (jednostka bazowa) = coef (ta jednostka)"
 
 msgctxt "help:product.uom,rounding:"
 msgid "The accuracy to which values are rounded."
-msgstr "四舍五入精度."
+msgstr "Dokładność, z jaką wartości są zaokrąglane."
 
 msgctxt "help:product.uom,symbol:"
 msgid "The symbol that represents the unit of measure."
-msgstr "表示计量单位的符号."
+msgstr "Symbol reprezentujący jednostkę miary."
 
 msgctxt "model:ir.action,name:act_category_list"
 msgid "Categories"
-msgstr "类别"
+msgstr "Kategorie"
 
 msgctxt "model:ir.action,name:act_category_product"
 msgid "Add products"
-msgstr "添加产品"
+msgstr "Dodaj produkty"
 
 msgctxt "model:ir.action,name:act_category_tree"
 msgid "Categories"
-msgstr "类别"
+msgstr "Kategorie"
 
 msgctxt "model:ir.action,name:act_product_configuration_form"
 msgid "Configuration"
-msgstr "设置"
+msgstr "Konfiguracja"
 
 msgctxt "model:ir.action,name:act_product_form"
 msgid "Variants"
-msgstr "变体"
+msgstr "Warianty"
 
 msgctxt "model:ir.action,name:act_product_from_template"
 msgid "Variants"
-msgstr "变体"
+msgstr "Warianty"
 
 msgctxt "model:ir.action,name:act_template_by_category"
 msgid "Product by Category"
-msgstr "按类别划分的产品"
+msgstr "Produkt wg kategorii"
 
 msgctxt "model:ir.action,name:act_template_form"
 msgid "Products"
-msgstr "产品"
+msgstr "Produkty"
 
 msgctxt "model:ir.action,name:act_uom_category_form"
 msgid "Categories"
-msgstr "类别"
+msgstr "Kategorie"
 
 msgctxt "model:ir.action,name:act_uom_form"
 msgid "Units of Measure"
-msgstr "计量单位"
+msgstr "Jednostki miary"
+
+msgctxt "model:ir.message,text:msg_category_code_unique"
+msgid "The code on product category must be unique."
+msgstr "Kod kategorii produktu musi być unikalny."
 
 msgctxt "model:ir.message,text:msg_invalid_code"
 msgid "The %(type)s \"%(code)s\" for product \"%(product)s\" is not valid."
-msgstr "%(type)s \"%(code)s\" 对产品 \"%(product)s\" 是无效的."
+msgstr "%(type) s \"% (code) s” dla produktu \"% (product) s” jest nieprawidłowy."
 
 msgctxt "model:ir.message,text:msg_product_code_unique"
 msgid "Code of active product must be unique."
-msgstr "已启用产品的代码不能重复."
+msgstr "Kod aktywnego produktu musi być unikalny."
 
 msgctxt "model:ir.message,text:msg_uom_decrease_digits"
 msgid "You cannot decrease the digits of the unit of measure \"%(uom)s\"."
-msgstr "不能减少计量单位 \"%(uom)s\" 的位数。"
+msgstr "Nie można zmniejszyć cyfr jednostki miary \"%(uom)s\"."
 
 msgctxt "model:ir.message,text:msg_uom_incompatible_factor_rate"
 msgid "Incompatible factor and rate values on unit of measure\"%(uom)s\"."
-msgstr "与计量单位 \"%(uom)s\" 不兼容的换算因子和换算率."
+msgstr "Niezgodne wartości współczynnika i stawki w jednostce miary \"%(uom)s\"."
 
 msgctxt "model:ir.message,text:msg_uom_modify_category"
 msgid "You cannot modify the category of the unit of measure \"%(uom)s\"."
-msgstr "不能改变计量单位 \"%(uom)s\" 的类别."
+msgstr "Nie można modyfikować kategorii jednostki miary \"%(uom)s\"."
 
 msgctxt "model:ir.message,text:msg_uom_modify_factor"
 msgid "You cannot modify the factor of the unit of measure \"%(uom)s\"."
-msgstr "不能更改计量单位 \"%(uom)s\" 的换算因子."
+msgstr "Nie można modyfikować współczynnika jednostki miary \"%(uom)s\"."
 
 msgctxt "model:ir.message,text:msg_uom_modify_options"
 msgid ""
 "If the unit of measure is still not used, you can delete it otherwise you "
 "can deactivate it and create a new one."
-msgstr "从未使用过的计量单位可以删除，否则只能停用后再新建。"
+msgstr ""
+"Jeśli jednostka miary nadal nie jest używana, możesz ją usunąć, w przeciwnym"
+" razie możesz ją dezaktywować i utworzyć nową."
 
 msgctxt "model:ir.message,text:msg_uom_modify_rate"
 msgid "You cannot modify the rate of the unit of measure\"%(uom)s\"."
-msgstr "不能修改计量单位 \"%(uom)s\" 的换算率."
+msgstr "Nie można modyfikować stawki jednostki miary \"%(uom)s”."
 
 msgctxt "model:ir.message,text:msg_uom_no_zero_factor_rate"
 msgid "Rate and factor can not be both equal to zero."
-msgstr "换算率和换算因子不能同时为零."
+msgstr "Stawka i współczynnik nie mogą być równe zeru."
 
 msgctxt "model:ir.model.button,string:category_add_products_button"
 msgid "Add products"
-msgstr "添加产品"
+msgstr "Dodaj produkty"
+
+msgctxt "model:ir.sequence.type,name:sequence_type_category"
+msgid "Category"
+msgstr "Kategoria"
 
 msgctxt "model:ir.sequence.type,name:sequence_type_product"
 msgid "Variant"
-msgstr "变体"
+msgstr "Wariant"
 
 msgctxt "model:ir.sequence.type,name:sequence_type_template"
 msgid "Product"
-msgstr "产品"
+msgstr "Produkt"
 
 msgctxt "model:ir.ui.menu,name:menu_category_list"
 msgid "Categories"
-msgstr "类别"
+msgstr "Kategorie"
 
 msgctxt "model:ir.ui.menu,name:menu_category_tree"
 msgid "Categories"
-msgstr "类别"
+msgstr "Kategorie"
 
 msgctxt "model:ir.ui.menu,name:menu_configuration"
 msgid "Configuration"
-msgstr "设置"
+msgstr "Konfiguracja"
 
 msgctxt "model:ir.ui.menu,name:menu_main_product"
 msgid "Products"
-msgstr "产品"
+msgstr "Produkty"
 
 msgctxt "model:ir.ui.menu,name:menu_product"
 msgid "Variants"
-msgstr "变体"
+msgstr "Warianty"
 
 msgctxt "model:ir.ui.menu,name:menu_product_configuration"
 msgid "Configuration"
-msgstr "设置"
+msgstr "Konfiguracja"
 
 msgctxt "model:ir.ui.menu,name:menu_reporting"
 msgid "Reporting"
-msgstr "报告"
+msgstr "Raportowanie"
 
 msgctxt "model:ir.ui.menu,name:menu_template"
 msgid "Products"
-msgstr "产品设置"
+msgstr "Produkty"
 
 msgctxt "model:ir.ui.menu,name:menu_uom_category_form"
 msgid "Categories"
-msgstr "类别"
+msgstr "Kategorie"
 
 msgctxt "model:ir.ui.menu,name:menu_uom_form"
 msgid "Units of Measure"
-msgstr "计量单位"
+msgstr "Jednostki miary"
 
 msgctxt "model:product.category,name:"
 msgid "Product Category"
-msgstr "按类别划分的产品"
+msgstr "Produkt wg kategorii"
 
 msgctxt "model:product.configuration,name:"
 msgid "Product Configuration"
-msgstr "产品设置"
+msgstr "Konfiguracja produktu"
 
 msgctxt "model:product.configuration.default_cost_price_method,name:"
 msgid "Product Configuration Default Cost Price Method"
-msgstr "产品设置 - 默认的成本价法"
+msgstr "Konfiguracja domyślnej metody wyceny zapasów"
 
 msgctxt "model:product.cost_price,name:"
 msgid "Product Cost Price"
-msgstr "产品成本价"
+msgstr "Cena kosztów produktu"
 
 msgctxt "model:product.cost_price_method,name:"
 msgid "Product Cost Price Method"
-msgstr "产品成本价法"
+msgstr "Metoda wyceny zapasów produktów"
 
 msgctxt "model:product.identifier,name:"
 msgid "Product Identifier"
-msgstr "产品标识"
+msgstr "Identyfikator produktu"
 
 msgctxt "model:product.list_price,name:"
 msgid "Product List Price"
-msgstr "产品定价"
+msgstr "Cena sprzedaży produktu"
 
 msgctxt "model:product.product,name:"
 msgid "Product Variant"
-msgstr "产品变体"
+msgstr "Wariant produktu"
 
 msgctxt "model:product.template,name:"
 msgid "Product Template"
-msgstr "产品模板"
+msgstr "Szablon produktu"
 
 msgctxt "model:product.template-product.category,name:"
 msgid "Template - Category"
-msgstr "模板 - 类别"
+msgstr "Szablon - Kategoria"
 
 msgctxt "model:product.template-product.category.all,name:"
 msgid "Template - Category All"
-msgstr "模板 -所有类别"
+msgstr "Szablon - Wszystkie kategorie"
 
 msgctxt "model:product.uom,name:"
 msgid "Unit of Measure"
-msgstr "计量单位"
+msgstr "Jednostka miary"
 
 msgctxt "model:product.uom,name:uom_are"
 msgid "Are"
-msgstr "公亩"
+msgstr "Ar"
 
 msgctxt "model:product.uom,name:uom_carat"
 msgid "Carat"
-msgstr "克拉"
+msgstr "Karat"
 
 msgctxt "model:product.uom,name:uom_centimeter"
 msgid "Centimeter"
-msgstr "厘米"
+msgstr "Centymetr"
 
 msgctxt "model:product.uom,name:uom_cubic_centimeter"
 msgid "Cubic centimeter"
-msgstr "立方厘米"
+msgstr "Centymetr sześcienny"
 
 msgctxt "model:product.uom,name:uom_cubic_foot"
 msgid "Cubic foot"
-msgstr "立方英尺"
+msgstr "Stopa sześcienna"
 
 msgctxt "model:product.uom,name:uom_cubic_inch"
 msgid "Cubic inch"
-msgstr "立方英寸"
+msgstr "Cal sześcienny"
 
 msgctxt "model:product.uom,name:uom_cubic_meter"
 msgid "Cubic meter"
-msgstr "立方米"
+msgstr "Metr sześcienny"
 
 msgctxt "model:product.uom,name:uom_day"
 msgid "Day"
-msgstr "天"
+msgstr "Dzień"
 
 msgctxt "model:product.uom,name:uom_energy_joule"
 msgid "Joule"
-msgstr "焦耳"
+msgstr "Dżul"
 
 msgctxt "model:product.uom,name:uom_energy_kwh"
 msgid "Kilowatt-hour"
-msgstr "千瓦时"
+msgstr "Kilowatogodzina"
 
 msgctxt "model:product.uom,name:uom_energy_megajoule"
 msgid "Megajoule"
-msgstr "兆焦耳"
+msgstr "Megadżul"
 
 msgctxt "model:product.uom,name:uom_energy_mwh"
 msgid "Megawatt-hour"
-msgstr "兆瓦时"
+msgstr "Megawatogodzina"
 
 msgctxt "model:product.uom,name:uom_foot"
 msgid "Foot"
-msgstr "英尺"
+msgstr "Stopa"
 
 msgctxt "model:product.uom,name:uom_gallon"
 msgid "Gallon"
-msgstr "加仑"
+msgstr "Galon"
 
 msgctxt "model:product.uom,name:uom_gram"
 msgid "Gram"
-msgstr "加仑"
+msgstr "Gram"
 
 msgctxt "model:product.uom,name:uom_hectare"
 msgid "Hectare"
-msgstr "公顷"
+msgstr "Hektar"
 
 msgctxt "model:product.uom,name:uom_hour"
 msgid "Hour"
-msgstr "小时"
+msgstr "Godzina"
 
 msgctxt "model:product.uom,name:uom_inch"
 msgid "Inch"
-msgstr "英寸"
+msgstr "Cal"
 
 msgctxt "model:product.uom,name:uom_kilogram"
 msgid "Kilogram"
-msgstr "千克"
+msgstr "Kilogram"
 
 msgctxt "model:product.uom,name:uom_kilometer"
 msgid "Kilometer"
-msgstr "千米"
+msgstr "Kilometr"
 
 msgctxt "model:product.uom,name:uom_liter"
 msgid "Liter"
-msgstr "公升"
+msgstr "Litr"
 
 msgctxt "model:product.uom,name:uom_meter"
 msgid "Meter"
-msgstr "米"
+msgstr "Metr"
 
 msgctxt "model:product.uom,name:uom_mile"
 msgid "Mile"
-msgstr "英里"
+msgstr "Mila"
 
 msgctxt "model:product.uom,name:uom_millimeter"
 msgid "Millimeter"
-msgstr "毫米"
+msgstr "Milimetr"
 
 msgctxt "model:product.uom,name:uom_minute"
 msgid "Minute"
-msgstr "分钟"
+msgstr "Minuta"
 
 msgctxt "model:product.uom,name:uom_ounce"
 msgid "Ounce"
-msgstr "盎司"
+msgstr "Uncja"
 
 msgctxt "model:product.uom,name:uom_pound"
 msgid "Pound"
-msgstr "英镑"
+msgstr "Funt"
 
 msgctxt "model:product.uom,name:uom_second"
 msgid "Second"
-msgstr "秒"
+msgstr "Sekunda"
 
 msgctxt "model:product.uom,name:uom_square_centimeter"
 msgid "Square centimeter"
-msgstr "平方厘米"
+msgstr "Centymetr kwadratowy"
 
 msgctxt "model:product.uom,name:uom_square_foot"
 msgid "Square foot"
-msgstr "平方英尺"
+msgstr "Stopa kwadratowa"
 
 msgctxt "model:product.uom,name:uom_square_inch"
 msgid "Square inch"
-msgstr "平方英寸"
+msgstr "Cal kwadratowy"
 
 msgctxt "model:product.uom,name:uom_square_meter"
 msgid "Square meter"
-msgstr "平方米"
+msgstr "Metr kwadratowy"
 
 msgctxt "model:product.uom,name:uom_square_yard"
 msgid "Square yard"
-msgstr "平方码"
+msgstr "Jard kwadratowy"
 
 msgctxt "model:product.uom,name:uom_unit"
 msgid "Unit"
-msgstr "单位"
+msgstr "Jednostka"
 
 msgctxt "model:product.uom,name:uom_yard"
 msgid "Yard"
-msgstr "码"
+msgstr "Jard"
 
 msgctxt "model:product.uom,symbol:uom_are"
 msgid "a"
 msgstr "a"
 
 msgctxt "model:product.uom,symbol:uom_carat"
 msgid "c"
@@ -801,23 +833,23 @@
 
 msgctxt "model:product.uom,symbol:uom_energy_joule"
 msgid "J"
 msgstr "J"
 
 msgctxt "model:product.uom,symbol:uom_energy_kwh"
 msgid "kW⋅h"
-msgstr "kW⋅h"
+msgstr "kWh"
 
 msgctxt "model:product.uom,symbol:uom_energy_megajoule"
 msgid "MJ"
 msgstr "MJ"
 
 msgctxt "model:product.uom,symbol:uom_energy_mwh"
 msgid "MW⋅h"
-msgstr "MW⋅h"
+msgstr "MWh"
 
 msgctxt "model:product.uom,symbol:uom_foot"
 msgid "ft"
 msgstr "ft"
 
 msgctxt "model:product.uom,symbol:uom_gallon"
 msgid "gal"
@@ -897,124 +929,132 @@
 
 msgctxt "model:product.uom,symbol:uom_square_yard"
 msgid "yd²"
 msgstr "yd²"
 
 msgctxt "model:product.uom,symbol:uom_unit"
 msgid "u"
-msgstr "u"
+msgstr "szt."
 
 msgctxt "model:product.uom,symbol:uom_yard"
 msgid "yd"
 msgstr "yd"
 
 msgctxt "model:product.uom.category,name:"
 msgid "Unit of Measure Category"
-msgstr "计量单位类别"
+msgstr "Kategoria jednostek miary"
 
 msgctxt "model:product.uom.category,name:uom_cat_energy"
 msgid "Energy"
-msgstr "能量"
+msgstr "Energia"
 
 msgctxt "model:product.uom.category,name:uom_cat_length"
 msgid "Length"
-msgstr "长度"
+msgstr "Długość"
 
 msgctxt "model:product.uom.category,name:uom_cat_surface"
 msgid "Surface"
-msgstr "面积"
+msgstr "Powierzchnia"
 
 msgctxt "model:product.uom.category,name:uom_cat_time"
 msgid "Time"
-msgstr "时间"
+msgstr "Czas"
 
 msgctxt "model:product.uom.category,name:uom_cat_unit"
 msgid "Units"
-msgstr "单位"
+msgstr "Sztuki"
 
 msgctxt "model:product.uom.category,name:uom_cat_volume"
 msgid "Volume"
-msgstr "体积或容量"
+msgstr "Objętość"
 
 msgctxt "model:product.uom.category,name:uom_cat_weight"
 msgid "Weight"
-msgstr "重量"
+msgstr "Waga"
 
 msgctxt "model:res.group,name:group_product_admin"
 msgid "Product Administration"
-msgstr "产品管理"
+msgstr "Administracja ustawieniami produktu"
+
+msgctxt "selection:product.identifier,type:"
+msgid "Brand"
+msgstr "Marka"
 
 msgctxt "selection:product.identifier,type:"
 msgid "International Article Number"
-msgstr "国际商品编码"
+msgstr "Międzynarodowy numer artykułu"
 
 msgctxt "selection:product.identifier,type:"
 msgid "International Securities Identification Number"
-msgstr "国际证券识别码"
+msgstr "Międzynarodowy numer identyfikacyjny papierów wartościowych"
 
 msgctxt "selection:product.identifier,type:"
 msgid "International Standard Audiovisual Number"
-msgstr "国际标准音视频编号"
+msgstr "Międzynarodowy Standardowy Numer Audiowizualny"
 
 msgctxt "selection:product.identifier,type:"
 msgid "International Standard Book Number"
-msgstr "国际标准书号"
+msgstr "Międzynarodowy standardowy numer książki"
 
 msgctxt "selection:product.identifier,type:"
 msgid "International Standard Identifier for Libraries"
-msgstr "图书馆国际标准标识符"
+msgstr "Międzynarodowy identyfikator standardu dla bibliotek"
 
 msgctxt "selection:product.identifier,type:"
 msgid "International Standard Music Number"
-msgstr "国际标准乐谱号"
+msgstr "Międzynarodowy standardowy numer muzyczny"
+
+msgctxt "selection:product.identifier,type:"
+msgid "Manufacturer Part Number"
+msgstr "Numer części producenta"
 
 msgctxt "selection:product.product,cost_price_method:"
 msgid "Average"
-msgstr "平均成本价法"
+msgstr "Średnia"
 
 msgctxt "selection:product.product,cost_price_method:"
 msgid "Fixed"
-msgstr "固定成本价法"
+msgstr "Stała"
 
 msgctxt "selection:product.product,type:"
 msgid "Assets"
-msgstr "资产"
+msgstr "Majątek"
 
 msgctxt "selection:product.product,type:"
 msgid "Goods"
-msgstr "货物"
+msgstr "Towar"
 
 msgctxt "selection:product.product,type:"
 msgid "Service"
-msgstr "服务"
+msgstr "Usługa"
 
 msgctxt "selection:product.template,cost_price_method:"
 msgid "Average"
-msgstr "平均成本价法"
+msgstr "Średnia"
 
 msgctxt "selection:product.template,cost_price_method:"
 msgid "Fixed"
-msgstr "固定成本价法"
+msgstr "Stała"
 
 msgctxt "selection:product.template,type:"
 msgid "Assets"
-msgstr "资产"
+msgstr "Majątek"
 
 msgctxt "selection:product.template,type:"
 msgid "Goods"
-msgstr "货物"
+msgstr "Towar"
 
 msgctxt "selection:product.template,type:"
 msgid "Service"
-msgstr "服务"
+msgstr "Usługa"
 
 msgctxt "view:product.category:"
 msgid "Children"
-msgstr "子类别"
+msgstr "Kategorie podrzędne"
 
 msgctxt "view:product.configuration:"
 msgid "Sequences"
-msgstr "产品序列"
+msgstr "Sekwencje"
 
 msgctxt "view:product.template:"
 msgid "General"
-msgstr "常规"
+msgstr "Ogólne"
```

### Comparing `trytond_product-7.2.0/message.xml` & `trytond_product-7.2.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_product-7.2.0/product.py` & `trytond_product-7.2.1/product.py`

 * *Files identical despite different names*

### Comparing `trytond_product-7.2.0/product.xml` & `trytond_product-7.2.1/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_product-7.2.0/setup.py` & `trytond_product-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_product-7.2.0/tests/scenario_product_identifier.rst` & `trytond_product-7.2.1/tests/scenario_product_identifier.rst`

 * *Files identical despite different names*

### Comparing `trytond_product-7.2.0/tests/scenario_product_variant.rst` & `trytond_product-7.2.1/tests/scenario_product_variant.rst`

 * *Files identical despite different names*

### Comparing `trytond_product-7.2.0/tests/test_module.py` & `trytond_product-7.2.1/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_product-7.2.0/tox.ini` & `trytond_product-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_product-7.2.0/trytond_product.egg-info/PKG-INFO` & `trytond_product-7.2.1/trytond_product.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_product
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module with products
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_product-7.2.0/trytond_product.egg-info/SOURCES.txt` & `trytond_product-7.2.1/trytond_product.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_product-7.2.0/uom.py` & `trytond_product-7.2.1/uom.py`

 * *Files identical despite different names*

### Comparing `trytond_product-7.2.0/uom.xml` & `trytond_product-7.2.1/uom.xml`

 * *Files identical despite different names*

### Comparing `trytond_product-7.2.0/view/category_form.xml` & `trytond_product-7.2.1/view/category_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_product-7.2.0/view/configuration_form.xml` & `trytond_product-7.2.1/view/configuration_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_product-7.2.0/view/product_form.xml` & `trytond_product-7.2.1/view/product_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_product-7.2.0/view/product_form_simple.xml` & `trytond_product-7.2.1/view/product_form_simple.xml`

 * *Files identical despite different names*

### Comparing `trytond_product-7.2.0/view/template_form.xml` & `trytond_product-7.2.1/view/template_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_product-7.2.0/view/uom_form.xml` & `trytond_product-7.2.1/view/uom_form.xml`

 * *Files identical despite different names*

