# Comparing `tmp/trytond_product_kit-7.0.3.tar.gz` & `tmp/trytond_product_kit-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_product_kit-7.0.3.tar", last modified: Wed May  1 11:50:48 2024, max compression
+gzip compressed data, was "trytond_product_kit-7.2.0.tar", last modified: Mon Apr 29 15:43:20 2024, max compression
```

## Comparing `trytond_product_kit-7.0.3.tar` & `trytond_product_kit-7.2.0.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:50:48.943682 trytond_product_kit-7.0.3/
--rw-r--r--   0 ced       (1000) ced       (1000)     1217 2024-05-01 11:50:45.000000 trytond_product_kit-7.0.3/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      730 2024-05-01 11:50:45.000000 trytond_product_kit-7.0.3/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_product_kit-7.0.3/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_product_kit-7.0.3/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3095 2024-05-01 11:50:48.943682 trytond_product_kit-7.0.3/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      261 2023-10-30 17:06:38.000000 trytond_product_kit-7.0.3/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1884 2023-10-30 17:06:38.000000 trytond_product_kit-7.0.3/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1880 2023-10-30 17:06:38.000000 trytond_product_kit-7.0.3/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)    16878 2024-04-26 15:20:58.000000 trytond_product_kit-7.0.3/common.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:50:48.933682 trytond_product_kit-7.0.3/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2790 2024-03-03 16:24:20.000000 trytond_product_kit-7.0.3/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3587 2023-10-30 17:06:38.000000 trytond_product_kit-7.0.3/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      261 2023-10-30 17:06:38.000000 trytond_product_kit-7.0.3/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-10-30 17:06:38.000000 trytond_product_kit-7.0.3/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_product_kit-7.0.3/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:50:48.937015 trytond_product_kit-7.0.3/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     5729 2023-10-30 17:06:38.000000 trytond_product_kit-7.0.3/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6984 2023-10-30 17:06:38.000000 trytond_product_kit-7.0.3/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5729 2023-10-30 17:06:38.000000 trytond_product_kit-7.0.3/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7128 2023-10-30 17:06:38.000000 trytond_product_kit-7.0.3/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7056 2023-10-30 17:06:38.000000 trytond_product_kit-7.0.3/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5729 2023-10-30 17:06:38.000000 trytond_product_kit-7.0.3/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5729 2023-10-30 17:06:38.000000 trytond_product_kit-7.0.3/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5729 2023-10-30 17:06:38.000000 trytond_product_kit-7.0.3/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5729 2023-10-30 17:06:38.000000 trytond_product_kit-7.0.3/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6999 2023-10-30 17:06:38.000000 trytond_product_kit-7.0.3/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5729 2023-10-30 17:06:38.000000 trytond_product_kit-7.0.3/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5735 2023-10-30 17:06:38.000000 trytond_product_kit-7.0.3/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5756 2023-10-30 17:06:38.000000 trytond_product_kit-7.0.3/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5729 2023-10-30 17:06:38.000000 trytond_product_kit-7.0.3/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5729 2023-10-30 17:06:38.000000 trytond_product_kit-7.0.3/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7040 2023-10-30 17:06:38.000000 trytond_product_kit-7.0.3/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5729 2023-10-30 17:06:38.000000 trytond_product_kit-7.0.3/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5729 2023-10-30 17:06:38.000000 trytond_product_kit-7.0.3/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5729 2023-10-30 17:06:38.000000 trytond_product_kit-7.0.3/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5729 2023-10-30 17:06:38.000000 trytond_product_kit-7.0.3/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5729 2023-10-30 17:06:38.000000 trytond_product_kit-7.0.3/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5729 2023-10-30 17:06:38.000000 trytond_product_kit-7.0.3/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5729 2023-10-30 17:06:38.000000 trytond_product_kit-7.0.3/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5729 2023-10-30 17:06:38.000000 trytond_product_kit-7.0.3/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10061 2023-10-30 17:06:38.000000 trytond_product_kit-7.0.3/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      992 2023-10-30 17:06:38.000000 trytond_product_kit-7.0.3/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     6529 2023-10-30 17:06:38.000000 trytond_product_kit-7.0.3/purchase.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1044 2023-10-30 17:06:38.000000 trytond_product_kit-7.0.3/purchase.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     6951 2024-02-05 16:24:27.000000 trytond_product_kit-7.0.3/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)      996 2023-10-30 17:06:38.000000 trytond_product_kit-7.0.3/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 11:50:48.943682 trytond_product_kit-7.0.3/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4937 2024-03-03 16:24:03.000000 trytond_product_kit-7.0.3/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9303 2023-12-10 12:55:22.000000 trytond_product_kit-7.0.3/stock.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:50:48.937015 trytond_product_kit-7.0.3/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_product_kit-7.0.3/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4448 2024-02-05 16:24:27.000000 trytond_product_kit-7.0.3/tests/scenario_product_kit.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2043 2024-02-05 16:24:27.000000 trytond_product_kit-7.0.3/tests/scenario_product_kit_copy.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2406 2024-02-05 16:24:27.000000 trytond_product_kit-7.0.3/tests/scenario_product_kit_duplicate.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     8358 2024-02-05 16:24:27.000000 trytond_product_kit-7.0.3/tests/scenario_product_kit_purchase.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     8012 2024-02-05 16:24:27.000000 trytond_product_kit-7.0.3/tests/scenario_product_kit_sale.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      471 2023-10-30 17:06:38.000000 trytond_product_kit-7.0.3/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-10-30 17:06:38.000000 trytond_product_kit-7.0.3/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_product_kit-7.0.3/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      249 2024-02-05 16:24:27.000000 trytond_product_kit-7.0.3/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:50:48.943682 trytond_product_kit-7.0.3/trytond_product_kit.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3095 2024-05-01 11:50:48.000000 trytond_product_kit-7.0.3/trytond_product_kit.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2504 2024-05-01 11:50:48.000000 trytond_product_kit-7.0.3/trytond_product_kit.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:50:48.000000 trytond_product_kit-7.0.3/trytond_product_kit.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       60 2024-05-01 11:50:48.000000 trytond_product_kit-7.0.3/trytond_product_kit.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:07:56.000000 trytond_product_kit-7.0.3/trytond_product_kit.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      314 2024-05-01 11:50:48.000000 trytond_product_kit-7.0.3/trytond_product_kit.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 11:50:48.000000 trytond_product_kit-7.0.3/trytond_product_kit.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:50:48.943682 trytond_product_kit-7.0.3/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      678 2023-10-30 17:06:38.000000 trytond_product_kit-7.0.3/view/product_component_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      380 2023-10-30 17:06:38.000000 trytond_product_kit-7.0.3/view/product_component_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      356 2023-10-30 17:06:38.000000 trytond_product_kit-7.0.3/view/product_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      511 2023-10-30 17:06:38.000000 trytond_product_kit-7.0.3/view/purchase_line_component_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      323 2023-10-30 17:06:38.000000 trytond_product_kit-7.0.3/view/purchase_line_component_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      434 2023-10-30 17:06:38.000000 trytond_product_kit-7.0.3/view/purchase_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      511 2023-10-30 17:06:38.000000 trytond_product_kit-7.0.3/view/sale_line_component_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      323 2023-10-30 17:06:38.000000 trytond_product_kit-7.0.3/view/sale_line_component_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      434 2023-10-30 17:06:38.000000 trytond_product_kit-7.0.3/view/sale_line_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:20.674866 trytond_product_kit-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1015 2024-04-29 15:21:59.000000 trytond_product_kit-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      730 2024-04-29 15:21:59.000000 trytond_product_kit-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_product_kit-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_product_kit-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3095 2024-04-29 15:43:20.674866 trytond_product_kit-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      261 2023-04-15 07:12:15.000000 trytond_product_kit-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1884 2024-02-04 18:51:26.000000 trytond_product_kit-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1880 2023-04-15 07:12:15.000000 trytond_product_kit-7.2.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    16878 2024-04-27 16:30:39.000000 trytond_product_kit-7.2.0/common.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:20.671533 trytond_product_kit-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3074 2024-04-27 16:30:39.000000 trytond_product_kit-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3587 2023-04-15 07:12:15.000000 trytond_product_kit-7.2.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      261 2023-04-15 07:12:15.000000 trytond_product_kit-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_product_kit-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:16.000000 trytond_product_kit-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:20.671533 trytond_product_kit-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     5729 2024-04-27 16:43:25.000000 trytond_product_kit-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6984 2024-04-27 16:43:25.000000 trytond_product_kit-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5729 2024-04-27 16:43:25.000000 trytond_product_kit-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7128 2024-04-27 16:43:25.000000 trytond_product_kit-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7056 2024-04-27 16:43:25.000000 trytond_product_kit-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5729 2024-04-27 16:43:25.000000 trytond_product_kit-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5729 2024-04-27 16:43:25.000000 trytond_product_kit-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5729 2024-04-27 16:43:25.000000 trytond_product_kit-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5729 2024-04-27 16:43:25.000000 trytond_product_kit-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6999 2024-04-27 16:43:25.000000 trytond_product_kit-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5729 2024-04-27 16:43:25.000000 trytond_product_kit-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5735 2024-04-27 16:43:25.000000 trytond_product_kit-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5756 2024-04-27 16:43:25.000000 trytond_product_kit-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5729 2024-04-27 16:43:25.000000 trytond_product_kit-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5729 2024-04-27 16:43:25.000000 trytond_product_kit-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7040 2024-04-27 16:43:25.000000 trytond_product_kit-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5729 2024-04-27 16:43:25.000000 trytond_product_kit-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5729 2024-04-27 16:43:25.000000 trytond_product_kit-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5729 2024-04-27 16:43:25.000000 trytond_product_kit-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5729 2024-04-27 16:43:25.000000 trytond_product_kit-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5729 2024-04-27 16:43:25.000000 trytond_product_kit-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5729 2024-04-27 16:43:25.000000 trytond_product_kit-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5729 2024-04-27 16:43:25.000000 trytond_product_kit-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5729 2024-04-27 16:43:25.000000 trytond_product_kit-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10061 2024-01-27 09:58:52.000000 trytond_product_kit-7.2.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      992 2023-04-15 07:12:15.000000 trytond_product_kit-7.2.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     6529 2024-02-04 18:51:26.000000 trytond_product_kit-7.2.0/purchase.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1044 2023-04-15 07:12:15.000000 trytond_product_kit-7.2.0/purchase.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     7677 2024-04-22 12:14:36.000000 trytond_product_kit-7.2.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      996 2023-04-15 07:12:15.000000 trytond_product_kit-7.2.0/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:43:20.674866 trytond_product_kit-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4937 2024-04-27 16:30:39.000000 trytond_product_kit-7.2.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9303 2024-04-13 17:12:23.000000 trytond_product_kit-7.2.0/stock.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:20.674866 trytond_product_kit-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_product_kit-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4426 2024-04-22 12:14:36.000000 trytond_product_kit-7.2.0/tests/scenario_product_kit.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2036 2024-04-22 12:14:36.000000 trytond_product_kit-7.2.0/tests/scenario_product_kit_copy.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2384 2024-04-22 12:14:36.000000 trytond_product_kit-7.2.0/tests/scenario_product_kit_duplicate.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     8350 2024-04-27 16:30:39.000000 trytond_product_kit-7.2.0/tests/scenario_product_kit_purchase.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     8003 2024-04-27 16:30:39.000000 trytond_product_kit-7.2.0/tests/scenario_product_kit_sale.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      471 2024-02-04 18:51:26.000000 trytond_product_kit-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_product_kit-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:16.000000 trytond_product_kit-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      249 2024-04-29 15:21:55.000000 trytond_product_kit-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:20.674866 trytond_product_kit-7.2.0/trytond_product_kit.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3095 2024-04-29 15:43:20.000000 trytond_product_kit-7.2.0/trytond_product_kit.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2504 2024-04-29 15:43:20.000000 trytond_product_kit-7.2.0/trytond_product_kit.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:43:20.000000 trytond_product_kit-7.2.0/trytond_product_kit.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       60 2024-04-29 15:43:20.000000 trytond_product_kit-7.2.0/trytond_product_kit.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:58.000000 trytond_product_kit-7.2.0/trytond_product_kit.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      314 2024-04-29 15:43:20.000000 trytond_product_kit-7.2.0/trytond_product_kit.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:43:20.000000 trytond_product_kit-7.2.0/trytond_product_kit.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:20.674866 trytond_product_kit-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      678 2023-04-15 07:12:15.000000 trytond_product_kit-7.2.0/view/product_component_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      380 2023-04-15 07:12:15.000000 trytond_product_kit-7.2.0/view/product_component_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      356 2023-04-15 07:12:15.000000 trytond_product_kit-7.2.0/view/product_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      511 2023-04-15 07:12:15.000000 trytond_product_kit-7.2.0/view/purchase_line_component_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      323 2023-04-15 07:12:15.000000 trytond_product_kit-7.2.0/view/purchase_line_component_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      434 2023-04-15 07:12:15.000000 trytond_product_kit-7.2.0/view/purchase_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      511 2023-04-15 07:12:15.000000 trytond_product_kit-7.2.0/view/sale_line_component_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      323 2023-04-15 07:12:15.000000 trytond_product_kit-7.2.0/view/sale_line_component_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      434 2023-04-15 07:12:15.000000 trytond_product_kit-7.2.0/view/sale_line_form.xml
```

### Comparing `trytond_product_kit-7.0.3/CHANGELOG` & `trytond_product_kit-7.2.0/CHANGELOG`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,9 @@
 
-Version 7.0.3 - 2024-05-01
---------------------------
-* Bug fixes (see mercurial logs for details)
-
-
-Version 7.0.2 - 2024-01-15
---------------------------
-* Bug fixes (see mercurial logs for details)
-
-
-Version 7.0.1 - 2023-12-16
+Version 7.2.0 - 2024-04-29
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 
 Version 7.0.0 - 2023-10-30
 --------------------------
 * Bug fixes (see mercurial logs for details)
```

