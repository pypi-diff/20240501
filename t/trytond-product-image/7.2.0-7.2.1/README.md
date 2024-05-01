# Comparing `tmp/trytond_product_image-7.2.0.tar.gz` & `tmp/trytond_product_image-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_product_image-7.2.0.tar", last modified: Mon Apr 29 15:43:07 2024, max compression
+gzip compressed data, was "trytond_product_image-7.2.1.tar", last modified: Wed May  1 11:53:34 2024, max compression
```

## Comparing `trytond_product_image-7.2.0.tar` & `trytond_product_image-7.2.1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:07.778537 trytond_product_image-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      783 2024-04-29 15:21:49.000000 trytond_product_image-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      651 2024-04-29 15:21:49.000000 trytond_product_image-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_product_image-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_product_image-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2530 2024-04-29 15:43:07.778537 trytond_product_image-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      202 2023-04-15 07:12:15.000000 trytond_product_image-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      653 2024-04-27 16:30:39.000000 trytond_product_image-7.2.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:07.775204 trytond_product_image-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3076 2024-04-27 16:30:39.000000 trytond_product_image-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1228 2024-03-17 11:01:36.000000 trytond_product_image-7.2.0/doc/configuration.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      627 2024-04-27 16:30:39.000000 trytond_product_image-7.2.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      202 2023-04-15 07:12:15.000000 trytond_product_image-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_product_image-7.2.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:15.000000 trytond_product_image-7.2.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:07.775204 trytond_product_image-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1304 2024-04-29 13:17:17.000000 trytond_product_image-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1545 2024-04-29 13:17:17.000000 trytond_product_image-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1304 2024-04-29 13:17:17.000000 trytond_product_image-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1468 2024-04-29 13:17:17.000000 trytond_product_image-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1499 2024-04-29 13:17:17.000000 trytond_product_image-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1304 2024-04-29 13:17:17.000000 trytond_product_image-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1304 2024-04-29 13:17:17.000000 trytond_product_image-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1304 2024-04-29 13:17:17.000000 trytond_product_image-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1304 2024-04-29 13:17:17.000000 trytond_product_image-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1524 2024-04-29 13:17:17.000000 trytond_product_image-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1334 2024-04-29 13:17:17.000000 trytond_product_image-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1304 2024-04-29 13:17:17.000000 trytond_product_image-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1312 2024-04-29 13:17:17.000000 trytond_product_image-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1304 2024-04-29 13:17:17.000000 trytond_product_image-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1304 2024-04-29 13:17:17.000000 trytond_product_image-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1542 2024-04-29 13:17:17.000000 trytond_product_image-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1304 2024-04-29 13:17:17.000000 trytond_product_image-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1304 2024-04-29 13:17:17.000000 trytond_product_image-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1304 2024-04-29 13:17:17.000000 trytond_product_image-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1304 2024-04-29 13:17:17.000000 trytond_product_image-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1498 2024-04-29 13:17:17.000000 trytond_product_image-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1304 2024-04-29 13:17:17.000000 trytond_product_image-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1304 2024-04-29 13:17:17.000000 trytond_product_image-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1304 2024-04-29 13:17:17.000000 trytond_product_image-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      380 2024-04-27 16:30:39.000000 trytond_product_image-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    10700 2024-04-29 13:17:17.000000 trytond_product_image-7.2.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2689 2024-04-27 16:30:39.000000 trytond_product_image-7.2.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2896 2024-04-27 16:30:39.000000 trytond_product_image-7.2.0/routes.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:43:07.778537 trytond_product_image-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4551 2024-04-27 16:30:39.000000 trytond_product_image-7.2.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:07.775204 trytond_product_image-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_product_image-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3646 2024-03-17 11:01:36.000000 trytond_product_image-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:15.000000 trytond_product_image-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       88 2024-04-29 15:21:45.000000 trytond_product_image-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:07.778537 trytond_product_image-7.2.0/trytond_product_image.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2530 2024-04-29 15:43:07.000000 trytond_product_image-7.2.0/trytond_product_image.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1800 2024-04-29 15:43:07.000000 trytond_product_image-7.2.0/trytond_product_image.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:43:07.000000 trytond_product_image-7.2.0/trytond_product_image.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       64 2024-04-29 15:43:07.000000 trytond_product_image-7.2.0/trytond_product_image.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:01.000000 trytond_product_image-7.2.0/trytond_product_image.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       59 2024-04-29 15:43:07.000000 trytond_product_image-7.2.0/trytond_product_image.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:43:07.000000 trytond_product_image-7.2.0/trytond_product_image.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:07.778537 trytond_product_image-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      366 2024-04-27 16:30:39.000000 trytond_product_image-7.2.0/view/category_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      603 2024-04-27 16:30:39.000000 trytond_product_image-7.2.0/view/category_image_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      283 2024-04-27 16:30:39.000000 trytond_product_image-7.2.0/view/category_image_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      333 2024-04-27 16:30:39.000000 trytond_product_image-7.2.0/view/category_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      667 2023-04-15 07:12:15.000000 trytond_product_image-7.2.0/view/image_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      322 2023-04-15 07:12:15.000000 trytond_product_image-7.2.0/view/image_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      366 2023-04-15 07:12:15.000000 trytond_product_image-7.2.0/view/template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      333 2023-04-15 07:12:15.000000 trytond_product_image-7.2.0/view/template_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:53:34.122695 trytond_product_image-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)      884 2024-05-01 11:53:30.000000 trytond_product_image-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      651 2024-05-01 11:53:30.000000 trytond_product_image-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:20:59.000000 trytond_product_image-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:20:59.000000 trytond_product_image-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2530 2024-05-01 11:53:34.122695 trytond_product_image-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      202 2024-04-30 17:20:59.000000 trytond_product_image-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      653 2024-04-30 17:20:59.000000 trytond_product_image-7.2.1/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:53:34.119362 trytond_product_image-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3076 2024-04-30 17:20:59.000000 trytond_product_image-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1228 2024-04-30 17:20:59.000000 trytond_product_image-7.2.1/doc/configuration.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      627 2024-04-30 17:20:59.000000 trytond_product_image-7.2.1/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      202 2024-04-30 17:20:59.000000 trytond_product_image-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-30 17:20:59.000000 trytond_product_image-7.2.1/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:20:59.000000 trytond_product_image-7.2.1/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:53:34.122695 trytond_product_image-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2316 2024-04-30 17:21:59.000000 trytond_product_image-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2715 2024-04-30 17:21:59.000000 trytond_product_image-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2316 2024-04-30 17:21:59.000000 trytond_product_image-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2622 2024-04-30 17:21:59.000000 trytond_product_image-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2661 2024-04-30 17:21:59.000000 trytond_product_image-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2316 2024-04-30 17:21:59.000000 trytond_product_image-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2316 2024-04-30 17:21:59.000000 trytond_product_image-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2316 2024-04-30 17:21:59.000000 trytond_product_image-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2316 2024-04-30 17:21:59.000000 trytond_product_image-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2689 2024-04-30 17:21:59.000000 trytond_product_image-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2436 2024-04-30 17:21:59.000000 trytond_product_image-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2316 2024-04-30 17:21:59.000000 trytond_product_image-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2324 2024-04-30 17:21:59.000000 trytond_product_image-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2316 2024-04-30 17:21:59.000000 trytond_product_image-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2316 2024-04-30 17:21:59.000000 trytond_product_image-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2750 2024-04-30 17:21:59.000000 trytond_product_image-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2316 2024-04-30 17:21:59.000000 trytond_product_image-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2316 2024-04-30 17:21:59.000000 trytond_product_image-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2316 2024-04-30 17:21:59.000000 trytond_product_image-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2316 2024-04-30 17:21:59.000000 trytond_product_image-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2678 2024-04-30 17:21:59.000000 trytond_product_image-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2316 2024-04-30 17:21:59.000000 trytond_product_image-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2316 2024-04-30 17:21:59.000000 trytond_product_image-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2316 2024-04-30 17:21:59.000000 trytond_product_image-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      380 2024-04-30 17:20:59.000000 trytond_product_image-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    10700 2024-04-30 17:20:59.000000 trytond_product_image-7.2.1/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2689 2024-04-30 17:20:59.000000 trytond_product_image-7.2.1/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2896 2024-04-30 17:20:59.000000 trytond_product_image-7.2.1/routes.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 11:53:34.122695 trytond_product_image-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4551 2024-04-30 17:20:59.000000 trytond_product_image-7.2.1/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:53:34.122695 trytond_product_image-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:20:59.000000 trytond_product_image-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3646 2024-04-30 17:20:59.000000 trytond_product_image-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:20:59.000000 trytond_product_image-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       88 2024-04-30 17:21:06.000000 trytond_product_image-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:53:34.122695 trytond_product_image-7.2.1/trytond_product_image.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2530 2024-05-01 11:53:33.000000 trytond_product_image-7.2.1/trytond_product_image.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1800 2024-05-01 11:53:34.000000 trytond_product_image-7.2.1/trytond_product_image.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:53:33.000000 trytond_product_image-7.2.1/trytond_product_image.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       64 2024-05-01 11:53:33.000000 trytond_product_image-7.2.1/trytond_product_image.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:53:33.000000 trytond_product_image-7.2.1/trytond_product_image.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       59 2024-05-01 11:53:33.000000 trytond_product_image-7.2.1/trytond_product_image.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 11:53:33.000000 trytond_product_image-7.2.1/trytond_product_image.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:53:34.122695 trytond_product_image-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      366 2024-04-30 17:20:59.000000 trytond_product_image-7.2.1/view/category_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      603 2024-04-30 17:20:59.000000 trytond_product_image-7.2.1/view/category_image_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      283 2024-04-30 17:20:59.000000 trytond_product_image-7.2.1/view/category_image_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      333 2024-04-30 17:20:59.000000 trytond_product_image-7.2.1/view/category_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      667 2024-04-30 17:20:59.000000 trytond_product_image-7.2.1/view/image_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      322 2024-04-30 17:20:59.000000 trytond_product_image-7.2.1/view/image_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      366 2024-04-30 17:20:59.000000 trytond_product_image-7.2.1/view/template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      333 2024-04-30 17:20:59.000000 trytond_product_image-7.2.1/view/template_list.xml
```

### Comparing `trytond_product_image-7.2.0/CHANGELOG` & `trytond_product_image-7.2.1/CHANGELOG`

 * *Files 20% similar despite different names*

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
 * Add images on product category
 * Preserve image ratio
 
 Version 7.0.0 - 2023-10-30
```

