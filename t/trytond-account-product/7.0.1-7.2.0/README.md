# Comparing `tmp/trytond_account_product-7.0.1.tar.gz` & `tmp/trytond_account_product-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_product-7.0.1.tar", last modified: Wed May  1 12:18:19 2024, max compression
+gzip compressed data, was "trytond_account_product-7.2.0.tar", last modified: Mon Apr 29 15:35:22 2024, max compression
```

## Comparing `trytond_account_product-7.0.1.tar` & `trytond_account_product-7.2.0.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:18:19.870988 trytond_account_product-7.0.1/
--rw-r--r--   0 ced       (1000) ced       (1000)     4118 2024-05-01 12:18:16.000000 trytond_account_product-7.0.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      763 2024-05-01 12:18:16.000000 trytond_account_product-7.0.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_account_product-7.0.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_account_product-7.0.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2869 2024-05-01 12:18:19.870988 trytond_account_product-7.0.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      345 2023-10-30 17:06:38.000000 trytond_account_product-7.0.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      968 2023-10-30 17:06:38.000000 trytond_account_product-7.0.1/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3210 2023-10-30 17:06:38.000000 trytond_account_product-7.0.1/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1000 2023-10-30 17:06:38.000000 trytond_account_product-7.0.1/account.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1082 2023-10-30 17:06:38.000000 trytond_account_product-7.0.1/analytic_account.py
--rw-r--r--   0 ced       (1000) ced       (1000)      827 2023-10-30 17:06:38.000000 trytond_account_product-7.0.1/analytic_account.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1817 2023-10-30 17:06:38.000000 trytond_account_product-7.0.1/configuration.py
--rw-r--r--   0 ced       (1000) ced       (1000)      490 2023-10-30 17:06:38.000000 trytond_account_product-7.0.1/configuration.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:18:19.864321 trytond_account_product-7.0.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2794 2024-03-03 16:24:20.000000 trytond_account_product-7.0.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1917 2023-10-30 17:06:38.000000 trytond_account_product-7.0.1/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      345 2023-10-30 17:06:38.000000 trytond_account_product-7.0.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-10-30 17:06:38.000000 trytond_account_product-7.0.1/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_account_product-7.0.1/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     1052 2023-10-30 17:06:38.000000 trytond_account_product-7.0.1/doc/usage.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      333 2023-10-30 17:06:38.000000 trytond_account_product-7.0.1/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:18:19.867654 trytond_account_product-7.0.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     6065 2023-10-30 17:06:38.000000 trytond_account_product-7.0.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6173 2023-10-30 17:06:38.000000 trytond_account_product-7.0.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4930 2023-10-30 17:06:38.000000 trytond_account_product-7.0.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6164 2023-10-30 17:06:38.000000 trytond_account_product-7.0.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6206 2023-10-30 17:06:38.000000 trytond_account_product-7.0.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5275 2023-10-30 17:06:38.000000 trytond_account_product-7.0.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5923 2023-10-30 17:06:38.000000 trytond_account_product-7.0.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6770 2023-10-30 17:06:38.000000 trytond_account_product-7.0.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4930 2023-10-30 17:06:38.000000 trytond_account_product-7.0.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6243 2023-10-30 17:06:38.000000 trytond_account_product-7.0.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5845 2023-10-30 17:06:38.000000 trytond_account_product-7.0.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5142 2023-10-30 17:06:38.000000 trytond_account_product-7.0.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6158 2023-10-30 17:06:38.000000 trytond_account_product-7.0.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6253 2023-10-30 17:06:38.000000 trytond_account_product-7.0.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5034 2023-10-30 17:06:38.000000 trytond_account_product-7.0.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6486 2023-10-30 17:06:38.000000 trytond_account_product-7.0.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5050 2023-10-30 17:06:38.000000 trytond_account_product-7.0.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5950 2023-10-30 17:06:38.000000 trytond_account_product-7.0.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6023 2023-10-30 17:06:38.000000 trytond_account_product-7.0.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6209 2023-10-30 17:06:38.000000 trytond_account_product-7.0.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6049 2023-10-30 17:06:38.000000 trytond_account_product-7.0.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4930 2023-10-30 17:06:38.000000 trytond_account_product-7.0.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4930 2023-10-30 17:06:38.000000 trytond_account_product-7.0.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5721 2023-10-30 17:06:38.000000 trytond_account_product-7.0.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      567 2023-10-30 17:06:38.000000 trytond_account_product-7.0.1/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    15495 2024-04-27 05:19:51.000000 trytond_account_product-7.0.1/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3202 2023-10-30 17:06:38.000000 trytond_account_product-7.0.1/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 12:18:19.870988 trytond_account_product-7.0.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4573 2024-03-03 16:24:03.000000 trytond_account_product-7.0.1/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:18:19.867654 trytond_account_product-7.0.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_account_product-7.0.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4093 2023-10-30 17:06:38.000000 trytond_account_product-7.0.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_account_product-7.0.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      211 2024-02-05 16:24:27.000000 trytond_account_product-7.0.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:18:19.870988 trytond_account_product-7.0.1/trytond_account_product.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2869 2024-05-01 12:18:19.000000 trytond_account_product-7.0.1/trytond_account_product.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2056 2024-05-01 12:18:19.000000 trytond_account_product-7.0.1/trytond_account_product.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:18:19.000000 trytond_account_product-7.0.1/trytond_account_product.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       68 2024-05-01 12:18:19.000000 trytond_account_product-7.0.1/trytond_account_product.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:07:36.000000 trytond_account_product-7.0.1/trytond_account_product.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      139 2024-05-01 12:18:19.000000 trytond_account_product-7.0.1/trytond_account_product.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 12:18:19.000000 trytond_account_product-7.0.1/trytond_account_product.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:18:19.870988 trytond_account_product-7.0.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      425 2023-10-30 17:06:38.000000 trytond_account_product-7.0.1/view/analytic_account_rule_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      381 2023-10-30 17:06:38.000000 trytond_account_product-7.0.1/view/analytic_account_rule_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1262 2023-10-30 17:06:38.000000 trytond_account_product-7.0.1/view/category_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      579 2023-10-30 17:06:38.000000 trytond_account_product-7.0.1/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      533 2024-02-05 16:24:27.000000 trytond_account_product-7.0.1/view/create_chart_properties_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      451 2023-10-30 17:06:38.000000 trytond_account_product-7.0.1/view/template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      326 2023-10-30 17:06:38.000000 trytond_account_product-7.0.1/view/template_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:22.904029 trytond_account_product-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4118 2024-04-29 15:15:34.000000 trytond_account_product-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      763 2024-04-29 15:15:34.000000 trytond_account_product-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_product-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_product-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2869 2024-04-29 15:35:22.904029 trytond_account_product-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      345 2023-04-15 07:12:15.000000 trytond_account_product-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      968 2023-04-15 07:12:15.000000 trytond_account_product-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3210 2023-04-15 07:12:15.000000 trytond_account_product-7.2.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1000 2023-04-15 07:12:15.000000 trytond_account_product-7.2.0/account.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1082 2023-04-15 07:12:15.000000 trytond_account_product-7.2.0/analytic_account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      827 2023-04-15 07:12:15.000000 trytond_account_product-7.2.0/analytic_account.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1817 2023-04-15 07:12:15.000000 trytond_account_product-7.2.0/configuration.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      490 2023-01-16 14:00:20.000000 trytond_account_product-7.2.0/configuration.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:22.900695 trytond_account_product-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3078 2024-04-27 16:30:39.000000 trytond_account_product-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1917 2023-04-15 07:12:15.000000 trytond_account_product-7.2.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      345 2023-04-15 07:12:15.000000 trytond_account_product-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_account_product-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:36:58.000000 trytond_account_product-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     1052 2023-04-15 07:12:15.000000 trytond_account_product-7.2.0/doc/usage.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      333 2023-04-15 07:12:15.000000 trytond_account_product-7.2.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:22.900695 trytond_account_product-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     6060 2024-04-29 13:17:17.000000 trytond_account_product-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6171 2024-04-29 13:17:17.000000 trytond_account_product-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4929 2024-04-29 13:17:17.000000 trytond_account_product-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6161 2024-04-29 13:17:17.000000 trytond_account_product-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6203 2024-04-29 13:17:17.000000 trytond_account_product-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5274 2024-04-29 13:17:17.000000 trytond_account_product-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5926 2024-04-29 13:17:17.000000 trytond_account_product-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6757 2024-04-29 13:17:17.000000 trytond_account_product-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4929 2024-04-29 13:17:17.000000 trytond_account_product-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6239 2024-04-29 13:17:17.000000 trytond_account_product-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5850 2024-04-29 13:17:17.000000 trytond_account_product-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5148 2024-04-29 13:17:17.000000 trytond_account_product-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6156 2024-04-29 13:17:17.000000 trytond_account_product-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6273 2024-04-29 13:17:17.000000 trytond_account_product-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5033 2024-04-29 13:17:17.000000 trytond_account_product-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6483 2024-04-29 13:17:17.000000 trytond_account_product-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5047 2024-04-29 13:17:17.000000 trytond_account_product-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5947 2024-04-29 13:17:17.000000 trytond_account_product-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6028 2024-04-29 13:17:17.000000 trytond_account_product-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6255 2024-04-29 13:17:17.000000 trytond_account_product-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6054 2024-04-29 13:17:17.000000 trytond_account_product-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4929 2024-04-29 13:17:17.000000 trytond_account_product-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4929 2024-04-29 13:17:17.000000 trytond_account_product-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5729 2024-04-29 13:17:17.000000 trytond_account_product-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      567 2023-04-15 07:12:15.000000 trytond_account_product-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    15921 2024-04-29 13:17:17.000000 trytond_account_product-7.2.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3142 2024-04-27 16:30:39.000000 trytond_account_product-7.2.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:35:22.904029 trytond_account_product-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4573 2024-04-27 16:30:39.000000 trytond_account_product-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:22.900695 trytond_account_product-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_product-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4093 2023-04-15 07:12:15.000000 trytond_account_product-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:36:58.000000 trytond_account_product-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      211 2024-04-29 15:15:30.000000 trytond_account_product-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:22.904029 trytond_account_product-7.2.0/trytond_account_product.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2869 2024-04-29 15:35:22.000000 trytond_account_product-7.2.0/trytond_account_product.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2056 2024-04-29 15:35:22.000000 trytond_account_product-7.2.0/trytond_account_product.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:35:22.000000 trytond_account_product-7.2.0/trytond_account_product.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       68 2024-04-29 15:35:22.000000 trytond_account_product-7.2.0/trytond_account_product.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:06.000000 trytond_account_product-7.2.0/trytond_account_product.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      139 2024-04-29 15:35:22.000000 trytond_account_product-7.2.0/trytond_account_product.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:35:22.000000 trytond_account_product-7.2.0/trytond_account_product.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:22.904029 trytond_account_product-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      425 2023-04-15 07:12:15.000000 trytond_account_product-7.2.0/view/analytic_account_rule_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      381 2023-04-15 07:12:15.000000 trytond_account_product-7.2.0/view/analytic_account_rule_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1262 2023-04-15 07:12:15.000000 trytond_account_product-7.2.0/view/category_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      579 2023-04-15 07:12:15.000000 trytond_account_product-7.2.0/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      531 2024-04-22 12:14:36.000000 trytond_account_product-7.2.0/view/create_chart_properties_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      451 2023-01-16 14:00:20.000000 trytond_account_product-7.2.0/view/template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      326 2023-04-15 07:12:15.000000 trytond_account_product-7.2.0/view/template_tree.xml
```

### Comparing `trytond_account_product-7.0.1/CHANGELOG` & `trytond_account_product-7.2.0/CHANGELOG`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-Version 7.0.1 - 2024-05-01
+Version 7.2.0 - 2024-04-29
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 
 Version 7.0.0 - 2023-10-30
 --------------------------
 * Bug fixes (see mercurial logs for details)
```