### Comparing `trytond_product_kit-7.0.3/COPYRIGHT` & `trytond_product_kit-7.2.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_product_kit-7.0.3/LICENSE` & `trytond_product_kit-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_product_kit-7.0.3/PKG-INFO` & `trytond_product_kit-7.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_product_kit
-Version: 7.0.3
+Version: 7.2.0
 Summary: Tryton module to manage product kits and components
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/modules-product-kit
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
@@ -46,26 +46,26 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account_invoice<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account_invoice_stock<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_company<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_purchase<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_purchase_amendment<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale_amendment<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_stock<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_invoice<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_invoice_stock<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_company<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_purchase<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_purchase_amendment<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_amendment<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_stock<7.3,>=7.2; extra == "test"
 
 ##################
 Product Kit Module
 ##################
 
 The *Product Kit Module* adds kits and components to products.
 This enables a defined set of products to be sold or purchased using a single
```

### Comparing `trytond_product_kit-7.0.3/__init__.py` & `trytond_product_kit-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_product_kit-7.0.3/account.py` & `trytond_product_kit-7.2.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_product_kit-7.0.3/common.py` & `trytond_product_kit-7.2.0/common.py`

 * *Files identical despite different names*

### Comparing `trytond_product_kit-7.0.3/doc/conf.py` & `trytond_product_kit-7.2.0/doc/conf.py`

 * *Files 3% similar despite different names*

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

### Comparing `trytond_product_kit-7.0.3/doc/design.rst` & `trytond_product_kit-7.2.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_product_kit-7.0.3/locale/bg.po` & `trytond_product_kit-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_product_kit-7.0.3/locale/ca.po` & `trytond_product_kit-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_product_kit-7.0.3/locale/cs.po` & `trytond_product_kit-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_product_kit-7.0.3/locale/de.po` & `trytond_product_kit-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_product_kit-7.0.3/locale/es.po` & `trytond_product_kit-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_product_kit-7.0.3/locale/es_419.po` & `trytond_product_kit-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_product_kit-7.0.3/locale/et.po` & `trytond_product_kit-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_product_kit-7.0.3/locale/fa.po` & `trytond_product_kit-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_product_kit-7.0.3/locale/fi.po` & `trytond_product_kit-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_product_kit-7.0.3/locale/fr.po` & `trytond_product_kit-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_product_kit-7.0.3/locale/hu.po` & `trytond_product_kit-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_product_kit-7.0.3/locale/id.po` & `trytond_product_kit-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_product_kit-7.0.3/locale/it.po` & `trytond_product_kit-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_product_kit-7.0.3/locale/lo.po` & `trytond_product_kit-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_product_kit-7.0.3/locale/lt.po` & `trytond_product_kit-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_product_kit-7.0.3/locale/nl.po` & `trytond_product_kit-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_product_kit-7.0.3/locale/pl.po` & `trytond_product_kit-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_product_kit-7.0.3/locale/pt.po` & `trytond_product_kit-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_product_kit-7.0.3/locale/ro.po` & `trytond_product_kit-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_product_kit-7.0.3/locale/ru.po` & `trytond_product_kit-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_product_kit-7.0.3/locale/sl.po` & `trytond_product_kit-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_product_kit-7.0.3/locale/tr.po` & `trytond_product_kit-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_product_kit-7.0.3/locale/uk.po` & `trytond_product_kit-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_product_kit-7.0.3/locale/zh_CN.po` & `trytond_product_kit-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_product_kit-7.0.3/product.py` & `trytond_product_kit-7.2.0/product.py`

 * *Files identical despite different names*

### Comparing `trytond_product_kit-7.0.3/product.xml` & `trytond_product_kit-7.2.0/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_product_kit-7.0.3/purchase.py` & `trytond_product_kit-7.2.0/purchase.py`

 * *Files identical despite different names*

### Comparing `trytond_product_kit-7.0.3/purchase.xml` & `trytond_product_kit-7.2.0/purchase.xml`

 * *Files identical despite different names*

### Comparing `trytond_product_kit-7.0.3/sale.py` & `trytond_product_kit-7.2.0/sale.py`

 * *Files 4% similar despite different names*

```diff
@@ -128,14 +128,31 @@
             for invoice_line in self.line.invoice_lines:
                 if (invoice_line.invoice
                         and invoice_line.invoice.state == 'paid'):
                     quantity += Uom.compute_qty(invoice_line.unit,
                         invoice_line.quantity, self.line.unit)
             return self.quantity * quantity / self.line.quantity
 
