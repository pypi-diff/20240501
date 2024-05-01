# Comparing `tmp/trytond_web_shop-7.2.0.tar.gz` & `tmp/trytond_web_shop-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_web_shop-7.2.0.tar", last modified: Mon Apr 29 15:54:05 2024, max compression
+gzip compressed data, was "trytond_web_shop-7.2.1.tar", last modified: Wed May  1 09:51:23 2024, max compression
```

## Comparing `trytond_web_shop-7.2.0.tar` & `trytond_web_shop-7.2.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:05.018014 trytond_web_shop-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      929 2024-04-29 15:29:56.000000 trytond_web_shop-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:29:56.000000 trytond_web_shop-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_web_shop-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_web_shop-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2863 2024-04-29 15:54:05.018014 trytond_web_shop-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      116 2023-04-15 07:12:15.000000 trytond_web_shop-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      961 2024-04-27 16:30:39.000000 trytond_web_shop-7.2.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:05.014681 trytond_web_shop-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3071 2024-04-27 16:30:39.000000 trytond_web_shop-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      116 2023-04-15 07:12:15.000000 trytond_web_shop-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:38.000000 trytond_web_shop-7.2.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:05.014681 trytond_web_shop-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     4467 2024-04-27 16:43:28.000000 trytond_web_shop-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5569 2024-04-27 16:43:28.000000 trytond_web_shop-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4467 2024-04-27 16:43:28.000000 trytond_web_shop-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5712 2024-04-27 16:43:28.000000 trytond_web_shop-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5583 2024-04-27 16:43:28.000000 trytond_web_shop-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4467 2024-04-27 16:43:28.000000 trytond_web_shop-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4467 2024-04-27 16:43:28.000000 trytond_web_shop-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4467 2024-04-27 16:43:28.000000 trytond_web_shop-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4467 2024-04-27 16:43:28.000000 trytond_web_shop-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5795 2024-04-27 16:43:28.000000 trytond_web_shop-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4812 2024-04-27 16:43:28.000000 trytond_web_shop-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4565 2024-04-27 16:43:28.000000 trytond_web_shop-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4556 2024-04-27 16:43:28.000000 trytond_web_shop-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4467 2024-04-27 16:43:28.000000 trytond_web_shop-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4467 2024-04-27 16:43:28.000000 trytond_web_shop-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5690 2024-04-27 16:43:28.000000 trytond_web_shop-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4467 2024-04-27 16:43:28.000000 trytond_web_shop-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4467 2024-04-27 16:43:28.000000 trytond_web_shop-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4467 2024-04-27 16:43:28.000000 trytond_web_shop-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4467 2024-04-27 16:43:28.000000 trytond_web_shop-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5677 2024-04-27 16:43:28.000000 trytond_web_shop-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4467 2024-04-27 16:43:28.000000 trytond_web_shop-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6492 2024-04-27 16:43:28.000000 trytond_web_shop-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4467 2024-04-27 16:43:28.000000 trytond_web_shop-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      754 2023-04-15 07:12:15.000000 trytond_web_shop-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2419 2024-04-27 16:30:39.000000 trytond_web_shop-7.2.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2222 2023-04-15 07:12:15.000000 trytond_web_shop-7.2.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2208 2023-04-15 07:12:15.000000 trytond_web_shop-7.2.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)      448 2023-04-15 07:12:15.000000 trytond_web_shop-7.2.0/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:54:05.018014 trytond_web_shop-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4517 2024-04-27 16:30:39.000000 trytond_web_shop-7.2.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:05.014681 trytond_web_shop-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_web_shop-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      459 2024-04-27 16:30:39.000000 trytond_web_shop-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:38.000000 trytond_web_shop-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      269 2024-04-29 15:29:52.000000 trytond_web_shop-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:05.018014 trytond_web_shop-7.2.0/trytond_web_shop.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2863 2024-04-29 15:54:04.000000 trytond_web_shop-7.2.0/trytond_web_shop.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2019 2024-04-29 15:54:04.000000 trytond_web_shop-7.2.0/trytond_web_shop.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:54:04.000000 trytond_web_shop-7.2.0/trytond_web_shop.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       54 2024-04-29 15:54:04.000000 trytond_web_shop-7.2.0/trytond_web_shop.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:00.000000 trytond_web_shop-7.2.0/trytond_web_shop.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      333 2024-04-29 15:54:04.000000 trytond_web_shop-7.2.0/trytond_web_shop.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:54:04.000000 trytond_web_shop-7.2.0/trytond_web_shop.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:05.018014 trytond_web_shop-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      288 2023-04-15 07:12:15.000000 trytond_web_shop-7.2.0/view/product_attribute_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      359 2023-04-15 07:12:15.000000 trytond_web_shop-7.2.0/view/product_category_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      351 2023-04-15 07:12:15.000000 trytond_web_shop-7.2.0/view/product_image_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      293 2023-04-15 07:12:15.000000 trytond_web_shop-7.2.0/view/product_image_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-04-15 07:12:15.000000 trytond_web_shop-7.2.0/view/product_product_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      489 2023-04-15 07:12:15.000000 trytond_web_shop-7.2.0/view/product_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      405 2023-04-15 07:12:15.000000 trytond_web_shop-7.2.0/view/sale_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      294 2023-04-15 07:12:15.000000 trytond_web_shop-7.2.0/view/shop_attribute_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      984 2024-04-27 16:30:39.000000 trytond_web_shop-7.2.0/view/shop_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-04-15 07:12:15.000000 trytond_web_shop-7.2.0/view/shop_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      425 2024-04-27 16:30:39.000000 trytond_web_shop-7.2.0/view/shop_price_list_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      433 2023-04-15 07:12:15.000000 trytond_web_shop-7.2.0/view/user_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    12739 2024-04-29 13:17:17.000000 trytond_web_shop-7.2.0/web.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3595 2024-04-27 16:30:39.000000 trytond_web_shop-7.2.0/web.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:51:23.069357 trytond_web_shop-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1030 2024-05-01 09:51:20.000000 trytond_web_shop-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-05-01 09:51:19.000000 trytond_web_shop-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2863 2024-05-01 09:51:23.069357 trytond_web_shop-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      116 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      961 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.1/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:51:23.062691 trytond_web_shop-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3071 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      116 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.1/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:51:23.066024 trytond_web_shop-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     5176 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6476 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5176 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6639 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6501 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5176 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5176 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5176 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5176 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6741 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5575 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5287 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5265 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5176 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5176 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6631 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5176 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5176 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5176 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5176 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6457 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5176 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7294 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5176 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      754 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2419 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.1/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2222 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.1/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2208 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.1/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      448 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.1/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 09:51:23.069357 trytond_web_shop-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4517 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.1/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:51:23.066024 trytond_web_shop-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      459 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      269 2024-04-30 17:21:06.000000 trytond_web_shop-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:51:23.066024 trytond_web_shop-7.2.1/trytond_web_shop.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2863 2024-05-01 09:51:22.000000 trytond_web_shop-7.2.1/trytond_web_shop.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2019 2024-05-01 09:51:23.000000 trytond_web_shop-7.2.1/trytond_web_shop.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 09:51:22.000000 trytond_web_shop-7.2.1/trytond_web_shop.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       54 2024-05-01 09:51:22.000000 trytond_web_shop-7.2.1/trytond_web_shop.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 09:51:22.000000 trytond_web_shop-7.2.1/trytond_web_shop.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      333 2024-05-01 09:51:22.000000 trytond_web_shop-7.2.1/trytond_web_shop.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 09:51:22.000000 trytond_web_shop-7.2.1/trytond_web_shop.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:51:23.066024 trytond_web_shop-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      288 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.1/view/product_attribute_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      359 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.1/view/product_category_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      351 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.1/view/product_image_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      293 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.1/view/product_image_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      315 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.1/view/product_product_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      489 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.1/view/product_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      405 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.1/view/sale_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      294 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.1/view/shop_attribute_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      984 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.1/view/shop_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      354 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.1/view/shop_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      425 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.1/view/shop_price_list_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      433 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.1/view/user_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    12739 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.1/web.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3595 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.1/web.xml
```

### Comparing `trytond_web_shop-7.2.0/CHANGELOG` & `trytond_web_shop-7.2.1/CHANGELOG`

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
 * Add countries for web shop
 * Support sale price list per web shop
 
 Version 7.0.0 - 2023-10-30
```

### Comparing `trytond_web_shop-7.2.0/COPYRIGHT` & `trytond_web_shop-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.2.0/LICENSE` & `trytond_web_shop-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.2.0/PKG-INFO` & `trytond_web_shop-7.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_web_shop
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module that provides a common base for webshops
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_web_shop-7.2.0/__init__.py` & `trytond_web_shop-7.2.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.2.0/doc/conf.py` & `trytond_web_shop-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.2.0/locale/bg.po` & `trytond_web_shop-7.2.1/locale/id.po`

 * *Files 10% similar despite different names*

```diff
@@ -48,83 +48,104 @@
 
 msgctxt "field:web.shop,categories_removed:"
 msgid "Categories Removed"
 msgstr ""
 
 msgctxt "field:web.shop,company:"
 msgid "Company"
+msgstr "Perusahaan"
+
+msgctxt "field:web.shop,countries:"
+msgid "Countries"
 msgstr ""
 
 msgctxt "field:web.shop,currency:"
 msgid "Currency"
-msgstr ""
+msgstr "Mata Uang"
 
 msgctxt "field:web.shop,guest_party:"
 msgid "Guest Party"
 msgstr ""
 
 msgctxt "field:web.shop,language:"
 msgid "Language"
-msgstr ""
+msgstr "Bahasa"
 
 msgctxt "field:web.shop,name:"
 msgid "Name"
+msgstr "Nama"
+
+msgctxt "field:web.shop,non_sale_price_list:"
+msgid "Non-Sale Price List"
 msgstr ""
 
 msgctxt "field:web.shop,products:"
 msgid "Products"
 msgstr ""
 
 msgctxt "field:web.shop,products_removed:"
 msgid "Products Removed"
 msgstr ""
 
+msgctxt "field:web.shop,sale_price_list:"
+msgid "Sale Price List"
+msgstr ""
+
 msgctxt "field:web.shop,type:"
 msgid "Type"
 msgstr ""
 
 msgctxt "field:web.shop,warehouses:"
 msgid "Warehouses"
 msgstr ""
 
+msgctxt "field:web.shop-country.country,country:"
+msgid "Country"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:web.shop-country.country,shop:"
+msgid "Shop"
+msgstr "Toko"
+
 msgctxt "field:web.shop-product.attribute,attribute:"
 msgid "Attribute"
 msgstr ""
 
 msgctxt "field:web.shop-product.attribute,shop:"
 msgid "Shop"
-msgstr ""
+msgstr "Toko"
 
 msgctxt "field:web.shop-product.category,category:"
 msgid "Category"
-msgstr ""
+msgstr "Kategori"
 
 msgctxt "field:web.shop-product.category,shop:"
 msgid "Shop"
-msgstr ""
+msgstr "Toko"
 
 msgctxt "field:web.shop-product.product,product:"
 msgid "Product"
-msgstr ""
+msgstr "Produk"
 
 msgctxt "field:web.shop-product.product,shop:"
 msgid "Shop"
-msgstr ""
+msgstr "Toko"
 
 msgctxt "field:web.shop-stock.location,shop:"
 msgid "Shop"
-msgstr ""
+msgstr "Toko"
 
 msgctxt "field:web.shop-stock.location,warehouse:"
 msgid "Warehouse"
-msgstr ""
+msgstr "Gudang"
 
 msgctxt "field:web.user,invoice_address:"
 msgid "Invoice Address"
-msgstr ""
+msgstr "Alamat Faktur"
 
 msgctxt "field:web.user,shipment_address:"
 msgid "Shipment Address"
 msgstr ""
 
 msgctxt "help:product.attribute,web_shops:"
 msgid "The list of web shops on which the attribute is published."
@@ -150,22 +171,31 @@
 msgid "The list of categories to publish."
 msgstr ""
 
 msgctxt "help:web.shop,categories_removed:"
 msgid "The list of categories to unpublish."
 msgstr ""
 
+msgctxt "help:web.shop,non_sale_price_list:"
+msgid ""
+"The price list to compute the price of products when it is not on sale."
+msgstr ""
+
 msgctxt "help:web.shop,products:"
 msgid "The list of products to publish."
 msgstr ""
 
 msgctxt "help:web.shop,products_removed:"
 msgid "The list of products to unpublish."
 msgstr ""
 
+msgctxt "help:web.shop,sale_price_list:"
+msgid "The price list to compute sale price of products."
+msgstr ""
+
 msgctxt "help:web.shop,type:"
 msgid "The front-end used for the web shop."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_shop"
 msgid "Web Shops"
 msgstr ""
@@ -192,14 +222,18 @@
 msgid "Web Shops"
 msgstr ""
 
 msgctxt "model:web.shop,name:"
 msgid "Web Shop"
 msgstr ""
 
+msgctxt "model:web.shop-country.country,name:"
+msgid "Web Shop - Country"
+msgstr ""
+
 msgctxt "model:web.shop-product.attribute,name:"
 msgid "Web Shop - Attribute"
 msgstr ""
 
 msgctxt "model:web.shop-product.category,name:"
 msgid "Web Shop - Product Category"
 msgstr ""
@@ -210,12 +244,12 @@
 
 msgctxt "model:web.shop-stock.location,name:"
 msgid "Web Shop - Warehouse"
 msgstr ""
 
 msgctxt "view:product.template:"
 msgid "Edit"
-msgstr ""
+msgstr "Sunting"
 
 msgctxt "view:web.shop:"
 msgid "Products"
-msgstr ""
+msgstr "Produk-Produk"
```

### Comparing `trytond_web_shop-7.2.0/locale/ca.po` & `trytond_web_shop-7.2.1/locale/hu.po`

 * *Files 10% similar despite different names*

```diff
@@ -1,223 +1,260 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:product.attribute,web_shops:"
 msgid "Web Shops"
-msgstr "Botiga web"
+msgstr "Webáruházak"
 
 msgctxt "field:product.category,web_shops:"
 msgid "Web Shops"
-msgstr "Botigues web"
+msgstr "Webáruházak"
 
