# Comparing `tmp/trytond_marketing_automation-7.2.0.tar.gz` & `tmp/trytond_marketing_automation-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_marketing_automation-7.2.0.tar", last modified: Mon Apr 29 15:41:28 2024, max compression
+gzip compressed data, was "trytond_marketing_automation-7.2.1.tar", last modified: Wed May  1 11:58:01 2024, max compression
```

## Comparing `trytond_marketing_automation-7.2.0.tar` & `trytond_marketing_automation-7.2.1.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:28.061145 trytond_marketing_automation-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1639 2024-04-29 15:20:32.000000 trytond_marketing_automation-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      720 2024-04-29 15:20:32.000000 trytond_marketing_automation-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2957 2024-04-29 15:41:28.061145 trytond_marketing_automation-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      263 2024-04-22 12:14:36.000000 trytond_marketing_automation-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1072 2024-04-22 12:14:36.000000 trytond_marketing_automation-7.2.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:28.057812 trytond_marketing_automation-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3083 2024-04-27 16:30:39.000000 trytond_marketing_automation-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      583 2024-04-22 12:14:36.000000 trytond_marketing_automation-7.2.0/doc/configuration.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2615 2024-04-22 12:14:36.000000 trytond_marketing_automation-7.2.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      263 2024-04-22 12:14:36.000000 trytond_marketing_automation-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-22 12:14:36.000000 trytond_marketing_automation-7.2.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:12.000000 trytond_marketing_automation-7.2.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       43 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.2.0/empty.gif
--rw-r--r--   0 ced       (1000) ced       (1000)      344 2024-04-04 22:18:16.000000 trytond_marketing_automation-7.2.0/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1367 2024-01-27 09:58:52.000000 trytond_marketing_automation-7.2.0/ir.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1711 2024-01-27 09:58:52.000000 trytond_marketing_automation-7.2.0/ir.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:28.057812 trytond_marketing_automation-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    14798 2024-04-29 13:17:17.000000 trytond_marketing_automation-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    18429 2024-04-29 13:17:17.000000 trytond_marketing_automation-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14798 2024-04-29 13:17:17.000000 trytond_marketing_automation-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    18148 2024-04-29 13:17:17.000000 trytond_marketing_automation-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    18557 2024-04-29 13:17:17.000000 trytond_marketing_automation-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14798 2024-04-29 13:17:17.000000 trytond_marketing_automation-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16430 2024-04-29 13:17:17.000000 trytond_marketing_automation-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14798 2024-04-29 13:17:17.000000 trytond_marketing_automation-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14798 2024-04-29 13:17:17.000000 trytond_marketing_automation-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    18276 2024-04-29 13:17:17.000000 trytond_marketing_automation-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14798 2024-04-29 13:17:17.000000 trytond_marketing_automation-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15090 2024-04-29 13:17:17.000000 trytond_marketing_automation-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16077 2024-04-29 13:17:17.000000 trytond_marketing_automation-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14798 2024-04-29 13:17:17.000000 trytond_marketing_automation-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14798 2024-04-29 13:17:17.000000 trytond_marketing_automation-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17996 2024-04-29 13:17:17.000000 trytond_marketing_automation-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14798 2024-04-29 13:17:17.000000 trytond_marketing_automation-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14798 2024-04-29 13:17:17.000000 trytond_marketing_automation-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14826 2024-04-29 13:17:17.000000 trytond_marketing_automation-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14798 2024-04-29 13:17:17.000000 trytond_marketing_automation-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16995 2024-04-29 13:17:17.000000 trytond_marketing_automation-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14798 2024-04-29 13:17:17.000000 trytond_marketing_automation-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14798 2024-04-29 13:17:17.000000 trytond_marketing_automation-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14798 2024-04-29 13:17:17.000000 trytond_marketing_automation-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)    37559 2024-04-29 13:17:17.000000 trytond_marketing_automation-7.2.0/marketing_automation.py
--rw-r--r--   0 ced       (1000) ced       (1000)    16310 2024-04-27 16:30:39.000000 trytond_marketing_automation-7.2.0/marketing_automation.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     8800 2024-04-22 12:14:36.000000 trytond_marketing_automation-7.2.0/marketing_automation_reporting.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5353 2024-04-22 12:14:36.000000 trytond_marketing_automation-7.2.0/marketing_automation_reporting.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1574 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      575 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.2.0/mixin.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1683 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.2.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)      454 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.2.0/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1257 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.2.0/routes.py
--rw-r--r--   0 ced       (1000) ced       (1000)      539 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.2.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:41:28.061145 trytond_marketing_automation-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4817 2024-04-27 16:30:39.000000 trytond_marketing_automation-7.2.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:28.057812 trytond_marketing_automation-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      464 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.2.0/tests/email.html
--rw-r--r--   0 ced       (1000) ced       (1000)      218 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.2.0/tests/reminder.html
--rw-r--r--   0 ced       (1000) ced       (1000)     8496 2024-04-27 16:30:39.000000 trytond_marketing_automation-7.2.0/tests/scenario_marketing_automation.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3273 2024-04-27 16:30:39.000000 trytond_marketing_automation-7.2.0/tests/scenario_marketing_automation_unsubscribable.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      369 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.2.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:12.000000 trytond_marketing_automation-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      227 2024-04-29 15:20:28.000000 trytond_marketing_automation-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:28.061145 trytond_marketing_automation-7.2.0/trytond_marketing_automation.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2957 2024-04-29 15:41:27.000000 trytond_marketing_automation-7.2.0/trytond_marketing_automation.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     3201 2024-04-29 15:41:28.000000 trytond_marketing_automation-7.2.0/trytond_marketing_automation.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:41:27.000000 trytond_marketing_automation-7.2.0/trytond_marketing_automation.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       78 2024-04-29 15:41:27.000000 trytond_marketing_automation-7.2.0/trytond_marketing_automation.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:57.000000 trytond_marketing_automation-7.2.0/trytond_marketing_automation.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      200 2024-04-29 15:41:27.000000 trytond_marketing_automation-7.2.0/trytond_marketing_automation.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:41:27.000000 trytond_marketing_automation-7.2.0/trytond_marketing_automation.egg-info/top_level.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      554 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.2.0/unsubscribe.html
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:28.061145 trytond_marketing_automation-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)     1400 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.2.0/view/activity_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      825 2024-04-22 12:14:36.000000 trytond_marketing_automation-7.2.0/view/activity_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      472 2024-01-27 09:58:52.000000 trytond_marketing_automation-7.2.0/view/ir_email_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      422 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.2.0/view/party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      538 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.2.0/view/record_activity_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      445 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.2.0/view/record_activity_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      394 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.2.0/view/record_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      338 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.2.0/view/record_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      363 2024-04-22 12:14:36.000000 trytond_marketing_automation-7.2.0/view/reporting_activity_graph_count.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      423 2024-04-22 12:14:36.000000 trytond_marketing_automation-7.2.0/view/reporting_activity_graph_rate.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      734 2024-04-22 12:14:36.000000 trytond_marketing_automation-7.2.0/view/reporting_activity_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      364 2024-04-22 12:14:36.000000 trytond_marketing_automation-7.2.0/view/reporting_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      333 2024-04-22 12:14:36.000000 trytond_marketing_automation-7.2.0/view/reporting_scenario_graph_count.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      308 2024-04-22 12:14:36.000000 trytond_marketing_automation-7.2.0/view/reporting_scenario_graph_rate.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      444 2024-04-22 12:14:36.000000 trytond_marketing_automation-7.2.0/view/reporting_scenario_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      812 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.2.0/view/scenario_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      501 2024-04-22 12:14:36.000000 trytond_marketing_automation-7.2.0/view/scenario_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      645 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.2.0/web.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:58:01.855692 trytond_marketing_automation-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1740 2024-05-01 11:57:58.000000 trytond_marketing_automation-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      720 2024-05-01 11:57:58.000000 trytond_marketing_automation-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2957 2024-05-01 11:58:01.855692 trytond_marketing_automation-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      263 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1072 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:58:01.849026 trytond_marketing_automation-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3083 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      583 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/doc/configuration.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2615 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      263 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       43 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/empty.gif
+-rw-r--r--   0 ced       (1000) ced       (1000)      344 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1367 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/ir.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1711 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/ir.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:58:01.852359 trytond_marketing_automation-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    14798 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18368 2024-04-30 17:21:59.000000 trytond_marketing_automation-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14798 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17997 2024-04-30 17:21:59.000000 trytond_marketing_automation-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18427 2024-04-30 17:21:59.000000 trytond_marketing_automation-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14798 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16430 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14798 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14798 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18359 2024-04-30 17:21:59.000000 trytond_marketing_automation-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14798 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15090 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16077 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14798 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14798 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18039 2024-04-30 17:21:59.000000 trytond_marketing_automation-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14798 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14798 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14826 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14798 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16995 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14798 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14798 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14798 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37559 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/marketing_automation.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    16310 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/marketing_automation.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     8800 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/marketing_automation_reporting.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5353 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/marketing_automation_reporting.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1574 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      575 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/mixin.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1683 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      454 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1257 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/routes.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      539 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 11:58:01.855692 trytond_marketing_automation-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4817 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:58:01.852359 trytond_marketing_automation-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      464 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/tests/email.html
+-rw-r--r--   0 ced       (1000) ced       (1000)      218 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/tests/reminder.html
+-rw-r--r--   0 ced       (1000) ced       (1000)     8496 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/tests/scenario_marketing_automation.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3273 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/tests/scenario_marketing_automation_unsubscribable.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      369 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      227 2024-04-30 17:21:06.000000 trytond_marketing_automation-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:58:01.855692 trytond_marketing_automation-7.2.1/trytond_marketing_automation.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2957 2024-05-01 11:58:01.000000 trytond_marketing_automation-7.2.1/trytond_marketing_automation.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     3201 2024-05-01 11:58:01.000000 trytond_marketing_automation-7.2.1/trytond_marketing_automation.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:58:01.000000 trytond_marketing_automation-7.2.1/trytond_marketing_automation.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       78 2024-05-01 11:58:01.000000 trytond_marketing_automation-7.2.1/trytond_marketing_automation.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:58:01.000000 trytond_marketing_automation-7.2.1/trytond_marketing_automation.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      200 2024-05-01 11:58:01.000000 trytond_marketing_automation-7.2.1/trytond_marketing_automation.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 11:58:01.000000 trytond_marketing_automation-7.2.1/trytond_marketing_automation.egg-info/top_level.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      554 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/unsubscribe.html
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:58:01.855692 trytond_marketing_automation-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1400 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/view/activity_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      825 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/view/activity_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      472 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/view/ir_email_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      422 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/view/party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      538 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/view/record_activity_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      445 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/view/record_activity_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      394 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/view/record_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      338 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/view/record_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      363 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/view/reporting_activity_graph_count.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      423 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/view/reporting_activity_graph_rate.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      734 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/view/reporting_activity_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      364 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/view/reporting_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      333 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/view/reporting_scenario_graph_count.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      308 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/view/reporting_scenario_graph_rate.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      444 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/view/reporting_scenario_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      812 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/view/scenario_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      501 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/view/scenario_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      645 2024-04-30 17:20:59.000000 trytond_marketing_automation-7.2.1/web.py
```

### Comparing `trytond_marketing_automation-7.2.0/CHANGELOG` & `trytond_marketing_automation-7.2.1/CHANGELOG`

 * *Files 5% similar despite different names*

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
 * Add trend spark lines
 * Add reporting on scenario and activity per period
 * Display block rate instead of absolute value
 * Display email rates instead of absolute value
```