### Comparing `trytond_account_product-7.0.1/COPYRIGHT` & `trytond_account_product-7.2.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_account_product-7.0.1/LICENSE` & `trytond_account_product-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_product-7.0.1/PKG-INFO` & `trytond_account_product-7.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_account_product
-Version: 7.0.1
+Version: 7.2.0
 Summary: Tryton module to add accounting on product
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/modules-account-product/
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
@@ -48,20 +48,20 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: trytond_analytic_account<7.1,>=7.0; extra == "test"
+Requires-Dist: trytond_analytic_account<7.3,>=7.2; extra == "test"
 
 ######################
 Account Product Module
 ######################
 
 The *Account Product Module* allows products to be associated with accounting
 properties such as taxes and expense or revenue accounts.
```

### Comparing `trytond_account_product-7.0.1/__init__.py` & `trytond_account_product-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_product-7.0.1/account.py` & `trytond_account_product-7.2.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_product-7.0.1/account.xml` & `trytond_account_product-7.2.0/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_product-7.0.1/analytic_account.py` & `trytond_account_product-7.2.0/analytic_account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_product-7.0.1/analytic_account.xml` & `trytond_account_product-7.2.0/analytic_account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_product-7.0.1/configuration.py` & `trytond_account_product-7.2.0/configuration.py`

 * *Files identical despite different names*

### Comparing `trytond_account_product-7.0.1/doc/conf.py` & `trytond_account_product-7.2.0/doc/conf.py`

 * *Files 8% similar despite different names*

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

### Comparing `trytond_account_product-7.0.1/doc/design.rst` & `trytond_account_product-7.2.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_product-7.0.1/doc/usage.rst` & `trytond_account_product-7.2.0/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_product-7.0.1/locale/bg.po` & `trytond_account_product-7.2.0/locale/bg.po`

 * *Files 1% similar despite different names*

```diff
@@ -197,16 +197,16 @@
 #, fuzzy
 msgctxt "view:account.configuration:"
 msgid "Product"
 msgstr "Продукт"
 
 #, fuzzy
 msgctxt "view:account.create_chart.properties:"
