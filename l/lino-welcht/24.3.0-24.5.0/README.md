# Comparing `tmp/lino-welcht-24.3.0.tar.gz` & `tmp/lino-welcht-24.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lino-welcht-24.3.0.tar", last modified: Sat Mar  2 17:57:26 2024, max compression
+gzip compressed data, was "lino-welcht-24.5.0.tar", last modified: Wed May  1 06:06:16 2024, max compression
```

## Comparing `lino-welcht-24.3.0.tar` & `lino-welcht-24.5.0.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-02 17:57:26.711448 lino-welcht-24.3.0/
--rw-rw-rw-   0 luc       (1000) www-data    (33)    34523 2021-04-07 12:55:58.000000 lino-welcht-24.3.0/COPYING
--rw-rw-rw-   0 luc       (1000) www-data    (33)      105 2023-08-07 14:42:30.000000 lino-welcht-24.3.0/MANIFEST.in
--rw-r--r--   0 luc       (1000) www-data    (33)     1832 2024-03-02 17:57:26.711448 lino-welcht-24.3.0/PKG-INFO
--rw-rw-rw-   0 luc       (1000) www-data    (33)      734 2021-08-19 05:39:07.000000 lino-welcht-24.3.0/README.rst
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-02 17:57:26.707448 lino-welcht-24.3.0/lino_welcht/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      879 2024-02-14 17:30:47.000000 lino-welcht-24.3.0/lino_welcht/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      223 2024-02-14 17:30:47.000000 lino-welcht-24.3.0/lino_welcht/help_texts.py
--rw-rw-r--   0 luc       (1000) www-data    (33)     1684 2024-02-14 17:30:47.000000 lino-welcht-24.3.0/lino_welcht/layouts.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-02 17:57:26.707448 lino-welcht-24.3.0/lino_welcht/lib/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      257 2024-02-14 17:30:47.000000 lino-welcht-24.3.0/lino_welcht/lib/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-02 17:57:26.707448 lino-welcht-24.3.0/lino_welcht/lib/courses/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      545 2024-02-14 17:30:47.000000 lino-welcht-24.3.0/lino_welcht/lib/courses/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-02 17:57:26.703448 lino-welcht-24.3.0/lino_welcht/lib/courses/config/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-02 17:57:26.703448 lino-welcht-24.3.0/lino_welcht/lib/courses/config/courses/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-02 17:57:26.707448 lino-welcht-24.3.0/lino_welcht/lib/courses/config/courses/Enrolment/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1013 2015-09-19 03:53:35.000000 lino-welcht-24.3.0/lino_welcht/lib/courses/config/courses/Enrolment/enrolment.body.html
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1465 2015-09-19 03:53:35.000000 lino-welcht-24.3.0/lino_welcht/lib/courses/config/courses/Enrolment/intervention.body.html
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-02 17:57:26.707448 lino-welcht-24.3.0/lino_welcht/lib/courses/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:35.000000 lino-welcht-24.3.0/lino_welcht/lib/courses/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     4828 2024-02-14 17:30:47.000000 lino-welcht-24.3.0/lino_welcht/lib/courses/fixtures/demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      914 2024-02-14 17:30:47.000000 lino-welcht-24.3.0/lino_welcht/lib/courses/fixtures/std.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     3906 2024-02-14 17:30:47.000000 lino-welcht-24.3.0/lino_welcht/lib/courses/models.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1355 2024-02-14 17:30:47.000000 lino-welcht-24.3.0/lino_welcht/lib/courses/ui.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-02 17:57:26.707448 lino-welcht-24.3.0/lino_welcht/lib/cv/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1133 2024-02-14 17:30:47.000000 lino-welcht-24.3.0/lino_welcht/lib/cv/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-02 17:57:26.707448 lino-welcht-24.3.0/lino_welcht/lib/cv/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:36.000000 lino-welcht-24.3.0/lino_welcht/lib/cv/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      655 2024-02-14 17:30:47.000000 lino-welcht-24.3.0/lino_welcht/lib/cv/fixtures/demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      823 2023-10-20 06:35:18.000000 lino-welcht-24.3.0/lino_welcht/lib/cv/fixtures/std.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     7691 2024-02-14 17:30:47.000000 lino-welcht-24.3.0/lino_welcht/lib/cv/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-02 17:57:26.711448 lino-welcht-24.3.0/lino_welcht/lib/isip/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      288 2024-02-14 17:30:47.000000 lino-welcht-24.3.0/lino_welcht/lib/isip/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2038 2024-02-14 17:30:47.000000 lino-welcht-24.3.0/lino_welcht/lib/isip/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-02 17:57:26.711448 lino-welcht-24.3.0/lino_welcht/lib/pcsw/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      471 2024-02-14 17:30:47.000000 lino-welcht-24.3.0/lino_welcht/lib/pcsw/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      456 2024-02-14 17:30:47.000000 lino-welcht-24.3.0/lino_welcht/lib/pcsw/choicelists.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-02 17:57:26.703448 lino-welcht-24.3.0/lino_welcht/lib/pcsw/config/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-02 17:57:26.703448 lino-welcht-24.3.0/lino_welcht/lib/pcsw/config/pcsw/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-02 17:57:26.711448 lino-welcht-24.3.0/lino_welcht/lib/pcsw/config/pcsw/Coaching/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      613 2015-09-19 03:53:35.000000 lino-welcht-24.3.0/lino_welcht/lib/pcsw/config/pcsw/Coaching/coaching.body.html
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-02 17:57:26.711448 lino-welcht-24.3.0/lino_welcht/lib/pcsw/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2016-06-08 13:29:44.000000 lino-welcht-24.3.0/lino_welcht/lib/pcsw/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       60 2017-04-22 06:37:57.000000 lino-welcht-24.3.0/lino_welcht/lib/pcsw/fixtures/demo2.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       58 2016-06-08 13:30:04.000000 lino-welcht-24.3.0/lino_welcht/lib/pcsw/fixtures/std.py
--rw-rw-r--   0 luc       (1000) www-data    (33)     7705 2024-02-19 04:56:47.000000 lino-welcht-24.3.0/lino_welcht/lib/pcsw/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-02 17:57:26.703448 lino-welcht-24.3.0/lino_welcht/locale/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-02 17:57:26.703448 lino-welcht-24.3.0/lino_welcht/locale/de/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-02 17:57:26.711448 lino-welcht-24.3.0/lino_welcht/locale/de/LC_MESSAGES/
--rw-rw-rw-   0 luc       (1000) www-data    (33)    39041 2018-12-10 08:06:01.000000 lino-welcht-24.3.0/lino_welcht/locale/de/LC_MESSAGES/django.mo
--rw-rw-rw-   0 luc       (1000) www-data    (33)    74719 2021-02-11 19:06:41.000000 lino-welcht-24.3.0/lino_welcht/locale/de/LC_MESSAGES/django.po
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-02 17:57:26.703448 lino-welcht-24.3.0/lino_welcht/locale/fr/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-02 17:57:26.711448 lino-welcht-24.3.0/lino_welcht/locale/fr/LC_MESSAGES/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     4021 2019-03-29 10:29:37.000000 lino-welcht-24.3.0/lino_welcht/locale/fr/LC_MESSAGES/django.mo
--rw-rw-rw-   0 luc       (1000) www-data    (33)     9514 2021-02-11 19:06:42.000000 lino-welcht-24.3.0/lino_welcht/locale/fr/LC_MESSAGES/django.po
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-02 17:57:26.703448 lino-welcht-24.3.0/lino_welcht/locale/nl/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-02 17:57:26.711448 lino-welcht-24.3.0/lino_welcht/locale/nl/LC_MESSAGES/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      409 2015-09-19 03:53:53.000000 lino-welcht-24.3.0/lino_welcht/locale/nl/LC_MESSAGES/django.mo
--rw-rw-rw-   0 luc       (1000) www-data    (33)    93297 2021-02-11 17:36:49.000000 lino-welcht-24.3.0/lino_welcht/locale/nl/LC_MESSAGES/django.po
--rw-rw-rw-   0 luc       (1000) www-data    (33)     7231 2024-02-14 17:30:47.000000 lino-welcht-24.3.0/lino_welcht/migrate.py
--rw-rw-r--   0 luc       (1000) www-data    (33)     7609 2024-02-20 19:47:11.000000 lino-welcht-24.3.0/lino_welcht/settings.py
--rw-rw-r--   0 luc       (1000) www-data    (33)     4890 2024-03-02 17:57:02.000000 lino-welcht-24.3.0/lino_welcht/setup_info.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      247 2024-02-14 17:30:47.000000 lino-welcht-24.3.0/lino_welcht/workflows.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-02 17:57:26.711448 lino-welcht-24.3.0/lino_welcht.egg-info/
--rw-r--r--   0 luc       (1000) www-data    (33)     1832 2024-03-02 17:57:26.000000 lino-welcht-24.3.0/lino_welcht.egg-info/PKG-INFO
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1703 2024-03-02 17:57:26.000000 lino-welcht-24.3.0/lino_welcht.egg-info/SOURCES.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2024-03-02 17:57:26.000000 lino-welcht-24.3.0/lino_welcht.egg-info/dependency_links.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2019-02-27 20:03:15.000000 lino-welcht-24.3.0/lino_welcht.egg-info/not-zip-safe
--rw-rw-rw-   0 luc       (1000) www-data    (33)       72 2024-03-02 17:57:26.000000 lino-welcht-24.3.0/lino_welcht.egg-info/requires.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)       12 2024-03-02 17:57:26.000000 lino-welcht-24.3.0/lino_welcht.egg-info/top_level.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1052 2021-05-05 05:16:56.000000 lino-welcht-24.3.0/requirements.python3.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)      347 2021-05-05 05:16:56.000000 lino-welcht-24.3.0/requirements.stable.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)      931 2021-05-05 05:16:56.000000 lino-welcht-24.3.0/requirements.txt
--rw-rw-r--   0 luc       (1000) www-data    (33)       38 2024-03-02 17:57:26.711448 lino-welcht-24.3.0/setup.cfg
--rw-rw-rw-   0 luc       (1000) www-data    (33)      163 2024-02-14 17:30:47.000000 lino-welcht-24.3.0/setup.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      374 2024-02-14 17:30:47.000000 lino-welcht-24.3.0/tasks.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-02 17:57:26.711448 lino-welcht-24.3.0/tests/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      551 2024-02-14 17:30:47.000000 lino-welcht-24.3.0/tests/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      162 2024-02-14 17:30:47.000000 lino-welcht-24.3.0/tests/test_docs.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:06:16.145300 lino-welcht-24.5.0/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    34523 2021-04-07 12:55:58.000000 lino-welcht-24.5.0/COPYING
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      105 2023-08-07 14:42:30.000000 lino-welcht-24.5.0/MANIFEST.in
+-rw-r--r--   0 luc       (1000) www-data    (33)     1832 2024-05-01 06:06:16.145300 lino-welcht-24.5.0/PKG-INFO
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      734 2021-08-19 05:39:07.000000 lino-welcht-24.5.0/README.rst
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:06:16.141300 lino-welcht-24.5.0/lino_welcht/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      879 2024-02-14 17:30:47.000000 lino-welcht-24.5.0/lino_welcht/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      223 2024-02-14 17:30:47.000000 lino-welcht-24.5.0/lino_welcht/help_texts.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)     1684 2024-02-14 17:30:47.000000 lino-welcht-24.5.0/lino_welcht/layouts.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:06:16.141300 lino-welcht-24.5.0/lino_welcht/lib/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      257 2024-02-14 17:30:47.000000 lino-welcht-24.5.0/lino_welcht/lib/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:06:16.141300 lino-welcht-24.5.0/lino_welcht/lib/courses/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      545 2024-02-14 17:30:47.000000 lino-welcht-24.5.0/lino_welcht/lib/courses/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:06:16.137300 lino-welcht-24.5.0/lino_welcht/lib/courses/config/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:06:16.137300 lino-welcht-24.5.0/lino_welcht/lib/courses/config/courses/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:06:16.141300 lino-welcht-24.5.0/lino_welcht/lib/courses/config/courses/Enrolment/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1013 2015-09-19 03:53:35.000000 lino-welcht-24.5.0/lino_welcht/lib/courses/config/courses/Enrolment/enrolment.body.html
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1465 2015-09-19 03:53:35.000000 lino-welcht-24.5.0/lino_welcht/lib/courses/config/courses/Enrolment/intervention.body.html
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:06:16.141300 lino-welcht-24.5.0/lino_welcht/lib/courses/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:35.000000 lino-welcht-24.5.0/lino_welcht/lib/courses/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     4828 2024-02-14 17:30:47.000000 lino-welcht-24.5.0/lino_welcht/lib/courses/fixtures/demo.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      914 2024-02-14 17:30:47.000000 lino-welcht-24.5.0/lino_welcht/lib/courses/fixtures/std.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     3906 2024-02-14 17:30:47.000000 lino-welcht-24.5.0/lino_welcht/lib/courses/models.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1355 2024-02-14 17:30:47.000000 lino-welcht-24.5.0/lino_welcht/lib/courses/ui.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:06:16.141300 lino-welcht-24.5.0/lino_welcht/lib/cv/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1133 2024-02-14 17:30:47.000000 lino-welcht-24.5.0/lino_welcht/lib/cv/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:06:16.141300 lino-welcht-24.5.0/lino_welcht/lib/cv/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:36.000000 lino-welcht-24.5.0/lino_welcht/lib/cv/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      655 2024-02-14 17:30:47.000000 lino-welcht-24.5.0/lino_welcht/lib/cv/fixtures/demo.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      823 2023-10-20 06:35:18.000000 lino-welcht-24.5.0/lino_welcht/lib/cv/fixtures/std.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     7691 2024-02-14 17:30:47.000000 lino-welcht-24.5.0/lino_welcht/lib/cv/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:06:16.141300 lino-welcht-24.5.0/lino_welcht/lib/isip/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      288 2024-02-14 17:30:47.000000 lino-welcht-24.5.0/lino_welcht/lib/isip/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2038 2024-02-14 17:30:47.000000 lino-welcht-24.5.0/lino_welcht/lib/isip/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:06:16.141300 lino-welcht-24.5.0/lino_welcht/lib/pcsw/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      471 2024-02-14 17:30:47.000000 lino-welcht-24.5.0/lino_welcht/lib/pcsw/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      456 2024-02-14 17:30:47.000000 lino-welcht-24.5.0/lino_welcht/lib/pcsw/choicelists.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:06:16.137300 lino-welcht-24.5.0/lino_welcht/lib/pcsw/config/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:06:16.137300 lino-welcht-24.5.0/lino_welcht/lib/pcsw/config/pcsw/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:06:16.141300 lino-welcht-24.5.0/lino_welcht/lib/pcsw/config/pcsw/Coaching/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      613 2015-09-19 03:53:35.000000 lino-welcht-24.5.0/lino_welcht/lib/pcsw/config/pcsw/Coaching/coaching.body.html
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:06:16.141300 lino-welcht-24.5.0/lino_welcht/lib/pcsw/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2016-06-08 13:29:44.000000 lino-welcht-24.5.0/lino_welcht/lib/pcsw/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       60 2017-04-22 06:37:57.000000 lino-welcht-24.5.0/lino_welcht/lib/pcsw/fixtures/demo2.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       58 2016-06-08 13:30:04.000000 lino-welcht-24.5.0/lino_welcht/lib/pcsw/fixtures/std.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)     7705 2024-02-19 04:56:47.000000 lino-welcht-24.5.0/lino_welcht/lib/pcsw/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:06:16.137300 lino-welcht-24.5.0/lino_welcht/locale/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:06:16.137300 lino-welcht-24.5.0/lino_welcht/locale/de/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:06:16.141300 lino-welcht-24.5.0/lino_welcht/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1267 2024-04-08 10:16:17.000000 lino-welcht-24.5.0/lino_welcht/locale/de/LC_MESSAGES/django.mo
+-rw-rw-r--   0 luc       (1000) www-data    (33)     7858 2024-04-08 10:16:17.000000 lino-welcht-24.5.0/lino_welcht/locale/de/LC_MESSAGES/django.po
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:06:16.137300 lino-welcht-24.5.0/lino_welcht/locale/fr/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:06:16.141300 lino-welcht-24.5.0/lino_welcht/locale/fr/LC_MESSAGES/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     3978 2024-04-08 10:15:53.000000 lino-welcht-24.5.0/lino_welcht/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 luc       (1000) www-data    (33)     8187 2024-04-08 10:15:53.000000 lino-welcht-24.5.0/lino_welcht/locale/fr/LC_MESSAGES/django.po
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:06:16.137300 lino-welcht-24.5.0/lino_welcht/locale/nl/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:06:16.141300 lino-welcht-24.5.0/lino_welcht/locale/nl/LC_MESSAGES/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      409 2015-09-19 03:53:53.000000 lino-welcht-24.5.0/lino_welcht/locale/nl/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    93297 2021-02-11 17:36:49.000000 lino-welcht-24.5.0/lino_welcht/locale/nl/LC_MESSAGES/django.po
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     7231 2024-02-14 17:30:47.000000 lino-welcht-24.5.0/lino_welcht/migrate.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)     7678 2024-03-29 17:38:37.000000 lino-welcht-24.5.0/lino_welcht/settings.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)     4890 2024-05-01 06:06:07.000000 lino-welcht-24.5.0/lino_welcht/setup_info.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      247 2024-02-14 17:30:47.000000 lino-welcht-24.5.0/lino_welcht/workflows.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:06:16.145300 lino-welcht-24.5.0/lino_welcht.egg-info/
+-rw-r--r--   0 luc       (1000) www-data    (33)     1832 2024-05-01 06:06:16.000000 lino-welcht-24.5.0/lino_welcht.egg-info/PKG-INFO
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1703 2024-05-01 06:06:16.000000 lino-welcht-24.5.0/lino_welcht.egg-info/SOURCES.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2024-05-01 06:06:16.000000 lino-welcht-24.5.0/lino_welcht.egg-info/dependency_links.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2019-02-27 20:03:15.000000 lino-welcht-24.5.0/lino_welcht.egg-info/not-zip-safe
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       72 2024-05-01 06:06:16.000000 lino-welcht-24.5.0/lino_welcht.egg-info/requires.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       12 2024-05-01 06:06:16.000000 lino-welcht-24.5.0/lino_welcht.egg-info/top_level.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1052 2021-05-05 05:16:56.000000 lino-welcht-24.5.0/requirements.python3.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      347 2021-05-05 05:16:56.000000 lino-welcht-24.5.0/requirements.stable.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      931 2021-05-05 05:16:56.000000 lino-welcht-24.5.0/requirements.txt
+-rw-rw-r--   0 luc       (1000) www-data    (33)       38 2024-05-01 06:06:16.145300 lino-welcht-24.5.0/setup.cfg
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      163 2024-02-14 17:30:47.000000 lino-welcht-24.5.0/setup.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      374 2024-02-14 17:30:47.000000 lino-welcht-24.5.0/tasks.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-05-01 06:06:16.141300 lino-welcht-24.5.0/tests/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      551 2024-02-14 17:30:47.000000 lino-welcht-24.5.0/tests/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      162 2024-02-14 17:30:47.000000 lino-welcht-24.5.0/tests/test_docs.py
```

### Comparing `lino-welcht-24.3.0/COPYING` & `lino-welcht-24.5.0/COPYING`

 * *Files identical despite different names*

### Comparing `lino-welcht-24.3.0/PKG-INFO` & `lino-welcht-24.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lino-welcht
-Version: 24.3.0
+Version: 24.5.0
 Summary: A Lino Django application for the PCSW of Châtelet
 Home-page: https://gitlab.com/lino-framework/welcht
 Author: Rumma & Ko Ltd
 Author-email: hamza@lino-framework.org
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `lino-welcht-24.3.0/README.rst` & `lino-welcht-24.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `lino-welcht-24.3.0/lino_welcht/__init__.py` & `lino-welcht-24.5.0/lino_welcht/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welcht-24.3.0/lino_welcht/layouts.py` & `lino-welcht-24.5.0/lino_welcht/layouts.py`

 * *Files identical despite different names*

### Comparing `lino-welcht-24.3.0/lino_welcht/lib/courses/__init__.py` & `lino-welcht-24.5.0/lino_welcht/lib/courses/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welcht-24.3.0/lino_welcht/lib/courses/config/courses/Enrolment/enrolment.body.html` & `lino-welcht-24.5.0/lino_welcht/lib/courses/config/courses/Enrolment/enrolment.body.html`

 * *Files identical despite different names*

### Comparing `lino-welcht-24.3.0/lino_welcht/lib/courses/config/courses/Enrolment/intervention.body.html` & `lino-welcht-24.5.0/lino_welcht/lib/courses/config/courses/Enrolment/intervention.body.html`

 * *Files identical despite different names*

### Comparing `lino-welcht-24.3.0/lino_welcht/lib/courses/fixtures/demo.py` & `lino-welcht-24.5.0/lino_welcht/lib/courses/fixtures/demo.py`

 * *Files identical despite different names*

### Comparing `lino-welcht-24.3.0/lino_welcht/lib/courses/fixtures/std.py` & `lino-welcht-24.5.0/lino_welcht/lib/courses/fixtures/std.py`

 * *Files identical despite different names*

### Comparing `lino-welcht-24.3.0/lino_welcht/lib/courses/models.py` & `lino-welcht-24.5.0/lino_welcht/lib/courses/models.py`

 * *Files identical despite different names*

### Comparing `lino-welcht-24.3.0/lino_welcht/lib/courses/ui.py` & `lino-welcht-24.5.0/lino_welcht/lib/courses/ui.py`

 * *Files identical despite different names*

### Comparing `lino-welcht-24.3.0/lino_welcht/lib/cv/__init__.py` & `lino-welcht-24.5.0/lino_welcht/lib/cv/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welcht-24.3.0/lino_welcht/lib/cv/fixtures/demo.py` & `lino-welcht-24.5.0/lino_welcht/lib/cv/fixtures/demo.py`

 * *Files identical despite different names*

### Comparing `lino-welcht-24.3.0/lino_welcht/lib/cv/fixtures/std.py` & `lino-welcht-24.5.0/lino_welcht/lib/cv/fixtures/std.py`

 * *Files identical despite different names*

### Comparing `lino-welcht-24.3.0/lino_welcht/lib/cv/models.py` & `lino-welcht-24.5.0/lino_welcht/lib/cv/models.py`

 * *Files identical despite different names*

### Comparing `lino-welcht-24.3.0/lino_welcht/lib/isip/models.py` & `lino-welcht-24.5.0/lino_welcht/lib/isip/models.py`

 * *Files identical despite different names*

### Comparing `lino-welcht-24.3.0/lino_welcht/lib/pcsw/config/pcsw/Coaching/coaching.body.html` & `lino-welcht-24.5.0/lino_welcht/lib/pcsw/config/pcsw/Coaching/coaching.body.html`

 * *Files identical despite different names*

### Comparing `lino-welcht-24.3.0/lino_welcht/lib/pcsw/models.py` & `lino-welcht-24.5.0/lino_welcht/lib/pcsw/models.py`

 * *Files identical despite different names*

### Comparing `lino-welcht-24.3.0/lino_welcht/locale/fr/LC_MESSAGES/django.mo` & `lino-welcht-24.5.0/lino_welcht/locale/fr/LC_MESSAGES/django.mo`

 * *Files 17% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,21 +1,21 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: lino.apps.dsbe\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: 2019-03-29 12:29+0200\n"
+"PO-Revision-Date: 2024-04-08 13:15+0300\n"
 "Last-Translator: Luc Saffre <luc.saffre@gmail.com>\n"
-"Language: fr\n"
 "Language-Team: fr <lino-users@gmail.com>\n"
-"Plural-Forms: nplurals=2; plural=n>1;\n"
+"Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.6.0\n"
-"X-Generator: Poedit 2.0.6\n"
+"Plural-Forms: nplurals=2; plural=n>1;\n"
+"Generated-By: Babel 2.12.1\n"
+"X-Generator: Poedit 3.0.1\n"
 
 msgid "Active workshops"
 msgstr "Ateliers actifs"
 
 msgid "Advisor"
 msgstr "Conseiller"
 
@@ -126,17 +126,14 @@
 
 msgid "Kitchen"
 msgstr "Cuisine"
 
 msgid "Learning"
 msgstr "Avertissements"
 
-msgid "Lino Welfare"
-msgstr "Lino pour CPAS"
-
 msgid "Mathematics"
 msgstr "Mathématiques"
 
 msgid "Miscellaneous"
 msgstr "Divers"
 
 msgid "Never came"
```

