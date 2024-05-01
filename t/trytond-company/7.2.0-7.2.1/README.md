# Comparing `tmp/trytond_company-7.2.0.tar.gz` & `tmp/trytond_company-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_company-7.2.0.tar", last modified: Mon Apr 29 15:39:21 2024, max compression
+gzip compressed data, was "trytond_company-7.2.1.tar", last modified: Wed May  1 12:00:23 2024, max compression
```

## Comparing `trytond_company-7.2.0.tar` & `trytond_company-7.2.1.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:21.971109 trytond_company-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     4545 2024-04-29 15:18:56.000000 trytond_company-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      728 2024-04-29 15:18:55.000000 trytond_company-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_company-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_company-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2759 2024-04-29 15:39:21.971109 trytond_company-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      379 2024-04-29 13:17:17.000000 trytond_company-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1078 2024-04-29 13:17:17.000000 trytond_company-7.2.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7587 2024-04-29 13:17:17.000000 trytond_company-7.2.0/company.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9118 2024-04-27 16:30:39.000000 trytond_company-7.2.0/company.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:21.967776 trytond_company-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3070 2024-04-27 16:30:39.000000 trytond_company-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2500 2023-04-15 07:12:15.000000 trytond_company-7.2.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      379 2024-04-29 13:17:17.000000 trytond_company-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2685 2024-02-04 18:51:26.000000 trytond_company-7.2.0/doc/reference.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_company-7.2.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:07.000000 trytond_company-7.2.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     1037 2024-04-13 17:12:23.000000 trytond_company-7.2.0/doc/usage.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:21.967776 trytond_company-7.2.0/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_company-7.2.0/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      351 2023-01-16 14:00:20.000000 trytond_company-7.2.0/icons/tryton-company.svg
--rw-r--r--   0 ced       (1000) ced       (1000)     4009 2024-04-29 13:17:17.000000 trytond_company-7.2.0/ir.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3039 2024-04-27 16:30:39.000000 trytond_company-7.2.0/ir.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    39343 2024-04-29 13:17:17.000000 trytond_company-7.2.0/letter.fodt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:21.971109 trytond_company-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     8064 2024-04-29 13:17:17.000000 trytond_company-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8352 2024-04-29 13:17:17.000000 trytond_company-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7166 2024-04-29 13:17:17.000000 trytond_company-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8651 2024-04-29 13:17:17.000000 trytond_company-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8430 2024-04-29 13:17:17.000000 trytond_company-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6894 2024-04-29 13:17:17.000000 trytond_company-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8171 2024-04-29 13:17:17.000000 trytond_company-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8958 2024-04-29 13:17:17.000000 trytond_company-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7166 2024-04-29 13:17:17.000000 trytond_company-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9095 2024-04-29 13:17:17.000000 trytond_company-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8141 2024-04-29 13:17:17.000000 trytond_company-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7955 2024-04-29 13:17:17.000000 trytond_company-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7690 2024-04-29 13:17:17.000000 trytond_company-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8935 2024-04-29 13:17:17.000000 trytond_company-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7694 2024-04-29 13:17:17.000000 trytond_company-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8402 2024-04-29 13:17:17.000000 trytond_company-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8240 2024-04-29 13:17:17.000000 trytond_company-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8236 2024-04-29 13:17:17.000000 trytond_company-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8371 2024-04-29 13:17:17.000000 trytond_company-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8351 2024-04-29 13:17:17.000000 trytond_company-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8177 2024-04-29 13:17:17.000000 trytond_company-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7166 2024-04-29 13:17:17.000000 trytond_company-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9489 2024-04-29 13:17:17.000000 trytond_company-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8010 2024-04-29 13:17:17.000000 trytond_company-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3538 2024-02-04 18:51:26.000000 trytond_company-7.2.0/model.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2814 2024-04-22 12:14:36.000000 trytond_company-7.2.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10152 2024-04-22 12:14:36.000000 trytond_company-7.2.0/res.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:39:21.971109 trytond_company-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4415 2024-04-29 13:17:17.000000 trytond_company-7.2.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:21.971109 trytond_company-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      396 2023-04-15 07:12:15.000000 trytond_company-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15063 2024-04-27 16:30:39.000000 trytond_company-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1219 2024-01-27 09:58:52.000000 trytond_company-7.2.0/tests/tools.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:07.000000 trytond_company-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      102 2024-04-29 15:18:51.000000 trytond_company-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:21.971109 trytond_company-7.2.0/trytond_company.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2759 2024-04-29 15:39:21.000000 trytond_company-7.2.0/trytond_company.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2034 2024-04-29 15:39:21.000000 trytond_company-7.2.0/trytond_company.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:39:21.000000 trytond_company-7.2.0/trytond_company.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       52 2024-04-29 15:39:21.000000 trytond_company-7.2.0/trytond_company.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:59.000000 trytond_company-7.2.0/trytond_company.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       85 2024-04-29 15:39:21.000000 trytond_company-7.2.0/trytond_company.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:39:21.000000 trytond_company-7.2.0/trytond_company.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:21.971109 trytond_company-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-01-16 14:00:20.000000 trytond_company-7.2.0/view/company_config_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      716 2024-04-29 13:17:17.000000 trytond_company-7.2.0/view/company_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      307 2023-04-15 07:12:15.000000 trytond_company-7.2.0/view/company_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      286 2023-04-15 07:12:15.000000 trytond_company-7.2.0/view/cron_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      476 2023-04-15 07:12:15.000000 trytond_company-7.2.0/view/employee_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      416 2023-04-15 07:12:15.000000 trytond_company-7.2.0/view/employee_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      339 2023-01-16 14:00:20.000000 trytond_company-7.2.0/view/sequence_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      322 2023-04-15 07:12:15.000000 trytond_company-7.2.0/view/sequence_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      652 2023-04-15 07:12:15.000000 trytond_company-7.2.0/view/user_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      606 2023-04-15 07:12:15.000000 trytond_company-7.2.0/view/user_form_preferences.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:00:23.735315 trytond_company-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4646 2024-05-01 12:00:20.000000 trytond_company-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      728 2024-05-01 12:00:20.000000 trytond_company-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:20:59.000000 trytond_company-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:20:59.000000 trytond_company-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2759 2024-05-01 12:00:23.735315 trytond_company-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      379 2024-04-30 17:20:59.000000 trytond_company-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1078 2024-04-30 17:20:59.000000 trytond_company-7.2.1/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7587 2024-04-30 17:20:59.000000 trytond_company-7.2.1/company.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9118 2024-04-30 17:20:59.000000 trytond_company-7.2.1/company.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:00:23.731982 trytond_company-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3070 2024-04-30 17:20:59.000000 trytond_company-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2500 2024-04-30 17:20:59.000000 trytond_company-7.2.1/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      379 2024-04-30 17:20:59.000000 trytond_company-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2685 2024-04-30 17:20:59.000000 trytond_company-7.2.1/doc/reference.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-30 17:20:59.000000 trytond_company-7.2.1/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:20:59.000000 trytond_company-7.2.1/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     1037 2024-04-30 17:20:59.000000 trytond_company-7.2.1/doc/usage.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:00:23.731982 trytond_company-7.2.1/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2024-04-30 17:20:59.000000 trytond_company-7.2.1/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      351 2024-04-30 17:20:59.000000 trytond_company-7.2.1/icons/tryton-company.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)     4009 2024-04-30 17:20:59.000000 trytond_company-7.2.1/ir.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3039 2024-04-30 17:20:59.000000 trytond_company-7.2.1/ir.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    39343 2024-04-30 17:20:59.000000 trytond_company-7.2.1/letter.fodt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:00:23.731982 trytond_company-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     8131 2024-04-30 17:21:59.000000 trytond_company-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8890 2024-04-30 17:21:59.000000 trytond_company-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7233 2024-04-30 17:21:59.000000 trytond_company-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9217 2024-04-30 17:21:59.000000 trytond_company-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8972 2024-04-30 17:21:59.000000 trytond_company-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6961 2024-04-30 17:21:59.000000 trytond_company-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8238 2024-04-30 17:21:59.000000 trytond_company-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9025 2024-04-30 17:21:59.000000 trytond_company-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7233 2024-04-30 17:21:59.000000 trytond_company-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9167 2024-04-30 17:21:59.000000 trytond_company-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8208 2024-04-30 17:21:59.000000 trytond_company-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8022 2024-04-30 17:21:59.000000 trytond_company-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7757 2024-04-30 17:21:59.000000 trytond_company-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9002 2024-04-30 17:21:59.000000 trytond_company-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7761 2024-04-30 17:21:59.000000 trytond_company-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8967 2024-04-30 17:21:59.000000 trytond_company-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8307 2024-04-30 17:21:59.000000 trytond_company-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8303 2024-04-30 17:21:59.000000 trytond_company-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8438 2024-04-30 17:21:59.000000 trytond_company-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8418 2024-04-30 17:21:59.000000 trytond_company-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8244 2024-04-30 17:21:59.000000 trytond_company-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7233 2024-04-30 17:21:59.000000 trytond_company-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9556 2024-04-30 17:21:59.000000 trytond_company-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8077 2024-04-30 17:21:59.000000 trytond_company-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3538 2024-04-30 17:20:59.000000 trytond_company-7.2.1/model.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2814 2024-04-30 17:20:59.000000 trytond_company-7.2.1/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10152 2024-04-30 17:20:59.000000 trytond_company-7.2.1/res.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 12:00:23.735315 trytond_company-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4415 2024-04-30 17:20:59.000000 trytond_company-7.2.1/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:00:23.735315 trytond_company-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      396 2024-04-30 17:20:59.000000 trytond_company-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15063 2024-04-30 17:20:59.000000 trytond_company-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1219 2024-04-30 17:20:59.000000 trytond_company-7.2.1/tests/tools.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:20:59.000000 trytond_company-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      102 2024-04-30 17:21:06.000000 trytond_company-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:00:23.735315 trytond_company-7.2.1/trytond_company.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2759 2024-05-01 12:00:23.000000 trytond_company-7.2.1/trytond_company.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2034 2024-05-01 12:00:23.000000 trytond_company-7.2.1/trytond_company.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:00:23.000000 trytond_company-7.2.1/trytond_company.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       52 2024-05-01 12:00:23.000000 trytond_company-7.2.1/trytond_company.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:00:23.000000 trytond_company-7.2.1/trytond_company.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       85 2024-05-01 12:00:23.000000 trytond_company-7.2.1/trytond_company.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 12:00:23.000000 trytond_company-7.2.1/trytond_company.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:00:23.735315 trytond_company-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      371 2024-04-30 17:20:59.000000 trytond_company-7.2.1/view/company_config_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      716 2024-04-30 17:20:59.000000 trytond_company-7.2.1/view/company_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      307 2024-04-30 17:20:59.000000 trytond_company-7.2.1/view/company_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      286 2024-04-30 17:20:59.000000 trytond_company-7.2.1/view/cron_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      476 2024-04-30 17:20:59.000000 trytond_company-7.2.1/view/employee_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      416 2024-04-30 17:20:59.000000 trytond_company-7.2.1/view/employee_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      339 2024-04-30 17:20:59.000000 trytond_company-7.2.1/view/sequence_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      322 2024-04-30 17:20:59.000000 trytond_company-7.2.1/view/sequence_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      652 2024-04-30 17:20:59.000000 trytond_company-7.2.1/view/user_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      606 2024-04-30 17:20:59.000000 trytond_company-7.2.1/view/user_form_preferences.xml
```

### Comparing `trytond_company-7.2.0/CHANGELOG` & `trytond_company-7.2.1/CHANGELOG`

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
 * Activate employee based on dates
 * Use template substitution for company header/footer
 
 Version 7.0.0 - 2023-10-30
```

