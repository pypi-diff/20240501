# Comparing `tmp/trytond_web_user-7.2.0.tar.gz` & `tmp/trytond_web_user-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_web_user-7.2.0.tar", last modified: Mon Apr 29 15:54:37 2024, max compression
+gzip compressed data, was "trytond_web_user-7.2.1.tar", last modified: Wed May  1 09:50:06 2024, max compression
```

## Comparing `trytond_web_user-7.2.0.tar` & `trytond_web_user-7.2.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:37.433833 trytond_web_user-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     2096 2024-04-29 15:30:21.000000 trytond_web_user-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:30:21.000000 trytond_web_user-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_web_user-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_web_user-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2572 2024-04-29 15:54:37.433833 trytond_web_user-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      225 2024-04-22 12:14:37.000000 trytond_web_user-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      677 2023-04-15 07:12:15.000000 trytond_web_user-7.2.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:37.430499 trytond_web_user-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3071 2024-04-27 16:30:39.000000 trytond_web_user-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      946 2024-04-22 12:14:37.000000 trytond_web_user-7.2.0/doc/configuration.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1615 2024-04-22 12:14:37.000000 trytond_web_user-7.2.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      225 2024-04-22 12:14:37.000000 trytond_web_user-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-22 12:14:37.000000 trytond_web_user-7.2.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:40.000000 trytond_web_user-7.2.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     1690 2024-04-22 12:14:36.000000 trytond_web_user-7.2.0/email_reset_password.html
--rw-r--r--   0 ced       (1000) ced       (1000)     1187 2023-04-15 07:12:15.000000 trytond_web_user-7.2.0/email_validation.html
--rw-r--r--   0 ced       (1000) ced       (1000)      253 2024-02-04 18:51:27.000000 trytond_web_user-7.2.0/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1759 2023-04-15 07:12:15.000000 trytond_web_user-7.2.0/ir.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:37.433833 trytond_web_user-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     4621 2024-04-29 13:17:17.000000 trytond_web_user-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5227 2024-04-29 13:17:17.000000 trytond_web_user-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4374 2024-04-29 13:17:17.000000 trytond_web_user-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5355 2024-04-29 13:17:17.000000 trytond_web_user-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5325 2024-04-29 13:17:17.000000 trytond_web_user-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4148 2024-04-29 13:17:17.000000 trytond_web_user-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4528 2024-04-29 13:17:17.000000 trytond_web_user-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5624 2024-04-29 13:17:17.000000 trytond_web_user-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4374 2024-04-29 13:17:17.000000 trytond_web_user-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5298 2024-04-29 13:17:17.000000 trytond_web_user-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4993 2024-04-29 13:17:17.000000 trytond_web_user-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4623 2024-04-29 13:17:17.000000 trytond_web_user-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4635 2024-04-29 13:17:17.000000 trytond_web_user-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6395 2024-04-29 13:17:17.000000 trytond_web_user-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4444 2024-04-29 13:17:17.000000 trytond_web_user-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5051 2024-04-29 13:17:17.000000 trytond_web_user-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4374 2024-04-29 13:17:17.000000 trytond_web_user-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4904 2024-04-29 13:17:17.000000 trytond_web_user-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5133 2024-04-29 13:17:17.000000 trytond_web_user-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4574 2024-04-29 13:17:17.000000 trytond_web_user-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5225 2024-04-29 13:17:17.000000 trytond_web_user-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4374 2024-04-29 13:17:17.000000 trytond_web_user-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5781 2024-04-29 13:17:17.000000 trytond_web_user-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5031 2024-04-29 13:17:17.000000 trytond_web_user-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      730 2024-02-04 18:51:27.000000 trytond_web_user-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      812 2023-04-15 07:12:15.000000 trytond_web_user-7.2.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:54:37.433833 trytond_web_user-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4475 2024-04-27 16:30:39.000000 trytond_web_user-7.2.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:37.433833 trytond_web_user-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_web_user-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6663 2024-04-27 16:30:39.000000 trytond_web_user-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:40.000000 trytond_web_user-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       83 2024-04-29 15:30:17.000000 trytond_web_user-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:37.433833 trytond_web_user-7.2.0/trytond_web_user.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2572 2024-04-29 15:54:37.000000 trytond_web_user-7.2.0/trytond_web_user.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1579 2024-04-29 15:54:37.000000 trytond_web_user-7.2.0/trytond_web_user.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:54:37.000000 trytond_web_user-7.2.0/trytond_web_user.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       54 2024-04-29 15:54:37.000000 trytond_web_user-7.2.0/trytond_web_user.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:55.000000 trytond_web_user-7.2.0/trytond_web_user.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-29 15:54:37.000000 trytond_web_user-7.2.0/trytond_web_user.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:54:37.000000 trytond_web_user-7.2.0/trytond_web_user.egg-info/top_level.txt
--rw-r--r--   0 ced       (1000) ced       (1000)    18214 2024-04-27 16:30:39.000000 trytond_web_user-7.2.0/user.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4701 2024-04-27 16:30:39.000000 trytond_web_user-7.2.0/user.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:37.433833 trytond_web_user-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      853 2024-01-27 09:58:52.000000 trytond_web_user-7.2.0/view/user_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      518 2024-01-27 09:58:52.000000 trytond_web_user-7.2.0/view/user_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:50:06.811352 trytond_web_user-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2197 2024-05-01 09:50:03.000000 trytond_web_user-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-05-01 09:50:03.000000 trytond_web_user-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:21:00.000000 trytond_web_user-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:21:00.000000 trytond_web_user-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2572 2024-05-01 09:50:06.811352 trytond_web_user-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      225 2024-04-30 17:21:00.000000 trytond_web_user-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      677 2024-04-30 17:21:00.000000 trytond_web_user-7.2.1/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:50:06.808018 trytond_web_user-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3071 2024-04-30 17:21:00.000000 trytond_web_user-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      946 2024-04-30 17:21:00.000000 trytond_web_user-7.2.1/doc/configuration.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1615 2024-04-30 17:21:00.000000 trytond_web_user-7.2.1/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      225 2024-04-30 17:21:00.000000 trytond_web_user-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-30 17:21:00.000000 trytond_web_user-7.2.1/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:21:00.000000 trytond_web_user-7.2.1/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     1690 2024-04-30 17:21:00.000000 trytond_web_user-7.2.1/email_reset_password.html
+-rw-r--r--   0 ced       (1000) ced       (1000)     1187 2024-04-30 17:21:00.000000 trytond_web_user-7.2.1/email_validation.html
+-rw-r--r--   0 ced       (1000) ced       (1000)      253 2024-04-30 17:21:00.000000 trytond_web_user-7.2.1/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1759 2024-04-30 17:21:00.000000 trytond_web_user-7.2.1/ir.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:50:06.811352 trytond_web_user-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4621 2024-04-30 17:21:00.000000 trytond_web_user-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5559 2024-04-30 17:21:59.000000 trytond_web_user-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4374 2024-04-30 17:21:00.000000 trytond_web_user-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5729 2024-04-30 17:21:59.000000 trytond_web_user-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5664 2024-04-30 17:21:59.000000 trytond_web_user-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4148 2024-04-30 17:21:00.000000 trytond_web_user-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4528 2024-04-30 17:21:00.000000 trytond_web_user-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5624 2024-04-30 17:21:00.000000 trytond_web_user-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4374 2024-04-30 17:21:00.000000 trytond_web_user-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5681 2024-04-30 17:21:59.000000 trytond_web_user-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4993 2024-04-30 17:21:00.000000 trytond_web_user-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4623 2024-04-30 17:21:00.000000 trytond_web_user-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4635 2024-04-30 17:21:00.000000 trytond_web_user-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6395 2024-04-30 17:21:00.000000 trytond_web_user-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4444 2024-04-30 17:21:00.000000 trytond_web_user-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5403 2024-04-30 17:21:59.000000 trytond_web_user-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4374 2024-04-30 17:21:00.000000 trytond_web_user-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4904 2024-04-30 17:21:00.000000 trytond_web_user-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5133 2024-04-30 17:21:00.000000 trytond_web_user-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4574 2024-04-30 17:21:00.000000 trytond_web_user-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5225 2024-04-30 17:21:00.000000 trytond_web_user-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4374 2024-04-30 17:21:00.000000 trytond_web_user-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5781 2024-04-30 17:21:00.000000 trytond_web_user-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5031 2024-04-30 17:21:00.000000 trytond_web_user-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      730 2024-04-30 17:21:00.000000 trytond_web_user-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      812 2024-04-30 17:21:00.000000 trytond_web_user-7.2.1/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 09:50:06.811352 trytond_web_user-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4475 2024-04-30 17:21:00.000000 trytond_web_user-7.2.1/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:50:06.811352 trytond_web_user-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:21:00.000000 trytond_web_user-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6663 2024-04-30 17:21:00.000000 trytond_web_user-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:21:00.000000 trytond_web_user-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       83 2024-04-30 17:21:06.000000 trytond_web_user-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:50:06.811352 trytond_web_user-7.2.1/trytond_web_user.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2572 2024-05-01 09:50:06.000000 trytond_web_user-7.2.1/trytond_web_user.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1579 2024-05-01 09:50:06.000000 trytond_web_user-7.2.1/trytond_web_user.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 09:50:06.000000 trytond_web_user-7.2.1/trytond_web_user.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       54 2024-05-01 09:50:06.000000 trytond_web_user-7.2.1/trytond_web_user.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 09:50:06.000000 trytond_web_user-7.2.1/trytond_web_user.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-05-01 09:50:06.000000 trytond_web_user-7.2.1/trytond_web_user.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 09:50:06.000000 trytond_web_user-7.2.1/trytond_web_user.egg-info/top_level.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)    18214 2024-04-30 17:21:00.000000 trytond_web_user-7.2.1/user.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4701 2024-04-30 17:21:00.000000 trytond_web_user-7.2.1/user.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:50:06.811352 trytond_web_user-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      853 2024-04-30 17:21:00.000000 trytond_web_user-7.2.1/view/user_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      518 2024-04-30 17:21:00.000000 trytond_web_user-7.2.1/view/user_list.xml
```

### Comparing `trytond_web_user-7.2.0/CHANGELOG` & `trytond_web_user-7.2.1/CHANGELOG`

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
 
 
 Version 7.0.0 - 2023-10-30
 --------------------------
```