### Comparing `trytond_product_image-7.2.0/COPYRIGHT` & `trytond_product_image-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_product_image-7.2.0/LICENSE` & `trytond_product_image-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_product_image-7.2.0/PKG-INFO` & `trytond_product_image-7.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_product_image
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module that adds images to products
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_product_image-7.2.0/__init__.py` & `trytond_product_image-7.2.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_product_image-7.2.0/doc/conf.py` & `trytond_product_image-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_product_image-7.2.0/doc/configuration.rst` & `trytond_product_image-7.2.1/doc/configuration.rst`

 * *Files identical despite different names*

### Comparing `trytond_product_image-7.2.0/doc/design.rst` & `trytond_product_image-7.2.1/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_product_image-7.2.0/locale/bg.po` & `trytond_product_image-7.2.1/locale/sl.po`

 * *Files 21% similar despite different names*

```diff
@@ -1,71 +1,132 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
-msgctxt "field:product.image,cache:"
+#, fuzzy
+msgctxt "field:product.category,image_url:"
+msgid "Image URL"
+msgstr "URL podobe"
+
+#, fuzzy
+msgctxt "field:product.category,images:"
+msgid "Images"
+msgstr "Podobe"
+
+#, fuzzy
+msgctxt "field:product.category.image,cache:"
 msgid "Cache"