### Comparing `trytond_company-7.2.0/COPYRIGHT` & `trytond_company-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_company-7.2.0/LICENSE` & `trytond_company-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_company-7.2.0/PKG-INFO` & `trytond_company-7.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_company
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module with companies and employees
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_company-7.2.0/__init__.py` & `trytond_company-7.2.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_company-7.2.0/company.py` & `trytond_company-7.2.1/company.py`

 * *Files identical despite different names*

### Comparing `trytond_company-7.2.0/company.xml` & `trytond_company-7.2.1/company.xml`

 * *Files identical despite different names*

### Comparing `trytond_company-7.2.0/doc/conf.py` & `trytond_company-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_company-7.2.0/doc/design.rst` & `trytond_company-7.2.1/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_company-7.2.0/doc/reference.rst` & `trytond_company-7.2.1/doc/reference.rst`

 * *Files identical despite different names*

### Comparing `trytond_company-7.2.0/doc/usage.rst` & `trytond_company-7.2.1/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `trytond_company-7.2.0/icons/LICENSE` & `trytond_company-7.2.1/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_company-7.2.0/ir.py` & `trytond_company-7.2.1/ir.py`

 * *Files identical despite different names*

### Comparing `trytond_company-7.2.0/ir.xml` & `trytond_company-7.2.1/ir.xml`

 * *Files identical despite different names*

### Comparing `trytond_company-7.2.0/letter.fodt` & `trytond_company-7.2.1/letter.fodt`

 * *Files identical despite different names*

### Comparing `trytond_company-7.2.0/locale/bg.po` & `trytond_company-7.2.1/locale/bg.po`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,18 @@
 msgstr "Партньор"
 
 #, fuzzy
 msgctxt "field:company.company,timezone:"
 msgid "Timezone"
 msgstr "Времева зона"
 
+msgctxt "field:company.employee,active:"
+msgid "Active"
+msgstr ""
+
 msgctxt "field:company.employee,company:"
 msgid "Company"
 msgstr "Фирма"
 
 msgctxt "field:company.employee,end_date:"
 msgid "End Date"
 msgstr ""
```

### Comparing `trytond_company-7.2.0/locale/ca.po` & `trytond_company-7.2.1/locale/es.po`

 * *Files 6% similar despite different names*

```diff
@@ -4,67 +4,71 @@
 
 msgctxt "field:company.company,currency:"
 msgid "Currency"
 msgstr "Moneda"
 
 msgctxt "field:company.company,employees:"
 msgid "Employees"
-msgstr "Empleats"
+msgstr "Empleados"
 
 msgctxt "field:company.company,footer:"
 msgid "Footer"
-msgstr "Peu de pàgina"
+msgstr "Pie de página"
 
 msgctxt "field:company.company,header:"
 msgid "Header"
-msgstr "Capçalera"
+msgstr "Encabezado"
 
 msgctxt "field:company.company,party:"
 msgid "Party"
-msgstr "Tercer"
+msgstr "Tercero"
 
 msgctxt "field:company.company,timezone:"
 msgid "Timezone"
-msgstr "Zona horària"
+msgstr "Zona horaria"
+
+msgctxt "field:company.employee,active:"
+msgid "Active"
+msgstr "Activo"
 
 msgctxt "field:company.employee,company:"
 msgid "Company"
 msgstr "Empresa"
 
 msgctxt "field:company.employee,end_date:"
 msgid "End Date"
-msgstr "Data finalització"
+msgstr "Fecha finalización"
 
 msgctxt "field:company.employee,party:"
 msgid "Party"
-msgstr "Tercer"
+msgstr "Tercero"
 
 msgctxt "field:company.employee,start_date:"
 msgid "Start Date"
-msgstr "Data d'inici"
+msgstr "Fecha Inicio"
 
 msgctxt "field:company.employee,subordinates:"
 msgid "Subordinates"
-msgstr "Subordinats"
+msgstr "Subordinados"
 
 msgctxt "field:company.employee,supervisor:"
 msgid "Supervisor"
 msgstr "Supervisor"
 
 msgctxt "field:ir.cron,companies:"
 msgid "Companies"
-msgstr "Empreses"
+msgstr "Empresas"
 
 msgctxt "field:ir.cron-company.company,company:"
 msgid "Company"
 msgstr "Empresa"
 
 msgctxt "field:ir.cron-company.company,cron:"
 msgid "Cron"
-msgstr "Planificador de tasques"
+msgstr "Planificador de tareas"
 
 msgctxt "field:ir.sequence,company:"
 msgid "Company"
 msgstr "Empresa"
 
 msgctxt "field:ir.sequence.strict,company:"
 msgid "Company"
@@ -80,264 +84,284 @@
 
 msgctxt "field:party.party.lang,company:"
 msgid "Company"
 msgstr "Empresa"
 
 msgctxt "field:res.user,companies:"
 msgid "Companies"
-msgstr "Empreses"
+msgstr "Empresas"
 
 msgctxt "field:res.user,company:"
 msgid "Current Company"
 msgstr "Empresa actual"
 
 msgctxt "field:res.user,company_filter:"
 msgid "Company Filter"
-msgstr "Filtre empresa"
+msgstr "Filtro de empresa"
 
 msgctxt "field:res.user,employee:"
 msgid "Current Employee"
-msgstr "Empleat"
+msgstr "Empleado actual"
 
 msgctxt "field:res.user,employees:"
 msgid "Employees"
-msgstr "Empleats"
+msgstr "Empleados"
 
 msgctxt "field:res.user-company.company,company:"
 msgid "Company"
 msgstr "Empresa"
 
 msgctxt "field:res.user-company.company,user:"
 msgid "User"
-msgstr "Usuari"
+msgstr "Usuario"
 
 msgctxt "field:res.user-company.employee,employee:"
 msgid "Employee"
-msgstr "Empleat"
+msgstr "Empleado"
 
 msgctxt "field:res.user-company.employee,user:"
 msgid "User"
-msgstr "Usuari"
+msgstr "Usuario"
 
 msgctxt "help:company.company,currency:"
 msgid "The main currency for the company."
-msgstr "La moneda principal de l'empresa."
+msgstr "La moneda principal de la empresa."
 
 msgctxt "help:company.company,employees:"
 msgid "Add employees to the company."
-msgstr "Afegiu empleats a l'empresa."
+msgstr "Añade empleados a la empresa."
 
 msgctxt "help:company.company,footer:"
 msgid ""
 "The text to display on report footers.\n"
 "The following placeholders can be used:\n"
 "- ${name}\n"
 "- ${phone}\n"
 "- ${mobile}\n"
 "- ${fax}\n"
 "- ${email}\n"
 "- ${website}\n"
 "- ${address}\n"
 "- ${tax_identifier}\n"
 msgstr ""
+"Texto a mostrar en el pie de pagina de los informes.\n"
+"Se pueden usar las siguientes sustituciones:\n"
+"- ${name}\n"
+"- ${phone}\n"
+"- ${mobile}\n"
+"- ${fax}\n"
+"- ${email}\n"
+"- ${website}\n"
+"- ${address}\n"
+"- ${tax_identifier}\n"
 
 msgctxt "help:company.company,header:"
 msgid ""
 "The text to display on report headers.\n"
 "The following placeholders can be used:\n"
 "- ${name}\n"
 "- ${phone}\n"
 "- ${mobile}\n"
 "- ${fax}\n"
 "- ${email}\n"
 "- ${website}\n"
 "- ${address}\n"
 "- ${tax_identifier}\n"
 msgstr ""
+"Texto a mostrar en la cabecera de los informes.\n"
+"Se pueden usar las siguientes sustituciones:\n"
+"- ${name}\n"
+"- ${phone}\n"
+"- ${mobile}\n"
+"- ${fax}\n"
+"- ${email}\n"
+"- ${website}\n"
+"- ${address}\n"
+"- ${tax_identifier}\n"
 
 msgctxt "help:company.company,timezone:"
 msgid "Used to compute the today date."
-msgstr "Utilitzat per calcular la data d'avui."
+msgstr "Utilizado para calcular la fecha de hoy."
 
 msgctxt "help:company.employee,company:"
 msgid "The company to which the employee belongs."
-msgstr "L'empresa a la que pertany l'empleat."
+msgstr "La empresa a la que pertenece el empleado."
 
 msgctxt "help:company.employee,end_date:"
 msgid "When the employee leaves the company."
-msgstr "Quan l'empleat marxa de l'empresa."
+msgstr "Cuando el empleado se va de la empresa."
 
 msgctxt "help:company.employee,party:"
 msgid "The party which represents the employee."
-msgstr "El tercer que representa l'empleat."
+msgstr "El tercero que representa el empleado."
 
 msgctxt "help:company.employee,start_date:"
 msgid "When the employee joins the company."
-msgstr "Quan l'empleat entra a l'empresa."
+msgstr "Cuando el empleado entra en la empresa."
 
 msgctxt "help:company.employee,subordinates:"
 msgid "The employees to be overseen by this employee."
-msgstr "Els empleats que són supervisats per aquest empleat."
+msgstr "Los empleados que són supervisados por este empleado."
 
 msgctxt "help:company.employee,supervisor:"
 msgid "The employee who oversees this employee."
-msgstr "L'empleat que supervisa aquest empleat."
+msgstr "El empleado que supervisa este empleado."
 
 msgctxt "help:ir.cron,companies:"
 msgid "Companies registered for this cron."
-msgstr "Empreses registrades per aquest planificador."
+msgstr "Empresas registradas para este planificador."
 
 msgctxt "help:ir.rule,domain:"
 msgid ""
 "\n"
 "- \"companies\" as list of ids from the current user"
 msgstr ""
 "\n"
-"- \"companies\" com una llista de ids de les empreses del usuari actual"
+"- \"companies\" como una lista de ids de la empresas del usuario actual"
 
 msgctxt "help:ir.sequence,company:"
 msgid "Restricts the sequence usage to the company."
-msgstr "Restringeix l'ús de la seqüencia a l'empresa."
+msgstr "Restringir el uso de la secuencia para la empresa."
 
 msgctxt "help:ir.sequence.strict,company:"
 msgid "Restricts the sequence usage to the company."
-msgstr "Restringeix l'ús de la seqüencia a l'empresa."
+msgstr "Restringir el uso de la secuencia para la empresa."
 
 msgctxt "help:res.user,companies:"
 msgid "The companies that the user has access to."
-msgstr "Les empreses a les que té accés l'usuari."
+msgstr "Las empresas a las que tiene acceso el usuario."
 
 msgctxt "help:res.user,company:"
 msgid "Select the company to work for."
-msgstr "Seleccioneu l'empresa en la que voleu treballar."
+msgstr "Seleccionar la empresa en la que se quiere trabajar."
 
 msgctxt "help:res.user,company_filter:"
 msgid "Define records of which companies are shown."
-msgstr "Defineix els registres de quines empreses es mostren."
+msgstr "Define los registros de que empresas se muestran."
 
 msgctxt "help:res.user,employee:"
 msgid "Select the employee to make the user behave as such."
-msgstr "Seleccioneu l'empleat com al que es comportarà l'usuari."
+msgstr "Seleccionar el empleado para que el usuario se comporte como tal."
 
 msgctxt "help:res.user,employees:"
 msgid "Add employees to grant the user access to them."
-msgstr "Afegeix empleats als que podrà accedir l'usuari."
+msgstr "Añadir empleados a los que podrá acceder el usuario."
 
 msgctxt "model:company.company,name:"
 msgid "Company"
 msgstr "Empresa"
 
 msgctxt "model:company.company.config.start,name:"
 msgid "Company Config"
-msgstr "Configuració empresa"
+msgstr "Configuración empresa"
 
 msgctxt "model:company.employee,name:"
 msgid "Employee"
-msgstr "Empleat"
+msgstr "Empleado"
 
 msgctxt "model:ir.action,name:act_company_config"
 msgid "Configure Company"
-msgstr "Configura l'empresa"
+msgstr "Configurar la empresa"
 
 msgctxt "model:ir.action,name:act_company_list"
 msgid "Companies"
-msgstr "Empreses"
+msgstr "Empresas"
 
 msgctxt "model:ir.action,name:act_employee_form"
 msgid "Employees"
-msgstr "Empleats"
+msgstr "Empleados"
 
 msgctxt "model:ir.action,name:act_employee_subordinates"
 msgid "Supervised by"
-msgstr "Supervisat per"
+msgstr "Supervisador por"
 
 msgctxt "model:ir.action,name:report_letter"
 msgid "Letter"
 msgstr "Carta"
 
 msgctxt "model:ir.cron-company.company,name:"
 msgid "Cron - Company"
 msgstr "Planificador - Empresa"
 
 msgctxt "model:ir.rule.group,name:rule_group_sequence_companies"
 msgid "User in companies"
