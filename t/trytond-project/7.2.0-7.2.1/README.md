# Comparing `tmp/trytond_project-7.2.0.tar.gz` & `tmp/trytond_project-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_project-7.2.0.tar", last modified: Mon Apr 29 15:44:40 2024, max compression
+gzip compressed data, was "trytond_project-7.2.1.tar", last modified: Wed May  1 11:48:23 2024, max compression
```

## Comparing `trytond_project-7.2.0.tar` & `trytond_project-7.2.1.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:40.802770 trytond_project-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     3638 2024-04-29 15:23:02.000000 trytond_project-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      728 2024-04-29 15:23:02.000000 trytond_project-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_project-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_project-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2736 2024-04-29 15:44:40.802770 trytond_project-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      203 2023-04-15 07:12:15.000000 trytond_project-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      589 2023-04-15 07:12:15.000000 trytond_project-7.2.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:40.799437 trytond_project-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3070 2024-04-27 16:30:39.000000 trytond_project-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3201 2023-04-15 07:12:15.000000 trytond_project-7.2.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      203 2023-04-15 07:12:15.000000 trytond_project-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_project-7.2.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:19.000000 trytond_project-7.2.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      868 2023-04-15 07:12:15.000000 trytond_project-7.2.0/doc/usage.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      320 2023-04-15 07:12:15.000000 trytond_project-7.2.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:40.799437 trytond_project-7.2.0/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_project-7.2.0/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      301 2023-01-16 14:00:21.000000 trytond_project-7.2.0/icons/tryton-project.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      548 2023-04-15 07:12:15.000000 trytond_project-7.2.0/ir.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:40.799437 trytond_project-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     7126 2024-04-27 16:43:25.000000 trytond_project-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7477 2024-04-27 16:43:25.000000 trytond_project-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6169 2024-04-27 16:43:25.000000 trytond_project-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7909 2024-04-27 16:43:25.000000 trytond_project-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7467 2024-04-27 16:43:25.000000 trytond_project-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6240 2024-04-27 16:43:25.000000 trytond_project-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6437 2024-04-27 16:43:25.000000 trytond_project-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7513 2024-04-27 16:43:25.000000 trytond_project-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6143 2024-04-27 16:43:25.000000 trytond_project-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7520 2024-04-27 16:43:25.000000 trytond_project-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6409 2024-04-27 16:43:25.000000 trytond_project-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5965 2024-04-27 16:43:25.000000 trytond_project-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6337 2024-04-27 16:43:25.000000 trytond_project-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6676 2024-04-27 16:43:25.000000 trytond_project-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6218 2024-04-27 16:43:25.000000 trytond_project-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7426 2024-04-27 16:43:25.000000 trytond_project-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6385 2024-04-27 16:43:25.000000 trytond_project-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7106 2024-04-27 16:43:25.000000 trytond_project-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7236 2024-04-29 13:17:17.000000 trytond_project-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7382 2024-04-27 16:43:25.000000 trytond_project-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7289 2024-04-27 16:43:25.000000 trytond_project-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6157 2024-04-27 16:43:25.000000 trytond_project-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5961 2024-04-27 16:43:25.000000 trytond_project-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7061 2024-04-27 16:43:25.000000 trytond_project-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1195 2023-04-15 07:12:15.000000 trytond_project-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1101 2023-04-15 07:12:15.000000 trytond_project-7.2.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1458 2023-04-15 07:12:15.000000 trytond_project-7.2.0/project.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:44:40.802770 trytond_project-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4519 2024-04-27 16:30:39.000000 trytond_project-7.2.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:40.799437 trytond_project-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_project-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2109 2024-04-22 12:14:36.000000 trytond_project-7.2.0/tests/scenario_project_status.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     7386 2023-04-15 07:12:15.000000 trytond_project-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_project-7.2.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1288 2023-04-15 07:12:15.000000 trytond_project-7.2.0/timesheet.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1117 2023-04-15 07:12:15.000000 trytond_project-7.2.0/timesheet.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:19.000000 trytond_project-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      165 2024-04-29 15:22:58.000000 trytond_project-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:40.802770 trytond_project-7.2.0/trytond_project.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2736 2024-04-29 15:44:40.000000 trytond_project-7.2.0/trytond_project.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2046 2024-04-29 15:44:40.000000 trytond_project-7.2.0/trytond_project.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:44:40.000000 trytond_project-7.2.0/trytond_project.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       52 2024-04-29 15:44:40.000000 trytond_project-7.2.0/trytond_project.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:01.000000 trytond_project-7.2.0/trytond_project.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      174 2024-04-29 15:44:40.000000 trytond_project-7.2.0/trytond_project.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:44:40.000000 trytond_project-7.2.0/trytond_project.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:40.802770 trytond_project-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)     2346 2023-04-15 07:12:15.000000 trytond_project-7.2.0/view/work_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      541 2023-04-15 07:12:15.000000 trytond_project-7.2.0/view/work_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      405 2023-04-15 07:12:15.000000 trytond_project-7.2.0/view/work_list_children.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      356 2023-04-15 07:12:15.000000 trytond_project-7.2.0/view/work_list_simple.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      887 2023-04-15 07:12:15.000000 trytond_project-7.2.0/view/work_status_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_project-7.2.0/view/work_status_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      537 2023-04-15 07:12:15.000000 trytond_project-7.2.0/view/work_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      372 2023-04-15 07:12:15.000000 trytond_project-7.2.0/view/work_tree_simple.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    16077 2024-01-27 09:58:52.000000 trytond_project-7.2.0/work.py
--rw-r--r--   0 ced       (1000) ced       (1000)    11944 2024-04-27 16:30:39.000000 trytond_project-7.2.0/work.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:48:23.950807 trytond_project-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3739 2024-05-01 11:48:20.000000 trytond_project-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      728 2024-05-01 11:48:20.000000 trytond_project-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:21:00.000000 trytond_project-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:21:00.000000 trytond_project-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2736 2024-05-01 11:48:23.950807 trytond_project-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      203 2024-04-30 17:21:00.000000 trytond_project-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      589 2024-04-30 17:21:00.000000 trytond_project-7.2.1/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:48:23.947474 trytond_project-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3070 2024-04-30 17:21:00.000000 trytond_project-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3201 2024-04-30 17:21:00.000000 trytond_project-7.2.1/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      203 2024-04-30 17:21:00.000000 trytond_project-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-30 17:21:00.000000 trytond_project-7.2.1/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:21:00.000000 trytond_project-7.2.1/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      868 2024-04-30 17:21:00.000000 trytond_project-7.2.1/doc/usage.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      320 2024-04-30 17:21:00.000000 trytond_project-7.2.1/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:48:23.947474 trytond_project-7.2.1/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2024-04-30 17:21:00.000000 trytond_project-7.2.1/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      301 2024-04-30 17:21:00.000000 trytond_project-7.2.1/icons/tryton-project.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      548 2024-04-30 17:21:00.000000 trytond_project-7.2.1/ir.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:48:23.947474 trytond_project-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     7126 2024-04-30 17:21:00.000000 trytond_project-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7477 2024-04-30 17:21:00.000000 trytond_project-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6169 2024-04-30 17:21:00.000000 trytond_project-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7922 2024-04-30 17:21:59.000000 trytond_project-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7467 2024-04-30 17:21:00.000000 trytond_project-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6240 2024-04-30 17:21:00.000000 trytond_project-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6437 2024-04-30 17:21:00.000000 trytond_project-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7513 2024-04-30 17:21:00.000000 trytond_project-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6143 2024-04-30 17:21:00.000000 trytond_project-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7520 2024-04-30 17:21:00.000000 trytond_project-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6409 2024-04-30 17:21:00.000000 trytond_project-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5965 2024-04-30 17:21:00.000000 trytond_project-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6337 2024-04-30 17:21:00.000000 trytond_project-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6676 2024-04-30 17:21:00.000000 trytond_project-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6218 2024-04-30 17:21:00.000000 trytond_project-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7426 2024-04-30 17:21:00.000000 trytond_project-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6397 2024-04-30 17:21:59.000000 trytond_project-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7106 2024-04-30 17:21:00.000000 trytond_project-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7236 2024-04-30 17:21:00.000000 trytond_project-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7382 2024-04-30 17:21:00.000000 trytond_project-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7289 2024-04-30 17:21:00.000000 trytond_project-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6157 2024-04-30 17:21:00.000000 trytond_project-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5961 2024-04-30 17:21:00.000000 trytond_project-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7061 2024-04-30 17:21:00.000000 trytond_project-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1195 2024-04-30 17:21:00.000000 trytond_project-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1101 2024-04-30 17:21:00.000000 trytond_project-7.2.1/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1458 2024-04-30 17:21:00.000000 trytond_project-7.2.1/project.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 11:48:23.950807 trytond_project-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4519 2024-04-30 17:21:00.000000 trytond_project-7.2.1/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:48:23.947474 trytond_project-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:21:00.000000 trytond_project-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2109 2024-04-30 17:21:00.000000 trytond_project-7.2.1/tests/scenario_project_status.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     7386 2024-04-30 17:21:00.000000 trytond_project-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:21:00.000000 trytond_project-7.2.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1288 2024-04-30 17:21:00.000000 trytond_project-7.2.1/timesheet.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1117 2024-04-30 17:21:00.000000 trytond_project-7.2.1/timesheet.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:21:00.000000 trytond_project-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      165 2024-04-30 17:21:06.000000 trytond_project-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:48:23.950807 trytond_project-7.2.1/trytond_project.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2736 2024-05-01 11:48:23.000000 trytond_project-7.2.1/trytond_project.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2046 2024-05-01 11:48:23.000000 trytond_project-7.2.1/trytond_project.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:48:23.000000 trytond_project-7.2.1/trytond_project.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       52 2024-05-01 11:48:23.000000 trytond_project-7.2.1/trytond_project.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:48:23.000000 trytond_project-7.2.1/trytond_project.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      174 2024-05-01 11:48:23.000000 trytond_project-7.2.1/trytond_project.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 11:48:23.000000 trytond_project-7.2.1/trytond_project.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:48:23.950807 trytond_project-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2346 2024-04-30 17:21:00.000000 trytond_project-7.2.1/view/work_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      541 2024-04-30 17:21:00.000000 trytond_project-7.2.1/view/work_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      405 2024-04-30 17:21:00.000000 trytond_project-7.2.1/view/work_list_children.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      356 2024-04-30 17:21:00.000000 trytond_project-7.2.1/view/work_list_simple.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      887 2024-04-30 17:21:00.000000 trytond_project-7.2.1/view/work_status_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:21:00.000000 trytond_project-7.2.1/view/work_status_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      537 2024-04-30 17:21:00.000000 trytond_project-7.2.1/view/work_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      372 2024-04-30 17:21:00.000000 trytond_project-7.2.1/view/work_tree_simple.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    16077 2024-04-30 17:21:00.000000 trytond_project-7.2.1/work.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    11944 2024-04-30 17:21:00.000000 trytond_project-7.2.1/work.xml
```

### Comparing `trytond_project-7.2.0/CHANGELOG` & `trytond_project-7.2.1/CHANGELOG`

 * *Files 2% similar despite different names*

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

### Comparing `trytond_project-7.2.0/COPYRIGHT` & `trytond_project-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_project-7.2.0/LICENSE` & `trytond_project-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_project-7.2.0/PKG-INFO` & `trytond_project-7.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_project
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module with projects
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_project-7.2.0/__init__.py` & `trytond_project-7.2.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_project-7.2.0/doc/conf.py` & `trytond_project-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_project-7.2.0/doc/design.rst` & `trytond_project-7.2.1/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_project-7.2.0/doc/usage.rst` & `trytond_project-7.2.1/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `trytond_project-7.2.0/icons/LICENSE` & `trytond_project-7.2.1/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_project-7.2.0/ir.py` & `trytond_project-7.2.1/ir.py`

 * *Files identical despite different names*