+msgstr "Predpomnilnik"
+
+msgctxt "field:product.category.image,category:"
+msgid "Category"
 msgstr ""
 
-msgctxt "field:product.image,image:"
+#, fuzzy
+msgctxt "field:product.category.image,image:"
 msgid "Image"
+msgstr "Podoba"
+
+#, fuzzy
+msgctxt "field:product.category.image,image_id:"
+msgid "Image ID"
+msgstr "ID podobe"
+
+msgctxt "field:product.category.image.cache,category_image:"
+msgid "Category Image"
 msgstr ""
 
-msgctxt "field:product.image,image_id:"
+msgctxt "field:product.category.image.cache,height:"
+msgid "Height"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:product.category.image.cache,image:"
+msgid "Image"
+msgstr "Podoba"
+
+#, fuzzy
+msgctxt "field:product.category.image.cache,image_id:"
 msgid "Image ID"
+msgstr "ID podobe"
+
+msgctxt "field:product.category.image.cache,width:"
+msgid "Width"
 msgstr ""
 
+msgctxt "field:product.image,cache:"
+msgid "Cache"
+msgstr "Predpomnilnik"
+
+msgctxt "field:product.image,image:"
+msgid "Image"
+msgstr "Podoba"
+
+msgctxt "field:product.image,image_id:"
+msgid "Image ID"
+msgstr "ID podobe"
+
 msgctxt "field:product.image,product:"
 msgid "Variant"
-msgstr ""
+msgstr "Različica"
 
 msgctxt "field:product.image,template:"
 msgid "Product"
-msgstr ""
+msgstr "Izdelek"
 
 msgctxt "field:product.image.cache,height:"
 msgid "Height"
 msgstr ""
 
 msgctxt "field:product.image.cache,image:"
 msgid "Image"
-msgstr ""
+msgstr "Podoba"
 
 msgctxt "field:product.image.cache,image_id:"
 msgid "Image ID"
-msgstr ""
+msgstr "ID podobe"
 
 msgctxt "field:product.image.cache,product_image:"
 msgid "Product Image"
-msgstr ""
+msgstr "Podoba produkta"
 
 msgctxt "field:product.image.cache,width:"
 msgid "Width"
 msgstr ""
 
 msgctxt "field:product.product,image_url:"
 msgid "Image URL"
-msgstr ""
+msgstr "URL podobe"
 
 msgctxt "field:product.product,images:"
 msgid "Images"
-msgstr ""
+msgstr "Podobe"
 
 msgctxt "field:product.template,image_url:"
 msgid "Image URL"
-msgstr ""
+msgstr "URL podobe"
 
 msgctxt "field:product.template,images:"
 msgid "Images"
-msgstr ""
+msgstr "Podobe"
+
+#, fuzzy
+msgctxt "model:ir.message,text:msg_image_cache_size_unique"
+msgid "The size of cached image must be unique."
+msgstr "Velikost podobe izdelka mora biti edinstvena."
 
-msgctxt "model:ir.message,text:msg_product_image_size_unique"
-msgid "The size of a product image must be unique."
+msgctxt "model:product.category.image,name:"
+msgid "Category Image"
 msgstr ""
 
+#, fuzzy
+msgctxt "model:product.category.image.cache,name:"
+msgid "Category Image Cache"
+msgstr "Predpomnilnik podobe izdelka"
+
 msgctxt "model:product.image,name:"
 msgid "Product Image"
-msgstr ""
+msgstr "Podoba izdelka"
 
 msgctxt "model:product.image.cache,name:"
 msgid "Product Image Cache"
-msgstr ""
+msgstr "Predpomnilnik podobe izdelka"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_product_image-7.2.0/locale/ca.po` & `trytond_product_image-7.2.1/locale/fr.po`

 * *Files 14% similar despite different names*

```diff
@@ -1,71 +1,123 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+msgctxt "field:product.category,image_url:"
+msgid "Image URL"
+msgstr "URL de l'image"
+
+msgctxt "field:product.category,images:"
+msgid "Images"
+msgstr "Images"
+
+msgctxt "field:product.category.image,cache:"
+msgid "Cache"
+msgstr "Cache"
+
+msgctxt "field:product.category.image,category:"
+msgid "Category"
+msgstr "Catégorie"
+
+msgctxt "field:product.category.image,image:"
+msgid "Image"
+msgstr "Image"
+
+msgctxt "field:product.category.image,image_id:"
+msgid "Image ID"
+msgstr "ID de l'image"
+
+msgctxt "field:product.category.image.cache,category_image:"
+msgid "Category Image"
+msgstr "Image de catégorie"
+
+msgctxt "field:product.category.image.cache,height:"
+msgid "Height"
+msgstr "Hauteur"
+
+msgctxt "field:product.category.image.cache,image:"
+msgid "Image"
+msgstr "Image"
+
+msgctxt "field:product.category.image.cache,image_id:"
+msgid "Image ID"
+msgstr "ID de l'image"
+
+msgctxt "field:product.category.image.cache,width:"
+msgid "Width"
+msgstr "Largeur"
+
 msgctxt "field:product.image,cache:"
 msgid "Cache"
