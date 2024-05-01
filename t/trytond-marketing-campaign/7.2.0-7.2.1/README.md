# Comparing `tmp/trytond_marketing_campaign-7.2.0.tar.gz` & `tmp/trytond_marketing_campaign-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_marketing_campaign-7.2.0.tar", last modified: Mon Apr 29 15:41:34 2024, max compression
+gzip compressed data, was "trytond_marketing_campaign-7.2.1.tar", last modified: Wed May  1 11:57:41 2024, max compression
```

## Comparing `trytond_marketing_campaign-7.2.0.tar` & `trytond_marketing_campaign-7.2.1.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:34.447645 trytond_marketing_campaign-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      561 2024-04-29 15:20:37.000000 trytond_marketing_campaign-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:20:37.000000 trytond_marketing_campaign-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_marketing_campaign-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_marketing_campaign-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3012 2024-04-29 15:41:34.447645 trytond_marketing_campaign-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      214 2023-04-15 07:12:15.000000 trytond_marketing_campaign-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2316 2024-04-22 12:14:36.000000 trytond_marketing_campaign-7.2.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:34.444311 trytond_marketing_campaign-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3081 2024-04-27 16:30:39.000000 trytond_marketing_campaign-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      526 2023-04-15 07:12:15.000000 trytond_marketing_campaign-7.2.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      214 2023-04-15 07:12:15.000000 trytond_marketing_campaign-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1048 2024-04-22 12:14:36.000000 trytond_marketing_campaign-7.2.0/doc/reference.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:12.000000 trytond_marketing_campaign-7.2.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:34.444311 trytond_marketing_campaign-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     4988 2024-04-29 13:17:17.000000 trytond_marketing_campaign-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5878 2024-04-29 13:17:17.000000 trytond_marketing_campaign-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4988 2024-04-29 13:17:17.000000 trytond_marketing_campaign-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6018 2024-04-29 13:17:17.000000 trytond_marketing_campaign-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5859 2024-04-29 13:17:17.000000 trytond_marketing_campaign-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4988 2024-04-29 13:17:17.000000 trytond_marketing_campaign-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4988 2024-04-29 13:17:17.000000 trytond_marketing_campaign-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4988 2024-04-29 13:17:17.000000 trytond_marketing_campaign-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4988 2024-04-29 13:17:17.000000 trytond_marketing_campaign-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5903 2024-04-29 13:17:17.000000 trytond_marketing_campaign-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4988 2024-04-29 13:17:17.000000 trytond_marketing_campaign-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4988 2024-04-29 13:17:17.000000 trytond_marketing_campaign-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4988 2024-04-29 13:17:17.000000 trytond_marketing_campaign-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4988 2024-04-29 13:17:17.000000 trytond_marketing_campaign-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4988 2024-04-29 13:17:17.000000 trytond_marketing_campaign-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5780 2024-04-29 13:17:17.000000 trytond_marketing_campaign-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4988 2024-04-29 13:17:17.000000 trytond_marketing_campaign-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4988 2024-04-29 13:17:17.000000 trytond_marketing_campaign-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4988 2024-04-29 13:17:17.000000 trytond_marketing_campaign-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4988 2024-04-29 13:17:17.000000 trytond_marketing_campaign-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5857 2024-04-29 13:17:17.000000 trytond_marketing_campaign-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4988 2024-04-29 13:17:17.000000 trytond_marketing_campaign-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4988 2024-04-29 13:17:17.000000 trytond_marketing_campaign-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4988 2024-04-29 13:17:17.000000 trytond_marketing_campaign-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5652 2024-04-22 12:14:36.000000 trytond_marketing_campaign-7.2.0/marketing.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4956 2024-04-22 12:14:36.000000 trytond_marketing_campaign-7.2.0/marketing.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      812 2023-04-15 07:12:15.000000 trytond_marketing_campaign-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      839 2023-04-15 07:12:15.000000 trytond_marketing_campaign-7.2.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1123 2023-04-15 07:12:15.000000 trytond_marketing_campaign-7.2.0/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3520 2024-02-04 18:51:26.000000 trytond_marketing_campaign-7.2.0/sale_opportunity_reporting.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2338 2023-04-15 07:12:15.000000 trytond_marketing_campaign-7.2.0/sale_opportunity_reporting.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3805 2023-04-15 07:12:15.000000 trytond_marketing_campaign-7.2.0/sale_reporting.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2071 2023-04-15 07:12:15.000000 trytond_marketing_campaign-7.2.0/sale_reporting.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:41:34.447645 trytond_marketing_campaign-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4940 2024-04-27 16:30:39.000000 trytond_marketing_campaign-7.2.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:34.444311 trytond_marketing_campaign-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_marketing_campaign-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5284 2024-04-22 12:14:36.000000 trytond_marketing_campaign-7.2.0/tests/scenario_marketing_campaign_sale.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1646 2024-04-22 12:14:36.000000 trytond_marketing_campaign-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_marketing_campaign-7.2.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:12.000000 trytond_marketing_campaign-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      286 2024-04-29 15:20:33.000000 trytond_marketing_campaign-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:34.447645 trytond_marketing_campaign-7.2.0/trytond_marketing_campaign.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3012 2024-04-29 15:41:34.000000 trytond_marketing_campaign-7.2.0/trytond_marketing_campaign.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2534 2024-04-29 15:41:34.000000 trytond_marketing_campaign-7.2.0/trytond_marketing_campaign.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:41:34.000000 trytond_marketing_campaign-7.2.0/trytond_marketing_campaign.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       74 2024-04-29 15:41:34.000000 trytond_marketing_campaign-7.2.0/trytond_marketing_campaign.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:55.000000 trytond_marketing_campaign-7.2.0/trytond_marketing_campaign.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      275 2024-04-29 15:41:34.000000 trytond_marketing_campaign-7.2.0/trytond_marketing_campaign.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:41:34.000000 trytond_marketing_campaign-7.2.0/trytond_marketing_campaign.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:34.447645 trytond_marketing_campaign-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      668 2023-04-15 07:12:15.000000 trytond_marketing_campaign-7.2.0/view/campaign_mixin_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      290 2023-04-15 07:12:15.000000 trytond_marketing_campaign-7.2.0/view/parameter_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      226 2023-04-15 07:12:15.000000 trytond_marketing_campaign-7.2.0/view/parameter_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      637 2023-04-15 07:12:15.000000 trytond_marketing_campaign-7.2.0/view/sale_opportunity_reporting_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      949 2023-04-15 07:12:15.000000 trytond_marketing_campaign-7.2.0/view/sale_opportunity_reporting_marketing_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      498 2023-04-15 07:12:15.000000 trytond_marketing_campaign-7.2.0/view/sale_opportunity_reporting_marketing_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      637 2023-04-15 07:12:15.000000 trytond_marketing_campaign-7.2.0/view/sale_reporting_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1009 2023-04-15 07:12:15.000000 trytond_marketing_campaign-7.2.0/view/sale_reporting_marketing_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      495 2023-04-15 07:12:15.000000 trytond_marketing_campaign-7.2.0/view/sale_reporting_marketing_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      505 2024-04-22 12:14:36.000000 trytond_marketing_campaign-7.2.0/web.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:57:41.699553 trytond_marketing_campaign-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)      662 2024-05-01 11:57:38.000000 trytond_marketing_campaign-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-05-01 11:57:38.000000 trytond_marketing_campaign-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:20:59.000000 trytond_marketing_campaign-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:20:59.000000 trytond_marketing_campaign-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3012 2024-05-01 11:57:41.699553 trytond_marketing_campaign-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      214 2024-04-30 17:20:59.000000 trytond_marketing_campaign-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2316 2024-04-30 17:20:59.000000 trytond_marketing_campaign-7.2.1/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:57:41.692887 trytond_marketing_campaign-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3081 2024-04-30 17:20:59.000000 trytond_marketing_campaign-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      526 2024-04-30 17:20:59.000000 trytond_marketing_campaign-7.2.1/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      214 2024-04-30 17:20:59.000000 trytond_marketing_campaign-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1048 2024-04-30 17:20:59.000000 trytond_marketing_campaign-7.2.1/doc/reference.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:20:59.000000 trytond_marketing_campaign-7.2.1/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:57:41.696220 trytond_marketing_campaign-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4988 2024-04-30 17:20:59.000000 trytond_marketing_campaign-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5804 2024-04-30 17:21:59.000000 trytond_marketing_campaign-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4988 2024-04-30 17:20:59.000000 trytond_marketing_campaign-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5922 2024-04-30 17:21:59.000000 trytond_marketing_campaign-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5787 2024-04-30 17:21:59.000000 trytond_marketing_campaign-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4988 2024-04-30 17:20:59.000000 trytond_marketing_campaign-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4988 2024-04-30 17:20:59.000000 trytond_marketing_campaign-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4988 2024-04-30 17:20:59.000000 trytond_marketing_campaign-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4988 2024-04-30 17:20:59.000000 trytond_marketing_campaign-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5831 2024-04-30 17:21:59.000000 trytond_marketing_campaign-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4988 2024-04-30 17:20:59.000000 trytond_marketing_campaign-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4988 2024-04-30 17:20:59.000000 trytond_marketing_campaign-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4988 2024-04-30 17:20:59.000000 trytond_marketing_campaign-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4988 2024-04-30 17:20:59.000000 trytond_marketing_campaign-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4988 2024-04-30 17:20:59.000000 trytond_marketing_campaign-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5708 2024-04-30 17:21:59.000000 trytond_marketing_campaign-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4988 2024-04-30 17:20:59.000000 trytond_marketing_campaign-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4988 2024-04-30 17:20:59.000000 trytond_marketing_campaign-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4988 2024-04-30 17:20:59.000000 trytond_marketing_campaign-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4988 2024-04-30 17:20:59.000000 trytond_marketing_campaign-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5857 2024-04-30 17:20:59.000000 trytond_marketing_campaign-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4988 2024-04-30 17:20:59.000000 trytond_marketing_campaign-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4988 2024-04-30 17:20:59.000000 trytond_marketing_campaign-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4988 2024-04-30 17:20:59.000000 trytond_marketing_campaign-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5652 2024-04-30 17:20:59.000000 trytond_marketing_campaign-7.2.1/marketing.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4956 2024-04-30 17:20:59.000000 trytond_marketing_campaign-7.2.1/marketing.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      812 2024-04-30 17:20:59.000000 trytond_marketing_campaign-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      839 2024-04-30 17:20:59.000000 trytond_marketing_campaign-7.2.1/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1123 2024-04-30 17:20:59.000000 trytond_marketing_campaign-7.2.1/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3520 2024-04-30 17:20:59.000000 trytond_marketing_campaign-7.2.1/sale_opportunity_reporting.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2338 2024-04-30 17:20:59.000000 trytond_marketing_campaign-7.2.1/sale_opportunity_reporting.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3805 2024-04-30 17:20:59.000000 trytond_marketing_campaign-7.2.1/sale_reporting.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2071 2024-04-30 17:20:59.000000 trytond_marketing_campaign-7.2.1/sale_reporting.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 11:57:41.699553 trytond_marketing_campaign-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4940 2024-04-30 17:20:59.000000 trytond_marketing_campaign-7.2.1/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:57:41.696220 trytond_marketing_campaign-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:20:59.000000 trytond_marketing_campaign-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5284 2024-04-30 17:20:59.000000 trytond_marketing_campaign-7.2.1/tests/scenario_marketing_campaign_sale.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1646 2024-04-30 17:20:59.000000 trytond_marketing_campaign-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:20:59.000000 trytond_marketing_campaign-7.2.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:20:59.000000 trytond_marketing_campaign-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      286 2024-04-30 17:21:06.000000 trytond_marketing_campaign-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:57:41.696220 trytond_marketing_campaign-7.2.1/trytond_marketing_campaign.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3012 2024-05-01 11:57:41.000000 trytond_marketing_campaign-7.2.1/trytond_marketing_campaign.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2534 2024-05-01 11:57:41.000000 trytond_marketing_campaign-7.2.1/trytond_marketing_campaign.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:57:41.000000 trytond_marketing_campaign-7.2.1/trytond_marketing_campaign.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       74 2024-05-01 11:57:41.000000 trytond_marketing_campaign-7.2.1/trytond_marketing_campaign.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:57:41.000000 trytond_marketing_campaign-7.2.1/trytond_marketing_campaign.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      275 2024-05-01 11:57:41.000000 trytond_marketing_campaign-7.2.1/trytond_marketing_campaign.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 11:57:41.000000 trytond_marketing_campaign-7.2.1/trytond_marketing_campaign.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:57:41.696220 trytond_marketing_campaign-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      668 2024-04-30 17:20:59.000000 trytond_marketing_campaign-7.2.1/view/campaign_mixin_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      290 2024-04-30 17:20:59.000000 trytond_marketing_campaign-7.2.1/view/parameter_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      226 2024-04-30 17:20:59.000000 trytond_marketing_campaign-7.2.1/view/parameter_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      637 2024-04-30 17:20:59.000000 trytond_marketing_campaign-7.2.1/view/sale_opportunity_reporting_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      949 2024-04-30 17:20:59.000000 trytond_marketing_campaign-7.2.1/view/sale_opportunity_reporting_marketing_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      498 2024-04-30 17:20:59.000000 trytond_marketing_campaign-7.2.1/view/sale_opportunity_reporting_marketing_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      637 2024-04-30 17:20:59.000000 trytond_marketing_campaign-7.2.1/view/sale_reporting_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1009 2024-04-30 17:20:59.000000 trytond_marketing_campaign-7.2.1/view/sale_reporting_marketing_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      495 2024-04-30 17:20:59.000000 trytond_marketing_campaign-7.2.1/view/sale_reporting_marketing_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      505 2024-04-30 17:20:59.000000 trytond_marketing_campaign-7.2.1/web.py
```

### Comparing `trytond_marketing_campaign-7.2.0/CHANGELOG` & `trytond_marketing_campaign-7.2.1/CHANGELOG`

 * *Files 13% similar despite different names*

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
 * Add UTM to automation activity
 * Add UTM to email message
 * Add UTM parameters to shortened URL
```