### Comparing `trytond_marketing_automation-7.2.0/COPYRIGHT` & `trytond_marketing_automation-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-7.2.0/LICENSE` & `trytond_marketing_automation-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-7.2.0/PKG-INFO` & `trytond_marketing_automation-7.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_marketing_automation
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module to plan, coordinate and manage marketing campaigns
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_marketing_automation-7.2.0/__init__.py` & `trytond_marketing_automation-7.2.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-7.2.0/doc/conf.py` & `trytond_marketing_automation-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-7.2.0/doc/configuration.rst` & `trytond_marketing_automation-7.2.1/doc/configuration.rst`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-7.2.0/doc/design.rst` & `trytond_marketing_automation-7.2.1/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-7.2.0/ir.py` & `trytond_marketing_automation-7.2.1/ir.py`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-7.2.0/ir.xml` & `trytond_marketing_automation-7.2.1/ir.xml`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-7.2.0/locale/bg.po` & `trytond_marketing_automation-7.2.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-7.2.0/locale/ca.po` & `trytond_marketing_automation-7.2.1/locale/nl.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,668 +1,645 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:ir.email,marketing_automation_activity:"
 msgid "Activity"
-msgstr "Activitat"
+msgstr "Activiteit"
 
 msgctxt "field:ir.email,marketing_automation_record:"
 msgid "Record"
-msgstr "Registre"
+msgstr "Record"
 
 msgctxt "field:marketing.automation.activity,action:"
 msgid "Action"
-msgstr "Acció"
+msgstr "Actie"
 
 msgctxt "field:marketing.automation.activity,children:"
 msgid "Children"
-msgstr "Fills"
+msgstr "Onderliggende niveaus"
 
 msgctxt "field:marketing.automation.activity,condition:"
 msgid "Condition"
-msgstr "Condició"
+msgstr "Voorwaarde"
 
 msgctxt "field:marketing.automation.activity,delay:"
 msgid "Delay"
-msgstr "Retard"
+msgstr "Vertraging"
 
-#, fuzzy
 msgctxt "field:marketing.automation.activity,email_click_rate:"
 msgid "E-mail Click Rate"
-msgstr "Correus electrònics clicats"
+msgstr "Percentage email geklikt"
 
-#, fuzzy
 msgctxt "field:marketing.automation.activity,email_click_rate_trend:"
 msgid "E-mail Click Rate Trend"
-msgstr "Correus electrònics clicats"
+msgstr "Trend percentage email geklikt"
 
-#, fuzzy
 msgctxt "field:marketing.automation.activity,email_click_through_rate:"
 msgid "E-mail Click-Through Rate"
-msgstr "Correus electrònics clicats"
+msgstr "Percentage email doorgeklikt"
 
 msgctxt "field:marketing.automation.activity,email_click_through_rate_trend:"
 msgid "E-mail Click-Through Rate Trend"
-msgstr ""
+msgstr "Trend percentage email doorgeklikt"
 
 msgctxt "field:marketing.automation.activity,email_clicked:"
 msgid "E-Mails Clicked"
-msgstr "Correus electrònics clicats"
+msgstr "E-mails Geklikt"
 
 msgctxt "field:marketing.automation.activity,email_from:"
 msgid "From"
-msgstr "De"
+msgstr "Van"
 
-#, fuzzy
 msgctxt "field:marketing.automation.activity,email_open_rate:"
 msgid "E-mail Open Rate"
-msgstr "Correus electrònics oberts"
+msgstr "Percentage email geopend"
 
-#, fuzzy
 msgctxt "field:marketing.automation.activity,email_open_rate_trend:"
 msgid "E-mail Open Rate Trend"
-msgstr "Correus electrònics oberts"
+msgstr "Trend percentage email geopend"
 
 msgctxt "field:marketing.automation.activity,email_opened:"
 msgid "E-Mails Opened"
-msgstr "Correus electrònics oberts"
+msgstr "E-mails geopend"
 
 msgctxt "field:marketing.automation.activity,email_template:"
 msgid "E-Mail Template"
-msgstr "Plantilla de correu electrònic"
+msgstr "Email sjabloon"
 
 msgctxt "field:marketing.automation.activity,email_title:"
 msgid "E-Mail Title"
-msgstr "Títol del correu electrònic"
+msgstr "E-mail titel"
 
 msgctxt "field:marketing.automation.activity,event:"
 msgid "Event"
-msgstr "Esdeveniment"
+msgstr "Evenement"
 
 msgctxt "field:marketing.automation.activity,name:"
 msgid "Name"
-msgstr "Nom"
+msgstr "Naam"
 
 msgctxt "field:marketing.automation.activity,negative:"
 msgid "Negative"
-msgstr "Negatiu"
+msgstr "Negatief"
 
 msgctxt "field:marketing.automation.activity,on:"
 msgid "On"
-msgstr "A"
+msgstr "Op"
 
 msgctxt "field:marketing.automation.activity,parent:"
 msgid "Parent"
-msgstr "Pare"
+msgstr "Bovenliggend niveau"
 
 msgctxt "field:marketing.automation.activity,parent_action:"
 msgid "Parent Action"
-msgstr "Acció pare"
+msgstr "Bovenliggende actie (parent)"
 
 msgctxt "field:marketing.automation.activity,record_count:"
 msgid "Records"
-msgstr "Registres"
+msgstr "Records"
 
 msgctxt "field:marketing.automation.record,blocked:"
 msgid "Blocked"
-msgstr "Bloquejat"
+msgstr "geblokkeerd"
 
 msgctxt "field:marketing.automation.record,record:"
 msgid "Record"
-msgstr "Registre"
+msgstr "Record"
 
 msgctxt "field:marketing.automation.record,scenario:"
 msgid "Scenario"
-msgstr "Escenari"
+msgstr "Scenario"
 
 msgctxt "field:marketing.automation.record,uuid:"
 msgid "UUID"
-msgstr "Identificador únic universal"
+msgstr "UUID"
 
 msgctxt "field:marketing.automation.record.activity,activity:"
 msgid "Activity"
-msgstr "Activitat"
+msgstr "Activiteit"
 
 msgctxt "field:marketing.automation.record.activity,activity_action:"
 msgid "Activity Action"
-msgstr "Acció d'activitat"
+msgstr "Activiteit actie"
 
 msgctxt "field:marketing.automation.record.activity,at:"
 msgid "At"
-msgstr "A"
+msgstr "Op"
 
 msgctxt "field:marketing.automation.record.activity,email_clicked:"
 msgid "E-Mail Clicked"
-msgstr "Correus electrònics clicats"
+msgstr "E-mail Geklikt"
 
 msgctxt "field:marketing.automation.record.activity,email_opened:"
 msgid "E-Mail Opened"
-msgstr "Correus electrònics oberts"
+msgstr "E-mails geopend"
 
 msgctxt "field:marketing.automation.record.activity,record:"
 msgid "Record"
-msgstr "Registre"
+msgstr "Record"
 
 msgctxt "field:marketing.automation.record.activity,state:"
 msgid "State"
-msgstr "Estat"
+msgstr "Status"
 
-#, fuzzy
 msgctxt "field:marketing.automation.reporting.activity,activity:"
 msgid "Activity"
-msgstr "Activitat"
+msgstr "Activiteit"
 
-#, fuzzy
 msgctxt "field:marketing.automation.reporting.activity,activity_action:"
 msgid "Activity Action"
-msgstr "Acció d'activitat"
+msgstr "Activiteit actie"
 
 msgctxt "field:marketing.automation.reporting.activity,date:"
 msgid "Date"
-msgstr ""
+msgstr "Datum"
 
-#, fuzzy
 msgctxt "field:marketing.automation.reporting.activity,email_click_rate:"
 msgid "E-mail Click Rate"
-msgstr "Correus electrònics clicats"
+msgstr "Percentage email geklikt"
 
-#, fuzzy
 msgctxt ""
 "field:marketing.automation.reporting.activity,email_click_through_rate:"
 msgid "E-mail Click-Through Rate"
-msgstr "Correus electrònics clicats"
+msgstr "Percentage email doorgeklikt"
 
-#, fuzzy
 msgctxt "field:marketing.automation.reporting.activity,email_clicked:"
 msgid "E-Mails Clicked"
-msgstr "Correus electrònics clicats"
+msgstr "Op email geklikt"
 
-#, fuzzy
 msgctxt "field:marketing.automation.reporting.activity,email_open_rate:"
 msgid "E-mail Open Rate"
-msgstr "Correus electrònics oberts"
+msgstr "Percentage email geopend"
 
-#, fuzzy
 msgctxt "field:marketing.automation.reporting.activity,email_opened:"
 msgid "E-Mails Opened"
-msgstr "Correus electrònics oberts"
+msgstr "Email geopend"
 
-#, fuzzy
 msgctxt "field:marketing.automation.reporting.activity,record_count:"
 msgid "Records"
-msgstr "Registres"
+msgstr "Records"
 
-#, fuzzy
 msgctxt "field:marketing.automation.reporting.context,from_date:"
 msgid "From Date"
-msgstr "Data de modificació"
+msgstr "Vanaf datum"
 
 msgctxt "field:marketing.automation.reporting.context,period:"
 msgid "Period"
-msgstr ""
+msgstr "Periode"
 
 msgctxt "field:marketing.automation.reporting.context,to_date:"
 msgid "To Date"
-msgstr ""
+msgstr "Tot datum"
 
-#, fuzzy
 msgctxt "field:marketing.automation.reporting.scenario,block_rate:"
 msgid "Block Rate"
-msgstr "Bloquejat"
+msgstr "Percentage geblokkeerd"
 
 msgctxt "field:marketing.automation.reporting.scenario,date:"
 msgid "Date"
-msgstr ""
+msgstr "Datum"
 
-#, fuzzy
 msgctxt "field:marketing.automation.reporting.scenario,record_count:"
 msgid "Records"
-msgstr "Registres"
+msgstr "Records"
 
-#, fuzzy
 msgctxt "field:marketing.automation.reporting.scenario,record_count_blocked:"
 msgid "Records Blocked"
-msgstr "Registres bloquejats"
+msgstr "Geblokkeerde records"
 
-#, fuzzy
 msgctxt "field:marketing.automation.reporting.scenario,scenario:"
 msgid "Scenario"
-msgstr "Escenari"
+msgstr "Scenario"
 
 msgctxt "field:marketing.automation.scenario,activities:"
 msgid "Activities"
-msgstr "Activitats"
+msgstr "Activiteiten"
 
-#, fuzzy
 msgctxt "field:marketing.automation.scenario,block_rate:"
 msgid "Block Rate"
-msgstr "Bloquejat"
+msgstr "Percentage geblokkeerd"
 
-#, fuzzy
 msgctxt "field:marketing.automation.scenario,block_rate_trend:"
 msgid "Block Rate Trend"
-msgstr "Bloquejat"
+msgstr "Trend percentage geblokkeerd"
 
 msgctxt "field:marketing.automation.scenario,domain:"
 msgid "Domain"
-msgstr "Domini"
+msgstr "Domein (domain)"
 
 msgctxt "field:marketing.automation.scenario,model:"
 msgid "Model"
 msgstr "Model"
 
 msgctxt "field:marketing.automation.scenario,name:"
 msgid "Name"
-msgstr "Nom"
+msgstr "Naam"
 
 msgctxt "field:marketing.automation.scenario,record_count:"
 msgid "Records"
-msgstr "Registres"
+msgstr "Records"
 
 msgctxt "field:marketing.automation.scenario,record_count_blocked:"
 msgid "Records Blocked"
-msgstr "Registres bloquejats"
+msgstr "Geblokkeerde records"
 
 msgctxt "field:marketing.automation.scenario,state:"
 msgid "State"
-msgstr "Estat"
+msgstr "Status"
 
 msgctxt "field:marketing.automation.scenario,unsubscribable:"
 msgid "Unsubscribable"
-msgstr "Donar-se de baixa"
+msgstr "Afmelden mogelijk"
 
 msgctxt "field:party.party,marketing_party:"
 msgid "Marketing Party"
-msgstr "Tercer de màrqueting"
+msgstr "Marketing Relatie"
 
 msgctxt "field:party.party,marketing_scenario_unsubscribed:"
 msgid "Marketing Automation Scenario Unsubscribed"
-msgstr "Escenàris d'automatització de màrqueting no subscrits"
+msgstr "Marketing Abonnement opgezegd"
 
 msgctxt "field:party.party-unsubscribed-marketing.automation.scenario,party:"
 msgid "Party"
-msgstr "Tercer"
+msgstr "Relatie"
 
 msgctxt ""
 "field:party.party-unsubscribed-marketing.automation.scenario,scenario:"
 msgid "Scenario"
-msgstr "Escenari"
+msgstr "Scenario"
 
 msgctxt "field:sale.sale,marketing_party:"
 msgid "Marketing Party"
-msgstr "Tercer de màrqueting"
+msgstr "Marketing Relatie"
 
 msgctxt "help:marketing.automation.activity,condition:"
 msgid ""
 "The PYSON statement that the record must match in order to execute the activity.\n"
 "The record is represented by \"self\"."
 msgstr ""
-"L'expressió PYSON que el registre ha de complir per tal d'executar-se l'activitat.\n"
-"El registre s'expressa amb \"self\"."
+"De PYSON-expressie waaraan het record moet voldoen om de activiteit te kunnen uitvoeren.\n"
+"Het record wordt vertegenwoordigd door \"self\"."
 
 msgctxt "help:marketing.automation.activity,delay:"
 msgid "After how much time the action should be executed."
-msgstr "Desprès de quant temps s'hauria d'executar l'acció."
+msgstr "Na hoeveel tijd moet de actie worden uitgevoerd."
 
 msgctxt "help:marketing.automation.activity,email_from:"
 msgid "Leave empty to use the value defined in the configuration file."
-msgstr "Deixa buit per utilizar el valor definit al fitxer de configuració."
+msgstr ""
+"Laat leeg om de waarde te gebruiken die gedefinieerd is in het "
+"configuratiebestand."
 
 msgctxt "help:marketing.automation.activity,email_template:"
 msgid ""
 "The HTML content of the E-mail.\n"
 "The Genshi syntax can be used with 'record' in the evaluation context."
 msgstr ""
-"El contingut HTML del correu electrònic.\n"
-"La sintaxi Genshi es pot fer servir amb 'record' al context d'avaluació."
+"De HTML-inhoud van de e-mail.\n"
+"De Genshi-syntaxis kan gebruikt worden met 'record' in de evaluatiecontext."
 
 msgctxt "help:marketing.automation.activity,email_title:"
 msgid ""
 "The subject of the email.\n"
 "The Genshi syntax can be used with 'record' in the evaluation context."
 msgstr ""
-"L'assumpte del correu electrònic.\n"
-"La sintaxi Genshi es pot fer servir amb 'record' al context d'avaluació."
+"Het onderwerp van de e-mail.\n"
+"De Genshi-syntaxis kan gebruikt worden met 'record' in de evaluatiecontext."
 
 msgctxt "help:marketing.automation.activity,negative:"
 msgid ""
 "Check to execute the activity if the event has not happened by the end of "
 "the delay."
 msgstr ""
-"Marcar per executar l'activitat si l'esdeveniment no s'ha executat al acabar"
-" el retard."
+"Schakel het selectievakje in om de activiteit uit te voeren als het "
+"evenement niet is gebeurd aan het einde van de vertraging."
 
 msgctxt "help:marketing.automation.scenario,domain:"
 msgid "A PYSON domain used to filter records valid for this scenario."
 msgstr ""
-"Un domini PYSON utilitzat per filtrar registres vàlid per aquest escenari."
+"Een PYSON-domein dat wordt gebruikt om records te filteren die geldig zijn "
+"voor dit scenario."
 
 msgctxt "help:marketing.automation.scenario,unsubscribable:"
 msgid "If checked parties are also unsubscribed from the scenario."
-msgstr "Si es marca els tercer també es de-suscribeixen de l'escenari."
+msgstr ""
+"Indien aangevinkt worden de relaties ook uitgeschreven uit het scenario."
 
 msgctxt "model:ir.action,name:act_activity_tree"
 msgid "Activities"
-msgstr "Activitats"
+msgstr "Activiteiten"
 
 msgctxt "model:ir.action,name:act_ir_email_form_relate_activity"
 msgid "E-mails"
-msgstr "Correus electrònics"
+msgstr "E-mails"
 
 msgctxt "model:ir.action,name:act_record_activity_form"
 msgid "Record Activities"
-msgstr "Activitats del registre"
+msgstr "Activiteiten opnemen"
 
 msgctxt "model:ir.action,name:act_record_form"
 msgid "Records"
-msgstr "Registres"
+msgstr "Records"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_reporting_activity"
 msgid "Activity Reporting"
-msgstr "Acció d'activitat"
+msgstr "Activiteit rapportage"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_reporting_scenario"
 msgid "Scenario Reporting"
-msgstr "Escenari"
+msgstr "Scenario rapportage"
 
 msgctxt "model:ir.action,name:act_scenario_form"
 msgid "Scenarios"
-msgstr "Escenaris"
+msgstr "scenario's"
 
 msgctxt "model:ir.action,name:report_unsubscribe"
 msgid "Marketing Automation Unsubscribe"
-msgstr "Baixa d'automatització de màrqueting"
+msgstr "Marketing Automatizerings Abonnement opzeggen"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_record_activity_form_domain_all"
 msgid "All"
-msgstr "Tot"
+msgstr "Alle"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_record_activity_form_domain_cancelled"
 msgid "Cancelled"
-msgstr "Cancel·lat"
+msgstr "Geannuleerd"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_record_activity_form_domain_done"
 msgid "Done"
-msgstr "Finalitzat"
+msgstr "Klaar"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_record_activity_form_domain_waiting"
 msgid "Waiting"
-msgstr "En espera"
+msgstr "In afwachting"
 
 msgctxt "model:ir.action.act_window.domain,name:act_scenario_form_domain_all"
 msgid "All"
-msgstr "Tot"
+msgstr "Alle"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_scenario_form_domain_draft"
 msgid "Draft"
-msgstr "Esborrany"
+msgstr "Concept"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_scenario_form_domain_running"
 msgid "Running"
-msgstr "En execució"
+msgstr "in uitvoering"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_scenario_form_domain_stopped"
 msgid "Stopped"
-msgstr "Aturat"
+msgstr "gestopt"
 
 msgctxt "model:ir.message,text:msg_activity_invalid_condition"
 msgid ""
 "Invalid condition \"%(condition)s\" in activity \"%(activity)s\" with "
 "exception \"%(exception)s\"."
 msgstr ""
-"Condició no vàlida \"%(condition)s\" a l'activitat \"%(activity)s\" amb "
-"l'excepció \"%(exception)s\"."
+"Ongeldige voorwaarde \"%(condition)s\" in activiteit \"%(activity)s\" met "
+"uitzondering \"%(exception)s\"."
 
 msgctxt "model:ir.message,text:msg_activity_invalid_email_template"
 msgid ""
 "Invalid e-mail template in activity \"%(activity)s\" with exception "
 "\"%(exception)s\"."
 msgstr ""
-"Plantilla de correu electrònic no vàlida a l'activitat \"%(activity)s\" amb "
-"l'excepció \"%(exception)s\"."
+"Ongeldige e-mail template in activiteit \"%(activity)s\" met uitzondering "
+"\"%(exception)s\"."
 
 msgctxt "model:ir.message,text:msg_activity_invalid_email_title"
 msgid ""
 "Invalid e-mail title in activity \"%(activity)s\" with exception "
 "\"%(exception)s\"."
 msgstr ""
-"Ttítol de la plantilla de correu electrònic no vàlida a l'activitat "
-"\"%(activity)s\" amb l'excepció \"%(exception)s\"."
+"Ongeldige e-mail titel in activiteit \"%(activity)s\" met uitzondering "
+"\"%(exception)s\"."
 
 msgctxt "model:ir.message,text:msg_activity_record_unique"
 msgid "Record Activity must be unique by record and activity."
-msgstr "L'activitat del registre ha de ser única per registre i activitat."
+msgstr "Recordactiviteit moet uniek zijn per record en activiteit."
 
 msgctxt "model:ir.message,text:msg_record_scenario_record_unique"
 msgid "Record must be unique by scenario."
-msgstr "El registre ha de ser únic per cada escenari."
+msgstr "Record moet uniek zijn per scenario."
 
 msgctxt "model:ir.message,text:msg_record_uuid_unique"
 msgid "UUID of record must be unique."
-msgstr "L'UUID del registre ha de ser únic."
+msgstr "UUID van het record moet uniek zijn."
 
 msgctxt "model:ir.message,text:msg_scenario_invalid_domain"
 msgid "Invalid domain in scenario \"%(scenario)s\" with exception \"%(exception)s\"."
 msgstr ""
-"Domini no vàlid a l'escenari \"%(scenario)s\" amb l'excepció "
+"Ongeldig domein in scenario \"%(scenario)s\" met uitzondering "
 "\"%(exception)s\"."
 
 msgctxt "model:ir.model.button,string:record_activity_on_email_clicked_button"
 msgid "E-Mail Clicked"
-msgstr "Correu electrònic clicat"
+msgstr "E-mail Geklikt"
 
 msgctxt "model:ir.model.button,string:record_activity_on_email_opened_button"
 msgid "E-Mail Opened"
-msgstr "Correu electrònic obert"
+msgstr "E-mails geopend"
 
 msgctxt "model:ir.model.button,string:record_block_button"
 msgid "Block"
-msgstr "Bloqueja"
+msgstr "Blokkeer"
 
 msgctxt "model:ir.model.button,string:scenario_draft_button"
 msgid "Draft"
-msgstr "Esborrany"
+msgstr "Concept"
 
 msgctxt "model:ir.model.button,string:scenario_run_button"
 msgid "Run"
-msgstr "Executa"
+msgstr "uitvoeren"
 
 msgctxt "model:ir.model.button,string:scenario_stop_button"
 msgid "Stop"
-msgstr "Atura"
+msgstr "stop"
 
 msgctxt "model:ir.ui.menu,name:menu_scenario_form"
 msgid "Scenarios"
-msgstr "Escenaris"
+msgstr "scenario's"
 
 msgctxt "model:marketing.automation.activity,name:"
 msgid "Marketing Activity"
-msgstr "Activitat de màrqueting"
+msgstr "Marketing activiteit"
 
 msgctxt "model:marketing.automation.record,name:"
 msgid "Marketing Record"
-msgstr "Registre de màrqueting"
+msgstr "Marketingrecord"
 
 msgctxt "model:marketing.automation.record.activity,name:"
 msgid "Marketing Record Activity"
-msgstr "Activitat del registre de màrqueting"
+msgstr "Marketingrecordactiviteit"
 
-#, fuzzy
 msgctxt "model:marketing.automation.reporting.activity,name:"
 msgid "Marketing Automation Reporting Activity"
-msgstr "Activitat del registre de màrqueting"
+msgstr "Activiteit rapportage voor marketingautomatisering"
 
-#, fuzzy
 msgctxt "model:marketing.automation.reporting.context,name:"
 msgid "Marketing Automation Reporting Context"
-msgstr "Automatització de màrqueting"
+msgstr "Rapportage context voor marketingautomatisering"
 
-#, fuzzy
 msgctxt "model:marketing.automation.reporting.scenario,name:"
 msgid "Marketing Automation Reporting Scenario"
-msgstr "Escenàris d'automatització de màrqueting no subscrits"
+msgstr "Scenario rapportage voor marketingautomatisering"
 
 msgctxt "model:marketing.automation.scenario,name:"
 msgid "Marketing Scenario"
-msgstr "Escenari de màrqueting"
+msgstr "Marketingscenario"
 
 msgctxt "model:party.party-unsubscribed-marketing.automation.scenario,name:"
 msgid "Party Unsubscribed Scenario"
-msgstr "Escenaris de-suscrits del tercer"
+msgstr "Relatie Uitschrijf Scenario"
 
 msgctxt "report:marketing.automation.unsubscribe:"
 msgid "Unsubscribe"
-msgstr "Donar-se de baixa"
+msgstr "Afmelden"
 
 msgctxt "report:marketing.automation.unsubscribe:"
 msgid ""
 "We are sorry to see you go, and apologize if we have overwhelmed your inbox."
 msgstr ""
-"Sentim veure't marxar, i ens disculpem si hem aclaparat la teva safata "
-"d'entrada."
+"Het spijt ons u te zien gaan. Onze excuses als we uw inbox vervuild hebben ."
 
 msgctxt "report:marketing.automation.unsubscribe:"
 msgid "You are unsubscribed"
-msgstr "T'has donat de baixa"
+msgstr "U bent uitgeschreven"
 
 msgctxt "report:marketing.automation.unsubscribe:"
 msgid "You have been successfully unsubscribed from this kind of email."
-msgstr "T'has donat de baixa amb èxit d'aquest tipus de correu electrònic."
+msgstr "U bent succesvol afgemeld voor dit soort e-mail."
 
 msgctxt "selection:ir.cron,method:"
 msgid "Process Marketing Activity"
-msgstr "Processar activitats de màrqueting"
+msgstr "Marketingactiviteit verwerken"
 
 msgctxt "selection:ir.cron,method:"
 msgid "Trigger Marketing Scenarios"
-msgstr "Executar disparadors del escenaris de màrqueting"
+msgstr "Trigger Marketing Scenario's"
 
 msgctxt "selection:marketing.automation.activity,action:"
 msgid "Send E-Mail"
-msgstr "Correu electrònic enviat"
+msgstr "E-mail verzenden"
 
 msgctxt "selection:marketing.automation.activity,event:"
 msgid "E-Mail Clicked"
-msgstr "Correu electrònic clicat"
+msgstr "E-mail Geklikt"
 
 msgctxt "selection:marketing.automation.activity,event:"
 msgid "E-Mail Opened"
-msgstr "Correu electrònic obert"
+msgstr "E-mails geopend"
 
 msgctxt "selection:marketing.automation.activity,on:"
 msgid "E-Mail Clicked"
-msgstr "Correu electrònic clicat"
+msgstr "E-mail Geklikt"
 
 msgctxt "selection:marketing.automation.activity,on:"
 msgid "E-Mail Not Clicked"
-msgstr "Correu electrònic no clicat"
+msgstr "E-mail niet aangeklikt"
 
 msgctxt "selection:marketing.automation.activity,on:"
 msgid "E-Mail Not Opened"
-msgstr "Correu electrònic no obert"
+msgstr "E-mail niet geopend"
 
 msgctxt "selection:marketing.automation.activity,on:"
 msgid "E-Mail Opened"
-msgstr "Correu electrònic obert"
+msgstr "E-mails geopend"
 
 msgctxt "selection:marketing.automation.activity,parent:"
 msgid "Activity"
-msgstr "Activitat"
+msgstr "Activiteit"
 
 msgctxt "selection:marketing.automation.activity,parent:"
 msgid "Scenario"
-msgstr "Escenari"
+msgstr "Scenario"
 
 msgctxt "selection:marketing.automation.record.activity,state:"
 msgid "Cancelled"
-msgstr "Cancel·lada"
+msgstr "Geannuleerd"
 
 msgctxt "selection:marketing.automation.record.activity,state:"
 msgid "Done"
-msgstr "Finalitzada"
+msgstr "Klaar"
 
 msgctxt "selection:marketing.automation.record.activity,state:"
 msgid "Waiting"
-msgstr "En espera"
+msgstr "In afwachting"
 
-#, fuzzy
 msgctxt "selection:marketing.automation.reporting.context,period:"
 msgid "Day"
-msgstr "Retard"
+msgstr "Dag"
 
 msgctxt "selection:marketing.automation.reporting.context,period:"
 msgid "Month"
-msgstr ""
+msgstr "Maand"
 
 msgctxt "selection:marketing.automation.reporting.context,period:"
 msgid "Year"
-msgstr ""
+msgstr "Jaar"
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Draft"
-msgstr "Esborrany"
+msgstr "Concept"
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Running"
-msgstr "En execució"
+msgstr "in uitvoering"
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Stopped"
-msgstr "Aturat"
+msgstr "gestopt"
 
 msgctxt "view:marketing.automation.activity:"
 msgid "%"
-msgstr ""
+msgstr "%"
 
 msgctxt "view:marketing.automation.activity:"
 msgid "After"
-msgstr "Desprès"
+msgstr "Na"
 
 msgctxt "view:marketing.automation.activity:"
 msgid "Edit"
-msgstr "Edita"
+msgstr "Bewerk"
 
 msgctxt "view:marketing.automation.activity:"
 msgid "If"
-msgstr "Si"
+msgstr "Als"
 
 msgctxt "view:marketing.automation.activity:"
 msgid "On"
-msgstr "A"
+msgstr "Op"
 
 msgctxt "view:marketing.automation.activity:"
 msgid "Template:"
-msgstr "Plantilla:"
+msgstr "Sjabloon:"
 
 msgctxt "view:marketing.automation.activity:"
 msgid "Title:"
-msgstr "Títol:"
+msgstr "Titel:"
 
 msgctxt "view:marketing.automation.record.activity:"
 msgid "Time"
-msgstr "Hora"
+msgstr "Tijd"
 
 msgctxt "view:marketing.automation.reporting.activity:"
 msgid "%"
-msgstr ""
+msgstr "%"
 
 msgctxt "view:marketing.automation.reporting.scenario:"
 msgid "%"
-msgstr ""
+msgstr "%"
 
 msgctxt "view:marketing.automation.scenario:"
 msgid "%"
-msgstr ""
+msgstr "%"
 
 msgctxt "view:party.party:"
 msgid "Marketing Automation"
-msgstr "Automatització de màrqueting"
+msgstr "Marketing Abonnement Opzeggen"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_marketing_automation-7.2.0/locale/cs.po` & `trytond_marketing_automation-7.2.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-7.2.0/locale/de.po` & `trytond_marketing_automation-7.2.1/locale/de.po`

 * *Files 3% similar despite different names*

