# Comparing `tmp/trytond_product_attribute-7.2.0.tar.gz` & `tmp/trytond_product_attribute-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_product_attribute-7.2.0.tar", last modified: Mon Apr 29 15:42:28 2024, max compression
+gzip compressed data, was "trytond_product_attribute-7.2.1.tar", last modified: Wed May  1 11:54:38 2024, max compression
```

## Comparing `trytond_product_attribute-7.2.0.tar` & `trytond_product_attribute-7.2.1.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:28.626227 trytond_product_attribute-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     2061 2024-04-29 15:21:19.000000 trytond_product_attribute-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-04-29 15:21:18.000000 trytond_product_attribute-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_product_attribute-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_product_attribute-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2745 2024-04-29 15:42:28.626227 trytond_product_attribute-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      372 2023-01-16 14:00:20.000000 trytond_product_attribute-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      433 2023-04-15 07:12:15.000000 trytond_product_attribute-7.2.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:28.619561 trytond_product_attribute-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3080 2024-04-27 16:30:39.000000 trytond_product_attribute-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      372 2023-01-16 14:00:20.000000 trytond_product_attribute-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:14.000000 trytond_product_attribute-7.2.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:28.622894 trytond_product_attribute-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     2381 2024-04-27 16:43:24.000000 trytond_product_attribute-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2652 2024-04-27 16:43:24.000000 trytond_product_attribute-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2351 2024-04-27 16:43:24.000000 trytond_product_attribute-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2673 2024-04-27 16:43:24.000000 trytond_product_attribute-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2708 2024-04-27 16:43:24.000000 trytond_product_attribute-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2149 2024-04-27 16:43:24.000000 trytond_product_attribute-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2293 2024-04-27 16:43:24.000000 trytond_product_attribute-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2923 2024-04-27 16:43:24.000000 trytond_product_attribute-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2338 2024-04-27 16:43:24.000000 trytond_product_attribute-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2721 2024-04-27 16:43:24.000000 trytond_product_attribute-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2781 2024-04-27 16:43:24.000000 trytond_product_attribute-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2153 2024-04-27 16:43:24.000000 trytond_product_attribute-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2348 2024-04-27 16:43:24.000000 trytond_product_attribute-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2356 2024-04-27 16:43:24.000000 trytond_product_attribute-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2661 2024-04-27 16:43:24.000000 trytond_product_attribute-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2737 2024-04-27 16:43:24.000000 trytond_product_attribute-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2635 2024-04-27 16:43:24.000000 trytond_product_attribute-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2683 2024-04-27 16:43:24.000000 trytond_product_attribute-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2149 2024-04-27 16:43:24.000000 trytond_product_attribute-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2428 2024-04-27 16:43:24.000000 trytond_product_attribute-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2346 2024-04-27 16:43:24.000000 trytond_product_attribute-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2404 2024-04-27 16:43:24.000000 trytond_product_attribute-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2149 2024-04-27 16:43:24.000000 trytond_product_attribute-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2383 2024-04-27 16:43:24.000000 trytond_product_attribute-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      348 2023-04-15 07:12:15.000000 trytond_product_attribute-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3085 2023-04-15 07:12:15.000000 trytond_product_attribute-7.2.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5959 2024-04-27 16:30:39.000000 trytond_product_attribute-7.2.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:42:28.626227 trytond_product_attribute-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4307 2024-03-17 11:01:36.000000 trytond_product_attribute-7.2.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:28.622894 trytond_product_attribute-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_product_attribute-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      329 2023-04-15 07:12:15.000000 trytond_product_attribute-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:14.000000 trytond_product_attribute-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       88 2024-04-29 15:21:14.000000 trytond_product_attribute-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:28.626227 trytond_product_attribute-7.2.0/trytond_product_attribute.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2745 2024-04-29 15:42:28.000000 trytond_product_attribute-7.2.0/trytond_product_attribute.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1824 2024-04-29 15:42:28.000000 trytond_product_attribute-7.2.0/trytond_product_attribute.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:42:28.000000 trytond_product_attribute-7.2.0/trytond_product_attribute.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       72 2024-04-29 15:42:28.000000 trytond_product_attribute-7.2.0/trytond_product_attribute.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:58.000000 trytond_product_attribute-7.2.0/trytond_product_attribute.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       44 2024-04-29 15:42:28.000000 trytond_product_attribute-7.2.0/trytond_product_attribute.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:42:28.000000 trytond_product_attribute-7.2.0/trytond_product_attribute.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:28.626227 trytond_product_attribute-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      789 2023-04-15 07:12:15.000000 trytond_product_attribute-7.2.0/view/attribute_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      294 2023-04-15 07:12:15.000000 trytond_product_attribute-7.2.0/view/attribute_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-04-15 07:12:15.000000 trytond_product_attribute-7.2.0/view/attribute_list_simple.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      328 2023-04-15 07:12:15.000000 trytond_product_attribute-7.2.0/view/attribute_set_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-01-16 14:00:20.000000 trytond_product_attribute-7.2.0/view/attribute_set_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      522 2023-04-15 07:12:15.000000 trytond_product_attribute-7.2.0/view/product_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      455 2023-04-15 07:12:15.000000 trytond_product_attribute-7.2.0/view/product_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      402 2023-01-16 14:00:20.000000 trytond_product_attribute-7.2.0/view/template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      308 2023-04-15 07:12:15.000000 trytond_product_attribute-7.2.0/view/template_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:54:38.677673 trytond_product_attribute-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2162 2024-05-01 11:54:35.000000 trytond_product_attribute-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-05-01 11:54:35.000000 trytond_product_attribute-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:20:59.000000 trytond_product_attribute-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:20:59.000000 trytond_product_attribute-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2745 2024-05-01 11:54:38.677673 trytond_product_attribute-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      372 2024-04-30 17:20:59.000000 trytond_product_attribute-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      433 2024-04-30 17:20:59.000000 trytond_product_attribute-7.2.1/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:54:38.674340 trytond_product_attribute-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3080 2024-04-30 17:20:59.000000 trytond_product_attribute-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      372 2024-04-30 17:20:59.000000 trytond_product_attribute-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:20:59.000000 trytond_product_attribute-7.2.1/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:54:38.677673 trytond_product_attribute-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2381 2024-04-30 17:20:59.000000 trytond_product_attribute-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2652 2024-04-30 17:20:59.000000 trytond_product_attribute-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2351 2024-04-30 17:20:59.000000 trytond_product_attribute-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2673 2024-04-30 17:20:59.000000 trytond_product_attribute-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2708 2024-04-30 17:20:59.000000 trytond_product_attribute-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2149 2024-04-30 17:20:59.000000 trytond_product_attribute-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2293 2024-04-30 17:20:59.000000 trytond_product_attribute-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2923 2024-04-30 17:20:59.000000 trytond_product_attribute-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2338 2024-04-30 17:20:59.000000 trytond_product_attribute-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2721 2024-04-30 17:20:59.000000 trytond_product_attribute-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2781 2024-04-30 17:20:59.000000 trytond_product_attribute-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2153 2024-04-30 17:20:59.000000 trytond_product_attribute-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2348 2024-04-30 17:20:59.000000 trytond_product_attribute-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2356 2024-04-30 17:20:59.000000 trytond_product_attribute-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2661 2024-04-30 17:20:59.000000 trytond_product_attribute-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2737 2024-04-30 17:20:59.000000 trytond_product_attribute-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2652 2024-04-30 17:21:59.000000 trytond_product_attribute-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2683 2024-04-30 17:20:59.000000 trytond_product_attribute-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2149 2024-04-30 17:20:59.000000 trytond_product_attribute-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2428 2024-04-30 17:20:59.000000 trytond_product_attribute-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2346 2024-04-30 17:20:59.000000 trytond_product_attribute-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2404 2024-04-30 17:20:59.000000 trytond_product_attribute-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2149 2024-04-30 17:20:59.000000 trytond_product_attribute-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2383 2024-04-30 17:20:59.000000 trytond_product_attribute-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      348 2024-04-30 17:20:59.000000 trytond_product_attribute-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3085 2024-04-30 17:20:59.000000 trytond_product_attribute-7.2.1/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5959 2024-04-30 17:20:59.000000 trytond_product_attribute-7.2.1/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 11:54:38.677673 trytond_product_attribute-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4307 2024-04-30 17:20:59.000000 trytond_product_attribute-7.2.1/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:54:38.677673 trytond_product_attribute-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:20:59.000000 trytond_product_attribute-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      329 2024-04-30 17:20:59.000000 trytond_product_attribute-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:20:59.000000 trytond_product_attribute-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       88 2024-04-30 17:21:06.000000 trytond_product_attribute-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:54:38.677673 trytond_product_attribute-7.2.1/trytond_product_attribute.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2745 2024-05-01 11:54:38.000000 trytond_product_attribute-7.2.1/trytond_product_attribute.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1824 2024-05-01 11:54:38.000000 trytond_product_attribute-7.2.1/trytond_product_attribute.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:54:38.000000 trytond_product_attribute-7.2.1/trytond_product_attribute.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       72 2024-05-01 11:54:38.000000 trytond_product_attribute-7.2.1/trytond_product_attribute.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:54:38.000000 trytond_product_attribute-7.2.1/trytond_product_attribute.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       44 2024-05-01 11:54:38.000000 trytond_product_attribute-7.2.1/trytond_product_attribute.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 11:54:38.000000 trytond_product_attribute-7.2.1/trytond_product_attribute.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:54:38.677673 trytond_product_attribute-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      789 2024-04-30 17:20:59.000000 trytond_product_attribute-7.2.1/view/attribute_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      294 2024-04-30 17:20:59.000000 trytond_product_attribute-7.2.1/view/attribute_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      224 2024-04-30 17:20:59.000000 trytond_product_attribute-7.2.1/view/attribute_list_simple.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      328 2024-04-30 17:20:59.000000 trytond_product_attribute-7.2.1/view/attribute_set_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2024-04-30 17:20:59.000000 trytond_product_attribute-7.2.1/view/attribute_set_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      522 2024-04-30 17:20:59.000000 trytond_product_attribute-7.2.1/view/product_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      455 2024-04-30 17:20:59.000000 trytond_product_attribute-7.2.1/view/product_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      402 2024-04-30 17:20:59.000000 trytond_product_attribute-7.2.1/view/template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      308 2024-04-30 17:20:59.000000 trytond_product_attribute-7.2.1/view/template_tree.xml
```

### Comparing `trytond_product_attribute-7.2.0/CHANGELOG` & `trytond_product_attribute-7.2.1/CHANGELOG`

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

### Comparing `trytond_product_attribute-7.2.0/COPYRIGHT` & `trytond_product_attribute-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-7.2.0/LICENSE` & `trytond_product_attribute-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-7.2.0/PKG-INFO` & `trytond_product_attribute-7.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_product_attribute
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module with product attributes
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_product_attribute-7.2.0/doc/conf.py` & `trytond_product_attribute-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-7.2.0/locale/bg.po` & `trytond_product_attribute-7.2.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-7.2.0/locale/ca.po` & `trytond_product_attribute-7.2.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-7.2.0/locale/cs.po` & `trytond_product_attribute-7.2.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-7.2.0/locale/de.po` & `trytond_product_attribute-7.2.1/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-7.2.0/locale/es.po` & `trytond_product_attribute-7.2.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-7.2.0/locale/es_419.po` & `trytond_product_attribute-7.2.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-7.2.0/locale/et.po` & `trytond_product_attribute-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-7.2.0/locale/fa.po` & `trytond_product_attribute-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-7.2.0/locale/fi.po` & `trytond_product_attribute-7.2.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-7.2.0/locale/fr.po` & `trytond_product_attribute-7.2.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-7.2.0/locale/hu.po` & `trytond_product_attribute-7.2.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-7.2.0/locale/id.po` & `trytond_product_attribute-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-7.2.0/locale/it.po` & `trytond_product_attribute-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-7.2.0/locale/lo.po` & `trytond_product_attribute-7.2.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-7.2.0/locale/lt.po` & `trytond_product_attribute-7.2.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-7.2.0/locale/nl.po` & `trytond_product_attribute-7.2.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-7.2.0/locale/pl.po` & `trytond_product_attribute-7.2.1/locale/pl.po`

 * *Files 3% similar despite different names*

```diff
@@ -26,18 +26,17 @@
 msgid "Attribute Set"
 msgstr "Zestaw atrybutów"
 
 msgctxt "field:product.product,attributes:"
 msgid "Attributes"
 msgstr "Atrybuty"
 
