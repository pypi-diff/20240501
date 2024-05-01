# Comparing `tmp/trytond_authentication_sms-7.2.0.tar.gz` & `tmp/trytond_authentication_sms-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_authentication_sms-7.2.0.tar", last modified: Mon Apr 29 15:38:23 2024, max compression
+gzip compressed data, was "trytond_authentication_sms-7.2.1.tar", last modified: Wed May  1 12:05:35 2024, max compression
```

## Comparing `trytond_authentication_sms-7.2.0.tar` & `trytond_authentication_sms-7.2.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:38:23.309310 trytond_authentication_sms-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1512 2024-04-29 15:18:10.000000 trytond_authentication_sms-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:18:09.000000 trytond_authentication_sms-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_authentication_sms-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_authentication_sms-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3388 2024-04-29 15:38:23.309310 trytond_authentication_sms-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1112 2023-04-15 07:12:15.000000 trytond_authentication_sms-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      331 2023-04-15 07:12:15.000000 trytond_authentication_sms-7.2.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:38:23.305977 trytond_authentication_sms-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3081 2024-04-27 16:30:39.000000 trytond_authentication_sms-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1112 2023-04-15 07:12:15.000000 trytond_authentication_sms-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:05.000000 trytond_authentication_sms-7.2.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:38:23.305977 trytond_authentication_sms-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      750 2024-04-27 16:43:22.000000 trytond_authentication_sms-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)      795 2024-04-27 16:43:22.000000 trytond_authentication_sms-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      683 2024-04-27 16:43:22.000000 trytond_authentication_sms-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)      828 2024-04-27 16:43:22.000000 trytond_authentication_sms-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)      818 2024-04-27 16:43:22.000000 trytond_authentication_sms-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      683 2024-04-27 16:43:22.000000 trytond_authentication_sms-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      795 2024-04-27 16:43:22.000000 trytond_authentication_sms-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)      868 2024-04-27 16:43:22.000000 trytond_authentication_sms-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      683 2024-04-27 16:43:22.000000 trytond_authentication_sms-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)      829 2024-04-27 16:43:22.000000 trytond_authentication_sms-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      747 2024-04-27 16:43:22.000000 trytond_authentication_sms-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      810 2024-04-27 16:43:22.000000 trytond_authentication_sms-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)      821 2024-04-27 16:43:22.000000 trytond_authentication_sms-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)      991 2024-04-27 16:43:22.000000 trytond_authentication_sms-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      683 2024-04-27 16:43:22.000000 trytond_authentication_sms-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      824 2024-04-27 16:43:22.000000 trytond_authentication_sms-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      820 2024-04-27 16:43:22.000000 trytond_authentication_sms-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      804 2024-04-27 16:43:22.000000 trytond_authentication_sms-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      803 2024-04-29 13:17:17.000000 trytond_authentication_sms-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      772 2024-04-27 16:43:22.000000 trytond_authentication_sms-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      818 2024-04-27 16:43:22.000000 trytond_authentication_sms-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      683 2024-04-27 16:43:22.000000 trytond_authentication_sms-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      683 2024-04-27 16:43:22.000000 trytond_authentication_sms-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      719 2024-04-27 16:43:22.000000 trytond_authentication_sms-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      498 2023-04-15 07:12:15.000000 trytond_authentication_sms-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3787 2023-04-15 07:12:15.000000 trytond_authentication_sms-7.2.0/res.py
--rw-r--r--   0 ced       (1000) ced       (1000)      567 2023-01-16 14:00:20.000000 trytond_authentication_sms-7.2.0/res.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:38:23.309310 trytond_authentication_sms-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4374 2024-03-17 11:01:36.000000 trytond_authentication_sms-7.2.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:38:23.305977 trytond_authentication_sms-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      202 2023-04-15 07:12:15.000000 trytond_authentication_sms-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3660 2024-01-27 09:58:52.000000 trytond_authentication_sms-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:05.000000 trytond_authentication_sms-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       80 2024-04-29 15:18:05.000000 trytond_authentication_sms-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:38:23.309310 trytond_authentication_sms-7.2.0/trytond_authentication_sms.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3388 2024-04-29 15:38:22.000000 trytond_authentication_sms-7.2.0/trytond_authentication_sms.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1451 2024-04-29 15:38:23.000000 trytond_authentication_sms-7.2.0/trytond_authentication_sms.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:38:22.000000 trytond_authentication_sms-7.2.0/trytond_authentication_sms.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       74 2024-04-29 15:38:22.000000 trytond_authentication_sms-7.2.0/trytond_authentication_sms.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:54.000000 trytond_authentication_sms-7.2.0/trytond_authentication_sms.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       26 2024-04-29 15:38:22.000000 trytond_authentication_sms-7.2.0/trytond_authentication_sms.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:38:22.000000 trytond_authentication_sms-7.2.0/trytond_authentication_sms.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:38:23.309310 trytond_authentication_sms-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      190 2023-04-15 07:12:15.000000 trytond_authentication_sms-7.2.0/view/user_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      193 2023-04-15 07:12:15.000000 trytond_authentication_sms-7.2.0/view/user_form_preferences.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:05:35.920483 trytond_authentication_sms-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1613 2024-05-01 12:05:32.000000 trytond_authentication_sms-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-05-01 12:05:32.000000 trytond_authentication_sms-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:20:59.000000 trytond_authentication_sms-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:20:59.000000 trytond_authentication_sms-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3388 2024-05-01 12:05:35.920483 trytond_authentication_sms-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1112 2024-04-30 17:20:59.000000 trytond_authentication_sms-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      331 2024-04-30 17:20:59.000000 trytond_authentication_sms-7.2.1/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:05:35.917150 trytond_authentication_sms-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3081 2024-04-30 17:20:59.000000 trytond_authentication_sms-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1112 2024-04-30 17:20:59.000000 trytond_authentication_sms-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:20:59.000000 trytond_authentication_sms-7.2.1/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:05:35.917150 trytond_authentication_sms-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)      750 2024-04-30 17:20:59.000000 trytond_authentication_sms-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      795 2024-04-30 17:20:59.000000 trytond_authentication_sms-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      683 2024-04-30 17:20:59.000000 trytond_authentication_sms-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      828 2024-04-30 17:20:59.000000 trytond_authentication_sms-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      818 2024-04-30 17:20:59.000000 trytond_authentication_sms-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      683 2024-04-30 17:20:59.000000 trytond_authentication_sms-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      795 2024-04-30 17:20:59.000000 trytond_authentication_sms-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      868 2024-04-30 17:20:59.000000 trytond_authentication_sms-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      683 2024-04-30 17:20:59.000000 trytond_authentication_sms-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      829 2024-04-30 17:20:59.000000 trytond_authentication_sms-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      747 2024-04-30 17:20:59.000000 trytond_authentication_sms-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      810 2024-04-30 17:20:59.000000 trytond_authentication_sms-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      821 2024-04-30 17:20:59.000000 trytond_authentication_sms-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      991 2024-04-30 17:20:59.000000 trytond_authentication_sms-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      683 2024-04-30 17:20:59.000000 trytond_authentication_sms-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      822 2024-04-30 17:21:59.000000 trytond_authentication_sms-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      820 2024-04-30 17:20:59.000000 trytond_authentication_sms-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      804 2024-04-30 17:20:59.000000 trytond_authentication_sms-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      803 2024-04-30 17:20:59.000000 trytond_authentication_sms-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      772 2024-04-30 17:20:59.000000 trytond_authentication_sms-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      818 2024-04-30 17:20:59.000000 trytond_authentication_sms-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      683 2024-04-30 17:20:59.000000 trytond_authentication_sms-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      683 2024-04-30 17:20:59.000000 trytond_authentication_sms-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      719 2024-04-30 17:20:59.000000 trytond_authentication_sms-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      498 2024-04-30 17:20:59.000000 trytond_authentication_sms-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3787 2024-04-30 17:20:59.000000 trytond_authentication_sms-7.2.1/res.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      567 2024-04-30 17:20:59.000000 trytond_authentication_sms-7.2.1/res.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 12:05:35.920483 trytond_authentication_sms-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4374 2024-04-30 17:20:59.000000 trytond_authentication_sms-7.2.1/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:05:35.917150 trytond_authentication_sms-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      202 2024-04-30 17:20:59.000000 trytond_authentication_sms-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3660 2024-04-30 17:20:59.000000 trytond_authentication_sms-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:20:59.000000 trytond_authentication_sms-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       80 2024-04-30 17:21:06.000000 trytond_authentication_sms-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:05:35.917150 trytond_authentication_sms-7.2.1/trytond_authentication_sms.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3388 2024-05-01 12:05:35.000000 trytond_authentication_sms-7.2.1/trytond_authentication_sms.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1451 2024-05-01 12:05:35.000000 trytond_authentication_sms-7.2.1/trytond_authentication_sms.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:05:35.000000 trytond_authentication_sms-7.2.1/trytond_authentication_sms.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       74 2024-05-01 12:05:35.000000 trytond_authentication_sms-7.2.1/trytond_authentication_sms.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:05:35.000000 trytond_authentication_sms-7.2.1/trytond_authentication_sms.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       26 2024-05-01 12:05:35.000000 trytond_authentication_sms-7.2.1/trytond_authentication_sms.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 12:05:35.000000 trytond_authentication_sms-7.2.1/trytond_authentication_sms.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:05:35.917150 trytond_authentication_sms-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      190 2024-04-30 17:20:59.000000 trytond_authentication_sms-7.2.1/view/user_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      193 2024-04-30 17:20:59.000000 trytond_authentication_sms-7.2.1/view/user_form_preferences.xml
```

### Comparing `trytond_authentication_sms-7.2.0/CHANGELOG` & `trytond_authentication_sms-7.2.1/CHANGELOG`

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

### Comparing `trytond_authentication_sms-7.2.0/COPYRIGHT` & `trytond_authentication_sms-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_authentication_sms-7.2.0/LICENSE` & `trytond_authentication_sms-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_authentication_sms-7.2.0/PKG-INFO` & `trytond_authentication_sms-7.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_authentication_sms
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module to authenticate users via SMS
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_authentication_sms-7.2.0/README.rst` & `trytond_authentication_sms-7.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_authentication_sms-7.2.0/doc/conf.py` & `trytond_authentication_sms-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_authentication_sms-7.2.0/doc/index.rst` & `trytond_authentication_sms-7.2.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_authentication_sms-7.2.0/locale/bg.po` & `trytond_authentication_sms-7.2.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_authentication_sms-7.2.0/locale/ca.po` & `trytond_authentication_sms-7.2.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_authentication_sms-7.2.0/locale/cs.po` & `trytond_authentication_sms-7.2.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_authentication_sms-7.2.0/locale/de.po` & `trytond_authentication_sms-7.2.1/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_authentication_sms-7.2.0/locale/es.po` & `trytond_authentication_sms-7.2.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_authentication_sms-7.2.0/locale/es_419.po` & `trytond_authentication_sms-7.2.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_authentication_sms-7.2.0/locale/et.po` & `trytond_authentication_sms-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_authentication_sms-7.2.0/locale/fa.po` & `trytond_authentication_sms-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_authentication_sms-7.2.0/locale/fi.po` & `trytond_authentication_sms-7.2.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_authentication_sms-7.2.0/locale/fr.po` & `trytond_authentication_sms-7.2.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_authentication_sms-7.2.0/locale/hu.po` & `trytond_authentication_sms-7.2.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_authentication_sms-7.2.0/locale/id.po` & `trytond_authentication_sms-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_authentication_sms-7.2.0/locale/it.po` & `trytond_authentication_sms-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_authentication_sms-7.2.0/locale/lo.po` & `trytond_authentication_sms-7.2.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_authentication_sms-7.2.0/locale/lt.po` & `trytond_authentication_sms-7.2.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_authentication_sms-7.2.0/locale/nl.po` & `trytond_authentication_sms-7.2.1/locale/nl.po`

 * *Files 1% similar despite different names*

```diff
@@ -24,12 +24,12 @@
 
 msgctxt "model:ir.message,text:msg_sms_text"
 msgid "%(name)s code %(code)s"
 msgstr "%(name)s code %(code)s"
 
 msgctxt "model:ir.message,text:msg_user_sms_code"
 msgid "SMS Code for %(login)s"