-msgstr "Memòria cau"
+msgstr "Cache"
 
 msgctxt "field:product.image,image:"
 msgid "Image"
-msgstr "Imatge"
+msgstr "Image"
 
 msgctxt "field:product.image,image_id:"
 msgid "Image ID"
-msgstr "ID de la imatge"
+msgstr "ID de l'image"
 
 msgctxt "field:product.image,product:"
 msgid "Variant"
-msgstr "Variant"
+msgstr "Variante"
 
 msgctxt "field:product.image,template:"
 msgid "Product"
-msgstr "Producte"
+msgstr "Produit"
 
 msgctxt "field:product.image.cache,height:"
 msgid "Height"
-msgstr ""
+msgstr "Hauteur"
 
 msgctxt "field:product.image.cache,image:"
 msgid "Image"
-msgstr "Imatge"
+msgstr "Image"
 
 msgctxt "field:product.image.cache,image_id:"
 msgid "Image ID"
-msgstr "ID de la imatge"
+msgstr "ID de l'image"
 
 msgctxt "field:product.image.cache,product_image:"
 msgid "Product Image"
-msgstr "Imatge del producte"
+msgstr "Image du produit"
 
 msgctxt "field:product.image.cache,width:"
 msgid "Width"
-msgstr ""
+msgstr "Largeur"
 
 msgctxt "field:product.product,image_url:"
 msgid "Image URL"
-msgstr "URL de la imatge"
+msgstr "URL de l'image"
 
 msgctxt "field:product.product,images:"
 msgid "Images"
-msgstr "Imatges"
+msgstr "Images"
 
 msgctxt "field:product.template,image_url:"
 msgid "Image URL"
-msgstr "URL de la imatge"
+msgstr "URL de l'image"
 
 msgctxt "field:product.template,images:"
 msgid "Images"
-msgstr "Imatges"
+msgstr "Images"
 
-msgctxt "model:ir.message,text:msg_product_image_size_unique"
-msgid "The size of a product image must be unique."
-msgstr "La mida d'una imatge de producte ha de ser única."
+msgctxt "model:ir.message,text:msg_image_cache_size_unique"
+msgid "The size of cached image must be unique."
+msgstr "La taille de l'image mise en cache doit être unique."
+
+msgctxt "model:product.category.image,name:"
+msgid "Category Image"
+msgstr "Image de catégorie"
+
+msgctxt "model:product.category.image.cache,name:"
+msgid "Category Image Cache"
+msgstr "Cache d'images de catégorie"
 
 msgctxt "model:product.image,name:"
 msgid "Product Image"
-msgstr "Imatge del producte"
+msgstr "Image du produit"
 
 msgctxt "model:product.image.cache,name:"
 msgid "Product Image Cache"
-msgstr "Memòria cau de la imatge del producte"
+msgstr "Cache de l'image du produit"
```

### Comparing `trytond_product_image-7.2.0/locale/cs.po` & `trytond_product_image-7.2.1/locale/de.po`

 * *Files 23% similar despite different names*

```diff
@@ -1,71 +1,124 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+msgctxt "field:product.category,image_url:"
+msgid "Image URL"
+msgstr "Bild-URL"
+
+msgctxt "field:product.category,images:"
+msgid "Images"
+msgstr "Bilder"
+
+msgctxt "field:product.category.image,cache:"
+msgid "Cache"
+msgstr "Cache"
+
+msgctxt "field:product.category.image,category:"
+msgid "Category"
+msgstr "Kategorie"
+
+msgctxt "field:product.category.image,image:"
+msgid "Image"
+msgstr "Bild"
+
+msgctxt "field:product.category.image,image_id:"
+msgid "Image ID"
+msgstr "Bild-ID"
+
+msgctxt "field:product.category.image.cache,category_image:"
+msgid "Category Image"
+msgstr "Kategoriebild"
+
+msgctxt "field:product.category.image.cache,height:"
+msgid "Height"
+msgstr "Höhe"
+
+msgctxt "field:product.category.image.cache,image:"
+msgid "Image"
+msgstr "Bild"
+
+msgctxt "field:product.category.image.cache,image_id:"
+msgid "Image ID"
+msgstr "Bild-ID"
+
+msgctxt "field:product.category.image.cache,width:"
+msgid "Width"
+msgstr "Breite"
+
 msgctxt "field:product.image,cache:"
 msgid "Cache"
-msgstr ""
+msgstr "Cache"
 
 msgctxt "field:product.image,image:"
 msgid "Image"
-msgstr ""
+msgstr "Bild"
 
 msgctxt "field:product.image,image_id:"
 msgid "Image ID"
-msgstr ""
+msgstr "Bild ID"
 
 msgctxt "field:product.image,product:"
 msgid "Variant"
-msgstr ""
+msgstr "Variante"
 
 msgctxt "field:product.image,template:"
 msgid "Product"
-msgstr ""
+msgstr "Artikel"
 
 msgctxt "field:product.image.cache,height:"
 msgid "Height"
-msgstr ""
+msgstr "Höhe"
 
 msgctxt "field:product.image.cache,image:"
 msgid "Image"
-msgstr ""
+msgstr "Bild"
 
 msgctxt "field:product.image.cache,image_id:"
 msgid "Image ID"
-msgstr ""
+msgstr "Bild ID"
 
 msgctxt "field:product.image.cache,product_image:"
 msgid "Product Image"