### Comparing `trytond_marketing_campaign-7.2.0/COPYRIGHT` & `trytond_marketing_campaign-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-7.2.0/LICENSE` & `trytond_marketing_campaign-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-7.2.0/PKG-INFO` & `trytond_marketing_campaign-7.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_marketing_campaign
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module to manage marketing campaign
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_marketing_campaign-7.2.0/__init__.py` & `trytond_marketing_campaign-7.2.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-7.2.0/doc/conf.py` & `trytond_marketing_campaign-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-7.2.0/doc/design.rst` & `trytond_marketing_campaign-7.2.1/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-7.2.0/doc/reference.rst` & `trytond_marketing_campaign-7.2.1/doc/reference.rst`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-7.2.0/locale/bg.po` & `trytond_marketing_campaign-7.2.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-7.2.0/locale/ca.po` & `trytond_marketing_campaign-7.2.1/locale/ca.po`

 * *Files 8% similar despite different names*

```diff
@@ -146,50 +146,42 @@
 msgid "Month"
 msgstr "Mes"
 
 msgctxt "selection:sale.reporting.marketing.context,period:"
 msgid "Year"
 msgstr "Any"
 
-#, fuzzy
 msgctxt "view:marketing.automation.activity:"
 msgid "Campaign"
 msgstr "Campanya"
 
-#, fuzzy
 msgctxt "view:marketing.automation.activity:"
 msgid "Marketing Campaign"
-msgstr "Campanyes de màrqueting"
+msgstr "Campanya de màrqueting"
 
-#, fuzzy
 msgctxt "view:marketing.automation.activity:"
 msgid "Medium"
 msgstr "Medi"
 
-#, fuzzy
 msgctxt "view:marketing.automation.activity:"
 msgid "Source"
 msgstr "Origen"
 
-#, fuzzy
 msgctxt "view:marketing.email.message:"
 msgid "Campaign"
 msgstr "Campanya"
 
-#, fuzzy
 msgctxt "view:marketing.email.message:"
 msgid "Marketing Campaign"
-msgstr "Campanyes de màrqueting"
+msgstr "Campanya de màrqueting"
 
-#, fuzzy
 msgctxt "view:marketing.email.message:"
 msgid "Medium"
 msgstr "Medi"
 
-#, fuzzy
 msgctxt "view:marketing.email.message:"
 msgid "Source"
 msgstr "Origen"
 
 msgctxt "view:sale.opportunity.reporting.context:"
 msgid "Marketing Campaign"
 msgstr "Campanya de màrqueting"
```