-msgstr "Usuari a les empreses"
+msgstr "Usuario en las empresas"
 
 msgctxt "model:ir.rule.group,name:rule_group_sequence_strict_companies"
 msgid "User in companies"
-msgstr "Usuari a les empreses"
+msgstr "Usuario en las empresas"
 
 msgctxt "model:ir.ui.menu,name:menu_company"
 msgid "Companies"
-msgstr "Empreses"
+msgstr "Empresas"
 
 msgctxt "model:ir.ui.menu,name:menu_company_list"
 msgid "Companies"
-msgstr "Empreses"
+msgstr "Empresas"
 
 msgctxt "model:ir.ui.menu,name:menu_employee_form"
 msgid "Employees"
-msgstr "Empleats"
+msgstr "Empleados"
 
 msgctxt "model:res.group,name:group_company_admin"
 msgid "Company Administration"
-msgstr "Administració d'empreses"
+msgstr "Administración empresas"
 
 msgctxt "model:res.group,name:group_employee_admin"
 msgid "Employee Administration"
-msgstr "Administració d'empleats"
+msgstr "Administración empleados"
 
 msgctxt "model:res.user-company.company,name:"
 msgid "User - Company"
-msgstr "Usuari - Empresa"
+msgstr "Usuario - Empresa"
 
 msgctxt "model:res.user-company.employee,name:"
 msgid "User - Employee"
-msgstr "Usuari - Emprat"
+msgstr "Usuario - Empleado"
 
 msgctxt "report:party.letter:"
 msgid "Best Regards,"
-msgstr "Atentament,"
+msgstr "Atentamente,"
 
 msgctxt "report:party.letter:"
 msgid "Date:"
-msgstr "Data:"
+msgstr "Fecha:"
 
 msgctxt "report:party.letter:"
 msgid "Dear Madams and Sirs,"
-msgstr "Estimats senyors i senyores,"
+msgstr "Estimados señores y señoras,"
 
 msgctxt "report:party.letter:"
 msgid "Subject:"
-msgstr "Assumpte:"
+msgstr "Asunto:"
 
 msgctxt "selection:res.user,company_filter:"
 msgid "All"
-msgstr "Totes"
+msgstr "Todas"
 
 msgctxt "selection:res.user,company_filter:"
 msgid "Current"
 msgstr "Actual"
 
 msgctxt "view:company.company.config.start:"
 msgid "You can now add your company into the system."
-msgstr "Ara podeu afegir la vostra empresa al sistema."
+msgstr "Ahora puede añadir su empresa en el sistema."
 
 msgctxt "view:company.company:"
 msgid "Reports"
 msgstr "Informes"
 
 msgctxt "wizard_button:company.company.config,company,add:"
 msgid "Add"
-msgstr "Afegeix"
+msgstr "Añadir"
 
 msgctxt "wizard_button:company.company.config,company,end:"
 msgid "Cancel"
-msgstr "Cancel·la"
+msgstr "Cancelar"
 
 msgctxt "wizard_button:company.company.config,start,company:"
 msgid "OK"
-msgstr "D'acord"
+msgstr "Aceptar"
 
 msgctxt "wizard_button:company.company.config,start,end:"
 msgid "Cancel"
-msgstr "Cancel·la"
+msgstr "Cancelar"
```

### Comparing `trytond_company-7.2.0/locale/cs.po` & `trytond_company-7.2.1/locale/cs.po`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,18 @@
 msgid "Party"
 msgstr ""
 
 msgctxt "field:company.company,timezone:"
 msgid "Timezone"
 msgstr ""
 
+msgctxt "field:company.employee,active:"
+msgid "Active"
+msgstr ""
+
 msgctxt "field:company.employee,company:"
 msgid "Company"
 msgstr ""
 
 msgctxt "field:company.employee,end_date:"
 msgid "End Date"
 msgstr ""
```

### Comparing `trytond_company-7.2.0/locale/de.po` & `trytond_company-7.2.1/locale/de.po`

 * *Files 7% similar despite different names*

```diff
@@ -22,14 +22,18 @@
 msgid "Party"
 msgstr "Partei"
 
 msgctxt "field:company.company,timezone:"
 msgid "Timezone"
 msgstr "Zeitzone"
 
+msgctxt "field:company.employee,active:"
+msgid "Active"
+msgstr "Aktiv"
+
 msgctxt "field:company.employee,company:"
 msgid "Company"
 msgstr "Unternehmen"
 
 msgctxt "field:company.employee,end_date:"
 msgid "End Date"
 msgstr "Enddatum"
@@ -135,32 +139,52 @@
 "- ${mobile}\n"
 "- ${fax}\n"
 "- ${email}\n"
 "- ${website}\n"
 "- ${address}\n"
 "- ${tax_identifier}\n"
 msgstr ""
+"Der Text der in den Fußzeilen von Berichten angezeigt wird.\n"
+"Es stehen folgende Platzhalter zur Verfügung:\n"
+"- ${name}\n"
+"- ${phone}\n"
+"- ${mobile}\n"
+"- ${fax}\n"
+"- ${email}\n"
+"- ${website}\n"
+"- ${address}\n"
+"- ${tax_identifier}\n"
 
 msgctxt "help:company.company,header:"
 msgid ""
 "The text to display on report headers.\n"
 "The following placeholders can be used:\n"
 "- ${name}\n"
 "- ${phone}\n"
 "- ${mobile}\n"
 "- ${fax}\n"
 "- ${email}\n"
 "- ${website}\n"
 "- ${address}\n"
 "- ${tax_identifier}\n"
 msgstr ""
+"Der Text der in den Kopfzeilen von Berichten angezeigt wird.\n"
+"Es stehen folgende Platzhalter zur Verfügung:\n"
+"- ${name}\n"
+"- ${phone}\n"
+"- ${mobile}\n"
+"- ${fax}\n"
+"- ${email}\n"
+"- ${website}\n"
+"- ${address}\n"
+"- ${tax_identifier}\n"
 
 msgctxt "help:company.company,timezone:"
 msgid "Used to compute the today date."
-msgstr "Wird zum berechnen des heutigen Datums verwendet."
+msgstr "Wird zum Berechnen des heutigen Datums verwendet."
 
 msgctxt "help:company.employee,company:"
 msgid "The company to which the employee belongs."
 msgstr "Das Unternehmen dem der Mitarbeiter angehört."
 
 msgctxt "help:company.employee,end_date:"
 msgid "When the employee leaves the company."
@@ -256,19 +280,19 @@
 
 msgctxt "model:ir.cron-company.company,name:"
 msgid "Cron - Company"
 msgstr "Zeitplaner - Unternehmen"
 
 msgctxt "model:ir.rule.group,name:rule_group_sequence_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.rule.group,name:rule_group_sequence_strict_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.ui.menu,name:menu_company"
 msgid "Companies"
 msgstr "Unternehmen"
 
 msgctxt "model:ir.ui.menu,name:menu_company_list"
 msgid "Companies"
```

### Comparing `trytond_company-7.2.0/locale/es.po` & `trytond_company-7.2.1/locale/nl.po`

 * *Files 8% similar despite different names*