-msgstr ""
+msgstr "Artikelbild"
 
 msgctxt "field:product.image.cache,width:"
 msgid "Width"
-msgstr ""
+msgstr "Breite"
 
 msgctxt "field:product.product,image_url:"
 msgid "Image URL"
-msgstr ""
+msgstr "Bild-URL"
 
 msgctxt "field:product.product,images:"
 msgid "Images"
-msgstr ""
+msgstr "Bilder"
 
 msgctxt "field:product.template,image_url:"
 msgid "Image URL"
-msgstr ""
+msgstr "Bild-URL"
 
 msgctxt "field:product.template,images:"
 msgid "Images"
-msgstr ""
+msgstr "Bilder"
 
-msgctxt "model:ir.message,text:msg_product_image_size_unique"
-msgid "The size of a product image must be unique."
+msgctxt "model:ir.message,text:msg_image_cache_size_unique"
+msgid "The size of cached image must be unique."
 msgstr ""
+"Die Größe für zwischengespeicherte Bilder kann nur einmal vergeben werden."
+
+msgctxt "model:product.category.image,name:"
+msgid "Category Image"
+msgstr "Kategoriebild"
+
+msgctxt "model:product.category.image.cache,name:"
+msgid "Category Image Cache"
+msgstr "Kategoriebild Cache"
 
 msgctxt "model:product.image,name:"
 msgid "Product Image"
-msgstr ""
+msgstr "Artikelbild"
 
 msgctxt "model:product.image.cache,name:"
 msgid "Product Image Cache"
-msgstr ""
+msgstr "Artikelbild Cache"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_product_image-7.2.0/locale/de.po` & `trytond_product_image-7.2.1/locale/hu.po`

 * *Files 22% similar despite different names*

```diff
@@ -1,71 +1,129 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+#, fuzzy
+msgctxt "field:product.category,image_url:"
+msgid "Image URL"
+msgstr "Képek"
+
+#, fuzzy
+msgctxt "field:product.category,images:"
+msgid "Images"
+msgstr "Képek"
+
+msgctxt "field:product.category.image,cache:"
+msgid "Cache"
+msgstr ""
+
+msgctxt "field:product.category.image,category:"
+msgid "Category"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:product.category.image,image:"
+msgid "Image"
+msgstr "Képek"
+
+#, fuzzy
+msgctxt "field:product.category.image,image_id:"
+msgid "Image ID"
+msgstr "Képek"
+
+msgctxt "field:product.category.image.cache,category_image:"
+msgid "Category Image"
+msgstr ""
+
+msgctxt "field:product.category.image.cache,height:"
+msgid "Height"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:product.category.image.cache,image:"
+msgid "Image"
+msgstr "Képek"
+
+#, fuzzy
+msgctxt "field:product.category.image.cache,image_id:"
+msgid "Image ID"
+msgstr "Képek"
+
+msgctxt "field:product.category.image.cache,width:"
+msgid "Width"
+msgstr ""
+
 msgctxt "field:product.image,cache:"
 msgid "Cache"
-msgstr "Cache"
+msgstr ""
 
 msgctxt "field:product.image,image:"
 msgid "Image"
-msgstr "Bild"
+msgstr ""
 
 msgctxt "field:product.image,image_id:"
 msgid "Image ID"
-msgstr "Bild ID"
+msgstr ""
 
 msgctxt "field:product.image,product:"
 msgid "Variant"
-msgstr "Variante"
+msgstr ""
 
 msgctxt "field:product.image,template:"
 msgid "Product"
-msgstr "Artikel"
+msgstr "Termék"
 
 msgctxt "field:product.image.cache,height:"
 msgid "Height"
 msgstr ""
 
 msgctxt "field:product.image.cache,image:"
 msgid "Image"
-msgstr "Bild"
+msgstr ""
 
 msgctxt "field:product.image.cache,image_id:"
 msgid "Image ID"
-msgstr "Bild ID"
+msgstr ""
 
 msgctxt "field:product.image.cache,product_image:"
 msgid "Product Image"
-msgstr "Artikelbild"
+msgstr "Termékkép"
 
 msgctxt "field:product.image.cache,width:"
 msgid "Width"
 msgstr ""
 
 msgctxt "field:product.product,image_url:"
 msgid "Image URL"
-msgstr "Bild-URL"
+msgstr ""
 
 msgctxt "field:product.product,images:"
 msgid "Images"
-msgstr "Bilder"
+msgstr "Képek"
 
 msgctxt "field:product.template,image_url:"
 msgid "Image URL"
-msgstr "Bild-URL"
+msgstr ""
 
 msgctxt "field:product.template,images:"
 msgid "Images"
-msgstr "Bilder"
+msgstr "Képek"
+
+msgctxt "model:ir.message,text:msg_image_cache_size_unique"
+msgid "The size of cached image must be unique."
+msgstr ""
 
-msgctxt "model:ir.message,text:msg_product_image_size_unique"
-msgid "The size of a product image must be unique."
-msgstr "Es kann nur einen Bildgrößendatensatz pro Bild geben."
+msgctxt "model:product.category.image,name:"
+msgid "Category Image"
+msgstr ""
+
+msgctxt "model:product.category.image.cache,name:"
+msgid "Category Image Cache"
+msgstr ""
 
 msgctxt "model:product.image,name:"
 msgid "Product Image"
-msgstr "Artikelbild"
+msgstr ""
 
 msgctxt "model:product.image.cache,name:"
 msgid "Product Image Cache"