-msgid "Category"
-msgstr "Категория"
+msgid "Product"
+msgstr "Продукт"
 
 msgctxt "view:product.category:"
 msgid "Accounting"
 msgstr "Счетоводство"
 
 msgctxt "view:product.category:"
 msgid "Accounts"
```

### Comparing `trytond_account_product-7.0.1/locale/ca.po` & `trytond_account_product-7.2.0/locale/ca.po`

 * *Files 2% similar despite different names*

```diff
@@ -185,16 +185,16 @@
 msgstr "Administració comptable de productes"
 
 msgctxt "view:account.configuration:"
 msgid "Product"
 msgstr "Producte"
 
 msgctxt "view:account.create_chart.properties:"
-msgid "Category"
-msgstr "Categoria"
+msgid "Product"
+msgstr "Producte"
 
 msgctxt "view:product.category:"
 msgid "Accounting"
 msgstr "Comptabilitat"
 
 msgctxt "view:product.category:"
 msgid "Accounts"
```

### Comparing `trytond_account_product-7.0.1/locale/cs.po` & `trytond_account_product-7.2.0/locale/cs.po`

 * *Files 0% similar despite different names*

```diff
@@ -185,15 +185,15 @@
 msgstr ""
 
 msgctxt "view:account.configuration:"
 msgid "Product"
 msgstr ""
 
 msgctxt "view:account.create_chart.properties:"