+#, fuzzy
 msgctxt "field:product.image,web_shop:"
 msgid "Web Shop"
-msgstr "Botiga Web"
+msgstr "Webáruház"
 
+#, fuzzy
 msgctxt "field:product.product,web_shop_description:"
 msgid "Web Shop Description"
-msgstr "Descripció botiga web"
+msgstr "Webáruházak"
 
 msgctxt "field:product.product,web_shops:"
 msgid "Web Shops"
-msgstr "Botigues web"
+msgstr "Webáruházak"
 
+#, fuzzy
 msgctxt "field:product.template,web_shop_description:"
 msgid "Web Shop Description"
-msgstr "Descripció botiga web"
+msgstr "Webáruházak"
 
 msgctxt "field:sale.sale,web_id:"
 msgid "Web ID"
-msgstr "ID Web"
+msgstr ""
 
 msgctxt "field:sale.sale,web_shop:"
 msgid "Web Shop"
-msgstr "Botiga Web"
+msgstr "Webáruház"
 
 msgctxt "field:web.shop,attributes:"
 msgid "Attributes"
-msgstr "Atributs"
+msgstr "Jellemző értékek"
 
 msgctxt "field:web.shop,attributes_removed:"
 msgid "Attributes Removed"
-msgstr "Atributes eliminats"
+msgstr ""
 
 msgctxt "field:web.shop,categories:"
 msgid "Categories"
-msgstr "Categories"
+msgstr "Kategóriák"
 
 msgctxt "field:web.shop,categories_removed:"
 msgid "Categories Removed"
-msgstr "Categories eliminades"
+msgstr ""
 
 msgctxt "field:web.shop,company:"
 msgid "Company"
-msgstr "Empresa"
+msgstr "Cég"
+
+#, fuzzy
+msgctxt "field:web.shop,countries:"
+msgid "Countries"
+msgstr "Kategóriák"
 
 msgctxt "field:web.shop,currency:"
 msgid "Currency"
-msgstr "Moneda"
+msgstr "Pénznem"
 
 msgctxt "field:web.shop,guest_party:"
 msgid "Guest Party"
-msgstr "Tercer Invitat"
+msgstr "Vendég ügyfél"
 
 msgctxt "field:web.shop,language:"
 msgid "Language"
-msgstr "Idioma"
+msgstr "Nyelv"
 
 msgctxt "field:web.shop,name:"
 msgid "Name"
-msgstr "Nom"
+msgstr "Név"
+
+msgctxt "field:web.shop,non_sale_price_list:"
+msgid "Non-Sale Price List"
+msgstr ""
 
 msgctxt "field:web.shop,products:"
 msgid "Products"
-msgstr "Productes"
+msgstr "Termékek"
 
 msgctxt "field:web.shop,products_removed:"
 msgid "Products Removed"
-msgstr "Productes eliminats"
+msgstr ""
+
+msgctxt "field:web.shop,sale_price_list:"
+msgid "Sale Price List"
+msgstr ""
 
 msgctxt "field:web.shop,type:"
 msgid "Type"
-msgstr "Tipus"
+msgstr "Típus"
 
 msgctxt "field:web.shop,warehouses:"
 msgid "Warehouses"
-msgstr "Magatzems"
+msgstr "Raktárak"
+
+msgctxt "field:web.shop-country.country,country:"
+msgid "Country"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:web.shop-country.country,shop:"
+msgid "Shop"
+msgstr "Bolt"
 
 msgctxt "field:web.shop-product.attribute,attribute:"
 msgid "Attribute"
-msgstr "Atribut"
+msgstr "Jellemző érték"
 
 msgctxt "field:web.shop-product.attribute,shop:"
 msgid "Shop"
-msgstr "Botiga"
+msgstr "Bolt"
 
 msgctxt "field:web.shop-product.category,category:"
 msgid "Category"
-msgstr "Categoria"
+msgstr "Kategória"
 
 msgctxt "field:web.shop-product.category,shop:"
 msgid "Shop"
-msgstr "Botiga"
+msgstr "Bolt"
 
 msgctxt "field:web.shop-product.product,product:"
 msgid "Product"
-msgstr "Producte"
+msgstr "Termék"
 
 msgctxt "field:web.shop-product.product,shop:"
 msgid "Shop"
-msgstr "Botiga"
+msgstr "Bolt"
 
 msgctxt "field:web.shop-stock.location,shop:"
 msgid "Shop"
-msgstr "Botiga"
+msgstr "Bolt"
 
 msgctxt "field:web.shop-stock.location,warehouse:"
 msgid "Warehouse"
-msgstr "Magatzem"
+msgstr "Raktár"
 
 msgctxt "field:web.user,invoice_address:"
 msgid "Invoice Address"
-msgstr "Adreça de facturació"
+msgstr "Számlázási cím"
 
 msgctxt "field:web.user,shipment_address:"
 msgid "Shipment Address"
-msgstr "Adreça d'enviament"
+msgstr "Szállítási cím"
 
 msgctxt "help:product.attribute,web_shops:"
 msgid "The list of web shops on which the attribute is published."
-msgstr "La llista de botigues online on s'ha publicat l'atribut."
+msgstr ""
 
 msgctxt "help:product.category,web_shops:"
 msgid "The list of web shops on which the category is published."
-msgstr "La llista de botigues on esta publicada la categoria."
+msgstr ""
 
 msgctxt "help:product.product,web_shops:"
 msgid "The list of web shops on which the product is published."
-msgstr "La llista de botigues on esta publicat el producte."
+msgstr ""
 
 msgctxt "help:web.shop,attributes:"
 msgid "The list of attributes to publish."
-msgstr "La llista d'atributs a publicar."
+msgstr ""
 
 msgctxt "help:web.shop,attributes_removed:"
 msgid "The list of attributes to unpublish."
-msgstr "La llista d'atributs a despublicar."
+msgstr ""
 
 msgctxt "help:web.shop,categories:"
 msgid "The list of categories to publish."
-msgstr "La llsita de categories a publicar."
+msgstr ""
 
 msgctxt "help:web.shop,categories_removed:"
 msgid "The list of categories to unpublish."
-msgstr "La llista de categories a despublicar."
+msgstr ""
+
+msgctxt "help:web.shop,non_sale_price_list:"
+msgid ""
+"The price list to compute the price of products when it is not on sale."
+msgstr ""
 
 msgctxt "help:web.shop,products:"
 msgid "The list of products to publish."
-msgstr "La llista de productes a publicar."
+msgstr ""
 
 msgctxt "help:web.shop,products_removed:"
 msgid "The list of products to unpublish."
-msgstr "La llista de productes a despublicar."
+msgstr ""
+
+msgctxt "help:web.shop,sale_price_list:"
+msgid "The price list to compute sale price of products."
+msgstr ""
 
 msgctxt "help:web.shop,type:"
 msgid "The front-end used for the web shop."
-msgstr "El front-end utiltizat per aquesta botiga."
+msgstr ""
 
 msgctxt "model:ir.action,name:act_shop"
 msgid "Web Shops"
-msgstr "Botigues web"
+msgstr "Webáruházak"
 
 msgctxt "model:ir.message,text:msg_sale_invalid_party"
 msgid ""
 "To process the sale \"%(sale)s\" you must select another party instead of "
 "the guest \"%(party)s\"."
 msgstr ""
-"Per a processar la venda \"%(sale)s\" heu de seleccionar un tercer diferent "
-"del invitat \"%(party)s\"."
 
 msgctxt "model:ir.message,text:msg_sale_web_id_unique"
 msgid "The web ID on the sale must be unique."
-msgstr "El ID de la botiga web ha de ser únic."
+msgstr ""
 
 msgctxt "model:ir.message,text:msg_shop_name_unique"
 msgid "The web shop name must be unique."
-msgstr "El nom de la botiga web ha de ser únic."
+msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_shop_companies"
 msgid "User in companies"
-msgstr "Usuari a les empreses"
+msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_shop"
 msgid "Web Shops"
-msgstr "Botigues web"
+msgstr "Webáruházak"
 
 msgctxt "model:web.shop,name:"
 msgid "Web Shop"
-msgstr "Botiga Web"
+msgstr "Webáruház"
+
+#, fuzzy
+msgctxt "model:web.shop-country.country,name:"
+msgid "Web Shop - Country"
+msgstr "Webáruház"
 
 msgctxt "model:web.shop-product.attribute,name:"
 msgid "Web Shop - Attribute"
-msgstr "Botiga Web - Atribut"
+msgstr ""
 
 msgctxt "model:web.shop-product.category,name:"
 msgid "Web Shop - Product Category"
-msgstr "Botiga web - Categoria de producte"
+msgstr ""
 
 msgctxt "model:web.shop-product.product,name:"
 msgid "Web Shop - Product"
-msgstr "Botiga web - Producte"
+msgstr ""
 
 msgctxt "model:web.shop-stock.location,name:"
 msgid "Web Shop - Warehouse"
-msgstr "Botiga web - Magatzem"
+msgstr ""
 
 msgctxt "view:product.template:"
 msgid "Edit"
-msgstr "Edita"
+msgstr ""
 
 msgctxt "view:web.shop:"
 msgid "Products"
-msgstr "Productes"
+msgstr "Termékek"
```

### Comparing `trytond_web_shop-7.2.0/locale/cs.po` & `trytond_web_shop-7.2.1/locale/it.po`

 * *Files 18% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 msgctxt "field:sale.sale,web_shop:"
 msgid "Web Shop"
 msgstr ""
 
 msgctxt "field:web.shop,attributes:"
 msgid "Attributes"
-msgstr ""
+msgstr "Attributi"
 
 msgctxt "field:web.shop,attributes_removed:"
 msgid "Attributes Removed"
 msgstr ""
 
 msgctxt "field:web.shop,categories:"
 msgid "Categories"
@@ -50,44 +50,64 @@
 msgid "Categories Removed"
 msgstr ""
 
 msgctxt "field:web.shop,company:"
 msgid "Company"
 msgstr ""
 
+msgctxt "field:web.shop,countries:"
+msgid "Countries"
+msgstr ""
+
 msgctxt "field:web.shop,currency:"
 msgid "Currency"
-msgstr ""
+msgstr "Valuta"
 
 msgctxt "field:web.shop,guest_party:"
 msgid "Guest Party"
 msgstr ""
 
 msgctxt "field:web.shop,language:"
 msgid "Language"
 msgstr ""
 
 msgctxt "field:web.shop,name:"
 msgid "Name"
 msgstr ""
 
+msgctxt "field:web.shop,non_sale_price_list:"
+msgid "Non-Sale Price List"
+msgstr ""
+
 msgctxt "field:web.shop,products:"
 msgid "Products"
 msgstr ""
 
 msgctxt "field:web.shop,products_removed:"
 msgid "Products Removed"
 msgstr ""
 
+msgctxt "field:web.shop,sale_price_list:"
+msgid "Sale Price List"
+msgstr ""
+
 msgctxt "field:web.shop,type:"
 msgid "Type"
 msgstr ""
 
 msgctxt "field:web.shop,warehouses:"
 msgid "Warehouses"
+msgstr "Magazzini"
+
+msgctxt "field:web.shop-country.country,country:"
+msgid "Country"
+msgstr ""
+
+msgctxt "field:web.shop-country.country,shop:"
+msgid "Shop"
 msgstr ""
 
 msgctxt "field:web.shop-product.attribute,attribute:"
 msgid "Attribute"
 msgstr ""
 
 msgctxt "field:web.shop-product.attribute,shop:"
@@ -100,35 +120,35 @@
 
 msgctxt "field:web.shop-product.category,shop:"
 msgid "Shop"
 msgstr ""
 
 msgctxt "field:web.shop-product.product,product:"
 msgid "Product"
-msgstr ""
+msgstr "Prodotto"
 
 msgctxt "field:web.shop-product.product,shop:"
 msgid "Shop"
 msgstr ""
 
 msgctxt "field:web.shop-stock.location,shop:"
 msgid "Shop"
 msgstr ""
 
 msgctxt "field:web.shop-stock.location,warehouse:"
 msgid "Warehouse"
-msgstr ""
+msgstr "Magazzino"
 
 msgctxt "field:web.user,invoice_address:"
 msgid "Invoice Address"
-msgstr ""
+msgstr "Indirizzo di fatturazione"
 
 msgctxt "field:web.user,shipment_address:"
 msgid "Shipment Address"
-msgstr ""
+msgstr "indirizzo di spedizione"
 
 msgctxt "help:product.attribute,web_shops:"
 msgid "The list of web shops on which the attribute is published."
 msgstr ""
 
 msgctxt "help:product.category,web_shops:"
 msgid "The list of web shops on which the category is published."
@@ -150,22 +170,31 @@
 msgid "The list of categories to publish."
 msgstr ""
 
 msgctxt "help:web.shop,categories_removed:"
 msgid "The list of categories to unpublish."
 msgstr ""
 
+msgctxt "help:web.shop,non_sale_price_list:"
+msgid ""
+"The price list to compute the price of products when it is not on sale."
+msgstr ""
+
 msgctxt "help:web.shop,products:"
 msgid "The list of products to publish."
 msgstr ""
 
 msgctxt "help:web.shop,products_removed:"
 msgid "The list of products to unpublish."
 msgstr ""
 
+msgctxt "help:web.shop,sale_price_list:"
+msgid "The price list to compute sale price of products."
+msgstr ""
+
 msgctxt "help:web.shop,type:"
 msgid "The front-end used for the web shop."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_shop"
 msgid "Web Shops"
 msgstr ""
@@ -192,14 +221,18 @@
 msgid "Web Shops"
 msgstr ""
 
 msgctxt "model:web.shop,name:"
 msgid "Web Shop"
 msgstr ""
 
+msgctxt "model:web.shop-country.country,name:"
+msgid "Web Shop - Country"
+msgstr ""
+
 msgctxt "model:web.shop-product.attribute,name:"
 msgid "Web Shop - Attribute"
 msgstr ""
 
 msgctxt "model:web.shop-product.category,name:"
 msgid "Web Shop - Product Category"
 msgstr ""
```

### Comparing `trytond_web_shop-7.2.0/locale/de.po` & `trytond_web_shop-7.2.1/locale/de.po`

 * *Files 3% similar despite different names*