```diff
@@ -22,50 +22,45 @@
 msgid "Condition"
 msgstr "Bedingung"
 
 msgctxt "field:marketing.automation.activity,delay:"
 msgid "Delay"
 msgstr "Verzögerung"
 
-#, fuzzy
 msgctxt "field:marketing.automation.activity,email_click_rate:"
 msgid "E-mail Click Rate"
-msgstr "Angeklickte E-Mail"
+msgstr "Klickrate (CR)"
 
-#, fuzzy
 msgctxt "field:marketing.automation.activity,email_click_rate_trend:"
 msgid "E-mail Click Rate Trend"
-msgstr "Angeklickte E-Mail"
+msgstr "Klickrate Trend"
 
-#, fuzzy
 msgctxt "field:marketing.automation.activity,email_click_through_rate:"
 msgid "E-mail Click-Through Rate"
-msgstr "Angeklickte E-Mail"
+msgstr "Durchklickrate (CTR)"
 
 msgctxt "field:marketing.automation.activity,email_click_through_rate_trend:"
 msgid "E-mail Click-Through Rate Trend"
-msgstr ""
+msgstr "Durchklickrate Trend"
 
 msgctxt "field:marketing.automation.activity,email_clicked:"
 msgid "E-Mails Clicked"
 msgstr "Angeklickte E-Mails"
 
 msgctxt "field:marketing.automation.activity,email_from:"
 msgid "From"
 msgstr "Von"
 
-#, fuzzy
 msgctxt "field:marketing.automation.activity,email_open_rate:"
 msgid "E-mail Open Rate"
-msgstr "Geöffnete E-Mail"
+msgstr "Öffnungsrate"
 
-#, fuzzy
 msgctxt "field:marketing.automation.activity,email_open_rate_trend:"
 msgid "E-mail Open Rate Trend"
-msgstr "Geöffnete E-Mail"
+msgstr "Öffnungsrate Trend"
 
 msgctxt "field:marketing.automation.activity,email_opened:"
 msgid "E-Mails Opened"
 msgstr "Geöffnete E-Mails"
 
 msgctxt "field:marketing.automation.activity,email_template:"
 msgid "E-Mail Template"
@@ -121,131 +116,116 @@
 
 msgctxt "field:marketing.automation.record.activity,activity:"
 msgid "Activity"
 msgstr "Aktivität"
 
 msgctxt "field:marketing.automation.record.activity,activity_action:"
 msgid "Activity Action"
-msgstr "Aktivität Aktion"
+msgstr "Aktion der Aktivität"
 
 msgctxt "field:marketing.automation.record.activity,at:"
 msgid "At"
 msgstr "Um"
 
 msgctxt "field:marketing.automation.record.activity,email_clicked:"
 msgid "E-Mail Clicked"
-msgstr "Angeklickte E-Mail"
+msgstr "E-Mail angeklickt"
 
 msgctxt "field:marketing.automation.record.activity,email_opened:"
 msgid "E-Mail Opened"
-msgstr "Geöffnete E-Mail"
+msgstr "E-Mail geöffnet"
 
 msgctxt "field:marketing.automation.record.activity,record:"
 msgid "Record"
 msgstr "Datensatz"
 
 msgctxt "field:marketing.automation.record.activity,state:"
 msgid "State"
 msgstr "Status"
 
-#, fuzzy
 msgctxt "field:marketing.automation.reporting.activity,activity:"
 msgid "Activity"
 msgstr "Aktivität"
 
-#, fuzzy
 msgctxt "field:marketing.automation.reporting.activity,activity_action:"
 msgid "Activity Action"
-msgstr "Aktivität Aktion"
+msgstr "Aktion der Aktivität"
 
 msgctxt "field:marketing.automation.reporting.activity,date:"
 msgid "Date"
-msgstr ""
+msgstr "Datum"
 
-#, fuzzy
 msgctxt "field:marketing.automation.reporting.activity,email_click_rate:"
 msgid "E-mail Click Rate"
-msgstr "Angeklickte E-Mail"
+msgstr "Klickrate (CR)"
 
-#, fuzzy
 msgctxt ""
 "field:marketing.automation.reporting.activity,email_click_through_rate:"
 msgid "E-mail Click-Through Rate"
-msgstr "Angeklickte E-Mail"
+msgstr "Durchklickrate (CTR)"
 
-#, fuzzy
 msgctxt "field:marketing.automation.reporting.activity,email_clicked:"
 msgid "E-Mails Clicked"
-msgstr "Angeklickte E-Mails"
+msgstr "Angeklickt"
 
-#, fuzzy
 msgctxt "field:marketing.automation.reporting.activity,email_open_rate:"
 msgid "E-mail Open Rate"
-msgstr "Geöffnete E-Mail"
+msgstr "Öffnungsrate"
 
-#, fuzzy
 msgctxt "field:marketing.automation.reporting.activity,email_opened:"
 msgid "E-Mails Opened"
-msgstr "Geöffnete E-Mails"
+msgstr "Geöffnet"
 
-#, fuzzy
 msgctxt "field:marketing.automation.reporting.activity,record_count:"
 msgid "Records"
 msgstr "Datensätze"
 
-#, fuzzy
 msgctxt "field:marketing.automation.reporting.context,from_date:"
 msgid "From Date"
-msgstr "Zuletzt geändert"
+msgstr "Von Datum"
 
 msgctxt "field:marketing.automation.reporting.context,period:"
 msgid "Period"
-msgstr ""
+msgstr "Zeitraum"
 
 msgctxt "field:marketing.automation.reporting.context,to_date:"
 msgid "To Date"
-msgstr ""
+msgstr "Bis Datum"
 
-#, fuzzy
 msgctxt "field:marketing.automation.reporting.scenario,block_rate:"
 msgid "Block Rate"
-msgstr "Gesperrt"
+msgstr "Blockrate"
 
 msgctxt "field:marketing.automation.reporting.scenario,date:"
 msgid "Date"
-msgstr ""
+msgstr "Datum"
 
-#, fuzzy
 msgctxt "field:marketing.automation.reporting.scenario,record_count:"
 msgid "Records"
 msgstr "Datensätze"
 
-#, fuzzy
 msgctxt "field:marketing.automation.reporting.scenario,record_count_blocked:"
 msgid "Records Blocked"
 msgstr "Blockierte Datensätze"
 
-#, fuzzy
 msgctxt "field:marketing.automation.reporting.scenario,scenario:"
 msgid "Scenario"
 msgstr "Szenario"
 
 msgctxt "field:marketing.automation.scenario,activities:"
 msgid "Activities"
 msgstr "Aktivitäten"
 
-#, fuzzy
 msgctxt "field:marketing.automation.scenario,block_rate:"
 msgid "Block Rate"
-msgstr "Gesperrt"
+msgstr "Blockrate"
 
-#, fuzzy
 msgctxt "field:marketing.automation.scenario,block_rate_trend:"
 msgid "Block Rate Trend"
-msgstr "Gesperrt"
+msgstr "Blockrate Trend"
 
 msgctxt "field:marketing.automation.scenario,domain:"
 msgid "Domain"
 msgstr "Wertebereich (Domain)"
 
 msgctxt "field:marketing.automation.scenario,model:"
 msgid "Model"
@@ -265,15 +245,15 @@
 
 msgctxt "field:marketing.automation.scenario,state:"
 msgid "State"
 msgstr "Status"
 
 msgctxt "field:marketing.automation.scenario,unsubscribable:"
 msgid "Unsubscribable"
-msgstr "Abmeldbar"
+msgstr "Abmeldung möglich"
 
 msgctxt "field:party.party,marketing_party:"
 msgid "Marketing Party"
 msgstr "Marketing Partei"
 
 msgctxt "field:party.party,marketing_scenario_unsubscribed:"
 msgid "Marketing Automation Scenario Unsubscribed"
@@ -298,15 +278,15 @@
 "The record is represented by \"self\"."
 msgstr ""
 "Der PYSON Ausdruck, dem der Datensatz entsprechen muss, damit die Aktivität ausgeführt wird.\n"
 "Der Datensatz wird durch \"self\" repräsentiert."
 
 msgctxt "help:marketing.automation.activity,delay:"
 msgid "After how much time the action should be executed."
-msgstr "Nach welcher Zeit die Aktion ausgeführt werden soll."
+msgstr "Dauer, nach der die Aktion ausgeführt werden soll."
 
 msgctxt "help:marketing.automation.activity,email_from:"
 msgid "Leave empty to use the value defined in the configuration file."
 msgstr "Leer lassen, um den Wert aus der Konfigurationsdatei zu verwenden."
 
 msgctxt "help:marketing.automation.activity,email_template:"
 msgid ""
@@ -326,15 +306,15 @@
 
 msgctxt "help:marketing.automation.activity,negative:"
 msgid ""
 "Check to execute the activity if the event has not happened by the end of "
 "the delay."
 msgstr ""
 "Aktivieren um die Aktivität auszulösen, wenn das Ereignis nach Ablauf des "
-"Verzögerungszeitraums noch nicht eingetreten ist."
+"Zeitintervalls noch nicht eingetreten ist."
 
 msgctxt "help:marketing.automation.scenario,domain:"
 msgid "A PYSON domain used to filter records valid for this scenario."
 msgstr ""
 "Ein PYSON Wertebereich (Domain) zum Filtern der Datensätze, die diesem "
 "Szenario entsprechen."
 
@@ -354,23 +334,21 @@
 msgid "Record Activities"
 msgstr "Datensatzaktivitäten"
 
 msgctxt "model:ir.action,name:act_record_form"
 msgid "Records"
 msgstr "Datensätze"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_reporting_activity"
 msgid "Activity Reporting"
-msgstr "Aktivität Aktion"
+msgstr "Aktivitätsauswertung"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_reporting_scenario"
 msgid "Scenario Reporting"
-msgstr "Szenario"
+msgstr "Szenarioauswertung"
 
 msgctxt "model:ir.action,name:act_scenario_form"
 msgid "Scenarios"
 msgstr "Szenarien"
 
 msgctxt "model:ir.action,name:report_unsubscribe"
 msgid "Marketing Automation Unsubscribe"
@@ -442,15 +420,15 @@
 msgctxt "model:ir.message,text:msg_activity_record_unique"
 msgid "Record Activity must be unique by record and activity."
 msgstr ""
 "Eine Datensatzaktivität kann es je Datensatz und Aktivität nur einmal geben."
 
 msgctxt "model:ir.message,text:msg_record_scenario_record_unique"
 msgid "Record must be unique by scenario."
-msgstr "Es kann je Szenario nur einen Datensatz geben."
+msgstr "Datensätze müssen je Szenario eindeutig sein."
 
 msgctxt "model:ir.message,text:msg_record_uuid_unique"
 msgid "UUID of record must be unique."
 msgstr "Die UUID des Datensatzes existiert bereits."
 
 msgctxt "model:ir.message,text:msg_scenario_invalid_domain"
 msgid "Invalid domain in scenario \"%(scenario)s\" with exception \"%(exception)s\"."
@@ -464,27 +442,27 @@
 
 msgctxt "model:ir.model.button,string:record_activity_on_email_opened_button"
 msgid "E-Mail Opened"
 msgstr "E-Mail geöffnet"
 
 msgctxt "model:ir.model.button,string:record_block_button"
 msgid "Block"
-msgstr "Gesperrt"
+msgstr "Sperren"
 
 msgctxt "model:ir.model.button,string:scenario_draft_button"
 msgid "Draft"
 msgstr "Entwurf"
 
 msgctxt "model:ir.model.button,string:scenario_run_button"
 msgid "Run"
 msgstr "Ausführen"
 
 msgctxt "model:ir.model.button,string:scenario_stop_button"
 msgid "Stop"
-msgstr "Stopp"
+msgstr "Stoppen"
 
 msgctxt "model:ir.ui.menu,name:menu_scenario_form"
 msgid "Scenarios"
 msgstr "Szenarien"
 
 msgctxt "model:marketing.automation.activity,name:"
 msgid "Marketing Activity"
@@ -494,36 +472,33 @@
 msgid "Marketing Record"
 msgstr "Marketingdatensatz"
 
 msgctxt "model:marketing.automation.record.activity,name:"
 msgid "Marketing Record Activity"
 msgstr "Marketing Datensatzaktivität"
 
-#, fuzzy
 msgctxt "model:marketing.automation.reporting.activity,name:"
 msgid "Marketing Automation Reporting Activity"
-msgstr "Marketing Datensatzaktivität"
+msgstr "Marketing Automatisierung Auswertung Aktivität"
 
-#, fuzzy
 msgctxt "model:marketing.automation.reporting.context,name:"
 msgid "Marketing Automation Reporting Context"
-msgstr "Marketingautomatisierung"
+msgstr "Marketing Automatisierung Auswertung Kontext"
 
-#, fuzzy
 msgctxt "model:marketing.automation.reporting.scenario,name:"
 msgid "Marketing Automation Reporting Scenario"
-msgstr "Marketingautomatisierungsszenario abgemeldet"
+msgstr "Marketing Automatisierung Auswertung Szenario"
 
 msgctxt "model:marketing.automation.scenario,name:"
 msgid "Marketing Scenario"
 msgstr "Marketing Szenario"
 
 msgctxt "model:party.party-unsubscribed-marketing.automation.scenario,name:"
 msgid "Party Unsubscribed Scenario"
-msgstr "Partei Abmelden Szenario"
+msgstr "Partei Abgemeldet Szenario"
 
 msgctxt "report:marketing.automation.unsubscribe:"
 msgid "Unsubscribe"
 msgstr "Abmelden"
 
 msgctxt "report:marketing.automation.unsubscribe:"
 msgid ""
@@ -592,26 +567,25 @@
 msgid "Done"
 msgstr "Erledigt"
 
 msgctxt "selection:marketing.automation.record.activity,state:"
 msgid "Waiting"
 msgstr "Wartend"
 
-#, fuzzy
 msgctxt "selection:marketing.automation.reporting.context,period:"
 msgid "Day"
-msgstr "Verzögerung"
+msgstr "Tag"
 
 msgctxt "selection:marketing.automation.reporting.context,period:"
 msgid "Month"
-msgstr ""
+msgstr "Monat"
 
 msgctxt "selection:marketing.automation.reporting.context,period:"
 msgid "Year"
-msgstr ""
+msgstr "Jahr"
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Draft"
 msgstr "Entwurf"
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Running"
@@ -619,15 +593,15 @@
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Stopped"
 msgstr "Gestoppt"
 
 msgctxt "view:marketing.automation.activity:"
 msgid "%"
-msgstr ""
+msgstr "%"
 
 msgctxt "view:marketing.automation.activity:"
 msgid "After"
 msgstr "Nach"
 
 msgctxt "view:marketing.automation.activity:"
 msgid "Edit"
@@ -651,20 +625,20 @@
 
 msgctxt "view:marketing.automation.record.activity:"
 msgid "Time"
 msgstr "Zeit"
 
 msgctxt "view:marketing.automation.reporting.activity:"
 msgid "%"
-msgstr ""
+msgstr "%"
 
 msgctxt "view:marketing.automation.reporting.scenario:"
 msgid "%"
-msgstr ""
+msgstr "%"
 
 msgctxt "view:marketing.automation.scenario:"
 msgid "%"
-msgstr ""
+msgstr "%"
 
 msgctxt "view:party.party:"
 msgid "Marketing Automation"
 msgstr "Marketingautomatisierung"
```

### Comparing `trytond_marketing_automation-7.2.0/locale/es.po` & `trytond_marketing_automation-7.2.1/locale/sl.po`

 * *Files 8% similar despite different names*