-msgstr "Artikelbild Cache"
+msgstr ""
```

### Comparing `trytond_product_image-7.2.0/locale/es.po` & `trytond_product_image-7.2.1/locale/bg.po`

 * *Files 14% similar despite different names*

```diff
@@ -1,71 +1,123 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+msgctxt "field:product.category,image_url:"
+msgid "Image URL"
+msgstr ""
+
+msgctxt "field:product.category,images:"
+msgid "Images"
+msgstr ""
+
+msgctxt "field:product.category.image,cache:"
+msgid "Cache"
+msgstr ""
+
+msgctxt "field:product.category.image,category:"
+msgid "Category"
+msgstr ""
+
+msgctxt "field:product.category.image,image:"
+msgid "Image"
+msgstr ""
+
+msgctxt "field:product.category.image,image_id:"
+msgid "Image ID"
+msgstr ""
+
+msgctxt "field:product.category.image.cache,category_image:"
+msgid "Category Image"
+msgstr ""
+
+msgctxt "field:product.category.image.cache,height:"
+msgid "Height"
+msgstr ""
+
+msgctxt "field:product.category.image.cache,image:"
+msgid "Image"
+msgstr ""
+
+msgctxt "field:product.category.image.cache,image_id:"
+msgid "Image ID"
+msgstr ""
+
+msgctxt "field:product.category.image.cache,width:"
+msgid "Width"
+msgstr ""
+
 msgctxt "field:product.image,cache:"
 msgid "Cache"
-msgstr "Caché"
+msgstr ""
 
 msgctxt "field:product.image,image:"
 msgid "Image"
-msgstr "Imagen"
+msgstr ""
 
 msgctxt "field:product.image,image_id:"
 msgid "Image ID"
-msgstr "ID Imagen"
+msgstr ""
 
 msgctxt "field:product.image,product:"
 msgid "Variant"
-msgstr "Variante"
+msgstr ""
 
 msgctxt "field:product.image,template:"
 msgid "Product"
-msgstr "Producto"
+msgstr ""
 
 msgctxt "field:product.image.cache,height:"
 msgid "Height"
 msgstr ""
 
 msgctxt "field:product.image.cache,image:"
 msgid "Image"
-msgstr "Imagen"
+msgstr ""
 
 msgctxt "field:product.image.cache,image_id:"
 msgid "Image ID"
-msgstr "ID Imagen"
+msgstr ""
 
 msgctxt "field:product.image.cache,product_image:"
 msgid "Product Image"
-msgstr "Imagen producto"
+msgstr ""
 
 msgctxt "field:product.image.cache,width:"
 msgid "Width"
 msgstr ""
 
 msgctxt "field:product.product,image_url:"
 msgid "Image URL"
-msgstr "URL Imagen"
+msgstr ""
 
 msgctxt "field:product.product,images:"
 msgid "Images"
-msgstr "Imágenes"
+msgstr ""
 
 msgctxt "field:product.template,image_url:"
 msgid "Image URL"
-msgstr "URL Imagen"
+msgstr ""
 
 msgctxt "field:product.template,images:"
 msgid "Images"
-msgstr "Imágenes"
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_image_cache_size_unique"
+msgid "The size of cached image must be unique."
+msgstr ""
+
+msgctxt "model:product.category.image,name:"
+msgid "Category Image"
+msgstr ""
 
-msgctxt "model:ir.message,text:msg_product_image_size_unique"
-msgid "The size of a product image must be unique."
-msgstr "El tamaño de una imagen de producto debe ser único."
+msgctxt "model:product.category.image.cache,name:"
+msgid "Category Image Cache"
+msgstr ""
 
 msgctxt "model:product.image,name:"
 msgid "Product Image"
-msgstr "Imagen producto"
+msgstr ""
 
 msgctxt "model:product.image.cache,name:"
 msgid "Product Image Cache"
-msgstr "Caché imagen producto"
+msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_product_image-7.2.0/locale/es_419.po` & `trytond_product_image-7.2.1/locale/es.po`

 * *Files 27% similar despite different names*

```diff
@@ -1,71 +1,123 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+msgctxt "field:product.category,image_url:"
+msgid "Image URL"
+msgstr "URL Imagen"
+
+msgctxt "field:product.category,images:"
+msgid "Images"
+msgstr "Imágenes"
+
+msgctxt "field:product.category.image,cache:"
+msgid "Cache"
+msgstr "Caché"
+
+msgctxt "field:product.category.image,category:"
+msgid "Category"
+msgstr "Categoría"
+
+msgctxt "field:product.category.image,image:"
+msgid "Image"
+msgstr "Imagen"
+
+msgctxt "field:product.category.image,image_id:"
+msgid "Image ID"
+msgstr "ID de la Imagen"
+
+msgctxt "field:product.category.image.cache,category_image:"
+msgid "Category Image"
+msgstr "Imagen Categoría"
+
+msgctxt "field:product.category.image.cache,height:"
+msgid "Height"
+msgstr "Alto"
+
+msgctxt "field:product.category.image.cache,image:"
+msgid "Image"
+msgstr "Imagen"
+
+msgctxt "field:product.category.image.cache,image_id:"
+msgid "Image ID"
+msgstr "ID de la Imagen"
+
+msgctxt "field:product.category.image.cache,width:"
+msgid "Width"
+msgstr "Ancho"
+
 msgctxt "field:product.image,cache:"
 msgid "Cache"
-msgstr ""
+msgstr "Caché"
 
 msgctxt "field:product.image,image:"
 msgid "Image"
-msgstr ""
+msgstr "Imagen"
 
 msgctxt "field:product.image,image_id:"
 msgid "Image ID"
-msgstr ""
+msgstr "ID Imagen"
 
 msgctxt "field:product.image,product:"
 msgid "Variant"