```diff
@@ -1,343 +1,367 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:company.company,currency:"
 msgid "Currency"
-msgstr "Moneda"
+msgstr "Valuta"
 
 msgctxt "field:company.company,employees:"
 msgid "Employees"
-msgstr "Empleados"
+msgstr "Werknemers"
 
 msgctxt "field:company.company,footer:"
 msgid "Footer"
-msgstr "Pie de página"
+msgstr "Voettekst"
 
 msgctxt "field:company.company,header:"
 msgid "Header"
-msgstr "Encabezado"
+msgstr "Koptekst"
 
 msgctxt "field:company.company,party:"
 msgid "Party"
-msgstr "Tercero"
+msgstr "Relatie"
 
 msgctxt "field:company.company,timezone:"
 msgid "Timezone"
-msgstr "Zona horaria"
+msgstr "Tijdzone"
+
+msgctxt "field:company.employee,active:"
+msgid "Active"
+msgstr "Actief"
 
 msgctxt "field:company.employee,company:"
 msgid "Company"
-msgstr "Empresa"
+msgstr "Bedrijf"
 
 msgctxt "field:company.employee,end_date:"
 msgid "End Date"
-msgstr "Fecha finalización"
+msgstr "Eind datum"
 
 msgctxt "field:company.employee,party:"
 msgid "Party"
-msgstr "Tercero"
+msgstr "Relatie"
 
 msgctxt "field:company.employee,start_date:"
 msgid "Start Date"
-msgstr "Fecha Inicio"
+msgstr "Start Datum"
 
 msgctxt "field:company.employee,subordinates:"
 msgid "Subordinates"
-msgstr "Subordinados"
+msgstr "Ondergeschikten"
 
 msgctxt "field:company.employee,supervisor:"
 msgid "Supervisor"
-msgstr "Supervisor"
+msgstr "Leidinggevende"
 
 msgctxt "field:ir.cron,companies:"
 msgid "Companies"
-msgstr "Empresas"
+msgstr "Bedrijven"
 
 msgctxt "field:ir.cron-company.company,company:"
 msgid "Company"
-msgstr "Empresa"
+msgstr "Bedrijf"
 
 msgctxt "field:ir.cron-company.company,cron:"
 msgid "Cron"
-msgstr "Planificador de tareas"
+msgstr "Planner"
 
 msgctxt "field:ir.sequence,company:"
 msgid "Company"
-msgstr "Empresa"
+msgstr "Bedrijf"
 
 msgctxt "field:ir.sequence.strict,company:"
 msgid "Company"
-msgstr "Empresa"
+msgstr "Bedrijf"
 
 msgctxt "field:party.configuration.party_lang,company:"
 msgid "Company"
-msgstr "Empresa"
+msgstr "Bedrijf"
 
 msgctxt "field:party.contact_mechanism.language,company:"
 msgid "Company"
-msgstr "Empresa"
+msgstr "Bedrijf"
 
 msgctxt "field:party.party.lang,company:"
 msgid "Company"
-msgstr "Empresa"
+msgstr "Bedrijf"
 
 msgctxt "field:res.user,companies:"
 msgid "Companies"
-msgstr "Empresas"
+msgstr "Bedrijven"
 
 msgctxt "field:res.user,company:"
 msgid "Current Company"
-msgstr "Empresa actual"
+msgstr "Huidig bedrijf"
 
 msgctxt "field:res.user,company_filter:"
 msgid "Company Filter"
-msgstr "Filtro de empresa"
+msgstr "Bedrijfsfilter"
 
 msgctxt "field:res.user,employee:"
 msgid "Current Employee"
-msgstr "Empleado actual"
+msgstr "Huidige werknemer"
 
 msgctxt "field:res.user,employees:"
 msgid "Employees"
-msgstr "Empleados"
+msgstr "Werknemers"
 
 msgctxt "field:res.user-company.company,company:"
 msgid "Company"
-msgstr "Empresa"
+msgstr "Bedrijf"
 
 msgctxt "field:res.user-company.company,user:"
 msgid "User"
-msgstr "Usuario"
+msgstr "Gebruiker"
 
 msgctxt "field:res.user-company.employee,employee:"
 msgid "Employee"
-msgstr "Empleado"
+msgstr "Werknemer"
 
 msgctxt "field:res.user-company.employee,user:"
 msgid "User"
-msgstr "Usuario"
+msgstr "Gebruiker"
 
 msgctxt "help:company.company,currency:"
 msgid "The main currency for the company."
-msgstr "La moneda principal de la empresa."
+msgstr "De hoofd-valuta voor het bedrijf."
 
 msgctxt "help:company.company,employees:"
 msgid "Add employees to the company."
-msgstr "Añade empleados a la empresa."
+msgstr "Voeg medewerkers toe aan het bedrijf."
 
 msgctxt "help:company.company,footer:"
 msgid ""
 "The text to display on report footers.\n"
 "The following placeholders can be used:\n"
 "- ${name}\n"
 "- ${phone}\n"
 "- ${mobile}\n"
 "- ${fax}\n"
 "- ${email}\n"
 "- ${website}\n"
 "- ${address}\n"
 "- ${tax_identifier}\n"
 msgstr ""
+"De tekst die in de rapport footer kan worden weergegeven.\n"
+"De volgende aanduidingen kunnen gebruikt worden:\n"
+"- ${name}\n"
+"- ${phone}\n"
+"- ${mobile}\n"
+"- ${fax}\n"
+"- ${email}\n"
+"- ${website}\n"
+"- ${address}\n"
+"- ${tax_identifier}\n"
 
 msgctxt "help:company.company,header:"
 msgid ""
 "The text to display on report headers.\n"
 "The following placeholders can be used:\n"
 "- ${name}\n"
 "- ${phone}\n"
 "- ${mobile}\n"
 "- ${fax}\n"
 "- ${email}\n"
 "- ${website}\n"
 "- ${address}\n"
 "- ${tax_identifier}\n"
 msgstr ""
+"De tekst die in de rapport header kan worden weergegeven.\n"
+"De volgende aanduidingen kunnen gebruikt worden:\n"
+"- ${name}\n"
+"- ${phone}\n"
+"- ${mobile}\n"
+"- ${fax}\n"
+"- ${email}\n"
+"- ${website}\n"
+"- ${address}\n"
+"- ${tax_identifier}\n"
 
 msgctxt "help:company.company,timezone:"
 msgid "Used to compute the today date."
-msgstr "Utilizado para calcular la fecha de hoy."
+msgstr "Gebruikt om de datum van vandaag te berekenen."
 
 msgctxt "help:company.employee,company:"
 msgid "The company to which the employee belongs."
-msgstr "La empresa a la que pertenece el empleado."
+msgstr "Het bedrijf waartoe de werknemer behoort."
 
 msgctxt "help:company.employee,end_date:"
 msgid "When the employee leaves the company."
-msgstr "Cuando el empleado se va de la empresa."
+msgstr "Wanneer de werknemer uit dienst treedt."
 
 msgctxt "help:company.employee,party:"
 msgid "The party which represents the employee."
-msgstr "El tercero que representa el empleado."
+msgstr "De relatie die de werknemer weergeeft."
 
 msgctxt "help:company.employee,start_date:"
 msgid "When the employee joins the company."
-msgstr "Cuando el empleado entra en la empresa."
+msgstr "Wanneer de werknemer in dienst treedt."
 
 msgctxt "help:company.employee,subordinates:"
 msgid "The employees to be overseen by this employee."
-msgstr "Los empleados que són supervisados por este empleado."
+msgstr "De werknemers waar deze werknemer leiding aan geeft."
 
 msgctxt "help:company.employee,supervisor:"
 msgid "The employee who oversees this employee."
-msgstr "El empleado que supervisa este empleado."
+msgstr "De werknemer die leiding geeft aan deze werknemer."
 
 msgctxt "help:ir.cron,companies:"
 msgid "Companies registered for this cron."
-msgstr "Empresas registradas para este planificador."
+msgstr "Bedrijven aangesloten op deze planner."
 
 msgctxt "help:ir.rule,domain:"
 msgid ""
 "\n"
 "- \"companies\" as list of ids from the current user"
 msgstr ""
 "\n"
-"- \"companies\" como una lista de ids de la empresas del usuario actual"
+"- \"bedrijven\" als een lijst met ID's van de huidige gebruiker"
 
 msgctxt "help:ir.sequence,company:"
 msgid "Restricts the sequence usage to the company."
-msgstr "Restringir el uso de la secuencia para la empresa."
+msgstr "Beperkt het gebruik van de reeks tot het bedrijf."
 
 msgctxt "help:ir.sequence.strict,company:"
 msgid "Restricts the sequence usage to the company."
-msgstr "Restringir el uso de la secuencia para la empresa."
+msgstr "Beperkt het gebruik van de reeks tot het bedrijf."
 
 msgctxt "help:res.user,companies:"
 msgid "The companies that the user has access to."
-msgstr "Las empresas a las que tiene acceso el usuario."
+msgstr "De bedrijven waar de gebruiker toegang tot heeft."
 
 msgctxt "help:res.user,company:"
 msgid "Select the company to work for."
-msgstr "Seleccionar la empresa en la que se quiere trabajar."
+msgstr "Selecteer het bedrijf om voor te werken."
 
 msgctxt "help:res.user,company_filter:"
 msgid "Define records of which companies are shown."
-msgstr "Define los registros de que empresas se muestran."
+msgstr "Leg vast welke bedrijven worden getoond."
 
 msgctxt "help:res.user,employee:"
 msgid "Select the employee to make the user behave as such."
-msgstr "Seleccionar el empleado para que el usuario se comporte como tal."
+msgstr "Selecteer de medewerker zodat de gebruiker zich als zodanig gedraagt."
 
 msgctxt "help:res.user,employees:"
 msgid "Add employees to grant the user access to them."
-msgstr "Añadir empleados a los que podrá acceder el usuario."
+msgstr "Voeg de werknemers toe die toegestaan voor de gebruiker."
 
 msgctxt "model:company.company,name:"
 msgid "Company"
-msgstr "Empresa"
+msgstr "Bedrijf"
 
 msgctxt "model:company.company.config.start,name:"
 msgid "Company Config"
-msgstr "Configuración empresa"
+msgstr "Bedrijf configuratie"
 
 msgctxt "model:company.employee,name:"
 msgid "Employee"
-msgstr "Empleado"
+msgstr "Werknemer"
 
 msgctxt "model:ir.action,name:act_company_config"
 msgid "Configure Company"
-msgstr "Configurar la empresa"
+msgstr "Bedrijf configureren"
 
 msgctxt "model:ir.action,name:act_company_list"
 msgid "Companies"
-msgstr "Empresas"
+msgstr "Bedrijven"
 
 msgctxt "model:ir.action,name:act_employee_form"
 msgid "Employees"
-msgstr "Empleados"
+msgstr "Werknemers"
 
 msgctxt "model:ir.action,name:act_employee_subordinates"
 msgid "Supervised by"
-msgstr "Supervisador por"
+msgstr "Onder leiding van"
 
 msgctxt "model:ir.action,name:report_letter"
 msgid "Letter"
-msgstr "Carta"
+msgstr "Brief"
 
 msgctxt "model:ir.cron-company.company,name:"
 msgid "Cron - Company"
-msgstr "Planificador - Empresa"
+msgstr "Planner - Bedrijf"
 
 msgctxt "model:ir.rule.group,name:rule_group_sequence_companies"
 msgid "User in companies"
-msgstr "Usuario en las empresas"
+msgstr "Gebruiker in bedrijven"
 
 msgctxt "model:ir.rule.group,name:rule_group_sequence_strict_companies"
 msgid "User in companies"
-msgstr "Usuario en las empresas"
+msgstr "Gebruiker in bedrijven"
 
 msgctxt "model:ir.ui.menu,name:menu_company"
 msgid "Companies"
-msgstr "Empresas"
+msgstr "Bedrijven"
 
 msgctxt "model:ir.ui.menu,name:menu_company_list"
 msgid "Companies"
-msgstr "Empresas"
+msgstr "Bedrijven"
 
 msgctxt "model:ir.ui.menu,name:menu_employee_form"
 msgid "Employees"
-msgstr "Empleados"
+msgstr "Werknemers"
 
 msgctxt "model:res.group,name:group_company_admin"
 msgid "Company Administration"
-msgstr "Administración empresas"
+msgstr "Bedrijf administratie"
 
 msgctxt "model:res.group,name:group_employee_admin"
 msgid "Employee Administration"
-msgstr "Administración empleados"
+msgstr "Werknemer administratie"
 
 msgctxt "model:res.user-company.company,name:"
 msgid "User - Company"
-msgstr "Usuario - Empresa"
+msgstr "Gebruiker in het bedrijf"
 
 msgctxt "model:res.user-company.employee,name:"
 msgid "User - Employee"
-msgstr "Usuario - Empleado"
+msgstr "Gebruiker - Werknemer"
 
 msgctxt "report:party.letter:"
 msgid "Best Regards,"
-msgstr "Atentamente,"
+msgstr "Met vriendelijke groet,"
 
 msgctxt "report:party.letter:"
 msgid "Date:"
-msgstr "Fecha:"
+msgstr "Datum:"
 
 msgctxt "report:party.letter:"
 msgid "Dear Madams and Sirs,"
-msgstr "Estimados señores y señoras,"
+msgstr "Geachte heer/mevrouw,"
 
 msgctxt "report:party.letter:"
 msgid "Subject:"
-msgstr "Asunto:"
+msgstr "Betreft:"
 
 msgctxt "selection:res.user,company_filter:"
 msgid "All"
-msgstr "Todas"
+msgstr "Alle"
 
 msgctxt "selection:res.user,company_filter:"
 msgid "Current"
-msgstr "Actual"
+msgstr "Huidig"
 
 msgctxt "view:company.company.config.start:"
 msgid "You can now add your company into the system."
-msgstr "Ahora puede añadir su empresa en el sistema."
+msgstr "U kunt nu uw bedrijf toevoegen aan het systeem."
 
 msgctxt "view:company.company:"
 msgid "Reports"
-msgstr "Informes"
+msgstr "Rapporten"
 
 msgctxt "wizard_button:company.company.config,company,add:"
 msgid "Add"
-msgstr "Añadir"
+msgstr "Toevoegen"
 
 msgctxt "wizard_button:company.company.config,company,end:"
 msgid "Cancel"
-msgstr "Cancelar"
+msgstr "Annuleer"
 
 msgctxt "wizard_button:company.company.config,start,company:"
 msgid "OK"
-msgstr "Aceptar"
+msgstr "OK"
 
 msgctxt "wizard_button:company.company.config,start,end:"
 msgid "Cancel"
-msgstr "Cancelar"
+msgstr "Annuleer"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_company-7.2.0/locale/es_419.po` & `trytond_company-7.2.1/locale/es_419.po`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,18 @@
 msgid "Party"
 msgstr ""
 
 msgctxt "field:company.company,timezone:"
 msgid "Timezone"
 msgstr ""
 
+msgctxt "field:company.employee,active:"
+msgid "Active"
+msgstr ""
+
 msgctxt "field:company.employee,company:"
 msgid "Company"
 msgstr ""
 
 msgctxt "field:company.employee,end_date:"
 msgid "End Date"
 msgstr ""
```

### Comparing `trytond_company-7.2.0/locale/et.po` & `trytond_company-7.2.1/locale/et.po`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,18 @@
 msgid "Party"
 msgstr "Osapool"
 
 msgctxt "field:company.company,timezone:"
 msgid "Timezone"
 msgstr "Ajavöönd"
 
+msgctxt "field:company.employee,active:"
+msgid "Active"
+msgstr ""
+
 msgctxt "field:company.employee,company:"
 msgid "Company"
 msgstr "Ettevõte"
 
 msgctxt "field:company.employee,end_date:"
 msgid "End Date"
 msgstr "Lõppkuupäev"
```

### Comparing `trytond_company-7.2.0/locale/fa.po` & `trytond_company-7.2.1/locale/fa.po`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,18 @@
 msgid "Party"
 msgstr "نهاد/سازمان"
 
 msgctxt "field:company.company,timezone:"
 msgid "Timezone"
 msgstr "منطقه زمانی"
 
+msgctxt "field:company.employee,active:"
+msgid "Active"
+msgstr ""
+
 msgctxt "field:company.employee,company:"
 msgid "Company"
 msgstr "شرکت"
 
 msgctxt "field:company.employee,end_date:"
 msgid "End Date"
 msgstr "تاریخ پایان"
```

### Comparing `trytond_company-7.2.0/locale/fi.po` & `trytond_company-7.2.1/locale/fi.po`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,18 @@
 msgid "Party"
 msgstr ""
 
 msgctxt "field:company.company,timezone:"
 msgid "Timezone"
 msgstr ""
 
+msgctxt "field:company.employee,active:"
+msgid "Active"
+msgstr ""
+
 msgctxt "field:company.employee,company:"
 msgid "Company"
 msgstr ""
 
 msgctxt "field:company.employee,end_date:"
 msgid "End Date"
 msgstr ""
```