-msgid "Category"
+msgid "Product"
 msgstr ""
 
 msgctxt "view:product.category:"
 msgid "Accounting"
 msgstr ""
 
 msgctxt "view:product.category:"
```

### Comparing `trytond_account_product-7.0.1/locale/de.po` & `trytond_account_product-7.2.0/locale/de.po`

 * *Files 1% similar despite different names*

```diff
@@ -188,16 +188,16 @@
 msgstr "Buchhaltung Artikel Einstellungen"
 
 msgctxt "view:account.configuration:"
 msgid "Product"
 msgstr "Artikel"
 
 msgctxt "view:account.create_chart.properties:"
-msgid "Category"
-msgstr "Kategorie"
+msgid "Product"
+msgstr "Artikel"
 
 msgctxt "view:product.category:"
 msgid "Accounting"
 msgstr "Buchhaltung"
 
 msgctxt "view:product.category:"
 msgid "Accounts"
```

### Comparing `trytond_account_product-7.0.1/locale/es.po` & `trytond_account_product-7.2.0/locale/es.po`

 * *Files 1% similar despite different names*

```diff
@@ -187,16 +187,16 @@
 msgstr "Administración contable de productos"
 
 msgctxt "view:account.configuration:"
 msgid "Product"
 msgstr "Producto"
 
 msgctxt "view:account.create_chart.properties:"
-msgid "Category"
-msgstr "Categoría"
+msgid "Product"
+msgstr "Producto"
 
 msgctxt "view:product.category:"
 msgid "Accounting"
 msgstr "Contabilidad"
 
 msgctxt "view:product.category:"
 msgid "Accounts"
```

### Comparing `trytond_account_product-7.0.1/locale/es_419.po` & `trytond_account_product-7.2.0/locale/es_419.po`

 * *Files 1% similar despite different names*

```diff
@@ -186,15 +186,15 @@
 msgstr ""
 
 msgctxt "view:account.configuration:"
 msgid "Product"
 msgstr ""
 
 msgctxt "view:account.create_chart.properties:"
-msgid "Category"
+msgid "Product"
 msgstr ""
 
 msgctxt "view:product.category:"
 msgid "Accounting"
 msgstr ""
 
 msgctxt "view:product.category:"
```

### Comparing `trytond_account_product-7.0.1/locale/et.po` & `trytond_account_product-7.2.0/locale/et.po`

 * *Files 2% similar despite different names*

```diff
@@ -186,17 +186,18 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "view:account.configuration:"
 msgid "Product"
 msgstr "Toode"
 
+#, fuzzy
 msgctxt "view:account.create_chart.properties:"
-msgid "Category"
-msgstr "Kategooria"
+msgid "Product"
+msgstr "Toode"
 
 msgctxt "view:product.category:"
 msgid "Accounting"
 msgstr "Raamatupidamine"
 
 msgctxt "view:product.category:"
 msgid "Accounts"
```

### Comparing `trytond_account_product-7.0.1/locale/fa.po` & `trytond_account_product-7.2.0/locale/fa.po`

 * *Files 0% similar despite different names*

```diff
@@ -190,16 +190,16 @@
 
 #, fuzzy
 msgctxt "view:account.configuration:"
 msgid "Product"
 msgstr "محصول"
 
 msgctxt "view:account.create_chart.properties:"