### Comparing `lino-welcht-24.3.0/lino_welcht/locale/fr/LC_MESSAGES/django.po` & `lino-welcht-24.5.0/lino_welcht/locale/fr/LC_MESSAGES/django.po`

 * *Files 20% similar despite different names*

```diff
@@ -2,123 +2,49 @@
 # Copyright (C) 2016 ORGANIZATION
 # This file is distributed under the same license as the lino-welfare
 # project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2016.
 #
 msgid ""
 msgstr ""
-"Project-Id-Version:  lino.apps.dsbe\n"
+"Project-Id-Version: lino.apps.dsbe\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-02-11 21:06+0200\n"
-"PO-Revision-Date: 2019-03-29 12:29+0200\n"
+"POT-Creation-Date: 2024-04-08 13:15+0300\n"
+"PO-Revision-Date: 2024-04-08 13:15+0300\n"
 "Last-Translator: Luc Saffre <luc.saffre@gmail.com>\n"
-"Language: fr\n"
 "Language-Team: fr <lino-users@gmail.com>\n"
-"Plural-Forms: nplurals=2; plural=n>1\n"
+"Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.9.0\n"
-
-#: lino_welcht/help_texts.py:7
-msgid "Miscellaneous tests on an empty database."
-msgstr ""
-
-#: lino_welcht/help_texts.py:8
-msgid ""
-"Test whether cv.Obstacle.user is correctly set to the requesting\n"
-"user."
-msgstr ""
-
-#: lino_welcht/help_texts.py:10
-msgid ""
-"Since dupable_clients is hidden, we can create duplicate partners\n"
-"without warning."
-msgstr ""
-
-#: lino_welcht/help_texts.py:12
-msgid "Tests a bugfix in suggest_cal_guests."
-msgstr ""
-
-#: lino_welcht/help_texts.py:13
-msgid ""
-"Select only clients who are “learning” during the given date.\n"
-"That is, who have an active Study, Training or\n"
-"Experience.\n"
-"Only the start_date is used, end_date has no effect when\n"
-"this criteria."
-msgstr ""
-
-#: lino_welcht/help_texts.py:18
-msgid ""
-"A proof is some document which certifies that a given person\n"
-"has a given skill."
-msgstr ""
+"Plural-Forms: nplurals=2; plural=n>1;\n"
+"Generated-By: Babel 2.12.1\n"
+"X-Generator: Poedit 3.0.1\n"
 
-#: lino_welcht/help_texts.py:20
-msgid ""
-"Abstract base for Skill, SoftSkill and\n"
-"Obstacle."
-msgstr ""
-
-#: lino_welcht/help_texts.py:22
-msgid ""
-"An obstacle is an observed fact or characteristic of a client\n"
-"which might be reason to not get a given job."
-msgstr ""
-
-#: lino_welcht/help_texts.py:24
-msgid "A pointer to ObstacleType."
-msgstr ""
-
-#: lino_welcht/help_texts.py:25
-msgid "The agent who observed this obstacle."
-msgstr ""
-
-#: lino_welcht/help_texts.py:26
-msgid "The date when the agent observed this obstacle."
+#: lino_welcht/help_texts.py:6
+msgid "See lino.core.plugin.Plugin."
 msgstr ""
 
-#: lino_welcht/layouts.py:27 lino_welcht/layouts.py:33
-#: lino_welcht/layouts.py:38
+#: lino_welcht/layouts.py:35 lino_welcht/layouts.py:42
+#: lino_welcht/layouts.py:48
 msgid "Contact"
 msgstr "Contact"
 
-#: lino_welcht/settings.py:13
-msgid "Lino Welfare"
-msgstr "Lino pour CPAS"
-
-#: lino_welcht/settings.py:175
+#: lino_welcht/settings.py:177
 msgid "Contact details"
 msgstr "Coordonnées"
 
-#: lino_welcht/lib/courses/__init__.py:21 lino_welcht/lib/courses/models.py:63
+#: lino_welcht/lib/courses/__init__.py:20 lino_welcht/lib/courses/models.py:61
 msgid "Workshops"
 msgstr "Ateliers"
 
 #: lino_welcht/lib/courses/__init__.py:23
 msgid "IO"
 msgstr "O.I."
 
-#: lino_welcht/lib/courses/desktop.py:47
-msgid "Active workshops"
-msgstr "Ateliers actifs"
-
-#: lino_welcht/lib/courses/desktop.py:53
-msgid "Draft workshops"
-msgstr "Ateliers en préparation"
-
-#: lino_welcht/lib/courses/desktop.py:58
-msgid "Inactive workshops"
-msgstr "Ateliers inactifs"
-
-#: lino_welcht/lib/courses/desktop.py:62
-msgid "Closed workshops"
-msgstr "Ateliers terminés"
-
 #: lino_welcht/lib/courses/models.py:16
 msgid "Integration workshops"
 msgstr "Ateliers d'insertion sociale"
 
 #: lino_welcht/lib/courses/models.py:17
 msgid "Job search workshops"
 msgstr "Ateliers d'Insertion socioprofessionnelle"
@@ -131,269 +57,285 @@
 msgid "Started"
 msgstr "Commencé"
 
 #: lino_welcht/lib/courses/models.py:35
 msgid "Finished"
 msgstr "Terminé"
 
-#: lino_welcht/lib/courses/fixtures/demo.py:28
-#: lino_welcht/lib/courses/models.py:62
+#: lino_welcht/lib/courses/fixtures/demo.py:24
+#: lino_welcht/lib/courses/models.py:60
 msgid "Workshop"
 msgstr "Atelier"
 
-#: lino_welcht/lib/courses/models.py:77
+#: lino_welcht/lib/courses/models.py:83
 msgid "Motif de l'orientation"
 msgstr ""
 
-#: lino_welcht/lib/courses/models.py:80
+#: lino_welcht/lib/courses/models.py:86
 msgid "Difficultés à l'origine de la demande / Problématiques repérées"
 msgstr ""
 
-#: lino_welcht/lib/courses/models.py:96
+#: lino_welcht/lib/courses/models.py:104
 msgid "Workshop series"
 msgstr "Série d'ateliers"
 
-#: lino_welcht/lib/courses/models.py:97
+#: lino_welcht/lib/courses/models.py:105
 msgid "Workshop lines"
 msgstr "Séries d'ateliers"
 
+#: lino_welcht/lib/courses/ui.py:45
+msgid "Active workshops"
+msgstr "Ateliers actifs"
+
+#: lino_welcht/lib/courses/ui.py:51
+msgid "Draft workshops"
+msgstr "Ateliers en préparation"
+
+#: lino_welcht/lib/courses/ui.py:56
+msgid "Inactive workshops"
+msgstr "Ateliers inactifs"
+
+#: lino_welcht/lib/courses/ui.py:60
+msgid "Closed workshops"
+msgstr "Ateliers terminés"
+
 #: lino_welcht/lib/courses/config/courses/Enrolment/enrolment.body.html:12
 #: lino_welcht/lib/courses/config/courses/Enrolment/intervention.body.html:12
 msgid "Translation"
 msgstr "Traduction"
 
 #: lino_welcht/lib/courses/config/courses/Enrolment/intervention.body.html:24
 msgid "Phone"
 msgstr ""
 
 #: lino_welcht/lib/courses/config/courses/Enrolment/intervention.body.html:25
 msgid "GSM"
 msgstr ""
 
-#: lino_welcht/lib/courses/fixtures/demo.py:41
+#: lino_welcht/lib/courses/fixtures/demo.py:36
 msgid "Introduction to basic kitchen technologies."
 msgstr "Introduction aux techniques de cuisine élémentaires."
 
-#: lino_welcht/lib/courses/fixtures/demo.py:44
+#: lino_welcht/lib/courses/fixtures/demo.py:38
 msgid "Request for enrolment"
 msgstr "Demande d'inscription"
 
-#: lino_welcht/lib/courses/fixtures/demo.py:48
+#: lino_welcht/lib/courses/fixtures/demo.py:42
 msgid "Kitchen"
 msgstr "Cuisine"
 
-#: lino_welcht/lib/courses/fixtures/demo.py:59
+#: lino_welcht/lib/courses/fixtures/demo.py:55
 msgid "Creativity"
 msgstr "Créativité"
 
-#: lino_welcht/lib/courses/fixtures/demo.py:63
+#: lino_welcht/lib/courses/fixtures/demo.py:59
 msgid "Our first baby"
 msgstr "Notre premier bébé"
 
-#: lino_welcht/lib/courses/fixtures/demo.py:67
+#: lino_welcht/lib/courses/fixtures/demo.py:63
 msgid "Mathematics"
 msgstr "Mathématiques"
 
-#: lino_welcht/lib/courses/fixtures/demo.py:71
+#: lino_welcht/lib/courses/fixtures/demo.py:67
 msgid "French"
 msgstr ""
 
-#: lino_welcht/lib/courses/fixtures/demo.py:75
+#: lino_welcht/lib/courses/fixtures/demo.py:71
 msgid "Get active!"
 msgstr "Activons-nous!"
 
-#: lino_welcht/lib/courses/fixtures/demo.py:81
+#: lino_welcht/lib/courses/fixtures/demo.py:76
 msgid "Request for intervention"
 msgstr "Demande d'intervention"
 
-#: lino_welcht/lib/courses/fixtures/demo.py:83
+#: lino_welcht/lib/courses/fixtures/demo.py:78
 msgid "Psycho-social intervention"
 msgstr "Intervention psycho-sociale"
 
-#: lino_welcht/lib/courses/fixtures/std.py:19
+#: lino_welcht/lib/courses/fixtures/std.py:20
 msgid "Enrolment"
 msgstr "Inscription"
 
-#: lino_welcht/lib/cv/models.py:48
+#: lino_welcht/lib/cv/models.py:43
 msgid "Learning"
 msgstr "Avertissements"
 
-#: lino_welcht/lib/cv/models.py:96
+#: lino_welcht/lib/cv/models.py:92
 msgid "Skill proof"
 msgstr "Preuve de qualification"
 
-#: lino_welcht/lib/cv/models.py:97
+#: lino_welcht/lib/cv/models.py:93
 msgid "Skill proofs"
 msgstr "Preuves de qualification"
 
-#: lino_welcht/lib/cv/models.py:117
+#: lino_welcht/lib/cv/models.py:116
 msgid "Remark"
 msgstr "Remarque"
 
 #: lino_welcht/lib/cv/models.py:134
 msgid "Skill"
 msgstr "Compétence professionnelle"
 
 #: lino_welcht/lib/cv/models.py:135
 msgid "Skills"
 msgstr "Compétences professionnelles"
 
-#: lino_welcht/lib/cv/models.py:139 lino_welcht/lib/pcsw/models.py:219
+#: lino_welcht/lib/cv/models.py:140 lino_welcht/lib/pcsw/models.py:228
 msgid "Competences"
 msgstr "Compétences"
 
-#: lino_welcht/lib/cv/models.py:160
+#: lino_welcht/lib/cv/models.py:162
 msgid "Soft skill type"
 msgstr "Type de compétence sociale"
 
-#: lino_welcht/lib/cv/models.py:161
+#: lino_welcht/lib/cv/models.py:163
 msgid "Soft skill types"
 msgstr "Types de compétence sociale"
 
-#: lino_welcht/lib/cv/models.py:172
+#: lino_welcht/lib/cv/models.py:175
 msgid "Soft skill"
 msgstr "Compétence sociale"
 
-#: lino_welcht/lib/cv/models.py:173
+#: lino_welcht/lib/cv/models.py:176
 msgid "Soft skills"
 msgstr "Compétences sociales"
 
-#: lino_welcht/lib/cv/models.py:174 lino_welcht/lib/cv/models.py:225
+#: lino_welcht/lib/cv/models.py:178 lino_welcht/lib/cv/models.py:233
 msgid "Type"
 msgstr ""
 
-#: lino_welcht/lib/cv/models.py:195
+#: lino_welcht/lib/cv/models.py:201
 msgid "Obstacle type"
 msgstr "Type de frein"
 
-#: lino_welcht/lib/cv/models.py:196
+#: lino_welcht/lib/cv/models.py:202
 msgid "Obstacle types"
 msgstr "Types de freins"
 
-#: lino_welcht/lib/cv/models.py:223
+#: lino_welcht/lib/cv/models.py:230
 msgid "Obstacle"
 msgstr "Freins"
 
-#: lino_welcht/lib/cv/models.py:224 lino_welcht/lib/pcsw/models.py:225
+#: lino_welcht/lib/cv/models.py:231 lino_welcht/lib/pcsw/models.py:235
 msgid "Obstacles"
 msgstr "Freins"
 
-#: lino_welcht/lib/cv/models.py:229
+#: lino_welcht/lib/cv/models.py:236
 msgid "Detected by"
 msgstr "Détecté par"
 
-#: lino_welcht/lib/cv/models.py:232
+#: lino_welcht/lib/cv/models.py:239
 msgid "Date"
 msgstr ""
 
-#: lino_welcht/lib/cv/fixtures/std.py:29
+#: lino_welcht/lib/cv/fixtures/std.py:24
 msgid "Declarative"
 msgstr "Déclarative"
 
-#: lino_welcht/lib/cv/fixtures/std.py:30
+#: lino_welcht/lib/cv/fixtures/std.py:25
 msgid "Certificate"
 msgstr "Certificat médical"
 
-#: lino_welcht/lib/cv/fixtures/std.py:31
+#: lino_welcht/lib/cv/fixtures/std.py:26
 msgid "Attestation"
 msgstr "Attestation"
 
-#: lino_welcht/lib/cv/fixtures/std.py:32
+#: lino_welcht/lib/cv/fixtures/std.py:27
 msgid "Diploma"
 msgstr "Diplôme"
 
-#: lino_welcht/lib/cv/fixtures/std.py:34
+#: lino_welcht/lib/cv/fixtures/std.py:29
 msgid "Alcohol"
 msgstr ""
 
-#: lino_welcht/lib/cv/fixtures/std.py:35
+#: lino_welcht/lib/cv/fixtures/std.py:30
 msgid "Health"
 msgstr "Santé"
 
-#: lino_welcht/lib/cv/fixtures/std.py:36
+#: lino_welcht/lib/cv/fixtures/std.py:31
 msgid "Debts"
 msgstr "Dettes"
 
-#: lino_welcht/lib/cv/fixtures/std.py:37
+#: lino_welcht/lib/cv/fixtures/std.py:32
 msgid "Family problems"
 msgstr "Problèmes familiers"
 
-#: lino_welcht/lib/isip/models.py:21 lino_welcht/lib/isip/models.py:48
+#: lino_welcht/lib/isip/models.py:19 lino_welcht/lib/isip/models.py:50
 msgid "General"
 msgstr "Général"
 
-#: lino_welcht/lib/isip/models.py:29 lino_welcht/lib/isip/models.py:56
+#: lino_welcht/lib/isip/models.py:28 lino_welcht/lib/isip/models.py:59
 msgid "Evaluations"
 msgstr "Évaluations"
 
 #: lino_welcht/lib/isip/models.py:34
 msgid "Duties"
 msgstr "Obligations"
 
-#: lino_welcht/lib/pcsw/choicelists.py:16
+#: lino_welcht/lib/pcsw/choicelists.py:15
 msgid "Followed by FORem"
 msgstr "Suivi FORem"
 
-#: lino_welcht/lib/pcsw/choicelists.py:20
+#: lino_welcht/lib/pcsw/choicelists.py:19
 msgid "No"
 msgstr "Non"
 
-#: lino_welcht/lib/pcsw/choicelists.py:21
+#: lino_welcht/lib/pcsw/choicelists.py:20
 msgid "Yes"
 msgstr "Oui"
 
-#: lino_welcht/lib/pcsw/models.py:28
+#: lino_welcht/lib/pcsw/models.py:20
 msgid "Unemployment right"
 msgstr "Droit chômage"
 
-#: lino_welcht/lib/pcsw/models.py:29
+#: lino_welcht/lib/pcsw/models.py:21
 msgid "Unemployment rights"
 msgstr "Droits chômage"
 
-#: lino_welcht/lib/pcsw/models.py:32
+#: lino_welcht/lib/pcsw/models.py:24
 msgid "Designation"
 msgstr "Désignation"
 
-#: lino_welcht/lib/pcsw/models.py:33
+#: lino_welcht/lib/pcsw/models.py:25
 msgid "Reference name"
 msgstr "Nom de référence"
 
-#: lino_welcht/lib/pcsw/models.py:34
+#: lino_welcht/lib/pcsw/models.py:26
 msgid "Considered active"
 msgstr "Considéré actif"
 
-#: lino_welcht/lib/pcsw/models.py:55
+#: lino_welcht/lib/pcsw/models.py:45
 msgid "Advisor"
 msgstr "Conseiller"
 
-#: lino_welcht/lib/pcsw/models.py:91
+#: lino_welcht/lib/pcsw/models.py:84
 msgid "Person"
 msgstr "Personne"
 
-#: lino_welcht/lib/pcsw/models.py:110
+#: lino_welcht/lib/pcsw/models.py:104
 msgid "Family situation"
 msgstr "Situation familiale"
 
-#: lino_welcht/lib/pcsw/models.py:121
+#: lino_welcht/lib/pcsw/models.py:116
 msgid "Coaches"
 msgstr "Intervenants"
 
-#: lino_welcht/lib/pcsw/models.py:156
+#: lino_welcht/lib/pcsw/models.py:157
 msgid "History"
 msgstr "Historique"
 
-#: lino_welcht/lib/pcsw/models.py:176
+#: lino_welcht/lib/pcsw/models.py:178
 msgid "Calendar"
 msgstr "Calendrier"
 
-#: lino_welcht/lib/pcsw/models.py:184
+#: lino_welcht/lib/pcsw/models.py:187
 msgid "Miscellaneous"
 msgstr "Divers"
 
-#: lino_welcht/lib/pcsw/models.py:214
+#: lino_welcht/lib/pcsw/models.py:222
 msgid "Career"
 msgstr "Parcours"
 
 #: lino_welcht/lib/pcsw/config/pcsw/Coaching/coaching.body.html:17
 msgid "Client"
 msgstr "Bénéficiaire"
 
@@ -403,7 +345,9 @@
 
 #~ msgid "Unemployment Situation."
 #~ msgstr "Droit chômage."
 
 #~ msgid "Unemployment situations"
 #~ msgstr "Droits chômage"
 
+#~ msgid "Lino Welfare"
+#~ msgstr "Lino pour CPAS"
```