```diff
@@ -1,661 +1,658 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:ir.email,marketing_automation_activity:"
 msgid "Activity"
-msgstr "Actividad"
+msgstr "Aktivnost"
 
 msgctxt "field:ir.email,marketing_automation_record:"
 msgid "Record"
-msgstr "Registro"
+msgstr "Zapis"
 
 msgctxt "field:marketing.automation.activity,action:"
 msgid "Action"
-msgstr "Acción"
+msgstr "Ukrep"
 
 msgctxt "field:marketing.automation.activity,children:"
 msgid "Children"
-msgstr "Hijos"
+msgstr "Podukrepi"
 
 msgctxt "field:marketing.automation.activity,condition:"
 msgid "Condition"
-msgstr "Condición"
+msgstr "Pogoj"
 
 msgctxt "field:marketing.automation.activity,delay:"
 msgid "Delay"
-msgstr "Retraso"
+msgstr "Zakasnitev"
 
 #, fuzzy
 msgctxt "field:marketing.automation.activity,email_click_rate:"
 msgid "E-mail Click Rate"
-msgstr "Correo electrónico pulsado"
+msgstr "E-poštni kliki"
 
 #, fuzzy
 msgctxt "field:marketing.automation.activity,email_click_rate_trend:"
 msgid "E-mail Click Rate Trend"
-msgstr "Correo electrónico pulsado"
+msgstr "E-poštni kliki"
 
 #, fuzzy
 msgctxt "field:marketing.automation.activity,email_click_through_rate:"
 msgid "E-mail Click-Through Rate"
-msgstr "Correo electrónico pulsado"
+msgstr "E-poštni kliki"
 
 msgctxt "field:marketing.automation.activity,email_click_through_rate_trend:"
 msgid "E-mail Click-Through Rate Trend"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,email_clicked:"
 msgid "E-Mails Clicked"
-msgstr "Correos electrónicos pulsados"
+msgstr "E-poštni kliki"
 
 msgctxt "field:marketing.automation.activity,email_from:"
 msgid "From"
-msgstr "De"
+msgstr "Od"
 
 #, fuzzy
 msgctxt "field:marketing.automation.activity,email_open_rate:"
 msgid "E-mail Open Rate"
-msgstr "Correo electrónico abierto"
+msgstr "E-pošta odprta"
 
 #, fuzzy
 msgctxt "field:marketing.automation.activity,email_open_rate_trend:"
 msgid "E-mail Open Rate Trend"
-msgstr "Correo electrónico abierto"
+msgstr "E-pošta odprta"
 
 msgctxt "field:marketing.automation.activity,email_opened:"
 msgid "E-Mails Opened"
-msgstr "Correos electrónicos abiertos"
+msgstr "E-pošta odprta"
 
 msgctxt "field:marketing.automation.activity,email_template:"
 msgid "E-Mail Template"
-msgstr "Plantilla de correo electrónico"
+msgstr "E-poštna predloga"
 
 msgctxt "field:marketing.automation.activity,email_title:"
 msgid "E-Mail Title"
-msgstr "Titulo del correo electrónico"
+msgstr "E-poštna zadeva"
 
 msgctxt "field:marketing.automation.activity,event:"
 msgid "Event"
-msgstr "Evento"
+msgstr "Dogodek"
 
 msgctxt "field:marketing.automation.activity,name:"
 msgid "Name"
-msgstr "Nombre"
+msgstr "Naziv"
 
 msgctxt "field:marketing.automation.activity,negative:"
 msgid "Negative"
-msgstr "Negativo"
+msgstr "Negativno"
 
 msgctxt "field:marketing.automation.activity,on:"
 msgid "On"
-msgstr "A"
+msgstr "Na"
 
 msgctxt "field:marketing.automation.activity,parent:"
 msgid "Parent"
-msgstr "Padre"
+msgstr "Matični ukrep"
 
 msgctxt "field:marketing.automation.activity,parent_action:"
 msgid "Parent Action"
-msgstr "Acción padre"
+msgstr "Matični ukrep"
 
 msgctxt "field:marketing.automation.activity,record_count:"
 msgid "Records"
-msgstr "Registros"
+msgstr "Zapisi"
 
 msgctxt "field:marketing.automation.record,blocked:"
 msgid "Blocked"
-msgstr "Bloqueado"
+msgstr "Blokiran"
 
 msgctxt "field:marketing.automation.record,record:"
 msgid "Record"
-msgstr "Registro"
+msgstr "Zapis"
 
 msgctxt "field:marketing.automation.record,scenario:"
 msgid "Scenario"
-msgstr "Escenario"
+msgstr "Scenarij"
 
 msgctxt "field:marketing.automation.record,uuid:"
 msgid "UUID"
-msgstr "Identificador único universal"
+msgstr "UUID"
 
 msgctxt "field:marketing.automation.record.activity,activity:"
 msgid "Activity"
-msgstr "Actividad"
+msgstr "Aktivnost"
 
 msgctxt "field:marketing.automation.record.activity,activity_action:"
 msgid "Activity Action"
-msgstr "Acción de actividad"
+msgstr "Ukrep aktivnosti"
 
 msgctxt "field:marketing.automation.record.activity,at:"
 msgid "At"
-msgstr "A"
+msgstr "Ob"
 
 msgctxt "field:marketing.automation.record.activity,email_clicked:"
 msgid "E-Mail Clicked"
-msgstr "Correo electrónico pulsado"
+msgstr "E-poštni kliki"
 
 msgctxt "field:marketing.automation.record.activity,email_opened:"
 msgid "E-Mail Opened"
-msgstr "Correo electrónico abierto"
+msgstr "E-pošta odprta"
 
 msgctxt "field:marketing.automation.record.activity,record:"
 msgid "Record"
-msgstr "Registro"
+msgstr "Zapis"
 
 msgctxt "field:marketing.automation.record.activity,state:"
 msgid "State"
-msgstr "Estado"
+msgstr "Stanje"
 
 #, fuzzy
 msgctxt "field:marketing.automation.reporting.activity,activity:"
 msgid "Activity"
-msgstr "Actividad"
+msgstr "Aktivnost"
 
 #, fuzzy
 msgctxt "field:marketing.automation.reporting.activity,activity_action:"
 msgid "Activity Action"
-msgstr "Acción de actividad"
+msgstr "Ukrep aktivnosti"
 
 msgctxt "field:marketing.automation.reporting.activity,date:"
 msgid "Date"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:marketing.automation.reporting.activity,email_click_rate:"
 msgid "E-mail Click Rate"
-msgstr "Correo electrónico pulsado"
+msgstr "E-poštni kliki"
 
 #, fuzzy
 msgctxt ""
 "field:marketing.automation.reporting.activity,email_click_through_rate:"
 msgid "E-mail Click-Through Rate"
-msgstr "Correo electrónico pulsado"
+msgstr "E-poštni kliki"
 
 #, fuzzy
 msgctxt "field:marketing.automation.reporting.activity,email_clicked:"
 msgid "E-Mails Clicked"
-msgstr "Correos electrónicos pulsados"
+msgstr "E-poštni kliki"
 
 #, fuzzy
 msgctxt "field:marketing.automation.reporting.activity,email_open_rate:"
 msgid "E-mail Open Rate"
-msgstr "Correo electrónico abierto"
+msgstr "E-pošta odprta"
 
 #, fuzzy
 msgctxt "field:marketing.automation.reporting.activity,email_opened:"
 msgid "E-Mails Opened"
-msgstr "Correos electrónicos abiertos"
+msgstr "E-pošta odprta"
 
 #, fuzzy
 msgctxt "field:marketing.automation.reporting.activity,record_count:"
 msgid "Records"
-msgstr "Registros"
+msgstr "Zapisi"
 
 #, fuzzy
 msgctxt "field:marketing.automation.reporting.context,from_date:"
 msgid "From Date"
-msgstr "Fecha de modificación"
+msgstr "Od"
 
 msgctxt "field:marketing.automation.reporting.context,period:"
 msgid "Period"
 msgstr ""
 
 msgctxt "field:marketing.automation.reporting.context,to_date:"
 msgid "To Date"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:marketing.automation.reporting.scenario,block_rate:"
 msgid "Block Rate"
-msgstr "Bloqueado"
+msgstr "Blokiran"
 
 msgctxt "field:marketing.automation.reporting.scenario,date:"
 msgid "Date"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:marketing.automation.reporting.scenario,record_count:"
 msgid "Records"
-msgstr "Registros"
+msgstr "Zapisi"
 
 #, fuzzy
 msgctxt "field:marketing.automation.reporting.scenario,record_count_blocked:"
 msgid "Records Blocked"
-msgstr "Registros bloqueados"
+msgstr "Blokirani zapisi"
 
 #, fuzzy
 msgctxt "field:marketing.automation.reporting.scenario,scenario:"
 msgid "Scenario"
-msgstr "Escenario"
+msgstr "Scenarij"
 
 msgctxt "field:marketing.automation.scenario,activities:"
 msgid "Activities"
-msgstr "Actividades"
+msgstr "Aktivnosti"
 
 #, fuzzy
 msgctxt "field:marketing.automation.scenario,block_rate:"
 msgid "Block Rate"
-msgstr "Bloqueado"
+msgstr "Blokiran"
 
 #, fuzzy
 msgctxt "field:marketing.automation.scenario,block_rate_trend:"
 msgid "Block Rate Trend"
-msgstr "Bloqueado"
+msgstr "Blokiran"
 
 msgctxt "field:marketing.automation.scenario,domain:"
 msgid "Domain"
-msgstr "Dominio"
+msgstr "Domena"
 
 msgctxt "field:marketing.automation.scenario,model:"
 msgid "Model"
-msgstr "Modelo"
+msgstr "Model"
 
 msgctxt "field:marketing.automation.scenario,name:"
 msgid "Name"
-msgstr "Nombre"
+msgstr "Naziv"
 
 msgctxt "field:marketing.automation.scenario,record_count:"
 msgid "Records"
-msgstr "Registros"
+msgstr "Zapisi"
 
 msgctxt "field:marketing.automation.scenario,record_count_blocked:"
 msgid "Records Blocked"
-msgstr "Registros bloqueados"
+msgstr "Blokirani zapisi"
 
 msgctxt "field:marketing.automation.scenario,state:"
 msgid "State"
-msgstr "Estado"
+msgstr "Stanje"
 
 msgctxt "field:marketing.automation.scenario,unsubscribable:"
 msgid "Unsubscribable"
-msgstr "Darse de baja"
+msgstr "Odjava"
 
 msgctxt "field:party.party,marketing_party:"
 msgid "Marketing Party"
-msgstr "Tercero del marketing"
+msgstr "Marketing Partner"
 
 msgctxt "field:party.party,marketing_scenario_unsubscribed:"
 msgid "Marketing Automation Scenario Unsubscribed"
-msgstr "Escenarios de automatización de marketing no suscritos"
+msgstr ""
 
 msgctxt "field:party.party-unsubscribed-marketing.automation.scenario,party:"
 msgid "Party"
-msgstr "Tercero"
+msgstr "Partner"
 
 msgctxt ""
 "field:party.party-unsubscribed-marketing.automation.scenario,scenario:"
 msgid "Scenario"
-msgstr "Escenario"
+msgstr "Scenarij"
 
 msgctxt "field:sale.sale,marketing_party:"
 msgid "Marketing Party"
-msgstr "Tercero del marketing"
+msgstr "Marketing partner"
 
 msgctxt "help:marketing.automation.activity,condition:"
 msgid ""
 "The PYSON statement that the record must match in order to execute the activity.\n"
 "The record is represented by \"self\"."
 msgstr ""
-"La condicion PYSON que debe satisfacer el registro para ejecutar la actividad.\n"
-"El registro es representado por \"self\"."
+"Izraz PYSON, s katerim se mora zapis ujemati, da se aktivnost izvaja.\n"
+"Zapis je predstavljen s \"self\"."
 
 msgctxt "help:marketing.automation.activity,delay:"
 msgid "After how much time the action should be executed."
-msgstr "Después de cuánto tiempo debe ser ejecutada la acción."
+msgstr "Po koliko časa naj bo ukrep izveden."
 
 msgctxt "help:marketing.automation.activity,email_from:"
 msgid "Leave empty to use the value defined in the configuration file."
 msgstr ""
-"Dejar vacío para usar el valor definido en el archivo de configuración."
+"Pustite prazno, da uporabite vrednost opredeljeno v konfiguracijski "
+"datoteki."
 
 msgctxt "help:marketing.automation.activity,email_template:"
 msgid ""
 "The HTML content of the E-mail.\n"
 "The Genshi syntax can be used with 'record' in the evaluation context."
 msgstr ""
-"El contenido HTML del correo electrónico.\n"
-"La sintaxis Genshi puede ser utilizada con 'record' en el contexto de evaluación."
+"HTML vsebina e-pošte.\n"
+"Lahko uporabite Genshi sintakso z 'record' v kontekstu vrednotenja."
 
 msgctxt "help:marketing.automation.activity,email_title:"
 msgid ""
 "The subject of the email.\n"
 "The Genshi syntax can be used with 'record' in the evaluation context."
 msgstr ""
-"El asunto del correo electrónico.\n"
-"La sintaxis Genshi puede ser utilizada con 'record' en el contexto de evaluación."
+"Zadeva te e-pošte.\n"
+"Lahko uporabite Genshi sintakso z 'record' v kontekstu vrednotenja."
 
 msgctxt "help:marketing.automation.activity,negative:"
 msgid ""
 "Check to execute the activity if the event has not happened by the end of "
 "the delay."
 msgstr ""
-"Marcar para ejecutar la actividad si el evento no ha ocurrido al final de la"
-" fecha retrasada."
+"Označite, če želite izvesti aktivnost, v kolikor do dogodka ni prišlo v "
+"opredeljenem zamiku."
 
 msgctxt "help:marketing.automation.scenario,domain:"
 msgid "A PYSON domain used to filter records valid for this scenario."
 msgstr ""
-"Dominio PYSON usado para filtrar los registros válidos para este escenario."
+"PYSON domena, ki se uporabi za filtriranje zapisov, ki so veljavno za ta "
+"scenarij."
 
 msgctxt "help:marketing.automation.scenario,unsubscribable:"
 msgid "If checked parties are also unsubscribed from the scenario."
-msgstr "Si se marca los terceros también se de-suscriben del escenario."
+msgstr "Označite, da se partner lahko odjavi s tega scenarija."
 
 msgctxt "model:ir.action,name:act_activity_tree"
 msgid "Activities"
-msgstr "Actividades"
+msgstr "Aktivnosti"
 
 msgctxt "model:ir.action,name:act_ir_email_form_relate_activity"
 msgid "E-mails"
-msgstr "Correos electrónicos"
+msgstr "E-pošte"
 
 msgctxt "model:ir.action,name:act_record_activity_form"
 msgid "Record Activities"
-msgstr "Registro de actividades"
+msgstr "Zapisi aktivnosti"
 
 msgctxt "model:ir.action,name:act_record_form"
 msgid "Records"
-msgstr "Registros"
+msgstr "Zapisi"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_reporting_activity"
 msgid "Activity Reporting"
-msgstr "Acción de actividad"
+msgstr "Ukrep aktivnosti"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_reporting_scenario"
 msgid "Scenario Reporting"
-msgstr "Escenario"
+msgstr "Scenarij"
 
 msgctxt "model:ir.action,name:act_scenario_form"
 msgid "Scenarios"
-msgstr "Escenarios"
+msgstr "Scenariji"
 
 msgctxt "model:ir.action,name:report_unsubscribe"
 msgid "Marketing Automation Unsubscribe"
-msgstr "Baja de la automatización de marketing"
+msgstr "Odjave automatizacije marketinga"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_record_activity_form_domain_all"
 msgid "All"
-msgstr "Todo"
+msgstr "Vse"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_record_activity_form_domain_cancelled"
 msgid "Cancelled"
-msgstr "Cancelado"
+msgstr "Preklicano"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_record_activity_form_domain_done"
 msgid "Done"
-msgstr "Realizado"
+msgstr "Zaključeno"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_record_activity_form_domain_waiting"
 msgid "Waiting"
-msgstr "En espera"
+msgstr "V čakanju"
 
 msgctxt "model:ir.action.act_window.domain,name:act_scenario_form_domain_all"
 msgid "All"
-msgstr "Todo"
+msgstr "Vse"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_scenario_form_domain_draft"
 msgid "Draft"
-msgstr "Borrador"
+msgstr "Osnutek"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_scenario_form_domain_running"
 msgid "Running"
-msgstr "En ejecución"
+msgstr "V izvajanju"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_scenario_form_domain_stopped"
 msgid "Stopped"
-msgstr "Parado"
+msgstr "Ustavljeno"
 
 msgctxt "model:ir.message,text:msg_activity_invalid_condition"
 msgid ""
 "Invalid condition \"%(condition)s\" in activity \"%(activity)s\" with "
 "exception \"%(exception)s\"."
 msgstr ""
-"Condición \"%(condition)s\" inválida en la actividad \"%(activity)s\" con la"
-" excepción \"%(exception)s\"."
+"Neveljaven pogojo \"%(condition)s\" v aktivnosti \"%(activity)s\" z napako "
+"\"%(exception)s\"."
 
 msgctxt "model:ir.message,text:msg_activity_invalid_email_template"
 msgid ""
 "Invalid e-mail template in activity \"%(activity)s\" with exception "
 "\"%(exception)s\"."
 msgstr ""
-"Plantilla de correo electrónico inválida en la actividad \"%(activity)s\" "
-"con la excepción \"%(exception)s\"."
+"Neveljavna e-poštna predloga v aktivnosti \"%(activity)s\" z napako "
+"\"%(exception)s\"."
 
 msgctxt "model:ir.message,text:msg_activity_invalid_email_title"
 msgid ""
 "Invalid e-mail title in activity \"%(activity)s\" with exception "
 "\"%(exception)s\"."
 msgstr ""
-"Título de correo electrónico inválido en la actividad \"%(activity)s\" con "
-"la excepción \"%(exception)s\"."
+"Neveljavna e-poštna zadeva v aktivnosti \"%(activity)s\" z napako "
+"\"%(exception)s\"."
 
 msgctxt "model:ir.message,text:msg_activity_record_unique"
 msgid "Record Activity must be unique by record and activity."
-msgstr "La actividad del registro debe ser única por registro y actividad."
+msgstr "Zapis aktivnosti mora biti edinstven po zapisu in aktivnosti."
 
 msgctxt "model:ir.message,text:msg_record_scenario_record_unique"
 msgid "Record must be unique by scenario."
-msgstr "El registro debe ser único por escenario."
+msgstr "Zapis mora biti edinstven po scenariju."
 
 msgctxt "model:ir.message,text:msg_record_uuid_unique"
 msgid "UUID of record must be unique."
-msgstr "El UUID del registro debe ser único."
+msgstr "UUID zapisa mora biti edinstven."
 
 msgctxt "model:ir.message,text:msg_scenario_invalid_domain"
 msgid "Invalid domain in scenario \"%(scenario)s\" with exception \"%(exception)s\"."
 msgstr ""
-"Dominio inválido en el escenario \"%(scenario)s\" con la excepción "
-"\"%(exception)s\"."
 
 msgctxt "model:ir.model.button,string:record_activity_on_email_clicked_button"
 msgid "E-Mail Clicked"
-msgstr "Correo electrónico pulsado"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:record_activity_on_email_opened_button"
 msgid "E-Mail Opened"
-msgstr "Correo electrónico abierto"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:record_block_button"
 msgid "Block"
-msgstr "Bloquear"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:scenario_draft_button"
 msgid "Draft"
-msgstr "Borrador"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:scenario_run_button"
 msgid "Run"
-msgstr "Ejecutar"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:scenario_stop_button"
 msgid "Stop"
-msgstr "Parar"
+msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_scenario_form"
 msgid "Scenarios"
-msgstr "Escenarios"
+msgstr ""
 
 msgctxt "model:marketing.automation.activity,name:"
 msgid "Marketing Activity"
-msgstr "Actividad de marketing"
+msgstr ""
 
 msgctxt "model:marketing.automation.record,name:"
 msgid "Marketing Record"
-msgstr "Registro de marketing"
+msgstr ""
 
 msgctxt "model:marketing.automation.record.activity,name:"
 msgid "Marketing Record Activity"
-msgstr "Actividad del registro de marketing"
+msgstr ""
 
 #, fuzzy
 msgctxt "model:marketing.automation.reporting.activity,name:"
 msgid "Marketing Automation Reporting Activity"
-msgstr "Actividad del registro de marketing"
+msgstr "Odjave automatizacije marketinga"
 
 #, fuzzy
 msgctxt "model:marketing.automation.reporting.context,name:"
 msgid "Marketing Automation Reporting Context"
-msgstr "Automatización de marketing"
+msgstr "Odjave automatizacije marketinga"
 
 #, fuzzy
 msgctxt "model:marketing.automation.reporting.scenario,name:"
 msgid "Marketing Automation Reporting Scenario"
-msgstr "Escenarios de automatización de marketing no suscritos"
+msgstr "Odjave automatizacije marketinga"
 
 msgctxt "model:marketing.automation.scenario,name:"
 msgid "Marketing Scenario"
-msgstr "Escenario de marketing"
+msgstr ""
 
 msgctxt "model:party.party-unsubscribed-marketing.automation.scenario,name:"
 msgid "Party Unsubscribed Scenario"
-msgstr "Escenarios de-suscritos del tercero"
+msgstr ""
 
 msgctxt "report:marketing.automation.unsubscribe:"
 msgid "Unsubscribe"
-msgstr "Darse de baja"
+msgstr ""
 
 msgctxt "report:marketing.automation.unsubscribe:"
 msgid ""
 "We are sorry to see you go, and apologize if we have overwhelmed your inbox."
 msgstr ""
-"Lamentamos verle marchar y le pedimos disculpas en caso que hubiéramos "
-"abusado de su bandeja de entrada de correo electrónico."
 
 msgctxt "report:marketing.automation.unsubscribe:"
 msgid "You are unsubscribed"
-msgstr "Te has dado de baja"
+msgstr ""
 
 msgctxt "report:marketing.automation.unsubscribe:"
 msgid "You have been successfully unsubscribed from this kind of email."
 msgstr ""
-"Se ha dado de baja de este tipo de correo electrónico satisfactoriamente."
 
 msgctxt "selection:ir.cron,method:"
 msgid "Process Marketing Activity"
-msgstr "Procesar actividad de marketing"
+msgstr ""
 
 msgctxt "selection:ir.cron,method:"
 msgid "Trigger Marketing Scenarios"
-msgstr "Ejecutar disparadores de escenarios de marketing"
+msgstr ""
 
 msgctxt "selection:marketing.automation.activity,action:"
 msgid "Send E-Mail"
-msgstr "Enviar correo electrónico"
+msgstr ""
 
 msgctxt "selection:marketing.automation.activity,event:"
 msgid "E-Mail Clicked"
-msgstr "Correo electrónico pulsado"
+msgstr ""
 
 msgctxt "selection:marketing.automation.activity,event:"
 msgid "E-Mail Opened"
-msgstr "Correo electrónico abierto"
+msgstr ""
 
 msgctxt "selection:marketing.automation.activity,on:"
 msgid "E-Mail Clicked"
-msgstr "Correo electrónico pulsado"
+msgstr ""
 
 msgctxt "selection:marketing.automation.activity,on:"
 msgid "E-Mail Not Clicked"
-msgstr "Correo electrónico no pulsado"
+msgstr ""
 
 msgctxt "selection:marketing.automation.activity,on:"
 msgid "E-Mail Not Opened"
-msgstr "Correo electrónico no abierto"
+msgstr ""
 
 msgctxt "selection:marketing.automation.activity,on:"
 msgid "E-Mail Opened"
-msgstr "Correo electrónico abierto"
+msgstr ""
 
 msgctxt "selection:marketing.automation.activity,parent:"
 msgid "Activity"
-msgstr "Actividad"
+msgstr ""
 
 msgctxt "selection:marketing.automation.activity,parent:"
 msgid "Scenario"
-msgstr "Escenario"
+msgstr ""
 
 msgctxt "selection:marketing.automation.record.activity,state:"
 msgid "Cancelled"
-msgstr "Cancelado"
+msgstr ""
 
 msgctxt "selection:marketing.automation.record.activity,state:"
 msgid "Done"
-msgstr "Finalizado"
+msgstr ""
 
 msgctxt "selection:marketing.automation.record.activity,state:"
 msgid "Waiting"
-msgstr "En espera"
+msgstr ""
 
 #, fuzzy
 msgctxt "selection:marketing.automation.reporting.context,period:"
 msgid "Day"
-msgstr "Retraso"
+msgstr "Zakasnitev"
 
 msgctxt "selection:marketing.automation.reporting.context,period:"
 msgid "Month"
 msgstr ""
 
 msgctxt "selection:marketing.automation.reporting.context,period:"
 msgid "Year"
 msgstr ""
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Draft"
-msgstr "Borrador"
+msgstr ""
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Running"
-msgstr "En ejecución"
+msgstr ""
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Stopped"
-msgstr "Detenido"
+msgstr ""
 
 msgctxt "view:marketing.automation.activity:"
 msgid "%"
 msgstr ""
 
 msgctxt "view:marketing.automation.activity:"
 msgid "After"
-msgstr "Después"
+msgstr ""
 
 msgctxt "view:marketing.automation.activity:"
 msgid "Edit"
-msgstr "Editar"
+msgstr ""
 
 msgctxt "view:marketing.automation.activity:"
 msgid "If"
-msgstr "Si"
+msgstr ""
 
 msgctxt "view:marketing.automation.activity:"
 msgid "On"
-msgstr "En"
+msgstr ""
 
 msgctxt "view:marketing.automation.activity:"
 msgid "Template:"
-msgstr "Plantilla:"
+msgstr ""
 
 msgctxt "view:marketing.automation.activity:"
 msgid "Title:"
-msgstr "Título:"
+msgstr ""
 
 msgctxt "view:marketing.automation.record.activity:"
 msgid "Time"
-msgstr "Hora"
+msgstr ""
 
 msgctxt "view:marketing.automation.reporting.activity:"
 msgid "%"
 msgstr ""
 
 msgctxt "view:marketing.automation.reporting.scenario:"
 msgid "%"
@@ -663,8 +660,8 @@
 
 msgctxt "view:marketing.automation.scenario:"
 msgid "%"
 msgstr ""
 
 msgctxt "view:party.party:"
 msgid "Marketing Automation"
-msgstr "Automatización de marketing"
+msgstr ""
```