### Comparing `trytond_project-7.2.0/locale/bg.po` & `trytond_project-7.2.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_project-7.2.0/locale/ca.po` & `trytond_project-7.2.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_project-7.2.0/locale/cs.po` & `trytond_project-7.2.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_project-7.2.0/locale/de.po` & `trytond_project-7.2.1/locale/de.po`

 * *Files 1% similar despite different names*

```diff
@@ -188,16 +188,16 @@
 msgstr ""
 "Partei \"%(party)s\" kann nicht gelöscht werden solange für sie noch offene "
 "Projekte bei Unternehmen \"%(company)s\" bestehen."
 
 msgctxt "model:ir.message,text:msg_work_children_progress"
 msgid "To complete work \"%(work)s\" you must complete also all its children."
 msgstr ""
-"Um Projekt \"%(parent)s\" abschließen zu können, muss zuerst das "
-"untergeordnete Projekt \"%(child)s\" abgeschlossen werden."
+"Um das Projekt/die Projektaufgabe \"%(work)s\" abschließen zu können, müssen"
+" auch alle zugehörigen Unteraufgaben abgeschlossen werden."
 
 msgctxt "model:ir.message,text:msg_work_invalid_progress_status"
 msgid ""
 "To set work \"%(work)s\" in \"%(status)s\" status, you must increase its "
 "progress up to at least %(progress)s."
 msgstr ""
 "Um \"%(work)s\" in den Status \"%(status)s\" setzen zu können, muss der "
@@ -207,15 +207,15 @@
 msgid "To re-open work \"%(work)s\" you must re-open also its parent \"%(parent)s\"."
 msgstr ""
 "Um das Projekt \"%(work)s\" wieder öffnen zu können, muss zuerst das "
 "übergeordnete Projekt \"%(parent)s\" wieder geöffnet werden."
 
 msgctxt "model:ir.rule.group,name:rule_group_work_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.ui.menu,name:menu_configuration"
 msgid "Configuration"
 msgstr "Einstellungen"
 
 msgctxt "model:ir.ui.menu,name:menu_project"
 msgid "Projects"
```