### Comparing `trytond_marketing_campaign-7.2.0/locale/cs.po` & `trytond_marketing_campaign-7.2.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-7.2.0/locale/de.po` & `trytond_marketing_campaign-7.2.1/locale/de.po`

 * *Files 4% similar despite different names*

```diff
@@ -146,50 +146,42 @@
 msgid "Month"
 msgstr "Monat"
 
 msgctxt "selection:sale.reporting.marketing.context,period:"
 msgid "Year"
 msgstr "Jahr"
 
-#, fuzzy
 msgctxt "view:marketing.automation.activity:"
 msgid "Campaign"
 msgstr "Kampagne"
 
-#, fuzzy
 msgctxt "view:marketing.automation.activity:"
 msgid "Marketing Campaign"
-msgstr "Mar­ke­ting­kam­pa­g­ne"
+msgstr "Marketingkampagne"
 
-#, fuzzy
 msgctxt "view:marketing.automation.activity:"
 msgid "Medium"
 msgstr "Medium"
 
-#, fuzzy
 msgctxt "view:marketing.automation.activity:"
 msgid "Source"
 msgstr "Ursprung"
 
-#, fuzzy
 msgctxt "view:marketing.email.message:"
 msgid "Campaign"
 msgstr "Kampagne"
 
-#, fuzzy
 msgctxt "view:marketing.email.message:"
 msgid "Marketing Campaign"
-msgstr "Mar­ke­ting­kam­pa­g­ne"
+msgstr "Marketingkampagne"
 
-#, fuzzy
 msgctxt "view:marketing.email.message:"
 msgid "Medium"
 msgstr "Medium"
 
-#, fuzzy
 msgctxt "view:marketing.email.message:"
 msgid "Source"
 msgstr "Ursprung"
 
 msgctxt "view:sale.opportunity.reporting.context:"
 msgid "Marketing Campaign"
 msgstr "Mar­ke­ting­kam­pa­g­ne"
```