### Comparing `lino-welcht-24.3.0/lino_welcht/locale/nl/LC_MESSAGES/django.po` & `lino-welcht-24.5.0/lino_welcht/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `lino-welcht-24.3.0/lino_welcht/migrate.py` & `lino-welcht-24.5.0/lino_welcht/migrate.py`

 * *Files identical despite different names*

### Comparing `lino-welcht-24.3.0/lino_welcht/settings.py` & `lino-welcht-24.5.0/lino_welcht/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,17 +37,17 @@
 
     demo_fixtures = """std std2 few_languages all_countries
     demo cbss demo2 demo3 checksummaries checkdata""".split()
 
     migration_class = 'lino_welcht.migrate.Migrator'
     custom_layouts_module = 'lino_welcht.layouts'
 
-    def get_installed_apps(self):
+    def get_installed_plugins(self):
         yield 'lino_welfare.modlib.system'
-        yield super(Site, self).get_installed_apps()
+        yield super(Site, self).get_installed_plugins()
         yield 'lino.modlib.help'
         yield 'lino_xl.lib.statbel.countries'
         yield 'lino_welfare.modlib.contacts'
 
         # yield 'lino.modlib.gfks'
         yield 'lino_xl.lib.appypod'
         yield 'django.contrib.humanize'  # translations for