### Comparing `trytond_web_user-7.2.0/COPYRIGHT` & `trytond_web_user-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_web_user-7.2.0/LICENSE` & `trytond_web_user-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_web_user-7.2.0/PKG-INFO` & `trytond_web_user-7.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_web_user
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module to manage Web users
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_web_user-7.2.0/__init__.py` & `trytond_web_user-7.2.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_web_user-7.2.0/doc/conf.py` & `trytond_web_user-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_web_user-7.2.0/doc/configuration.rst` & `trytond_web_user-7.2.1/doc/configuration.rst`

 * *Files identical despite different names*

### Comparing `trytond_web_user-7.2.0/doc/design.rst` & `trytond_web_user-7.2.1/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_web_user-7.2.0/email_reset_password.html` & `trytond_web_user-7.2.1/email_reset_password.html`

 * *Files identical despite different names*

### Comparing `trytond_web_user-7.2.0/email_validation.html` & `trytond_web_user-7.2.1/email_validation.html`

 * *Files identical despite different names*

### Comparing `trytond_web_user-7.2.0/ir.py` & `trytond_web_user-7.2.1/ir.py`

 * *Files identical despite different names*

### Comparing `trytond_web_user-7.2.0/locale/bg.po` & `trytond_web_user-7.2.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_web_user-7.2.0/locale/ca.po` & `trytond_web_user-7.2.1/locale/ca.po`

 * *Files 2% similar despite different names*

```diff
@@ -122,27 +122,31 @@
 msgid "Web User Authenticate Attempt"
 msgstr "Intent d'autenticació usuari web"
 
 msgctxt "model:web.user.session,name:"
 msgid "Web User Session"
 msgstr "Sessió usuari web"
 
