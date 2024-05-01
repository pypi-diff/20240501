# Comparing `tmp/trytond_country-7.2.0.tar.gz` & `tmp/trytond_country-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_country-7.2.0.tar", last modified: Mon Apr 29 15:39:36 2024, max compression
+gzip compressed data, was "trytond_country-7.2.1.tar", last modified: Wed May  1 11:59:46 2024, max compression
```

## Comparing `trytond_country-7.2.0.tar` & `trytond_country-7.2.1.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:36.910719 trytond_country-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     3959 2024-04-29 15:19:06.000000 trytond_country-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      763 2024-04-29 15:19:05.000000 trytond_country-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_country-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_country-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3047 2024-04-29 15:39:36.910719 trytond_country-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      390 2023-04-15 07:12:15.000000 trytond_country-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      506 2023-04-15 07:12:15.000000 trytond_country-7.2.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    20545 2024-01-27 09:58:52.000000 trytond_country-7.2.0/country.py
--rw-r--r--   0 ced       (1000) ced       (1000)    13242 2024-04-27 16:30:39.000000 trytond_country-7.2.0/country.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:36.904052 trytond_country-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3070 2024-04-27 16:30:39.000000 trytond_country-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2738 2023-04-15 07:12:15.000000 trytond_country-7.2.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      390 2023-04-15 07:12:15.000000 trytond_country-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_country-7.2.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:08.000000 trytond_country-7.2.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     1114 2024-01-27 09:58:52.000000 trytond_country-7.2.0/doc/setup.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      379 2023-04-15 07:12:15.000000 trytond_country-7.2.0/doc/usage.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:36.904052 trytond_country-7.2.0/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_country-7.2.0/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      186 2023-01-16 14:00:20.000000 trytond_country-7.2.0/icons/tryton-country.svg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:36.907385 trytond_country-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    25666 2024-04-27 16:43:22.000000 trytond_country-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    25651 2024-04-27 16:43:22.000000 trytond_country-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    22688 2024-04-27 16:43:22.000000 trytond_country-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    25659 2024-04-27 16:43:22.000000 trytond_country-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    25807 2024-04-27 16:43:22.000000 trytond_country-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    22530 2024-04-27 16:43:23.000000 trytond_country-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    24628 2024-04-27 16:43:23.000000 trytond_country-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    25889 2024-04-27 16:43:23.000000 trytond_country-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    22571 2024-04-27 16:43:23.000000 trytond_country-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    25743 2024-04-27 16:43:23.000000 trytond_country-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    23696 2024-04-27 16:43:23.000000 trytond_country-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    21710 2024-04-27 16:43:23.000000 trytond_country-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    22889 2024-04-27 16:43:23.000000 trytond_country-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    25695 2024-04-27 16:43:23.000000 trytond_country-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    25164 2024-04-27 16:43:23.000000 trytond_country-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    25469 2024-04-27 16:43:23.000000 trytond_country-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    25421 2024-04-27 16:43:23.000000 trytond_country-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    25039 2024-04-27 16:43:23.000000 trytond_country-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    26032 2024-04-29 13:17:17.000000 trytond_country-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    26709 2024-04-27 16:43:23.000000 trytond_country-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    24710 2024-04-27 16:43:23.000000 trytond_country-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    22475 2024-04-27 16:43:23.000000 trytond_country-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    27230 2024-04-27 16:43:23.000000 trytond_country-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    23032 2024-04-27 16:43:23.000000 trytond_country-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4126 2023-04-15 07:12:15.000000 trytond_country-7.2.0/organization.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     8410 2023-04-15 07:12:15.000000 trytond_country-7.2.0/region.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:36.907385 trytond_country-7.2.0/scripts/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_country-7.2.0/scripts/__init__.py
--rwxr-xr-x   0 ced       (1000) ced       (1000)    19896 2024-02-04 18:51:26.000000 trytond_country-7.2.0/scripts/import_countries.py
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4041 2024-02-04 18:51:26.000000 trytond_country-7.2.0/scripts/import_postal_codes.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:39:36.910719 trytond_country-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4900 2024-04-27 16:30:39.000000 trytond_country-7.2.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:36.907385 trytond_country-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_country-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      571 2024-04-22 12:14:36.000000 trytond_country-7.2.0/tests/scenario_country_import.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3259 2023-04-15 07:12:15.000000 trytond_country-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_country-7.2.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:08.000000 trytond_country-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      104 2024-04-29 15:19:01.000000 trytond_country-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:36.910719 trytond_country-7.2.0/trytond_country.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3047 2024-04-29 15:39:36.000000 trytond_country-7.2.0/trytond_country.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2420 2024-04-29 15:39:36.000000 trytond_country-7.2.0/trytond_country.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:39:36.000000 trytond_country-7.2.0/trytond_country.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      255 2024-04-29 15:39:36.000000 trytond_country-7.2.0/trytond_country.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:07.000000 trytond_country-7.2.0/trytond_country.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      157 2024-04-29 15:39:36.000000 trytond_country-7.2.0/trytond_country.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:39:36.000000 trytond_country-7.2.0/trytond_country.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:36.910719 trytond_country-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      607 2023-04-15 07:12:15.000000 trytond_country-7.2.0/view/country_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      438 2023-04-15 07:12:15.000000 trytond_country-7.2.0/view/country_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      327 2023-04-15 07:12:15.000000 trytond_country-7.2.0/view/organization_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      260 2023-04-15 07:12:15.000000 trytond_country-7.2.0/view/organization_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      425 2023-04-15 07:12:15.000000 trytond_country-7.2.0/view/organization_member_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      353 2023-04-15 07:12:15.000000 trytond_country-7.2.0/view/organization_member_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      420 2023-04-15 07:12:15.000000 trytond_country-7.2.0/view/postal_code_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      347 2023-04-15 07:12:15.000000 trytond_country-7.2.0/view/postal_code_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      444 2023-04-15 07:12:15.000000 trytond_country-7.2.0/view/region_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      268 2023-04-15 07:12:15.000000 trytond_country-7.2.0/view/region_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      285 2023-04-15 07:12:15.000000 trytond_country-7.2.0/view/region_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      523 2023-04-15 07:12:15.000000 trytond_country-7.2.0/view/subdivision_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      272 2023-04-15 07:12:15.000000 trytond_country-7.2.0/view/subdivision_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:59:46.372959 trytond_country-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4060 2024-05-01 11:59:43.000000 trytond_country-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      763 2024-05-01 11:59:42.000000 trytond_country-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:20:59.000000 trytond_country-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:20:59.000000 trytond_country-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3047 2024-05-01 11:59:46.372959 trytond_country-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      390 2024-04-30 17:20:59.000000 trytond_country-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      506 2024-04-30 17:20:59.000000 trytond_country-7.2.1/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    20545 2024-04-30 17:20:59.000000 trytond_country-7.2.1/country.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    13242 2024-04-30 17:20:59.000000 trytond_country-7.2.1/country.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:59:46.366293 trytond_country-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3070 2024-04-30 17:20:59.000000 trytond_country-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2738 2024-04-30 17:20:59.000000 trytond_country-7.2.1/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      390 2024-04-30 17:20:59.000000 trytond_country-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-30 17:20:59.000000 trytond_country-7.2.1/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:20:59.000000 trytond_country-7.2.1/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     1114 2024-04-30 17:20:59.000000 trytond_country-7.2.1/doc/setup.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      379 2024-04-30 17:20:59.000000 trytond_country-7.2.1/doc/usage.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:59:46.366293 trytond_country-7.2.1/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2024-04-30 17:20:59.000000 trytond_country-7.2.1/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      186 2024-04-30 17:20:59.000000 trytond_country-7.2.1/icons/tryton-country.svg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:59:46.369626 trytond_country-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    25666 2024-04-30 17:20:59.000000 trytond_country-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    25651 2024-04-30 17:20:59.000000 trytond_country-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    22688 2024-04-30 17:20:59.000000 trytond_country-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    25659 2024-04-30 17:20:59.000000 trytond_country-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    25807 2024-04-30 17:20:59.000000 trytond_country-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    22530 2024-04-30 17:20:59.000000 trytond_country-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    24628 2024-04-30 17:20:59.000000 trytond_country-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    25889 2024-04-30 17:20:59.000000 trytond_country-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    22571 2024-04-30 17:20:59.000000 trytond_country-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    25743 2024-04-30 17:20:59.000000 trytond_country-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    23696 2024-04-30 17:20:59.000000 trytond_country-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    21710 2024-04-30 17:20:59.000000 trytond_country-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    22889 2024-04-30 17:20:59.000000 trytond_country-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    25695 2024-04-30 17:20:59.000000 trytond_country-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    25164 2024-04-30 17:20:59.000000 trytond_country-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    25469 2024-04-30 17:20:59.000000 trytond_country-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    25723 2024-04-30 17:21:59.000000 trytond_country-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    25039 2024-04-30 17:20:59.000000 trytond_country-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    26032 2024-04-30 17:20:59.000000 trytond_country-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    26709 2024-04-30 17:20:59.000000 trytond_country-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    24710 2024-04-30 17:20:59.000000 trytond_country-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    22475 2024-04-30 17:20:59.000000 trytond_country-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    27230 2024-04-30 17:20:59.000000 trytond_country-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    23032 2024-04-30 17:20:59.000000 trytond_country-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4126 2024-04-30 17:20:59.000000 trytond_country-7.2.1/organization.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     8410 2024-04-30 17:20:59.000000 trytond_country-7.2.1/region.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:59:46.369626 trytond_country-7.2.1/scripts/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:20:59.000000 trytond_country-7.2.1/scripts/__init__.py
+-rwxr-xr-x   0 ced       (1000) ced       (1000)    19896 2024-04-30 17:20:59.000000 trytond_country-7.2.1/scripts/import_countries.py
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4041 2024-04-30 17:20:59.000000 trytond_country-7.2.1/scripts/import_postal_codes.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 11:59:46.372959 trytond_country-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4900 2024-04-30 17:20:59.000000 trytond_country-7.2.1/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:59:46.369626 trytond_country-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:20:59.000000 trytond_country-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      571 2024-04-30 17:20:59.000000 trytond_country-7.2.1/tests/scenario_country_import.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3259 2024-04-30 17:20:59.000000 trytond_country-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:20:59.000000 trytond_country-7.2.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:20:59.000000 trytond_country-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      104 2024-04-30 17:21:06.000000 trytond_country-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:59:46.369626 trytond_country-7.2.1/trytond_country.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3047 2024-05-01 11:59:45.000000 trytond_country-7.2.1/trytond_country.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2420 2024-05-01 11:59:46.000000 trytond_country-7.2.1/trytond_country.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:59:45.000000 trytond_country-7.2.1/trytond_country.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      255 2024-05-01 11:59:45.000000 trytond_country-7.2.1/trytond_country.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:59:45.000000 trytond_country-7.2.1/trytond_country.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      157 2024-05-01 11:59:45.000000 trytond_country-7.2.1/trytond_country.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 11:59:45.000000 trytond_country-7.2.1/trytond_country.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:59:46.369626 trytond_country-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      607 2024-04-30 17:20:59.000000 trytond_country-7.2.1/view/country_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      438 2024-04-30 17:20:59.000000 trytond_country-7.2.1/view/country_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      327 2024-04-30 17:20:59.000000 trytond_country-7.2.1/view/organization_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      260 2024-04-30 17:20:59.000000 trytond_country-7.2.1/view/organization_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      425 2024-04-30 17:20:59.000000 trytond_country-7.2.1/view/organization_member_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      353 2024-04-30 17:20:59.000000 trytond_country-7.2.1/view/organization_member_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      420 2024-04-30 17:20:59.000000 trytond_country-7.2.1/view/postal_code_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      347 2024-04-30 17:20:59.000000 trytond_country-7.2.1/view/postal_code_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      444 2024-04-30 17:20:59.000000 trytond_country-7.2.1/view/region_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      268 2024-04-30 17:20:59.000000 trytond_country-7.2.1/view/region_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      285 2024-04-30 17:20:59.000000 trytond_country-7.2.1/view/region_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      523 2024-04-30 17:20:59.000000 trytond_country-7.2.1/view/subdivision_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      272 2024-04-30 17:20:59.000000 trytond_country-7.2.1/view/subdivision_tree.xml
```

### Comparing `trytond_country-7.2.0/CHANGELOG` & `trytond_country-7.2.1/CHANGELOG`

 * *Files 3% similar despite different names*

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

### Comparing `trytond_country-7.2.0/COPYRIGHT` & `trytond_country-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_country-7.2.0/LICENSE` & `trytond_country-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_country-7.2.0/PKG-INFO` & `trytond_country-7.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_country
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module with countries
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_country-7.2.0/country.py` & `trytond_country-7.2.1/country.py`

 * *Files identical despite different names*

### Comparing `trytond_country-7.2.0/country.xml` & `trytond_country-7.2.1/country.xml`

 * *Files identical despite different names*

### Comparing `trytond_country-7.2.0/doc/conf.py` & `trytond_country-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_country-7.2.0/doc/design.rst` & `trytond_country-7.2.1/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_country-7.2.0/doc/setup.rst` & `trytond_country-7.2.1/doc/setup.rst`

 * *Files identical despite different names*

### Comparing `trytond_country-7.2.0/icons/LICENSE` & `trytond_country-7.2.1/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_country-7.2.0/locale/bg.po` & `trytond_country-7.2.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_country-7.2.0/locale/ca.po` & `trytond_country-7.2.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_country-7.2.0/locale/cs.po` & `trytond_country-7.2.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_country-7.2.0/locale/de.po` & `trytond_country-7.2.1/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_country-7.2.0/locale/es.po` & `trytond_country-7.2.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_country-7.2.0/locale/es_419.po` & `trytond_country-7.2.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_country-7.2.0/locale/et.po` & `trytond_country-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_country-7.2.0/locale/fa.po` & `trytond_country-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_country-7.2.0/locale/fi.po` & `trytond_country-7.2.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_country-7.2.0/locale/fr.po` & `trytond_country-7.2.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_country-7.2.0/locale/hu.po` & `trytond_country-7.2.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_country-7.2.0/locale/id.po` & `trytond_country-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_country-7.2.0/locale/it.po` & `trytond_country-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_country-7.2.0/locale/lo.po` & `trytond_country-7.2.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_country-7.2.0/locale/lt.po` & `trytond_country-7.2.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_country-7.2.0/locale/nl.po` & `trytond_country-7.2.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_country-7.2.0/locale/pl.po` & `trytond_country-7.2.1/locale/pt.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,205 +1,210 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:country.country,code3:"
 msgid "3-letters Code"