```diff
@@ -50,14 +50,18 @@
 msgid "Categories Removed"
 msgstr "Entfernte Kategorien"
 
 msgctxt "field:web.shop,company:"
 msgid "Company"
 msgstr "Unternehmen"
 
+msgctxt "field:web.shop,countries:"
+msgid "Countries"
+msgstr "Länder"
+
 msgctxt "field:web.shop,currency:"
 msgid "Currency"
 msgstr "Währung"
 
 msgctxt "field:web.shop,guest_party:"
 msgid "Guest Party"
 msgstr "Partei für Gäste"
@@ -66,30 +70,46 @@
 msgid "Language"
 msgstr "Sprache"
 
 msgctxt "field:web.shop,name:"
 msgid "Name"
 msgstr "Name"
 
+msgctxt "field:web.shop,non_sale_price_list:"
+msgid "Non-Sale Price List"
+msgstr "Vergleichspreisliste"
+
 msgctxt "field:web.shop,products:"
 msgid "Products"
 msgstr "Artikel"
 
 msgctxt "field:web.shop,products_removed:"
 msgid "Products Removed"
 msgstr "Entfernte Artikel"
 
+msgctxt "field:web.shop,sale_price_list:"
+msgid "Sale Price List"
+msgstr "Preisliste Verkauf"
+
 msgctxt "field:web.shop,type:"
 msgid "Type"
 msgstr "Typ"
 
 msgctxt "field:web.shop,warehouses:"
 msgid "Warehouses"
 msgstr "Logistikstandorte"
 
+msgctxt "field:web.shop-country.country,country:"
+msgid "Country"
+msgstr "Land"
+
+msgctxt "field:web.shop-country.country,shop:"
+msgid "Shop"
+msgstr "Webshop"
+
 msgctxt "field:web.shop-product.attribute,attribute:"
 msgid "Attribute"
 msgstr "Attribut"
 
 msgctxt "field:web.shop-product.attribute,shop:"
 msgid "Shop"
 msgstr "Webshop"
@@ -150,22 +170,33 @@
 msgid "The list of categories to publish."
 msgstr "Liste der zu veröffentlichenden Kategorien."
 
 msgctxt "help:web.shop,categories_removed:"
 msgid "The list of categories to unpublish."
 msgstr "Liste der von der Veröffentlichung zurückzuziehenden Kategorien."
 
+msgctxt "help:web.shop,non_sale_price_list:"
+msgid ""
+"The price list to compute the price of products when it is not on sale."
+msgstr ""
+"Die Preisliste zur Berechnung des Basispreises zum Zweck der "
+"Preisgegenüberstellung."
+
 msgctxt "help:web.shop,products:"
 msgid "The list of products to publish."
 msgstr "Liste der zu veröffentlichenden Artikel."
 
 msgctxt "help:web.shop,products_removed:"
 msgid "The list of products to unpublish."
 msgstr "Liste der von der Veröffentlichung zurückzuziehenden Artikel."
 
+msgctxt "help:web.shop,sale_price_list:"
+msgid "The price list to compute sale price of products."
+msgstr "Preisliste zur Berechnung der Verkaufspreise der Artikel."
+
 msgctxt "help:web.shop,type:"
 msgid "The front-end used for the web shop."
 msgstr "Das für den Webshop genutzte Frontend."
 
 msgctxt "model:ir.action,name:act_shop"
 msgid "Web Shops"
 msgstr "Webshops"
@@ -184,24 +215,28 @@
 
 msgctxt "model:ir.message,text:msg_shop_name_unique"
 msgid "The web shop name must be unique."
 msgstr "Der Name des Webshops muss eindeutig sein."
 
 msgctxt "model:ir.rule.group,name:rule_group_shop_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.ui.menu,name:menu_shop"
 msgid "Web Shops"
 msgstr "Webshops"
 
 msgctxt "model:web.shop,name:"
 msgid "Web Shop"
 msgstr "Webshop"
 
+msgctxt "model:web.shop-country.country,name:"
+msgid "Web Shop - Country"
+msgstr "Webshop - Land"
+
 msgctxt "model:web.shop-product.attribute,name:"
 msgid "Web Shop - Attribute"
 msgstr "Webshop - Attribut"
 
 msgctxt "model:web.shop-product.category,name:"
 msgid "Web Shop - Product Category"
 msgstr "Webshop - Artikelkategorie"
```

### Comparing `trytond_web_shop-7.2.0/locale/es.po` & `trytond_web_shop-7.2.1/locale/es.po`

 * *Files 9% similar despite different names*

```diff
@@ -50,14 +50,18 @@
 msgid "Categories Removed"
 msgstr "Categorías eliminadas"
 
 msgctxt "field:web.shop,company:"
 msgid "Company"
 msgstr "Empresa"
 
+msgctxt "field:web.shop,countries:"
+msgid "Countries"
+msgstr "Países"
+
 msgctxt "field:web.shop,currency:"
 msgid "Currency"
 msgstr "Moneda"
 
 msgctxt "field:web.shop,guest_party:"
 msgid "Guest Party"
 msgstr "Tercero invitado"
@@ -66,30 +70,46 @@
 msgid "Language"
 msgstr "Idioma"
 
 msgctxt "field:web.shop,name:"
 msgid "Name"
 msgstr "Nombre"
 
+msgctxt "field:web.shop,non_sale_price_list:"
+msgid "Non-Sale Price List"
+msgstr "Tarifa de no-venta"
+
 msgctxt "field:web.shop,products:"
 msgid "Products"
 msgstr "Productos"
 
 msgctxt "field:web.shop,products_removed:"
 msgid "Products Removed"
 msgstr "Productos Eliminados"
 
+msgctxt "field:web.shop,sale_price_list:"
+msgid "Sale Price List"
+msgstr "Tarifa de venta"
+
 msgctxt "field:web.shop,type:"
 msgid "Type"
 msgstr "Tipo"
 
 msgctxt "field:web.shop,warehouses:"
 msgid "Warehouses"
 msgstr "Almacenes"
 
+msgctxt "field:web.shop-country.country,country:"
+msgid "Country"
+msgstr "País"
+
+msgctxt "field:web.shop-country.country,shop:"
+msgid "Shop"
+msgstr "Tienda"
+
 msgctxt "field:web.shop-product.attribute,attribute:"
 msgid "Attribute"
 msgstr "Atributo"
 
 msgctxt "field:web.shop-product.attribute,shop:"
 msgid "Shop"
 msgstr "Tienda"
@@ -150,22 +170,33 @@
 msgid "The list of categories to publish."
 msgstr "La lista de categorias a publicar."
 
 msgctxt "help:web.shop,categories_removed:"
 msgid "The list of categories to unpublish."
 msgstr "La lista de categorias a despublicar."
 
+msgctxt "help:web.shop,non_sale_price_list:"
+msgid ""
+"The price list to compute the price of products when it is not on sale."
+msgstr ""
+"La tarifa para calcular los precios de los productos cuando no se está en "
+"venta."
+
 msgctxt "help:web.shop,products:"
 msgid "The list of products to publish."
 msgstr "La lista de produtos a publicar."
 
 msgctxt "help:web.shop,products_removed:"
 msgid "The list of products to unpublish."
 msgstr "La lista de categorias a despublicar."
 
+msgctxt "help:web.shop,sale_price_list:"
+msgid "The price list to compute sale price of products."
+msgstr "La tarifa para calcular los precios de los productos."
+
 msgctxt "help:web.shop,type:"
 msgid "The front-end used for the web shop."
 msgstr "El frontend utilizado para la tienda web."
 
 msgctxt "model:ir.action,name:act_shop"
 msgid "Web Shops"
 msgstr "Tiendas Web"
@@ -194,14 +225,18 @@
 msgid "Web Shops"
 msgstr "Tiendas Web"
 
 msgctxt "model:web.shop,name:"
 msgid "Web Shop"
 msgstr "Tienda Web"
 
+msgctxt "model:web.shop-country.country,name:"
+msgid "Web Shop - Country"
+msgstr "Tienda Web - País"
+
 msgctxt "model:web.shop-product.attribute,name:"
 msgid "Web Shop - Attribute"
 msgstr "Tienda Web - Atributo"
 
 msgctxt "model:web.shop-product.category,name:"
 msgid "Web Shop - Product Category"
 msgstr "Tienda Web - Categoría Producto"
```

### Comparing `trytond_web_shop-7.2.0/locale/es_419.po` & `trytond_web_shop-7.2.1/locale/bg.po`

 * *Files 18% similar despite different names*

```diff
@@ -50,14 +50,18 @@
 msgid "Categories Removed"
 msgstr ""
 
 msgctxt "field:web.shop,company:"
 msgid "Company"
 msgstr ""
 
+msgctxt "field:web.shop,countries:"
+msgid "Countries"
+msgstr ""
+
 msgctxt "field:web.shop,currency:"
 msgid "Currency"
 msgstr ""
 
 msgctxt "field:web.shop,guest_party:"
 msgid "Guest Party"
 msgstr ""
@@ -66,30 +70,46 @@
 msgid "Language"
 msgstr ""
 
 msgctxt "field:web.shop,name:"
 msgid "Name"
 msgstr ""
 
+msgctxt "field:web.shop,non_sale_price_list:"
+msgid "Non-Sale Price List"
+msgstr ""
+
 msgctxt "field:web.shop,products:"
 msgid "Products"
 msgstr ""
 
 msgctxt "field:web.shop,products_removed:"
 msgid "Products Removed"
 msgstr ""
 
+msgctxt "field:web.shop,sale_price_list:"
+msgid "Sale Price List"
+msgstr ""
+
 msgctxt "field:web.shop,type:"
 msgid "Type"
 msgstr ""
 
 msgctxt "field:web.shop,warehouses:"
 msgid "Warehouses"
 msgstr ""
 
+msgctxt "field:web.shop-country.country,country:"
+msgid "Country"
+msgstr ""
+
+msgctxt "field:web.shop-country.country,shop:"
+msgid "Shop"
+msgstr ""
+
 msgctxt "field:web.shop-product.attribute,attribute:"
 msgid "Attribute"
 msgstr ""
 
 msgctxt "field:web.shop-product.attribute,shop:"
 msgid "Shop"
 msgstr ""
@@ -150,22 +170,31 @@
 msgid "The list of categories to publish."
 msgstr ""
 
 msgctxt "help:web.shop,categories_removed:"
 msgid "The list of categories to unpublish."
 msgstr ""
 
+msgctxt "help:web.shop,non_sale_price_list:"
+msgid ""
+"The price list to compute the price of products when it is not on sale."
+msgstr ""
+
 msgctxt "help:web.shop,products:"
 msgid "The list of products to publish."
 msgstr ""
 
 msgctxt "help:web.shop,products_removed:"
 msgid "The list of products to unpublish."
 msgstr ""
 
+msgctxt "help:web.shop,sale_price_list:"
+msgid "The price list to compute sale price of products."
+msgstr ""
+
 msgctxt "help:web.shop,type:"
 msgid "The front-end used for the web shop."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_shop"
 msgid "Web Shops"
 msgstr ""
@@ -192,14 +221,18 @@
 msgid "Web Shops"
 msgstr ""
 
 msgctxt "model:web.shop,name:"
 msgid "Web Shop"
 msgstr ""
 
+msgctxt "model:web.shop-country.country,name:"
+msgid "Web Shop - Country"
+msgstr ""
+
 msgctxt "model:web.shop-product.attribute,name:"
 msgid "Web Shop - Attribute"
 msgstr ""
 
 msgctxt "model:web.shop-product.category,name:"
 msgid "Web Shop - Product Category"
 msgstr ""
```

### Comparing `trytond_web_shop-7.2.0/locale/et.po` & `trytond_web_shop-7.2.1/locale/cs.po`

 * *Files 18% similar despite different names*

```diff
@@ -50,14 +50,18 @@
 msgid "Categories Removed"
 msgstr ""
 
 msgctxt "field:web.shop,company:"
 msgid "Company"
 msgstr ""
 
+msgctxt "field:web.shop,countries:"
+msgid "Countries"
+msgstr ""
+
 msgctxt "field:web.shop,currency:"
 msgid "Currency"
 msgstr ""
 
 msgctxt "field:web.shop,guest_party:"
 msgid "Guest Party"
 msgstr ""
@@ -66,30 +70,46 @@
 msgid "Language"
 msgstr ""
 
 msgctxt "field:web.shop,name:"
 msgid "Name"
 msgstr ""
 
+msgctxt "field:web.shop,non_sale_price_list:"
+msgid "Non-Sale Price List"
+msgstr ""
+
 msgctxt "field:web.shop,products:"
 msgid "Products"
 msgstr ""
 
 msgctxt "field:web.shop,products_removed:"
 msgid "Products Removed"
 msgstr ""
 
+msgctxt "field:web.shop,sale_price_list:"
+msgid "Sale Price List"
+msgstr ""
+
 msgctxt "field:web.shop,type:"
 msgid "Type"
 msgstr ""
 
 msgctxt "field:web.shop,warehouses:"
 msgid "Warehouses"
 msgstr ""
 
+msgctxt "field:web.shop-country.country,country:"
+msgid "Country"
+msgstr ""
+
+msgctxt "field:web.shop-country.country,shop:"
+msgid "Shop"
+msgstr ""
+
 msgctxt "field:web.shop-product.attribute,attribute:"
 msgid "Attribute"
 msgstr ""
 
 msgctxt "field:web.shop-product.attribute,shop:"
 msgid "Shop"
 msgstr ""
@@ -150,22 +170,31 @@
 msgid "The list of categories to publish."
 msgstr ""
 
 msgctxt "help:web.shop,categories_removed:"
 msgid "The list of categories to unpublish."
 msgstr ""
 
+msgctxt "help:web.shop,non_sale_price_list:"
+msgid ""
+"The price list to compute the price of products when it is not on sale."
+msgstr ""
+
 msgctxt "help:web.shop,products:"
 msgid "The list of products to publish."
 msgstr ""
 
 msgctxt "help:web.shop,products_removed:"
 msgid "The list of products to unpublish."
 msgstr ""
 
+msgctxt "help:web.shop,sale_price_list:"
+msgid "The price list to compute sale price of products."
+msgstr ""
+
 msgctxt "help:web.shop,type:"
 msgid "The front-end used for the web shop."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_shop"
 msgid "Web Shops"
 msgstr ""
@@ -192,14 +221,18 @@
 msgid "Web Shops"
 msgstr ""
 
 msgctxt "model:web.shop,name:"
 msgid "Web Shop"
 msgstr ""
 
+msgctxt "model:web.shop-country.country,name:"
+msgid "Web Shop - Country"
+msgstr ""
+
 msgctxt "model:web.shop-product.attribute,name:"
 msgid "Web Shop - Attribute"
 msgstr ""
 
 msgctxt "model:web.shop-product.category,name:"
 msgid "Web Shop - Product Category"
 msgstr ""
```