### Comparing `trytond_marketing_campaign-7.2.0/locale/es.po` & `trytond_marketing_campaign-7.2.1/locale/es.po`

 * *Files 3% similar despite different names*

```diff
@@ -146,50 +146,42 @@
 msgid "Month"
 msgstr "Mes"
 
 msgctxt "selection:sale.reporting.marketing.context,period:"
 msgid "Year"
 msgstr "Año"
 
-#, fuzzy
 msgctxt "view:marketing.automation.activity:"
 msgid "Campaign"
 msgstr "Campaña"
 
-#, fuzzy
 msgctxt "view:marketing.automation.activity:"
 msgid "Marketing Campaign"
 msgstr "Campaña de marketing"
 
-#, fuzzy
 msgctxt "view:marketing.automation.activity:"
 msgid "Medium"
 msgstr "Medio"
 
-#, fuzzy
 msgctxt "view:marketing.automation.activity:"
 msgid "Source"
 msgstr "Origen"
 
-#, fuzzy
 msgctxt "view:marketing.email.message:"
 msgid "Campaign"
 msgstr "Campaña"
 
-#, fuzzy
 msgctxt "view:marketing.email.message:"
 msgid "Marketing Campaign"
 msgstr "Campaña de marketing"
 
-#, fuzzy
 msgctxt "view:marketing.email.message:"
 msgid "Medium"
 msgstr "Medio"
 
-#, fuzzy
 msgctxt "view:marketing.email.message:"
 msgid "Source"
 msgstr "Origen"
 
 msgctxt "view:sale.opportunity.reporting.context:"
 msgid "Marketing Campaign"
 msgstr "Campaña de marketing"
```