+    @property
+    def _move_remaining_quantity(self):
+        pool = Pool()
+        UoM = pool.get('product.uom')
+        quantity = super()._move_remaining_quantity
+        if self.line.sale.shipment_method == 'invoice':
+            invoices_ignored = set(self.line.sale.invoices_ignored)
+            ratio = self.get_moved_ratio()
+            if ratio:
+                for invoice_line in self.line.invoice_lines:
+                    if invoice_line.invoice in invoices_ignored:
+                        quantity -= UoM.compute_qty(
+                            invoice_line.unit * self.line.unit,
+                            invoice_line.quantity / ratio,
+                            self.line.unit)
+        return quantity
+
     def check_move_quantity(self):
         from trytond.modules.sale.exceptions import SaleMoveQuantity
         pool = Pool()
         Lang = pool.get('ir.lang')
         Warning = pool.get('res.user.warning')
         lang = Lang.get()
         move_type = 'in' if self.quantity >= 0 else 'return'
```

### Comparing `trytond_product_kit-7.0.3/sale.xml` & `trytond_product_kit-7.2.0/sale.xml`

 * *Files identical despite different names*

### Comparing `trytond_product_kit-7.0.3/setup.py` & `trytond_product_kit-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_product_kit-7.0.3/stock.py` & `trytond_product_kit-7.2.0/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_product_kit-7.0.3/tests/scenario_product_kit.rst` & `trytond_product_kit-7.2.0/tests/scenario_product_kit.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 ====================
 Product Kit Scenario
 ====================
 
 Imports::
 
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard
+
+    >>> from proteus import Model
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
 
 Activate product_kit and stock::
 
     >>> config = activate_modules(['product_kit', 'stock'])
 
 Create company::