### Comparing `trytond_web_shop-7.2.0/locale/fa.po` & `trytond_web_shop-7.2.1/locale/es_419.po`

 * *Files 18% similar despite different names*

```diff
@@ -50,14 +50,18 @@
 msgid "Categories Removed"
 msgstr ""
 
 msgctxt "field:web.shop,company:"
 msgid "Company"
 msgstr ""
 
+msgctxt "field:web.shop,countries:"
+msgid "Countries"
+msgstr ""
+
 msgctxt "field:web.shop,currency:"
 msgid "Currency"
 msgstr ""
 
 msgctxt "field:web.shop,guest_party:"
 msgid "Guest Party"
 msgstr ""
@@ -66,30 +70,46 @@
 msgid "Language"
 msgstr ""
 
 msgctxt "field:web.shop,name:"
 msgid "Name"
 msgstr ""
 
+msgctxt "field:web.shop,non_sale_price_list:"
+msgid "Non-Sale Price List"
+msgstr ""
+
 msgctxt "field:web.shop,products:"
 msgid "Products"
 msgstr ""
 
 msgctxt "field:web.shop,products_removed:"
 msgid "Products Removed"
 msgstr ""
 
+msgctxt "field:web.shop,sale_price_list:"
+msgid "Sale Price List"
+msgstr ""
+
 msgctxt "field:web.shop,type:"
 msgid "Type"
 msgstr ""
 
 msgctxt "field:web.shop,warehouses:"
 msgid "Warehouses"
 msgstr ""
 
+msgctxt "field:web.shop-country.country,country:"
+msgid "Country"
+msgstr ""
+
+msgctxt "field:web.shop-country.country,shop:"
+msgid "Shop"
+msgstr ""
+
 msgctxt "field:web.shop-product.attribute,attribute:"
 msgid "Attribute"
 msgstr ""
 
 msgctxt "field:web.shop-product.attribute,shop:"
 msgid "Shop"
 msgstr ""
@@ -150,22 +170,31 @@
 msgid "The list of categories to publish."
 msgstr ""
 
 msgctxt "help:web.shop,categories_removed:"
 msgid "The list of categories to unpublish."
 msgstr ""
 
+msgctxt "help:web.shop,non_sale_price_list:"
+msgid ""
+"The price list to compute the price of products when it is not on sale."
+msgstr ""
+
 msgctxt "help:web.shop,products:"
 msgid "The list of products to publish."
 msgstr ""
 
 msgctxt "help:web.shop,products_removed:"
 msgid "The list of products to unpublish."
 msgstr ""
 
+msgctxt "help:web.shop,sale_price_list:"
+msgid "The price list to compute sale price of products."
+msgstr ""
+
 msgctxt "help:web.shop,type:"
 msgid "The front-end used for the web shop."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_shop"
 msgid "Web Shops"
 msgstr ""
@@ -192,14 +221,18 @@
 msgid "Web Shops"
 msgstr ""
 
 msgctxt "model:web.shop,name:"
 msgid "Web Shop"
 msgstr ""
 
+msgctxt "model:web.shop-country.country,name:"
+msgid "Web Shop - Country"
+msgstr ""
+
 msgctxt "model:web.shop-product.attribute,name:"
 msgid "Web Shop - Attribute"
 msgstr ""
 
 msgctxt "model:web.shop-product.category,name:"
 msgid "Web Shop - Product Category"
 msgstr ""
```

### Comparing `trytond_web_shop-7.2.0/locale/fi.po` & `trytond_web_shop-7.2.1/locale/et.po`

 * *Files 18% similar despite different names*

```diff
@@ -50,14 +50,18 @@
 msgid "Categories Removed"
 msgstr ""
 
 msgctxt "field:web.shop,company:"
 msgid "Company"
 msgstr ""
 
+msgctxt "field:web.shop,countries:"
+msgid "Countries"
+msgstr ""
+
 msgctxt "field:web.shop,currency:"
 msgid "Currency"
 msgstr ""
 
 msgctxt "field:web.shop,guest_party:"
 msgid "Guest Party"
 msgstr ""
@@ -66,30 +70,46 @@
 msgid "Language"
 msgstr ""
 
 msgctxt "field:web.shop,name:"
 msgid "Name"
 msgstr ""
 
+msgctxt "field:web.shop,non_sale_price_list:"
+msgid "Non-Sale Price List"
+msgstr ""
+
 msgctxt "field:web.shop,products:"
 msgid "Products"
 msgstr ""
 
 msgctxt "field:web.shop,products_removed:"
 msgid "Products Removed"
 msgstr ""
 
+msgctxt "field:web.shop,sale_price_list:"
+msgid "Sale Price List"
+msgstr ""
+
 msgctxt "field:web.shop,type:"
 msgid "Type"
 msgstr ""
 
 msgctxt "field:web.shop,warehouses:"
 msgid "Warehouses"
 msgstr ""
 
+msgctxt "field:web.shop-country.country,country:"
+msgid "Country"
+msgstr ""
+
+msgctxt "field:web.shop-country.country,shop:"
+msgid "Shop"
+msgstr ""
+
 msgctxt "field:web.shop-product.attribute,attribute:"
 msgid "Attribute"
 msgstr ""
 
 msgctxt "field:web.shop-product.attribute,shop:"
 msgid "Shop"
 msgstr ""
@@ -150,22 +170,31 @@
 msgid "The list of categories to publish."
 msgstr ""
 
 msgctxt "help:web.shop,categories_removed:"
 msgid "The list of categories to unpublish."
 msgstr ""
 
+msgctxt "help:web.shop,non_sale_price_list:"
+msgid ""
+"The price list to compute the price of products when it is not on sale."
+msgstr ""
+
 msgctxt "help:web.shop,products:"
 msgid "The list of products to publish."
 msgstr ""
 
 msgctxt "help:web.shop,products_removed:"
 msgid "The list of products to unpublish."
 msgstr ""
 
+msgctxt "help:web.shop,sale_price_list:"
+msgid "The price list to compute sale price of products."
+msgstr ""
+
 msgctxt "help:web.shop,type:"
 msgid "The front-end used for the web shop."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_shop"
 msgid "Web Shops"
 msgstr ""
@@ -192,14 +221,18 @@
 msgid "Web Shops"
 msgstr ""
 
 msgctxt "model:web.shop,name:"
 msgid "Web Shop"
 msgstr ""
 
+msgctxt "model:web.shop-country.country,name:"
+msgid "Web Shop - Country"
+msgstr ""
+
 msgctxt "model:web.shop-product.attribute,name:"
 msgid "Web Shop - Attribute"
 msgstr ""
 
 msgctxt "model:web.shop-product.category,name:"
 msgid "Web Shop - Product Category"
 msgstr ""
```

### Comparing `trytond_web_shop-7.2.0/locale/fr.po` & `trytond_web_shop-7.2.1/locale/fr.po`

 * *Files 13% similar despite different names*

```diff
@@ -50,14 +50,18 @@
 msgid "Categories Removed"
 msgstr "Catégories supprimées"
 
 msgctxt "field:web.shop,company:"
 msgid "Company"
 msgstr "Société"
 
+msgctxt "field:web.shop,countries:"
+msgid "Countries"
+msgstr "Pays"
+
 msgctxt "field:web.shop,currency:"
 msgid "Currency"
 msgstr "Devise"
 
 msgctxt "field:web.shop,guest_party:"
 msgid "Guest Party"
 msgstr "Tiers invité"
@@ -66,30 +70,46 @@
 msgid "Language"
 msgstr "Langue"
 
 msgctxt "field:web.shop,name:"
 msgid "Name"
 msgstr "Nom"
 
+msgctxt "field:web.shop,non_sale_price_list:"
+msgid "Non-Sale Price List"
+msgstr "Liste de prix hors vente"
+
 msgctxt "field:web.shop,products:"
 msgid "Products"
 msgstr "Produits"
 
 msgctxt "field:web.shop,products_removed:"
 msgid "Products Removed"
 msgstr "Produits supprimés"
 
+msgctxt "field:web.shop,sale_price_list:"
+msgid "Sale Price List"
+msgstr "Liste de prix de vente"
+
 msgctxt "field:web.shop,type:"
 msgid "Type"
 msgstr "Type"
 
 msgctxt "field:web.shop,warehouses:"
 msgid "Warehouses"
 msgstr "Entrepôts"
 
+msgctxt "field:web.shop-country.country,country:"
+msgid "Country"
+msgstr "Pays"
+
+msgctxt "field:web.shop-country.country,shop:"
+msgid "Shop"
+msgstr "Boutique"
+
 msgctxt "field:web.shop-product.attribute,attribute:"
 msgid "Attribute"
 msgstr "Attribut"
 
 msgctxt "field:web.shop-product.attribute,shop:"
 msgid "Shop"
 msgstr "Boutique"
@@ -151,22 +171,33 @@
 msgid "The list of categories to publish."
 msgstr "La liste des catégories à publier."
 
 msgctxt "help:web.shop,categories_removed:"
 msgid "The list of categories to unpublish."
 msgstr "La liste des catégories à dépublier."
 
+msgctxt "help:web.shop,non_sale_price_list:"
+msgid ""
+"The price list to compute the price of products when it is not on sale."
+msgstr ""
+"La liste de prix pour calculer le prix des produits lorsqu'ils ne sont pas "
+"en solde."
+
 msgctxt "help:web.shop,products:"
 msgid "The list of products to publish."
 msgstr "La liste des produits à publier."
 
 msgctxt "help:web.shop,products_removed:"
 msgid "The list of products to unpublish."
 msgstr "La liste des produits à dépublier."
 
+msgctxt "help:web.shop,sale_price_list:"
+msgid "The price list to compute sale price of products."
+msgstr "La liste de prix pour calculer le prix de vente des produits."
+
 msgctxt "help:web.shop,type:"
 msgid "The front-end used for the web shop."
 msgstr "Le frontal utilisé pour la boutique en ligne."
 
 msgctxt "model:ir.action,name:act_shop"
 msgid "Web Shops"
 msgstr "Boutiques en ligne"
@@ -195,14 +226,18 @@
 msgid "Web Shops"
 msgstr "Boutiques en ligne"
 
 msgctxt "model:web.shop,name:"
 msgid "Web Shop"
 msgstr "Boutique en ligne"
 
+msgctxt "model:web.shop-country.country,name:"
+msgid "Web Shop - Country"
+msgstr "Boutique en ligne - Pays"
+
 msgctxt "model:web.shop-product.attribute,name:"
 msgid "Web Shop - Attribute"
 msgstr "Boutique Web - Attribut"
 
 msgctxt "model:web.shop-product.category,name:"
 msgid "Web Shop - Product Category"
 msgstr "Boutique en ligne - Catégorie de produit"
```

### Comparing `trytond_web_shop-7.2.0/locale/hu.po` & `trytond_web_shop-7.2.1/locale/ca.po`

 * *Files 25% similar despite different names*