-#, fuzzy
 msgctxt "field:product.product,attributes_name:"
 msgid "Attributes Name"
-msgstr "Atrybuty"
+msgstr "Nazwa atrybutu"
 
 msgctxt "field:product.template,attribute_set:"
 msgid "Attribute Set"
 msgstr "Zestaw atrybutów"
 
 msgctxt "help:product.attribute,sets:"
 msgid "Add sets to the attribute."
@@ -69,15 +68,15 @@
 
 msgctxt "model:ir.action,name:act_attribute_set_form"
 msgid "Attribute Sets"
 msgstr "Zestawy atrybutów"
 
 msgctxt "model:ir.message,text:msg_label_value"
 msgid "%(label)s: %(value)s"
-msgstr ""
+msgstr "%(label)s: %(value)s"
 
 msgctxt "model:ir.ui.menu,name:menu_attribute"
 msgid "Attributes"
 msgstr "Atrybuty"
 
 msgctxt "model:ir.ui.menu,name:menu_attribute_set"
 msgid "Attribute Sets"
```

### Comparing `trytond_product_attribute-7.2.0/locale/pt.po` & `trytond_product_attribute-7.2.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-7.2.0/locale/ro.po` & `trytond_product_attribute-7.2.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-7.2.0/locale/ru.po` & `trytond_product_attribute-7.2.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-7.2.0/locale/sl.po` & `trytond_product_attribute-7.2.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-7.2.0/locale/tr.po` & `trytond_product_attribute-7.2.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-7.2.0/locale/uk.po` & `trytond_product_attribute-7.2.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-7.2.0/locale/zh_CN.po` & `trytond_product_attribute-7.2.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-7.2.0/product.py` & `trytond_product_attribute-7.2.1/product.py`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-7.2.0/product.xml` & `trytond_product_attribute-7.2.1/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-7.2.0/setup.py` & `trytond_product_attribute-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-7.2.0/tox.ini` & `trytond_product_attribute-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-7.2.0/trytond_product_attribute.egg-info/PKG-INFO` & `trytond_product_attribute-7.2.1/trytond_product_attribute.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_product_attribute
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module with product attributes
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_product_attribute-7.2.0/trytond_product_attribute.egg-info/SOURCES.txt` & `trytond_product_attribute-7.2.1/trytond_product_attribute.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-7.2.0/view/attribute_form.xml` & `trytond_product_attribute-7.2.1/view/attribute_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-7.2.0/view/product_form.xml` & `trytond_product_attribute-7.2.1/view/product_form.xml`

 * *Files identical despite different names*

