# Comparing `tmp/trytond_commission-7.2.0.tar.gz` & `tmp/trytond_commission-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_commission-7.2.0.tar", last modified: Mon Apr 29 15:39:08 2024, max compression
+gzip compressed data, was "trytond_commission-7.2.1.tar", last modified: Wed May  1 12:02:40 2024, max compression
```

## Comparing `trytond_commission-7.2.0.tar` & `trytond_commission-7.2.1.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:08.774788 trytond_commission-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     2700 2024-04-29 15:18:45.000000 trytond_commission-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-04-29 15:18:45.000000 trytond_commission-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_commission-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3218 2024-04-29 15:39:08.774788 trytond_commission-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      285 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1768 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      394 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)      452 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/account.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    22626 2024-01-27 09:58:52.000000 trytond_commission-7.2.0/commission.py
--rw-r--r--   0 ced       (1000) ced       (1000)    14258 2024-04-27 16:30:39.000000 trytond_commission-7.2.0/commission.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     8084 2024-04-22 12:14:36.000000 trytond_commission-7.2.0/commission_reporting.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8572 2024-04-27 16:30:39.000000 trytond_commission-7.2.0/commission_reporting.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:08.768121 trytond_commission-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3073 2024-04-27 16:30:39.000000 trytond_commission-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4008 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      285 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:07.000000 trytond_commission-7.2.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      872 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/doc/usage.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      246 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:08.768121 trytond_commission-7.2.0/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      586 2023-01-16 14:00:20.000000 trytond_commission-7.2.0/icons/tryton-commission.svg
--rw-r--r--   0 ced       (1000) ced       (1000)     9082 2024-01-27 09:58:52.000000 trytond_commission-7.2.0/invoice.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3713 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/invoice.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      936 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/ir.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:08.771454 trytond_commission-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    16314 2024-04-27 16:43:22.000000 trytond_commission-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17192 2024-04-27 16:43:22.000000 trytond_commission-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15228 2024-04-27 16:43:22.000000 trytond_commission-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17627 2024-04-27 16:43:22.000000 trytond_commission-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17297 2024-04-27 16:43:22.000000 trytond_commission-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14178 2024-04-27 16:43:22.000000 trytond_commission-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15826 2024-04-27 16:43:22.000000 trytond_commission-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17040 2024-04-27 16:43:22.000000 trytond_commission-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15215 2024-04-27 16:43:22.000000 trytond_commission-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17532 2024-04-27 16:43:22.000000 trytond_commission-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15741 2024-04-27 16:43:22.000000 trytond_commission-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14712 2024-04-27 16:43:22.000000 trytond_commission-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16162 2024-04-27 16:43:22.000000 trytond_commission-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16499 2024-04-27 16:43:22.000000 trytond_commission-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15442 2024-04-27 16:43:22.000000 trytond_commission-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17615 2024-04-29 13:17:17.000000 trytond_commission-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15612 2024-04-27 16:43:22.000000 trytond_commission-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16207 2024-04-27 16:43:22.000000 trytond_commission-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16639 2024-04-29 13:17:17.000000 trytond_commission-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16267 2024-04-27 16:43:22.000000 trytond_commission-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16131 2024-04-27 16:43:22.000000 trytond_commission-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15215 2024-04-27 16:43:22.000000 trytond_commission-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14133 2024-04-27 16:43:22.000000 trytond_commission-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15460 2024-04-27 16:43:22.000000 trytond_commission-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      682 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1327 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)      460 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1193 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-01-16 14:00:20.000000 trytond_commission-7.2.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3639 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)      715 2023-01-16 14:00:20.000000 trytond_commission-7.2.0/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:39:08.774788 trytond_commission-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4746 2024-03-17 11:01:36.000000 trytond_commission-7.2.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2132 2024-02-04 18:51:26.000000 trytond_commission-7.2.0/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)      478 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/stock.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1154 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/stock_reporting_margin.py
--rw-r--r--   0 ced       (1000) ced       (1000)      558 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/stock_reporting_margin.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:08.771454 trytond_commission-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2688 2024-04-22 12:14:36.000000 trytond_commission-7.2.0/tests/scenario_agent_selection.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     7319 2024-04-22 12:14:36.000000 trytond_commission-7.2.0/tests/scenario_commission.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3882 2024-04-22 12:14:36.000000 trytond_commission-7.2.0/tests/scenario_commission_credit_posted_invoice.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5752 2024-04-27 16:30:39.000000 trytond_commission-7.2.0/tests/scenario_commission_stock.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3670 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:07.000000 trytond_commission-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      382 2024-04-29 15:18:41.000000 trytond_commission-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:08.774788 trytond_commission-7.2.0/trytond_commission.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3218 2024-04-29 15:39:08.000000 trytond_commission-7.2.0/trytond_commission.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     4145 2024-04-29 15:39:08.000000 trytond_commission-7.2.0/trytond_commission.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:39:08.000000 trytond_commission-7.2.0/trytond_commission.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       58 2024-04-29 15:39:08.000000 trytond_commission-7.2.0/trytond_commission.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:02.000000 trytond_commission-7.2.0/trytond_commission.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      359 2024-04-29 15:39:08.000000 trytond_commission-7.2.0/trytond_commission.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:39:08.000000 trytond_commission-7.2.0/trytond_commission.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:08.774788 trytond_commission-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      334 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/view/account_invoice_credit_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      464 2023-01-16 14:00:20.000000 trytond_commission-7.2.0/view/agent_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      398 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/view/agent_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      587 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/view/agent_selection_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      327 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/view/agent_selection_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      347 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/view/agent_selection_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      376 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/view/commission_create_invoice_ask_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      720 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/view/commission_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      454 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/view/commission_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      358 2023-01-16 14:00:20.000000 trytond_commission-7.2.0/view/invoice_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      524 2023-01-16 14:00:20.000000 trytond_commission-7.2.0/view/invoice_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      399 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/view/party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      502 2023-01-16 14:00:20.000000 trytond_commission-7.2.0/view/plan_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      518 2023-01-16 14:00:20.000000 trytond_commission-7.2.0/view/plan_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      369 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/view/plan_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      324 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/view/plan_line_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/view/plan_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      319 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/view/reporting_agent_graph_amount.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      283 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/view/reporting_agent_graph_number.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      427 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/view/reporting_agent_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      318 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/view/reporting_agent_time_series_graph_amount.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      282 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/view/reporting_agent_time_series_graph_number.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      297 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/view/reporting_agent_time_series_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      537 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/view/reporting_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      359 2023-01-16 14:00:20.000000 trytond_commission-7.2.0/view/sale_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      415 2023-01-16 14:00:20.000000 trytond_commission-7.2.0/view/sale_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      345 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/view/stock_move_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      374 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/view/stock_reporting_margin_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-01-16 14:00:20.000000 trytond_commission-7.2.0/view/template_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:02:40.931727 trytond_commission-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2801 2024-05-01 12:02:37.000000 trytond_commission-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-05-01 12:02:37.000000 trytond_commission-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3218 2024-05-01 12:02:40.931727 trytond_commission-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      285 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1768 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      394 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      452 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/account.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    22626 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/commission.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    14258 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/commission.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     8084 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/commission_reporting.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8572 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/commission_reporting.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:02:40.921727 trytond_commission-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3073 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4008 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      285 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      872 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/doc/usage.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      246 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:02:40.925060 trytond_commission-7.2.1/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      586 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/icons/tryton-commission.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)     9082 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/invoice.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3713 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/invoice.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      936 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/ir.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:02:40.925060 trytond_commission-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    16314 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17192 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15228 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17627 2024-04-30 17:21:59.000000 trytond_commission-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17297 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14178 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15826 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17040 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15215 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17532 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15741 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14712 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16162 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16499 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15442 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17617 2024-04-30 17:21:59.000000 trytond_commission-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15624 2024-04-30 17:21:59.000000 trytond_commission-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16207 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16639 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16267 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16131 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15215 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14133 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15460 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      682 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1327 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      460 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1193 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      470 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3639 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      715 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 12:02:40.931727 trytond_commission-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4746 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2132 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      478 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/stock.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1154 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/stock_reporting_margin.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      558 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/stock_reporting_margin.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:02:40.925060 trytond_commission-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2688 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/tests/scenario_agent_selection.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     7319 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/tests/scenario_commission.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3882 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/tests/scenario_commission_credit_posted_invoice.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5752 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/tests/scenario_commission_stock.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3670 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      382 2024-04-30 17:21:06.000000 trytond_commission-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:02:40.928394 trytond_commission-7.2.1/trytond_commission.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3218 2024-05-01 12:02:40.000000 trytond_commission-7.2.1/trytond_commission.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     4145 2024-05-01 12:02:40.000000 trytond_commission-7.2.1/trytond_commission.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:02:40.000000 trytond_commission-7.2.1/trytond_commission.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       58 2024-05-01 12:02:40.000000 trytond_commission-7.2.1/trytond_commission.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:02:40.000000 trytond_commission-7.2.1/trytond_commission.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      359 2024-05-01 12:02:40.000000 trytond_commission-7.2.1/trytond_commission.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 12:02:40.000000 trytond_commission-7.2.1/trytond_commission.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:02:40.928394 trytond_commission-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      334 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/view/account_invoice_credit_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      464 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/view/agent_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      398 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/view/agent_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      587 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/view/agent_selection_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      327 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/view/agent_selection_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      347 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/view/agent_selection_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      376 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/view/commission_create_invoice_ask_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      720 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/view/commission_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      454 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/view/commission_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      358 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/view/invoice_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      524 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/view/invoice_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      399 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/view/party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      502 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/view/plan_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      518 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/view/plan_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      369 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/view/plan_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      324 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/view/plan_line_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/view/plan_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      319 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/view/reporting_agent_graph_amount.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      283 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/view/reporting_agent_graph_number.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      427 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/view/reporting_agent_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      318 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/view/reporting_agent_time_series_graph_amount.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      282 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/view/reporting_agent_time_series_graph_number.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      297 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/view/reporting_agent_time_series_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      537 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/view/reporting_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      359 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/view/sale_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      415 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/view/sale_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      345 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/view/stock_move_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      374 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/view/stock_reporting_margin_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      371 2024-04-30 17:20:59.000000 trytond_commission-7.2.1/view/template_form.xml
```

### Comparing `trytond_commission-7.2.0/CHANGELOG` & `trytond_commission-7.2.1/CHANGELOG`

 * *Files 7% similar despite different names*

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

### Comparing `trytond_commission-7.2.0/COPYRIGHT` & `trytond_commission-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.2.0/LICENSE` & `trytond_commission-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.2.0/PKG-INFO` & `trytond_commission-7.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_commission
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module for commission
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_commission-7.2.0/__init__.py` & `trytond_commission-7.2.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.2.0/commission.py` & `trytond_commission-7.2.1/commission.py`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.2.0/commission.xml` & `trytond_commission-7.2.1/commission.xml`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.2.0/commission_reporting.py` & `trytond_commission-7.2.1/commission_reporting.py`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.2.0/commission_reporting.xml` & `trytond_commission-7.2.1/commission_reporting.xml`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.2.0/doc/conf.py` & `trytond_commission-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.2.0/doc/design.rst` & `trytond_commission-7.2.1/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.2.0/doc/usage.rst` & `trytond_commission-7.2.1/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.2.0/icons/LICENSE` & `trytond_commission-7.2.1/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.2.0/icons/tryton-commission.svg` & `trytond_commission-7.2.1/icons/tryton-commission.svg`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.2.0/invoice.py` & `trytond_commission-7.2.1/invoice.py`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.2.0/invoice.xml` & `trytond_commission-7.2.1/invoice.xml`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.2.0/ir.py` & `trytond_commission-7.2.1/ir.py`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.2.0/locale/bg.po` & `trytond_commission-7.2.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.2.0/locale/ca.po` & `trytond_commission-7.2.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.2.0/locale/cs.po` & `trytond_commission-7.2.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.2.0/locale/de.po` & `trytond_commission-7.2.1/locale/de.po`

 * *Files 0% similar despite different names*

```diff
@@ -506,24 +506,24 @@
 
 msgctxt "model:ir.model.button,string:commission_invoice_button"
 msgid "Invoice"
 msgstr "Rechnung erstellen"
 
 msgctxt "model:ir.rule.group,name:rule_group_agent_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.rule.group,name:rule_group_reporting_agent_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt ""
 "model:ir.rule.group,name:rule_group_reporting_agent_time_series_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.ui.menu,name:menu_agent_form"
 msgid "Agents"
 msgstr "Vertreter"
 
 msgctxt "model:ir.ui.menu,name:menu_commission"
 msgid "Commission"