```diff
@@ -1,224 +1,257 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:product.attribute,web_shops:"
 msgid "Web Shops"
-msgstr "Webáruházak"
+msgstr "Botiga web"
 
 msgctxt "field:product.category,web_shops:"
 msgid "Web Shops"
-msgstr "Webáruházak"
+msgstr "Botigues web"
 
-#, fuzzy
 msgctxt "field:product.image,web_shop:"
 msgid "Web Shop"
-msgstr "Webáruház"
+msgstr "Botiga Web"
 
-#, fuzzy
 msgctxt "field:product.product,web_shop_description:"
 msgid "Web Shop Description"
-msgstr "Webáruházak"
+msgstr "Descripció botiga web"
 
 msgctxt "field:product.product,web_shops:"
 msgid "Web Shops"
-msgstr "Webáruházak"
+msgstr "Botigues web"
 
-#, fuzzy
 msgctxt "field:product.template,web_shop_description:"
 msgid "Web Shop Description"
-msgstr "Webáruházak"
+msgstr "Descripció botiga web"
 
 msgctxt "field:sale.sale,web_id:"
 msgid "Web ID"
-msgstr ""
+msgstr "ID Web"
 
 msgctxt "field:sale.sale,web_shop:"
 msgid "Web Shop"
-msgstr "Webáruház"
+msgstr "Botiga Web"
 
 msgctxt "field:web.shop,attributes:"
 msgid "Attributes"
-msgstr "Jellemző értékek"
+msgstr "Atributs"
 
 msgctxt "field:web.shop,attributes_removed:"
 msgid "Attributes Removed"
-msgstr ""
+msgstr "Atributes eliminats"
 
 msgctxt "field:web.shop,categories:"
 msgid "Categories"
-msgstr "Kategóriák"
+msgstr "Categories"
 
 msgctxt "field:web.shop,categories_removed:"
 msgid "Categories Removed"
-msgstr ""
+msgstr "Categories eliminades"
 
 msgctxt "field:web.shop,company:"
 msgid "Company"
-msgstr "Cég"
+msgstr "Empresa"
+
+msgctxt "field:web.shop,countries:"
+msgid "Countries"
+msgstr "Països"
 
 msgctxt "field:web.shop,currency:"
 msgid "Currency"
-msgstr "Pénznem"
+msgstr "Moneda"
 
 msgctxt "field:web.shop,guest_party:"
 msgid "Guest Party"
-msgstr "Vendég ügyfél"
+msgstr "Tercer Invitat"
 
 msgctxt "field:web.shop,language:"
 msgid "Language"
-msgstr "Nyelv"
+msgstr "Idioma"
 
 msgctxt "field:web.shop,name:"
 msgid "Name"
-msgstr "Név"
+msgstr "Nom"
+
+msgctxt "field:web.shop,non_sale_price_list:"
+msgid "Non-Sale Price List"
+msgstr "Tarifa de no-venda"
 
 msgctxt "field:web.shop,products:"
 msgid "Products"
-msgstr "Termékek"
+msgstr "Productes"
 
 msgctxt "field:web.shop,products_removed:"
 msgid "Products Removed"
-msgstr ""
+msgstr "Productes eliminats"
+
+msgctxt "field:web.shop,sale_price_list:"
+msgid "Sale Price List"
+msgstr "Tarifa de venda"
 
 msgctxt "field:web.shop,type:"
 msgid "Type"
-msgstr "Típus"
+msgstr "Tipus"
 
 msgctxt "field:web.shop,warehouses:"
 msgid "Warehouses"
-msgstr "Raktárak"
+msgstr "Magatzems"
+
+msgctxt "field:web.shop-country.country,country:"
+msgid "Country"
+msgstr "País"
+
+msgctxt "field:web.shop-country.country,shop:"
+msgid "Shop"
+msgstr "Botiga"
 
 msgctxt "field:web.shop-product.attribute,attribute:"
 msgid "Attribute"
-msgstr "Jellemző érték"
+msgstr "Atribut"
 
 msgctxt "field:web.shop-product.attribute,shop:"
 msgid "Shop"
-msgstr "Bolt"
+msgstr "Botiga"
 
 msgctxt "field:web.shop-product.category,category:"
 msgid "Category"
-msgstr "Kategória"
+msgstr "Categoria"
 
 msgctxt "field:web.shop-product.category,shop:"
 msgid "Shop"
-msgstr "Bolt"
+msgstr "Botiga"
 
 msgctxt "field:web.shop-product.product,product:"
 msgid "Product"
-msgstr "Termék"
+msgstr "Producte"
 
 msgctxt "field:web.shop-product.product,shop:"
 msgid "Shop"
-msgstr "Bolt"
+msgstr "Botiga"
 
 msgctxt "field:web.shop-stock.location,shop:"
 msgid "Shop"
-msgstr "Bolt"
+msgstr "Botiga"
 
 msgctxt "field:web.shop-stock.location,warehouse:"
 msgid "Warehouse"
-msgstr "Raktár"
+msgstr "Magatzem"
 
 msgctxt "field:web.user,invoice_address:"
 msgid "Invoice Address"
-msgstr "Számlázási cím"
+msgstr "Adreça de facturació"
 
 msgctxt "field:web.user,shipment_address:"
 msgid "Shipment Address"
-msgstr "Szállítási cím"
+msgstr "Adreça d'enviament"
 
 msgctxt "help:product.attribute,web_shops:"
 msgid "The list of web shops on which the attribute is published."
-msgstr ""
+msgstr "La llista de botigues online on s'ha publicat l'atribut."
 
 msgctxt "help:product.category,web_shops:"
 msgid "The list of web shops on which the category is published."
-msgstr ""
+msgstr "La llista de botigues on esta publicada la categoria."
 
 msgctxt "help:product.product,web_shops:"
 msgid "The list of web shops on which the product is published."
-msgstr ""
+msgstr "La llista de botigues on esta publicat el producte."
 
 msgctxt "help:web.shop,attributes:"
 msgid "The list of attributes to publish."
-msgstr ""
+msgstr "La llista d'atributs a publicar."
 
 msgctxt "help:web.shop,attributes_removed:"
 msgid "The list of attributes to unpublish."
-msgstr ""
+msgstr "La llista d'atributs a despublicar."
 
 msgctxt "help:web.shop,categories:"
 msgid "The list of categories to publish."
-msgstr ""
+msgstr "La llsita de categories a publicar."
 
 msgctxt "help:web.shop,categories_removed:"
 msgid "The list of categories to unpublish."
+msgstr "La llista de categories a despublicar."
+
+msgctxt "help:web.shop,non_sale_price_list:"
+msgid ""
+"The price list to compute the price of products when it is not on sale."
 msgstr ""
+"La tarifa per calcular el preu dels productes quan no està a la venda."
 
 msgctxt "help:web.shop,products:"
 msgid "The list of products to publish."
-msgstr ""
+msgstr "La llista de productes a publicar."
 
 msgctxt "help:web.shop,products_removed:"
 msgid "The list of products to unpublish."
-msgstr ""
+msgstr "La llista de productes a despublicar."
+
+msgctxt "help:web.shop,sale_price_list:"
+msgid "The price list to compute sale price of products."
+msgstr "La tarifa per calcular el preu de venda dels productes."
 
 msgctxt "help:web.shop,type:"
 msgid "The front-end used for the web shop."
-msgstr ""
+msgstr "El front-end utiltizat per aquesta botiga."
 
 msgctxt "model:ir.action,name:act_shop"
 msgid "Web Shops"
-msgstr "Webáruházak"
+msgstr "Botigues web"
 
 msgctxt "model:ir.message,text:msg_sale_invalid_party"
 msgid ""
 "To process the sale \"%(sale)s\" you must select another party instead of "
 "the guest \"%(party)s\"."
 msgstr ""
+"Per a processar la venda \"%(sale)s\" heu de seleccionar un tercer diferent "
+"del invitat \"%(party)s\"."
 
 msgctxt "model:ir.message,text:msg_sale_web_id_unique"
 msgid "The web ID on the sale must be unique."
-msgstr ""
+msgstr "El ID de la botiga web ha de ser únic."
 
 msgctxt "model:ir.message,text:msg_shop_name_unique"
 msgid "The web shop name must be unique."
-msgstr ""
+msgstr "El nom de la botiga web ha de ser únic."
 
 msgctxt "model:ir.rule.group,name:rule_group_shop_companies"
 msgid "User in companies"
-msgstr ""
+msgstr "Usuari a les empreses"
 
 msgctxt "model:ir.ui.menu,name:menu_shop"
 msgid "Web Shops"
-msgstr "Webáruházak"
+msgstr "Botigues web"
 
 msgctxt "model:web.shop,name:"
 msgid "Web Shop"
-msgstr "Webáruház"
+msgstr "Botiga Web"
+
+msgctxt "model:web.shop-country.country,name:"
+msgid "Web Shop - Country"
+msgstr "Botiga web - País"
 
 msgctxt "model:web.shop-product.attribute,name:"
 msgid "Web Shop - Attribute"
-msgstr ""
+msgstr "Botiga Web - Atribut"
 
 msgctxt "model:web.shop-product.category,name:"
 msgid "Web Shop - Product Category"
-msgstr ""
+msgstr "Botiga web - Categoria de producte"
 
 msgctxt "model:web.shop-product.product,name:"
 msgid "Web Shop - Product"
-msgstr ""
+msgstr "Botiga web - Producte"
 
 msgctxt "model:web.shop-stock.location,name:"
 msgid "Web Shop - Warehouse"
-msgstr ""
+msgstr "Botiga web - Magatzem"
 
 msgctxt "view:product.template:"
 msgid "Edit"
-msgstr ""
+msgstr "Edita"
 
 msgctxt "view:web.shop:"
 msgid "Products"
-msgstr "Termékek"
+msgstr "Productes"
```

### Comparing `trytond_web_shop-7.2.0/locale/id.po` & `trytond_web_shop-7.2.1/locale/fa.po`

 * *Files 18% similar despite different names*

```diff
@@ -48,83 +48,103 @@
 
 msgctxt "field:web.shop,categories_removed:"
 msgid "Categories Removed"
 msgstr ""
 
 msgctxt "field:web.shop,company:"
 msgid "Company"
-msgstr "Perusahaan"
+msgstr ""
+
+msgctxt "field:web.shop,countries:"
+msgid "Countries"
+msgstr ""
 
 msgctxt "field:web.shop,currency:"
 msgid "Currency"
-msgstr "Mata Uang"
+msgstr ""
 
 msgctxt "field:web.shop,guest_party:"
 msgid "Guest Party"
 msgstr ""
 
 msgctxt "field:web.shop,language:"
 msgid "Language"
-msgstr "Bahasa"
+msgstr ""
 
 msgctxt "field:web.shop,name:"
 msgid "Name"
-msgstr "Nama"
+msgstr ""
+
+msgctxt "field:web.shop,non_sale_price_list:"
+msgid "Non-Sale Price List"
+msgstr ""
 
 msgctxt "field:web.shop,products:"
 msgid "Products"
 msgstr ""
 
 msgctxt "field:web.shop,products_removed:"
 msgid "Products Removed"
 msgstr ""
 
+msgctxt "field:web.shop,sale_price_list:"
+msgid "Sale Price List"
+msgstr ""
+
 msgctxt "field:web.shop,type:"
 msgid "Type"
 msgstr ""
 
 msgctxt "field:web.shop,warehouses:"
 msgid "Warehouses"
 msgstr ""
 
+msgctxt "field:web.shop-country.country,country:"
+msgid "Country"
+msgstr ""
+
+msgctxt "field:web.shop-country.country,shop:"
+msgid "Shop"
+msgstr ""
+
 msgctxt "field:web.shop-product.attribute,attribute:"
 msgid "Attribute"
 msgstr ""
 
 msgctxt "field:web.shop-product.attribute,shop:"
 msgid "Shop"
-msgstr "Toko"
+msgstr ""
 
 msgctxt "field:web.shop-product.category,category:"
 msgid "Category"
-msgstr "Kategori"
+msgstr ""
 
 msgctxt "field:web.shop-product.category,shop:"
 msgid "Shop"
-msgstr "Toko"
+msgstr ""
 
 msgctxt "field:web.shop-product.product,product:"
 msgid "Product"
-msgstr "Produk"
+msgstr ""
 
 msgctxt "field:web.shop-product.product,shop:"
 msgid "Shop"
-msgstr "Toko"
+msgstr ""
 
 msgctxt "field:web.shop-stock.location,shop:"
 msgid "Shop"
-msgstr "Toko"
+msgstr ""
 
 msgctxt "field:web.shop-stock.location,warehouse:"
 msgid "Warehouse"
-msgstr "Gudang"
+msgstr ""
 
 msgctxt "field:web.user,invoice_address:"
 msgid "Invoice Address"
-msgstr "Alamat Faktur"
+msgstr ""
 
 msgctxt "field:web.user,shipment_address:"
 msgid "Shipment Address"
 msgstr ""
 
 msgctxt "help:product.attribute,web_shops:"
 msgid "The list of web shops on which the attribute is published."
@@ -150,22 +170,31 @@
 msgid "The list of categories to publish."
 msgstr ""
 
 msgctxt "help:web.shop,categories_removed:"
 msgid "The list of categories to unpublish."
 msgstr ""
 
+msgctxt "help:web.shop,non_sale_price_list:"
+msgid ""
+"The price list to compute the price of products when it is not on sale."
+msgstr ""
+
 msgctxt "help:web.shop,products:"
 msgid "The list of products to publish."
 msgstr ""
 
 msgctxt "help:web.shop,products_removed:"
 msgid "The list of products to unpublish."
 msgstr ""
 
+msgctxt "help:web.shop,sale_price_list:"
+msgid "The price list to compute sale price of products."
+msgstr ""
+
 msgctxt "help:web.shop,type:"
 msgid "The front-end used for the web shop."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_shop"
 msgid "Web Shops"
 msgstr ""
@@ -192,14 +221,18 @@
 msgid "Web Shops"
 msgstr ""
 
 msgctxt "model:web.shop,name:"
 msgid "Web Shop"
 msgstr ""
 
+msgctxt "model:web.shop-country.country,name:"
+msgid "Web Shop - Country"
+msgstr ""
+
 msgctxt "model:web.shop-product.attribute,name:"
 msgid "Web Shop - Attribute"
 msgstr ""
 
 msgctxt "model:web.shop-product.category,name:"
 msgid "Web Shop - Product Category"
 msgstr ""
@@ -210,12 +243,12 @@
 
 msgctxt "model:web.shop-stock.location,name:"
 msgid "Web Shop - Warehouse"
 msgstr ""
 
 msgctxt "view:product.template:"
 msgid "Edit"
-msgstr "Sunting"
+msgstr ""
 
 msgctxt "view:web.shop:"
 msgid "Products"
-msgstr "Produk-Produk"
+msgstr ""
```

### Comparing `trytond_web_shop-7.2.0/locale/it.po` & `trytond_web_shop-7.2.1/locale/fi.po`

 * *Files 16% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 msgctxt "field:sale.sale,web_shop:"
 msgid "Web Shop"
 msgstr ""
 
 msgctxt "field:web.shop,attributes:"
 msgid "Attributes"
-msgstr "Attributi"
+msgstr ""
 
 msgctxt "field:web.shop,attributes_removed:"
 msgid "Attributes Removed"
 msgstr ""
 
 msgctxt "field:web.shop,categories:"
 msgid "Categories"
@@ -50,45 +50,65 @@
 msgid "Categories Removed"
 msgstr ""
 
 msgctxt "field:web.shop,company:"
 msgid "Company"
 msgstr ""
 
+msgctxt "field:web.shop,countries:"
+msgid "Countries"
+msgstr ""
+
 msgctxt "field:web.shop,currency:"
 msgid "Currency"
-msgstr "Valuta"
+msgstr ""
 
 msgctxt "field:web.shop,guest_party:"
 msgid "Guest Party"
 msgstr ""
 
 msgctxt "field:web.shop,language:"
 msgid "Language"
 msgstr ""
 
 msgctxt "field:web.shop,name:"
 msgid "Name"
 msgstr ""
 
+msgctxt "field:web.shop,non_sale_price_list:"
+msgid "Non-Sale Price List"
+msgstr ""
+
 msgctxt "field:web.shop,products:"
 msgid "Products"
 msgstr ""
 
 msgctxt "field:web.shop,products_removed:"
 msgid "Products Removed"
 msgstr ""
 
+msgctxt "field:web.shop,sale_price_list:"
+msgid "Sale Price List"
+msgstr ""
+
 msgctxt "field:web.shop,type:"
 msgid "Type"
 msgstr ""
 
 msgctxt "field:web.shop,warehouses:"
 msgid "Warehouses"