### Comparing `trytond_marketing_automation-7.2.0/locale/es_419.po` & `trytond_marketing_automation-7.2.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-7.2.0/locale/et.po` & `trytond_marketing_automation-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-7.2.0/locale/fa.po` & `trytond_marketing_automation-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-7.2.0/locale/fi.po` & `trytond_marketing_automation-7.2.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-7.2.0/locale/fr.po` & `trytond_marketing_automation-7.2.1/locale/fr.po`

 * *Files 4% similar despite different names*

```diff
@@ -22,50 +22,45 @@
 msgid "Condition"
 msgstr "Condition"
 
 msgctxt "field:marketing.automation.activity,delay:"
 msgid "Delay"
 msgstr "Délai"
 
-#, fuzzy
 msgctxt "field:marketing.automation.activity,email_click_rate:"
 msgid "E-mail Click Rate"
-msgstr "E-mail cliqué"
+msgstr "Taux de clics sur les e-mails"
 
-#, fuzzy
 msgctxt "field:marketing.automation.activity,email_click_rate_trend:"
 msgid "E-mail Click Rate Trend"
-msgstr "E-mail cliqué"
+msgstr "Tendance du taux de clics sur les e-mails"
 
-#, fuzzy
 msgctxt "field:marketing.automation.activity,email_click_through_rate:"
 msgid "E-mail Click-Through Rate"
-msgstr "E-mail cliqué"
+msgstr "Taux de clics sur les e-mails ouverts"
 
 msgctxt "field:marketing.automation.activity,email_click_through_rate_trend:"
 msgid "E-mail Click-Through Rate Trend"
-msgstr ""
+msgstr "Tendance du taux de clics sur les e-mails ouverts"
 
 msgctxt "field:marketing.automation.activity,email_clicked:"
 msgid "E-Mails Clicked"
 msgstr "E-mails cliqués"
 
 msgctxt "field:marketing.automation.activity,email_from:"
 msgid "From"
 msgstr "De"
 
-#, fuzzy
 msgctxt "field:marketing.automation.activity,email_open_rate:"
 msgid "E-mail Open Rate"
-msgstr "E-mail ouvert"
+msgstr "Taux d'ouverture des e-mails"
 
-#, fuzzy
 msgctxt "field:marketing.automation.activity,email_open_rate_trend:"
 msgid "E-mail Open Rate Trend"
-msgstr "E-mail ouvert"
+msgstr "Tendance du taux d'ouverture des e-mails"
 
 msgctxt "field:marketing.automation.activity,email_opened:"
 msgid "E-Mails Opened"
 msgstr "E-mails ouverts"
 
 msgctxt "field:marketing.automation.activity,email_template:"
 msgid "E-Mail Template"
@@ -143,109 +138,94 @@
 msgid "Record"
 msgstr "Enregistrement"
 
 msgctxt "field:marketing.automation.record.activity,state:"
 msgid "State"
 msgstr "État"
 
-#, fuzzy
 msgctxt "field:marketing.automation.reporting.activity,activity:"
 msgid "Activity"
 msgstr "Activité"
 
-#, fuzzy
 msgctxt "field:marketing.automation.reporting.activity,activity_action:"
 msgid "Activity Action"
 msgstr "Action de l'activité"
 
 msgctxt "field:marketing.automation.reporting.activity,date:"
 msgid "Date"
-msgstr ""
+msgstr "Date"
 
-#, fuzzy
 msgctxt "field:marketing.automation.reporting.activity,email_click_rate:"
 msgid "E-mail Click Rate"
-msgstr "E-mail cliqué"
+msgstr "Taux de clics sur les e-mails"
 
-#, fuzzy
 msgctxt ""
 "field:marketing.automation.reporting.activity,email_click_through_rate:"
 msgid "E-mail Click-Through Rate"
-msgstr "E-mail cliqué"
+msgstr "Taux de clics sur les e-mails ouverts"
 
-#, fuzzy
 msgctxt "field:marketing.automation.reporting.activity,email_clicked:"
 msgid "E-Mails Clicked"
 msgstr "E-mails cliqués"
 
-#, fuzzy
 msgctxt "field:marketing.automation.reporting.activity,email_open_rate:"
 msgid "E-mail Open Rate"
-msgstr "E-mail ouvert"
+msgstr "Taux d'ouverture des e-mails"
 
-#, fuzzy
 msgctxt "field:marketing.automation.reporting.activity,email_opened:"
 msgid "E-Mails Opened"
 msgstr "E-mails ouverts"
 
-#, fuzzy
 msgctxt "field:marketing.automation.reporting.activity,record_count:"
 msgid "Records"
 msgstr "Enregistrements"
 
-#, fuzzy
 msgctxt "field:marketing.automation.reporting.context,from_date:"
 msgid "From Date"
-msgstr "Date de modification"
+msgstr "Date de début"
 
 msgctxt "field:marketing.automation.reporting.context,period:"
 msgid "Period"
-msgstr ""
+msgstr "Période"
 
 msgctxt "field:marketing.automation.reporting.context,to_date:"
 msgid "To Date"
-msgstr ""
+msgstr "Date de fin"
 
-#, fuzzy
 msgctxt "field:marketing.automation.reporting.scenario,block_rate:"
 msgid "Block Rate"
-msgstr "Bloqué"
+msgstr "Taux de blocage"
 
 msgctxt "field:marketing.automation.reporting.scenario,date:"
 msgid "Date"
-msgstr ""
+msgstr "Date"
 
-#, fuzzy
 msgctxt "field:marketing.automation.reporting.scenario,record_count:"
 msgid "Records"
 msgstr "Enregistrements"
 
-#, fuzzy
 msgctxt "field:marketing.automation.reporting.scenario,record_count_blocked:"
 msgid "Records Blocked"
 msgstr "Enregistrements bloqués"
 
-#, fuzzy
 msgctxt "field:marketing.automation.reporting.scenario,scenario:"
 msgid "Scenario"
 msgstr "Scénario"
 
 msgctxt "field:marketing.automation.scenario,activities:"
 msgid "Activities"
 msgstr "Activés"
 
-#, fuzzy
 msgctxt "field:marketing.automation.scenario,block_rate:"
 msgid "Block Rate"
-msgstr "Bloqué"
+msgstr "Taux de blocage"
 
-#, fuzzy
 msgctxt "field:marketing.automation.scenario,block_rate_trend:"
 msgid "Block Rate Trend"
-msgstr "Bloqué"
+msgstr "Tendance du taux de blocage"
 
 msgctxt "field:marketing.automation.scenario,domain:"
 msgid "Domain"
 msgstr "Domaine"
 
 msgctxt "field:marketing.automation.scenario,model:"
 msgid "Model"
@@ -356,23 +336,21 @@
 msgid "Record Activities"
 msgstr "Enregistrements d'activités"
 
 msgctxt "model:ir.action,name:act_record_form"
 msgid "Records"
 msgstr "Enregistrements"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_reporting_activity"
 msgid "Activity Reporting"
-msgstr "Action de l'activité"
+msgstr "Rapport d'activité"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_reporting_scenario"
 msgid "Scenario Reporting"
-msgstr "Scénario"
+msgstr "Rapport de scénario"
 
 msgctxt "model:ir.action,name:act_scenario_form"
 msgid "Scenarios"
 msgstr "Scénarios"
 
 msgctxt "model:ir.action,name:report_unsubscribe"
 msgid "Marketing Automation Unsubscribe"
@@ -496,28 +474,25 @@
 msgid "Marketing Record"
 msgstr "Enregistrement de marketing"
 
 msgctxt "model:marketing.automation.record.activity,name:"
 msgid "Marketing Record Activity"
 msgstr "Enregistrement d'activité marketing"
 
-#, fuzzy
 msgctxt "model:marketing.automation.reporting.activity,name:"
 msgid "Marketing Automation Reporting Activity"
-msgstr "Enregistrement d'activité marketing"
+msgstr "Rapport d'activité d’automatisation du marketing"
 
-#, fuzzy
 msgctxt "model:marketing.automation.reporting.context,name:"
 msgid "Marketing Automation Reporting Context"
-msgstr "Automatisation du marketing"
+msgstr "Contexte de rapport d'automatisation du marketing"
 
-#, fuzzy
 msgctxt "model:marketing.automation.reporting.scenario,name:"
 msgid "Marketing Automation Reporting Scenario"
-msgstr "Désinscription au scenario d'automatisation du marketing"
+msgstr "Scénario de rapport d'automatisation du marketing"
 
 msgctxt "model:marketing.automation.scenario,name:"
 msgid "Marketing Scenario"
 msgstr "Scénario marketing"
 
 msgctxt "model:party.party-unsubscribed-marketing.automation.scenario,name:"
 msgid "Party Unsubscribed Scenario"
@@ -594,26 +569,25 @@
 msgid "Done"
 msgstr "Terminé"
 
 msgctxt "selection:marketing.automation.record.activity,state:"
 msgid "Waiting"
 msgstr "En attente"
 
-#, fuzzy
 msgctxt "selection:marketing.automation.reporting.context,period:"
 msgid "Day"
-msgstr "Délai"
+msgstr "Jour"
 
 msgctxt "selection:marketing.automation.reporting.context,period:"
 msgid "Month"
-msgstr ""
+msgstr "Mois"
 
 msgctxt "selection:marketing.automation.reporting.context,period:"
 msgid "Year"
-msgstr ""
+msgstr "Année"
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Draft"
 msgstr "Brouillon"
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Running"
@@ -621,15 +595,15 @@
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Stopped"
 msgstr "Arrêté"
 
 msgctxt "view:marketing.automation.activity:"
 msgid "%"
-msgstr ""
+msgstr "%"
 
 msgctxt "view:marketing.automation.activity:"
 msgid "After"
 msgstr "Après"
 
 msgctxt "view:marketing.automation.activity:"
 msgid "Edit"
@@ -653,20 +627,20 @@
 
 msgctxt "view:marketing.automation.record.activity:"
 msgid "Time"
 msgstr "Heure"
 
 msgctxt "view:marketing.automation.reporting.activity:"
 msgid "%"
-msgstr ""
+msgstr "%"
 
 msgctxt "view:marketing.automation.reporting.scenario:"
 msgid "%"
-msgstr ""
+msgstr "%"
 
 msgctxt "view:marketing.automation.scenario:"
 msgid "%"
-msgstr ""
+msgstr "%"
 
 msgctxt "view:party.party:"
 msgid "Marketing Automation"
 msgstr "Automatisation du marketing"
```

### Comparing `trytond_marketing_automation-7.2.0/locale/hu.po` & `trytond_marketing_automation-7.2.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-7.2.0/locale/id.po` & `trytond_marketing_automation-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-7.2.0/locale/it.po` & `trytond_marketing_automation-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-7.2.0/locale/lo.po` & `trytond_marketing_automation-7.2.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-7.2.0/locale/lt.po` & `trytond_marketing_automation-7.2.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-7.2.0/locale/nl.po` & `trytond_marketing_automation-7.2.1/locale/ca.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,671 +1,642 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:ir.email,marketing_automation_activity:"
 msgid "Activity"
-msgstr "Activiteit"
+msgstr "Activitat"
 
 msgctxt "field:ir.email,marketing_automation_record:"
 msgid "Record"
-msgstr "Record"
+msgstr "Registre"
 
 msgctxt "field:marketing.automation.activity,action:"
 msgid "Action"
-msgstr "Actie"
+msgstr "Acció"
 
 msgctxt "field:marketing.automation.activity,children:"
 msgid "Children"
-msgstr "Onderliggende niveaus"
+msgstr "Fills"
 
 msgctxt "field:marketing.automation.activity,condition:"
 msgid "Condition"
-msgstr "Voorwaarde"
+msgstr "Condició"
 
 msgctxt "field:marketing.automation.activity,delay:"
 msgid "Delay"
-msgstr "Vertraging"
+msgstr "Retard"
 
-#, fuzzy
 msgctxt "field:marketing.automation.activity,email_click_rate:"
 msgid "E-mail Click Rate"
-msgstr "E-mail Geklikt"
+msgstr "Rati clicks correu"
 
-#, fuzzy
 msgctxt "field:marketing.automation.activity,email_click_rate_trend:"
 msgid "E-mail Click Rate Trend"
-msgstr "E-mail Geklikt"
+msgstr "Tendència rati clicks correu"
 
-#, fuzzy
 msgctxt "field:marketing.automation.activity,email_click_through_rate:"
 msgid "E-mail Click-Through Rate"
-msgstr "E-mail Geklikt"
+msgstr "Percentatge de clics del correu electrònic"
 
 msgctxt "field:marketing.automation.activity,email_click_through_rate_trend:"
 msgid "E-mail Click-Through Rate Trend"
-msgstr ""
+msgstr "Tendència del percentatge de clics del correu electrònic"
 
 msgctxt "field:marketing.automation.activity,email_clicked:"
 msgid "E-Mails Clicked"