-msgstr "Kod trzyliterowy"
+msgstr "Código de três letras"
 
 msgctxt "field:country.country,code:"
 msgid "Code"
-msgstr "Kod"
+msgstr "Código"
 
 msgctxt "field:country.country,code_numeric:"
 msgid "Numeric Code"
-msgstr "Kod numeryczny"
+msgstr "Código numérico"
 
 msgctxt "field:country.country,flag:"
 msgid "Flag"
 msgstr ""
 
 msgctxt "field:country.country,members:"
 msgid "Members"
 msgstr ""
 
 msgctxt "field:country.country,name:"
 msgid "Name"
-msgstr "Nazwa"
+msgstr "Nome"
 
 msgctxt "field:country.country,organizations:"
 msgid "Organizations"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:country.country,region:"
 msgid "Region"
 msgstr "Region"
 
 msgctxt "field:country.country,subdivisions:"
 msgid "Subdivisions"
-msgstr "Jednostki podrzędne"
+msgstr "Subdivisões"
 
 #, fuzzy
 msgctxt "field:country.organization,code:"
 msgid "Code"
-msgstr "Kod"
+msgstr "Código"
 
 #, fuzzy
 msgctxt "field:country.organization,countries:"
 msgid "Countries"
-msgstr "Kraje"
+msgstr "Países"
 
 msgctxt "field:country.organization,members:"
 msgid "Members"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:country.organization,name:"
 msgid "Name"
-msgstr "Nazwa"
+msgstr "Nome"
 
+#, fuzzy
 msgctxt "field:country.organization.member,active:"
 msgid "Active"
-msgstr ""
+msgstr "Ativo"
 
 #, fuzzy
 msgctxt "field:country.organization.member,country:"
 msgid "Country"
-msgstr "Kraj"
+msgstr "País"
 
 #, fuzzy
 msgctxt "field:country.organization.member,from_date:"
 msgid "From Date"
-msgstr "Data zapisu"
+msgstr "Data de Edição"
 
 msgctxt "field:country.organization.member,organization:"
 msgid "Organization"
 msgstr ""
 
 msgctxt "field:country.organization.member,to_date:"
 msgid "To Date"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:country.postal_code,city:"
 msgid "City"
-msgstr "Miejscowość"
+msgstr "Cidade"
 
+#, fuzzy
 msgctxt "field:country.postal_code,country:"
 msgid "Country"
-msgstr "Kraj"
+msgstr "País"
 
 msgctxt "field:country.postal_code,postal_code:"
 msgid "Postal Code"
-msgstr "Kod pocztowy"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:country.postal_code,subdivision:"
 msgid "Subdivision"
-msgstr "Jednostka podrzędna"
+msgstr "Subdivisão"
 
 #, fuzzy
 msgctxt "field:country.region,code_numeric:"
 msgid "Numeric Code"
-msgstr "Kod numeryczny"
+msgstr "Código numérico"
 
 #, fuzzy
 msgctxt "field:country.region,countries:"
 msgid "Countries"
-msgstr "Kraje"
+msgstr "Países"
 
 #, fuzzy
 msgctxt "field:country.region,name:"
 msgid "Name"
-msgstr "Nazwa"
+msgstr "Nome"
 
 #, fuzzy
 msgctxt "field:country.region,parent:"
 msgid "Parent"
-msgstr "Jednostka nadrzędna"
+msgstr "Pai"
 
 #, fuzzy
 msgctxt "field:country.region,subregions:"
 msgid "Subregions"
-msgstr "Region Południe"
+msgstr "Southern Region"
 
 msgctxt "field:country.subdivision,code:"
 msgid "Code"
-msgstr "Kod"
+msgstr "Código"
 
 msgctxt "field:country.subdivision,country:"
 msgid "Country"
-msgstr "Kraj"
+msgstr "País"
 
 msgctxt "field:country.subdivision,flag:"
 msgid "Flag"
 msgstr ""
 
 msgctxt "field:country.subdivision,name:"
 msgid "Name"
-msgstr "Nazwa"
+msgstr "Nome"
 
 msgctxt "field:country.subdivision,parent:"
 msgid "Parent"
-msgstr "Jednostka nadrzędna"
+msgstr "Pai"
 
 msgctxt "field:country.subdivision,type:"
 msgid "Type"
-msgstr "Typ"
+msgstr "Editado por"
 
 msgctxt "help:country.country,code3:"
 msgid "The 3 chars ISO country code."
-msgstr "Trzyliterowy kod ISO kraju."
+msgstr "O código ISO de 3 caracteres do país."
 
 msgctxt "help:country.country,code:"
 msgid "The 2 chars ISO country code."
-msgstr "Dwuliterowy kod ISO kraju."
+msgstr "O código ISO de 2 caracteres do país."
 
 msgctxt "help:country.country,code_numeric:"
 msgid "The ISO numeric country code."
-msgstr "Cyfrowy kod ISO kraju."
+msgstr "O código numérico ISO do país."
 
 msgctxt "help:country.country,name:"
 msgid "The main identifier of the country."
-msgstr "Główny identyfikator kraju."
+msgstr "O identificador principal do país."
 
 msgctxt "help:country.postal_code,city:"
 msgid "The city associated with the postal code."
-msgstr "Miejscowość powiązana z kodem pocztowym."
+msgstr ""
 
 msgctxt "help:country.postal_code,country:"
 msgid "The country that contains the postal code."
-msgstr "Kraj, który zawiera kod pocztowy."
+msgstr ""
 
+#, fuzzy
 msgctxt "help:country.postal_code,subdivision:"
 msgid "The subdivision where the postal code is."
-msgstr "Jednostka podrzędna, w której występuje kod pocztowy."
+msgstr "A subdivisão em que o código postal (CEP) está."
 
 msgctxt "help:country.region,code_numeric:"
 msgid "UN M49 region code."
 msgstr ""
 
 msgctxt "help:country.subdivision,code:"
 msgid "The ISO code of the subdivision."
-msgstr "Kod ISO jednostki podrzędnej."
+msgstr "O código ISO da subdivisão."
 
 msgctxt "help:country.subdivision,country:"
 msgid "The country where this subdivision is."
-msgstr "Kraj, w którym znajduje się jednostka podrzędna."
+msgstr "O país em que a subdivisão está."
 
 msgctxt "help:country.subdivision,name:"
 msgid "The main identifier of the subdivision."
-msgstr "Główny identyfikator jednostki podrzędnej."
+msgstr "O identificador principal da subdivisão."
 
 msgctxt "help:country.subdivision,parent:"
 msgid "Add subdivision below the parent."
-msgstr "Dodaj jednostkę podrzędną."
+msgstr "Adicionar subdivisão abaixo do pai."
 
 msgctxt "model:country.country,name:"
 msgid "Country"
-msgstr "Kraj"
+msgstr "País"
 
 msgctxt "model:country.organization,name:"
 msgid "Organization"
 msgstr ""
 
 msgctxt "model:country.organization,name:organization_amu"
 msgid "Arab Maghreb Union"
@@ -216,20 +221,20 @@
 msgctxt "model:country.organization,name:organization_benelux"
 msgid "Benelux Union"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:country.organization,name:organization_can"
 msgid "Andean Community"
-msgstr "Wspólnota autonomiczna"
+msgstr "Autonomous community"
 
 #, fuzzy
 msgctxt "model:country.organization,name:organization_caricom"
 msgid "Caribbean Community"
-msgstr "Wspólnota autonomiczna"
+msgstr "Autonomous community"
 
 msgctxt "model:country.organization,name:organization_cemac"
 msgid "Economic and Monetary Community of Central Africa"
 msgstr ""
 
 msgctxt "model:country.organization,name:organization_cen-sad"
 msgid "Community of Sahel–Saharan States"
@@ -238,15 +243,15 @@
 msgctxt "model:country.organization,name:organization_comesa"
 msgid "Common Market for Eastern and Southern Africa"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:country.organization,name:organization_eac"
 msgid "East African Community"
-msgstr "Wspólnota autonomiczna"
+msgstr "Autonomous community"
 
 msgctxt "model:country.organization,name:organization_eccas"
 msgid "Economic Community of Central African States"
 msgstr ""
 
 msgctxt "model:country.organization,name:organization_ecowas"
 msgid "Economic Community of West African States"
@@ -284,44 +289,44 @@
 
 msgctxt "model:country.organization.member,name:"
 msgid "Organization Member"
 msgstr ""
 
 msgctxt "model:country.postal_code,name:"
 msgid "Postal Code"
-msgstr "Kod pocztowy"
+msgstr ""
 
 #, fuzzy
 msgctxt "model:country.region,name:"
 msgid "Region"
 msgstr "Region"
 
 #, fuzzy
 msgctxt "model:country.region,name:region_africa"
 msgid "Africa"
-msgstr "Republika Południowej Afryki"
+msgstr "África do Sul"
 
 #, fuzzy
 msgctxt "model:country.region,name:region_americas"
 msgid "Americas"
-msgstr "Samoa Amerykańskie"
+msgstr "Samoa Americana"
 
 #, fuzzy
 msgctxt "model:country.region,name:region_antarctica"
 msgid "Antarctica"
-msgstr "Antarktyka"
+msgstr "Antárctida"
 
 msgctxt "model:country.region,name:region_asia"
 msgid "Asia"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:country.region,name:region_australia_new_zealand"
 msgid "Australia and New Zealand"
-msgstr "Nowa Zelandia"
+msgstr "Nova Zelândia"
 
 msgctxt "model:country.region,name:region_caribbean"
 msgid "Caribbean"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:country.region,name:region_central_america"
@@ -332,747 +337,747 @@
 msgctxt "model:country.region,name:region_central_asia"
 msgid "Central Asia"
 msgstr "Central Abaco"
 
 #, fuzzy
 msgctxt "model:country.region,name:region_channel_islands"
 msgid "Channel Islands"
-msgstr "Kajmany"
+msgstr "Ilhas Caimão"
 
 #, fuzzy
 msgctxt "model:country.region,name:region_eastern_africa"
 msgid "Eastern Africa"
-msgstr "Ekwatoria Wschodnia"
+msgstr "Eastern Equatoria"
 
 #, fuzzy
 msgctxt "model:country.region,name:region_eastern_asia"
 msgid "Eastern Asia"
-msgstr "Prowincja Przylądkowa Wschodnia"
+msgstr "Eastern Cape"
 
 #, fuzzy
 msgctxt "model:country.region,name:region_eastern_europe"
 msgid "Eastern Europe"
-msgstr "Prowincja Przylądkowa Wschodnia"
+msgstr "Eastern Cape"
 
 msgctxt "model:country.region,name:region_europe"
 msgid "Europe"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:country.region,name:region_latin_america_caribbean"
 msgid "Latin America and the Caribbean"