-#, fuzzy
 msgctxt "report:web.user.email_reset_password:"
 msgid "Button not working? Paste this into your browser:"
 msgstr "El botó no funciona? Empega això al teu navegador:"
 
 msgctxt "report:web.user.email_reset_password:"
 msgid ""
 "Hello, we received a request to reset the password for the account associated with [1:%(email)s]. No changes have been made to your account yet.[2:]\n"
 "                You can reset your password by clicking the link below:[3:]\n"
 "                [4:\n"
 "                    Reset Password\n"
 "                ]"
 msgstr ""
+"Hola, hem rebut una sol·licitud per restablir la contrasenya del compte associat a [1:%(email)s]. Encara no s'ha fet cap canvi al vostre compte.[2:]\n"
+"                Podeu restablir la vostra contrasenya fent clic a l'enllaç següent:[3:]\n"
+"                [4:\n"
+"                    Restablir la contrasenya\n"
+"                ]"
 
 msgctxt "report:web.user.email_reset_password:"
 msgid "If you didn't make this request, you can ignore this email."
 msgstr "Si no heu fet aquesta petició, podeu ignorar aquest correu."
 
 msgctxt "report:web.user.email_reset_password:"
 msgid "Reset Password"
```

### Comparing `trytond_web_user-7.2.0/locale/cs.po` & `trytond_web_user-7.2.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_web_user-7.2.0/locale/de.po` & `trytond_web_user-7.2.1/locale/de.po`

 * *Files 12% similar despite different names*

```diff
@@ -124,29 +124,33 @@
 msgid "Web User Authenticate Attempt"
 msgstr "Webbenutzer Authentifizierungsversuch"
 
 msgctxt "model:web.user.session,name:"
 msgid "Web User Session"
 msgstr "Webbenutzer Sitzung"
 