-msgstr "Magazzini"
+msgstr ""
+
+msgctxt "field:web.shop-country.country,country:"
+msgid "Country"
+msgstr ""
+
+msgctxt "field:web.shop-country.country,shop:"
+msgid "Shop"
+msgstr ""
 
 msgctxt "field:web.shop-product.attribute,attribute:"
 msgid "Attribute"
 msgstr ""
 
 msgctxt "field:web.shop-product.attribute,shop:"
 msgid "Shop"
@@ -100,35 +120,35 @@
 
 msgctxt "field:web.shop-product.category,shop:"
 msgid "Shop"
 msgstr ""
 
 msgctxt "field:web.shop-product.product,product:"
 msgid "Product"
-msgstr "Prodotto"
+msgstr ""
 
 msgctxt "field:web.shop-product.product,shop:"
 msgid "Shop"
 msgstr ""
 
 msgctxt "field:web.shop-stock.location,shop:"
 msgid "Shop"
 msgstr ""
 
 msgctxt "field:web.shop-stock.location,warehouse:"
 msgid "Warehouse"
-msgstr "Magazzino"
+msgstr ""
 
 msgctxt "field:web.user,invoice_address:"
 msgid "Invoice Address"
-msgstr "Indirizzo di fatturazione"
+msgstr ""
 
 msgctxt "field:web.user,shipment_address:"
 msgid "Shipment Address"
-msgstr "indirizzo di spedizione"
+msgstr ""
 
 msgctxt "help:product.attribute,web_shops:"
 msgid "The list of web shops on which the attribute is published."
 msgstr ""
 
 msgctxt "help:product.category,web_shops:"
 msgid "The list of web shops on which the category is published."
@@ -150,22 +170,31 @@
 msgid "The list of categories to publish."
 msgstr ""
 
 msgctxt "help:web.shop,categories_removed:"
 msgid "The list of categories to unpublish."
 msgstr ""
 
+msgctxt "help:web.shop,non_sale_price_list:"
+msgid ""
+"The price list to compute the price of products when it is not on sale."
+msgstr ""
+
 msgctxt "help:web.shop,products:"
 msgid "The list of products to publish."
 msgstr ""
 
 msgctxt "help:web.shop,products_removed:"
 msgid "The list of products to unpublish."
 msgstr ""
 
+msgctxt "help:web.shop,sale_price_list:"
+msgid "The price list to compute sale price of products."
+msgstr ""
+
 msgctxt "help:web.shop,type:"
 msgid "The front-end used for the web shop."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_shop"
 msgid "Web Shops"
 msgstr ""
@@ -192,14 +221,18 @@
 msgid "Web Shops"
 msgstr ""
 
 msgctxt "model:web.shop,name:"
 msgid "Web Shop"
 msgstr ""
 
+msgctxt "model:web.shop-country.country,name:"
+msgid "Web Shop - Country"
+msgstr ""
+
 msgctxt "model:web.shop-product.attribute,name:"
 msgid "Web Shop - Attribute"
 msgstr ""
 
 msgctxt "model:web.shop-product.category,name:"
 msgid "Web Shop - Product Category"
 msgstr ""
```

### Comparing `trytond_web_shop-7.2.0/locale/lo.po` & `trytond_web_shop-7.2.1/locale/lo.po`

 * *Files 18% similar despite different names*

```diff
@@ -50,14 +50,18 @@
 msgid "Categories Removed"
 msgstr ""
 
 msgctxt "field:web.shop,company:"
 msgid "Company"
 msgstr ""
 
+msgctxt "field:web.shop,countries:"
+msgid "Countries"
+msgstr ""
+
 msgctxt "field:web.shop,currency:"
 msgid "Currency"
 msgstr ""
 
 msgctxt "field:web.shop,guest_party:"
 msgid "Guest Party"
 msgstr ""
@@ -66,30 +70,46 @@
 msgid "Language"
 msgstr ""
 
 msgctxt "field:web.shop,name:"
 msgid "Name"
 msgstr ""
 
+msgctxt "field:web.shop,non_sale_price_list:"
+msgid "Non-Sale Price List"
+msgstr ""
+
 msgctxt "field:web.shop,products:"
 msgid "Products"
 msgstr ""
 
 msgctxt "field:web.shop,products_removed:"
 msgid "Products Removed"
 msgstr ""
 
+msgctxt "field:web.shop,sale_price_list:"
+msgid "Sale Price List"
+msgstr ""
+
 msgctxt "field:web.shop,type:"
 msgid "Type"
 msgstr ""
 
 msgctxt "field:web.shop,warehouses:"
 msgid "Warehouses"
 msgstr ""
 
+msgctxt "field:web.shop-country.country,country:"
+msgid "Country"
+msgstr ""
+
+msgctxt "field:web.shop-country.country,shop:"
+msgid "Shop"
+msgstr ""
+
 msgctxt "field:web.shop-product.attribute,attribute:"
 msgid "Attribute"
 msgstr ""
 
 msgctxt "field:web.shop-product.attribute,shop:"
 msgid "Shop"
 msgstr ""
@@ -150,22 +170,31 @@
 msgid "The list of categories to publish."
 msgstr ""
 
 msgctxt "help:web.shop,categories_removed:"
 msgid "The list of categories to unpublish."
 msgstr ""
 
+msgctxt "help:web.shop,non_sale_price_list:"
+msgid ""
+"The price list to compute the price of products when it is not on sale."
+msgstr ""
+
 msgctxt "help:web.shop,products:"
 msgid "The list of products to publish."
 msgstr ""
 
 msgctxt "help:web.shop,products_removed:"
 msgid "The list of products to unpublish."
 msgstr ""
 
+msgctxt "help:web.shop,sale_price_list:"
+msgid "The price list to compute sale price of products."
+msgstr ""
+
 msgctxt "help:web.shop,type:"
 msgid "The front-end used for the web shop."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_shop"
 msgid "Web Shops"
 msgstr ""
@@ -192,14 +221,18 @@
 msgid "Web Shops"
 msgstr ""
 
 msgctxt "model:web.shop,name:"
 msgid "Web Shop"
 msgstr ""
 
+msgctxt "model:web.shop-country.country,name:"
+msgid "Web Shop - Country"
+msgstr ""
+
 msgctxt "model:web.shop-product.attribute,name:"
 msgid "Web Shop - Attribute"
 msgstr ""
 
 msgctxt "model:web.shop-product.category,name:"
 msgid "Web Shop - Product Category"
 msgstr ""
```

### Comparing `trytond_web_shop-7.2.0/locale/lt.po` & `trytond_web_shop-7.2.1/locale/lt.po`

 * *Files 18% similar despite different names*

```diff
@@ -50,14 +50,18 @@
 msgid "Categories Removed"
 msgstr ""
 
 msgctxt "field:web.shop,company:"
 msgid "Company"
 msgstr ""
 
+msgctxt "field:web.shop,countries:"
+msgid "Countries"
+msgstr ""
+
 msgctxt "field:web.shop,currency:"
 msgid "Currency"
 msgstr ""
 
 msgctxt "field:web.shop,guest_party:"
 msgid "Guest Party"
 msgstr ""
@@ -66,30 +70,46 @@
 msgid "Language"
 msgstr ""
 
 msgctxt "field:web.shop,name:"
 msgid "Name"
 msgstr ""
 
+msgctxt "field:web.shop,non_sale_price_list:"
+msgid "Non-Sale Price List"
+msgstr ""
+
 msgctxt "field:web.shop,products:"
 msgid "Products"
 msgstr ""
 
 msgctxt "field:web.shop,products_removed:"
 msgid "Products Removed"
 msgstr ""
 
+msgctxt "field:web.shop,sale_price_list:"
+msgid "Sale Price List"
+msgstr ""
+
 msgctxt "field:web.shop,type:"
 msgid "Type"
 msgstr ""
 
 msgctxt "field:web.shop,warehouses:"
 msgid "Warehouses"
 msgstr ""
 
+msgctxt "field:web.shop-country.country,country:"
+msgid "Country"
+msgstr ""
+
+msgctxt "field:web.shop-country.country,shop:"
+msgid "Shop"
+msgstr ""
+
 msgctxt "field:web.shop-product.attribute,attribute:"
 msgid "Attribute"
 msgstr ""
 
 msgctxt "field:web.shop-product.attribute,shop:"
 msgid "Shop"
 msgstr ""
@@ -150,22 +170,31 @@
 msgid "The list of categories to publish."
 msgstr ""
 
 msgctxt "help:web.shop,categories_removed:"
 msgid "The list of categories to unpublish."
 msgstr ""
 
+msgctxt "help:web.shop,non_sale_price_list:"
+msgid ""
+"The price list to compute the price of products when it is not on sale."
+msgstr ""
+
 msgctxt "help:web.shop,products:"
 msgid "The list of products to publish."
 msgstr ""
 
 msgctxt "help:web.shop,products_removed:"
 msgid "The list of products to unpublish."
 msgstr ""
 
+msgctxt "help:web.shop,sale_price_list:"
+msgid "The price list to compute sale price of products."
+msgstr ""
+
 msgctxt "help:web.shop,type:"
 msgid "The front-end used for the web shop."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_shop"
 msgid "Web Shops"
 msgstr ""
@@ -192,14 +221,18 @@
 msgid "Web Shops"
 msgstr ""
 
 msgctxt "model:web.shop,name:"
 msgid "Web Shop"
 msgstr ""
 
+msgctxt "model:web.shop-country.country,name:"
+msgid "Web Shop - Country"
+msgstr ""
+
 msgctxt "model:web.shop-product.attribute,name:"
 msgid "Web Shop - Attribute"
 msgstr ""
 
 msgctxt "model:web.shop-product.category,name:"
 msgid "Web Shop - Product Category"
 msgstr ""
```

### Comparing `trytond_web_shop-7.2.0/locale/nl.po` & `trytond_web_shop-7.2.1/locale/nl.po`

 * *Files 14% similar despite different names*

```diff
@@ -50,14 +50,18 @@
 msgid "Categories Removed"
 msgstr "verwijderde Categorieën"
 
 msgctxt "field:web.shop,company:"
 msgid "Company"
 msgstr "Bedrijf"
 
+msgctxt "field:web.shop,countries:"
+msgid "Countries"
+msgstr "Landen"
+
 msgctxt "field:web.shop,currency:"
 msgid "Currency"
 msgstr "Valuta"
 
 msgctxt "field:web.shop,guest_party:"
 msgid "Guest Party"
 msgstr "Gast Relatie"
@@ -66,30 +70,46 @@
 msgid "Language"
 msgstr "Taal"
 
 msgctxt "field:web.shop,name:"
 msgid "Name"
 msgstr "Naam"
 
+msgctxt "field:web.shop,non_sale_price_list:"
+msgid "Non-Sale Price List"
+msgstr "Niet-verkoop prijslijst"
+
 msgctxt "field:web.shop,products:"
 msgid "Products"
 msgstr "Producten"
 
 msgctxt "field:web.shop,products_removed:"
 msgid "Products Removed"
 msgstr "Verwijderde Producten"
 
+msgctxt "field:web.shop,sale_price_list:"
+msgid "Sale Price List"
+msgstr "Verkoop prijslijst"
+
 msgctxt "field:web.shop,type:"
 msgid "Type"
 msgstr "Type"
 
 msgctxt "field:web.shop,warehouses:"
 msgid "Warehouses"
 msgstr "Magazijn"
 
+msgctxt "field:web.shop-country.country,country:"
+msgid "Country"
+msgstr "Land"
+
+msgctxt "field:web.shop-country.country,shop:"
+msgid "Shop"
+msgstr "Winkel"
+
 msgctxt "field:web.shop-product.attribute,attribute:"
 msgid "Attribute"
 msgstr "Attribuut"
 
 msgctxt "field:web.shop-product.attribute,shop:"
 msgid "Shop"
 msgstr "Winkel"
@@ -151,23 +171,34 @@
 msgstr "De lijst met te publiceren categorieën."
 
 msgctxt "help:web.shop,categories_removed:"
 msgid "The list of categories to unpublish."
 msgstr ""
 "De lijst met categorieën waarvan de publicatie ongedaan moet worden gemaakt."
 
+msgctxt "help:web.shop,non_sale_price_list:"
+msgid ""
+"The price list to compute the price of products when it is not on sale."
+msgstr ""
+"De prijslijst om de prijs van producten te berekenen wanneer deze niet in de"
+" uitverkoop zijn."
+
 msgctxt "help:web.shop,products:"
 msgid "The list of products to publish."
 msgstr "De lijst met te publiceren producten."
 
 msgctxt "help:web.shop,products_removed:"
 msgid "The list of products to unpublish."
 msgstr ""
 "De lijst met producten waarvan de publicatie ongedaan moet worden gemaakt."
 
+msgctxt "help:web.shop,sale_price_list:"
+msgid "The price list to compute sale price of products."
+msgstr "De prijslijst om de verkoopprijs van producten te berekenen."
+
 msgctxt "help:web.shop,type:"
 msgid "The front-end used for the web shop."
 msgstr "De front-end die wordt gebruikt voor de webshop."
 
 msgctxt "model:ir.action,name:act_shop"
 msgid "Web Shops"
 msgstr "Webwinkels"
@@ -196,14 +227,18 @@
 msgid "Web Shops"
 msgstr "Webwinkels"
 
 msgctxt "model:web.shop,name:"
 msgid "Web Shop"
 msgstr "Webwinkels"
 
+msgctxt "model:web.shop-country.country,name:"
+msgid "Web Shop - Country"
+msgstr "Webwinkel - Land"
+
 msgctxt "model:web.shop-product.attribute,name:"
 msgid "Web Shop - Attribute"
 msgstr "Webwinkel - Kenmerk"
 
 msgctxt "model:web.shop-product.category,name:"
 msgid "Web Shop - Product Category"
 msgstr "Webwinkel - Productcategorie"
```

### Comparing `trytond_web_shop-7.2.0/locale/pl.po` & `trytond_web_shop-7.2.1/locale/pl.po`

 * *Files 18% similar despite different names*

```diff
@@ -50,14 +50,18 @@
 msgid "Categories Removed"
 msgstr ""
 
 msgctxt "field:web.shop,company:"
 msgid "Company"
 msgstr ""
 