### Comparing `trytond_marketing_campaign-7.2.0/locale/es_419.po` & `trytond_marketing_campaign-7.2.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-7.2.0/locale/et.po` & `trytond_marketing_campaign-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-7.2.0/locale/fa.po` & `trytond_marketing_campaign-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-7.2.0/locale/fi.po` & `trytond_marketing_campaign-7.2.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-7.2.0/locale/fr.po` & `trytond_marketing_campaign-7.2.1/locale/fr.po`

 * *Files 6% similar despite different names*

```diff
@@ -146,50 +146,42 @@
 msgid "Month"
 msgstr "Mois"
 
 msgctxt "selection:sale.reporting.marketing.context,period:"
 msgid "Year"
 msgstr "Année"
 
-#, fuzzy
 msgctxt "view:marketing.automation.activity:"
 msgid "Campaign"
 msgstr "Campagne"
 
-#, fuzzy
 msgctxt "view:marketing.automation.activity:"
 msgid "Marketing Campaign"
 msgstr "Campagne de marketing"
 
-#, fuzzy
 msgctxt "view:marketing.automation.activity:"
 msgid "Medium"
 msgstr "Médium"
 
-#, fuzzy
 msgctxt "view:marketing.automation.activity:"
 msgid "Source"
 msgstr "Source"
 
-#, fuzzy
 msgctxt "view:marketing.email.message:"
 msgid "Campaign"
 msgstr "Campagne"
 
-#, fuzzy
 msgctxt "view:marketing.email.message:"
 msgid "Marketing Campaign"
 msgstr "Campagne de marketing"
 
-#, fuzzy
 msgctxt "view:marketing.email.message:"
 msgid "Medium"
 msgstr "Médium"
 
-#, fuzzy
 msgctxt "view:marketing.email.message:"
 msgid "Source"
 msgstr "Source"
 
 msgctxt "view:sale.opportunity.reporting.context:"
 msgid "Marketing Campaign"
 msgstr "Campagne de marketing"
```