### Comparing `trytond_company-7.2.0/locale/fr.po` & `trytond_company-7.2.1/locale/fr.po`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,18 @@
 msgid "Party"
 msgstr "Tiers"
 
 msgctxt "field:company.company,timezone:"
 msgid "Timezone"
 msgstr "Fuseau Horaire"
 
+msgctxt "field:company.employee,active:"
+msgid "Active"
+msgstr "Actif"
+
 msgctxt "field:company.employee,company:"
 msgid "Company"
 msgstr "Société"
 
 msgctxt "field:company.employee,end_date:"
 msgid "End Date"
 msgstr "Date de fin"
```

### Comparing `trytond_company-7.2.0/locale/hu.po` & `trytond_company-7.2.1/locale/hu.po`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,18 @@
 msgid "Party"
 msgstr "Ügyfél"
 
 msgctxt "field:company.company,timezone:"
 msgid "Timezone"
 msgstr "Időzóna"
 
+msgctxt "field:company.employee,active:"
+msgid "Active"
+msgstr ""
+
 msgctxt "field:company.employee,company:"
 msgid "Company"
 msgstr "Cég"
 
 msgctxt "field:company.employee,end_date:"
 msgid "End Date"
 msgstr "Befejező dátum"
```

### Comparing `trytond_company-7.2.0/locale/id.po` & `trytond_company-7.2.1/locale/id.po`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,18 @@
 msgid "Party"
 msgstr "Pihak"
 
 msgctxt "field:company.company,timezone:"
 msgid "Timezone"
 msgstr "Zona Waktu"
 
+msgctxt "field:company.employee,active:"
+msgid "Active"
+msgstr ""
+
 msgctxt "field:company.employee,company:"
 msgid "Company"
 msgstr "Perusahaan"
 
 msgctxt "field:company.employee,end_date:"
 msgid "End Date"
 msgstr "Tanggal Akhir"
```

### Comparing `trytond_company-7.2.0/locale/it.po` & `trytond_company-7.2.1/locale/it.po`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,18 @@
 msgid "Party"
 msgstr "Controparte"
 
 msgctxt "field:company.company,timezone:"
 msgid "Timezone"
 msgstr "Ora"
 
+msgctxt "field:company.employee,active:"
+msgid "Active"
+msgstr ""
+
 msgctxt "field:company.employee,company:"
 msgid "Company"
 msgstr "Azienda"
 
 msgctxt "field:company.employee,end_date:"
 msgid "End Date"
 msgstr "Data fine"
```

### Comparing `trytond_company-7.2.0/locale/lo.po` & `trytond_company-7.2.1/locale/lo.po`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,18 @@
 msgid "Party"
 msgstr "ພາກສ່ວນ"
 
 msgctxt "field:company.company,timezone:"
 msgid "Timezone"
 msgstr "ເຂດເວລາ"
 
+msgctxt "field:company.employee,active:"
+msgid "Active"
+msgstr ""
+
 msgctxt "field:company.employee,company:"
 msgid "Company"
 msgstr "ຫ້ອງການ/ສຳນັກງານ"
 
 msgctxt "field:company.employee,end_date:"
 msgid "End Date"
 msgstr "ວັນທີສິ້ນສຸດ"
```

### Comparing `trytond_company-7.2.0/locale/lt.po` & `trytond_company-7.2.1/locale/lt.po`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,18 @@
 msgid "Party"
 msgstr "Kontrahentas"
 
 msgctxt "field:company.company,timezone:"
 msgid "Timezone"
 msgstr "Laiko zona"
 
+msgctxt "field:company.employee,active:"
+msgid "Active"
+msgstr ""
+
 msgctxt "field:company.employee,company:"
 msgid "Company"
 msgstr "Organizacija"
 
 msgctxt "field:company.employee,end_date:"
 msgid "End Date"
 msgstr "Pabaigos data"
```

### Comparing `trytond_company-7.2.0/locale/nl.po` & `trytond_company-7.2.1/locale/ru.po`

 * *Files 14% similar despite different names*

```diff
@@ -1,134 +1,146 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:company.company,currency:"
 msgid "Currency"
-msgstr "Valuta"
+msgstr "Валюта"
 
 msgctxt "field:company.company,employees:"
 msgid "Employees"
-msgstr "Werknemers"
+msgstr "Сотрудники"
 
 msgctxt "field:company.company,footer:"
 msgid "Footer"
-msgstr "Voettekst"
+msgstr "Нижний колонтитул"
 
 msgctxt "field:company.company,header:"
 msgid "Header"
-msgstr "Koptekst"
+msgstr "Верхний колонтитул"
 
 msgctxt "field:company.company,party:"
 msgid "Party"
-msgstr "Relatie"
+msgstr "Контрагент"
 
+#, fuzzy
 msgctxt "field:company.company,timezone:"
 msgid "Timezone"
-msgstr "Tijdzone"
+msgstr "Зона времени"
+
+msgctxt "field:company.employee,active:"
+msgid "Active"
+msgstr ""
 
 msgctxt "field:company.employee,company:"
 msgid "Company"
-msgstr "Bedrijf"
+msgstr "Организация"
 
 msgctxt "field:company.employee,end_date:"
 msgid "End Date"
-msgstr "Eind datum"
+msgstr ""
 
 msgctxt "field:company.employee,party:"
 msgid "Party"
-msgstr "Relatie"
+msgstr "Контрагент"
 
 msgctxt "field:company.employee,start_date:"
 msgid "Start Date"
-msgstr "Start Datum"
+msgstr ""
 
 msgctxt "field:company.employee,subordinates:"
 msgid "Subordinates"
-msgstr "Ondergeschikten"
+msgstr ""
 
 msgctxt "field:company.employee,supervisor:"
 msgid "Supervisor"
-msgstr "Leidinggevende"
+msgstr ""
 
 msgctxt "field:ir.cron,companies:"
 msgid "Companies"
-msgstr "Bedrijven"
+msgstr "Организация"
 
 msgctxt "field:ir.cron-company.company,company:"
 msgid "Company"
-msgstr "Bedrijf"
+msgstr "Организация"
 
 msgctxt "field:ir.cron-company.company,cron:"
 msgid "Cron"
-msgstr "Planner"
+msgstr "Планировщик"
 
 msgctxt "field:ir.sequence,company:"
 msgid "Company"
-msgstr "Bedrijf"
+msgstr "Организация"
 
 msgctxt "field:ir.sequence.strict,company:"
 msgid "Company"
-msgstr "Bedrijf"
+msgstr "Организация"
 
+#, fuzzy
 msgctxt "field:party.configuration.party_lang,company:"
 msgid "Company"
-msgstr "Bedrijf"
+msgstr "Организация"
 
+#, fuzzy
 msgctxt "field:party.contact_mechanism.language,company:"
 msgid "Company"
-msgstr "Bedrijf"
+msgstr "Организация"
 
+#, fuzzy
 msgctxt "field:party.party.lang,company:"
 msgid "Company"
-msgstr "Bedrijf"
+msgstr "Организация"
 
+#, fuzzy
 msgctxt "field:res.user,companies:"
 msgid "Companies"
-msgstr "Bedrijven"
+msgstr "Организация"
 
 msgctxt "field:res.user,company:"
 msgid "Current Company"
-msgstr "Huidig bedrijf"
+msgstr "Текущая организация"
 
+#, fuzzy
 msgctxt "field:res.user,company_filter:"
 msgid "Company Filter"
-msgstr "Bedrijfsfilter"
+msgstr "Организация"
 
 msgctxt "field:res.user,employee:"
 msgid "Current Employee"
-msgstr "Huidige werknemer"
+msgstr "Сотрудник"
 
 msgctxt "field:res.user,employees:"
 msgid "Employees"
-msgstr "Werknemers"
+msgstr "Сотрудники"
 
+#, fuzzy
 msgctxt "field:res.user-company.company,company:"
 msgid "Company"
-msgstr "Bedrijf"
+msgstr "Организация"
 
+#, fuzzy
 msgctxt "field:res.user-company.company,user:"
 msgid "User"
-msgstr "Gebruiker"
+msgstr "Пользователь"
 
 msgctxt "field:res.user-company.employee,employee:"
 msgid "Employee"
-msgstr "Werknemer"
+msgstr "Сотрудник"
 
 msgctxt "field:res.user-company.employee,user:"
 msgid "User"
-msgstr "Gebruiker"
+msgstr "Пользователь"
 
 msgctxt "help:company.company,currency:"
 msgid "The main currency for the company."
-msgstr "De hoofd-valuta voor het bedrijf."
+msgstr ""
 
 msgctxt "help:company.company,employees:"
 msgid "Add employees to the company."
-msgstr "Voeg medewerkers toe aan het bedrijf."
+msgstr ""
 
 msgctxt "help:company.company,footer:"
 msgid ""
 "The text to display on report footers.\n"
 "The following placeholders can be used:\n"
 "- ${name}\n"
 "- ${phone}\n"
@@ -152,192 +164,202 @@
 "- ${website}\n"
 "- ${address}\n"
 "- ${tax_identifier}\n"
 msgstr ""
 
 msgctxt "help:company.company,timezone:"
 msgid "Used to compute the today date."
-msgstr "Gebruikt om de datum van vandaag te berekenen."
+msgstr ""
 
 msgctxt "help:company.employee,company:"
 msgid "The company to which the employee belongs."
-msgstr "Het bedrijf waartoe de werknemer behoort."
+msgstr ""
 
 msgctxt "help:company.employee,end_date:"
 msgid "When the employee leaves the company."
-msgstr "Wanneer de werknemer uit dienst treedt."
+msgstr ""
 
 msgctxt "help:company.employee,party:"
 msgid "The party which represents the employee."
-msgstr "De relatie die de werknemer weergeeft."
+msgstr ""
 
 msgctxt "help:company.employee,start_date:"
 msgid "When the employee joins the company."
-msgstr "Wanneer de werknemer in dienst treedt."
+msgstr ""
 
 msgctxt "help:company.employee,subordinates:"
 msgid "The employees to be overseen by this employee."
-msgstr "De werknemers waar deze werknemer leiding aan geeft."
+msgstr ""
 
 msgctxt "help:company.employee,supervisor:"
 msgid "The employee who oversees this employee."
-msgstr "De werknemer die leiding geeft aan deze werknemer."
+msgstr ""
 
+#, fuzzy
 msgctxt "help:ir.cron,companies:"
 msgid "Companies registered for this cron."
-msgstr "Bedrijven aangesloten op deze planner."
+msgstr "Организации зарегистрированные для этого планировщика"
 
 msgctxt "help:ir.rule,domain:"
 msgid ""
 "\n"
 "- \"companies\" as list of ids from the current user"
 msgstr ""
-"\n"
-"- \"bedrijven\" als een lijst met ID's van de huidige gebruiker"
 
 msgctxt "help:ir.sequence,company:"
 msgid "Restricts the sequence usage to the company."
-msgstr "Beperkt het gebruik van de reeks tot het bedrijf."
+msgstr ""
 
 msgctxt "help:ir.sequence.strict,company:"
 msgid "Restricts the sequence usage to the company."
-msgstr "Beperkt het gebruik van de reeks tot het bedrijf."
+msgstr ""
 
 msgctxt "help:res.user,companies:"
 msgid "The companies that the user has access to."
-msgstr "De bedrijven waar de gebruiker toegang tot heeft."
+msgstr ""
 
 msgctxt "help:res.user,company:"
 msgid "Select the company to work for."
-msgstr "Selecteer het bedrijf om voor te werken."
+msgstr ""
 
 msgctxt "help:res.user,company_filter:"
 msgid "Define records of which companies are shown."
-msgstr "Leg vast welke bedrijven worden getoond."
+msgstr ""
 
 msgctxt "help:res.user,employee:"
 msgid "Select the employee to make the user behave as such."
-msgstr "Selecteer de medewerker zodat de gebruiker zich als zodanig gedraagt."
+msgstr ""
 
 msgctxt "help:res.user,employees:"
 msgid "Add employees to grant the user access to them."
-msgstr "Voeg de werknemers toe die toegestaan voor de gebruiker."
+msgstr ""
 
 msgctxt "model:company.company,name:"
 msgid "Company"
-msgstr "Bedrijf"
+msgstr "Организация"
 
 msgctxt "model:company.company.config.start,name:"
 msgid "Company Config"
-msgstr "Bedrijf configuratie"
+msgstr "Настройка организации"
 
 msgctxt "model:company.employee,name:"
 msgid "Employee"
-msgstr "Werknemer"
+msgstr "Сотрудник"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_company_config"
 msgid "Configure Company"
-msgstr "Bedrijf configureren"
+msgstr "Configure Company"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_company_list"
 msgid "Companies"
-msgstr "Bedrijven"
+msgstr "Companies"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_employee_form"
 msgid "Employees"
-msgstr "Werknemers"
+msgstr "Employees"
 
 msgctxt "model:ir.action,name:act_employee_subordinates"
 msgid "Supervised by"
-msgstr "Onder leiding van"
+msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.action,name:report_letter"
 msgid "Letter"
-msgstr "Brief"
+msgstr "Letter"
 
 msgctxt "model:ir.cron-company.company,name:"
 msgid "Cron - Company"
-msgstr "Planner - Bedrijf"
+msgstr "Планировщик - Организация"
 
+#, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_sequence_companies"
 msgid "User in companies"
-msgstr "Gebruiker in bedrijven"
+msgstr "Планировщик - Организация"
 
+#, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_sequence_strict_companies"
 msgid "User in companies"
-msgstr "Gebruiker in bedrijven"
+msgstr "Планировщик - Организация"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_company"
 msgid "Companies"
-msgstr "Bedrijven"
+msgstr "Организация"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_company_list"
 msgid "Companies"
-msgstr "Bedrijven"
+msgstr "Companies"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_employee_form"
 msgid "Employees"
-msgstr "Werknemers"
+msgstr "Employees"
 
 msgctxt "model:res.group,name:group_company_admin"
 msgid "Company Administration"
-msgstr "Bedrijf administratie"
+msgstr ""
 
 msgctxt "model:res.group,name:group_employee_admin"
 msgid "Employee Administration"
-msgstr "Werknemer administratie"
+msgstr ""
 
+#, fuzzy
 msgctxt "model:res.user-company.company,name:"
 msgid "User - Company"
-msgstr "Gebruiker in het bedrijf"
+msgstr "Планировщик - Организация"
 
 msgctxt "model:res.user-company.employee,name:"
 msgid "User - Employee"
-msgstr "Gebruiker - Werknemer"
+msgstr "Пользователь - Сотрудник"
 
 msgctxt "report:party.letter:"
 msgid "Best Regards,"
-msgstr "Met vriendelijke groet,"
+msgstr "С уважением,"
 
 msgctxt "report:party.letter:"
 msgid "Date:"
-msgstr "Datum:"
+msgstr "Дата:"
 
 msgctxt "report:party.letter:"
 msgid "Dear Madams and Sirs,"
-msgstr "Geachte heer/mevrouw,"
+msgstr "Уважаемые дамы и годпода,"
 
 msgctxt "report:party.letter:"
 msgid "Subject:"
-msgstr "Betreft:"
+msgstr "Тема:"
 
 msgctxt "selection:res.user,company_filter:"
 msgid "All"
-msgstr "Alle"
+msgstr ""
 
+#, fuzzy
 msgctxt "selection:res.user,company_filter:"
 msgid "Current"
-msgstr "Huidig"
+msgstr "Валюта"
 
 msgctxt "view:company.company.config.start:"
 msgid "You can now add your company into the system."
-msgstr "U kunt nu uw bedrijf toevoegen aan het systeem."
+msgstr "Теперь вы можете добавить организации."
 
 msgctxt "view:company.company:"
 msgid "Reports"
-msgstr "Rapporten"
+msgstr "Отчеты"
 
 msgctxt "wizard_button:company.company.config,company,add:"
 msgid "Add"
-msgstr "Toevoegen"
+msgstr "Добавить"
 
 msgctxt "wizard_button:company.company.config,company,end:"
 msgid "Cancel"
-msgstr "Annuleer"
+msgstr "Отменить"
 
 msgctxt "wizard_button:company.company.config,start,company:"
 msgid "OK"
-msgstr "OK"
+msgstr "Ок"
 
 msgctxt "wizard_button:company.company.config,start,end:"
 msgid "Cancel"
-msgstr "Annuleer"
+msgstr "Отменить"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_company-7.2.0/locale/pl.po` & `trytond_company-7.2.1/locale/pl.po`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,18 @@
 msgid "Party"
 msgstr "Strona"
 
 msgctxt "field:company.company,timezone:"
 msgid "Timezone"
 msgstr "Strefa czasowa"
 