```

### Comparing `trytond_commission-7.2.0/locale/es.po` & `trytond_commission-7.2.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.2.0/locale/es_419.po` & `trytond_commission-7.2.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.2.0/locale/et.po` & `trytond_commission-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.2.0/locale/fa.po` & `trytond_commission-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.2.0/locale/fi.po` & `trytond_commission-7.2.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.2.0/locale/fr.po` & `trytond_commission-7.2.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.2.0/locale/hu.po` & `trytond_commission-7.2.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.2.0/locale/id.po` & `trytond_commission-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.2.0/locale/it.po` & `trytond_commission-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.2.0/locale/lo.po` & `trytond_commission-7.2.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.2.0/locale/lt.po` & `trytond_commission-7.2.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.2.0/locale/nl.po` & `trytond_commission-7.2.1/locale/nl.po`

 * *Files 0% similar despite different names*

```diff
@@ -497,15 +497,15 @@
 "aankopencommissies in behandeling hebben bij bedrijf \"%(company)s\"."
 
 msgctxt "model:ir.message,text:msg_plan_line_invalid_formula"
 msgid ""
 "Invalid formula \"%(formula)s\" in commission plan line \"%(line)s\" with "
 "exception \"%(exception)s\"."
 msgstr ""
-"Ongeldige formule \"%(formula)s\" in commissieplanlijn \"% (line)s\" met "
+"Ongeldige formule \"%(formula)s\" in regel commissie plan \"%(line)s\" met "
 "uitzondering \"%(exception)s\"."
 
 msgctxt "model:ir.model.button,string:commission_invoice_button"
 msgid "Invoice"
 msgstr "Factuur"
 
 msgctxt "model:ir.rule.group,name:rule_group_agent_companies"