### Comparing `trytond_project-7.2.0/locale/es.po` & `trytond_project-7.2.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_project-7.2.0/locale/es_419.po` & `trytond_project-7.2.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_project-7.2.0/locale/et.po` & `trytond_project-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_project-7.2.0/locale/fa.po` & `trytond_project-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_project-7.2.0/locale/fi.po` & `trytond_project-7.2.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_project-7.2.0/locale/fr.po` & `trytond_project-7.2.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_project-7.2.0/locale/hu.po` & `trytond_project-7.2.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_project-7.2.0/locale/id.po` & `trytond_project-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_project-7.2.0/locale/it.po` & `trytond_project-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_project-7.2.0/locale/lo.po` & `trytond_project-7.2.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_project-7.2.0/locale/lt.po` & `trytond_project-7.2.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_project-7.2.0/locale/nl.po` & `trytond_project-7.2.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_project-7.2.0/locale/pl.po` & `trytond_project-7.2.1/locale/pl.po`

 * *Files 0% similar despite different names*

```diff
@@ -225,15 +225,15 @@
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_project_tree"
 msgid "Projects"
 msgstr "Projects"
 
 msgctxt "model:ir.ui.menu,name:menu_reporting"
 msgid "Reporting"
-msgstr ""
+msgstr "Raportowanie"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_task_form"
 msgid "Tasks"
 msgstr "Tasks"
 
 #, fuzzy
```