+msgctxt "field:web.shop,countries:"
+msgid "Countries"
+msgstr ""
+
 msgctxt "field:web.shop,currency:"
 msgid "Currency"
 msgstr ""
 
 msgctxt "field:web.shop,guest_party:"
 msgid "Guest Party"
 msgstr ""
@@ -66,30 +70,46 @@
 msgid "Language"
 msgstr ""
 
 msgctxt "field:web.shop,name:"
 msgid "Name"
 msgstr ""
 
+msgctxt "field:web.shop,non_sale_price_list:"
+msgid "Non-Sale Price List"
+msgstr ""
+
 msgctxt "field:web.shop,products:"
 msgid "Products"
 msgstr ""
 
 msgctxt "field:web.shop,products_removed:"
 msgid "Products Removed"
 msgstr ""
 
+msgctxt "field:web.shop,sale_price_list:"
+msgid "Sale Price List"
+msgstr ""
+
 msgctxt "field:web.shop,type:"
 msgid "Type"
 msgstr ""
 
 msgctxt "field:web.shop,warehouses:"
 msgid "Warehouses"
 msgstr ""
 
+msgctxt "field:web.shop-country.country,country:"
+msgid "Country"
+msgstr ""
+
+msgctxt "field:web.shop-country.country,shop:"
+msgid "Shop"
+msgstr ""
+
 msgctxt "field:web.shop-product.attribute,attribute:"
 msgid "Attribute"
 msgstr ""
 
 msgctxt "field:web.shop-product.attribute,shop:"
 msgid "Shop"
 msgstr ""
@@ -150,22 +170,31 @@
 msgid "The list of categories to publish."
 msgstr ""
 
 msgctxt "help:web.shop,categories_removed:"
 msgid "The list of categories to unpublish."
 msgstr ""
 
+msgctxt "help:web.shop,non_sale_price_list:"
+msgid ""
+"The price list to compute the price of products when it is not on sale."
+msgstr ""
+
 msgctxt "help:web.shop,products:"
 msgid "The list of products to publish."
 msgstr ""
 
 msgctxt "help:web.shop,products_removed:"
 msgid "The list of products to unpublish."
 msgstr ""
 
+msgctxt "help:web.shop,sale_price_list:"
+msgid "The price list to compute sale price of products."
+msgstr ""
+
 msgctxt "help:web.shop,type:"
 msgid "The front-end used for the web shop."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_shop"
 msgid "Web Shops"
 msgstr ""
@@ -192,14 +221,18 @@
 msgid "Web Shops"
 msgstr ""
 
 msgctxt "model:web.shop,name:"
 msgid "Web Shop"
 msgstr ""
 
+msgctxt "model:web.shop-country.country,name:"
+msgid "Web Shop - Country"
+msgstr ""
+
 msgctxt "model:web.shop-product.attribute,name:"
 msgid "Web Shop - Attribute"
 msgstr ""
 
 msgctxt "model:web.shop-product.category,name:"
 msgid "Web Shop - Product Category"
 msgstr ""
```

### Comparing `trytond_web_shop-7.2.0/locale/pt.po` & `trytond_web_shop-7.2.1/locale/pt.po`

 * *Files 18% similar despite different names*

```diff
@@ -50,14 +50,18 @@
 msgid "Categories Removed"
 msgstr ""
 
 msgctxt "field:web.shop,company:"
 msgid "Company"
 msgstr ""
 
+msgctxt "field:web.shop,countries:"
+msgid "Countries"
+msgstr ""
+
 msgctxt "field:web.shop,currency:"
 msgid "Currency"
 msgstr ""
 
 msgctxt "field:web.shop,guest_party:"
 msgid "Guest Party"
 msgstr ""
@@ -66,30 +70,46 @@
 msgid "Language"
 msgstr ""
 
 msgctxt "field:web.shop,name:"
 msgid "Name"
 msgstr ""
 
+msgctxt "field:web.shop,non_sale_price_list:"
+msgid "Non-Sale Price List"
+msgstr ""
+
 msgctxt "field:web.shop,products:"
 msgid "Products"
 msgstr ""
 
 msgctxt "field:web.shop,products_removed:"
 msgid "Products Removed"
 msgstr ""
 
+msgctxt "field:web.shop,sale_price_list:"
+msgid "Sale Price List"
+msgstr ""
+
 msgctxt "field:web.shop,type:"
 msgid "Type"
 msgstr ""
 
 msgctxt "field:web.shop,warehouses:"
 msgid "Warehouses"
 msgstr ""
 
+msgctxt "field:web.shop-country.country,country:"
+msgid "Country"
+msgstr ""
+
+msgctxt "field:web.shop-country.country,shop:"
+msgid "Shop"
+msgstr ""
+
 msgctxt "field:web.shop-product.attribute,attribute:"
 msgid "Attribute"
 msgstr ""
 
 msgctxt "field:web.shop-product.attribute,shop:"
 msgid "Shop"
 msgstr ""
@@ -150,22 +170,31 @@
 msgid "The list of categories to publish."
 msgstr ""
 
 msgctxt "help:web.shop,categories_removed:"
 msgid "The list of categories to unpublish."
 msgstr ""
 
+msgctxt "help:web.shop,non_sale_price_list:"
+msgid ""
+"The price list to compute the price of products when it is not on sale."
+msgstr ""
+
 msgctxt "help:web.shop,products:"
 msgid "The list of products to publish."
 msgstr ""
 
 msgctxt "help:web.shop,products_removed:"
 msgid "The list of products to unpublish."
 msgstr ""
 
+msgctxt "help:web.shop,sale_price_list:"
+msgid "The price list to compute sale price of products."
+msgstr ""
+
 msgctxt "help:web.shop,type:"
 msgid "The front-end used for the web shop."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_shop"
 msgid "Web Shops"
 msgstr ""
@@ -192,14 +221,18 @@
 msgid "Web Shops"
 msgstr ""
 
 msgctxt "model:web.shop,name:"
 msgid "Web Shop"
 msgstr ""
 
+msgctxt "model:web.shop-country.country,name:"
+msgid "Web Shop - Country"
+msgstr ""
+
 msgctxt "model:web.shop-product.attribute,name:"
 msgid "Web Shop - Attribute"
 msgstr ""
 
 msgctxt "model:web.shop-product.category,name:"
 msgid "Web Shop - Product Category"
 msgstr ""
```

### Comparing `trytond_web_shop-7.2.0/locale/ro.po` & `trytond_web_shop-7.2.1/locale/ro.po`

 * *Files 18% similar despite different names*

```diff
@@ -50,14 +50,18 @@
 msgid "Categories Removed"
 msgstr ""
 
 msgctxt "field:web.shop,company:"
 msgid "Company"
 msgstr ""
 
+msgctxt "field:web.shop,countries:"
+msgid "Countries"
+msgstr ""
+
 msgctxt "field:web.shop,currency:"
 msgid "Currency"
 msgstr ""
 
 msgctxt "field:web.shop,guest_party:"
 msgid "Guest Party"
 msgstr ""
@@ -66,30 +70,46 @@
 msgid "Language"
 msgstr ""
 
 msgctxt "field:web.shop,name:"
 msgid "Name"
 msgstr ""
 
+msgctxt "field:web.shop,non_sale_price_list:"
+msgid "Non-Sale Price List"
+msgstr ""
+
 msgctxt "field:web.shop,products:"
 msgid "Products"
 msgstr ""
 
 msgctxt "field:web.shop,products_removed:"
 msgid "Products Removed"
 msgstr ""
 
+msgctxt "field:web.shop,sale_price_list:"
+msgid "Sale Price List"
+msgstr ""
+
 msgctxt "field:web.shop,type:"
 msgid "Type"
 msgstr ""
 
 msgctxt "field:web.shop,warehouses:"
 msgid "Warehouses"
 msgstr ""
 
+msgctxt "field:web.shop-country.country,country:"
+msgid "Country"
+msgstr ""
+
+msgctxt "field:web.shop-country.country,shop:"
+msgid "Shop"
+msgstr ""
+
 msgctxt "field:web.shop-product.attribute,attribute:"
 msgid "Attribute"
 msgstr ""
 
 msgctxt "field:web.shop-product.attribute,shop:"
 msgid "Shop"
 msgstr ""
@@ -150,22 +170,31 @@
 msgid "The list of categories to publish."
 msgstr ""
 
 msgctxt "help:web.shop,categories_removed:"
 msgid "The list of categories to unpublish."
 msgstr ""
 
+msgctxt "help:web.shop,non_sale_price_list:"
+msgid ""
+"The price list to compute the price of products when it is not on sale."
+msgstr ""
+
 msgctxt "help:web.shop,products:"
 msgid "The list of products to publish."
 msgstr ""
 
 msgctxt "help:web.shop,products_removed:"
 msgid "The list of products to unpublish."
 msgstr ""
 
+msgctxt "help:web.shop,sale_price_list:"
+msgid "The price list to compute sale price of products."
+msgstr ""
+
 msgctxt "help:web.shop,type:"
 msgid "The front-end used for the web shop."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_shop"
 msgid "Web Shops"
 msgstr ""
@@ -192,14 +221,18 @@
 msgid "Web Shops"
 msgstr ""
 
 msgctxt "model:web.shop,name:"
 msgid "Web Shop"
 msgstr ""
 
+msgctxt "model:web.shop-country.country,name:"
+msgid "Web Shop - Country"
+msgstr ""
+
 msgctxt "model:web.shop-product.attribute,name:"
 msgid "Web Shop - Attribute"
 msgstr ""
 
 msgctxt "model:web.shop-product.category,name:"
 msgid "Web Shop - Product Category"
 msgstr ""
```

### Comparing `trytond_web_shop-7.2.0/locale/ru.po` & `trytond_web_shop-7.2.1/locale/ru.po`

 * *Files 18% similar despite different names*

```diff
@@ -50,14 +50,18 @@
 msgid "Categories Removed"
 msgstr ""
 
 msgctxt "field:web.shop,company:"
 msgid "Company"
 msgstr ""
 
+msgctxt "field:web.shop,countries:"
+msgid "Countries"
+msgstr ""
+
 msgctxt "field:web.shop,currency:"
 msgid "Currency"
 msgstr ""
 
 msgctxt "field:web.shop,guest_party:"
 msgid "Guest Party"
 msgstr ""
@@ -66,30 +70,46 @@
 msgid "Language"
 msgstr ""
 
 msgctxt "field:web.shop,name:"
 msgid "Name"
 msgstr ""
 
+msgctxt "field:web.shop,non_sale_price_list:"
+msgid "Non-Sale Price List"
+msgstr ""
+
 msgctxt "field:web.shop,products:"
 msgid "Products"
 msgstr ""
 
 msgctxt "field:web.shop,products_removed:"
 msgid "Products Removed"
 msgstr ""
 
+msgctxt "field:web.shop,sale_price_list:"
+msgid "Sale Price List"
+msgstr ""
+
 msgctxt "field:web.shop,type:"
 msgid "Type"
 msgstr ""
 
 msgctxt "field:web.shop,warehouses:"
 msgid "Warehouses"
 msgstr ""
 
+msgctxt "field:web.shop-country.country,country:"
+msgid "Country"
+msgstr ""
+
+msgctxt "field:web.shop-country.country,shop:"
+msgid "Shop"
+msgstr ""
+
 msgctxt "field:web.shop-product.attribute,attribute:"
 msgid "Attribute"
 msgstr ""
 
 msgctxt "field:web.shop-product.attribute,shop:"
 msgid "Shop"
 msgstr ""
@@ -150,22 +170,31 @@
 msgid "The list of categories to publish."
 msgstr ""
 
 msgctxt "help:web.shop,categories_removed:"
 msgid "The list of categories to unpublish."
 msgstr ""
 
+msgctxt "help:web.shop,non_sale_price_list:"
+msgid ""
+"The price list to compute the price of products when it is not on sale."
+msgstr ""
+
 msgctxt "help:web.shop,products:"
 msgid "The list of products to publish."
 msgstr ""
 
 msgctxt "help:web.shop,products_removed:"
 msgid "The list of products to unpublish."
 msgstr ""
 
+msgctxt "help:web.shop,sale_price_list:"
+msgid "The price list to compute sale price of products."
+msgstr ""
+
 msgctxt "help:web.shop,type:"
 msgid "The front-end used for the web shop."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_shop"
 msgid "Web Shops"
 msgstr ""
@@ -192,14 +221,18 @@
 msgid "Web Shops"
 msgstr ""
 
 msgctxt "model:web.shop,name:"
 msgid "Web Shop"
 msgstr ""
 
+msgctxt "model:web.shop-country.country,name:"
+msgid "Web Shop - Country"
+msgstr ""
+
 msgctxt "model:web.shop-product.attribute,name:"
 msgid "Web Shop - Attribute"
 msgstr ""
 
 msgctxt "model:web.shop-product.category,name:"
 msgid "Web Shop - Product Category"
 msgstr ""
```

### Comparing `trytond_web_shop-7.2.0/locale/sl.po` & `trytond_web_shop-7.2.1/locale/sl.po`

 * *Files 6% similar despite different names*

```diff
@@ -50,14 +50,19 @@
 msgid "Categories Removed"
 msgstr "Odstranjene kategorije"
 
 msgctxt "field:web.shop,company:"
 msgid "Company"
 msgstr "Družba"
 
+#, fuzzy
+msgctxt "field:web.shop,countries:"
+msgid "Countries"
+msgstr "Kategorije"
+
 msgctxt "field:web.shop,currency:"
 msgid "Currency"
 msgstr "Valuta"
 
 msgctxt "field:web.shop,guest_party:"
 msgid "Guest Party"
 msgstr "Partner gost"
@@ -66,30 +71,47 @@
 msgid "Language"
 msgstr "Jezik"
 
 msgctxt "field:web.shop,name:"
 msgid "Name"
 msgstr "Naziv"
 
+msgctxt "field:web.shop,non_sale_price_list:"
+msgid "Non-Sale Price List"
+msgstr ""
+
 msgctxt "field:web.shop,products:"
 msgid "Products"
 msgstr "Izdelki"
 
 msgctxt "field:web.shop,products_removed:"
 msgid "Products Removed"
 msgstr "Odstranjeni izdeleki"
 
