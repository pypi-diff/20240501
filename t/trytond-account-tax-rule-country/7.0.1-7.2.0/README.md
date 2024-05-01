# Comparing `tmp/trytond_account_tax_rule_country-7.0.1.tar.gz` & `tmp/trytond_account_tax_rule_country-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_tax_rule_country-7.0.1.tar", last modified: Wed May  1 12:08:41 2024, max compression
+gzip compressed data, was "trytond_account_tax_rule_country-7.2.0.tar", last modified: Mon Apr 29 15:37:32 2024, max compression
```

## Comparing `trytond_account_tax_rule_country-7.0.1.tar` & `trytond_account_tax_rule_country-7.2.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:08:41.738957 trytond_account_tax_rule_country-7.0.1/
--rw-r--r--   0 ced       (1000) ced       (1000)     1774 2024-05-01 12:08:38.000000 trytond_account_tax_rule_country-7.0.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-05-01 12:08:38.000000 trytond_account_tax_rule_country-7.0.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_account_tax_rule_country-7.0.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_account_tax_rule_country-7.0.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3817 2024-05-01 12:08:41.738957 trytond_account_tax_rule_country-7.0.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1109 2023-10-30 17:06:38.000000 trytond_account_tax_rule_country-7.0.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      972 2023-10-30 17:06:38.000000 trytond_account_tax_rule_country-7.0.1/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5705 2024-04-27 05:19:50.000000 trytond_account_tax_rule_country-7.0.1/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1750 2023-10-30 17:06:38.000000 trytond_account_tax_rule_country-7.0.1/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:08:41.735624 trytond_account_tax_rule_country-7.0.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2803 2024-03-03 16:24:20.000000 trytond_account_tax_rule_country-7.0.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1109 2023-10-30 17:06:38.000000 trytond_account_tax_rule_country-7.0.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_account_tax_rule_country-7.0.1/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:08:41.735624 trytond_account_tax_rule_country-7.0.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1734 2023-10-30 17:06:38.000000 trytond_account_tax_rule_country-7.0.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2222 2023-10-30 17:06:38.000000 trytond_account_tax_rule_country-7.0.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1734 2023-10-30 17:06:38.000000 trytond_account_tax_rule_country-7.0.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2193 2023-10-30 17:06:38.000000 trytond_account_tax_rule_country-7.0.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2264 2023-10-30 17:06:38.000000 trytond_account_tax_rule_country-7.0.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1734 2023-10-30 17:06:38.000000 trytond_account_tax_rule_country-7.0.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1758 2023-10-30 17:06:38.000000 trytond_account_tax_rule_country-7.0.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1786 2023-10-30 17:06:38.000000 trytond_account_tax_rule_country-7.0.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1734 2023-10-30 17:06:38.000000 trytond_account_tax_rule_country-7.0.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2260 2023-10-30 17:06:38.000000 trytond_account_tax_rule_country-7.0.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1734 2023-10-30 17:06:38.000000 trytond_account_tax_rule_country-7.0.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1774 2023-10-30 17:06:38.000000 trytond_account_tax_rule_country-7.0.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2218 2023-10-30 17:06:38.000000 trytond_account_tax_rule_country-7.0.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1836 2023-10-30 17:06:38.000000 trytond_account_tax_rule_country-7.0.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1734 2023-10-30 17:06:38.000000 trytond_account_tax_rule_country-7.0.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2208 2023-10-30 17:06:38.000000 trytond_account_tax_rule_country-7.0.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1764 2023-10-30 17:06:38.000000 trytond_account_tax_rule_country-7.0.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1796 2023-10-30 17:06:38.000000 trytond_account_tax_rule_country-7.0.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2212 2023-10-30 17:06:38.000000 trytond_account_tax_rule_country-7.0.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1734 2023-10-30 17:06:38.000000 trytond_account_tax_rule_country-7.0.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1772 2023-10-30 17:06:38.000000 trytond_account_tax_rule_country-7.0.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1734 2023-10-30 17:06:38.000000 trytond_account_tax_rule_country-7.0.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1734 2023-10-30 17:06:38.000000 trytond_account_tax_rule_country-7.0.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1734 2023-10-30 17:06:38.000000 trytond_account_tax_rule_country-7.0.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1657 2023-10-30 17:06:38.000000 trytond_account_tax_rule_country-7.0.1/purchase.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1598 2023-10-30 17:06:38.000000 trytond_account_tax_rule_country-7.0.1/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 12:08:41.738957 trytond_account_tax_rule_country-7.0.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4593 2023-10-30 17:06:38.000000 trytond_account_tax_rule_country-7.0.1/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1907 2023-10-30 17:06:38.000000 trytond_account_tax_rule_country-7.0.1/stock.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:08:41.738957 trytond_account_tax_rule_country-7.0.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_account_tax_rule_country-7.0.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6344 2023-10-30 17:06:38.000000 trytond_account_tax_rule_country-7.0.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_account_tax_rule_country-7.0.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      156 2024-02-05 16:24:27.000000 trytond_account_tax_rule_country-7.0.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:08:41.738957 trytond_account_tax_rule_country-7.0.1/trytond_account_tax_rule_country.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3817 2024-05-01 12:08:41.000000 trytond_account_tax_rule_country-7.0.1/trytond_account_tax_rule_country.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1787 2024-05-01 12:08:41.000000 trytond_account_tax_rule_country-7.0.1/trytond_account_tax_rule_country.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:08:41.000000 trytond_account_tax_rule_country-7.0.1/trytond_account_tax_rule_country.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       86 2024-05-01 12:08:41.000000 trytond_account_tax_rule_country-7.0.1/trytond_account_tax_rule_country.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:07:42.000000 trytond_account_tax_rule_country-7.0.1/trytond_account_tax_rule_country.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      186 2024-05-01 12:08:41.000000 trytond_account_tax_rule_country-7.0.1/trytond_account_tax_rule_country.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 12:08:41.000000 trytond_account_tax_rule_country-7.0.1/trytond_account_tax_rule_country.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:08:41.738957 trytond_account_tax_rule_country-7.0.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      571 2023-10-30 17:06:38.000000 trytond_account_tax_rule_country-7.0.1/view/tax_rule_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      571 2023-10-30 17:06:38.000000 trytond_account_tax_rule_country-7.0.1/view/tax_rule_line_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      463 2023-10-30 17:06:38.000000 trytond_account_tax_rule_country-7.0.1/view/tax_rule_line_template_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      463 2023-10-30 17:06:38.000000 trytond_account_tax_rule_country-7.0.1/view/tax_rule_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      463 2023-10-30 17:06:38.000000 trytond_account_tax_rule_country-7.0.1/view/tax_rule_line_tree_sequence.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:37:32.117316 trytond_account_tax_rule_country-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1774 2024-04-29 15:17:29.000000 trytond_account_tax_rule_country-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-04-29 15:17:29.000000 trytond_account_tax_rule_country-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_tax_rule_country-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_tax_rule_country-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3817 2024-04-29 15:37:32.117316 trytond_account_tax_rule_country-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1109 2023-04-15 07:12:15.000000 trytond_account_tax_rule_country-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      972 2023-04-15 07:12:15.000000 trytond_account_tax_rule_country-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5705 2024-04-29 13:17:17.000000 trytond_account_tax_rule_country-7.2.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1750 2023-01-16 14:00:20.000000 trytond_account_tax_rule_country-7.2.0/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:37:32.113983 trytond_account_tax_rule_country-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3087 2024-04-27 16:30:39.000000 trytond_account_tax_rule_country-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1109 2023-04-15 07:12:15.000000 trytond_account_tax_rule_country-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:03.000000 trytond_account_tax_rule_country-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:37:32.117316 trytond_account_tax_rule_country-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1734 2024-04-27 16:43:22.000000 trytond_account_tax_rule_country-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2222 2024-04-27 16:43:22.000000 trytond_account_tax_rule_country-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1734 2024-04-27 16:43:22.000000 trytond_account_tax_rule_country-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2193 2024-04-27 16:43:22.000000 trytond_account_tax_rule_country-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2264 2024-04-27 16:43:22.000000 trytond_account_tax_rule_country-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1734 2024-04-27 16:43:22.000000 trytond_account_tax_rule_country-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1758 2024-04-27 16:43:22.000000 trytond_account_tax_rule_country-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1786 2024-04-27 16:43:22.000000 trytond_account_tax_rule_country-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1734 2024-04-27 16:43:22.000000 trytond_account_tax_rule_country-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2260 2024-04-27 16:43:22.000000 trytond_account_tax_rule_country-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1734 2024-04-27 16:43:22.000000 trytond_account_tax_rule_country-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1774 2024-04-27 16:43:22.000000 trytond_account_tax_rule_country-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2218 2024-04-27 16:43:22.000000 trytond_account_tax_rule_country-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1836 2024-04-27 16:43:22.000000 trytond_account_tax_rule_country-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1734 2024-04-27 16:43:22.000000 trytond_account_tax_rule_country-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2208 2024-04-27 16:43:22.000000 trytond_account_tax_rule_country-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1764 2024-04-27 16:43:22.000000 trytond_account_tax_rule_country-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1796 2024-04-27 16:43:22.000000 trytond_account_tax_rule_country-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2212 2024-04-27 16:43:22.000000 trytond_account_tax_rule_country-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1734 2024-04-27 16:43:22.000000 trytond_account_tax_rule_country-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1772 2024-04-27 16:43:22.000000 trytond_account_tax_rule_country-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1734 2024-04-27 16:43:22.000000 trytond_account_tax_rule_country-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1734 2024-04-27 16:43:22.000000 trytond_account_tax_rule_country-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1734 2024-04-27 16:43:22.000000 trytond_account_tax_rule_country-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1657 2024-01-27 09:58:52.000000 trytond_account_tax_rule_country-7.2.0/purchase.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1598 2024-01-27 09:58:52.000000 trytond_account_tax_rule_country-7.2.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:37:32.117316 trytond_account_tax_rule_country-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4593 2024-03-17 11:01:36.000000 trytond_account_tax_rule_country-7.2.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1907 2023-04-15 07:12:15.000000 trytond_account_tax_rule_country-7.2.0/stock.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:37:32.117316 trytond_account_tax_rule_country-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_tax_rule_country-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6344 2023-04-15 07:12:15.000000 trytond_account_tax_rule_country-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:03.000000 trytond_account_tax_rule_country-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      156 2024-04-29 15:17:24.000000 trytond_account_tax_rule_country-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:37:32.117316 trytond_account_tax_rule_country-7.2.0/trytond_account_tax_rule_country.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3817 2024-04-29 15:37:31.000000 trytond_account_tax_rule_country-7.2.0/trytond_account_tax_rule_country.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1787 2024-04-29 15:37:32.000000 trytond_account_tax_rule_country-7.2.0/trytond_account_tax_rule_country.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:37:31.000000 trytond_account_tax_rule_country-7.2.0/trytond_account_tax_rule_country.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       86 2024-04-29 15:37:31.000000 trytond_account_tax_rule_country-7.2.0/trytond_account_tax_rule_country.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:05.000000 trytond_account_tax_rule_country-7.2.0/trytond_account_tax_rule_country.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      186 2024-04-29 15:37:31.000000 trytond_account_tax_rule_country-7.2.0/trytond_account_tax_rule_country.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:37:31.000000 trytond_account_tax_rule_country-7.2.0/trytond_account_tax_rule_country.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:37:32.117316 trytond_account_tax_rule_country-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      571 2023-04-15 07:12:15.000000 trytond_account_tax_rule_country-7.2.0/view/tax_rule_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      571 2023-04-15 07:12:15.000000 trytond_account_tax_rule_country-7.2.0/view/tax_rule_line_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      463 2023-04-15 07:12:15.000000 trytond_account_tax_rule_country-7.2.0/view/tax_rule_line_template_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      463 2023-04-15 07:12:15.000000 trytond_account_tax_rule_country-7.2.0/view/tax_rule_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      463 2023-04-15 07:12:15.000000 trytond_account_tax_rule_country-7.2.0/view/tax_rule_line_tree_sequence.xml
```

### Comparing `trytond_account_tax_rule_country-7.0.1/CHANGELOG` & `trytond_account_tax_rule_country-7.2.0/CHANGELOG`

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

### Comparing `trytond_account_tax_rule_country-7.0.1/COPYRIGHT` & `trytond_account_tax_rule_country-7.2.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-7.0.1/LICENSE` & `trytond_account_tax_rule_country-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-7.0.1/PKG-INFO` & `trytond_account_tax_rule_country-7.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_account_tax_rule_country
-Version: 7.0.1
+Version: 7.2.0
 Summary: Tryton module to add countries on tax rules
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
@@ -48,22 +48,22 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_country<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_country<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: trytond_account_invoice<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_purchase<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_stock<7.1,>=7.0; extra == "test"
+Requires-Dist: trytond_account_invoice<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_purchase<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_stock<7.3,>=7.2; extra == "test"
 
 Account Tax Rule Country
 ########################
 
 The account_tax_rule module extends the tax rule to add origin and destination
 countries and subdivisions as criteria.