-msgstr "Saint Vincent i Grenadyny"
+msgstr "São Vicente e Grenadinas"
 
 #, fuzzy
 msgctxt "model:country.region,name:region_melanesia"
 msgid "Melanesia"
-msgstr "Malakka"
+msgstr "Melaka"
 
 #, fuzzy
 msgctxt "model:country.region,name:region_micronesia"
 msgid "Micronesia"
 msgstr "Misiones"
 
 msgctxt "model:country.region,name:region_middle_africa"
 msgid "Middle Africa"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:country.region,name:region_north_america"
 msgid "North America"
-msgstr "Republika Południowej Afryki"
+msgstr "África do Sul"
 
 #, fuzzy
 msgctxt "model:country.region,name:region_northern_africa"
 msgid "Northern Africa"
-msgstr "Republika Południowej Afryki"
+msgstr "África do Sul"
 
 #, fuzzy
 msgctxt "model:country.region,name:region_northern_america"
 msgid "Northern America"
 msgstr "Northern Samar"
 
 #, fuzzy
 msgctxt "model:country.region,name:region_northern_europe"
 msgid "Northern Europe"
-msgstr "Prowincja Przylądkowa Północna"
+msgstr "Northern Cape"
 
 #, fuzzy
 msgctxt "model:country.region,name:region_oceania"
 msgid "Oceania"
 msgstr "Chania"
 
 #, fuzzy
 msgctxt "model:country.region,name:region_polynesia"
 msgid "Polynesia"
-msgstr "Polinezja Francuska"
+msgstr "Polinésia Francesa"
 
 #, fuzzy
 msgctxt "model:country.region,name:region_south-eastern_asia"
 msgid "South-eastern Asia"
-msgstr "Prowincja Północno-Zachodnia"
+msgstr "North-Western"
 
 #, fuzzy
 msgctxt "model:country.region,name:region_south_america"
 msgid "South America"
-msgstr "Republika Południowej Afryki"
+msgstr "África do Sul"
 
 #, fuzzy
 msgctxt "model:country.region,name:region_southern_africa"
 msgid "Southern Africa"
-msgstr "Republika Południowej Afryki"
+msgstr "África do Sul"
 
 #, fuzzy
 msgctxt "model:country.region,name:region_southern_asia"
 msgid "Southern Asia"
-msgstr "Południowy"
+msgstr "Southern"
 
 #, fuzzy
 msgctxt "model:country.region,name:region_southern_europe"
 msgid "Southern Europe"
-msgstr "Południowy"
+msgstr "Southern"
 
 #, fuzzy
 msgctxt "model:country.region,name:region_sub-saharan_africa"
 msgid "Sub-Saharan Africa"
-msgstr "Republika Południowej Afryki"
+msgstr "África do Sul"
 
 #, fuzzy
 msgctxt "model:country.region,name:region_western_africa"
 msgid "Western Africa"
-msgstr "Australia Zachodnia"
+msgstr "Western Australia"
 
 #, fuzzy
 msgctxt "model:country.region,name:region_western_asia"
 msgid "Western Asia"
-msgstr "Australia Zachodnia"
+msgstr "Western Australia"
 
 #, fuzzy
 msgctxt "model:country.region,name:region_western_europe"
 msgid "Western Europe"
-msgstr "Prowincja Przylądkowa Zachodnia"
+msgstr "Western Cape"
 
 msgctxt "model:country.region,name:region_world"
 msgid "World"
 msgstr ""
 
 msgctxt "model:country.subdivision,name:"
 msgid "Subdivision"
-msgstr "Jednostka podrzędna"
+msgstr "Subdivisão"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_country_by_region"
 msgid "Countries by Region"
-msgstr "Region Centrum"
+msgstr "Central Region"
 
 msgctxt "model:ir.action,name:act_country_form"
 msgid "Countries"
-msgstr "Kraje"
+msgstr "Países"
 
 msgctxt "model:ir.action,name:act_organization_form"
 msgid "Organizations"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_postal_code_form"
 msgid "Postal Codes"
-msgstr "Kody pocztowe"
+msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_region_form"
 msgid "Regions"
 msgstr "Region"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_region_tree"
 msgid "Areas"
-msgstr "Obszar"
+msgstr "Area"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_country"
 msgid "Countries"
-msgstr "Kraje"
+msgstr "Países"
 
 msgctxt "model:ir.ui.menu,name:menu_country_form"
 msgid "Countries"
-msgstr "Kraje"
+msgstr "Countries"
 
 msgctxt "model:ir.ui.menu,name:menu_organization_form"
 msgid "Organizations"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_region_form"
 msgid "Regions"
 msgstr "Region"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_region_tree"
 msgid "Areas"
-msgstr "Obszar"
+msgstr "Area"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Administration"
-msgstr "Administracja"
+msgstr "Administration"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Administrative Region"
-msgstr "Region administracyjny"
+msgstr "Administrative Region"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Administrative Territory"
-msgstr "Terytorium administracyjne"
+msgstr "Administrative Territory"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Administrative area"
-msgstr "Obszar administracyjny"
+msgstr "Administrative area"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Administrative atoll"
-msgstr "Atol administracyjny"
+msgstr "Administrative atoll"
 
 #, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Administrative precinct"
-msgstr "Region administracyjny"
+msgstr "Administrative Region"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Arctic Region"
-msgstr "Region arktyczny"
+msgstr "Arctic Region"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Area"
-msgstr "Obszar"
+msgstr "Area"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Atoll"
-msgstr "Atol"
+msgstr "Atoll"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Autonomous City"
-msgstr "Miejscowość autonomiczna"
+msgstr "Autonomous City"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Autonomous Commune"
-msgstr "Gmina autonomiczna"
+msgstr "Autonomous Commune"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Autonomous District"
-msgstr "Dzielnica autonomiczna"
+msgstr "Autonomous District"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Autonomous Province"
-msgstr "Województwo autonomiczne"
+msgstr "Autonomous Province"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Autonomous Region"
-msgstr "Region autonomiczny"
+msgstr "Autonomous Region"
 
 #, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Autonomous city in north africa"
-msgstr "Dzielnica autonomiczna"
+msgstr "Autonomous District"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Autonomous communities"
-msgstr "Gminy autonomiczne"
+msgstr "Autonomous communities"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Autonomous community"
-msgstr "Wspólnota autonomiczna"
+msgstr "Autonomous community"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Autonomous island"
-msgstr "Wyspa autonomiczna"
+msgstr "Autonomous island"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Autonomous monastic state"
-msgstr "Autonomiczne państwo zakonne"
+msgstr "Autonomous monastic state"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Autonomous municipality"
-msgstr "Magistrat autonomiczny"
+msgstr "Autonomous municipality"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Autonomous republic"
-msgstr "Republika autonomiczna"
+msgstr "Autonomous republic"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Autonomous sector"
-msgstr "Sektor autonomiczny"
+msgstr "Autonomous sector"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Autonomous territorial unit"
-msgstr "Autonomiczna jednostka terytorialna"
+msgstr "Autonomous territorial unit"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Autonomous territory"
-msgstr "Terytorium autonomiczne"
+msgstr "Autonomous territory"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Borough"
-msgstr "Dzielnica"
+msgstr "Borough"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Canton"
-msgstr "Kanton"
+msgstr "Canton"
 
 #, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Capital"
-msgstr "Miasto stołeczne"
+msgstr "Capital city"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Capital District"
-msgstr "Okręg stołeczny"
+msgstr "Capital District"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Capital Metropolitan City"
-msgstr "Metropolitalne miasto stołeczne"
+msgstr "Capital Metropolitan City"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Capital Territory"
-msgstr "Terytorium stołeczne"
+msgstr "Capital Territory"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Capital city"
-msgstr "Miasto stołeczne"
+msgstr "Capital city"
 
 #, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Chain (of islands)"
-msgstr "Łańcuchy wysp"
+msgstr "Chains (of islands)"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Chains (of islands)"
-msgstr "Łańcuchy wysp"
+msgstr "Chains (of islands)"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "City"
-msgstr "Miasto"
+msgstr "Cidade"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "City corporation"
-msgstr "Miasto korporacyjne"
+msgstr "City corporation"
 
 #, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "City municipality"
-msgstr "Magistrat"
+msgstr "Municipality"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "City with county rights"
-msgstr "Miasto na prawach powiatu"
+msgstr "City with county rights"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Commune"
-msgstr "Gmina"
+msgstr "Commune"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Constitutional province"
-msgstr "Prowincja konstytucyjna"
+msgstr "Constitutional province"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Council area"
-msgstr "Obszar rady"
+msgstr "Council area"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Country"
-msgstr "Kraj"
+msgstr "País"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "County"
-msgstr "Powiat"
+msgstr "County"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Decentralized regional entity"
 msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Department"
-msgstr "Oddział"
+msgstr "Department"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Dependency"
-msgstr "Dependencja"
+msgstr "Dependency"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Development region"
-msgstr "Region rozwojowy"
+msgstr "Development region"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "District"
-msgstr "Okręg"
+msgstr "District"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "District council area"
-msgstr "Obszar rady dystryktu"
+msgstr "District council area"
 
 #, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "District municipality"
-msgstr "Prowincja Nairobi"
+msgstr "Nairobi Municipality"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "District with special status"
 msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Districts under republic administration"
 msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Division"
-msgstr "Podział"
+msgstr "Division"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Economic Prefecture"
-msgstr "Prefektura ekonomiczna"
+msgstr "Economic Prefecture"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Economic region"
-msgstr "Region gospodarczy"
+msgstr "Economic region"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Emirate"
-msgstr "Emirat"
+msgstr "Emirate"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Entity"
-msgstr "Jednostka"
+msgstr "Entity"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Federal Dependency"
-msgstr "Dependencja federalna"
+msgstr "Federal Dependency"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Federal District"
-msgstr "Okręg federalny"
+msgstr "Federal District"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Federal Territories"
-msgstr "Terytoria federalne"
+msgstr "Federal Territories"
 
 #, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Federal Territory"
-msgstr "Terytoria federalne"
+msgstr "Federal Territories"
 
 #, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Federal capital territory"
-msgstr "Australijskie Terytorium Stołeczne"
+msgstr "Australian Capital Territory"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Free municipal consortium"
 msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Geographical entity"
-msgstr "Obszar geograficzny"
+msgstr "Geographical entity"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Geographical region"
-msgstr "Region geograficzny"
+msgstr "Geographical region"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Geographical unit"
-msgstr "Jednostka geograficzna"
+msgstr "Geographical unit"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Governorate"
-msgstr "Gubernatorstwo"
+msgstr "Governorate"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Group of islands (20 inhabited islands)"
 msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Included for completeness"
-msgstr "Włączone do całości"
+msgstr "Included for completeness"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Indigenous region"
-msgstr "Region autochtoniczny"
+msgstr "Indigenous region"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Island"
-msgstr "Wyspa"
+msgstr "Island"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Island council"
-msgstr "Rada wyspy"
+msgstr "Island council"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Island group"
-msgstr "Grupa wysp"
+msgstr "Island group"
 
 #, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Islands, groups of islands"
-msgstr "Grupa wysp"
+msgstr "Island group"
 
 #, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Land"
-msgstr "Landy"
+msgstr "Landes"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Local council"
-msgstr "Rada lokalna"
+msgstr "Local council"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "London borough"
-msgstr "Dzielnica londyńska"
+msgstr "London borough"
 
 #, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Metropolitan administration"
-msgstr "Dystrykt metropolitalny"
+msgstr "Metropolitan district"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Metropolitan cities"
-msgstr "Metropolie"
+msgstr "Metropolitan cities"
 
 #, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Metropolitan city"
-msgstr "Metropolie"
+msgstr "Metropolitan cities"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Metropolitan collectivity with special status"
 msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Metropolitan department"
-msgstr "Oddział metropolitalny"
+msgstr "Metropolitan department"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Metropolitan district"
-msgstr "Dystrykt metropolitalny"
+msgstr "Metropolitan district"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Metropolitan region"
-msgstr "Region metropolitalny"
+msgstr "Metropolitan region"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Municipalities"
-msgstr "Gminy"
+msgstr "Municipalities"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Municipality"
-msgstr "Magistrat"
+msgstr "Municipality"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Nation"
-msgstr "Naród"
+msgstr "Nação"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Oblast"
-msgstr "Obwód"
+msgstr "Oblast"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Outlying area"
-msgstr "Obszar peryferyjny"
+msgstr "Outlying area"
 
 #, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Overseas collectivity"
-msgstr "Zagraniczna wspólnota terytorialna"
+msgstr "Overseas territorial collectivity"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Overseas collectivity with special status"
 msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Overseas department"