### Comparing `trytond_project-7.2.0/locale/pt.po` & `trytond_project-7.2.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_project-7.2.0/locale/ro.po` & `trytond_project-7.2.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_project-7.2.0/locale/ru.po` & `trytond_project-7.2.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_project-7.2.0/locale/sl.po` & `trytond_project-7.2.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_project-7.2.0/locale/tr.po` & `trytond_project-7.2.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_project-7.2.0/locale/uk.po` & `trytond_project-7.2.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_project-7.2.0/locale/zh_CN.po` & `trytond_project-7.2.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_project-7.2.0/message.xml` & `trytond_project-7.2.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_project-7.2.0/party.py` & `trytond_project-7.2.1/party.py`

 * *Files identical despite different names*

### Comparing `trytond_project-7.2.0/project.xml` & `trytond_project-7.2.1/project.xml`

 * *Files identical despite different names*

### Comparing `trytond_project-7.2.0/setup.py` & `trytond_project-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_project-7.2.0/tests/scenario_project_status.rst` & `trytond_project-7.2.1/tests/scenario_project_status.rst`

 * *Files identical despite different names*

### Comparing `trytond_project-7.2.0/tests/test_module.py` & `trytond_project-7.2.1/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_project-7.2.0/timesheet.py` & `trytond_project-7.2.1/timesheet.py`

 * *Files identical despite different names*

### Comparing `trytond_project-7.2.0/timesheet.xml` & `trytond_project-7.2.1/timesheet.xml`

 * *Files identical despite different names*

### Comparing `trytond_project-7.2.0/tox.ini` & `trytond_project-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_project-7.2.0/trytond_project.egg-info/PKG-INFO` & `trytond_project-7.2.1/trytond_project.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_project
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module with projects
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_project-7.2.0/trytond_project.egg-info/SOURCES.txt` & `trytond_project-7.2.1/trytond_project.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_project-7.2.0/view/work_form.xml` & `trytond_project-7.2.1/view/work_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_project-7.2.0/view/work_list.xml` & `trytond_project-7.2.1/view/work_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_project-7.2.0/view/work_status_form.xml` & `trytond_project-7.2.1/view/work_status_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_project-7.2.0/view/work_tree.xml` & `trytond_project-7.2.1/view/work_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_project-7.2.0/work.py` & `trytond_project-7.2.1/work.py`

 * *Files identical despite different names*

### Comparing `trytond_project-7.2.0/work.xml` & `trytond_project-7.2.1/work.xml`

 * *Files identical despite different names*