```

### Comparing `trytond_account_tax_rule_country-7.0.1/README.rst` & `trytond_account_tax_rule_country-7.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-7.0.1/__init__.py` & `trytond_account_tax_rule_country-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-7.0.1/account.py` & `trytond_account_tax_rule_country-7.2.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-7.0.1/account.xml` & `trytond_account_tax_rule_country-7.2.0/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-7.0.1/doc/conf.py` & `trytond_account_tax_rule_country-7.2.0/doc/conf.py`

 * *Files 6% similar despite different names*

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

### Comparing `trytond_account_tax_rule_country-7.0.1/doc/index.rst` & `trytond_account_tax_rule_country-7.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-7.0.1/locale/bg.po` & `trytond_account_tax_rule_country-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-7.0.1/locale/ca.po` & `trytond_account_tax_rule_country-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-7.0.1/locale/cs.po` & `trytond_account_tax_rule_country-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-7.0.1/locale/de.po` & `trytond_account_tax_rule_country-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-7.0.1/locale/es.po` & `trytond_account_tax_rule_country-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-7.0.1/locale/es_419.po` & `trytond_account_tax_rule_country-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-7.0.1/locale/et.po` & `trytond_account_tax_rule_country-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-7.0.1/locale/fa.po` & `trytond_account_tax_rule_country-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-7.0.1/locale/fi.po` & `trytond_account_tax_rule_country-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-7.0.1/locale/fr.po` & `trytond_account_tax_rule_country-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-7.0.1/locale/hu.po` & `trytond_account_tax_rule_country-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-7.0.1/locale/id.po` & `trytond_account_tax_rule_country-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-7.0.1/locale/it.po` & `trytond_account_tax_rule_country-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-7.0.1/locale/lo.po` & `trytond_account_tax_rule_country-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-7.0.1/locale/lt.po` & `trytond_account_tax_rule_country-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-7.0.1/locale/nl.po` & `trytond_account_tax_rule_country-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-7.0.1/locale/pl.po` & `trytond_account_tax_rule_country-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-7.0.1/locale/pt.po` & `trytond_account_tax_rule_country-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-7.0.1/locale/ro.po` & `trytond_account_tax_rule_country-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-7.0.1/locale/ru.po` & `trytond_account_tax_rule_country-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-7.0.1/locale/sl.po` & `trytond_account_tax_rule_country-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-7.0.1/locale/tr.po` & `trytond_account_tax_rule_country-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-7.0.1/locale/uk.po` & `trytond_account_tax_rule_country-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-7.0.1/locale/zh_CN.po` & `trytond_account_tax_rule_country-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-7.0.1/purchase.py` & `trytond_account_tax_rule_country-7.2.0/purchase.py`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-7.0.1/sale.py` & `trytond_account_tax_rule_country-7.2.0/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-7.0.1/setup.py` & `trytond_account_tax_rule_country-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-7.0.1/stock.py` & `trytond_account_tax_rule_country-7.2.0/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-7.0.1/tests/test_module.py` & `trytond_account_tax_rule_country-7.2.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-7.0.1/tox.ini` & `trytond_account_tax_rule_country-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-7.0.1/trytond_account_tax_rule_country.egg-info/PKG-INFO` & `trytond_account_tax_rule_country-7.2.0/trytond_account_tax_rule_country.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_account_tax_rule_country
-Version: 7.0.1
+Version: 7.2.0
 Summary: Tryton module to add countries on tax rules
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
@@ -48,22 +48,22 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_country<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_country<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: trytond_account_invoice<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_purchase<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_stock<7.1,>=7.0; extra == "test"
+Requires-Dist: trytond_account_invoice<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_purchase<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_stock<7.3,>=7.2; extra == "test"
 
 Account Tax Rule Country
 ########################
 
 The account_tax_rule module extends the tax rule to add origin and destination
 countries and subdivisions as criteria.
```

### Comparing `trytond_account_tax_rule_country-7.0.1/trytond_account_tax_rule_country.egg-info/SOURCES.txt` & `trytond_account_tax_rule_country-7.2.0/trytond_account_tax_rule_country.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-7.0.1/view/tax_rule_line_form.xml` & `trytond_account_tax_rule_country-7.2.0/view/tax_rule_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-7.0.1/view/tax_rule_line_template_form.xml` & `trytond_account_tax_rule_country-7.2.0/view/tax_rule_line_template_form.xml`

 * *Files identical despite different names*