-#, fuzzy
 msgctxt "report:web.user.email_reset_password:"
 msgid "Button not working? Paste this into your browser:"
 msgstr ""
-"Wenn der Button nicht funktioniert, kopieren Sie bitte die folgende Zeile in"
-" die Adresszeile Ihres Browsers:"
+"Sollte der Button nicht funktionieren, kopieren Sie bitte den folgenden Text"
+" in die Adresszeile Ihres Browsers:"
 
 msgctxt "report:web.user.email_reset_password:"
 msgid ""
 "Hello, we received a request to reset the password for the account associated with [1:%(email)s]. No changes have been made to your account yet.[2:]\n"
 "                You can reset your password by clicking the link below:[3:]\n"
 "                [4:\n"
 "                    Reset Password\n"
 "                ]"
 msgstr ""
+"Hallo, wir haben eine Anfrage zum Zurücksetzen des Passworts für das mit [1:%(email)s) verknüpfte Konto erhalten. An Ihrem Konto wurden noch keine Änderungen vorgenommen.[2:]\n"
+"                Sie können Ihr Passwort zurücksetzen, indem Sie auf den folgenden Link klicken:[3:]\n"
+"                [4:\n"
+"                    Passwort zurücksetzen\n"
+"                ]"
 
 msgctxt "report:web.user.email_reset_password:"
 msgid "If you didn't make this request, you can ignore this email."
 msgstr ""
 "Ignorieren Sie bitte diese E-Mail, wenn Sie nicht der Urheber dieser Anfrage"
 " sind."