-msgstr "Zagraniczny oddział"
+msgstr "Departamento no Exterior"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Overseas region"
-msgstr "Zagraniczny region"
+msgstr "Região no Exterior"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Overseas region/department"
-msgstr "Zagraniczny region/oddział"
+msgstr "Overseas region/department"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Overseas territorial collectivity"
-msgstr "Zagraniczna wspólnota terytorialna"
+msgstr "Overseas territorial collectivity"
 
 #, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Overseas territory"
-msgstr "Zagraniczny region"
+msgstr "Região no Exterior"
 
 #, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Pakistan administered area"
-msgstr "Obszar administracyjny"
+msgstr "Administrative area"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Parish"
-msgstr "Parafia"
+msgstr "Parish"
 
 #, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Popularate"
 msgstr "Popularates"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Popularates"
 msgstr "Popularates"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Prefecture"
-msgstr "Prefektura"
+msgstr "Prefecture"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Principality"
-msgstr "Księstwo"
+msgstr "Principality"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Province"
-msgstr "Województwo"
+msgstr "Province"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Quarter"
-msgstr "Dzielnica miasta"
+msgstr "Quarter"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Rayon"
-msgstr "Rejon"
+msgstr "Rayon"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Region"
 msgstr "Region"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Regional council"
-msgstr "Rada regionalna"
+msgstr "Regional council"
 
 #, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Regional state"
-msgstr "Rada regionalna"
+msgstr "Regional council"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Republic"
-msgstr "Republika"
+msgstr "Republic"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Republican City"
-msgstr "Miasto republikańskie"
+msgstr "Republican City"
 
 #, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Rural municipality"
-msgstr "Specjalny magistrat"
+msgstr "Special Municipality"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Self-governed part"
-msgstr "Część samorządna"
+msgstr "Self-governed part"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Special District"
-msgstr "Specjalny dystrykt"
+msgstr "Special District"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Special Municipality"
-msgstr "Specjalny magistrat"
+msgstr "Special Municipality"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Special Region"
-msgstr "Region specjalny"
+msgstr "Special Region"
 
 #, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Special administrative city"
-msgstr "Specjalny region administracyjny"
+msgstr "Special administrative region"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Special administrative region"
-msgstr "Specjalny region administracyjny"
+msgstr "Special administrative region"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Special city"
-msgstr "Specjalne miasto"
+msgstr "Special city"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Special island authority"
-msgstr "Specjalny organ wyspy"
+msgstr "Special island authority"
 
 #, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Special self-governing city"
-msgstr "Specjalne miasto"
+msgstr "Special city"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Special self-governing province"
 msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Special zone"
-msgstr "Strefa specjalna"
+msgstr "Special zone"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "State"
-msgstr "Stan"
+msgstr "State"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Territorial unit"
-msgstr "Jednostka terytorialna"
+msgstr "Territorial unit"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Territory"
-msgstr "Terytorium"
+msgstr "Territory"
 
 #, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Town"
 msgstr "Hope Town"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Town council"
-msgstr "Rada miasta"
+msgstr "Town council"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Two-tier county"
-msgstr "Dwupoziomowe hrabstwo"
+msgstr "Two-tier county"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Union territory"
-msgstr "Terytorium związkowe"
+msgstr "Union territory"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Unitary authority"
-msgstr "Organ jednolity"
+msgstr "Unitary authority"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Unitary authority (england)"
-msgstr "Organ jednolity (Anglia)"
+msgstr "Unitary authority (england)"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Unitary authority (wales)"
-msgstr "Organ jednolity (Walia)"
+msgstr "Unitary authority (wales)"
 
 #, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Urban community"
-msgstr "Wspólnota autonomiczna"
+msgstr "Autonomous community"
 
 #, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Urban municipality"
-msgstr "Prowincja Nairobi"
+msgstr "Nairobi Municipality"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Voivodship"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Ward"
 msgstr "Wardak"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "zone"
-msgstr "Strefa"
+msgstr "zone"
```

### Comparing `trytond_country-7.2.0/locale/pt.po` & `trytond_country-7.2.1/locale/ro.po`

 * *Files 5% similar despite different names*

```diff
@@ -1,1083 +1,1079 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:country.country,code3:"
 msgid "3-letters Code"
-msgstr "Código de três letras"
+msgstr "Cod din 3 litere"
 
 msgctxt "field:country.country,code:"
 msgid "Code"
-msgstr "Código"
+msgstr "Cod"
 
 msgctxt "field:country.country,code_numeric:"
 msgid "Numeric Code"
-msgstr "Código numérico"
+msgstr "Cod Numeric"
 
 msgctxt "field:country.country,flag:"
 msgid "Flag"
-msgstr ""
+msgstr "Steag"
 
 msgctxt "field:country.country,members:"
 msgid "Members"
-msgstr ""
+msgstr "Membri"
 
 msgctxt "field:country.country,name:"
 msgid "Name"
-msgstr "Nome"
+msgstr "Denumire"
 
 msgctxt "field:country.country,organizations:"
 msgid "Organizations"
-msgstr ""
+msgstr "Organizații"
 
-#, fuzzy
 msgctxt "field:country.country,region:"
 msgid "Region"
-msgstr "Region"
+msgstr "Regiune"
 
 msgctxt "field:country.country,subdivisions:"
 msgid "Subdivisions"
-msgstr "Subdivisões"
+msgstr "Subdiviziune"
 
-#, fuzzy
 msgctxt "field:country.organization,code:"
 msgid "Code"
-msgstr "Código"
+msgstr "Cod"
 
-#, fuzzy
 msgctxt "field:country.organization,countries:"
 msgid "Countries"
-msgstr "Países"
+msgstr "Țări"
 
 msgctxt "field:country.organization,members:"
 msgid "Members"
-msgstr ""
+msgstr "Membri"
 
 #, fuzzy
 msgctxt "field:country.organization,name:"
 msgid "Name"
-msgstr "Nome"
+msgstr "Denumire"
 
-#, fuzzy
 msgctxt "field:country.organization.member,active:"
 msgid "Active"
-msgstr "Ativo"
+msgstr "Activ"
 
-#, fuzzy
 msgctxt "field:country.organization.member,country:"
 msgid "Country"
-msgstr "País"
+msgstr "Țară"
 
-#, fuzzy
 msgctxt "field:country.organization.member,from_date:"
 msgid "From Date"
-msgstr "Data de Edição"
+msgstr "De la Data"
 
 msgctxt "field:country.organization.member,organization:"
 msgid "Organization"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:country.organization.member,to_date:"
 msgid "To Date"
-msgstr ""
+msgstr "Până la Data"
 
-#, fuzzy
 msgctxt "field:country.postal_code,city:"
 msgid "City"
-msgstr "Cidade"
+msgstr "Oraș"
 
-#, fuzzy
 msgctxt "field:country.postal_code,country:"
 msgid "Country"
-msgstr "País"
+msgstr "Țară"
 
 msgctxt "field:country.postal_code,postal_code:"
 msgid "Postal Code"
-msgstr ""
+msgstr "Cod Poștal"
 
-#, fuzzy
 msgctxt "field:country.postal_code,subdivision:"
 msgid "Subdivision"
-msgstr "Subdivisão"
+msgstr "Subdiviziune"
 
-#, fuzzy
 msgctxt "field:country.region,code_numeric:"
 msgid "Numeric Code"
-msgstr "Código numérico"
+msgstr "Cod Numeric"
 
-#, fuzzy
 msgctxt "field:country.region,countries:"
 msgid "Countries"
-msgstr "Países"
+msgstr "Țări"
 
 #, fuzzy
 msgctxt "field:country.region,name:"
 msgid "Name"
-msgstr "Nome"
+msgstr "Denumire"
 
 #, fuzzy
 msgctxt "field:country.region,parent:"
 msgid "Parent"
-msgstr "Pai"
+msgstr "Parinte"
 
 #, fuzzy
 msgctxt "field:country.region,subregions:"
 msgid "Subregions"
-msgstr "Southern Region"
+msgstr "Subregiuni"
 
 msgctxt "field:country.subdivision,code:"
 msgid "Code"
-msgstr "Código"
+msgstr "Cod"
 
 msgctxt "field:country.subdivision,country:"
 msgid "Country"
-msgstr "País"
+msgstr "Țară"
 
 msgctxt "field:country.subdivision,flag:"
 msgid "Flag"
-msgstr ""
+msgstr "Steag"
 
 msgctxt "field:country.subdivision,name:"
 msgid "Name"
-msgstr "Nome"
+msgstr "Denumire"
 
 msgctxt "field:country.subdivision,parent:"
 msgid "Parent"
-msgstr "Pai"
+msgstr "Parinte"
 
 msgctxt "field:country.subdivision,type:"
 msgid "Type"
-msgstr "Editado por"
+msgstr "Tip"
 
 msgctxt "help:country.country,code3:"
 msgid "The 3 chars ISO country code."
-msgstr "O código ISO de 3 caracteres do país."
+msgstr "Cod ISO de țara din 3 litere."
 
 msgctxt "help:country.country,code:"
 msgid "The 2 chars ISO country code."
-msgstr "O código ISO de 2 caracteres do país."
+msgstr "Cod ISO de țara din 2 litere."
 
 msgctxt "help:country.country,code_numeric:"
 msgid "The ISO numeric country code."
-msgstr "O código numérico ISO do país."
+msgstr "Cod numeric de țara ISO."
 
 msgctxt "help:country.country,name:"
 msgid "The main identifier of the country."
-msgstr "O identificador principal do país."
+msgstr "Identificatorul principal al țarii."
 
 msgctxt "help:country.postal_code,city:"
 msgid "The city associated with the postal code."
-msgstr ""
+msgstr "Orașul asociat cu codul poștal."
 
 msgctxt "help:country.postal_code,country:"
 msgid "The country that contains the postal code."
-msgstr ""
+msgstr "Țara care conține codul poștal."
 
-#, fuzzy
 msgctxt "help:country.postal_code,subdivision:"
 msgid "The subdivision where the postal code is."
-msgstr "A subdivisão em que o código postal (CEP) está."
+msgstr "Subdiviziunea în care se află codul poștal."
 
+#, fuzzy
 msgctxt "help:country.region,code_numeric:"
 msgid "UN M49 region code."
-msgstr ""
+msgstr "Cod de regiune ONU M49."
 
 msgctxt "help:country.subdivision,code:"
 msgid "The ISO code of the subdivision."
-msgstr "O código ISO da subdivisão."
+msgstr "Codul ISO al subdiviziuni."
 
 msgctxt "help:country.subdivision,country:"
 msgid "The country where this subdivision is."
-msgstr "O país em que a subdivisão está."
+msgstr "Țara unde se afla subdiviziunea."
 
 msgctxt "help:country.subdivision,name:"
 msgid "The main identifier of the subdivision."
-msgstr "O identificador principal da subdivisão."
+msgstr "Identificatorul principal al subdiviziunii."
 
 msgctxt "help:country.subdivision,parent:"
 msgid "Add subdivision below the parent."
-msgstr "Adicionar subdivisão abaixo do pai."
+msgstr "Adăugați subdiviziune sub părintele."
 
 msgctxt "model:country.country,name:"
 msgid "Country"
-msgstr "País"
+msgstr "Țară"
 
 msgctxt "model:country.organization,name:"
 msgid "Organization"
-msgstr ""
+msgstr "Organizație"
 
 msgctxt "model:country.organization,name:organization_amu"
 msgid "Arab Maghreb Union"
-msgstr ""
+msgstr "Uniunea Maghrebului Arab"
 
+#, fuzzy
 msgctxt "model:country.organization,name:organization_apec"
 msgid "Asia-Pacific Economic Cooperation"
-msgstr ""
+msgstr "Cooperarea Economică Asia-Pacific"
 
+#, fuzzy
 msgctxt "model:country.organization,name:organization_asean"
 msgid "Association of Southeast Asian Nations"
-msgstr ""
+msgstr "Asociația Națiunilor din Asia de Sud-Est"
 
 msgctxt "model:country.organization,name:organization_benelux"
 msgid "Benelux Union"
-msgstr ""
+msgstr "Uniunea Benelux"
 
 #, fuzzy
 msgctxt "model:country.organization,name:organization_can"
 msgid "Andean Community"
-msgstr "Autonomous community"
+msgstr "Comunitatea Andină"
 
 #, fuzzy
 msgctxt "model:country.organization,name:organization_caricom"
 msgid "Caribbean Community"
-msgstr "Autonomous community"
+msgstr "Comunitatea Caraibelor"
 
+#, fuzzy
 msgctxt "model:country.organization,name:organization_cemac"
 msgid "Economic and Monetary Community of Central Africa"
-msgstr ""
+msgstr "Comunitatea Economică și Monetară a Africii Centrale"
 