-msgid "Category"
-msgstr "دسته‌بندی‌"
+msgid "Product"
+msgstr "محصول"
 
 msgctxt "view:product.category:"
 msgid "Accounting"
 msgstr "حسابداری"
 
 msgctxt "view:product.category:"
 msgid "Accounts"
```

### Comparing `trytond_account_product-7.0.1/locale/fi.po` & `trytond_account_product-7.2.0/locale/fi.po`

 * *Files 0% similar despite different names*

```diff
@@ -185,15 +185,15 @@
 msgstr ""
 
 msgctxt "view:account.configuration:"
 msgid "Product"
 msgstr ""
 
 msgctxt "view:account.create_chart.properties:"
-msgid "Category"
+msgid "Product"
 msgstr ""
 
 msgctxt "view:product.category:"
 msgid "Accounting"
 msgstr ""
 
 msgctxt "view:product.category:"
```

### Comparing `trytond_account_product-7.0.1/locale/fr.po` & `trytond_account_product-7.2.0/locale/fr.po`

 * *Files 0% similar despite different names*

```diff
@@ -189,16 +189,16 @@
 msgstr "Administration comptable des produits"
 
 msgctxt "view:account.configuration:"
 msgid "Product"
 msgstr "Produit"
 
 msgctxt "view:account.create_chart.properties:"
-msgid "Category"
-msgstr "Catégorie"
+msgid "Product"
+msgstr "Produit"
 
 msgctxt "view:product.category:"
 msgid "Accounting"
 msgstr "Comptabilité"
 
 msgctxt "view:product.category:"
 msgid "Accounts"
```

### Comparing `trytond_account_product-7.0.1/locale/hu.po` & `trytond_account_product-7.2.0/locale/hu.po`

 * *Files 2% similar despite different names*

```diff
@@ -184,17 +184,18 @@
 msgid "Account Product Administration"
 msgstr ""
 
 msgctxt "view:account.configuration:"
 msgid "Product"
 msgstr "Termék"
 
+#, fuzzy
 msgctxt "view:account.create_chart.properties:"
-msgid "Category"
-msgstr "Kategória"
+msgid "Product"
+msgstr "Termék"
 
 msgctxt "view:product.category:"
 msgid "Accounting"
 msgstr "Pénzügy"
 
 msgctxt "view:product.category:"
 msgid "Accounts"
```

### Comparing `trytond_account_product-7.0.1/locale/id.po` & `trytond_account_product-7.2.0/locale/id.po`

 * *Files 2% similar despite different names*

```diff
@@ -184,17 +184,18 @@
 msgid "Account Product Administration"
 msgstr ""
 
 msgctxt "view:account.configuration:"
 msgid "Product"
 msgstr "Produk"
 
+#, fuzzy
 msgctxt "view:account.create_chart.properties:"
-msgid "Category"
-msgstr "Kategori"
+msgid "Product"
+msgstr "Produk"
 
 msgctxt "view:product.category:"
 msgid "Accounting"
 msgstr "Akuntansi"
 
 msgctxt "view:product.category:"
 msgid "Accounts"
```

### Comparing `trytond_account_product-7.0.1/locale/it.po` & `trytond_account_product-7.2.0/locale/it.po`

 * *Files 1% similar despite different names*

```diff
@@ -189,16 +189,16 @@
 msgstr "Amministrazione Conto Prodotto"
 
 msgctxt "view:account.configuration:"
 msgid "Product"
 msgstr "Prodotto"
 
 msgctxt "view:account.create_chart.properties:"
-msgid "Category"
-msgstr "Categoria"
+msgid "Product"
+msgstr "Prodotto"
 
 msgctxt "view:product.category:"
 msgid "Accounting"
 msgstr "Contabilità"
 
 msgctxt "view:product.category:"
 msgid "Accounts"
```

### Comparing `trytond_account_product-7.0.1/locale/lo.po` & `trytond_account_product-7.2.0/locale/lo.po`

 * *Files 0% similar despite different names*

```diff
@@ -198,16 +198,16 @@
 #, fuzzy
 msgctxt "view:account.configuration:"
 msgid "Product"
 msgstr "ຜະລິດຕະພັນ"
 
 #, fuzzy
 msgctxt "view:account.create_chart.properties:"
-msgid "Category"
-msgstr "ໝວດ"
+msgid "Product"
+msgstr "ຜະລິດຕະພັນ"
 
 msgctxt "view:product.category:"
 msgid "Accounting"
 msgstr "ການບັນຊີ"
 
 msgctxt "view:product.category:"
 msgid "Accounts"