```

### Comparing `trytond_web_user-7.2.0/locale/es.po` & `trytond_web_user-7.2.1/locale/es.po`

 * *Files 3% similar despite different names*

```diff
@@ -122,27 +122,31 @@
 msgid "Web User Authenticate Attempt"
 msgstr "Intento de identificación usuario web"
 
 msgctxt "model:web.user.session,name:"
 msgid "Web User Session"
 msgstr "Sesión usuario web"
 
-#, fuzzy
 msgctxt "report:web.user.email_reset_password:"
 msgid "Button not working? Paste this into your browser:"
 msgstr "¿El botón no funciona? Pega esto en tu navegador:"
 
 msgctxt "report:web.user.email_reset_password:"
 msgid ""
 "Hello, we received a request to reset the password for the account associated with [1:%(email)s]. No changes have been made to your account yet.[2:]\n"
 "                You can reset your password by clicking the link below:[3:]\n"
 "                [4:\n"
 "                    Reset Password\n"
 "                ]"
 msgstr ""
+"Hola, recibimos una solicitud para restablecer la contraseña de la cuenta asociada con [1:%(email)s]. Aún no se han realizado cambios en su cuenta.[2:]\n"
+"                Puede restablecer su contraseña haciendo clic en el siguiente enlace:[3:]\n"
+"                [4:\n"
+"                    Restablecer la contraseña\n"
+"                ]"
 
 msgctxt "report:web.user.email_reset_password:"
 msgid "If you didn't make this request, you can ignore this email."
 msgstr ""
 "Si no habéis realizado esta petición, podéis ignorar este correo "
 "electrónico."
```

### Comparing `trytond_web_user-7.2.0/locale/es_419.po` & `trytond_web_user-7.2.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_web_user-7.2.0/locale/et.po` & `trytond_web_user-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_web_user-7.2.0/locale/fa.po` & `trytond_web_user-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_web_user-7.2.0/locale/fi.po` & `trytond_web_user-7.2.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_web_user-7.2.0/locale/fr.po` & `trytond_web_user-7.2.1/locale/fr.po`

 * *Files 4% similar despite different names*

```diff
@@ -122,27 +122,31 @@
 msgid "Web User Authenticate Attempt"
 msgstr "Tentative d'authentification d'utilisateur web"
 
 msgctxt "model:web.user.session,name:"
 msgid "Web User Session"
 msgstr "Session d'utilisateur web"
 
-#, fuzzy
 msgctxt "report:web.user.email_reset_password:"
 msgid "Button not working? Paste this into your browser:"
 msgstr "Le bouton ne fonctionne pas ? Copier ceci dans votre navigateur :"
 
 msgctxt "report:web.user.email_reset_password:"
 msgid ""
 "Hello, we received a request to reset the password for the account associated with [1:%(email)s]. No changes have been made to your account yet.[2:]\n"
 "                You can reset your password by clicking the link below:[3:]\n"
 "                [4:\n"
 "                    Reset Password\n"
 "                ]"
 msgstr ""
+"Bonjour, nous avons reçu une demande de réinitialisation du mot de passe du compte associé à [1:%(email)s]. Aucune modification n'a encore été apportée à votre compte.[2:]\n"
+"                Vous pouvez réinitialiser votre mot de passe en cliquant sur le lien ci-dessous :[3:]\n"
+"                [4:\n"
+"                    Réinitialiser le mot de passe\n"
+"                ]"
 
 msgctxt "report:web.user.email_reset_password:"
 msgid "If you didn't make this request, you can ignore this email."
 msgstr ""
 "Si vous n'avez pas fait cette demande, vous pouvez ignorer cet E-mail."
 
 msgctxt "report:web.user.email_reset_password:"