+#, fuzzy
 msgctxt "model:country.organization,name:organization_cen-sad"
 msgid "Community of Sahel–Saharan States"
-msgstr ""
+msgstr "Comunitatea Statelor Sahel-Sahariene"
 
+#, fuzzy
 msgctxt "model:country.organization,name:organization_comesa"
 msgid "Common Market for Eastern and Southern Africa"
-msgstr ""
+msgstr "Piața comună pentru Africa de Est și de Sud"
 
 #, fuzzy
 msgctxt "model:country.organization,name:organization_eac"
 msgid "East African Community"
-msgstr "Autonomous community"
+msgstr "Comunitatea Est-Africană"
 
+#, fuzzy
 msgctxt "model:country.organization,name:organization_eccas"
 msgid "Economic Community of Central African States"
-msgstr ""
+msgstr "Comunitatea Economică a Statelor Africii Centrale"
 
+#, fuzzy
 msgctxt "model:country.organization,name:organization_ecowas"
 msgid "Economic Community of West African States"
-msgstr ""
+msgstr "Comunitatea Economică a Statelor Africii de Vest"
 
-#, fuzzy
 msgctxt "model:country.organization,name:organization_eu"
 msgid "European Union"
-msgstr "La Union"
+msgstr "Uniunea Europeană"
 
+#, fuzzy
 msgctxt "model:country.organization,name:organization_gcc"
 msgid "Cooperation Council for the Arab States of the Gulf"
-msgstr ""
+msgstr "Consiliul de Cooperare pentru Statele Arabe din Golf"
 
+#, fuzzy
 msgctxt "model:country.organization,name:organization_igad"
 msgid "Intergovernmental Authority on Development"
-msgstr ""
+msgstr "Autoritatea Interguvernamentală pentru Dezvoltare"
 
 #, fuzzy
 msgctxt "model:country.organization,name:organization_mercosur"
 msgid "Southern Common Market"
-msgstr "Southern Leyte"
+msgstr "Piața comună de sud"
 
+#, fuzzy
 msgctxt "model:country.organization,name:organization_nafta"
 msgid "North American Free Trade Agreement"
-msgstr ""
+msgstr "Acordul de Liber Schimb din America de Nord"
 
+#, fuzzy
 msgctxt "model:country.organization,name:organization_sadc"
 msgid "Southern African Development Community"
-msgstr ""
+msgstr "Comunitatea de Dezvoltare a Africii de Sud"
 
+#, fuzzy
 msgctxt "model:country.organization,name:organization_safta"
 msgid "South Asian Free Trade Area"
-msgstr ""
+msgstr "Zona de schimb liber din Asia de Sud"
 
 msgctxt "model:country.organization.member,name:"
 msgid "Organization Member"
-msgstr ""
+msgstr "Membru al organizației"
 
 msgctxt "model:country.postal_code,name:"
 msgid "Postal Code"
-msgstr ""
+msgstr "Cod Poștal"
 
-#, fuzzy
 msgctxt "model:country.region,name:"
 msgid "Region"
-msgstr "Region"
+msgstr "Regiune"
 
-#, fuzzy
 msgctxt "model:country.region,name:region_africa"
 msgid "Africa"
-msgstr "África do Sul"
+msgstr "Africa"
 
-#, fuzzy
 msgctxt "model:country.region,name:region_americas"
 msgid "Americas"
-msgstr "Samoa Americana"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:country.region,name:region_antarctica"
 msgid "Antarctica"
-msgstr "Antárctida"
+msgstr "Antarctica"
 
 msgctxt "model:country.region,name:region_asia"
 msgid "Asia"
-msgstr ""
+msgstr "Asia"
 
-#, fuzzy
 msgctxt "model:country.region,name:region_australia_new_zealand"
 msgid "Australia and New Zealand"
-msgstr "Nova Zelândia"
+msgstr "Australia și Noua Zeelandă"
 
 msgctxt "model:country.region,name:region_caribbean"
 msgid "Caribbean"
-msgstr ""
+msgstr "Caraibe"
 
-#, fuzzy
 msgctxt "model:country.region,name:region_central_america"
 msgid "Central America"
-msgstr "Central Abaco"
+msgstr "America Centrală"
 
-#, fuzzy
 msgctxt "model:country.region,name:region_central_asia"
 msgid "Central Asia"
-msgstr "Central Abaco"
+msgstr "Asia Centrala"
 
 #, fuzzy
 msgctxt "model:country.region,name:region_channel_islands"
 msgid "Channel Islands"
-msgstr "Ilhas Caimão"
+msgstr "Insulele Canalului"
 
-#, fuzzy
 msgctxt "model:country.region,name:region_eastern_africa"
 msgid "Eastern Africa"
-msgstr "Eastern Equatoria"
+msgstr "Africa de Est"
 
-#, fuzzy
 msgctxt "model:country.region,name:region_eastern_asia"
 msgid "Eastern Asia"
-msgstr "Eastern Cape"
+msgstr "Asia de Est"
 
-#, fuzzy
 msgctxt "model:country.region,name:region_eastern_europe"
 msgid "Eastern Europe"
-msgstr "Eastern Cape"
+msgstr "Europa de Est"
 
 msgctxt "model:country.region,name:region_europe"
 msgid "Europe"
-msgstr ""
+msgstr "Europa"
 
-#, fuzzy
 msgctxt "model:country.region,name:region_latin_america_caribbean"
 msgid "Latin America and the Caribbean"
-msgstr "São Vicente e Grenadinas"
+msgstr "America Latină și Caraibe"
 
-#, fuzzy
 msgctxt "model:country.region,name:region_melanesia"
 msgid "Melanesia"
-msgstr "Melaka"
+msgstr "Melanezia"
 
-#, fuzzy
 msgctxt "model:country.region,name:region_micronesia"
 msgid "Micronesia"
-msgstr "Misiones"
+msgstr "Micronezia"
 
+#, fuzzy
 msgctxt "model:country.region,name:region_middle_africa"
 msgid "Middle Africa"
-msgstr ""
+msgstr "Africa Centrală"
 
-#, fuzzy
 msgctxt "model:country.region,name:region_north_america"
 msgid "North America"
-msgstr "África do Sul"
+msgstr "America de Nord"
 
-#, fuzzy
 msgctxt "model:country.region,name:region_northern_africa"
 msgid "Northern Africa"
-msgstr "África do Sul"
+msgstr "Africa de Nord"
 
-#, fuzzy
 msgctxt "model:country.region,name:region_northern_america"
 msgid "Northern America"
-msgstr "Northern Samar"
+msgstr "America de Nord"
 
-#, fuzzy
 msgctxt "model:country.region,name:region_northern_europe"
 msgid "Northern Europe"
-msgstr "Northern Cape"
+msgstr "Europa de Nord"
 
-#, fuzzy
 msgctxt "model:country.region,name:region_oceania"
 msgid "Oceania"
-msgstr "Chania"
+msgstr "Oceania"
 
-#, fuzzy
 msgctxt "model:country.region,name:region_polynesia"
 msgid "Polynesia"
-msgstr "Polinésia Francesa"
+msgstr "Polinezia"
 
-#, fuzzy
 msgctxt "model:country.region,name:region_south-eastern_asia"
 msgid "South-eastern Asia"
-msgstr "North-Western"
+msgstr "Asia de Sud-Est"
 
-#, fuzzy
 msgctxt "model:country.region,name:region_south_america"
 msgid "South America"
-msgstr "África do Sul"
+msgstr "America de Sud"
 
-#, fuzzy
 msgctxt "model:country.region,name:region_southern_africa"
 msgid "Southern Africa"
-msgstr "África do Sul"
+msgstr "Africa de Sud"
 
-#, fuzzy
 msgctxt "model:country.region,name:region_southern_asia"
 msgid "Southern Asia"
-msgstr "Southern"
+msgstr "Asia de Sud"
 
-#, fuzzy
 msgctxt "model:country.region,name:region_southern_europe"
 msgid "Southern Europe"
-msgstr "Southern"
+msgstr "Europa de Sud"
 
-#, fuzzy
 msgctxt "model:country.region,name:region_sub-saharan_africa"
 msgid "Sub-Saharan Africa"
-msgstr "África do Sul"
+msgstr "Africa Sub-Sahariană"
 
-#, fuzzy
 msgctxt "model:country.region,name:region_western_africa"
 msgid "Western Africa"
-msgstr "Western Australia"
+msgstr "Africa de Vest"
 
-#, fuzzy
 msgctxt "model:country.region,name:region_western_asia"
 msgid "Western Asia"
-msgstr "Western Australia"
+msgstr "Asia de Vest"
 
-#, fuzzy
 msgctxt "model:country.region,name:region_western_europe"
 msgid "Western Europe"
-msgstr "Western Cape"
+msgstr "Europa de Vest"
 
 msgctxt "model:country.region,name:region_world"
 msgid "World"
-msgstr ""
+msgstr "Lume"
 
 msgctxt "model:country.subdivision,name:"
 msgid "Subdivision"
-msgstr "Subdivisão"
+msgstr "Subdiviziune"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_country_by_region"
 msgid "Countries by Region"
-msgstr "Central Region"
+msgstr "Țări după regiune"
 
 msgctxt "model:ir.action,name:act_country_form"
 msgid "Countries"
-msgstr "Países"
+msgstr "Țări"
 
 msgctxt "model:ir.action,name:act_organization_form"
 msgid "Organizations"
-msgstr ""
+msgstr "Organizații"
 
 msgctxt "model:ir.action,name:act_postal_code_form"
 msgid "Postal Codes"
-msgstr ""
+msgstr "Coduri Poștale"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_region_form"
 msgid "Regions"
-msgstr "Region"
+msgstr "Regiuni"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_region_tree"
 msgid "Areas"
-msgstr "Area"
+msgstr "Zone"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_country"
 msgid "Countries"
-msgstr "Países"
+msgstr "Țări"
 
 msgctxt "model:ir.ui.menu,name:menu_country_form"
 msgid "Countries"
-msgstr "Countries"
+msgstr "Țări"
 
 msgctxt "model:ir.ui.menu,name:menu_organization_form"
 msgid "Organizations"
-msgstr ""
+msgstr "Organizații"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_region_form"
 msgid "Regions"
-msgstr "Region"
+msgstr "Regiuni"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_region_tree"
 msgid "Areas"
-msgstr "Area"
+msgstr "Zone"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Administration"
-msgstr "Administration"
+msgstr "Administrare"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Administrative Region"
-msgstr "Administrative Region"
+msgstr "Regiunea administrativă"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Administrative Territory"
-msgstr "Administrative Territory"
+msgstr "Teritoriul administrativ"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Administrative area"
-msgstr "Administrative area"
+msgstr "Zona administrativă"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Administrative atoll"
-msgstr "Administrative atoll"
+msgstr "Atol administrativ"
 
 #, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Administrative precinct"
-msgstr "Administrative Region"
+msgstr "Regiunea administrativă"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Arctic Region"
-msgstr "Arctic Region"
+msgstr "Regiunea Arctică"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Area"
-msgstr "Area"
+msgstr "Zonă"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Atoll"
-msgstr "Atoll"
+msgstr "Atol"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Autonomous City"
-msgstr "Autonomous City"
+msgstr "Oraș autonom"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Autonomous Commune"
-msgstr "Autonomous Commune"
+msgstr "Comuna autonomă"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Autonomous District"
-msgstr "Autonomous District"
+msgstr "District autonom"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Autonomous Province"
-msgstr "Autonomous Province"
+msgstr "Provincia autonomă"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Autonomous Region"
-msgstr "Autonomous Region"
+msgstr "Regiune autonomă"
 
-#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Autonomous city in north africa"
-msgstr "Autonomous District"
+msgstr "Oraș autonom din Africa de Nord"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Autonomous communities"
-msgstr "Autonomous communities"
+msgstr "Comunitățile autonome"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Autonomous community"
-msgstr "Autonomous community"
+msgstr "Comunitatea autonomă"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Autonomous island"
-msgstr "Autonomous island"
+msgstr "Insula autonomă"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Autonomous monastic state"
-msgstr "Autonomous monastic state"
+msgstr "Stat monahal autonom"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Autonomous municipality"
-msgstr "Autonomous municipality"
+msgstr "Municipalitate autonomă"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Autonomous republic"
-msgstr "Autonomous republic"
+msgstr "Republica autonomă"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Autonomous sector"
-msgstr "Autonomous sector"
+msgstr "Sector autonom"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Autonomous territorial unit"
-msgstr "Autonomous territorial unit"
+msgstr "Unitatea teritorială autonomă"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Autonomous territory"
-msgstr "Autonomous territory"
+msgstr "Teritoriu autonom"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Borough"
-msgstr "Borough"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Canton"
 msgstr "Canton"
 