```

### Comparing `trytond_account_product-7.0.1/locale/lt.po` & `trytond_account_product-7.2.0/locale/lt.po`

 * *Files 0% similar despite different names*

```diff
@@ -185,15 +185,15 @@
 msgstr ""
 
 msgctxt "view:account.configuration:"
 msgid "Product"
 msgstr ""
 
 msgctxt "view:account.create_chart.properties:"
-msgid "Category"
+msgid "Product"
 msgstr ""
 
 msgctxt "view:product.category:"
 msgid "Accounting"
 msgstr ""
 
 msgctxt "view:product.category:"
```

### Comparing `trytond_account_product-7.0.1/locale/nl.po` & `trytond_account_product-7.2.0/locale/nl.po`

 * *Files 1% similar despite different names*

```diff
@@ -194,16 +194,16 @@
 msgstr "Product financiële administratie"
 
 msgctxt "view:account.configuration:"
 msgid "Product"
 msgstr "Product"
 
 msgctxt "view:account.create_chart.properties:"
-msgid "Category"
-msgstr "Categorie"
+msgid "Product"
+msgstr "Product"
 
 msgctxt "view:product.category:"
 msgid "Accounting"
 msgstr "Boekhouden"
 
 msgctxt "view:product.category:"
 msgid "Accounts"
```

### Comparing `trytond_account_product-7.0.1/locale/pl.po` & `trytond_account_product-7.2.0/locale/pl.po`

 * *Files 1% similar despite different names*

```diff
@@ -187,16 +187,16 @@
 
 #, fuzzy
 msgctxt "view:account.configuration:"
 msgid "Product"
 msgstr "Produkt"
 
 msgctxt "view:account.create_chart.properties:"
-msgid "Category"
-msgstr "Kategoria"
+msgid "Product"
+msgstr "Produkt"
 
 msgctxt "view:product.category:"
 msgid "Accounting"
 msgstr ""
 
 msgctxt "view:product.category:"
 msgid "Accounts"
```

### Comparing `trytond_account_product-7.0.1/locale/pt.po` & `trytond_account_product-7.2.0/locale/pt.po`

 * *Files 1% similar despite different names*

```diff
@@ -189,16 +189,16 @@
 
 #, fuzzy
 msgctxt "view:account.configuration:"
 msgid "Product"
 msgstr "Produto"
 
 msgctxt "view:account.create_chart.properties:"
-msgid "Category"
-msgstr "Categoria"
+msgid "Product"
+msgstr "Produto"
 
 msgctxt "view:product.category:"
 msgid "Accounting"
 msgstr "Contabilidade"
 
 msgctxt "view:product.category:"
 msgid "Accounts"
```

### Comparing `trytond_account_product-7.0.1/locale/ro.po` & `trytond_account_product-7.2.0/locale/ro.po`

 * *Files 1% similar despite different names*

```diff
@@ -184,17 +184,18 @@
 msgid "Account Product Administration"
 msgstr "Cont Administrare Produs"
 
 msgctxt "view:account.configuration:"
 msgid "Product"
 msgstr "Produs"
 
+#, fuzzy
 msgctxt "view:account.create_chart.properties:"
-msgid "Category"
-msgstr "Categorie"
+msgid "Product"
+msgstr "Produs"
 
 msgctxt "view:product.category:"
 msgid "Accounting"
 msgstr "Contabilitate"
 
 msgctxt "view:product.category:"
 msgid "Accounts"
```

### Comparing `trytond_account_product-7.0.1/locale/ru.po` & `trytond_account_product-7.2.0/locale/ru.po`

 * *Files 2% similar despite different names*

```diff
@@ -197,16 +197,16 @@
 #, fuzzy
 msgctxt "view:account.configuration:"
 msgid "Product"
 msgstr "Товарно материальные ценности (ТМЦ)"
 
 #, fuzzy
 msgctxt "view:account.create_chart.properties:"
-msgid "Category"
-msgstr "Категория"
+msgid "Product"
+msgstr "Товарно материальные ценности (ТМЦ)"
 
 msgctxt "view:product.category:"
 msgid "Accounting"
 msgstr "Регистрационные данные"
 
 msgctxt "view:product.category:"
 msgid "Accounts"
```

### Comparing `trytond_account_product-7.0.1/locale/sl.po` & `trytond_account_product-7.2.0/locale/sl.po`

 * *Files 1% similar despite different names*

```diff
@@ -184,17 +184,18 @@
 msgid "Account Product Administration"
 msgstr "Administracija računovodskih postavk"
 
 msgctxt "view:account.configuration:"
 msgid "Product"
 msgstr "Izdelek"
 
+#, fuzzy
 msgctxt "view:account.create_chart.properties:"