```

### Comparing `trytond_commission-7.2.0/locale/pl.po` & `trytond_commission-7.2.1/locale/pl.po`

 * *Files 0% similar despite different names*

```diff
@@ -584,15 +584,15 @@
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_plan_form"
 msgid "Plans"
 msgstr "Plan"
 
 msgctxt "model:ir.ui.menu,name:menu_reporting"
 msgid "Reporting"
-msgstr ""
+msgstr "Raportowanie"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_reporting_commission"
 msgid "Commissions"
 msgstr "Commissions"
 
 msgctxt "model:product.template-commission.agent,name:"
```

### Comparing `trytond_commission-7.2.0/locale/pt.po` & `trytond_commission-7.2.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.2.0/locale/ro.po` & `trytond_commission-7.2.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.2.0/locale/ru.po` & `trytond_commission-7.2.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.2.0/locale/sl.po` & `trytond_commission-7.2.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.2.0/locale/tr.po` & `trytond_commission-7.2.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.2.0/locale/uk.po` & `trytond_commission-7.2.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.2.0/locale/zh_CN.po` & `trytond_commission-7.2.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.2.0/message.xml` & `trytond_commission-7.2.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.2.0/party.py` & `trytond_commission-7.2.1/party.py`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.2.0/product.py` & `trytond_commission-7.2.1/product.py`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.2.0/sale.py` & `trytond_commission-7.2.1/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.2.0/sale.xml` & `trytond_commission-7.2.1/sale.xml`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.2.0/setup.py` & `trytond_commission-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.2.0/stock.py` & `trytond_commission-7.2.1/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.2.0/stock_reporting_margin.py` & `trytond_commission-7.2.1/stock_reporting_margin.py`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.2.0/stock_reporting_margin.xml` & `trytond_commission-7.2.1/stock_reporting_margin.xml`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.2.0/tests/scenario_agent_selection.rst` & `trytond_commission-7.2.1/tests/scenario_agent_selection.rst`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.2.0/tests/scenario_commission.rst` & `trytond_commission-7.2.1/tests/scenario_commission.rst`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.2.0/tests/scenario_commission_credit_posted_invoice.rst` & `trytond_commission-7.2.1/tests/scenario_commission_credit_posted_invoice.rst`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.2.0/tests/scenario_commission_stock.rst` & `trytond_commission-7.2.1/tests/scenario_commission_stock.rst`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.2.0/tests/test_module.py` & `trytond_commission-7.2.1/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.2.0/tox.ini` & `trytond_commission-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.2.0/trytond_commission.egg-info/PKG-INFO` & `trytond_commission-7.2.1/trytond_commission.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_commission
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module for commission
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_commission-7.2.0/trytond_commission.egg-info/SOURCES.txt` & `trytond_commission-7.2.1/trytond_commission.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.2.0/view/agent_selection_form.xml` & `trytond_commission-7.2.1/view/agent_selection_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.2.0/view/commission_form.xml` & `trytond_commission-7.2.1/view/commission_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.2.0/view/invoice_line_form.xml` & `trytond_commission-7.2.1/view/invoice_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.2.0/view/plan_line_form.xml` & `trytond_commission-7.2.1/view/plan_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.2.0/view/reporting_context_form.xml` & `trytond_commission-7.2.1/view/reporting_context_form.xml`

 * *Files identical despite different names*