-#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Capital"
-msgstr "Capital city"
+msgstr "Capitala"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Capital District"
-msgstr "Capital District"
+msgstr ""
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Capital Metropolitan City"
-msgstr "Capital Metropolitan City"
+msgstr "Capitala Metropolitană"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Capital Territory"
-msgstr "Capital Territory"
+msgstr "Teritoriul Capitalei"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Capital city"
-msgstr "Capital city"
+msgstr "Capitala"
 
 #, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Chain (of islands)"
-msgstr "Chains (of islands)"
+msgstr "Lanț (de insule)"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Chains (of islands)"
-msgstr "Chains (of islands)"
+msgstr "Lanțuri (de insule)"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "City"
-msgstr "Cidade"
+msgstr "Oraș"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "City corporation"
-msgstr "City corporation"
+msgstr "Corporația orașului"
 
 #, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "City municipality"
-msgstr "Municipality"
+msgstr "Municipiul orașului"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "City with county rights"
-msgstr "City with county rights"
+msgstr "Oraș cu drepturi județene"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Commune"
-msgstr "Commune"
+msgstr "Comună"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Constitutional province"
-msgstr "Constitutional province"
+msgstr "Provincie constituțională"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Council area"
-msgstr "Council area"
+msgstr "zona Consiliului"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Country"
-msgstr "País"
+msgstr "Țară"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "County"
-msgstr "County"
+msgstr "Județ"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Decentralized regional entity"
-msgstr ""
+msgstr "Entitate regională descentralizată"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Department"
-msgstr "Department"
+msgstr "Departament"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Dependency"
-msgstr "Dependency"
+msgstr "Dependenţă"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Development region"
-msgstr "Development region"
+msgstr "Regiunea de dezvoltare"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "District"
 msgstr "District"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "District council area"
-msgstr "District council area"
+msgstr ""
 
 #, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "District municipality"
-msgstr "Nairobi Municipality"
+msgstr "Municipalitate autonomă"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "District with special status"
-msgstr ""
+msgstr "District cu statut special"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Districts under republic administration"
-msgstr ""
+msgstr "Districte aflate în administrarea republicii"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Division"
-msgstr "Division"
+msgstr "Divizia"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Economic Prefecture"
-msgstr "Economic Prefecture"
+msgstr "Prefectura economică"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Economic region"
-msgstr "Economic region"
+msgstr "Regiunea economică"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Emirate"
-msgstr "Emirate"
+msgstr "Emirat"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Entity"
-msgstr "Entity"
+msgstr "Entitate"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Federal Dependency"
-msgstr "Federal Dependency"
+msgstr "Dependență federală"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Federal District"
-msgstr "Federal District"
+msgstr "District federal"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Federal Territories"
-msgstr "Federal Territories"
+msgstr "Teritoriile Federale"
 
 #, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Federal Territory"
-msgstr "Federal Territories"
+msgstr "Teritoriu federal"
 
-#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Federal capital territory"
-msgstr "Australian Capital Territory"
+msgstr ""
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Free municipal consortium"
-msgstr ""
+msgstr "Consorțiu municipal gratuit"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Geographical entity"
-msgstr "Geographical entity"
+msgstr "Entitate geografică"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Geographical region"
-msgstr "Geographical region"
+msgstr "Regiunea geografică"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Geographical unit"
-msgstr "Geographical unit"
+msgstr "Unitate geografică"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Governorate"
-msgstr "Governorate"
+msgstr "Guvernorat"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Group of islands (20 inhabited islands)"
-msgstr ""
+msgstr "Grup de insule (20 de insule locuite)"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Included for completeness"
-msgstr "Included for completeness"
+msgstr ""
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Indigenous region"
-msgstr "Indigenous region"
+msgstr "Regiune indigenă"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Island"
-msgstr "Island"
+msgstr "Insulă"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Island council"
-msgstr "Island council"
+msgstr "Consiliu Insular"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Island group"
-msgstr "Island group"
+msgstr "Grup de insule"
 
 #, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Islands, groups of islands"
-msgstr "Island group"
+msgstr "Insule, grupuri de insule"
 
 #, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Land"
-msgstr "Landes"
+msgstr "Teren"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Local council"
-msgstr "Local council"
+msgstr "Consiliu Local"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "London borough"
-msgstr "London borough"
+msgstr "Cartier Londonez"
 
 #, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Metropolitan administration"
-msgstr "Metropolitan district"
+msgstr "Administrația metropolitană"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Metropolitan cities"
-msgstr "Metropolitan cities"
+msgstr "Orașe metropolitane"
 
 #, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Metropolitan city"
-msgstr "Metropolitan cities"
+msgstr "Oraș metropolitan"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Metropolitan collectivity with special status"
-msgstr ""
+msgstr "Colectivitate metropolitană cu statut special"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Metropolitan department"
-msgstr "Metropolitan department"
+msgstr "Departament metropolitan"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Metropolitan district"
-msgstr "Metropolitan district"
+msgstr "District Metropolitan"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Metropolitan region"
-msgstr "Metropolitan region"
+msgstr "Regiune metropolitană"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Municipalities"
-msgstr "Municipalities"
+msgstr "Municipalități"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Municipality"
-msgstr "Municipality"
+msgstr "Municipiu"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Nation"
-msgstr "Nação"
+msgstr "Naţiune"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Oblast"
 msgstr "Oblast"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Outlying area"
-msgstr "Outlying area"
+msgstr "Zona periferică"
 
 #, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Overseas collectivity"
-msgstr "Overseas territorial collectivity"
+msgstr "Colectivitatea de peste mări"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Overseas collectivity with special status"
-msgstr ""
+msgstr "Colectivitate de peste mări cu statut special"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Overseas department"
-msgstr "Departamento no Exterior"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Overseas region"
-msgstr "Região no Exterior"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Overseas region/department"
-msgstr "Overseas region/department"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Overseas territorial collectivity"
-msgstr "Overseas territorial collectivity"
+msgstr ""
 
-#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Overseas territory"
-msgstr "Região no Exterior"
+msgstr ""
 
 #, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Pakistan administered area"
-msgstr "Administrative area"
+msgstr "Zonă administrată de Pakistan"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Parish"
-msgstr "Parish"
+msgstr "Parohie"
 
-#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Popularate"
-msgstr "Popularates"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Popularates"
-msgstr "Popularates"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Prefecture"
-msgstr "Prefecture"
+msgstr "Prefectură"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Principality"
-msgstr "Principality"
+msgstr "Principat"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Province"
-msgstr "Province"
+msgstr "Provincie"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Quarter"
-msgstr "Quarter"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Rayon"
-msgstr "Rayon"
+msgstr "Raion"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Region"
-msgstr "Region"
+msgstr "Regiune"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Regional council"
-msgstr "Regional council"
+msgstr "Consiliul regional"
 
 #, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Regional state"
-msgstr "Regional council"
+msgstr "Stat regional"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Republic"
-msgstr "Republic"
+msgstr "Republică"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Republican City"
-msgstr "Republican City"
+msgstr "Oraș Republican"
 
 #, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Rural municipality"
-msgstr "Special Municipality"
+msgstr "Municipalitate rurală"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Self-governed part"
-msgstr "Self-governed part"
+msgstr "Parte autonomă"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Special District"
-msgstr "Special District"
+msgstr "District special"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Special Municipality"
-msgstr "Special Municipality"
+msgstr "Municipalitatea specială"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Special Region"
-msgstr "Special Region"
+msgstr "Regiunea specială"
 
 #, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Special administrative city"
-msgstr "Special administrative region"
+msgstr "Oraș administrativ special"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Special administrative region"
-msgstr "Special administrative region"
+msgstr "Regiunea administrativă specială"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Special city"
-msgstr "Special city"
+msgstr "Oraș special"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Special island authority"
-msgstr "Special island authority"
+msgstr "Autoritate specială insulară"
 
 #, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Special self-governing city"
-msgstr "Special city"
+msgstr "Oraș special autonom"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Special self-governing province"
-msgstr ""
+msgstr "Provincie Autonomă Specială"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Special zone"
-msgstr "Special zone"
+msgstr "Zona specială"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "State"
-msgstr "State"
+msgstr "Stat"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Territorial unit"
-msgstr "Territorial unit"
+msgstr "Unitatea teritorială"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Territory"
-msgstr "Territory"
+msgstr "Teritoriu"
 
-#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Town"
-msgstr "Hope Town"
+msgstr "Oraș"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Town council"
-msgstr "Town council"
+msgstr "Consiliul Local"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Two-tier county"
-msgstr "Two-tier county"
+msgstr "Județul cu două niveluri"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Union territory"
-msgstr "Union territory"
+msgstr "Teritoriul Uniunii"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Unitary authority"
-msgstr "Unitary authority"
+msgstr "Autoritate unitară"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Unitary authority (england)"
-msgstr "Unitary authority (england)"
+msgstr "Autoritate unitară (Anglia)"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Unitary authority (wales)"
-msgstr "Unitary authority (wales)"
+msgstr "Autoritate unitară (Țara Galilor)"
 
 #, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Urban community"
-msgstr "Autonomous community"
+msgstr "Comunitate urbană"
 
 #, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Urban municipality"
-msgstr "Nairobi Municipality"
+msgstr "Municipalitate urbană"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Voivodship"
-msgstr ""
+msgstr "Voievodat"
 
-#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Ward"
-msgstr "Wardak"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "zone"
-msgstr "zone"
+msgstr "zona"
```

### Comparing `trytond_country-7.2.0/locale/ro.po` & `trytond_country-7.2.1/locale/tr.po`

 * *Files 15% similar despite different names*

```diff
@@ -1,885 +1,875 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:country.country,code3:"
 msgid "3-letters Code"
-msgstr "Cod din 3 litere"
+msgstr ""
 
 msgctxt "field:country.country,code:"
 msgid "Code"
-msgstr "Cod"
+msgstr ""
 
 msgctxt "field:country.country,code_numeric:"
 msgid "Numeric Code"
-msgstr "Cod Numeric"
+msgstr ""
 
 msgctxt "field:country.country,flag:"
 msgid "Flag"
-msgstr "Steag"
+msgstr ""
 
 msgctxt "field:country.country,members:"
 msgid "Members"
-msgstr "Membri"
+msgstr ""
 
 msgctxt "field:country.country,name:"
 msgid "Name"
-msgstr "Denumire"
+msgstr "Ad"
 
 msgctxt "field:country.country,organizations:"
 msgid "Organizations"
-msgstr "Organizații"
+msgstr ""
 
 msgctxt "field:country.country,region:"
 msgid "Region"
-msgstr "Regiune"
+msgstr ""
 
 msgctxt "field:country.country,subdivisions:"
 msgid "Subdivisions"
-msgstr "Subdiviziune"
+msgstr ""
 
 msgctxt "field:country.organization,code:"
 msgid "Code"
-msgstr "Cod"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:country.organization,countries:"
 msgid "Countries"
-msgstr "Țări"
+msgstr "Countries"
 
 msgctxt "field:country.organization,members:"
 msgid "Members"
-msgstr "Membri"
+msgstr ""
 
 #, fuzzy
 msgctxt "field:country.organization,name:"
 msgid "Name"
-msgstr "Denumire"
+msgstr "Ad"
 
 msgctxt "field:country.organization.member,active:"
 msgid "Active"
-msgstr "Activ"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:country.organization.member,country:"
 msgid "Country"
-msgstr "Țară"
+msgstr "Ülke"
 
 msgctxt "field:country.organization.member,from_date:"
 msgid "From Date"
-msgstr "De la Data"
+msgstr ""
 
 msgctxt "field:country.organization.member,organization:"
 msgid "Organization"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:country.organization.member,to_date:"
 msgid "To Date"
-msgstr "Până la Data"
+msgstr ""
 
 msgctxt "field:country.postal_code,city:"
 msgid "City"
-msgstr "Oraș"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:country.postal_code,country:"
 msgid "Country"
-msgstr "Țară"
+msgstr "Ülke"
 
 msgctxt "field:country.postal_code,postal_code:"
 msgid "Postal Code"
-msgstr "Cod Poștal"
+msgstr ""
 
 msgctxt "field:country.postal_code,subdivision:"
 msgid "Subdivision"
-msgstr "Subdiviziune"
+msgstr ""
 
 msgctxt "field:country.region,code_numeric:"
 msgid "Numeric Code"
-msgstr "Cod Numeric"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:country.region,countries:"
 msgid "Countries"
-msgstr "Țări"
+msgstr "Countries"
 
 #, fuzzy
 msgctxt "field:country.region,name:"
 msgid "Name"
-msgstr "Denumire"
+msgstr "Ad"
 
 #, fuzzy
 msgctxt "field:country.region,parent:"
 msgid "Parent"