```

### Comparing `trytond_web_user-7.2.0/locale/hu.po` & `trytond_web_user-7.2.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_web_user-7.2.0/locale/id.po` & `trytond_web_user-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_web_user-7.2.0/locale/it.po` & `trytond_web_user-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_web_user-7.2.0/locale/lo.po` & `trytond_web_user-7.2.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_web_user-7.2.0/locale/lt.po` & `trytond_web_user-7.2.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_web_user-7.2.0/locale/nl.po` & `trytond_web_user-7.2.1/locale/nl.po`

 * *Files 4% similar despite different names*

```diff
@@ -122,27 +122,31 @@
 msgid "Web User Authenticate Attempt"
 msgstr "Inlog poging webgebruikers"
 
 msgctxt "model:web.user.session,name:"
 msgid "Web User Session"
 msgstr "Webgebruikerssessie"
 
-#, fuzzy
 msgctxt "report:web.user.email_reset_password:"
 msgid "Button not working? Paste this into your browser:"
-msgstr "Knop werkt niet? Plak dit in uw browser:"
+msgstr "Werkt de knop niet? Plak dit in uw browser:"
 
 msgctxt "report:web.user.email_reset_password:"
 msgid ""
 "Hello, we received a request to reset the password for the account associated with [1:%(email)s]. No changes have been made to your account yet.[2:]\n"
 "                You can reset your password by clicking the link below:[3:]\n"
 "                [4:\n"
 "                    Reset Password\n"
 "                ]"
 msgstr ""
+"Hallo, we hebben een aanvraag ontvangen om het wachtwoord voor gebruiker [1:%(email)s] te resetten. Op dit moment zijn er nog geen wijzigingen gedaan aan de gebruiker.[2:]\n"
+"                U kunt het wachtwoord resetten door op de onderstaande link te klikken:[3:]\n"
+"                [4:\n"
+"                     Reset wachtwoord\n"
+"                ]"
 
 msgctxt "report:web.user.email_reset_password:"
 msgid "If you didn't make this request, you can ignore this email."
 msgstr "Indien u dit verzoek niet hebt gedaan, kunt u deze e-mail negeren."
 
 msgctxt "report:web.user.email_reset_password:"
 msgid "Reset Password"
```

### Comparing `trytond_web_user-7.2.0/locale/pl.po` & `trytond_web_user-7.2.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_web_user-7.2.0/locale/pt.po` & `trytond_web_user-7.2.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_web_user-7.2.0/locale/ro.po` & `trytond_web_user-7.2.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_web_user-7.2.0/locale/ru.po` & `trytond_web_user-7.2.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_web_user-7.2.0/locale/sl.po` & `trytond_web_user-7.2.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_web_user-7.2.0/locale/tr.po` & `trytond_web_user-7.2.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_web_user-7.2.0/locale/uk.po` & `trytond_web_user-7.2.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_web_user-7.2.0/locale/zh_CN.po` & `trytond_web_user-7.2.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_web_user-7.2.0/message.xml` & `trytond_web_user-7.2.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_web_user-7.2.0/party.py` & `trytond_web_user-7.2.1/party.py`

 * *Files identical despite different names*

### Comparing `trytond_web_user-7.2.0/setup.py` & `trytond_web_user-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_web_user-7.2.0/tests/test_module.py` & `trytond_web_user-7.2.1/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_web_user-7.2.0/tox.ini` & `trytond_web_user-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_web_user-7.2.0/trytond_web_user.egg-info/PKG-INFO` & `trytond_web_user-7.2.1/trytond_web_user.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_web_user
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module to manage Web users
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_web_user-7.2.0/trytond_web_user.egg-info/SOURCES.txt` & `trytond_web_user-7.2.1/trytond_web_user.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_web_user-7.2.0/user.py` & `trytond_web_user-7.2.1/user.py`

 * *Files identical despite different names*

### Comparing `trytond_web_user-7.2.0/user.xml` & `trytond_web_user-7.2.1/user.xml`

 * *Files identical despite different names*

### Comparing `trytond_web_user-7.2.0/view/user_form.xml` & `trytond_web_user-7.2.1/view/user_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_web_user-7.2.0/view/user_list.xml` & `trytond_web_user-7.2.1/view/user_list.xml`

 * *Files identical despite different names*