+msgctxt "field:company.employee,active:"
+msgid "Active"
+msgstr ""
+
 msgctxt "field:company.employee,company:"
 msgid "Company"
 msgstr "Firma"
 
 msgctxt "field:company.employee,end_date:"
 msgid "End Date"
 msgstr "Data zakończenia"
```

### Comparing `trytond_company-7.2.0/locale/pt.po` & `trytond_company-7.2.1/locale/pt.po`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,18 @@
 msgid "Party"
 msgstr "Pessoa"
 
 msgctxt "field:company.company,timezone:"
 msgid "Timezone"
 msgstr "Fuso Horário"
 
+msgctxt "field:company.employee,active:"
+msgid "Active"
+msgstr ""
+
 msgctxt "field:company.employee,company:"
 msgid "Company"
 msgstr "Empresa"
 
 msgctxt "field:company.employee,end_date:"
 msgid "End Date"
 msgstr "Data de término"
```

### Comparing `trytond_company-7.2.0/locale/ro.po` & `trytond_company-7.2.1/locale/ro.po`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,18 @@
 msgid "Party"
 msgstr "Parte"
 
 msgctxt "field:company.company,timezone:"
 msgid "Timezone"
 msgstr "Fus orar"
 
+msgctxt "field:company.employee,active:"
+msgid "Active"
+msgstr ""
+
 msgctxt "field:company.employee,company:"
 msgid "Company"
 msgstr "Companie"
 
 msgctxt "field:company.employee,end_date:"
 msgid "End Date"
 msgstr "Data Încheiere"
```

### Comparing `trytond_company-7.2.0/locale/ru.po` & `trytond_company-7.2.1/locale/sl.po`

 * *Files 19% similar despite different names*

```diff
@@ -1,142 +1,138 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:company.company,currency:"
 msgid "Currency"
-msgstr "Валюта"
+msgstr "Valuta"
 
 msgctxt "field:company.company,employees:"
 msgid "Employees"
-msgstr "Сотрудники"
+msgstr "Zaposlenci"
 
 msgctxt "field:company.company,footer:"
 msgid "Footer"
-msgstr "Нижний колонтитул"
+msgstr "Noga"
 
 msgctxt "field:company.company,header:"
 msgid "Header"
-msgstr "Верхний колонтитул"
+msgstr "Glava"
 
 msgctxt "field:company.company,party:"
 msgid "Party"
-msgstr "Контрагент"
+msgstr "Partner"
 
-#, fuzzy
 msgctxt "field:company.company,timezone:"
 msgid "Timezone"
-msgstr "Зона времени"
+msgstr "Časovni pas"
+
+msgctxt "field:company.employee,active:"
+msgid "Active"
+msgstr ""
 
 msgctxt "field:company.employee,company:"
 msgid "Company"
-msgstr "Организация"
+msgstr "Družba"
 
 msgctxt "field:company.employee,end_date:"
 msgid "End Date"
-msgstr ""
+msgstr "Zapustil"
 
 msgctxt "field:company.employee,party:"
 msgid "Party"
-msgstr "Контрагент"
+msgstr "Partner"
 
 msgctxt "field:company.employee,start_date:"
 msgid "Start Date"
-msgstr ""
+msgstr "Začetni datum"
 
 msgctxt "field:company.employee,subordinates:"
 msgid "Subordinates"
-msgstr ""
+msgstr "Podrejeni"
 
 msgctxt "field:company.employee,supervisor:"
 msgid "Supervisor"
-msgstr ""
+msgstr "Nadzornik"
 
 msgctxt "field:ir.cron,companies:"
 msgid "Companies"
-msgstr "Организация"
+msgstr "Družbe"
 
 msgctxt "field:ir.cron-company.company,company:"
 msgid "Company"
-msgstr "Организация"
+msgstr "Družba"
 
 msgctxt "field:ir.cron-company.company,cron:"
 msgid "Cron"
-msgstr "Планировщик"
+msgstr "Razporejevalnik"
 
 msgctxt "field:ir.sequence,company:"
 msgid "Company"
-msgstr "Организация"
+msgstr "Družba"
 
 msgctxt "field:ir.sequence.strict,company:"
 msgid "Company"
-msgstr "Организация"
+msgstr "Družba"
 
-#, fuzzy
 msgctxt "field:party.configuration.party_lang,company:"
 msgid "Company"
-msgstr "Организация"
+msgstr "Družba"
 
-#, fuzzy
 msgctxt "field:party.contact_mechanism.language,company:"
 msgid "Company"
-msgstr "Организация"
+msgstr "Družba"
 
-#, fuzzy
 msgctxt "field:party.party.lang,company:"
 msgid "Company"
-msgstr "Организация"
+msgstr "Družba"
 
-#, fuzzy
 msgctxt "field:res.user,companies:"
 msgid "Companies"
-msgstr "Организация"
+msgstr "Družbe"
 
 msgctxt "field:res.user,company:"
 msgid "Current Company"
-msgstr "Текущая организация"
+msgstr "Trenutna družba"
 
-#, fuzzy
 msgctxt "field:res.user,company_filter:"
 msgid "Company Filter"
-msgstr "Организация"
+msgstr "Filter družbe"
 
 msgctxt "field:res.user,employee:"
 msgid "Current Employee"
-msgstr "Сотрудник"
+msgstr "Zaposlenec"
 
 msgctxt "field:res.user,employees:"
 msgid "Employees"
-msgstr "Сотрудники"
+msgstr "Zaposlenci"
 
-#, fuzzy
 msgctxt "field:res.user-company.company,company:"
 msgid "Company"
-msgstr "Организация"
+msgstr "Družba"
 
-#, fuzzy
 msgctxt "field:res.user-company.company,user:"
 msgid "User"
-msgstr "Пользователь"
+msgstr "Uporabnik"
 
 msgctxt "field:res.user-company.employee,employee:"
 msgid "Employee"
-msgstr "Сотрудник"
+msgstr "Zaposlenec"
 
 msgctxt "field:res.user-company.employee,user:"
 msgid "User"
-msgstr "Пользователь"
+msgstr "Uporabnik"
 
 msgctxt "help:company.company,currency:"
 msgid "The main currency for the company."
-msgstr ""
+msgstr "Glavna valuta družbe."
 
 msgctxt "help:company.company,employees:"
 msgid "Add employees to the company."
-msgstr ""
+msgstr "Dodaj družbi zaposlence."
 
 msgctxt "help:company.company,footer:"
 msgid ""
 "The text to display on report footers.\n"
 "The following placeholders can be used:\n"
 "- ${name}\n"
 "- ${phone}\n"
@@ -160,202 +156,190 @@
 "- ${website}\n"
 "- ${address}\n"
 "- ${tax_identifier}\n"
 msgstr ""
 
 msgctxt "help:company.company,timezone:"
 msgid "Used to compute the today date."
-msgstr ""
+msgstr "Se uporablja za izračun današnjega datuma."
 
 msgctxt "help:company.employee,company:"
 msgid "The company to which the employee belongs."
-msgstr ""
+msgstr "Družba, ki ji pripada zaposlenec."
 
 msgctxt "help:company.employee,end_date:"
 msgid "When the employee leaves the company."
-msgstr ""
+msgstr "Datum, ko zaposlenec zapusti družbo."
 
 msgctxt "help:company.employee,party:"
 msgid "The party which represents the employee."
-msgstr ""
+msgstr "Partner, ki predstavlja zaposlenca."
 
 msgctxt "help:company.employee,start_date:"
 msgid "When the employee joins the company."
-msgstr ""
+msgstr "Datum, ko zaposlenec vstopi v družbo."
 
 msgctxt "help:company.employee,subordinates:"
 msgid "The employees to be overseen by this employee."