-msgid "Category"
-msgstr "Kategorija"
+msgid "Product"
+msgstr "Izdelek"
 
 msgctxt "view:product.category:"
 msgid "Accounting"
 msgstr "Računovodstvo"
 
 msgctxt "view:product.category:"
 msgid "Accounts"
```

### Comparing `trytond_account_product-7.0.1/locale/tr.po` & `trytond_account_product-7.2.0/locale/tr.po`

 * *Files 0% similar despite different names*

```diff
@@ -185,15 +185,15 @@
 msgstr ""
 
 msgctxt "view:account.configuration:"
 msgid "Product"
 msgstr ""
 
 msgctxt "view:account.create_chart.properties:"
-msgid "Category"
+msgid "Product"
 msgstr ""
 
 msgctxt "view:product.category:"
 msgid "Accounting"
 msgstr ""
 
 msgctxt "view:product.category:"
```

### Comparing `trytond_account_product-7.0.1/locale/uk.po` & `trytond_account_product-7.2.0/locale/uk.po`

 * *Files 0% similar despite different names*

```diff
@@ -185,15 +185,15 @@
 msgstr ""
 
 msgctxt "view:account.configuration:"
 msgid "Product"
 msgstr ""
 
 msgctxt "view:account.create_chart.properties:"
-msgid "Category"
+msgid "Product"
 msgstr ""
 
 msgctxt "view:product.category:"
 msgid "Accounting"
 msgstr ""
 
 msgctxt "view:product.category:"
```

### Comparing `trytond_account_product-7.0.1/locale/zh_CN.po` & `trytond_account_product-7.2.0/locale/zh_CN.po`

 * *Files 4% similar despite different names*

```diff
@@ -184,17 +184,18 @@
 msgid "Account Product Administration"
 msgstr "帐户产品管理"
 
 msgctxt "view:account.configuration:"
 msgid "Product"
 msgstr "产品"
 
+#, fuzzy
 msgctxt "view:account.create_chart.properties:"
-msgid "Category"
-msgstr "类别"
+msgid "Product"
+msgstr "产品"
 
 msgctxt "view:product.category:"
 msgid "Accounting"
 msgstr "会计"
 
 msgctxt "view:product.category:"
 msgid "Accounts"
```

### Comparing `trytond_account_product-7.0.1/message.xml` & `trytond_account_product-7.2.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_product-7.0.1/product.py` & `trytond_account_product-7.2.0/product.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 from functools import wraps
 
 from sql import Null
 
+from trytond import backend
 from trytond.i18n import gettext
 from trytond.model import ModelSQL, fields
 from trytond.modules.company.model import (
     CompanyMultiValueMixin, CompanyValueMixin)
 from trytond.pool import Pool, PoolMeta
 from trytond.pyson import Bool, Eval, Or
 from trytond.transaction import Transaction
@@ -275,40 +276,52 @@
             ('company', '=', Eval('company', -1)),
             ])
 
 
 class CategoryCustomerTax(ModelSQL):
     'Category - Customer Tax'
     __name__ = 'product.category-customer-account.tax'
-    _table = 'product_category_customer_taxes_rel'
     category = fields.Many2One(
         'product.category', "Category", ondelete='CASCADE', required=True)
     tax = fields.Many2One('account.tax', 'Tax', ondelete='RESTRICT',
             required=True)
 
     @classmethod
     def __setup__(cls):
         super().__setup__()
         cls.__access__.add('tax')
 
+    @classmethod
+    def __register__(cls, module):
+        # Migration from 7.0: rename to standard name
+        backend.TableHandler.table_rename(
+            'product_category_customer_taxes_rel', cls._table)
+        super().__register__(module)
+
 
 class CategorySupplierTax(ModelSQL):
     'Category - Supplier Tax'
     __name__ = 'product.category-supplier-account.tax'
-    _table = 'product_category_supplier_taxes_rel'
     category = fields.Many2One(
         'product.category', "Category", ondelete='CASCADE', required=True)
     tax = fields.Many2One('account.tax', 'Tax', ondelete='RESTRICT',
             required=True)
 
     @classmethod
     def __setup__(cls):
         super().__setup__()
         cls.__access__.add('tax')
 
+    @classmethod
+    def __register__(cls, module):
+        # Migration from 7.0: rename to standard name
+        backend.TableHandler.table_rename(
+            'product_category_supplier_taxes_rel', cls._table)
+        super().__register__(module)
+
 
 class Template(CompanyMultiValueMixin, metaclass=PoolMeta):
     __name__ = 'product.template'
     account_category = fields.Many2One('product.category', 'Account Category',
         domain=[
             ('accounting', '=', True),
             ])