-msgstr ""
+msgstr "Variante"
 
 msgctxt "field:product.image,template:"
 msgid "Product"
-msgstr ""
+msgstr "Producto"
 
 msgctxt "field:product.image.cache,height:"
 msgid "Height"
-msgstr ""
+msgstr "Alto"
 
 msgctxt "field:product.image.cache,image:"
 msgid "Image"
-msgstr ""
+msgstr "Imagen"
 
 msgctxt "field:product.image.cache,image_id:"
 msgid "Image ID"
-msgstr ""
+msgstr "ID Imagen"
 
 msgctxt "field:product.image.cache,product_image:"
 msgid "Product Image"
-msgstr ""
+msgstr "Imagen producto"
 
 msgctxt "field:product.image.cache,width:"
 msgid "Width"
-msgstr ""
+msgstr "Ancho"
 
 msgctxt "field:product.product,image_url:"
 msgid "Image URL"
-msgstr ""
+msgstr "URL Imagen"
 
 msgctxt "field:product.product,images:"
 msgid "Images"
-msgstr ""
+msgstr "Imágenes"
 
 msgctxt "field:product.template,image_url:"
 msgid "Image URL"
-msgstr ""
+msgstr "URL Imagen"
 
 msgctxt "field:product.template,images:"
 msgid "Images"
-msgstr ""
+msgstr "Imágenes"
 
-msgctxt "model:ir.message,text:msg_product_image_size_unique"
-msgid "The size of a product image must be unique."
-msgstr ""
+msgctxt "model:ir.message,text:msg_image_cache_size_unique"
+msgid "The size of cached image must be unique."
+msgstr "El tamaño de una imagen en cache debe ser único."
+
+msgctxt "model:product.category.image,name:"
+msgid "Category Image"
+msgstr "Imagen Categoría"
+
+msgctxt "model:product.category.image.cache,name:"
+msgid "Category Image Cache"
+msgstr "Caché imagen categoría"
 
 msgctxt "model:product.image,name:"
 msgid "Product Image"
-msgstr ""
+msgstr "Imagen producto"
 
 msgctxt "model:product.image.cache,name:"
 msgid "Product Image Cache"
-msgstr ""
+msgstr "Caché imagen producto"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_product_image-7.2.0/locale/fr.po` & `trytond_product_image-7.2.1/locale/cs.po`

 * *Files 26% similar despite different names*

```diff
@@ -1,71 +1,123 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+msgctxt "field:product.category,image_url:"
+msgid "Image URL"
+msgstr ""
+
+msgctxt "field:product.category,images:"
+msgid "Images"
+msgstr ""
+
+msgctxt "field:product.category.image,cache:"
+msgid "Cache"
+msgstr ""
+
+msgctxt "field:product.category.image,category:"
+msgid "Category"
+msgstr ""
+
+msgctxt "field:product.category.image,image:"
+msgid "Image"
+msgstr ""
+
+msgctxt "field:product.category.image,image_id:"
+msgid "Image ID"
+msgstr ""
+
+msgctxt "field:product.category.image.cache,category_image:"
+msgid "Category Image"
+msgstr ""
+
+msgctxt "field:product.category.image.cache,height:"
+msgid "Height"
+msgstr ""
+
+msgctxt "field:product.category.image.cache,image:"
+msgid "Image"
+msgstr ""
+
+msgctxt "field:product.category.image.cache,image_id:"
+msgid "Image ID"
+msgstr ""
+
+msgctxt "field:product.category.image.cache,width:"
+msgid "Width"
+msgstr ""
+
 msgctxt "field:product.image,cache:"
 msgid "Cache"
-msgstr "Cache"
+msgstr ""
 
 msgctxt "field:product.image,image:"
 msgid "Image"
-msgstr "Image"
+msgstr ""
 
 msgctxt "field:product.image,image_id:"
 msgid "Image ID"
-msgstr "ID de l'image"
+msgstr ""
 
 msgctxt "field:product.image,product:"
 msgid "Variant"
-msgstr "Variante"
+msgstr ""
 
 msgctxt "field:product.image,template:"
 msgid "Product"
-msgstr "Produit"
+msgstr ""
 
 msgctxt "field:product.image.cache,height:"
 msgid "Height"
-msgstr "Hauteur"
+msgstr ""
 
 msgctxt "field:product.image.cache,image:"
 msgid "Image"
-msgstr "Image"
+msgstr ""
 
 msgctxt "field:product.image.cache,image_id:"
 msgid "Image ID"
-msgstr "ID de l'image"
+msgstr ""
 
 msgctxt "field:product.image.cache,product_image:"
 msgid "Product Image"
-msgstr "Image du produit"
+msgstr ""
 
 msgctxt "field:product.image.cache,width:"
 msgid "Width"
-msgstr "Largeur"
+msgstr ""
 
 msgctxt "field:product.product,image_url:"
 msgid "Image URL"
-msgstr "URL de l'image"
+msgstr ""
 
 msgctxt "field:product.product,images:"
 msgid "Images"
-msgstr "Images"
+msgstr ""
 
 msgctxt "field:product.template,image_url:"
 msgid "Image URL"
-msgstr "URL de l'image"
+msgstr ""
 
 msgctxt "field:product.template,images:"
 msgid "Images"
-msgstr "Images"
+msgstr ""
 