-msgstr "E-mails Geklikt"
+msgstr "Correus electrònics clicats"
 
 msgctxt "field:marketing.automation.activity,email_from:"
 msgid "From"
-msgstr "Van"
+msgstr "De"
 
-#, fuzzy
 msgctxt "field:marketing.automation.activity,email_open_rate:"
 msgid "E-mail Open Rate"
-msgstr "E-mails geopend"
+msgstr "Rati d'obertura correus"
 
-#, fuzzy
 msgctxt "field:marketing.automation.activity,email_open_rate_trend:"
 msgid "E-mail Open Rate Trend"
-msgstr "E-mails geopend"
+msgstr "Tendència rati d'obertura correu"
 
 msgctxt "field:marketing.automation.activity,email_opened:"
 msgid "E-Mails Opened"
-msgstr "E-mails geopend"
+msgstr "Correus electrònics oberts"
 
 msgctxt "field:marketing.automation.activity,email_template:"
 msgid "E-Mail Template"
-msgstr "Email sjabloon"
+msgstr "Plantilla de correu electrònic"
 
 msgctxt "field:marketing.automation.activity,email_title:"
 msgid "E-Mail Title"
-msgstr "E-mail titel"
+msgstr "Títol del correu electrònic"
 
 msgctxt "field:marketing.automation.activity,event:"
 msgid "Event"
-msgstr "Evenement"
+msgstr "Esdeveniment"
 
 msgctxt "field:marketing.automation.activity,name:"
 msgid "Name"
-msgstr "Naam"
+msgstr "Nom"
 
 msgctxt "field:marketing.automation.activity,negative:"
 msgid "Negative"
-msgstr "Negatief"
+msgstr "Negatiu"
 
 msgctxt "field:marketing.automation.activity,on:"
 msgid "On"
-msgstr "Op"
+msgstr "A"
 
 msgctxt "field:marketing.automation.activity,parent:"
 msgid "Parent"
-msgstr "Bovenliggend niveau"
+msgstr "Pare"
 
 msgctxt "field:marketing.automation.activity,parent_action:"
 msgid "Parent Action"
-msgstr "Bovenliggende actie (parent)"
+msgstr "Acció pare"
 
 msgctxt "field:marketing.automation.activity,record_count:"
 msgid "Records"
-msgstr "Records"
+msgstr "Registres"
 
 msgctxt "field:marketing.automation.record,blocked:"
 msgid "Blocked"
-msgstr "geblokkeerd"
+msgstr "Bloquejat"
 
 msgctxt "field:marketing.automation.record,record:"
 msgid "Record"
-msgstr "Record"
+msgstr "Registre"
 
 msgctxt "field:marketing.automation.record,scenario:"
 msgid "Scenario"
-msgstr "Scenario"
+msgstr "Escenari"
 
 msgctxt "field:marketing.automation.record,uuid:"
 msgid "UUID"
-msgstr "UUID"
+msgstr "Identificador únic universal"
 
 msgctxt "field:marketing.automation.record.activity,activity:"
 msgid "Activity"
-msgstr "Activiteit"
+msgstr "Activitat"
 
 msgctxt "field:marketing.automation.record.activity,activity_action:"
 msgid "Activity Action"
-msgstr "Activiteit actie"
+msgstr "Acció d'activitat"
 
 msgctxt "field:marketing.automation.record.activity,at:"
 msgid "At"
-msgstr "Op"
+msgstr "A"
 
 msgctxt "field:marketing.automation.record.activity,email_clicked:"
 msgid "E-Mail Clicked"
-msgstr "E-mail Geklikt"
+msgstr "Correus electrònics clicats"
 
 msgctxt "field:marketing.automation.record.activity,email_opened:"
 msgid "E-Mail Opened"
-msgstr "E-mails geopend"
+msgstr "Correus electrònics oberts"
 
 msgctxt "field:marketing.automation.record.activity,record:"
 msgid "Record"
-msgstr "Record"
+msgstr "Registre"
 
 msgctxt "field:marketing.automation.record.activity,state:"
 msgid "State"
-msgstr "Status"
+msgstr "Estat"
 
-#, fuzzy
 msgctxt "field:marketing.automation.reporting.activity,activity:"
 msgid "Activity"
-msgstr "Activiteit"
+msgstr "Activitat"
 
-#, fuzzy
 msgctxt "field:marketing.automation.reporting.activity,activity_action:"
 msgid "Activity Action"
-msgstr "Activiteit actie"
+msgstr "Acció d'activitat"
 
 msgctxt "field:marketing.automation.reporting.activity,date:"
 msgid "Date"
-msgstr ""
+msgstr "Data"
 
-#, fuzzy
 msgctxt "field:marketing.automation.reporting.activity,email_click_rate:"
 msgid "E-mail Click Rate"
-msgstr "E-mail Geklikt"
+msgstr "Rati clicks correu"
 
-#, fuzzy
 msgctxt ""
 "field:marketing.automation.reporting.activity,email_click_through_rate:"
 msgid "E-mail Click-Through Rate"
-msgstr "E-mail Geklikt"
+msgstr "Percentatge de clics del correu electrònic"
 
-#, fuzzy
 msgctxt "field:marketing.automation.reporting.activity,email_clicked:"
 msgid "E-Mails Clicked"
-msgstr "E-mails Geklikt"
+msgstr "Correus electrònics clicats"
 
-#, fuzzy
 msgctxt "field:marketing.automation.reporting.activity,email_open_rate:"
 msgid "E-mail Open Rate"
-msgstr "E-mails geopend"
+msgstr "Rati d'obertura correus"
 
-#, fuzzy
 msgctxt "field:marketing.automation.reporting.activity,email_opened:"
 msgid "E-Mails Opened"
-msgstr "E-mails geopend"
+msgstr "Correus electrònics oberts"
 
-#, fuzzy
 msgctxt "field:marketing.automation.reporting.activity,record_count:"
 msgid "Records"
-msgstr "Records"
+msgstr "Registres"
 
-#, fuzzy
 msgctxt "field:marketing.automation.reporting.context,from_date:"
 msgid "From Date"
-msgstr "Bewerkingsdatum"
+msgstr "Des de la data"
 
 msgctxt "field:marketing.automation.reporting.context,period:"
 msgid "Period"
-msgstr ""
+msgstr "Període"
 
 msgctxt "field:marketing.automation.reporting.context,to_date:"
 msgid "To Date"
-msgstr ""
+msgstr "Fins a la data"
 
-#, fuzzy
 msgctxt "field:marketing.automation.reporting.scenario,block_rate:"
 msgid "Block Rate"
-msgstr "geblokkeerd"
+msgstr "Rati bloquejos"
 
 msgctxt "field:marketing.automation.reporting.scenario,date:"
 msgid "Date"
-msgstr ""
+msgstr "Data"
 
-#, fuzzy
 msgctxt "field:marketing.automation.reporting.scenario,record_count:"
 msgid "Records"
-msgstr "Records"
+msgstr "Registres"
 
-#, fuzzy
 msgctxt "field:marketing.automation.reporting.scenario,record_count_blocked:"
 msgid "Records Blocked"
-msgstr "Geblokkeerde records"
+msgstr "Registres bloquejats"
 
-#, fuzzy
 msgctxt "field:marketing.automation.reporting.scenario,scenario:"
 msgid "Scenario"
-msgstr "Scenario"
+msgstr "Escenari"
 
 msgctxt "field:marketing.automation.scenario,activities:"
 msgid "Activities"
-msgstr "Activiteiten"
+msgstr "Activitats"
 
-#, fuzzy
 msgctxt "field:marketing.automation.scenario,block_rate:"
 msgid "Block Rate"
-msgstr "geblokkeerd"
+msgstr "Rati bloquejos"
 
-#, fuzzy
 msgctxt "field:marketing.automation.scenario,block_rate_trend:"
 msgid "Block Rate Trend"
-msgstr "geblokkeerd"
+msgstr "Tendència rati bloquejos"
 
 msgctxt "field:marketing.automation.scenario,domain:"
 msgid "Domain"
-msgstr "Domein (domain)"
+msgstr "Domini"
 
 msgctxt "field:marketing.automation.scenario,model:"
 msgid "Model"
 msgstr "Model"
 
 msgctxt "field:marketing.automation.scenario,name:"
 msgid "Name"
-msgstr "Naam"
+msgstr "Nom"
 
 msgctxt "field:marketing.automation.scenario,record_count:"
 msgid "Records"
-msgstr "Records"
+msgstr "Registres"
 
 msgctxt "field:marketing.automation.scenario,record_count_blocked:"
 msgid "Records Blocked"
-msgstr "Geblokkeerde records"
+msgstr "Registres bloquejats"
 
 msgctxt "field:marketing.automation.scenario,state:"
 msgid "State"
-msgstr "Status"
+msgstr "Estat"
 
 msgctxt "field:marketing.automation.scenario,unsubscribable:"
 msgid "Unsubscribable"
-msgstr "Afmelden mogelijk"
+msgstr "Donar-se de baixa"
 
 msgctxt "field:party.party,marketing_party:"
 msgid "Marketing Party"
-msgstr "Marketing Relatie"
+msgstr "Tercer de màrqueting"
 
 msgctxt "field:party.party,marketing_scenario_unsubscribed:"
 msgid "Marketing Automation Scenario Unsubscribed"
-msgstr "Marketing Abonnement opgezegd"
+msgstr "Escenàris d'automatització de màrqueting no subscrits"
 
 msgctxt "field:party.party-unsubscribed-marketing.automation.scenario,party:"
 msgid "Party"
-msgstr "Relatie"
+msgstr "Tercer"
 
 msgctxt ""
 "field:party.party-unsubscribed-marketing.automation.scenario,scenario:"
 msgid "Scenario"
-msgstr "Scenario"
+msgstr "Escenari"
 
 msgctxt "field:sale.sale,marketing_party:"
 msgid "Marketing Party"
-msgstr "Marketing Relatie"
+msgstr "Tercer de màrqueting"
 
 msgctxt "help:marketing.automation.activity,condition:"
 msgid ""
 "The PYSON statement that the record must match in order to execute the activity.\n"
 "The record is represented by \"self\"."
 msgstr ""
-"De PYSON-expressie waaraan het record moet voldoen om de activiteit te kunnen uitvoeren.\n"
-"Het record wordt vertegenwoordigd door \"self\"."
+"L'expressió PYSON que el registre ha de complir per tal d'executar-se l'activitat.\n"
+"El registre s'expressa amb \"self\"."
 
 msgctxt "help:marketing.automation.activity,delay:"
 msgid "After how much time the action should be executed."
-msgstr "Na hoeveel tijd moet de actie worden uitgevoerd."
+msgstr "Desprès de quant temps s'hauria d'executar l'acció."
 
 msgctxt "help:marketing.automation.activity,email_from:"
 msgid "Leave empty to use the value defined in the configuration file."
-msgstr ""
-"Laat leeg om de waarde te gebruiken die gedefinieerd is in het "
-"configuratiebestand."
+msgstr "Deixa buit per utilizar el valor definit al fitxer de configuració."
 
 msgctxt "help:marketing.automation.activity,email_template:"
 msgid ""
 "The HTML content of the E-mail.\n"
 "The Genshi syntax can be used with 'record' in the evaluation context."
 msgstr ""
-"De HTML-inhoud van de e-mail.\n"
-"De Genshi-syntaxis kan gebruikt worden met 'record' in de evaluatiecontext."
+"El contingut HTML del correu electrònic.\n"
+"La sintaxi Genshi es pot fer servir amb 'record' al context d'avaluació."
 
 msgctxt "help:marketing.automation.activity,email_title:"
 msgid ""
 "The subject of the email.\n"
 "The Genshi syntax can be used with 'record' in the evaluation context."
 msgstr ""
-"Het onderwerp van de e-mail.\n"
-"De Genshi-syntaxis kan gebruikt worden met 'record' in de evaluatiecontext."
+"L'assumpte del correu electrònic.\n"
+"La sintaxi Genshi es pot fer servir amb 'record' al context d'avaluació."
 
 msgctxt "help:marketing.automation.activity,negative:"
 msgid ""
 "Check to execute the activity if the event has not happened by the end of "
 "the delay."
 msgstr ""
-"Schakel het selectievakje in om de activiteit uit te voeren als het "
-"evenement niet is gebeurd aan het einde van de vertraging."
+"Marcar per executar l'activitat si l'esdeveniment no s'ha executat al acabar"
+" el retard."
 
 msgctxt "help:marketing.automation.scenario,domain:"
 msgid "A PYSON domain used to filter records valid for this scenario."
 msgstr ""
-"Een PYSON-domein dat wordt gebruikt om records te filteren die geldig zijn "
-"voor dit scenario."
+"Un domini PYSON utilitzat per filtrar registres vàlid per aquest escenari."
 
 msgctxt "help:marketing.automation.scenario,unsubscribable:"
 msgid "If checked parties are also unsubscribed from the scenario."
-msgstr ""
-"Indien aangevinkt worden de relaties ook uitgeschreven uit het scenario."
+msgstr "Si es marca els tercer també es de-suscribeixen de l'escenari."
 
 msgctxt "model:ir.action,name:act_activity_tree"
 msgid "Activities"
-msgstr "Activiteiten"
+msgstr "Activitats"
 
 msgctxt "model:ir.action,name:act_ir_email_form_relate_activity"
 msgid "E-mails"
-msgstr "E-mails"
+msgstr "Correus electrònics"
 
 msgctxt "model:ir.action,name:act_record_activity_form"
 msgid "Record Activities"
-msgstr "Activiteiten opnemen"
+msgstr "Activitats del registre"
 
 msgctxt "model:ir.action,name:act_record_form"
 msgid "Records"
-msgstr "Records"
+msgstr "Registres"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_reporting_activity"
 msgid "Activity Reporting"
-msgstr "Activiteit actie"
+msgstr "Informe d'activitats"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_reporting_scenario"
 msgid "Scenario Reporting"
-msgstr "Scenario"
+msgstr "Informe d'escenaris"
 
 msgctxt "model:ir.action,name:act_scenario_form"
 msgid "Scenarios"
-msgstr "scenario's"
+msgstr "Escenaris"
 
 msgctxt "model:ir.action,name:report_unsubscribe"
 msgid "Marketing Automation Unsubscribe"
-msgstr "Marketing Automatizerings Abonnement opzeggen"
+msgstr "Baixa d'automatització de màrqueting"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_record_activity_form_domain_all"
 msgid "All"
-msgstr "Alle"
+msgstr "Tot"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_record_activity_form_domain_cancelled"
 msgid "Cancelled"
-msgstr "Geannuleerd"
+msgstr "Cancel·lat"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_record_activity_form_domain_done"
 msgid "Done"
-msgstr "Klaar"
+msgstr "Finalitzat"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_record_activity_form_domain_waiting"
 msgid "Waiting"
-msgstr "In afwachting"
+msgstr "En espera"
 
 msgctxt "model:ir.action.act_window.domain,name:act_scenario_form_domain_all"
 msgid "All"
-msgstr "Alle"
+msgstr "Tot"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_scenario_form_domain_draft"
 msgid "Draft"
-msgstr "Concept"
+msgstr "Esborrany"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_scenario_form_domain_running"
 msgid "Running"
-msgstr "in uitvoering"
+msgstr "En execució"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_scenario_form_domain_stopped"
 msgid "Stopped"
-msgstr "gestopt"
+msgstr "Aturat"
 
 msgctxt "model:ir.message,text:msg_activity_invalid_condition"
 msgid ""
 "Invalid condition \"%(condition)s\" in activity \"%(activity)s\" with "
 "exception \"%(exception)s\"."
 msgstr ""
-"Ongeldige voorwaarde \"%(condition)s\" in activiteit \"%(activity)s\" met "
-"uitzondering \"%(exception)s\"."
+"Condició no vàlida \"%(condition)s\" a l'activitat \"%(activity)s\" amb "
+"l'excepció \"%(exception)s\"."
 
 msgctxt "model:ir.message,text:msg_activity_invalid_email_template"
 msgid ""
 "Invalid e-mail template in activity \"%(activity)s\" with exception "
 "\"%(exception)s\"."
 msgstr ""
-"Ongeldige e-mailsjabloon in activiteit \"%(activity s\" met uitzondering "
-"\"%(exception)s\"."
+"Plantilla de correu electrònic no vàlida a l'activitat \"%(activity)s\" amb "
+"l'excepció \"%(exception)s\"."
 
 msgctxt "model:ir.message,text:msg_activity_invalid_email_title"
 msgid ""
 "Invalid e-mail title in activity \"%(activity)s\" with exception "
 "\"%(exception)s\"."
 msgstr ""
-"Ongeldige e-mailtitel in activiteit \"%(activity s\" met uitzondering "
-"\"%(exception)s\"."
+"Ttítol de la plantilla de correu electrònic no vàlida a l'activitat "
+"\"%(activity)s\" amb l'excepció \"%(exception)s\"."
 
 msgctxt "model:ir.message,text:msg_activity_record_unique"
 msgid "Record Activity must be unique by record and activity."
-msgstr "Recordactiviteit moet uniek zijn per record en activiteit."
+msgstr "L'activitat del registre ha de ser única per registre i activitat."
 
 msgctxt "model:ir.message,text:msg_record_scenario_record_unique"
 msgid "Record must be unique by scenario."
-msgstr "Record moet uniek zijn per scenario."
+msgstr "El registre ha de ser únic per cada escenari."
 
 msgctxt "model:ir.message,text:msg_record_uuid_unique"
 msgid "UUID of record must be unique."
-msgstr "UUID van het record moet uniek zijn."
+msgstr "L'UUID del registre ha de ser únic."
 
 msgctxt "model:ir.message,text:msg_scenario_invalid_domain"
 msgid "Invalid domain in scenario \"%(scenario)s\" with exception \"%(exception)s\"."
 msgstr ""
-"Ongeldig domein in scenario \"%(scenario)s\" met uitzondering "
+"Domini no vàlid a l'escenari \"%(scenario)s\" amb l'excepció "
 "\"%(exception)s\"."
 
 msgctxt "model:ir.model.button,string:record_activity_on_email_clicked_button"
 msgid "E-Mail Clicked"
-msgstr "E-mail Geklikt"
+msgstr "Correu electrònic clicat"
 
 msgctxt "model:ir.model.button,string:record_activity_on_email_opened_button"
 msgid "E-Mail Opened"
-msgstr "E-mails geopend"
+msgstr "Correu electrònic obert"
 
 msgctxt "model:ir.model.button,string:record_block_button"
 msgid "Block"
-msgstr "Blokkeer"
+msgstr "Bloqueja"
 
 msgctxt "model:ir.model.button,string:scenario_draft_button"
 msgid "Draft"
-msgstr "Concept"
+msgstr "Esborrany"
 
 msgctxt "model:ir.model.button,string:scenario_run_button"
 msgid "Run"
-msgstr "uitvoeren"
+msgstr "Executa"
 
 msgctxt "model:ir.model.button,string:scenario_stop_button"
 msgid "Stop"
-msgstr "stop"
+msgstr "Atura"
 
 msgctxt "model:ir.ui.menu,name:menu_scenario_form"
 msgid "Scenarios"