+msgctxt "field:web.shop,sale_price_list:"
+msgid "Sale Price List"
+msgstr ""
+
 msgctxt "field:web.shop,type:"
 msgid "Type"
 msgstr "Vrsta"
 
 msgctxt "field:web.shop,warehouses:"
 msgid "Warehouses"
 msgstr "Skladišča"
 
+msgctxt "field:web.shop-country.country,country:"
+msgid "Country"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:web.shop-country.country,shop:"
+msgid "Shop"
+msgstr "Trgovina"
+
 msgctxt "field:web.shop-product.attribute,attribute:"
 msgid "Attribute"
 msgstr "Atribut"
 
 msgctxt "field:web.shop-product.attribute,shop:"
 msgid "Shop"
 msgstr "Trgovina"
@@ -150,22 +172,31 @@
 msgid "The list of categories to publish."
 msgstr "Seznam kategorij za objavo."
 
 msgctxt "help:web.shop,categories_removed:"
 msgid "The list of categories to unpublish."
 msgstr "Seznam kategorij za odstranitev iz objave."
 
+msgctxt "help:web.shop,non_sale_price_list:"
+msgid ""
+"The price list to compute the price of products when it is not on sale."
+msgstr ""
+
 msgctxt "help:web.shop,products:"
 msgid "The list of products to publish."
 msgstr "Seznam izdelekov za objavo."
 
 msgctxt "help:web.shop,products_removed:"
 msgid "The list of products to unpublish."
 msgstr "Seznam izdelekov za odstranitev iz objave."
 
+msgctxt "help:web.shop,sale_price_list:"
+msgid "The price list to compute sale price of products."
+msgstr ""
+
 msgctxt "help:web.shop,type:"
 msgid "The front-end used for the web shop."
 msgstr "Frontend, ki ga uporablja spletna trgovina."
 
 msgctxt "model:ir.action,name:act_shop"
 msgid "Web Shops"
 msgstr "Spletne trgovine"
@@ -194,14 +225,19 @@
 msgid "Web Shops"
 msgstr "Spletne trgovine"
 
 msgctxt "model:web.shop,name:"
 msgid "Web Shop"
 msgstr "Spletna trgovina"
 
+#, fuzzy
+msgctxt "model:web.shop-country.country,name:"
+msgid "Web Shop - Country"
+msgstr "Spletna trgovina - Izdelek"
+
 msgctxt "model:web.shop-product.attribute,name:"
 msgid "Web Shop - Attribute"
 msgstr "Spletna trgovina - Atribut"
 
 msgctxt "model:web.shop-product.category,name:"
 msgid "Web Shop - Product Category"
 msgstr "Spletna trgovina - Kategorija izdeleka"
```

### Comparing `trytond_web_shop-7.2.0/locale/tr.po` & `trytond_web_shop-7.2.1/locale/tr.po`

 * *Files 18% similar despite different names*

```diff
@@ -50,14 +50,18 @@
 msgid "Categories Removed"
 msgstr ""
 
 msgctxt "field:web.shop,company:"
 msgid "Company"
 msgstr ""
 
+msgctxt "field:web.shop,countries:"
+msgid "Countries"
+msgstr ""
+
 msgctxt "field:web.shop,currency:"
 msgid "Currency"
 msgstr ""
 
 msgctxt "field:web.shop,guest_party:"
 msgid "Guest Party"
 msgstr ""
@@ -66,30 +70,46 @@
 msgid "Language"
 msgstr ""
 
 msgctxt "field:web.shop,name:"
 msgid "Name"
 msgstr ""
 
+msgctxt "field:web.shop,non_sale_price_list:"
+msgid "Non-Sale Price List"
+msgstr ""
+
 msgctxt "field:web.shop,products:"
 msgid "Products"
 msgstr ""
 
 msgctxt "field:web.shop,products_removed:"
 msgid "Products Removed"
 msgstr ""
 
+msgctxt "field:web.shop,sale_price_list:"
+msgid "Sale Price List"
+msgstr ""
+
 msgctxt "field:web.shop,type:"
 msgid "Type"
 msgstr ""
 
 msgctxt "field:web.shop,warehouses:"
 msgid "Warehouses"
 msgstr ""
 
+msgctxt "field:web.shop-country.country,country:"
+msgid "Country"
+msgstr ""
+
+msgctxt "field:web.shop-country.country,shop:"
+msgid "Shop"
+msgstr ""
+
 msgctxt "field:web.shop-product.attribute,attribute:"
 msgid "Attribute"
 msgstr ""
 
 msgctxt "field:web.shop-product.attribute,shop:"
 msgid "Shop"
 msgstr ""
@@ -150,22 +170,31 @@
 msgid "The list of categories to publish."
 msgstr ""
 
 msgctxt "help:web.shop,categories_removed:"
 msgid "The list of categories to unpublish."
 msgstr ""
 
+msgctxt "help:web.shop,non_sale_price_list:"
+msgid ""
+"The price list to compute the price of products when it is not on sale."
+msgstr ""
+
 msgctxt "help:web.shop,products:"
 msgid "The list of products to publish."
 msgstr ""
 
 msgctxt "help:web.shop,products_removed:"
 msgid "The list of products to unpublish."
 msgstr ""
 
+msgctxt "help:web.shop,sale_price_list:"
+msgid "The price list to compute sale price of products."
+msgstr ""
+
 msgctxt "help:web.shop,type:"
 msgid "The front-end used for the web shop."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_shop"
 msgid "Web Shops"
 msgstr ""
@@ -192,14 +221,18 @@
 msgid "Web Shops"
 msgstr ""
 
 msgctxt "model:web.shop,name:"
 msgid "Web Shop"
 msgstr ""
 
+msgctxt "model:web.shop-country.country,name:"
+msgid "Web Shop - Country"
+msgstr ""
+
 msgctxt "model:web.shop-product.attribute,name:"
 msgid "Web Shop - Attribute"
 msgstr ""
 
 msgctxt "model:web.shop-product.category,name:"
 msgid "Web Shop - Product Category"
 msgstr ""
```

### Comparing `trytond_web_shop-7.2.0/locale/uk.po` & `trytond_web_shop-7.2.1/locale/uk.po`

 * *Files 4% similar despite different names*

```diff
@@ -50,14 +50,19 @@
 msgid "Categories Removed"
 msgstr "Категорії видалено"
 
 msgctxt "field:web.shop,company:"
 msgid "Company"
 msgstr "Компанія"
 
+#, fuzzy
+msgctxt "field:web.shop,countries:"
+msgid "Countries"
+msgstr "Категорії"
+
 msgctxt "field:web.shop,currency:"
 msgid "Currency"
 msgstr "Валюта"
 
 msgctxt "field:web.shop,guest_party:"
 msgid "Guest Party"
 msgstr "Гостьова особа"
@@ -66,30 +71,47 @@
 msgid "Language"
 msgstr "Мова"
 
 msgctxt "field:web.shop,name:"
 msgid "Name"
 msgstr "Назва"
 
+msgctxt "field:web.shop,non_sale_price_list:"
+msgid "Non-Sale Price List"
+msgstr ""
+
 msgctxt "field:web.shop,products:"
 msgid "Products"
 msgstr "Товари"
 
 msgctxt "field:web.shop,products_removed:"
 msgid "Products Removed"
 msgstr "Товари видалено"
 
+msgctxt "field:web.shop,sale_price_list:"
+msgid "Sale Price List"
+msgstr ""
+
 msgctxt "field:web.shop,type:"
 msgid "Type"
 msgstr "Тип"
 
 msgctxt "field:web.shop,warehouses:"
 msgid "Warehouses"
 msgstr "Склади"
 
+msgctxt "field:web.shop-country.country,country:"
+msgid "Country"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:web.shop-country.country,shop:"
+msgid "Shop"
+msgstr "Магазин"
+
 msgctxt "field:web.shop-product.attribute,attribute:"
 msgid "Attribute"
 msgstr "Атрибут"
 
 msgctxt "field:web.shop-product.attribute,shop:"
 msgid "Shop"
 msgstr "Магазин"
@@ -150,22 +172,31 @@
 msgid "The list of categories to publish."
 msgstr "Список категорій для публікації."
 
 msgctxt "help:web.shop,categories_removed:"
 msgid "The list of categories to unpublish."
 msgstr "Список категорій, публікацію яких потрібно скасувати."
 
+msgctxt "help:web.shop,non_sale_price_list:"
+msgid ""
+"The price list to compute the price of products when it is not on sale."
+msgstr ""
+
 msgctxt "help:web.shop,products:"
 msgid "The list of products to publish."
 msgstr "Список товарів для публікації."
 
 msgctxt "help:web.shop,products_removed:"
 msgid "The list of products to unpublish."
 msgstr "Список товарів, публікацію яких потрібно скасувати."
 
+msgctxt "help:web.shop,sale_price_list:"
+msgid "The price list to compute sale price of products."
+msgstr ""
+
 msgctxt "help:web.shop,type:"
 msgid "The front-end used for the web shop."
 msgstr "Інтерфейс, який використовується для веб-магазину."
 
 msgctxt "model:ir.action,name:act_shop"
 msgid "Web Shops"
 msgstr "Веб-магазини"
@@ -194,14 +225,19 @@
 msgid "Web Shops"
 msgstr "Веб-магазини"
 
 msgctxt "model:web.shop,name:"
 msgid "Web Shop"
 msgstr "Веб-магазин"
 
+#, fuzzy
+msgctxt "model:web.shop-country.country,name:"
+msgid "Web Shop - Country"
+msgstr "Веб-магазин - Товар"
+
 msgctxt "model:web.shop-product.attribute,name:"
 msgid "Web Shop - Attribute"
 msgstr "Веб-магазин – Атрибут"
 
 msgctxt "model:web.shop-product.category,name:"
 msgid "Web Shop - Product Category"
 msgstr "Веб-магазин – Категорія товару"
```

### Comparing `trytond_web_shop-7.2.0/locale/zh_CN.po` & `trytond_web_shop-7.2.1/locale/zh_CN.po`

 * *Files 18% similar despite different names*

```diff
@@ -50,14 +50,18 @@
 msgid "Categories Removed"
 msgstr ""
 
 msgctxt "field:web.shop,company:"
 msgid "Company"
 msgstr ""
 
+msgctxt "field:web.shop,countries:"
+msgid "Countries"
+msgstr ""
+
 msgctxt "field:web.shop,currency:"
 msgid "Currency"
 msgstr ""
 
 msgctxt "field:web.shop,guest_party:"
 msgid "Guest Party"
 msgstr ""
@@ -66,30 +70,46 @@
 msgid "Language"
 msgstr ""
 
 msgctxt "field:web.shop,name:"
 msgid "Name"
 msgstr ""
 
+msgctxt "field:web.shop,non_sale_price_list:"
+msgid "Non-Sale Price List"
+msgstr ""
+
 msgctxt "field:web.shop,products:"
 msgid "Products"
 msgstr ""
 
 msgctxt "field:web.shop,products_removed:"
 msgid "Products Removed"
 msgstr ""
 
+msgctxt "field:web.shop,sale_price_list:"
+msgid "Sale Price List"
+msgstr ""
+
 msgctxt "field:web.shop,type:"
 msgid "Type"
 msgstr ""
 
 msgctxt "field:web.shop,warehouses:"
 msgid "Warehouses"
 msgstr ""
 
+msgctxt "field:web.shop-country.country,country:"
+msgid "Country"
+msgstr ""
+
+msgctxt "field:web.shop-country.country,shop:"
+msgid "Shop"
+msgstr ""
+
 msgctxt "field:web.shop-product.attribute,attribute:"
 msgid "Attribute"
 msgstr ""
 
 msgctxt "field:web.shop-product.attribute,shop:"
 msgid "Shop"
 msgstr ""
@@ -150,22 +170,31 @@
 msgid "The list of categories to publish."
 msgstr ""
 
 msgctxt "help:web.shop,categories_removed:"
 msgid "The list of categories to unpublish."
 msgstr ""
 
+msgctxt "help:web.shop,non_sale_price_list:"
+msgid ""
+"The price list to compute the price of products when it is not on sale."
+msgstr ""
+
 msgctxt "help:web.shop,products:"
 msgid "The list of products to publish."
 msgstr ""
 
 msgctxt "help:web.shop,products_removed:"
 msgid "The list of products to unpublish."
 msgstr ""
 
+msgctxt "help:web.shop,sale_price_list:"
+msgid "The price list to compute sale price of products."
+msgstr ""
+
 msgctxt "help:web.shop,type:"
 msgid "The front-end used for the web shop."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_shop"
 msgid "Web Shops"
 msgstr ""
@@ -192,14 +221,18 @@
 msgid "Web Shops"
 msgstr ""
 
 msgctxt "model:web.shop,name:"
 msgid "Web Shop"
 msgstr ""
 
+msgctxt "model:web.shop-country.country,name:"
+msgid "Web Shop - Country"
+msgstr ""
+
 msgctxt "model:web.shop-product.attribute,name:"
 msgid "Web Shop - Attribute"
 msgstr ""
 
 msgctxt "model:web.shop-product.category,name:"
 msgid "Web Shop - Product Category"
 msgstr ""
```

### Comparing `trytond_web_shop-7.2.0/message.xml` & `trytond_web_shop-7.2.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.2.0/product.py` & `trytond_web_shop-7.2.1/product.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.2.0/product.xml` & `trytond_web_shop-7.2.1/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.2.0/sale.py` & `trytond_web_shop-7.2.1/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.2.0/setup.py` & `trytond_web_shop-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.2.0/tox.ini` & `trytond_web_shop-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.2.0/trytond_web_shop.egg-info/PKG-INFO` & `trytond_web_shop-7.2.1/trytond_web_shop.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_web_shop
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module that provides a common base for webshops
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_web_shop-7.2.0/trytond_web_shop.egg-info/SOURCES.txt` & `trytond_web_shop-7.2.1/trytond_web_shop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.2.0/view/shop_form.xml` & `trytond_web_shop-7.2.1/view/shop_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.2.0/web.py` & `trytond_web_shop-7.2.1/web.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.2.0/web.xml` & `trytond_web_shop-7.2.1/web.xml`

 * *Files identical despite different names*

