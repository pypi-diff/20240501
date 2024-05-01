# Comparing `tmp/trytond_web_shop_product_data_feed-7.2.0.tar.gz` & `tmp/trytond_web_shop_product_data_feed-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_web_shop_product_data_feed-7.2.0.tar", last modified: Mon Apr 29 15:55:02 2024, max compression
+gzip compressed data, was "trytond_web_shop_product_data_feed-7.2.1.tar", last modified: Wed May  1 09:50:58 2024, max compression
```

## Comparing `trytond_web_shop_product_data_feed-7.2.0.tar` & `trytond_web_shop_product_data_feed-7.2.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:02.083188 trytond_web_shop_product_data_feed-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)       71 2024-04-29 15:30:42.000000 trytond_web_shop_product_data_feed-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      670 2024-04-29 15:30:42.000000 trytond_web_shop_product_data_feed-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-27 16:30:39.000000 trytond_web_shop_product_data_feed-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-27 16:30:39.000000 trytond_web_shop_product_data_feed-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2955 2024-04-29 15:55:02.083188 trytond_web_shop_product_data_feed-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      395 2024-04-27 16:30:39.000000 trytond_web_shop_product_data_feed-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      933 2024-04-27 16:30:39.000000 trytond_web_shop_product_data_feed-7.2.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:02.079855 trytond_web_shop_product_data_feed-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3089 2024-04-27 16:30:39.000000 trytond_web_shop_product_data_feed-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      442 2024-04-27 16:30:39.000000 trytond_web_shop_product_data_feed-7.2.0/doc/configuration.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1778 2024-04-27 16:30:39.000000 trytond_web_shop_product_data_feed-7.2.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      395 2024-04-27 16:30:39.000000 trytond_web_shop_product_data_feed-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      555 2024-04-27 16:30:39.000000 trytond_web_shop_product_data_feed-7.2.0/doc/reference.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-27 16:30:39.000000 trytond_web_shop_product_data_feed-7.2.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-27 16:30:39.000000 trytond_web_shop_product_data_feed-7.2.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      557 2024-04-27 16:30:39.000000 trytond_web_shop_product_data_feed-7.2.0/doc/usage.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:02.079855 trytond_web_shop_product_data_feed-7.2.0/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2024-04-27 16:30:39.000000 trytond_web_shop_product_data_feed-7.2.0/icons/LICENSE
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:02.079855 trytond_web_shop_product_data_feed-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_web_shop_product_data_feed-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_web_shop_product_data_feed-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_web_shop_product_data_feed-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_web_shop_product_data_feed-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_web_shop_product_data_feed-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_web_shop_product_data_feed-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_web_shop_product_data_feed-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_web_shop_product_data_feed-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_web_shop_product_data_feed-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_web_shop_product_data_feed-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_web_shop_product_data_feed-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_web_shop_product_data_feed-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_web_shop_product_data_feed-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_web_shop_product_data_feed-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_web_shop_product_data_feed-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_web_shop_product_data_feed-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_web_shop_product_data_feed-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_web_shop_product_data_feed-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_web_shop_product_data_feed-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_web_shop_product_data_feed-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_web_shop_product_data_feed-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_web_shop_product_data_feed-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_web_shop_product_data_feed-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_web_shop_product_data_feed-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1516 2024-04-27 16:30:39.000000 trytond_web_shop_product_data_feed-7.2.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6208 2024-04-27 16:30:39.000000 trytond_web_shop_product_data_feed-7.2.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      801 2024-04-27 16:30:39.000000 trytond_web_shop_product_data_feed-7.2.0/routes.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:55:02.083188 trytond_web_shop_product_data_feed-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4864 2024-04-27 16:30:39.000000 trytond_web_shop_product_data_feed-7.2.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:02.079855 trytond_web_shop_product_data_feed-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-27 16:30:39.000000 trytond_web_shop_product_data_feed-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      454 2024-04-29 13:17:17.000000 trytond_web_shop_product_data_feed-7.2.0/tests/google-products.csv
--rw-r--r--   0 ced       (1000) ced       (1000)     5485 2024-04-29 13:17:17.000000 trytond_web_shop_product_data_feed-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-27 16:30:39.000000 trytond_web_shop_product_data_feed-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      176 2024-04-29 15:30:37.000000 trytond_web_shop_product_data_feed-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:02.083188 trytond_web_shop_product_data_feed-7.2.0/trytond_web_shop_product_data_feed.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2955 2024-04-29 15:55:01.000000 trytond_web_shop_product_data_feed-7.2.0/trytond_web_shop_product_data_feed.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2035 2024-04-29 15:55:02.000000 trytond_web_shop_product_data_feed-7.2.0/trytond_web_shop_product_data_feed.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:55:01.000000 trytond_web_shop_product_data_feed-7.2.0/trytond_web_shop_product_data_feed.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-29 15:55:01.000000 trytond_web_shop_product_data_feed-7.2.0/trytond_web_shop_product_data_feed.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:55:01.000000 trytond_web_shop_product_data_feed-7.2.0/trytond_web_shop_product_data_feed.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      185 2024-04-29 15:55:01.000000 trytond_web_shop_product_data_feed-7.2.0/trytond_web_shop_product_data_feed.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:55:01.000000 trytond_web_shop_product_data_feed-7.2.0/trytond_web_shop_product_data_feed.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:02.083188 trytond_web_shop_product_data_feed-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      295 2024-04-27 16:30:39.000000 trytond_web_shop_product_data_feed-7.2.0/view/product_category_facebook_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      247 2024-04-27 16:30:39.000000 trytond_web_shop_product_data_feed-7.2.0/view/product_category_facebook_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      295 2024-04-27 16:30:39.000000 trytond_web_shop_product_data_feed-7.2.0/view/product_category_google_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      247 2024-04-27 16:30:39.000000 trytond_web_shop_product_data_feed-7.2.0/view/product_category_google_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      427 2024-04-27 16:30:39.000000 trytond_web_shop_product_data_feed-7.2.0/view/product_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      449 2024-04-27 16:30:39.000000 trytond_web_shop_product_data_feed-7.2.0/view/web_shop_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    14227 2024-04-29 13:17:17.000000 trytond_web_shop_product_data_feed-7.2.0/web.py
--rw-r--r--   0 ced       (1000) ced       (1000)      469 2024-04-27 16:30:39.000000 trytond_web_shop_product_data_feed-7.2.0/web.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:50:58.296672 trytond_web_shop_product_data_feed-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)      172 2024-05-01 09:50:55.000000 trytond_web_shop_product_data_feed-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      670 2024-05-01 09:50:55.000000 trytond_web_shop_product_data_feed-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2955 2024-05-01 09:50:58.296672 trytond_web_shop_product_data_feed-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      395 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      933 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.1/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:50:58.293338 trytond_web_shop_product_data_feed-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3089 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      442 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.1/doc/configuration.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1778 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.1/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      395 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      555 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.1/doc/reference.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.1/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.1/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      557 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.1/doc/usage.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:50:58.293338 trytond_web_shop_product_data_feed-7.2.1/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.1/icons/LICENSE
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:50:58.293338 trytond_web_shop_product_data_feed-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1969 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2682 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1969 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2602 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2671 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1969 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1969 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1969 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1969 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2686 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1969 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1969 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1969 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1969 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1969 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2638 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1969 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1969 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1969 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1969 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1969 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1969 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1969 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1969 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1516 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.1/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6208 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.1/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      801 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.1/routes.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 09:50:58.296672 trytond_web_shop_product_data_feed-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4864 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.1/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:50:58.293338 trytond_web_shop_product_data_feed-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      454 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.1/tests/google-products.csv
+-rw-r--r--   0 ced       (1000) ced       (1000)     5485 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      176 2024-04-30 17:21:06.000000 trytond_web_shop_product_data_feed-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:50:58.296672 trytond_web_shop_product_data_feed-7.2.1/trytond_web_shop_product_data_feed.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2955 2024-05-01 09:50:57.000000 trytond_web_shop_product_data_feed-7.2.1/trytond_web_shop_product_data_feed.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2035 2024-05-01 09:50:58.000000 trytond_web_shop_product_data_feed-7.2.1/trytond_web_shop_product_data_feed.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 09:50:57.000000 trytond_web_shop_product_data_feed-7.2.1/trytond_web_shop_product_data_feed.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-05-01 09:50:57.000000 trytond_web_shop_product_data_feed-7.2.1/trytond_web_shop_product_data_feed.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 09:50:57.000000 trytond_web_shop_product_data_feed-7.2.1/trytond_web_shop_product_data_feed.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      185 2024-05-01 09:50:57.000000 trytond_web_shop_product_data_feed-7.2.1/trytond_web_shop_product_data_feed.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 09:50:57.000000 trytond_web_shop_product_data_feed-7.2.1/trytond_web_shop_product_data_feed.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:50:58.296672 trytond_web_shop_product_data_feed-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      295 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.1/view/product_category_facebook_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      247 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.1/view/product_category_facebook_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      295 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.1/view/product_category_google_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      247 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.1/view/product_category_google_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      427 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.1/view/product_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      449 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.1/view/web_shop_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    14227 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.1/web.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      469 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.1/web.xml
```

### Comparing `trytond_web_shop_product_data_feed-7.2.0/COPYRIGHT` & `trytond_web_shop_product_data_feed-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_product_data_feed-7.2.0/LICENSE` & `trytond_web_shop_product_data_feed-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_product_data_feed-7.2.0/PKG-INFO` & `trytond_web_shop_product_data_feed-7.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_web_shop_product_data_feed
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module to expose product data feed
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_web_shop_product_data_feed-7.2.0/__init__.py` & `trytond_web_shop_product_data_feed-7.2.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_product_data_feed-7.2.0/doc/conf.py` & `trytond_web_shop_product_data_feed-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_product_data_feed-7.2.0/doc/design.rst` & `trytond_web_shop_product_data_feed-7.2.1/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_product_data_feed-7.2.0/doc/reference.rst` & `trytond_web_shop_product_data_feed-7.2.1/doc/reference.rst`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_product_data_feed-7.2.0/doc/usage.rst` & `trytond_web_shop_product_data_feed-7.2.1/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_product_data_feed-7.2.0/icons/LICENSE` & `trytond_web_shop_product_data_feed-7.2.1/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_product_data_feed-7.2.0/product.py` & `trytond_web_shop_product_data_feed-7.2.1/product.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_product_data_feed-7.2.0/product.xml` & `trytond_web_shop_product_data_feed-7.2.1/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_product_data_feed-7.2.0/routes.py` & `trytond_web_shop_product_data_feed-7.2.1/routes.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_product_data_feed-7.2.0/setup.py` & `trytond_web_shop_product_data_feed-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_product_data_feed-7.2.0/tests/test_module.py` & `trytond_web_shop_product_data_feed-7.2.1/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_product_data_feed-7.2.0/tox.ini` & `trytond_web_shop_product_data_feed-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_product_data_feed-7.2.0/trytond_web_shop_product_data_feed.egg-info/PKG-INFO` & `trytond_web_shop_product_data_feed-7.2.1/trytond_web_shop_product_data_feed.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_web_shop_product_data_feed
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module to expose product data feed
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_web_shop_product_data_feed-7.2.0/trytond_web_shop_product_data_feed.egg-info/SOURCES.txt` & `trytond_web_shop_product_data_feed-7.2.1/trytond_web_shop_product_data_feed.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_product_data_feed-7.2.0/web.py` & `trytond_web_shop_product_data_feed-7.2.1/web.py`

 * *Files identical despite different names*