```

### Comparing `trytond_account_product-7.0.1/product.xml` & `trytond_account_product-7.2.0/product.xml`

 * *Files 16% similar despite different names*

#### Comparing `trytond_account_product-7.0.1/product.xml` & `trytond_account_product-7.2.0/product.xml`

```diff
@@ -6,26 +6,26 @@
     <record model="ir.ui.view" id="category_view_form">
       <field name="model">product.category</field>
       <field name="inherit" ref="product.category_view_form"/>
       <field name="name">category_form</field>
     </record>
     <record model="ir.rule.group" id="rule_group_category_default">
       <field name="name">Not accounting category</field>
-      <field name="model" search="[('model', '=', 'product.category')]"/>
+      <field name="model">product.category</field>
       <field name="default_p" eval="True"/>
       <field name="global_p" eval="False"/>
       <field name="perm_read" eval="False"/>
     </record>
     <record model="ir.rule" id="rule_category_default_non_accounting">
       <field name="domain" eval="[('accounting', '=', False)]" pyson="1"/>
       <field name="rule_group" ref="rule_group_category_default"/>
     </record>
     <record model="ir.rule.group" id="rule_group_category_accounting">
       <field name="name">Any category</field>
-      <field name="model" search="[('model', '=', 'product.category')]"/>
+      <field name="model">product.category</field>
       <field name="global_p" eval="False"/>
       <field name="perm_read" eval="False"/>
     </record>
     <record model="ir.rule.group-res.group" id="rule_group_category_account-account_product_admin">
       <field name="rule_group" ref="rule_group_category_accounting"/>
       <field name="group" ref="group_account_product_admin"/>
     </record>
@@ -40,19 +40,21 @@
     </record>
     <record model="ir.ui.view" id="template_view_tree">
       <field name="model">product.template</field>
       <field name="inherit" ref="product.template_view_tree"/>
       <field name="name">template_tree</field>
     </record>
     <record model="ir.model.field.access" id="access_template_account_category">
-      <field name="field" search="[('model.model', '=', 'product.template'), ('name', '=', 'account_category')]"/>
+      <field name="model">product.template</field>
+      <field name="field">account_category</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
     </record>
     <record model="ir.model.field.access" id="access_template_account_category_account_product_admin">
-      <field name="field" search="[('model.model', '=', 'product.template'), ('name', '=', 'account_category')]"/>
+      <field name="model">product.template</field>
+      <field name="field">account_category</field>
       <field name="group" ref="group_account_product_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
     </record>
   </data>
 </tryton>
```

### Comparing `trytond_account_product-7.0.1/setup.py` & `trytond_account_product-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_account_product-7.0.1/tests/test_module.py` & `trytond_account_product-7.2.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_account_product-7.0.1/tox.ini` & `trytond_account_product-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_product-7.0.1/trytond_account_product.egg-info/PKG-INFO` & `trytond_account_product-7.2.0/trytond_account_product.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_account_product
-Version: 7.0.1
+Version: 7.2.0
 Summary: Tryton module to add accounting on product
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/modules-account-product/
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
@@ -48,20 +48,20 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: trytond_analytic_account<7.1,>=7.0; extra == "test"
+Requires-Dist: trytond_analytic_account<7.3,>=7.2; extra == "test"
 
 ######################
 Account Product Module
 ######################
 
 The *Account Product Module* allows products to be associated with accounting
 properties such as taxes and expense or revenue accounts.
```

### Comparing `trytond_account_product-7.0.1/trytond_account_product.egg-info/SOURCES.txt` & `trytond_account_product-7.2.0/trytond_account_product.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_product-7.0.1/view/category_form.xml` & `trytond_account_product-7.2.0/view/category_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_product-7.0.1/view/configuration_form.xml` & `trytond_account_product-7.2.0/view/configuration_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_product-7.0.1/view/create_chart_properties_form.xml` & `trytond_account_product-7.2.0/view/create_chart_properties_form.xml`

 * *Files 22% similar despite different names*

#### Comparing `trytond_account_product-7.0.1/view/create_chart_properties_form.xml` & `trytond_account_product-7.2.0/view/create_chart_properties_form.xml`

```diff
@@ -1,12 +1,12 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!-- This file is part of Tryton.  The COPYRIGHT file at the top level of
 this repository contains the full copyright notices and license terms. -->
 <data>
   <xpath expr="/form/field[@name='account_payable']" position="after">
-    <separator id="category" string="Category" colspan="4"/>
+    <separator id="product" string="Product" colspan="4"/>
     <label name="category_account_revenue"/>
     <field name="category_account_revenue"/>
     <label name="category_account_expense"/>
     <field name="category_account_expense"/>
   </xpath>
 </data>
```