```

### Comparing `trytond_product_kit-7.0.3/tests/scenario_product_kit_copy.rst` & `trytond_product_kit-7.2.0/tests/scenario_product_kit_duplicate.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,73 +1,86 @@
-=========================
-Product Kit Copy Scenario
-=========================
+==============================
+Product Kit Duplicate Scenario
+==============================
 
 Imports::
 
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard
+
+    >>> from proteus import Model
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company
 
-Activate product_kit and stock::
+Activate product_kit::
 
     >>> config = activate_modules('product_kit')
 
+    >>> Uom = Model.get('product.uom')
+    >>> ProductTemplate = Model.get('product.template')
+    >>> Product = Model.get('product.product')
+
 Create company::
 
     >>> _ = create_company()
+    >>> company = get_company()
 
 Create products::
 
-    >>> Uom = Model.get('product.uom')
     >>> unit, = Uom.find([('name', '=', 'Unit')])
-    >>> meter, = Uom.find([('name', '=', "Meter")])
-    >>> ProductTemplate = Model.get('product.template')
-    >>> Product = Model.get('product.product')
-
     >>> template = ProductTemplate()
     >>> template.name = "Product 1"
     >>> template.default_uom = unit
     >>> template.type = 'goods'
     >>> template.save()
     >>> product1, = template.products
     >>> product1.cost_price = Decimal('10.0000')
     >>> product1.save()
 
     >>> template = ProductTemplate()
     >>> template.name = "Product 2"