@@ -70,15 +70,15 @@
 
         # yield 'lino_xl.lib.clients'
         # yield 'lino_xl.lib.coachings'
         yield 'lino_welfare.modlib.welfare'
 
         # NOTE: ordering influences (1) main menu (2) fixtures loading
         # e.g. pcsw.demo creates clients needed by cbss.demo
-        yield 'lino_welfare.modlib.sales'
+        yield 'lino_welfare.modlib.trading'
         # yield 'lino_welfare.modlib.pcsw'
         # yield 'lino_welfare.modlib.ledger'
 
         yield 'lino_welcht.lib.cv'
         yield 'lino_welfare.modlib.integ'
         yield 'lino_welcht.lib.isip'
         yield 'lino_welfare.modlib.jobs'
@@ -164,23 +164,26 @@
         #~ yield self.models.reception.ReceivedVisitors
         # yield self.models.cal.MyOverdueAppointments
 
         if user.is_authenticated:
             yield self.models.notify.MyMessages
 
     def do_site_startup(self):
-        super(Site, self).do_site_startup()
+        super().do_site_startup()
 
         from lino.core.inject import update_field
         # ctt = self.models.clients.ClientContactTypes
         ct = self.models.clients.ClientContact
         ct.column_names = "company contact_person remark"
         update_field(ct, 'remark', verbose_name=_("Contact details"))
 