-msgstr "scenario's"
+msgstr "Escenaris"
 
 msgctxt "model:marketing.automation.activity,name:"
 msgid "Marketing Activity"
-msgstr "Marketing activiteit"
+msgstr "Activitat de màrqueting"
 
 msgctxt "model:marketing.automation.record,name:"
 msgid "Marketing Record"
-msgstr "Marketingrecord"
+msgstr "Registre de màrqueting"
 
 msgctxt "model:marketing.automation.record.activity,name:"
 msgid "Marketing Record Activity"
-msgstr "Marketingrecordactiviteit"
+msgstr "Activitat del registre de màrqueting"
 
-#, fuzzy
 msgctxt "model:marketing.automation.reporting.activity,name:"
 msgid "Marketing Automation Reporting Activity"
-msgstr "Marketingrecordactiviteit"
+msgstr "Activitat d'informes d'automatització del màrqueting"
 
-#, fuzzy
 msgctxt "model:marketing.automation.reporting.context,name:"
 msgid "Marketing Automation Reporting Context"
-msgstr "Marketing Abonnement Opzeggen"
+msgstr "Context d'informes d'automatització del màrqueting"
 
-#, fuzzy
 msgctxt "model:marketing.automation.reporting.scenario,name:"
 msgid "Marketing Automation Reporting Scenario"
-msgstr "Marketing Abonnement opgezegd"
+msgstr "Escenari d'informes d'automatització del màrqueting"
 
 msgctxt "model:marketing.automation.scenario,name:"
 msgid "Marketing Scenario"
-msgstr "Marketingscenario"
+msgstr "Escenari de màrqueting"
 
 msgctxt "model:party.party-unsubscribed-marketing.automation.scenario,name:"
 msgid "Party Unsubscribed Scenario"
-msgstr "Relatie Uitschrijf Scenario"
+msgstr "Escenaris de-suscrits del tercer"
 
 msgctxt "report:marketing.automation.unsubscribe:"
 msgid "Unsubscribe"
-msgstr "Afmelden"
+msgstr "Donar-se de baixa"
 
 msgctxt "report:marketing.automation.unsubscribe:"
 msgid ""
 "We are sorry to see you go, and apologize if we have overwhelmed your inbox."
 msgstr ""
-"Het spijt ons u te zien gaan. Onze excuses als we uw inbox vervuild hebben ."
+"Sentim veure't marxar, i ens disculpem si hem aclaparat la teva safata "
+"d'entrada."
 
 msgctxt "report:marketing.automation.unsubscribe:"
 msgid "You are unsubscribed"
-msgstr "U bent uitgeschreven"
+msgstr "T'has donat de baixa"
 
 msgctxt "report:marketing.automation.unsubscribe:"
 msgid "You have been successfully unsubscribed from this kind of email."
-msgstr "U bent succesvol afgemeld voor dit soort e-mail."
+msgstr "T'has donat de baixa amb èxit d'aquest tipus de correu electrònic."
 
 msgctxt "selection:ir.cron,method:"
 msgid "Process Marketing Activity"
-msgstr "Marketingactiviteit verwerken"
+msgstr "Processar activitats de màrqueting"
 
 msgctxt "selection:ir.cron,method:"
 msgid "Trigger Marketing Scenarios"
-msgstr "Trigger Marketing Scenario's"
+msgstr "Executar disparadors del escenaris de màrqueting"
 
 msgctxt "selection:marketing.automation.activity,action:"
 msgid "Send E-Mail"
-msgstr "E-mail verzenden"
+msgstr "Correu electrònic enviat"
 
 msgctxt "selection:marketing.automation.activity,event:"
 msgid "E-Mail Clicked"
-msgstr "E-mail Geklikt"
+msgstr "Correu electrònic clicat"
 
 msgctxt "selection:marketing.automation.activity,event:"
 msgid "E-Mail Opened"
-msgstr "E-mails geopend"
+msgstr "Correu electrònic obert"
 
 msgctxt "selection:marketing.automation.activity,on:"
 msgid "E-Mail Clicked"
-msgstr "E-mail Geklikt"
+msgstr "Correu electrònic clicat"
 
 msgctxt "selection:marketing.automation.activity,on:"
 msgid "E-Mail Not Clicked"
-msgstr "E-mail niet aangeklikt"
+msgstr "Correu electrònic no clicat"
 
 msgctxt "selection:marketing.automation.activity,on:"
 msgid "E-Mail Not Opened"
-msgstr "E-mail niet geopend"
+msgstr "Correu electrònic no obert"
 
 msgctxt "selection:marketing.automation.activity,on:"
 msgid "E-Mail Opened"
-msgstr "E-mails geopend"
+msgstr "Correu electrònic obert"
 
 msgctxt "selection:marketing.automation.activity,parent:"
 msgid "Activity"
-msgstr "Activiteit"
+msgstr "Activitat"
 
 msgctxt "selection:marketing.automation.activity,parent:"
 msgid "Scenario"
-msgstr "Scenario"
+msgstr "Escenari"
 
 msgctxt "selection:marketing.automation.record.activity,state:"
 msgid "Cancelled"
-msgstr "Geannuleerd"
+msgstr "Cancel·lada"
 
 msgctxt "selection:marketing.automation.record.activity,state:"
 msgid "Done"
-msgstr "Klaar"
+msgstr "Finalitzada"
 
 msgctxt "selection:marketing.automation.record.activity,state:"
 msgid "Waiting"
-msgstr "In afwachting"
+msgstr "En espera"
 
-#, fuzzy
 msgctxt "selection:marketing.automation.reporting.context,period:"
 msgid "Day"
-msgstr "Vertraging"
+msgstr "Dia"
 
 msgctxt "selection:marketing.automation.reporting.context,period:"
 msgid "Month"
-msgstr ""
+msgstr "Mes"
 
 msgctxt "selection:marketing.automation.reporting.context,period:"
 msgid "Year"
-msgstr ""
+msgstr "Any"
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Draft"
-msgstr "Concept"
+msgstr "Esborrany"
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Running"
-msgstr "in uitvoering"
+msgstr "En execució"
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Stopped"
-msgstr "gestopt"
+msgstr "Aturat"
 
 msgctxt "view:marketing.automation.activity:"
 msgid "%"
-msgstr ""
+msgstr "%"
 
 msgctxt "view:marketing.automation.activity:"
 msgid "After"
-msgstr "Na"
+msgstr "Desprès"
 
 msgctxt "view:marketing.automation.activity:"
 msgid "Edit"
-msgstr "Bewerk"
+msgstr "Edita"
 
 msgctxt "view:marketing.automation.activity:"
 msgid "If"
-msgstr "Als"
+msgstr "Si"
 
 msgctxt "view:marketing.automation.activity:"
 msgid "On"
-msgstr "Op"
+msgstr "A"
 
 msgctxt "view:marketing.automation.activity:"
 msgid "Template:"
-msgstr "Sjabloon:"
+msgstr "Plantilla:"
 
 msgctxt "view:marketing.automation.activity:"
 msgid "Title:"
-msgstr "Titel:"
+msgstr "Títol:"
 
 msgctxt "view:marketing.automation.record.activity:"
 msgid "Time"
-msgstr "Tijd"
+msgstr "Hora"
 
 msgctxt "view:marketing.automation.reporting.activity:"
 msgid "%"
-msgstr ""
+msgstr "%"
 
 msgctxt "view:marketing.automation.reporting.scenario:"
 msgid "%"
-msgstr ""
+msgstr "%"
 
 msgctxt "view:marketing.automation.scenario:"
 msgid "%"
-msgstr ""
+msgstr "%"
 
 msgctxt "view:party.party:"
 msgid "Marketing Automation"
-msgstr "Marketing Abonnement Opzeggen"
+msgstr "Automatització de màrqueting"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_marketing_automation-7.2.0/locale/pl.po` & `trytond_marketing_automation-7.2.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-7.2.0/locale/pt.po` & `trytond_marketing_automation-7.2.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-7.2.0/locale/ro.po` & `trytond_marketing_automation-7.2.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-7.2.0/locale/ru.po` & `trytond_marketing_automation-7.2.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-7.2.0/locale/sl.po` & `trytond_marketing_automation-7.2.1/locale/es.po`

 * *Files 14% similar despite different names*

```diff
@@ -1,667 +1,644 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:ir.email,marketing_automation_activity:"
 msgid "Activity"
-msgstr "Aktivnost"
+msgstr "Actividad"
 
 msgctxt "field:ir.email,marketing_automation_record:"
 msgid "Record"
-msgstr "Zapis"
+msgstr "Registro"
 
 msgctxt "field:marketing.automation.activity,action:"
 msgid "Action"
-msgstr "Ukrep"
+msgstr "Acción"
 
 msgctxt "field:marketing.automation.activity,children:"
 msgid "Children"
-msgstr "Podukrepi"
+msgstr "Hijos"
 
 msgctxt "field:marketing.automation.activity,condition:"
 msgid "Condition"
-msgstr "Pogoj"
+msgstr "Condición"
 
 msgctxt "field:marketing.automation.activity,delay:"
 msgid "Delay"
-msgstr "Zakasnitev"
+msgstr "Retraso"
 
-#, fuzzy
 msgctxt "field:marketing.automation.activity,email_click_rate:"
 msgid "E-mail Click Rate"
-msgstr "E-poštni kliki"
+msgstr "Ratio Clicks correo"
 
-#, fuzzy
 msgctxt "field:marketing.automation.activity,email_click_rate_trend:"
 msgid "E-mail Click Rate Trend"
-msgstr "E-poštni kliki"
+msgstr "Tendencia ratio clicks correo"
 
-#, fuzzy
 msgctxt "field:marketing.automation.activity,email_click_through_rate:"
 msgid "E-mail Click-Through Rate"
-msgstr "E-poštni kliki"
+msgstr "Tasa de clics de correo electrónico"
 
 msgctxt "field:marketing.automation.activity,email_click_through_rate_trend:"
 msgid "E-mail Click-Through Rate Trend"
-msgstr ""
+msgstr "Tendencia de la tasa de clics de correo electrónico"
 
 msgctxt "field:marketing.automation.activity,email_clicked:"
 msgid "E-Mails Clicked"
-msgstr "E-poštni kliki"
+msgstr "Correos electrónicos pulsados"
 
 msgctxt "field:marketing.automation.activity,email_from:"
 msgid "From"
-msgstr "Od"
+msgstr "De"
 
-#, fuzzy
 msgctxt "field:marketing.automation.activity,email_open_rate:"
 msgid "E-mail Open Rate"
-msgstr "E-pošta odprta"
+msgstr "Ratio apertura correo"
 
-#, fuzzy
 msgctxt "field:marketing.automation.activity,email_open_rate_trend:"
 msgid "E-mail Open Rate Trend"
-msgstr "E-pošta odprta"
+msgstr "Tendencia ratio apertura correo"
 
 msgctxt "field:marketing.automation.activity,email_opened:"
 msgid "E-Mails Opened"
-msgstr "E-pošta odprta"
+msgstr "Correos electrónicos abiertos"
 
 msgctxt "field:marketing.automation.activity,email_template:"
 msgid "E-Mail Template"
-msgstr "E-poštna predloga"
+msgstr "Plantilla de correo electrónico"
 
 msgctxt "field:marketing.automation.activity,email_title:"
 msgid "E-Mail Title"
-msgstr "E-poštna zadeva"
+msgstr "Titulo del correo electrónico"
 
 msgctxt "field:marketing.automation.activity,event:"
 msgid "Event"
-msgstr "Dogodek"
+msgstr "Evento"
 
 msgctxt "field:marketing.automation.activity,name:"
 msgid "Name"
-msgstr "Naziv"
+msgstr "Nombre"
 
 msgctxt "field:marketing.automation.activity,negative:"
 msgid "Negative"
-msgstr "Negativno"
+msgstr "Negativo"
 
 msgctxt "field:marketing.automation.activity,on:"
 msgid "On"
-msgstr "Na"
+msgstr "A"
 
 msgctxt "field:marketing.automation.activity,parent:"
 msgid "Parent"
-msgstr "Matični ukrep"
+msgstr "Padre"
 
 msgctxt "field:marketing.automation.activity,parent_action:"
 msgid "Parent Action"
-msgstr "Matični ukrep"
+msgstr "Acción padre"
 
 msgctxt "field:marketing.automation.activity,record_count:"
 msgid "Records"
-msgstr "Zapisi"
+msgstr "Registros"
 
 msgctxt "field:marketing.automation.record,blocked:"
 msgid "Blocked"
-msgstr "Blokiran"
+msgstr "Bloqueado"
 
 msgctxt "field:marketing.automation.record,record:"
 msgid "Record"
-msgstr "Zapis"
+msgstr "Registro"
 
 msgctxt "field:marketing.automation.record,scenario:"
 msgid "Scenario"
-msgstr "Scenarij"
+msgstr "Escenario"
 
 msgctxt "field:marketing.automation.record,uuid:"
 msgid "UUID"
-msgstr "UUID"
+msgstr "Identificador único universal"
 
 msgctxt "field:marketing.automation.record.activity,activity:"
 msgid "Activity"
-msgstr "Aktivnost"
+msgstr "Actividad"
 
 msgctxt "field:marketing.automation.record.activity,activity_action:"
 msgid "Activity Action"
-msgstr "Ukrep aktivnosti"
+msgstr "Acción de actividad"
 
 msgctxt "field:marketing.automation.record.activity,at:"
 msgid "At"
-msgstr "Ob"
+msgstr "A"
 
 msgctxt "field:marketing.automation.record.activity,email_clicked:"
 msgid "E-Mail Clicked"
-msgstr "E-poštni kliki"
+msgstr "Correo electrónico pulsado"
 
 msgctxt "field:marketing.automation.record.activity,email_opened:"
 msgid "E-Mail Opened"
-msgstr "E-pošta odprta"
+msgstr "Correo electrónico abierto"
 
 msgctxt "field:marketing.automation.record.activity,record:"
 msgid "Record"
-msgstr "Zapis"
+msgstr "Registro"
 
 msgctxt "field:marketing.automation.record.activity,state:"
 msgid "State"
-msgstr "Stanje"
+msgstr "Estado"
 
-#, fuzzy
 msgctxt "field:marketing.automation.reporting.activity,activity:"
 msgid "Activity"
-msgstr "Aktivnost"
+msgstr "Actividad"
 
-#, fuzzy
 msgctxt "field:marketing.automation.reporting.activity,activity_action:"
 msgid "Activity Action"
-msgstr "Ukrep aktivnosti"
+msgstr "Acción de actividad"
 
 msgctxt "field:marketing.automation.reporting.activity,date:"
 msgid "Date"
-msgstr ""
+msgstr "Fecha"
 
-#, fuzzy
 msgctxt "field:marketing.automation.reporting.activity,email_click_rate:"
 msgid "E-mail Click Rate"
-msgstr "E-poštni kliki"
+msgstr "Ratio Clicks correo"
 
-#, fuzzy
 msgctxt ""
 "field:marketing.automation.reporting.activity,email_click_through_rate:"
 msgid "E-mail Click-Through Rate"
-msgstr "E-poštni kliki"
+msgstr "Tasa de clics de correo electrónico"
 
-#, fuzzy
 msgctxt "field:marketing.automation.reporting.activity,email_clicked:"
 msgid "E-Mails Clicked"
-msgstr "E-poštni kliki"
+msgstr "Emails clicados"
 
-#, fuzzy
 msgctxt "field:marketing.automation.reporting.activity,email_open_rate:"
 msgid "E-mail Open Rate"
-msgstr "E-pošta odprta"
+msgstr "Ratio apertura correo"
 
-#, fuzzy
 msgctxt "field:marketing.automation.reporting.activity,email_opened:"
 msgid "E-Mails Opened"
-msgstr "E-pošta odprta"
+msgstr "Correos abiertos"
 
-#, fuzzy
 msgctxt "field:marketing.automation.reporting.activity,record_count:"
 msgid "Records"
-msgstr "Zapisi"
+msgstr "Registros"
 
-#, fuzzy
 msgctxt "field:marketing.automation.reporting.context,from_date:"
 msgid "From Date"
-msgstr "Od"
+msgstr "Desde la fecha"
 
 msgctxt "field:marketing.automation.reporting.context,period:"
 msgid "Period"
-msgstr ""
+msgstr "Periodo"
 
 msgctxt "field:marketing.automation.reporting.context,to_date:"
 msgid "To Date"
-msgstr ""
+msgstr "Hasta la fecha"
 
-#, fuzzy
 msgctxt "field:marketing.automation.reporting.scenario,block_rate:"
 msgid "Block Rate"
-msgstr "Blokiran"
+msgstr "Ratio bloqueos"
 
 msgctxt "field:marketing.automation.reporting.scenario,date:"
 msgid "Date"
-msgstr ""
+msgstr "Fecha"
 
-#, fuzzy
 msgctxt "field:marketing.automation.reporting.scenario,record_count:"
 msgid "Records"
-msgstr "Zapisi"
+msgstr "Registros"
 
-#, fuzzy
 msgctxt "field:marketing.automation.reporting.scenario,record_count_blocked:"
 msgid "Records Blocked"
-msgstr "Blokirani zapisi"
+msgstr "Registros bloqueados"
 
-#, fuzzy
 msgctxt "field:marketing.automation.reporting.scenario,scenario:"
 msgid "Scenario"
-msgstr "Scenarij"
+msgstr "Escenario"
 
 msgctxt "field:marketing.automation.scenario,activities:"
 msgid "Activities"
-msgstr "Aktivnosti"
+msgstr "Actividades"
 
-#, fuzzy
 msgctxt "field:marketing.automation.scenario,block_rate:"
 msgid "Block Rate"
-msgstr "Blokiran"
+msgstr "Ratio bloqueos"
 
-#, fuzzy
 msgctxt "field:marketing.automation.scenario,block_rate_trend:"
 msgid "Block Rate Trend"
-msgstr "Blokiran"
+msgstr "Tendencia ratio bloqueos"
 
 msgctxt "field:marketing.automation.scenario,domain:"
 msgid "Domain"
-msgstr "Domena"
+msgstr "Dominio"
 
 msgctxt "field:marketing.automation.scenario,model:"
 msgid "Model"
-msgstr "Model"
+msgstr "Modelo"
 
 msgctxt "field:marketing.automation.scenario,name:"
 msgid "Name"
-msgstr "Naziv"
+msgstr "Nombre"
 
 msgctxt "field:marketing.automation.scenario,record_count:"
 msgid "Records"
-msgstr "Zapisi"
+msgstr "Registros"
 
 msgctxt "field:marketing.automation.scenario,record_count_blocked:"
 msgid "Records Blocked"
-msgstr "Blokirani zapisi"
+msgstr "Registros bloqueados"
 
 msgctxt "field:marketing.automation.scenario,state:"
 msgid "State"
-msgstr "Stanje"
+msgstr "Estado"
 
 msgctxt "field:marketing.automation.scenario,unsubscribable:"
 msgid "Unsubscribable"
-msgstr "Odjava"
+msgstr "Darse de baja"
 
 msgctxt "field:party.party,marketing_party:"
 msgid "Marketing Party"
-msgstr "Marketing Partner"
+msgstr "Tercero del marketing"
 
 msgctxt "field:party.party,marketing_scenario_unsubscribed:"
 msgid "Marketing Automation Scenario Unsubscribed"