-    >>> template.default_uom = meter
+    >>> template.default_uom = unit
     >>> template.type = 'goods'
     >>> template.save()
     >>> product2, = template.products
     >>> product2.cost_price = Decimal('20.0000')
     >>> product2.save()
 
+Create composed product::
+
+    >>> template = ProductTemplate()
+    >>> template.name = "Composed Product"
+    >>> template.default_uom = unit
+    >>> template.type = 'goods'
+    >>> template.save()
+    >>> composed_product, = template.products
+    >>> composed_product.cost_price = Decimal('10.0000')
+
+    >>> component = composed_product.components.new()
+    >>> component.product = product1
+    >>> component.quantity = 2
+    >>> composed_product.save()
+
 Create a kit::
 
     >>> template = ProductTemplate()
     >>> template.name = "Kit"
     >>> template.default_uom = unit
     >>> template.type = 'kit'
     >>> template.save()
     >>> kit, = template.products
 
     >>> component = template.components.new()
     >>> component.product = product1
-    >>> component.parent_product = kit
     >>> component.quantity = 1
     >>> component = template.components.new()
     >>> component.product = product2
-    >>> component.parent_product = kit
-    >>> component.quantity = 1
-    >>> component.fixed = True
+    >>> component.quantity = 2
     >>> template.save()
 