-msgstr "Parinte"
+msgstr "Brent"
 
 #, fuzzy
 msgctxt "field:country.region,subregions:"
 msgid "Subregions"
-msgstr "Subregiuni"
+msgstr "Southern Region"
 
 msgctxt "field:country.subdivision,code:"
 msgid "Code"
-msgstr "Cod"
+msgstr ""
 
 msgctxt "field:country.subdivision,country:"
 msgid "Country"
-msgstr "Țară"
+msgstr "Ülke"
 
 msgctxt "field:country.subdivision,flag:"
 msgid "Flag"
-msgstr "Steag"
+msgstr ""
 
 msgctxt "field:country.subdivision,name:"
 msgid "Name"
-msgstr "Denumire"
+msgstr "Ad"
 
 msgctxt "field:country.subdivision,parent:"
 msgid "Parent"
-msgstr "Parinte"
+msgstr ""
 
 msgctxt "field:country.subdivision,type:"
 msgid "Type"
-msgstr "Tip"
+msgstr ""
 
 msgctxt "help:country.country,code3:"
 msgid "The 3 chars ISO country code."
-msgstr "Cod ISO de țara din 3 litere."
+msgstr ""
 
 msgctxt "help:country.country,code:"
 msgid "The 2 chars ISO country code."
-msgstr "Cod ISO de țara din 2 litere."
+msgstr ""
 
 msgctxt "help:country.country,code_numeric:"
 msgid "The ISO numeric country code."
-msgstr "Cod numeric de țara ISO."
+msgstr ""
 
 msgctxt "help:country.country,name:"
 msgid "The main identifier of the country."
-msgstr "Identificatorul principal al țarii."
+msgstr ""
 
 msgctxt "help:country.postal_code,city:"
 msgid "The city associated with the postal code."
-msgstr "Orașul asociat cu codul poștal."
+msgstr ""
 
 msgctxt "help:country.postal_code,country:"
 msgid "The country that contains the postal code."
-msgstr "Țara care conține codul poștal."
+msgstr ""
 
 msgctxt "help:country.postal_code,subdivision:"
 msgid "The subdivision where the postal code is."
-msgstr "Subdiviziunea în care se află codul poștal."
+msgstr ""
 
-#, fuzzy
 msgctxt "help:country.region,code_numeric:"
 msgid "UN M49 region code."
-msgstr "Cod de regiune ONU M49."
+msgstr ""
 
 msgctxt "help:country.subdivision,code:"
 msgid "The ISO code of the subdivision."
-msgstr "Codul ISO al subdiviziuni."
+msgstr ""
 
 msgctxt "help:country.subdivision,country:"
 msgid "The country where this subdivision is."
-msgstr "Țara unde se afla subdiviziunea."
+msgstr ""
 
 msgctxt "help:country.subdivision,name:"
 msgid "The main identifier of the subdivision."
-msgstr "Identificatorul principal al subdiviziunii."
+msgstr ""
 
 msgctxt "help:country.subdivision,parent:"
 msgid "Add subdivision below the parent."
-msgstr "Adăugați subdiviziune sub părintele."
+msgstr ""
 
 msgctxt "model:country.country,name:"
 msgid "Country"
-msgstr "Țară"
+msgstr "Ülke"
 
 msgctxt "model:country.organization,name:"
 msgid "Organization"
-msgstr "Organizație"
+msgstr ""
 
 msgctxt "model:country.organization,name:organization_amu"
 msgid "Arab Maghreb Union"
-msgstr "Uniunea Maghrebului Arab"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:country.organization,name:organization_apec"
 msgid "Asia-Pacific Economic Cooperation"
-msgstr "Cooperarea Economică Asia-Pacific"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:country.organization,name:organization_asean"
 msgid "Association of Southeast Asian Nations"
-msgstr "Asociația Națiunilor din Asia de Sud-Est"
+msgstr ""
 
 msgctxt "model:country.organization,name:organization_benelux"
 msgid "Benelux Union"
-msgstr "Uniunea Benelux"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:country.organization,name:organization_can"
 msgid "Andean Community"
-msgstr "Comunitatea Andină"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:country.organization,name:organization_caricom"
 msgid "Caribbean Community"
-msgstr "Comunitatea Caraibelor"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:country.organization,name:organization_cemac"
 msgid "Economic and Monetary Community of Central Africa"
-msgstr "Comunitatea Economică și Monetară a Africii Centrale"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:country.organization,name:organization_cen-sad"
 msgid "Community of Sahel–Saharan States"
-msgstr "Comunitatea Statelor Sahel-Sahariene"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:country.organization,name:organization_comesa"
 msgid "Common Market for Eastern and Southern Africa"
-msgstr "Piața comună pentru Africa de Est și de Sud"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:country.organization,name:organization_eac"
 msgid "East African Community"
-msgstr "Comunitatea Est-Africană"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:country.organization,name:organization_eccas"
 msgid "Economic Community of Central African States"
-msgstr "Comunitatea Economică a Statelor Africii Centrale"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:country.organization,name:organization_ecowas"
 msgid "Economic Community of West African States"
-msgstr "Comunitatea Economică a Statelor Africii de Vest"
+msgstr ""
 
+#, fuzzy
 msgctxt "model:country.organization,name:organization_eu"
 msgid "European Union"
-msgstr "Uniunea Europeană"
+msgstr "La Union"
 
-#, fuzzy
 msgctxt "model:country.organization,name:organization_gcc"
 msgid "Cooperation Council for the Arab States of the Gulf"
-msgstr "Consiliul de Cooperare pentru Statele Arabe din Golf"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:country.organization,name:organization_igad"
 msgid "Intergovernmental Authority on Development"
-msgstr "Autoritatea Interguvernamentală pentru Dezvoltare"
+msgstr ""
 
 #, fuzzy
 msgctxt "model:country.organization,name:organization_mercosur"
 msgid "Southern Common Market"
-msgstr "Piața comună de sud"
+msgstr "Southern Leyte"
 
-#, fuzzy
 msgctxt "model:country.organization,name:organization_nafta"
 msgid "North American Free Trade Agreement"
-msgstr "Acordul de Liber Schimb din America de Nord"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:country.organization,name:organization_sadc"
 msgid "Southern African Development Community"
-msgstr "Comunitatea de Dezvoltare a Africii de Sud"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:country.organization,name:organization_safta"
 msgid "South Asian Free Trade Area"
-msgstr "Zona de schimb liber din Asia de Sud"
+msgstr ""
 
 msgctxt "model:country.organization.member,name:"
 msgid "Organization Member"
-msgstr "Membru al organizației"
+msgstr ""
 
 msgctxt "model:country.postal_code,name:"
 msgid "Postal Code"
-msgstr "Cod Poștal"
+msgstr ""
 
 msgctxt "model:country.region,name:"
 msgid "Region"
-msgstr "Regiune"
+msgstr ""
 
+#, fuzzy
 msgctxt "model:country.region,name:region_africa"
 msgid "Africa"
-msgstr "Africa"
+msgstr "Güney Afrika"
 
+#, fuzzy
 msgctxt "model:country.region,name:region_americas"
 msgid "Americas"
-msgstr ""
+msgstr "Amerikan Samoası"
 
+#, fuzzy
 msgctxt "model:country.region,name:region_antarctica"
 msgid "Antarctica"
-msgstr "Antarctica"
+msgstr "Antarktika"
 
 msgctxt "model:country.region,name:region_asia"
 msgid "Asia"
-msgstr "Asia"
+msgstr ""
 
+#, fuzzy
 msgctxt "model:country.region,name:region_australia_new_zealand"
 msgid "Australia and New Zealand"
-msgstr "Australia și Noua Zeelandă"
+msgstr "Yeni Zelanda"
 
 msgctxt "model:country.region,name:region_caribbean"
 msgid "Caribbean"
-msgstr "Caraibe"
+msgstr ""
 
+#, fuzzy
 msgctxt "model:country.region,name:region_central_america"
 msgid "Central America"
-msgstr "America Centrală"
+msgstr "Central Abaco"
 
+#, fuzzy
 msgctxt "model:country.region,name:region_central_asia"
 msgid "Central Asia"
-msgstr "Asia Centrala"
+msgstr "Central Abaco"
 
 #, fuzzy
 msgctxt "model:country.region,name:region_channel_islands"
 msgid "Channel Islands"
-msgstr "Insulele Canalului"
+msgstr "Line Islands"
 
+#, fuzzy
 msgctxt "model:country.region,name:region_eastern_africa"
 msgid "Eastern Africa"
-msgstr "Africa de Est"
+msgstr "Eastern Equatoria"
 
+#, fuzzy
 msgctxt "model:country.region,name:region_eastern_asia"
 msgid "Eastern Asia"
-msgstr "Asia de Est"
+msgstr "Eastern Cape"
 
+#, fuzzy
 msgctxt "model:country.region,name:region_eastern_europe"
 msgid "Eastern Europe"
-msgstr "Europa de Est"
+msgstr "Eastern Cape"
 
 msgctxt "model:country.region,name:region_europe"
 msgid "Europe"
-msgstr "Europa"
+msgstr ""
 
+#, fuzzy
 msgctxt "model:country.region,name:region_latin_america_caribbean"
 msgid "Latin America and the Caribbean"
-msgstr "America Latină și Caraibe"
+msgstr "Sen Vinsınt ve Granadalar"
 
+#, fuzzy
 msgctxt "model:country.region,name:region_melanesia"
 msgid "Melanesia"
-msgstr "Melanezia"
+msgstr "Melaka"
 
+#, fuzzy
 msgctxt "model:country.region,name:region_micronesia"
 msgid "Micronesia"
-msgstr "Micronezia"
+msgstr "Misiones"
 
-#, fuzzy
 msgctxt "model:country.region,name:region_middle_africa"
 msgid "Middle Africa"
-msgstr "Africa Centrală"
+msgstr ""
 
+#, fuzzy
 msgctxt "model:country.region,name:region_north_america"
 msgid "North America"
-msgstr "America de Nord"
+msgstr "Güney Afrika"
 
+#, fuzzy
 msgctxt "model:country.region,name:region_northern_africa"
 msgid "Northern Africa"
-msgstr "Africa de Nord"
+msgstr "Güney Afrika"
 
+#, fuzzy
 msgctxt "model:country.region,name:region_northern_america"
 msgid "Northern America"
-msgstr "America de Nord"
+msgstr "Northern Samar"
 
+#, fuzzy
 msgctxt "model:country.region,name:region_northern_europe"
 msgid "Northern Europe"
-msgstr "Europa de Nord"
+msgstr "Northern Cape"
 
+#, fuzzy
 msgctxt "model:country.region,name:region_oceania"
 msgid "Oceania"
-msgstr "Oceania"
+msgstr "Chania"
 
+#, fuzzy
 msgctxt "model:country.region,name:region_polynesia"
 msgid "Polynesia"
-msgstr "Polinezia"
+msgstr "Fransız Polinezyası"
 
+#, fuzzy
 msgctxt "model:country.region,name:region_south-eastern_asia"
 msgid "South-eastern Asia"
-msgstr "Asia de Sud-Est"
+msgstr "North-Western"
 
+#, fuzzy
 msgctxt "model:country.region,name:region_south_america"
 msgid "South America"
-msgstr "America de Sud"
+msgstr "Güney Afrika"
 
+#, fuzzy
 msgctxt "model:country.region,name:region_southern_africa"
 msgid "Southern Africa"
-msgstr "Africa de Sud"
+msgstr "Güney Afrika"
 
+#, fuzzy
 msgctxt "model:country.region,name:region_southern_asia"
 msgid "Southern Asia"
-msgstr "Asia de Sud"
+msgstr "Southern"
 
+#, fuzzy
 msgctxt "model:country.region,name:region_southern_europe"
 msgid "Southern Europe"
-msgstr "Europa de Sud"
+msgstr "Southern"
 
+#, fuzzy
 msgctxt "model:country.region,name:region_sub-saharan_africa"
 msgid "Sub-Saharan Africa"
-msgstr "Africa Sub-Sahariană"
+msgstr "Güney Afrika"
 
+#, fuzzy
 msgctxt "model:country.region,name:region_western_africa"
 msgid "Western Africa"
-msgstr "Africa de Vest"
+msgstr "Western Australia"
 
+#, fuzzy
 msgctxt "model:country.region,name:region_western_asia"
 msgid "Western Asia"
-msgstr "Asia de Vest"
+msgstr "Western Australia"
 
+#, fuzzy
 msgctxt "model:country.region,name:region_western_europe"
 msgid "Western Europe"
-msgstr "Europa de Vest"
+msgstr "Western Cape"
 
 msgctxt "model:country.region,name:region_world"
 msgid "World"