### Comparing `trytond_marketing_campaign-7.2.0/locale/hu.po` & `trytond_marketing_campaign-7.2.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-7.2.0/locale/id.po` & `trytond_marketing_campaign-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-7.2.0/locale/it.po` & `trytond_marketing_campaign-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-7.2.0/locale/lo.po` & `trytond_marketing_campaign-7.2.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-7.2.0/locale/lt.po` & `trytond_marketing_campaign-7.2.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-7.2.0/locale/nl.po` & `trytond_marketing_campaign-7.2.1/locale/nl.po`

 * *Files 3% similar despite different names*

```diff
@@ -146,50 +146,42 @@
 msgid "Month"
 msgstr "Maand"
 
 msgctxt "selection:sale.reporting.marketing.context,period:"
 msgid "Year"
 msgstr "Jaar"
 
-#, fuzzy
 msgctxt "view:marketing.automation.activity:"
 msgid "Campaign"
 msgstr "Campagne"
 
-#, fuzzy
 msgctxt "view:marketing.automation.activity:"
 msgid "Marketing Campaign"
 msgstr "Marketing campagne"
 
-#, fuzzy
 msgctxt "view:marketing.automation.activity:"
 msgid "Medium"
 msgstr "Medium"
 
-#, fuzzy
 msgctxt "view:marketing.automation.activity:"
 msgid "Source"
 msgstr "Bron"
 
-#, fuzzy
 msgctxt "view:marketing.email.message:"
 msgid "Campaign"
 msgstr "Campagne"
 
-#, fuzzy
 msgctxt "view:marketing.email.message:"
 msgid "Marketing Campaign"
 msgstr "Marketing campagne"
 
-#, fuzzy
 msgctxt "view:marketing.email.message:"
 msgid "Medium"
 msgstr "Medium"
 
-#, fuzzy
 msgctxt "view:marketing.email.message:"
 msgid "Source"
 msgstr "Bron"
 
 msgctxt "view:sale.opportunity.reporting.context:"
 msgid "Marketing Campaign"
 msgstr "Marketing campagne"
```