-Components are copied when copying the template::
+Test duplicate copies components::
 
-    >>> template_copy, = template.duplicate()
-    >>> product_copy, = template.products
-    >>> len(template_copy.components)
-    2
-    >>> len(product_copy.components)
+    >>> duplicated, = template.duplicate()
+    >>> len(duplicated.components)
     2
+    >>> duplicated_product, = composed_product.duplicate()
+    >>> len(duplicated_product.components)
+    1
```

### Comparing `trytond_product_kit-7.0.3/tests/scenario_product_kit_duplicate.rst` & `trytond_product_kit-7.2.0/tests/scenario_product_kit_copy.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,86 +1,74 @@
-==============================
-Product Kit Duplicate Scenario
-==============================
+=========================
+Product Kit Copy Scenario
+=========================
 
 Imports::
 
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard
+
+    >>> from proteus import Model
+    >>> from trytond.modules.company.tests.tools import create_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
 
-Activate product_kit::
+Activate product_kit and stock::
 
     >>> config = activate_modules('product_kit')
 
-    >>> Uom = Model.get('product.uom')
-    >>> ProductTemplate = Model.get('product.template')
-    >>> Product = Model.get('product.product')
-
 Create company::
 
     >>> _ = create_company()
-    >>> company = get_company()
 
 Create products::
 