-msgstr "SMS-code voor% (login) s"
+msgstr "SMS-code voor%(login)s"
 
 msgctxt "model:res.user.login.sms_code,name:"
 msgid "SMS Code"
 msgstr "SMS-code"
```

### Comparing `trytond_authentication_sms-7.2.0/locale/pl.po` & `trytond_authentication_sms-7.2.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_authentication_sms-7.2.0/locale/pt.po` & `trytond_authentication_sms-7.2.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_authentication_sms-7.2.0/locale/ro.po` & `trytond_authentication_sms-7.2.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_authentication_sms-7.2.0/locale/ru.po` & `trytond_authentication_sms-7.2.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_authentication_sms-7.2.0/locale/sl.po` & `trytond_authentication_sms-7.2.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_authentication_sms-7.2.0/locale/tr.po` & `trytond_authentication_sms-7.2.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_authentication_sms-7.2.0/locale/uk.po` & `trytond_authentication_sms-7.2.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_authentication_sms-7.2.0/locale/zh_CN.po` & `trytond_authentication_sms-7.2.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_authentication_sms-7.2.0/res.py` & `trytond_authentication_sms-7.2.1/res.py`

 * *Files identical despite different names*

### Comparing `trytond_authentication_sms-7.2.0/res.xml` & `trytond_authentication_sms-7.2.1/res.xml`

 * *Files identical despite different names*

### Comparing `trytond_authentication_sms-7.2.0/setup.py` & `trytond_authentication_sms-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_authentication_sms-7.2.0/tests/test_module.py` & `trytond_authentication_sms-7.2.1/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_authentication_sms-7.2.0/tox.ini` & `trytond_authentication_sms-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_authentication_sms-7.2.0/trytond_authentication_sms.egg-info/PKG-INFO` & `trytond_authentication_sms-7.2.1/trytond_authentication_sms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_authentication_sms
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module to authenticate users via SMS
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_authentication_sms-7.2.0/trytond_authentication_sms.egg-info/SOURCES.txt` & `trytond_authentication_sms-7.2.1/trytond_authentication_sms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