-msgstr ""
+msgstr "Zaposlenci, ki jih nadzira ta zaposlenec."
 
 msgctxt "help:company.employee,supervisor:"
 msgid "The employee who oversees this employee."
-msgstr ""
+msgstr "Zaposlenec, ki nadzira tega zaposlenca."
 
-#, fuzzy
 msgctxt "help:ir.cron,companies:"
 msgid "Companies registered for this cron."
-msgstr "Организации зарегистрированные для этого планировщика"
+msgstr "Družbe, registrirane na ta razporejevalnik."
 
 msgctxt "help:ir.rule,domain:"
 msgid ""
 "\n"
 "- \"companies\" as list of ids from the current user"
 msgstr ""
 
 msgctxt "help:ir.sequence,company:"
 msgid "Restricts the sequence usage to the company."
-msgstr ""
+msgstr "Omeji uporabo šifranta na družbo."
 
 msgctxt "help:ir.sequence.strict,company:"
 msgid "Restricts the sequence usage to the company."
-msgstr ""
+msgstr "Omeji uporabo šifranta na družbo."
 
 msgctxt "help:res.user,companies:"
 msgid "The companies that the user has access to."
-msgstr ""
+msgstr "Družbe do katerih lahko ta zaposlenec dostopa."
 
 msgctxt "help:res.user,company:"
 msgid "Select the company to work for."
-msgstr ""
+msgstr "Izberite družbo za delo."
 
 msgctxt "help:res.user,company_filter:"
 msgid "Define records of which companies are shown."
-msgstr ""
+msgstr "Opredeli zapise na katerih so družbe prikazane."
 
 msgctxt "help:res.user,employee:"
 msgid "Select the employee to make the user behave as such."
-msgstr ""
+msgstr "Poveži uporabniško ime z zaposlencem."
 
 msgctxt "help:res.user,employees:"
 msgid "Add employees to grant the user access to them."
-msgstr ""
+msgstr "Dodeli dostop preko uporabniškega imena izbranim zaposlencem."
 
 msgctxt "model:company.company,name:"
 msgid "Company"
-msgstr "Организация"
+msgstr "Družba"
 
 msgctxt "model:company.company.config.start,name:"
 msgid "Company Config"
-msgstr "Настройка организации"
+msgstr "Konfiguracija družbe"
 
 msgctxt "model:company.employee,name:"
 msgid "Employee"
-msgstr "Сотрудник"
+msgstr "Zaposlenec"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_company_config"
 msgid "Configure Company"
-msgstr "Configure Company"
+msgstr "Nastavi družbo"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_company_list"
 msgid "Companies"
-msgstr "Companies"
+msgstr "Družbe"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_employee_form"
 msgid "Employees"
-msgstr "Employees"
+msgstr "Zaposlenci"
 
 msgctxt "model:ir.action,name:act_employee_subordinates"
 msgid "Supervised by"
-msgstr ""
+msgstr "Nadzornik"
 
-#, fuzzy
 msgctxt "model:ir.action,name:report_letter"
 msgid "Letter"
-msgstr "Letter"
+msgstr "Pismo"
 
 msgctxt "model:ir.cron-company.company,name:"
 msgid "Cron - Company"
-msgstr "Планировщик - Организация"
+msgstr "Razporejevalnik - Družba"
 
-#, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_sequence_companies"
 msgid "User in companies"
-msgstr "Планировщик - Организация"
+msgstr "Uporabnik v družbah"
 
-#, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_sequence_strict_companies"
 msgid "User in companies"
-msgstr "Планировщик - Организация"
+msgstr "Uporabnik v družbah"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_company"
 msgid "Companies"
-msgstr "Организация"
+msgstr "Družbe"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_company_list"
 msgid "Companies"
-msgstr "Companies"
+msgstr "Družbe"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_employee_form"
 msgid "Employees"
-msgstr "Employees"
+msgstr "Zaposlenci"
 
 msgctxt "model:res.group,name:group_company_admin"
 msgid "Company Administration"
-msgstr ""
+msgstr "Skrbništvo družb"
 
 msgctxt "model:res.group,name:group_employee_admin"
 msgid "Employee Administration"
-msgstr ""
+msgstr "Skrbništvo zaposlencev"
 
-#, fuzzy
 msgctxt "model:res.user-company.company,name:"
 msgid "User - Company"
-msgstr "Планировщик - Организация"
+msgstr "Uporabnik - Družba"
 
 msgctxt "model:res.user-company.employee,name:"
 msgid "User - Employee"
-msgstr "Пользователь - Сотрудник"
+msgstr "Uporabnik - Zaposlenec"
 
 msgctxt "report:party.letter:"
 msgid "Best Regards,"
-msgstr "С уважением,"
+msgstr "S spoštovanjem,"
 
 msgctxt "report:party.letter:"
 msgid "Date:"
-msgstr "Дата:"
+msgstr "Datum:"
 
 msgctxt "report:party.letter:"
 msgid "Dear Madams and Sirs,"
-msgstr "Уважаемые дамы и годпода,"
+msgstr "Spoštovani gospa in gospod,"
 
 msgctxt "report:party.letter:"
 msgid "Subject:"
-msgstr "Тема:"
+msgstr "Zadeva:"
 
 msgctxt "selection:res.user,company_filter:"
 msgid "All"
-msgstr ""
+msgstr "Vse"
 
-#, fuzzy
 msgctxt "selection:res.user,company_filter:"
 msgid "Current"
-msgstr "Валюта"
+msgstr "Trenutno"
 
 msgctxt "view:company.company.config.start:"
 msgid "You can now add your company into the system."
-msgstr "Теперь вы можете добавить организации."
+msgstr "Zdaj je možno v sistem dodati družbo."
 
 msgctxt "view:company.company:"
 msgid "Reports"
-msgstr "Отчеты"
+msgstr "Poročila"
 
 msgctxt "wizard_button:company.company.config,company,add:"
 msgid "Add"
-msgstr "Добавить"
+msgstr "Dodaj"
 
 msgctxt "wizard_button:company.company.config,company,end:"
 msgid "Cancel"
-msgstr "Отменить"
+msgstr "Prekliči"
 
 msgctxt "wizard_button:company.company.config,start,company:"
 msgid "OK"
-msgstr "Ок"
+msgstr "V redu"
 
 msgctxt "wizard_button:company.company.config,start,end:"
 msgid "Cancel"
-msgstr "Отменить"
+msgstr "Prekliči"
```

### Comparing `trytond_company-7.2.0/locale/sl.po` & `trytond_company-7.2.1/locale/ca.po`

 * *Files 10% similar despite different names*

```diff
@@ -1,341 +1,367 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:company.company,currency:"
 msgid "Currency"
-msgstr "Valuta"
+msgstr "Moneda"
 
 msgctxt "field:company.company,employees:"
 msgid "Employees"
-msgstr "Zaposlenci"
+msgstr "Empleats"
 
 msgctxt "field:company.company,footer:"
 msgid "Footer"
-msgstr "Noga"
+msgstr "Peu de pàgina"
 
 msgctxt "field:company.company,header:"
 msgid "Header"
-msgstr "Glava"
+msgstr "Capçalera"
 
 msgctxt "field:company.company,party:"
 msgid "Party"
-msgstr "Partner"
+msgstr "Tercer"
 
 msgctxt "field:company.company,timezone:"
 msgid "Timezone"
-msgstr "Časovni pas"
+msgstr "Zona horària"
+
+msgctxt "field:company.employee,active:"
+msgid "Active"
+msgstr "Actiu"
 
 msgctxt "field:company.employee,company:"
 msgid "Company"
-msgstr "Družba"
+msgstr "Empresa"
 
 msgctxt "field:company.employee,end_date:"
 msgid "End Date"
-msgstr "Zapustil"
+msgstr "Data finalització"
 
 msgctxt "field:company.employee,party:"
 msgid "Party"
-msgstr "Partner"
+msgstr "Tercer"
 
 msgctxt "field:company.employee,start_date:"
 msgid "Start Date"
-msgstr "Začetni datum"
+msgstr "Data d'inici"
 
 msgctxt "field:company.employee,subordinates:"
 msgid "Subordinates"
-msgstr "Podrejeni"
+msgstr "Subordinats"
 
 msgctxt "field:company.employee,supervisor:"
 msgid "Supervisor"
-msgstr "Nadzornik"
+msgstr "Supervisor"
 
 msgctxt "field:ir.cron,companies:"
 msgid "Companies"
-msgstr "Družbe"
+msgstr "Empreses"
 
 msgctxt "field:ir.cron-company.company,company:"
 msgid "Company"
-msgstr "Družba"
+msgstr "Empresa"
 
 msgctxt "field:ir.cron-company.company,cron:"
 msgid "Cron"
-msgstr "Razporejevalnik"
+msgstr "Planificador de tasques"
 
 msgctxt "field:ir.sequence,company:"
 msgid "Company"
-msgstr "Družba"
+msgstr "Empresa"
 
 msgctxt "field:ir.sequence.strict,company:"
 msgid "Company"
-msgstr "Družba"
+msgstr "Empresa"
 
 msgctxt "field:party.configuration.party_lang,company:"
 msgid "Company"
-msgstr "Družba"
+msgstr "Empresa"
 
 msgctxt "field:party.contact_mechanism.language,company:"
 msgid "Company"
-msgstr "Družba"
+msgstr "Empresa"
 
 msgctxt "field:party.party.lang,company:"
 msgid "Company"
-msgstr "Družba"
+msgstr "Empresa"
 
 msgctxt "field:res.user,companies:"
 msgid "Companies"
-msgstr "Družbe"
+msgstr "Empreses"
 
 msgctxt "field:res.user,company:"
 msgid "Current Company"
-msgstr "Trenutna družba"
+msgstr "Empresa actual"
 
 msgctxt "field:res.user,company_filter:"
 msgid "Company Filter"
-msgstr "Filter družbe"
+msgstr "Filtre empresa"
 
 msgctxt "field:res.user,employee:"
 msgid "Current Employee"
-msgstr "Zaposlenec"
+msgstr "Empleat"
 
 msgctxt "field:res.user,employees:"
 msgid "Employees"
-msgstr "Zaposlenci"
+msgstr "Empleats"
 
 msgctxt "field:res.user-company.company,company:"
 msgid "Company"
-msgstr "Družba"
+msgstr "Empresa"
 
 msgctxt "field:res.user-company.company,user:"
 msgid "User"
-msgstr "Uporabnik"
+msgstr "Usuari"
 
 msgctxt "field:res.user-company.employee,employee:"
 msgid "Employee"
-msgstr "Zaposlenec"
+msgstr "Empleat"
 
 msgctxt "field:res.user-company.employee,user:"
 msgid "User"
-msgstr "Uporabnik"
+msgstr "Usuari"
 
 msgctxt "help:company.company,currency:"
 msgid "The main currency for the company."
-msgstr "Glavna valuta družbe."
+msgstr "La moneda principal de l'empresa."
 
 msgctxt "help:company.company,employees:"
 msgid "Add employees to the company."
-msgstr "Dodaj družbi zaposlence."
+msgstr "Afegiu empleats a l'empresa."
 
 msgctxt "help:company.company,footer:"
 msgid ""
 "The text to display on report footers.\n"
 "The following placeholders can be used:\n"
 "- ${name}\n"
 "- ${phone}\n"
 "- ${mobile}\n"
 "- ${fax}\n"
 "- ${email}\n"
 "- ${website}\n"
 "- ${address}\n"
 "- ${tax_identifier}\n"
 msgstr ""
+"Text a mostrar al peu de pàgina dels informes\n"
+"Es poden utilitzar les següents substitucions:\n"
+"- ${name}\n"
+"- ${phone}\n"
+"- ${mobile}\n"
+"- ${fax}\n"
+"- ${email}\n"
+"- ${website}\n"
+"- ${address}\n"
+"- ${tax_identifier}\n"
 
 msgctxt "help:company.company,header:"
 msgid ""
 "The text to display on report headers.\n"
 "The following placeholders can be used:\n"
 "- ${name}\n"
 "- ${phone}\n"
 "- ${mobile}\n"
 "- ${fax}\n"
 "- ${email}\n"
 "- ${website}\n"
 "- ${address}\n"
 "- ${tax_identifier}\n"
 msgstr ""
