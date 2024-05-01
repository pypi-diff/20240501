# Comparing `tmp/trytond_account_export-7.2.0.tar.gz` & `tmp/trytond_account_export-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_export-7.2.0.tar", last modified: Mon Apr 29 15:54:49 2024, max compression
+gzip compressed data, was "trytond_account_export-7.2.1.tar", last modified: Wed May  1 12:23:55 2024, max compression
```

## Comparing `trytond_account_export-7.2.0.tar` & `trytond_account_export-7.2.1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:49.690179 trytond_account_export-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)       71 2024-04-29 15:30:31.000000 trytond_account_export-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      670 2024-04-29 15:30:31.000000 trytond_account_export-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-27 16:30:39.000000 trytond_account_export-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-27 16:30:39.000000 trytond_account_export-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2653 2024-04-29 15:54:49.690179 trytond_account_export-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      244 2024-04-27 16:30:39.000000 trytond_account_export-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      425 2024-04-27 16:30:39.000000 trytond_account_export-7.2.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6984 2024-04-27 16:30:39.000000 trytond_account_export-7.2.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5672 2024-04-27 16:30:39.000000 trytond_account_export-7.2.0/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:49.686846 trytond_account_export-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3077 2024-04-27 16:30:39.000000 trytond_account_export-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      733 2024-04-27 16:30:39.000000 trytond_account_export-7.2.0/doc/configuration.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      959 2024-04-27 16:30:39.000000 trytond_account_export-7.2.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      244 2024-04-27 16:30:39.000000 trytond_account_export-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-27 16:30:39.000000 trytond_account_export-7.2.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-27 16:30:39.000000 trytond_account_export-7.2.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:49.686846 trytond_account_export-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_account_export-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_account_export-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_account_export-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_account_export-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_account_export-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_account_export-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_account_export-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_account_export-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_account_export-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_account_export-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_account_export-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_account_export-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_account_export-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_account_export-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_account_export-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_account_export-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_account_export-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_account_export-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_account_export-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_account_export-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_account_export-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_account_export-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_account_export-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 13:17:17.000000 trytond_account_export-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      423 2024-04-27 16:30:39.000000 trytond_account_export-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:54:49.690179 trytond_account_export-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4607 2024-04-27 16:30:39.000000 trytond_account_export-7.2.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:49.686846 trytond_account_export-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-27 16:30:39.000000 trytond_account_export-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2300 2024-04-27 16:30:39.000000 trytond_account_export-7.2.0/tests/scenario_account_export.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      328 2024-04-27 16:30:39.000000 trytond_account_export-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-27 16:30:39.000000 trytond_account_export-7.2.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-27 16:30:39.000000 trytond_account_export-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      100 2024-04-29 15:30:27.000000 trytond_account_export-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:49.690179 trytond_account_export-7.2.0/trytond_account_export.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2653 2024-04-29 15:54:49.000000 trytond_account_export-7.2.0/trytond_account_export.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1721 2024-04-29 15:54:49.000000 trytond_account_export-7.2.0/trytond_account_export.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:54:49.000000 trytond_account_export-7.2.0/trytond_account_export.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       66 2024-04-29 15:54:49.000000 trytond_account_export-7.2.0/trytond_account_export.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:54:49.000000 trytond_account_export-7.2.0/trytond_account_export.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       96 2024-04-29 15:54:49.000000 trytond_account_export-7.2.0/trytond_account_export.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:54:49.000000 trytond_account_export-7.2.0/trytond_account_export.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:49.690179 trytond_account_export-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      404 2024-04-27 16:30:39.000000 trytond_account_export-7.2.0/view/account_configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      716 2024-04-27 16:30:39.000000 trytond_account_export-7.2.0/view/account_move_export_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      266 2024-04-27 16:30:39.000000 trytond_account_export-7.2.0/view/account_move_export_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:23:55.842200 trytond_account_export-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)      172 2024-05-01 12:23:52.000000 trytond_account_export-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      670 2024-05-01 12:23:52.000000 trytond_account_export-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:20:59.000000 trytond_account_export-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:20:59.000000 trytond_account_export-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2653 2024-05-01 12:23:55.842200 trytond_account_export-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      244 2024-04-30 17:20:59.000000 trytond_account_export-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      425 2024-04-30 17:20:59.000000 trytond_account_export-7.2.1/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6984 2024-04-30 17:20:59.000000 trytond_account_export-7.2.1/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5672 2024-04-30 17:20:59.000000 trytond_account_export-7.2.1/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:23:55.838867 trytond_account_export-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3077 2024-04-30 17:20:59.000000 trytond_account_export-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      733 2024-04-30 17:20:59.000000 trytond_account_export-7.2.1/doc/configuration.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      959 2024-04-30 17:20:59.000000 trytond_account_export-7.2.1/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      244 2024-04-30 17:20:59.000000 trytond_account_export-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-30 17:20:59.000000 trytond_account_export-7.2.1/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:20:59.000000 trytond_account_export-7.2.1/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:23:55.838867 trytond_account_export-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2556 2024-04-30 17:21:59.000000 trytond_account_export-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3055 2024-04-30 17:21:59.000000 trytond_account_export-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2556 2024-04-30 17:21:59.000000 trytond_account_export-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3038 2024-04-30 17:21:59.000000 trytond_account_export-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3061 2024-04-30 17:21:59.000000 trytond_account_export-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2556 2024-04-30 17:21:59.000000 trytond_account_export-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2556 2024-04-30 17:21:59.000000 trytond_account_export-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2556 2024-04-30 17:21:59.000000 trytond_account_export-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2556 2024-04-30 17:21:59.000000 trytond_account_export-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3078 2024-04-30 17:21:59.000000 trytond_account_export-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2556 2024-04-30 17:21:59.000000 trytond_account_export-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2556 2024-04-30 17:21:59.000000 trytond_account_export-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2556 2024-04-30 17:21:59.000000 trytond_account_export-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2556 2024-04-30 17:21:59.000000 trytond_account_export-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2556 2024-04-30 17:21:59.000000 trytond_account_export-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3025 2024-04-30 17:21:59.000000 trytond_account_export-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2556 2024-04-30 17:21:59.000000 trytond_account_export-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2556 2024-04-30 17:21:59.000000 trytond_account_export-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2556 2024-04-30 17:21:59.000000 trytond_account_export-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2556 2024-04-30 17:21:59.000000 trytond_account_export-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2556 2024-04-30 17:21:59.000000 trytond_account_export-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2556 2024-04-30 17:21:59.000000 trytond_account_export-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2556 2024-04-30 17:21:59.000000 trytond_account_export-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2556 2024-04-30 17:21:59.000000 trytond_account_export-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      423 2024-04-30 17:20:59.000000 trytond_account_export-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 12:23:55.842200 trytond_account_export-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4607 2024-04-30 17:20:59.000000 trytond_account_export-7.2.1/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:23:55.838867 trytond_account_export-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:20:59.000000 trytond_account_export-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2300 2024-04-30 17:20:59.000000 trytond_account_export-7.2.1/tests/scenario_account_export.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      328 2024-04-30 17:20:59.000000 trytond_account_export-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:20:59.000000 trytond_account_export-7.2.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:20:59.000000 trytond_account_export-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      100 2024-04-30 17:21:06.000000 trytond_account_export-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:23:55.842200 trytond_account_export-7.2.1/trytond_account_export.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2653 2024-05-01 12:23:55.000000 trytond_account_export-7.2.1/trytond_account_export.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1721 2024-05-01 12:23:55.000000 trytond_account_export-7.2.1/trytond_account_export.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:23:55.000000 trytond_account_export-7.2.1/trytond_account_export.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       66 2024-05-01 12:23:55.000000 trytond_account_export-7.2.1/trytond_account_export.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:23:55.000000 trytond_account_export-7.2.1/trytond_account_export.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       96 2024-05-01 12:23:55.000000 trytond_account_export-7.2.1/trytond_account_export.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 12:23:55.000000 trytond_account_export-7.2.1/trytond_account_export.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:23:55.842200 trytond_account_export-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      404 2024-04-30 17:20:59.000000 trytond_account_export-7.2.1/view/account_configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      716 2024-04-30 17:20:59.000000 trytond_account_export-7.2.1/view/account_move_export_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      266 2024-04-30 17:20:59.000000 trytond_account_export-7.2.1/view/account_move_export_list.xml
```

### Comparing `trytond_account_export-7.2.0/COPYRIGHT` & `trytond_account_export-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_account_export-7.2.0/LICENSE` & `trytond_account_export-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_export-7.2.0/PKG-INFO` & `trytond_account_export-7.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_account_export
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module to export accounting to other software
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account_export-7.2.0/account.py` & `trytond_account_export-7.2.1/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_export-7.2.0/account.xml` & `trytond_account_export-7.2.1/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_export-7.2.0/doc/conf.py` & `trytond_account_export-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_account_export-7.2.0/doc/configuration.rst` & `trytond_account_export-7.2.1/doc/configuration.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_export-7.2.0/doc/design.rst` & `trytond_account_export-7.2.1/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_export-7.2.0/setup.py` & `trytond_account_export-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_account_export-7.2.0/tests/scenario_account_export.rst` & `trytond_account_export-7.2.1/tests/scenario_account_export.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_export-7.2.0/tox.ini` & `trytond_account_export-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_export-7.2.0/trytond_account_export.egg-info/PKG-INFO` & `trytond_account_export-7.2.1/trytond_account_export.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_account_export
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module to export accounting to other software
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account_export-7.2.0/trytond_account_export.egg-info/SOURCES.txt` & `trytond_account_export-7.2.1/trytond_account_export.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_export-7.2.0/view/account_move_export_form.xml` & `trytond_account_export-7.2.1/view/account_move_export_form.xml`

 * *Files identical despite different names*

