# Comparing `tmp/trytond_account_export_winbooks-7.2.0.tar.gz` & `tmp/trytond_account_export_winbooks-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_export_winbooks-7.2.0.tar", last modified: Mon Apr 29 15:54:55 2024, max compression
+gzip compressed data, was "trytond_account_export_winbooks-7.2.1.tar", last modified: Wed May  1 12:23:31 2024, max compression
```

## Comparing `trytond_account_export_winbooks-7.2.0.tar` & `trytond_account_export_winbooks-7.2.1.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:55.433362 trytond_account_export_winbooks-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)       71 2024-04-29 15:30:37.000000 trytond_account_export_winbooks-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      646 2024-04-29 15:30:36.000000 trytond_account_export_winbooks-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-27 16:30:39.000000 trytond_account_export_winbooks-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-27 16:30:39.000000 trytond_account_export_winbooks-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2984 2024-04-29 15:54:55.433362 trytond_account_export_winbooks-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      287 2024-04-27 16:30:39.000000 trytond_account_export_winbooks-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      762 2024-04-27 16:30:39.000000 trytond_account_export_winbooks-7.2.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    11225 2024-04-27 16:30:39.000000 trytond_account_export_winbooks-7.2.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1578 2024-04-27 16:30:39.000000 trytond_account_export_winbooks-7.2.0/account.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     9005 2024-04-27 16:30:39.000000 trytond_account_export_winbooks-7.2.0/account_be.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     9172 2024-04-27 16:30:39.000000 trytond_account_export_winbooks-7.2.0/account_be_fr.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     9172 2024-04-27 16:30:39.000000 trytond_account_export_winbooks-7.2.0/account_be_nl.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:55.430029 trytond_account_export_winbooks-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3086 2024-04-27 16:30:39.000000 trytond_account_export_winbooks-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2327 2024-04-27 16:30:39.000000 trytond_account_export_winbooks-7.2.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      287 2024-04-27 16:30:39.000000 trytond_account_export_winbooks-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-27 16:30:39.000000 trytond_account_export_winbooks-7.2.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-27 16:30:39.000000 trytond_account_export_winbooks-7.2.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:55.430029 trytond_account_export_winbooks-7.2.0/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2024-04-27 16:30:39.000000 trytond_account_export_winbooks-7.2.0/icons/LICENSE
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:55.433362 trytond_account_export_winbooks-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_account_export_winbooks-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_account_export_winbooks-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_account_export_winbooks-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_account_export_winbooks-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_account_export_winbooks-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_account_export_winbooks-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_account_export_winbooks-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_account_export_winbooks-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_account_export_winbooks-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_account_export_winbooks-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_account_export_winbooks-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_account_export_winbooks-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_account_export_winbooks-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_account_export_winbooks-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_account_export_winbooks-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_account_export_winbooks-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_account_export_winbooks-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_account_export_winbooks-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_account_export_winbooks-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_account_export_winbooks-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_account_export_winbooks-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_account_export_winbooks-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_account_export_winbooks-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_account_export_winbooks-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      798 2024-04-27 16:30:39.000000 trytond_account_export_winbooks-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2283 2024-04-27 16:30:39.000000 trytond_account_export_winbooks-7.2.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)      466 2024-04-27 16:30:39.000000 trytond_account_export_winbooks-7.2.0/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:54:55.433362 trytond_account_export_winbooks-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4836 2024-04-27 16:30:39.000000 trytond_account_export_winbooks-7.2.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:55.433362 trytond_account_export_winbooks-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)     1686 2024-04-27 16:30:39.000000 trytond_account_export_winbooks-7.2.0/tests/ACT.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-27 16:30:39.000000 trytond_account_export_winbooks-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6582 2024-04-27 16:30:39.000000 trytond_account_export_winbooks-7.2.0/tests/scenario_account_export_winbooks.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      402 2024-04-27 16:30:39.000000 trytond_account_export_winbooks-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-27 16:30:39.000000 trytond_account_export_winbooks-7.2.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-27 16:30:39.000000 trytond_account_export_winbooks-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      247 2024-04-29 15:30:32.000000 trytond_account_export_winbooks-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:55.433362 trytond_account_export_winbooks-7.2.0/trytond_account_export_winbooks.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2984 2024-04-29 15:54:55.000000 trytond_account_export_winbooks-7.2.0/trytond_account_export_winbooks.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2115 2024-04-29 15:54:55.000000 trytond_account_export_winbooks-7.2.0/trytond_account_export_winbooks.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:54:55.000000 trytond_account_export_winbooks-7.2.0/trytond_account_export_winbooks.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       84 2024-04-29 15:54:55.000000 trytond_account_export_winbooks-7.2.0/trytond_account_export_winbooks.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:54:55.000000 trytond_account_export_winbooks-7.2.0/trytond_account_export_winbooks.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      237 2024-04-29 15:54:55.000000 trytond_account_export_winbooks-7.2.0/trytond_account_export_winbooks.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:54:55.000000 trytond_account_export_winbooks-7.2.0/trytond_account_export_winbooks.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:55.433362 trytond_account_export_winbooks-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      381 2024-04-27 16:30:39.000000 trytond_account_export_winbooks-7.2.0/view/account_account_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      356 2024-04-27 16:30:39.000000 trytond_account_export_winbooks-7.2.0/view/account_fiscalyear_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      446 2024-04-27 16:30:39.000000 trytond_account_export_winbooks-7.2.0/view/account_journal_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      367 2024-04-27 16:30:39.000000 trytond_account_export_winbooks-7.2.0/view/account_tax_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      367 2024-04-27 16:30:39.000000 trytond_account_export_winbooks-7.2.0/view/account_tax_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      399 2024-04-27 16:30:39.000000 trytond_account_export_winbooks-7.2.0/view/party_party_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:23:31.879494 trytond_account_export_winbooks-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)      172 2024-05-01 12:23:28.000000 trytond_account_export_winbooks-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      646 2024-05-01 12:23:28.000000 trytond_account_export_winbooks-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:20:59.000000 trytond_account_export_winbooks-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:20:59.000000 trytond_account_export_winbooks-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2984 2024-05-01 12:23:31.879494 trytond_account_export_winbooks-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      287 2024-04-30 17:20:59.000000 trytond_account_export_winbooks-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      762 2024-04-30 17:20:59.000000 trytond_account_export_winbooks-7.2.1/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    11225 2024-04-30 17:20:59.000000 trytond_account_export_winbooks-7.2.1/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1578 2024-04-30 17:20:59.000000 trytond_account_export_winbooks-7.2.1/account.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     9005 2024-04-30 17:20:59.000000 trytond_account_export_winbooks-7.2.1/account_be.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     9172 2024-04-30 17:20:59.000000 trytond_account_export_winbooks-7.2.1/account_be_fr.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     9172 2024-04-30 17:20:59.000000 trytond_account_export_winbooks-7.2.1/account_be_nl.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:23:31.872827 trytond_account_export_winbooks-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3086 2024-04-30 17:20:59.000000 trytond_account_export_winbooks-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2327 2024-04-30 17:20:59.000000 trytond_account_export_winbooks-7.2.1/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      287 2024-04-30 17:20:59.000000 trytond_account_export_winbooks-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-30 17:20:59.000000 trytond_account_export_winbooks-7.2.1/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:20:59.000000 trytond_account_export_winbooks-7.2.1/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:23:31.872827 trytond_account_export_winbooks-7.2.1/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2024-04-30 17:20:59.000000 trytond_account_export_winbooks-7.2.1/icons/LICENSE
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:23:31.876160 trytond_account_export_winbooks-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1634 2024-04-30 17:21:59.000000 trytond_account_export_winbooks-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2128 2024-04-30 17:21:59.000000 trytond_account_export_winbooks-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1634 2024-04-30 17:21:59.000000 trytond_account_export_winbooks-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2111 2024-04-30 17:21:59.000000 trytond_account_export_winbooks-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2152 2024-04-30 17:21:59.000000 trytond_account_export_winbooks-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1634 2024-04-30 17:21:59.000000 trytond_account_export_winbooks-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1634 2024-04-30 17:21:59.000000 trytond_account_export_winbooks-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1634 2024-04-30 17:21:59.000000 trytond_account_export_winbooks-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1634 2024-04-30 17:21:59.000000 trytond_account_export_winbooks-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2135 2024-04-30 17:21:59.000000 trytond_account_export_winbooks-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1634 2024-04-30 17:21:59.000000 trytond_account_export_winbooks-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1634 2024-04-30 17:21:59.000000 trytond_account_export_winbooks-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1634 2024-04-30 17:21:59.000000 trytond_account_export_winbooks-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1634 2024-04-30 17:21:59.000000 trytond_account_export_winbooks-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1634 2024-04-30 17:21:59.000000 trytond_account_export_winbooks-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2117 2024-04-30 17:21:59.000000 trytond_account_export_winbooks-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1634 2024-04-30 17:21:59.000000 trytond_account_export_winbooks-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1634 2024-04-30 17:21:59.000000 trytond_account_export_winbooks-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1634 2024-04-30 17:21:59.000000 trytond_account_export_winbooks-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1634 2024-04-30 17:21:59.000000 trytond_account_export_winbooks-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1634 2024-04-30 17:21:59.000000 trytond_account_export_winbooks-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1634 2024-04-30 17:21:59.000000 trytond_account_export_winbooks-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1634 2024-04-30 17:21:59.000000 trytond_account_export_winbooks-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1634 2024-04-30 17:21:59.000000 trytond_account_export_winbooks-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      798 2024-04-30 17:20:59.000000 trytond_account_export_winbooks-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2283 2024-04-30 17:20:59.000000 trytond_account_export_winbooks-7.2.1/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      466 2024-04-30 17:20:59.000000 trytond_account_export_winbooks-7.2.1/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 12:23:31.879494 trytond_account_export_winbooks-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4836 2024-04-30 17:20:59.000000 trytond_account_export_winbooks-7.2.1/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:23:31.876160 trytond_account_export_winbooks-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1686 2024-04-30 17:20:59.000000 trytond_account_export_winbooks-7.2.1/tests/ACT.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:20:59.000000 trytond_account_export_winbooks-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6582 2024-04-30 17:20:59.000000 trytond_account_export_winbooks-7.2.1/tests/scenario_account_export_winbooks.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      402 2024-04-30 17:20:59.000000 trytond_account_export_winbooks-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:20:59.000000 trytond_account_export_winbooks-7.2.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:20:59.000000 trytond_account_export_winbooks-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      247 2024-04-30 17:21:06.000000 trytond_account_export_winbooks-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:23:31.876160 trytond_account_export_winbooks-7.2.1/trytond_account_export_winbooks.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2984 2024-05-01 12:23:31.000000 trytond_account_export_winbooks-7.2.1/trytond_account_export_winbooks.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2115 2024-05-01 12:23:31.000000 trytond_account_export_winbooks-7.2.1/trytond_account_export_winbooks.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:23:31.000000 trytond_account_export_winbooks-7.2.1/trytond_account_export_winbooks.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       84 2024-05-01 12:23:31.000000 trytond_account_export_winbooks-7.2.1/trytond_account_export_winbooks.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:23:31.000000 trytond_account_export_winbooks-7.2.1/trytond_account_export_winbooks.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      237 2024-05-01 12:23:31.000000 trytond_account_export_winbooks-7.2.1/trytond_account_export_winbooks.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 12:23:31.000000 trytond_account_export_winbooks-7.2.1/trytond_account_export_winbooks.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:23:31.876160 trytond_account_export_winbooks-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      381 2024-04-30 17:20:59.000000 trytond_account_export_winbooks-7.2.1/view/account_account_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      356 2024-04-30 17:20:59.000000 trytond_account_export_winbooks-7.2.1/view/account_fiscalyear_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      446 2024-04-30 17:20:59.000000 trytond_account_export_winbooks-7.2.1/view/account_journal_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      367 2024-04-30 17:20:59.000000 trytond_account_export_winbooks-7.2.1/view/account_tax_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      367 2024-04-30 17:20:59.000000 trytond_account_export_winbooks-7.2.1/view/account_tax_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      399 2024-04-30 17:20:59.000000 trytond_account_export_winbooks-7.2.1/view/party_party_list.xml
```

### Comparing `trytond_account_export_winbooks-7.2.0/COPYRIGHT` & `trytond_account_export_winbooks-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_account_export_winbooks-7.2.0/LICENSE` & `trytond_account_export_winbooks-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_export_winbooks-7.2.0/PKG-INFO` & `trytond_account_export_winbooks-7.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_account_export_winbooks
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module to export accounting to WinBooks
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account_export_winbooks-7.2.0/__init__.py` & `trytond_account_export_winbooks-7.2.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_export_winbooks-7.2.0/account.py` & `trytond_account_export_winbooks-7.2.1/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_export_winbooks-7.2.0/account.xml` & `trytond_account_export_winbooks-7.2.1/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_export_winbooks-7.2.0/account_be.xml` & `trytond_account_export_winbooks-7.2.1/account_be.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_export_winbooks-7.2.0/account_be_fr.xml` & `trytond_account_export_winbooks-7.2.1/account_be_fr.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_export_winbooks-7.2.0/account_be_nl.xml` & `trytond_account_export_winbooks-7.2.1/account_be_nl.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_export_winbooks-7.2.0/doc/conf.py` & `trytond_account_export_winbooks-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_account_export_winbooks-7.2.0/doc/design.rst` & `trytond_account_export_winbooks-7.2.1/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_export_winbooks-7.2.0/icons/LICENSE` & `trytond_account_export_winbooks-7.2.1/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_export_winbooks-7.2.0/message.xml` & `trytond_account_export_winbooks-7.2.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_export_winbooks-7.2.0/party.py` & `trytond_account_export_winbooks-7.2.1/party.py`

 * *Files identical despite different names*

### Comparing `trytond_account_export_winbooks-7.2.0/setup.py` & `trytond_account_export_winbooks-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_account_export_winbooks-7.2.0/tests/ACT.txt` & `trytond_account_export_winbooks-7.2.1/tests/ACT.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_export_winbooks-7.2.0/tests/scenario_account_export_winbooks.rst` & `trytond_account_export_winbooks-7.2.1/tests/scenario_account_export_winbooks.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_export_winbooks-7.2.0/tox.ini` & `trytond_account_export_winbooks-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_export_winbooks-7.2.0/trytond_account_export_winbooks.egg-info/PKG-INFO` & `trytond_account_export_winbooks-7.2.1/trytond_account_export_winbooks.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_account_export_winbooks
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module to export accounting to WinBooks
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account_export_winbooks-7.2.0/trytond_account_export_winbooks.egg-info/SOURCES.txt` & `trytond_account_export_winbooks-7.2.1/trytond_account_export_winbooks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