+    >>> Uom = Model.get('product.uom')
     >>> unit, = Uom.find([('name', '=', 'Unit')])
+    >>> meter, = Uom.find([('name', '=', "Meter")])
+    >>> ProductTemplate = Model.get('product.template')
+    >>> Product = Model.get('product.product')
+
     >>> template = ProductTemplate()
     >>> template.name = "Product 1"
     >>> template.default_uom = unit
     >>> template.type = 'goods'
     >>> template.save()
     >>> product1, = template.products
     >>> product1.cost_price = Decimal('10.0000')
     >>> product1.save()
 
     >>> template = ProductTemplate()
     >>> template.name = "Product 2"
-    >>> template.default_uom = unit
+    >>> template.default_uom = meter
     >>> template.type = 'goods'
     >>> template.save()
     >>> product2, = template.products
     >>> product2.cost_price = Decimal('20.0000')
     >>> product2.save()
 
-Create composed product::
-
-    >>> template = ProductTemplate()
-    >>> template.name = "Composed Product"
-    >>> template.default_uom = unit
-    >>> template.type = 'goods'
-    >>> template.save()
-    >>> composed_product, = template.products
-    >>> composed_product.cost_price = Decimal('10.0000')
-
-    >>> component = composed_product.components.new()
-    >>> component.product = product1
-    >>> component.quantity = 2
-    >>> composed_product.save()
-
 Create a kit::
 
     >>> template = ProductTemplate()
     >>> template.name = "Kit"
     >>> template.default_uom = unit
     >>> template.type = 'kit'
     >>> template.save()
     >>> kit, = template.products
 
     >>> component = template.components.new()
     >>> component.product = product1
+    >>> component.parent_product = kit
     >>> component.quantity = 1
     >>> component = template.components.new()
     >>> component.product = product2
-    >>> component.quantity = 2
+    >>> component.parent_product = kit
+    >>> component.quantity = 1
+    >>> component.fixed = True
     >>> template.save()
 
-Test duplicate copies components::
+Components are copied when copying the template::
 
-    >>> duplicated, = template.duplicate()
-    >>> len(duplicated.components)
+    >>> template_copy, = template.duplicate()
+    >>> product_copy, = template.products
+    >>> len(template_copy.components)
+    2
+    >>> len(product_copy.components)
     2
-    >>> duplicated_product, = composed_product.duplicate()
-    >>> len(duplicated_product.components)
-    1
```

### Comparing `trytond_product_kit-7.0.3/tests/scenario_product_kit_purchase.rst` & `trytond_product_kit-7.2.0/tests/scenario_product_kit_purchase.rst`

 * *Files 1% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 Purchase Product Kit Scenario
 =============================
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
+
+    >>> from proteus import Model
     >>> from trytond.modules.account.tests.tools import (
-    ...     create_fiscalyear, create_chart, get_accounts)
+    ...     create_chart, create_fiscalyear, get_accounts)
     >>> from trytond.modules.account_invoice.tests.tools import (
     ...     set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
+
     >>> today = dt.date.today()
 
 Activate product_kit, purchase and account_invoice::
 
     >>> config = activate_modules(
     ...     ['product_kit', 'purchase', 'account_invoice',
     ...         'account_invoice_stock'])
@@ -188,16 +189,15 @@
     >>> len(purchase.shipments), len(purchase.invoices)
     (0, 1)
 
 Check invoice::
 
     >>> invoice, = purchase.invoices
     >>> line, = invoice.lines
-    >>> line.product == service
-    True
+    >>> assertEqual(line.product, service)
 
 Check stock moves::
 
     >>> Move = Model.get('stock.move')
     >>> len(purchase.moves)
     4
     >>> len(Move.find([('purchase', '!=', None)]))
@@ -227,15 +227,15 @@
     ...     shipment.incoming_moves.append(incoming_move)
     >>> shipment.save()
 
     >>> product2move = {
     ...     m.product: m for m in shipment.incoming_moves}
     >>> product2move[product2].quantity = 2.0
     >>> shipment.click('receive')
-    >>> shipment.click('done')
+    >>> shipment.click('do')
     >>> shipment.state
     'done'
 
 Check new invoice::
 
     >>> purchase.reload()
     >>> _, invoice = purchase.invoices
```