### Comparing `trytond_marketing_campaign-7.2.0/locale/pl.po` & `trytond_marketing_campaign-7.2.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-7.2.0/locale/pt.po` & `trytond_marketing_campaign-7.2.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-7.2.0/locale/ro.po` & `trytond_marketing_campaign-7.2.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-7.2.0/locale/ru.po` & `trytond_marketing_campaign-7.2.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-7.2.0/locale/sl.po` & `trytond_marketing_campaign-7.2.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-7.2.0/locale/tr.po` & `trytond_marketing_campaign-7.2.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-7.2.0/locale/uk.po` & `trytond_marketing_campaign-7.2.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-7.2.0/locale/zh_CN.po` & `trytond_marketing_campaign-7.2.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-7.2.0/marketing.py` & `trytond_marketing_campaign-7.2.1/marketing.py`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-7.2.0/marketing.xml` & `trytond_marketing_campaign-7.2.1/marketing.xml`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-7.2.0/message.xml` & `trytond_marketing_campaign-7.2.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-7.2.0/sale.py` & `trytond_marketing_campaign-7.2.1/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-7.2.0/sale.xml` & `trytond_marketing_campaign-7.2.1/sale.xml`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-7.2.0/sale_opportunity_reporting.py` & `trytond_marketing_campaign-7.2.1/sale_opportunity_reporting.py`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-7.2.0/sale_opportunity_reporting.xml` & `trytond_marketing_campaign-7.2.1/sale_opportunity_reporting.xml`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-7.2.0/sale_reporting.py` & `trytond_marketing_campaign-7.2.1/sale_reporting.py`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-7.2.0/sale_reporting.xml` & `trytond_marketing_campaign-7.2.1/sale_reporting.xml`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-7.2.0/setup.py` & `trytond_marketing_campaign-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-7.2.0/tests/scenario_marketing_campaign_sale.rst` & `trytond_marketing_campaign-7.2.1/tests/scenario_marketing_campaign_sale.rst`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-7.2.0/tests/test_module.py` & `trytond_marketing_campaign-7.2.1/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-7.2.0/tox.ini` & `trytond_marketing_campaign-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-7.2.0/trytond_marketing_campaign.egg-info/PKG-INFO` & `trytond_marketing_campaign-7.2.1/trytond_marketing_campaign.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_marketing_campaign
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module to manage marketing campaign
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_marketing_campaign-7.2.0/trytond_marketing_campaign.egg-info/SOURCES.txt` & `trytond_marketing_campaign-7.2.1/trytond_marketing_campaign.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-7.2.0/view/campaign_mixin_form.xml` & `trytond_marketing_campaign-7.2.1/view/campaign_mixin_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-7.2.0/view/sale_opportunity_reporting_context_form.xml` & `trytond_marketing_campaign-7.2.1/view/sale_opportunity_reporting_context_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-7.2.0/view/sale_opportunity_reporting_marketing_context_form.xml` & `trytond_marketing_campaign-7.2.1/view/sale_opportunity_reporting_marketing_context_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-7.2.0/view/sale_reporting_context_form.xml` & `trytond_marketing_campaign-7.2.1/view/sale_reporting_context_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-7.2.0/view/sale_reporting_marketing_context_form.xml` & `trytond_marketing_campaign-7.2.1/view/sale_reporting_marketing_context_form.xml`

 * *Files identical despite different names*