-msgstr ""
+msgstr "Escenarios de automatización de marketing no suscritos"
 
 msgctxt "field:party.party-unsubscribed-marketing.automation.scenario,party:"
 msgid "Party"
-msgstr "Partner"
+msgstr "Tercero"
 
 msgctxt ""
 "field:party.party-unsubscribed-marketing.automation.scenario,scenario:"
 msgid "Scenario"
-msgstr "Scenarij"
+msgstr "Escenario"
 
 msgctxt "field:sale.sale,marketing_party:"
 msgid "Marketing Party"
-msgstr "Marketing partner"
+msgstr "Tercero del marketing"
 
 msgctxt "help:marketing.automation.activity,condition:"
 msgid ""
 "The PYSON statement that the record must match in order to execute the activity.\n"
 "The record is represented by \"self\"."
 msgstr ""
-"Izraz PYSON, s katerim se mora zapis ujemati, da se aktivnost izvaja.\n"
-"Zapis je predstavljen s \"self\"."
+"La condicion PYSON que debe satisfacer el registro para ejecutar la actividad.\n"
+"El registro es representado por \"self\"."
 
 msgctxt "help:marketing.automation.activity,delay:"
 msgid "After how much time the action should be executed."
-msgstr "Po koliko časa naj bo ukrep izveden."
+msgstr "Después de cuánto tiempo debe ser ejecutada la acción."
 
 msgctxt "help:marketing.automation.activity,email_from:"
 msgid "Leave empty to use the value defined in the configuration file."
 msgstr ""
-"Pustite prazno, da uporabite vrednost opredeljeno v konfiguracijski "
-"datoteki."
+"Dejar vacío para usar el valor definido en el archivo de configuración."
 
 msgctxt "help:marketing.automation.activity,email_template:"
 msgid ""
 "The HTML content of the E-mail.\n"
 "The Genshi syntax can be used with 'record' in the evaluation context."
 msgstr ""
-"HTML vsebina e-pošte.\n"
-"Lahko uporabite Genshi sintakso z 'record' v kontekstu vrednotenja."
+"El contenido HTML del correo electrónico.\n"
+"La sintaxis Genshi puede ser utilizada con 'record' en el contexto de evaluación."
 
 msgctxt "help:marketing.automation.activity,email_title:"
 msgid ""
 "The subject of the email.\n"
 "The Genshi syntax can be used with 'record' in the evaluation context."
 msgstr ""
-"Zadeva te e-pošte.\n"
-"Lahko uporabite Genshi sintakso z 'record' v kontekstu vrednotenja."
+"El asunto del correo electrónico.\n"
+"La sintaxis Genshi puede ser utilizada con 'record' en el contexto de evaluación."
 
 msgctxt "help:marketing.automation.activity,negative:"
 msgid ""
 "Check to execute the activity if the event has not happened by the end of "
 "the delay."
 msgstr ""
-"Označite, če želite izvesti aktivnost, v kolikor do dogodka ni prišlo v "
-"opredeljenem zamiku."
+"Marcar para ejecutar la actividad si el evento no ha ocurrido al final de la"
+" fecha retrasada."
 
 msgctxt "help:marketing.automation.scenario,domain:"
 msgid "A PYSON domain used to filter records valid for this scenario."
 msgstr ""
-"PYSON domena, ki se uporabi za filtriranje zapisov, ki so veljavno za ta "
-"scenarij."
+"Dominio PYSON usado para filtrar los registros válidos para este escenario."
 
 msgctxt "help:marketing.automation.scenario,unsubscribable:"
 msgid "If checked parties are also unsubscribed from the scenario."
-msgstr "Označite, da se partner lahko odjavi s tega scenarija."
+msgstr "Si se marca los terceros también se de-suscriben del escenario."
 
 msgctxt "model:ir.action,name:act_activity_tree"
 msgid "Activities"
-msgstr "Aktivnosti"
+msgstr "Actividades"
 
 msgctxt "model:ir.action,name:act_ir_email_form_relate_activity"
 msgid "E-mails"
-msgstr "E-pošte"
+msgstr "Correos electrónicos"
 
 msgctxt "model:ir.action,name:act_record_activity_form"
 msgid "Record Activities"
-msgstr "Zapisi aktivnosti"
+msgstr "Registro de actividades"
 
 msgctxt "model:ir.action,name:act_record_form"
 msgid "Records"
-msgstr "Zapisi"
+msgstr "Registros"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_reporting_activity"
 msgid "Activity Reporting"
-msgstr "Ukrep aktivnosti"
+msgstr "Informe actividades"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_reporting_scenario"
 msgid "Scenario Reporting"
-msgstr "Scenarij"
+msgstr "Informe escenario"
 
 msgctxt "model:ir.action,name:act_scenario_form"
 msgid "Scenarios"
-msgstr "Scenariji"
+msgstr "Escenarios"
 
 msgctxt "model:ir.action,name:report_unsubscribe"
 msgid "Marketing Automation Unsubscribe"
-msgstr "Odjave automatizacije marketinga"
+msgstr "Baja de la automatización de marketing"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_record_activity_form_domain_all"
 msgid "All"
-msgstr "Vse"
+msgstr "Todo"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_record_activity_form_domain_cancelled"
 msgid "Cancelled"
-msgstr "Preklicano"
+msgstr "Cancelado"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_record_activity_form_domain_done"
 msgid "Done"
-msgstr "Zaključeno"
+msgstr "Realizado"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_record_activity_form_domain_waiting"
 msgid "Waiting"
-msgstr "V čakanju"
+msgstr "En espera"
 
 msgctxt "model:ir.action.act_window.domain,name:act_scenario_form_domain_all"
 msgid "All"
-msgstr "Vse"
+msgstr "Todo"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_scenario_form_domain_draft"
 msgid "Draft"
-msgstr "Osnutek"
+msgstr "Borrador"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_scenario_form_domain_running"
 msgid "Running"
-msgstr "V izvajanju"
+msgstr "En ejecución"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_scenario_form_domain_stopped"
 msgid "Stopped"
-msgstr "Ustavljeno"
+msgstr "Parado"
 
 msgctxt "model:ir.message,text:msg_activity_invalid_condition"
 msgid ""
 "Invalid condition \"%(condition)s\" in activity \"%(activity)s\" with "
 "exception \"%(exception)s\"."
 msgstr ""
-"Neveljaven pogojo \"%(condition)s\" v aktivnosti \"%(activity)s\" z napako "
-"\"%(exception)s\"."
+"Condición \"%(condition)s\" inválida en la actividad \"%(activity)s\" con la"
+" excepción \"%(exception)s\"."
 
 msgctxt "model:ir.message,text:msg_activity_invalid_email_template"
 msgid ""
 "Invalid e-mail template in activity \"%(activity)s\" with exception "
 "\"%(exception)s\"."
 msgstr ""
-"Neveljavna e-poštna predloga v aktivnosti \"%(activity)s\" z napako "
-"\"%(exception)s\"."
+"Plantilla de correo electrónico inválida en la actividad \"%(activity)s\" "
+"con la excepción \"%(exception)s\"."
 
 msgctxt "model:ir.message,text:msg_activity_invalid_email_title"
 msgid ""
 "Invalid e-mail title in activity \"%(activity)s\" with exception "
 "\"%(exception)s\"."
 msgstr ""
-"Neveljavna e-poštna zadeva v aktivnosti \"%(activity)s\" z napako "
-"\"%(exception)s\"."
+"Título de correo electrónico inválido en la actividad \"%(activity)s\" con "
+"la excepción \"%(exception)s\"."
 
 msgctxt "model:ir.message,text:msg_activity_record_unique"
 msgid "Record Activity must be unique by record and activity."
-msgstr "Zapis aktivnosti mora biti edinstven po zapisu in aktivnosti."
+msgstr "La actividad del registro debe ser única por registro y actividad."
 
 msgctxt "model:ir.message,text:msg_record_scenario_record_unique"
 msgid "Record must be unique by scenario."
-msgstr "Zapis mora biti edinstven po scenariju."
+msgstr "El registro debe ser único por escenario."
 
 msgctxt "model:ir.message,text:msg_record_uuid_unique"
 msgid "UUID of record must be unique."
-msgstr "UUID zapisa mora biti edinstven."
+msgstr "El UUID del registro debe ser único."
 
 msgctxt "model:ir.message,text:msg_scenario_invalid_domain"
 msgid "Invalid domain in scenario \"%(scenario)s\" with exception \"%(exception)s\"."
 msgstr ""
+"Dominio inválido en el escenario \"%(scenario)s\" con la excepción "
+"\"%(exception)s\"."
 
 msgctxt "model:ir.model.button,string:record_activity_on_email_clicked_button"
 msgid "E-Mail Clicked"
-msgstr ""
+msgstr "Correo electrónico pulsado"
 
 msgctxt "model:ir.model.button,string:record_activity_on_email_opened_button"
 msgid "E-Mail Opened"
-msgstr ""
+msgstr "Correo electrónico abierto"
 
 msgctxt "model:ir.model.button,string:record_block_button"
 msgid "Block"
-msgstr ""
+msgstr "Bloquear"
 
 msgctxt "model:ir.model.button,string:scenario_draft_button"
 msgid "Draft"
-msgstr ""
+msgstr "Borrador"
 
 msgctxt "model:ir.model.button,string:scenario_run_button"
 msgid "Run"
-msgstr ""
+msgstr "Ejecutar"
 
 msgctxt "model:ir.model.button,string:scenario_stop_button"
 msgid "Stop"
-msgstr ""
+msgstr "Parar"
 
 msgctxt "model:ir.ui.menu,name:menu_scenario_form"
 msgid "Scenarios"
-msgstr ""
+msgstr "Escenarios"
 
 msgctxt "model:marketing.automation.activity,name:"
 msgid "Marketing Activity"
-msgstr ""
+msgstr "Actividad de marketing"
 
 msgctxt "model:marketing.automation.record,name:"
 msgid "Marketing Record"
-msgstr ""
+msgstr "Registro de marketing"
 
 msgctxt "model:marketing.automation.record.activity,name:"
 msgid "Marketing Record Activity"
-msgstr ""
+msgstr "Actividad del registro de marketing"
 
-#, fuzzy
 msgctxt "model:marketing.automation.reporting.activity,name:"
 msgid "Marketing Automation Reporting Activity"
-msgstr "Odjave automatizacije marketinga"
+msgstr "Informe Actividad del registro de marketing"
 
-#, fuzzy
 msgctxt "model:marketing.automation.reporting.context,name:"
 msgid "Marketing Automation Reporting Context"
-msgstr "Odjave automatizacije marketinga"
+msgstr "Contexto Informes Automatización de marketing"
 
-#, fuzzy
 msgctxt "model:marketing.automation.reporting.scenario,name:"
 msgid "Marketing Automation Reporting Scenario"
-msgstr "Odjave automatizacije marketinga"
+msgstr "Informes Escenarios de automatización de marketing"
 
 msgctxt "model:marketing.automation.scenario,name:"
 msgid "Marketing Scenario"
-msgstr ""
+msgstr "Escenario de marketing"
 
 msgctxt "model:party.party-unsubscribed-marketing.automation.scenario,name:"
 msgid "Party Unsubscribed Scenario"
-msgstr ""
+msgstr "Escenarios de-suscritos del tercero"
 
 msgctxt "report:marketing.automation.unsubscribe:"
 msgid "Unsubscribe"
-msgstr ""
+msgstr "Darse de baja"
 
 msgctxt "report:marketing.automation.unsubscribe:"
 msgid ""
 "We are sorry to see you go, and apologize if we have overwhelmed your inbox."
 msgstr ""
+"Lamentamos verle marchar y le pedimos disculpas en caso que hubiéramos "
+"abusado de su bandeja de entrada de correo electrónico."
 
 msgctxt "report:marketing.automation.unsubscribe:"
 msgid "You are unsubscribed"
-msgstr ""
+msgstr "Te has dado de baja"
 
 msgctxt "report:marketing.automation.unsubscribe:"
 msgid "You have been successfully unsubscribed from this kind of email."
 msgstr ""
+"Se ha dado de baja de este tipo de correo electrónico satisfactoriamente."
 
 msgctxt "selection:ir.cron,method:"
 msgid "Process Marketing Activity"
-msgstr ""
+msgstr "Procesar actividad de marketing"
 
 msgctxt "selection:ir.cron,method:"
 msgid "Trigger Marketing Scenarios"
-msgstr ""
+msgstr "Ejecutar disparadores de escenarios de marketing"
 
 msgctxt "selection:marketing.automation.activity,action:"
 msgid "Send E-Mail"
-msgstr ""
+msgstr "Enviar correo electrónico"
 
 msgctxt "selection:marketing.automation.activity,event:"
 msgid "E-Mail Clicked"
-msgstr ""
+msgstr "Correo electrónico pulsado"
 
 msgctxt "selection:marketing.automation.activity,event:"
 msgid "E-Mail Opened"
-msgstr ""
+msgstr "Correo electrónico abierto"
 
 msgctxt "selection:marketing.automation.activity,on:"
 msgid "E-Mail Clicked"
-msgstr ""
+msgstr "Correo electrónico pulsado"
 
 msgctxt "selection:marketing.automation.activity,on:"
 msgid "E-Mail Not Clicked"
-msgstr ""
+msgstr "Correo electrónico no pulsado"
 
 msgctxt "selection:marketing.automation.activity,on:"
 msgid "E-Mail Not Opened"
-msgstr ""
+msgstr "Correo electrónico no abierto"
 
 msgctxt "selection:marketing.automation.activity,on:"
 msgid "E-Mail Opened"
-msgstr ""
+msgstr "Correo electrónico abierto"
 
 msgctxt "selection:marketing.automation.activity,parent:"
 msgid "Activity"
-msgstr ""
+msgstr "Actividad"
 
 msgctxt "selection:marketing.automation.activity,parent:"
 msgid "Scenario"
-msgstr ""
+msgstr "Escenario"
 
 msgctxt "selection:marketing.automation.record.activity,state:"
 msgid "Cancelled"
-msgstr ""
+msgstr "Cancelado"
 
 msgctxt "selection:marketing.automation.record.activity,state:"
 msgid "Done"
-msgstr ""
+msgstr "Finalizado"
 
 msgctxt "selection:marketing.automation.record.activity,state:"
 msgid "Waiting"
-msgstr ""
+msgstr "En espera"
 
-#, fuzzy
 msgctxt "selection:marketing.automation.reporting.context,period:"
 msgid "Day"
-msgstr "Zakasnitev"
+msgstr "Día"
 
 msgctxt "selection:marketing.automation.reporting.context,period:"
 msgid "Month"
-msgstr ""
+msgstr "Mes"
 
 msgctxt "selection:marketing.automation.reporting.context,period:"
 msgid "Year"
-msgstr ""
+msgstr "Año"
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Draft"
-msgstr ""
+msgstr "Borrador"
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Running"
-msgstr ""
+msgstr "En ejecución"
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Stopped"
-msgstr ""
+msgstr "Detenido"
 
 msgctxt "view:marketing.automation.activity:"
 msgid "%"
-msgstr ""
+msgstr "%"
 
 msgctxt "view:marketing.automation.activity:"
 msgid "After"
-msgstr ""
+msgstr "Después"
 
 msgctxt "view:marketing.automation.activity:"
 msgid "Edit"
-msgstr ""
+msgstr "Editar"
 
 msgctxt "view:marketing.automation.activity:"
 msgid "If"
-msgstr ""
+msgstr "Si"
 
 msgctxt "view:marketing.automation.activity:"
 msgid "On"
-msgstr ""
+msgstr "En"
 
 msgctxt "view:marketing.automation.activity:"
 msgid "Template:"
-msgstr ""
+msgstr "Plantilla:"
 
 msgctxt "view:marketing.automation.activity:"
 msgid "Title:"
-msgstr ""
+msgstr "Título:"
 
 msgctxt "view:marketing.automation.record.activity:"
 msgid "Time"
-msgstr ""
+msgstr "Hora"
 
 msgctxt "view:marketing.automation.reporting.activity:"
 msgid "%"
-msgstr ""
+msgstr "%"
 
 msgctxt "view:marketing.automation.reporting.scenario:"
 msgid "%"
-msgstr ""
+msgstr "%"
 
 msgctxt "view:marketing.automation.scenario:"
 msgid "%"
-msgstr ""
+msgstr "%"
 
 msgctxt "view:party.party:"
 msgid "Marketing Automation"
-msgstr ""
+msgstr "Automatización de marketing"
```

### Comparing `trytond_marketing_automation-7.2.0/locale/tr.po` & `trytond_marketing_automation-7.2.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-7.2.0/locale/uk.po` & `trytond_marketing_automation-7.2.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-7.2.0/locale/zh_CN.po` & `trytond_marketing_automation-7.2.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-7.2.0/marketing_automation.py` & `trytond_marketing_automation-7.2.1/marketing_automation.py`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-7.2.0/marketing_automation.xml` & `trytond_marketing_automation-7.2.1/marketing_automation.xml`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-7.2.0/marketing_automation_reporting.py` & `trytond_marketing_automation-7.2.1/marketing_automation_reporting.py`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-7.2.0/marketing_automation_reporting.xml` & `trytond_marketing_automation-7.2.1/marketing_automation_reporting.xml`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-7.2.0/message.xml` & `trytond_marketing_automation-7.2.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-7.2.0/mixin.py` & `trytond_marketing_automation-7.2.1/mixin.py`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-7.2.0/party.py` & `trytond_marketing_automation-7.2.1/party.py`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-7.2.0/routes.py` & `trytond_marketing_automation-7.2.1/routes.py`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-7.2.0/sale.py` & `trytond_marketing_automation-7.2.1/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-7.2.0/setup.py` & `trytond_marketing_automation-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-7.2.0/tests/scenario_marketing_automation.rst` & `trytond_marketing_automation-7.2.1/tests/scenario_marketing_automation.rst`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-7.2.0/tests/scenario_marketing_automation_unsubscribable.rst` & `trytond_marketing_automation-7.2.1/tests/scenario_marketing_automation_unsubscribable.rst`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-7.2.0/tox.ini` & `trytond_marketing_automation-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-7.2.0/trytond_marketing_automation.egg-info/PKG-INFO` & `trytond_marketing_automation-7.2.1/trytond_marketing_automation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_marketing_automation
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module to plan, coordinate and manage marketing campaigns
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_marketing_automation-7.2.0/trytond_marketing_automation.egg-info/SOURCES.txt` & `trytond_marketing_automation-7.2.1/trytond_marketing_automation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-7.2.0/unsubscribe.html` & `trytond_marketing_automation-7.2.1/unsubscribe.html`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-7.2.0/view/activity_form.xml` & `trytond_marketing_automation-7.2.1/view/activity_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-7.2.0/view/activity_tree.xml` & `trytond_marketing_automation-7.2.1/view/activity_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-7.2.0/view/record_activity_form.xml` & `trytond_marketing_automation-7.2.1/view/record_activity_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-7.2.0/view/reporting_activity_list.xml` & `trytond_marketing_automation-7.2.1/view/reporting_activity_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-7.2.0/view/scenario_form.xml` & `trytond_marketing_automation-7.2.1/view/scenario_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-7.2.0/web.py` & `trytond_marketing_automation-7.2.1/web.py`

 * *Files identical despite different names*