-msgctxt "model:ir.message,text:msg_product_image_size_unique"
-msgid "The size of a product image must be unique."
-msgstr "La taille d'une image de produit doit être unique."
+msgctxt "model:ir.message,text:msg_image_cache_size_unique"
+msgid "The size of cached image must be unique."
+msgstr ""
+
+msgctxt "model:product.category.image,name:"
+msgid "Category Image"
+msgstr ""
+
+msgctxt "model:product.category.image.cache,name:"
+msgid "Category Image Cache"
+msgstr ""
 
 msgctxt "model:product.image,name:"
 msgid "Product Image"
-msgstr "Image du produit"
+msgstr ""
 
 msgctxt "model:product.image.cache,name:"
 msgid "Product Image Cache"
-msgstr "Cache de l'image du produit"
+msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_product_image-7.2.0/locale/nl.po` & `trytond_product_image-7.2.1/locale/es_419.po`

 * *Files 27% similar despite different names*

```diff
@@ -1,71 +1,123 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+msgctxt "field:product.category,image_url:"
+msgid "Image URL"
+msgstr ""
+
+msgctxt "field:product.category,images:"
+msgid "Images"
+msgstr ""
+
+msgctxt "field:product.category.image,cache:"
+msgid "Cache"
+msgstr ""
+
+msgctxt "field:product.category.image,category:"
+msgid "Category"
+msgstr ""
+
+msgctxt "field:product.category.image,image:"
+msgid "Image"
+msgstr ""
+
+msgctxt "field:product.category.image,image_id:"
+msgid "Image ID"
+msgstr ""
+
+msgctxt "field:product.category.image.cache,category_image:"
+msgid "Category Image"
+msgstr ""
+
+msgctxt "field:product.category.image.cache,height:"
+msgid "Height"
+msgstr ""
+
+msgctxt "field:product.category.image.cache,image:"
+msgid "Image"
+msgstr ""
+
+msgctxt "field:product.category.image.cache,image_id:"
+msgid "Image ID"
+msgstr ""
+
+msgctxt "field:product.category.image.cache,width:"
+msgid "Width"
+msgstr ""
+
 msgctxt "field:product.image,cache:"
 msgid "Cache"
-msgstr "Cache"
+msgstr ""
 
 msgctxt "field:product.image,image:"
 msgid "Image"
-msgstr "Afbeelding"
+msgstr ""
 
 msgctxt "field:product.image,image_id:"
 msgid "Image ID"
-msgstr "Afbeeldings-ID"
+msgstr ""
 
 msgctxt "field:product.image,product:"
 msgid "Variant"
-msgstr "Variant"
+msgstr ""
 
 msgctxt "field:product.image,template:"
 msgid "Product"
-msgstr "Product"
+msgstr ""
 
 msgctxt "field:product.image.cache,height:"
 msgid "Height"
 msgstr ""
 
 msgctxt "field:product.image.cache,image:"
 msgid "Image"
-msgstr "Afbeelding"
+msgstr ""
 
 msgctxt "field:product.image.cache,image_id:"
 msgid "Image ID"
-msgstr "Afbeeldings-ID"
+msgstr ""
 
 msgctxt "field:product.image.cache,product_image:"
 msgid "Product Image"
-msgstr "Product afbeelding"
+msgstr ""
 
 msgctxt "field:product.image.cache,width:"
 msgid "Width"
 msgstr ""
 
 msgctxt "field:product.product,image_url:"
 msgid "Image URL"
-msgstr "Afbeelding URL"
+msgstr ""
 
 msgctxt "field:product.product,images:"
 msgid "Images"
-msgstr "Afbeeldingen"
+msgstr ""
 
 msgctxt "field:product.template,image_url:"
 msgid "Image URL"
-msgstr "Afbeelding URL"
+msgstr ""
 
 msgctxt "field:product.template,images:"
 msgid "Images"
-msgstr "Afbeeldingen"
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_image_cache_size_unique"
+msgid "The size of cached image must be unique."
+msgstr ""
+
+msgctxt "model:product.category.image,name:"
+msgid "Category Image"
+msgstr ""
 
-msgctxt "model:ir.message,text:msg_product_image_size_unique"
-msgid "The size of a product image must be unique."
-msgstr "De grootte van een product afbeelding moet uniek zijn."
+msgctxt "model:product.category.image.cache,name:"
+msgid "Category Image Cache"
+msgstr ""
 
 msgctxt "model:product.image,name:"
 msgid "Product Image"
-msgstr "Product afbeelding"
+msgstr ""
 
 msgctxt "model:product.image.cache,name:"
 msgid "Product Image Cache"
-msgstr "Cache van productafbeeldingen"
+msgstr ""
```

### Comparing `trytond_product_image-7.2.0/product.py` & `trytond_product_image-7.2.1/product.py`

 * *Files identical despite different names*

### Comparing `trytond_product_image-7.2.0/product.xml` & `trytond_product_image-7.2.1/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_product_image-7.2.0/routes.py` & `trytond_product_image-7.2.1/routes.py`

 * *Files identical despite different names*

### Comparing `trytond_product_image-7.2.0/setup.py` & `trytond_product_image-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_product_image-7.2.0/tests/test_module.py` & `trytond_product_image-7.2.1/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_product_image-7.2.0/tox.ini` & `trytond_product_image-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_product_image-7.2.0/trytond_product_image.egg-info/PKG-INFO` & `trytond_product_image-7.2.1/trytond_product_image.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_product_image
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module that adds images to products
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_product_image-7.2.0/trytond_product_image.egg-info/SOURCES.txt` & `trytond_product_image-7.2.1/trytond_product_image.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_product_image-7.2.0/view/category_image_form.xml` & `trytond_product_image-7.2.1/view/category_image_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_product_image-7.2.0/view/image_form.xml` & `trytond_product_image-7.2.1/view/image_form.xml`

 * *Files identical despite different names*