### Comparing `trytond_product_kit-7.0.3/tests/scenario_product_kit_sale.rst` & `trytond_product_kit-7.2.0/tests/scenario_product_kit_sale.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 =========================
 Sale Product Kit Scenario
 =========================
 
 Imports::
 
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
+
+    >>> from proteus import Model
     >>> from trytond.modules.account.tests.tools import (
-    ...     create_fiscalyear, create_chart, get_accounts)
+    ...     create_chart, create_fiscalyear, get_accounts)
     >>> from trytond.modules.account_invoice.tests.tools import (
     ...     set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
 Activate product_kit, sale and account_invoice::
 
     >>> config = activate_modules(
     ...     ['product_kit', 'sale', 'account_invoice',
     ...         'account_invoice_stock'])
 
@@ -175,16 +175,15 @@
     >>> len(sale.shipments), len(sale.invoices)
     (1, 1)
 
 Check invoice::
 
     >>> invoice, = sale.invoices
     >>> line, = invoice.lines
-    >>> line.product == service
-    True
+    >>> assertEqual(line.product, service)
 
 Check shipment::
 
     >>> Move = Model.get('stock.move')
     >>> shipment, = sale.shipments
     >>> len(shipment.outgoing_moves)
     4
@@ -212,15 +211,15 @@
     >>> product2move = {
     ...     m.product: m for m in shipment.inventory_moves}
     >>> product2move[product1].quantity = 2.0
     >>> product2move[product2].quantity = 3.0
     >>> shipment.click('assign_force')
     >>> shipment.click('pick')
     >>> shipment.click('pack')
-    >>> shipment.click('done')
+    >>> shipment.click('do')
     >>> shipment.state
     'done'
 
 Check new invoice::
 
     >>> sale.reload()
     >>> _, invoice = sale.invoices
```

### Comparing `trytond_product_kit-7.0.3/tox.ini` & `trytond_product_kit-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_product_kit-7.0.3/trytond_product_kit.egg-info/PKG-INFO` & `trytond_product_kit-7.2.0/trytond_product_kit.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_product_kit
-Version: 7.0.3
+Version: 7.2.0
 Summary: Tryton module to manage product kits and components
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/modules-product-kit
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
@@ -46,26 +46,26 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account_invoice<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account_invoice_stock<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_company<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_purchase<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_purchase_amendment<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale_amendment<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_stock<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_invoice<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_invoice_stock<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_company<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_purchase<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_purchase_amendment<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_amendment<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_stock<7.3,>=7.2; extra == "test"
 
 ##################
 Product Kit Module
 ##################
 
 The *Product Kit Module* adds kits and components to products.
 This enables a defined set of products to be sold or purchased using a single
```

### Comparing `trytond_product_kit-7.0.3/trytond_product_kit.egg-info/SOURCES.txt` & `trytond_product_kit-7.2.0/trytond_product_kit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_product_kit-7.0.3/view/product_component_form.xml` & `trytond_product_kit-7.2.0/view/product_component_form.xml`

 * *Files identical despite different names*