-        from lino.utils.watch import watch_changes as wc
+    def setup_actions(self):
+        super().setup_actions()
+
+        from lino.modlib.changes.utils import watch_changes as wc
 
         wc(self.models.contacts.Partner)
         wc(self.models.contacts.Person, master_key='partner_ptr')
         wc(self.models.contacts.Company, master_key='partner_ptr')
         wc(self.models.pcsw.Client, master_key='partner_ptr')
 
         wc(self.models.coachings.Coaching, master_key='client__partner_ptr')
```

### Comparing `lino-welcht-24.3.0/lino_welcht/setup_info.py` & `lino-welcht-24.5.0/lino_welcht/setup_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 else:
     requires.append('channels')
     requires.append('suds-py3')
     # requires.append('suds-jurko')
 
 SETUP_INFO = dict(
     name='lino-welcht',
-    version='24.3.0',
+    version='24.5.0',
     install_requires=requires,
     test_suite='tests',
     tests_require=['pytest'],
     include_package_data=True,
     zip_safe=False,
     description="A Lino Django application for the PCSW of Châtelet",
     long_description=u"""\
```

### Comparing `lino-welcht-24.3.0/lino_welcht.egg-info/PKG-INFO` & `lino-welcht-24.5.0/lino_welcht.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lino-welcht
-Version: 24.3.0
+Version: 24.5.0
 Summary: A Lino Django application for the PCSW of Châtelet
 Home-page: https://gitlab.com/lino-framework/welcht
 Author: Rumma & Ko Ltd
 Author-email: hamza@lino-framework.org
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `lino-welcht-24.3.0/lino_welcht.egg-info/SOURCES.txt` & `lino-welcht-24.5.0/lino_welcht.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lino-welcht-24.3.0/requirements.python3.txt` & `lino-welcht-24.5.0/requirements.python3.txt`

 * *Files identical despite different names*

### Comparing `lino-welcht-24.3.0/requirements.txt` & `lino-welcht-24.5.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `lino-welcht-24.3.0/tests/__init__.py` & `lino-welcht-24.5.0/tests/__init__.py`

 * *Files identical despite different names*