+"Text a mostrar a la capçalera dels informes\n"
+"Es poden utilitzar les següents substitucions:\n"
+"- ${name}\n"
+"- ${phone}\n"
+"- ${mobile}\n"
+"- ${fax}\n"
+"- ${email}\n"
+"- ${website}\n"
+"- ${address}\n"
+"- ${tax_identifier}\n"
 
 msgctxt "help:company.company,timezone:"
 msgid "Used to compute the today date."
-msgstr "Se uporablja za izračun današnjega datuma."
+msgstr "Utilitzat per calcular la data d'avui."
 
 msgctxt "help:company.employee,company:"
 msgid "The company to which the employee belongs."
-msgstr "Družba, ki ji pripada zaposlenec."
+msgstr "L'empresa a la que pertany l'empleat."
 
 msgctxt "help:company.employee,end_date:"
 msgid "When the employee leaves the company."
-msgstr "Datum, ko zaposlenec zapusti družbo."
+msgstr "Quan l'empleat marxa de l'empresa."
 
 msgctxt "help:company.employee,party:"
 msgid "The party which represents the employee."
-msgstr "Partner, ki predstavlja zaposlenca."
+msgstr "El tercer que representa l'empleat."
 
 msgctxt "help:company.employee,start_date:"
 msgid "When the employee joins the company."
-msgstr "Datum, ko zaposlenec vstopi v družbo."
+msgstr "Quan l'empleat entra a l'empresa."
 
 msgctxt "help:company.employee,subordinates:"
 msgid "The employees to be overseen by this employee."
-msgstr "Zaposlenci, ki jih nadzira ta zaposlenec."
+msgstr "Els empleats que són supervisats per aquest empleat."
 
 msgctxt "help:company.employee,supervisor:"
 msgid "The employee who oversees this employee."
-msgstr "Zaposlenec, ki nadzira tega zaposlenca."
+msgstr "L'empleat que supervisa aquest empleat."
 
 msgctxt "help:ir.cron,companies:"
 msgid "Companies registered for this cron."
-msgstr "Družbe, registrirane na ta razporejevalnik."
+msgstr "Empreses registrades per aquest planificador."
 
 msgctxt "help:ir.rule,domain:"
 msgid ""
 "\n"
 "- \"companies\" as list of ids from the current user"
 msgstr ""
+"\n"
+"- \"companies\" com una llista de ids de les empreses del usuari actual"
 
 msgctxt "help:ir.sequence,company:"
 msgid "Restricts the sequence usage to the company."
-msgstr "Omeji uporabo šifranta na družbo."
+msgstr "Restringeix l'ús de la seqüencia a l'empresa."
 
 msgctxt "help:ir.sequence.strict,company:"
 msgid "Restricts the sequence usage to the company."
-msgstr "Omeji uporabo šifranta na družbo."
+msgstr "Restringeix l'ús de la seqüencia a l'empresa."
 
 msgctxt "help:res.user,companies:"
 msgid "The companies that the user has access to."
-msgstr "Družbe do katerih lahko ta zaposlenec dostopa."
+msgstr "Les empreses a les que té accés l'usuari."
 
 msgctxt "help:res.user,company:"
 msgid "Select the company to work for."
-msgstr "Izberite družbo za delo."
+msgstr "Seleccioneu l'empresa en la que voleu treballar."
 
 msgctxt "help:res.user,company_filter:"
 msgid "Define records of which companies are shown."
-msgstr "Opredeli zapise na katerih so družbe prikazane."
+msgstr "Defineix els registres de quines empreses es mostren."
 
 msgctxt "help:res.user,employee:"
 msgid "Select the employee to make the user behave as such."
-msgstr "Poveži uporabniško ime z zaposlencem."
+msgstr "Seleccioneu l'empleat com al que es comportarà l'usuari."
 
 msgctxt "help:res.user,employees:"
 msgid "Add employees to grant the user access to them."
-msgstr "Dodeli dostop preko uporabniškega imena izbranim zaposlencem."
+msgstr "Afegeix empleats als que podrà accedir l'usuari."
 
 msgctxt "model:company.company,name:"
 msgid "Company"
-msgstr "Družba"
+msgstr "Empresa"
 
 msgctxt "model:company.company.config.start,name:"
 msgid "Company Config"
-msgstr "Konfiguracija družbe"
+msgstr "Configuració empresa"
 
 msgctxt "model:company.employee,name:"
 msgid "Employee"
-msgstr "Zaposlenec"
+msgstr "Empleat"
 
 msgctxt "model:ir.action,name:act_company_config"
 msgid "Configure Company"
-msgstr "Nastavi družbo"
+msgstr "Configura l'empresa"
 
 msgctxt "model:ir.action,name:act_company_list"
 msgid "Companies"
-msgstr "Družbe"
+msgstr "Empreses"
 
 msgctxt "model:ir.action,name:act_employee_form"
 msgid "Employees"
-msgstr "Zaposlenci"
+msgstr "Empleats"
 
 msgctxt "model:ir.action,name:act_employee_subordinates"
 msgid "Supervised by"
-msgstr "Nadzornik"
+msgstr "Supervisat per"
 
 msgctxt "model:ir.action,name:report_letter"
 msgid "Letter"
-msgstr "Pismo"
+msgstr "Carta"
 
 msgctxt "model:ir.cron-company.company,name:"
 msgid "Cron - Company"
-msgstr "Razporejevalnik - Družba"
+msgstr "Planificador - Empresa"
 
 msgctxt "model:ir.rule.group,name:rule_group_sequence_companies"
 msgid "User in companies"
-msgstr "Uporabnik v družbah"
+msgstr "Usuari a les empreses"
 
 msgctxt "model:ir.rule.group,name:rule_group_sequence_strict_companies"
 msgid "User in companies"
-msgstr "Uporabnik v družbah"
+msgstr "Usuari a les empreses"
 
 msgctxt "model:ir.ui.menu,name:menu_company"
 msgid "Companies"
-msgstr "Družbe"
+msgstr "Empreses"
 
 msgctxt "model:ir.ui.menu,name:menu_company_list"
 msgid "Companies"
-msgstr "Družbe"
+msgstr "Empreses"
 
 msgctxt "model:ir.ui.menu,name:menu_employee_form"
 msgid "Employees"
-msgstr "Zaposlenci"
+msgstr "Empleats"
 
 msgctxt "model:res.group,name:group_company_admin"
 msgid "Company Administration"
-msgstr "Skrbništvo družb"
+msgstr "Administració d'empreses"
 
 msgctxt "model:res.group,name:group_employee_admin"
 msgid "Employee Administration"
-msgstr "Skrbništvo zaposlencev"
+msgstr "Administració d'empleats"
 
 msgctxt "model:res.user-company.company,name:"
 msgid "User - Company"
-msgstr "Uporabnik - Družba"
+msgstr "Usuari - Empresa"
 
 msgctxt "model:res.user-company.employee,name:"
 msgid "User - Employee"
-msgstr "Uporabnik - Zaposlenec"
+msgstr "Usuari - Emprat"
 
 msgctxt "report:party.letter:"
 msgid "Best Regards,"
-msgstr "S spoštovanjem,"
+msgstr "Atentament,"
 
 msgctxt "report:party.letter:"
 msgid "Date:"
-msgstr "Datum:"
+msgstr "Data:"
 
 msgctxt "report:party.letter:"
 msgid "Dear Madams and Sirs,"
-msgstr "Spoštovani gospa in gospod,"
+msgstr "Estimats senyors i senyores,"
 
 msgctxt "report:party.letter:"
 msgid "Subject:"
-msgstr "Zadeva:"
+msgstr "Assumpte:"
 
 msgctxt "selection:res.user,company_filter:"
 msgid "All"
-msgstr "Vse"
+msgstr "Totes"
 
 msgctxt "selection:res.user,company_filter:"
 msgid "Current"
-msgstr "Trenutno"
+msgstr "Actual"
 
 msgctxt "view:company.company.config.start:"
 msgid "You can now add your company into the system."
-msgstr "Zdaj je možno v sistem dodati družbo."
+msgstr "Ara podeu afegir la vostra empresa al sistema."
 
 msgctxt "view:company.company:"
 msgid "Reports"
-msgstr "Poročila"
+msgstr "Informes"
 
 msgctxt "wizard_button:company.company.config,company,add:"
 msgid "Add"
-msgstr "Dodaj"
+msgstr "Afegeix"
 
 msgctxt "wizard_button:company.company.config,company,end:"
 msgid "Cancel"
-msgstr "Prekliči"
+msgstr "Cancel·la"
 
 msgctxt "wizard_button:company.company.config,start,company:"
 msgid "OK"
-msgstr "V redu"
+msgstr "D'acord"
 
 msgctxt "wizard_button:company.company.config,start,end:"
 msgid "Cancel"
-msgstr "Prekliči"
+msgstr "Cancel·la"
```

### Comparing `trytond_company-7.2.0/locale/tr.po` & `trytond_company-7.2.1/locale/tr.po`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,18 @@
 msgid "Party"
 msgstr ""
 
 msgctxt "field:company.company,timezone:"
 msgid "Timezone"
 msgstr ""
 
+msgctxt "field:company.employee,active:"
+msgid "Active"
+msgstr ""
+
 msgctxt "field:company.employee,company:"
 msgid "Company"
 msgstr ""
 
 msgctxt "field:company.employee,end_date:"
 msgid "End Date"
 msgstr ""
```

### Comparing `trytond_company-7.2.0/locale/uk.po` & `trytond_company-7.2.1/locale/uk.po`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,18 @@
 msgid "Party"
 msgstr "Особа"
 
 msgctxt "field:company.company,timezone:"
 msgid "Timezone"
 msgstr "Часовий пояс"
 
+msgctxt "field:company.employee,active:"
+msgid "Active"
+msgstr ""
+
 msgctxt "field:company.employee,company:"
 msgid "Company"
 msgstr "Компанія"
 
 msgctxt "field:company.employee,end_date:"
 msgid "End Date"
 msgstr "Дата завершення"
```

### Comparing `trytond_company-7.2.0/locale/zh_CN.po` & `trytond_company-7.2.1/locale/zh_CN.po`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,18 @@
 msgid "Party"
 msgstr "参与者"
 
 msgctxt "field:company.company,timezone:"
 msgid "Timezone"
 msgstr "时区"
 
+msgctxt "field:company.employee,active:"
+msgid "Active"
+msgstr ""
+
 msgctxt "field:company.employee,company:"
 msgid "Company"
 msgstr "公司"
 
 msgctxt "field:company.employee,end_date:"
 msgid "End Date"
 msgstr "离职日期"
```

### Comparing `trytond_company-7.2.0/model.py` & `trytond_company-7.2.1/model.py`

 * *Files identical despite different names*

### Comparing `trytond_company-7.2.0/party.py` & `trytond_company-7.2.1/party.py`

 * *Files identical despite different names*

### Comparing `trytond_company-7.2.0/res.py` & `trytond_company-7.2.1/res.py`

 * *Files identical despite different names*

### Comparing `trytond_company-7.2.0/setup.py` & `trytond_company-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_company-7.2.0/tests/test_module.py` & `trytond_company-7.2.1/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_company-7.2.0/tests/tools.py` & `trytond_company-7.2.1/tests/tools.py`

 * *Files identical despite different names*

### Comparing `trytond_company-7.2.0/tox.ini` & `trytond_company-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_company-7.2.0/trytond_company.egg-info/PKG-INFO` & `trytond_company-7.2.1/trytond_company.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_company
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module with companies and employees
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_company-7.2.0/trytond_company.egg-info/SOURCES.txt` & `trytond_company-7.2.1/trytond_company.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_company-7.2.0/view/company_form.xml` & `trytond_company-7.2.1/view/company_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_company-7.2.0/view/user_form.xml` & `trytond_company-7.2.1/view/user_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_company-7.2.0/view/user_form_preferences.xml` & `trytond_company-7.2.1/view/user_form_preferences.xml`

 * *Files identical despite different names*