-msgstr "Lume"
+msgstr ""
 
 msgctxt "model:country.subdivision,name:"
 msgid "Subdivision"
-msgstr "Subdiviziune"
+msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_country_by_region"
 msgid "Countries by Region"
-msgstr "Țări după regiune"
+msgstr "Central Region"
 
 msgctxt "model:ir.action,name:act_country_form"
 msgid "Countries"
-msgstr "Țări"
+msgstr "Countries"
 
 msgctxt "model:ir.action,name:act_organization_form"
 msgid "Organizations"
-msgstr "Organizații"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_postal_code_form"
 msgid "Postal Codes"
-msgstr "Coduri Poștale"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_region_form"
 msgid "Regions"
-msgstr "Regiuni"
+msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_region_tree"
 msgid "Areas"
-msgstr "Zone"
+msgstr "Alan"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_country"
 msgid "Countries"
-msgstr "Țări"
+msgstr "Countries"
 
 msgctxt "model:ir.ui.menu,name:menu_country_form"
 msgid "Countries"
-msgstr "Țări"
+msgstr "Countries"
 
 msgctxt "model:ir.ui.menu,name:menu_organization_form"
 msgid "Organizations"
-msgstr "Organizații"
+msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_region_form"
 msgid "Regions"
-msgstr "Regiuni"
+msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_region_tree"
 msgid "Areas"
-msgstr "Zone"
+msgstr "Alan"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Administration"
-msgstr "Administrare"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Administrative Region"
-msgstr "Regiunea administrativă"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Administrative Territory"
-msgstr "Teritoriul administrativ"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Administrative area"
-msgstr "Zona administrativă"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Administrative atoll"
-msgstr "Atol administrativ"
+msgstr ""
 
-#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Administrative precinct"
-msgstr "Regiunea administrativă"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Arctic Region"
-msgstr "Regiunea Arctică"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Area"
-msgstr "Zonă"
+msgstr "Alan"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Atoll"
-msgstr "Atol"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Autonomous City"
-msgstr "Oraș autonom"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Autonomous Commune"
-msgstr "Comuna autonomă"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Autonomous District"
-msgstr "District autonom"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Autonomous Province"
-msgstr "Provincia autonomă"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Autonomous Region"
-msgstr "Regiune autonomă"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Autonomous city in north africa"
-msgstr "Oraș autonom din Africa de Nord"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Autonomous communities"
-msgstr "Comunitățile autonome"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Autonomous community"
-msgstr "Comunitatea autonomă"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Autonomous island"
-msgstr "Insula autonomă"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Autonomous monastic state"
-msgstr "Stat monahal autonom"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Autonomous municipality"
-msgstr "Municipalitate autonomă"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Autonomous republic"
-msgstr "Republica autonomă"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Autonomous sector"
-msgstr "Sector autonom"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Autonomous territorial unit"
-msgstr "Unitatea teritorială autonomă"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Autonomous territory"
-msgstr "Teritoriu autonom"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Borough"
 msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Canton"
-msgstr "Canton"
+msgstr ""
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Capital"
-msgstr "Capitala"
+msgstr "Capiz"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Capital District"
 msgstr ""
 
-#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Capital Metropolitan City"
-msgstr "Capitala Metropolitană"
+msgstr ""
 
-#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Capital Territory"
-msgstr "Teritoriul Capitalei"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Capital city"
-msgstr "Capitala"
+msgstr ""
 
 #, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Chain (of islands)"
-msgstr "Lanț (de insule)"
+msgstr "Seyman Adaları"
 
-#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Chains (of islands)"
-msgstr "Lanțuri (de insule)"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "City"
-msgstr "Oraș"
+msgstr ""
 
-#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "City corporation"
-msgstr "Corporația orașului"
+msgstr ""
 
 #, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "City municipality"
-msgstr "Municipiul orașului"
+msgstr "Nairobi Municipality"
 
-#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "City with county rights"
-msgstr "Oraș cu drepturi județene"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Commune"
-msgstr "Comună"
+msgstr ""
 
-#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Constitutional province"
-msgstr "Provincie constituțională"
+msgstr ""
 
-#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Council area"
-msgstr "zona Consiliului"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Country"
-msgstr "Țară"
+msgstr "Ülke"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "County"
-msgstr "Județ"
+msgstr "Ülke"
 
-#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Decentralized regional entity"
-msgstr "Entitate regională descentralizată"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Department"
-msgstr "Departament"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Dependency"
-msgstr "Dependenţă"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Development region"
-msgstr "Regiunea de dezvoltare"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "District"
-msgstr "District"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "District council area"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "District municipality"
-msgstr "Municipalitate autonomă"
+msgstr "Nairobi Municipality"
 
-#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "District with special status"
-msgstr "District cu statut special"
+msgstr ""
 
-#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Districts under republic administration"
-msgstr "Districte aflate în administrarea republicii"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Division"
-msgstr "Divizia"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Economic Prefecture"
-msgstr "Prefectura economică"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Economic region"
-msgstr "Regiunea economică"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Emirate"
-msgstr "Emirat"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Entity"
-msgstr "Entitate"
+msgstr ""
 
-#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Federal Dependency"
-msgstr "Dependență federală"
+msgstr ""
 
-#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Federal District"
-msgstr "District federal"
+msgstr ""
 
-#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Federal Territories"
-msgstr "Teritoriile Federale"
+msgstr ""
 
 #, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Federal Territory"
-msgstr "Teritoriu federal"
+msgstr "Northern Territory"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Federal capital territory"
-msgstr ""
+msgstr "Australian Capital Territory"
 
-#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Free municipal consortium"
-msgstr "Consorțiu municipal gratuit"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Geographical entity"
-msgstr "Entitate geografică"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Geographical region"
-msgstr "Regiunea geografică"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Geographical unit"
-msgstr "Unitate geografică"
+msgstr ""
 
-#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Governorate"
-msgstr "Guvernorat"
+msgstr ""
 
-#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Group of islands (20 inhabited islands)"
-msgstr "Grup de insule (20 de insule locuite)"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Included for completeness"
 msgstr ""
 
-#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Indigenous region"
-msgstr "Regiune indigenă"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Island"
-msgstr "Insulă"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Island council"
-msgstr "Consiliu Insular"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Island group"
-msgstr "Grup de insule"
+msgstr ""
 
-#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Islands, groups of islands"
-msgstr "Insule, grupuri de insule"
+msgstr ""
 
 #, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Land"
-msgstr "Teren"
+msgstr "Landes"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Local council"
-msgstr "Consiliu Local"
+msgstr ""
 
-#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "London borough"
-msgstr "Cartier Londonez"
+msgstr ""
 
-#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Metropolitan administration"
-msgstr "Administrația metropolitană"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Metropolitan cities"
-msgstr "Orașe metropolitane"
+msgstr ""
 
-#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Metropolitan city"
-msgstr "Oraș metropolitan"
+msgstr ""
 
-#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Metropolitan collectivity with special status"
-msgstr "Colectivitate metropolitană cu statut special"
+msgstr ""
 
-#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Metropolitan department"
-msgstr "Departament metropolitan"
+msgstr ""
 
-#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Metropolitan district"
-msgstr "District Metropolitan"
+msgstr ""
 
-#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Metropolitan region"
-msgstr "Regiune metropolitană"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Municipalities"
-msgstr "Municipalități"
+msgstr ""
 
-#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Municipality"
-msgstr "Municipiu"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Nation"
-msgstr "Naţiune"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Oblast"
-msgstr "Oblast"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Outlying area"
-msgstr "Zona periferică"
+msgstr ""
 
-#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Overseas collectivity"
-msgstr "Colectivitatea de peste mări"
+msgstr ""
 
-#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Overseas collectivity with special status"
-msgstr "Colectivitate de peste mări cu statut special"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Overseas department"
 msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Overseas region"
@@ -889,191 +879,181 @@
 msgid "Overseas region/department"
 msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Overseas territorial collectivity"
 msgstr ""
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Overseas territory"
-msgstr ""
+msgstr "Northern Territory"
 
-#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Pakistan administered area"
-msgstr "Zonă administrată de Pakistan"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Parish"
-msgstr "Parohie"
+msgstr "Paris"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Popularate"
-msgstr ""
+msgstr "Papua Barat"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Popularates"
 msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Prefecture"
-msgstr "Prefectură"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Principality"
-msgstr "Principat"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Province"
-msgstr "Provincie"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Quarter"
 msgstr ""
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Rayon"
-msgstr "Raion"
+msgstr "Rayong"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Region"
-msgstr "Regiune"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Regional council"
-msgstr "Consiliul regional"
+msgstr ""
 
-#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Regional state"
-msgstr "Stat regional"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Republic"
-msgstr "Republică"
+msgstr ""
 
-#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Republican City"
-msgstr "Oraș Republican"
+msgstr ""
 
 #, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Rural municipality"
-msgstr "Municipalitate rurală"
+msgstr "Nairobi Municipality"
 
-#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Self-governed part"
-msgstr "Parte autonomă"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Special District"
-msgstr "District special"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Special Municipality"
-msgstr "Municipalitatea specială"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Special Region"
-msgstr "Regiunea specială"
+msgstr ""
 
-#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Special administrative city"
-msgstr "Oraș administrativ special"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Special administrative region"
-msgstr "Regiunea administrativă specială"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Special city"
-msgstr "Oraș special"
+msgstr ""
 
-#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Special island authority"
-msgstr "Autoritate specială insulară"
+msgstr ""
 
-#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Special self-governing city"
-msgstr "Oraș special autonom"
+msgstr ""
 
-#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Special self-governing province"
-msgstr "Provincie Autonomă Specială"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Special zone"
-msgstr "Zona specială"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "State"
-msgstr "Stat"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Territorial unit"
-msgstr "Unitatea teritorială"
+msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Territory"
-msgstr "Teritoriu"
+msgstr ""
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Town"
-msgstr "Oraș"
+msgstr "Hope Town"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Town council"
-msgstr "Consiliul Local"
+msgstr ""
 
-#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Two-tier county"
-msgstr "Județul cu două niveluri"
+msgstr ""
 
-#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Union territory"
-msgstr "Teritoriul Uniunii"
+msgstr ""
 
-#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Unitary authority"
-msgstr "Autoritate unitară"
+msgstr ""
 
-#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Unitary authority (england)"
-msgstr "Autoritate unitară (Anglia)"
+msgstr ""
 
-#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Unitary authority (wales)"
-msgstr "Autoritate unitară (Țara Galilor)"
+msgstr ""
 
-#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Urban community"
-msgstr "Comunitate urbană"
+msgstr ""
 
 #, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Urban municipality"
-msgstr "Municipalitate urbană"
+msgstr "Nairobi Municipality"
 
-#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Voivodship"
-msgstr "Voievodat"
+msgstr ""
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Ward"
-msgstr ""
+msgstr "Wardak"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "zone"
-msgstr "zona"
+msgstr ""
```

### Comparing `trytond_country-7.2.0/locale/ru.po` & `trytond_country-7.2.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_country-7.2.0/locale/sl.po` & `trytond_country-7.2.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_country-7.2.0/locale/uk.po` & `trytond_country-7.2.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_country-7.2.0/locale/zh_CN.po` & `trytond_country-7.2.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_country-7.2.0/organization.xml` & `trytond_country-7.2.1/organization.xml`

 * *Files identical despite different names*

### Comparing `trytond_country-7.2.0/region.xml` & `trytond_country-7.2.1/region.xml`

 * *Files identical despite different names*

### Comparing `trytond_country-7.2.0/scripts/import_countries.py` & `trytond_country-7.2.1/scripts/import_countries.py`

 * *Files identical despite different names*

### Comparing `trytond_country-7.2.0/scripts/import_postal_codes.py` & `trytond_country-7.2.1/scripts/import_postal_codes.py`

 * *Files identical despite different names*

### Comparing `trytond_country-7.2.0/setup.py` & `trytond_country-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_country-7.2.0/tests/scenario_country_import.rst` & `trytond_country-7.2.1/tests/scenario_country_import.rst`

 * *Files identical despite different names*

### Comparing `trytond_country-7.2.0/tests/test_module.py` & `trytond_country-7.2.1/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_country-7.2.0/tox.ini` & `trytond_country-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_country-7.2.0/trytond_country.egg-info/PKG-INFO` & `trytond_country-7.2.1/trytond_country.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_country
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module with countries
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_country-7.2.0/trytond_country.egg-info/SOURCES.txt` & `trytond_country-7.2.1/trytond_country.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_country-7.2.0/view/country_form.xml` & `trytond_country-7.2.1/view/country_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_country-7.2.0/view/subdivision_form.xml` & `trytond_country-7.2.1/view/subdivision_form.xml`

 * *Files identical despite different names*

