# Comparing `tmp/pyslth-0.2.4.tar.gz` & `tmp/pyslth-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyslth-0.2.4.tar", last modified: Wed May  1 15:42:18 2024, max compression
+gzip compressed data, was "pyslth-0.2.5.tar", last modified: Wed May  1 17:49:31 2024, max compression
```

## Comparing `pyslth-0.2.4.tar` & `pyslth-0.2.5.tar`

### file list

```diff
@@ -1,80 +1,81 @@
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-01 15:42:18.844153 pyslth-0.2.4/
--rw-r--r--   0 breno      (501) staff       (20)       96 2024-04-27 20:11:05.000000 pyslth-0.2.4/MANIFEST.in
--rw-r--r--   0 breno      (501) staff       (20)      590 2024-05-01 15:42:18.843930 pyslth-0.2.4/PKG-INFO
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-01 15:42:18.814843 pyslth-0.2.4/pyslth.egg-info/
--rw-r--r--   0 breno      (501) staff       (20)      590 2024-05-01 15:42:18.000000 pyslth-0.2.4/pyslth.egg-info/PKG-INFO
--rw-r--r--   0 breno      (501) staff       (20)     1757 2024-05-01 15:42:18.000000 pyslth-0.2.4/pyslth.egg-info/SOURCES.txt
--rw-r--r--   0 breno      (501) staff       (20)        1 2024-05-01 15:42:18.000000 pyslth-0.2.4/pyslth.egg-info/dependency_links.txt
--rw-r--r--   0 breno      (501) staff       (20)      163 2024-05-01 15:42:18.000000 pyslth-0.2.4/pyslth.egg-info/requires.txt
--rw-r--r--   0 breno      (501) staff       (20)        5 2024-05-01 15:42:18.000000 pyslth-0.2.4/pyslth.egg-info/top_level.txt
--rw-r--r--   0 breno      (501) staff       (20)      155 2024-04-27 19:55:48.000000 pyslth-0.2.4/requirements.txt
--rw-r--r--   0 breno      (501) staff       (20)       38 2024-05-01 15:42:18.844218 pyslth-0.2.4/setup.cfg
--rw-r--r--   0 breno      (501) staff       (20)      929 2024-05-01 15:41:16.000000 pyslth-0.2.4/setup.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-01 15:42:18.822825 pyslth-0.2.4/slth/
--rw-r--r--   0 breno      (501) staff       (20)     3774 2024-04-28 09:42:58.000000 pyslth-0.2.4/slth/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     6945 2024-04-30 16:46:55.000000 pyslth-0.2.4/slth/components.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-01 15:42:18.823395 pyslth-0.2.4/slth/db/
--rw-r--r--   0 breno      (501) staff       (20)       46 2024-04-21 03:07:00.000000 pyslth-0.2.4/slth/db/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     4817 2024-04-23 11:29:24.000000 pyslth-0.2.4/slth/db/models.py
--rw-r--r--   0 breno      (501) staff       (20)    20556 2024-05-01 15:37:13.000000 pyslth-0.2.4/slth/endpoints.py
--rw-r--r--   0 breno      (501) staff       (20)      156 2024-04-09 12:56:09.000000 pyslth-0.2.4/slth/exceptions.py
--rw-r--r--   0 breno      (501) staff       (20)     2527 2024-05-01 13:30:46.000000 pyslth-0.2.4/slth/factory.py
--rw-r--r--   0 breno      (501) staff       (20)    25521 2024-05-01 15:36:17.000000 pyslth-0.2.4/slth/forms.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-01 15:42:18.823710 pyslth-0.2.4/slth/management/
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.2.4/slth/management/__init__.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-01 15:42:18.824349 pyslth-0.2.4/slth/management/commands/
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.2.4/slth/management/commands/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     1599 2024-04-13 14:42:59.000000 pyslth-0.2.4/slth/management/commands/integration_test.py
--rw-r--r--   0 breno      (501) staff       (20)     1276 2024-04-09 17:55:35.000000 pyslth-0.2.4/slth/management/commands/sync.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-01 15:42:18.826785 pyslth-0.2.4/slth/migrations/
--rw-r--r--   0 breno      (501) staff       (20)     1392 2024-05-01 14:04:01.000000 pyslth-0.2.4/slth/migrations/0001_initial.py
--rw-r--r--   0 breno      (501) staff       (20)     3513 2024-04-19 09:33:48.000000 pyslth-0.2.4/slth/migrations/0002_email_role_pushsubscription_error.py
--rw-r--r--   0 breno      (501) staff       (20)      601 2024-05-01 14:04:01.000000 pyslth-0.2.4/slth/migrations/0003_rename_photo_profile_alter_profile_options.py
--rw-r--r--   0 breno      (501) staff       (20)      451 2024-05-01 14:04:01.000000 pyslth-0.2.4/slth/migrations/0004_alter_profile_photo.py
--rw-r--r--   0 breno      (501) staff       (20)      450 2024-05-01 14:04:01.000000 pyslth-0.2.4/slth/migrations/0005_alter_profile_photo.py
--rw-r--r--   0 breno      (501) staff       (20)      854 2024-04-28 09:44:45.000000 pyslth-0.2.4/slth/migrations/0006_user.py
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.2.4/slth/migrations/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     6441 2024-05-01 14:04:01.000000 pyslth-0.2.4/slth/models.py
--rw-r--r--   0 breno      (501) staff       (20)      394 2024-04-13 09:58:46.000000 pyslth-0.2.4/slth/notifications.py
--rw-r--r--   0 breno      (501) staff       (20)     1906 2024-04-09 12:56:09.000000 pyslth-0.2.4/slth/permissions.py
--rw-r--r--   0 breno      (501) staff       (20)    19351 2024-05-01 11:31:08.000000 pyslth-0.2.4/slth/queryset.py
--rw-r--r--   0 breno      (501) staff       (20)     4724 2024-04-19 09:29:01.000000 pyslth-0.2.4/slth/roles.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-01 15:42:18.827275 pyslth-0.2.4/slth/selenium/
--rw-r--r--   0 breno      (501) staff       (20)     9095 2024-04-28 09:44:40.000000 pyslth-0.2.4/slth/selenium/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)    11350 2024-04-30 08:48:10.000000 pyslth-0.2.4/slth/selenium/browser.py
--rw-r--r--   0 breno      (501) staff       (20)    14408 2024-05-01 13:49:16.000000 pyslth-0.2.4/slth/serializer.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-01 15:42:18.827599 pyslth-0.2.4/slth/static/
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-01 15:42:18.829217 pyslth-0.2.4/slth/static/css/
--rw-r--r--   0 breno      (501) staff       (20)     6148 2024-04-29 19:56:09.000000 pyslth-0.2.4/slth/static/css/.DS_Store
--rw-r--r--   0 breno      (501) staff       (20)    80823 2024-04-27 15:01:32.000000 pyslth-0.2.4/slth/static/css/fontawesome.min.css
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-01 15:42:18.833640 pyslth-0.2.4/slth/static/css/fonts/
--rw-r--r--   0 breno      (501) staff       (20)     6148 2024-04-29 19:36:17.000000 pyslth-0.2.4/slth/static/css/fonts/.DS_Store
--rw-r--r--   0 breno      (501) staff       (20)   150020 2024-04-27 15:01:32.000000 pyslth-0.2.4/slth/static/css/fonts/fa-solid-900.woff2
--rw-r--r--   0 breno      (501) staff       (20)   115080 2024-04-29 19:28:27.000000 pyslth-0.2.4/slth/static/css/fonts/rawline-400.woff
--rw-r--r--   0 breno      (501) staff       (20)   117252 2024-04-29 19:29:24.000000 pyslth-0.2.4/slth/static/css/fonts/rawline-500i.woff
--rw-r--r--   0 breno      (501) staff       (20)   117076 2024-04-29 19:36:27.000000 pyslth-0.2.4/slth/static/css/fonts/rawline-700.woff
--rw-r--r--   0 breno      (501) staff       (20)      752 2024-05-01 13:59:41.000000 pyslth-0.2.4/slth/static/css/slth.css
--rw-r--r--   0 breno      (501) staff       (20)      515 2024-04-27 15:44:29.000000 pyslth-0.2.4/slth/static/css/solid.min.css
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-01 15:42:18.835160 pyslth-0.2.4/slth/static/images/
--rw-r--r--   0 breno      (501) staff       (20)    10828 2024-04-15 11:56:33.000000 pyslth-0.2.4/slth/static/images/logo.png
--rw-r--r--   0 breno      (501) staff       (20)     2432 2024-04-13 03:35:59.000000 pyslth-0.2.4/slth/static/images/logo.svg
--rw-r--r--   0 breno      (501) staff       (20)    16754 2024-04-16 09:42:03.000000 pyslth-0.2.4/slth/static/images/user.png
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-27 17:47:02.000000 pyslth-0.2.4/slth/static/index.html
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-01 15:42:18.842963 pyslth-0.2.4/slth/static/js/
--rw-r--r--   0 breno      (501) staff       (20)  1112414 2024-04-27 15:01:32.000000 pyslth-0.2.4/slth/static/js/echarts.min.js
--rw-r--r--   0 breno      (501) staff       (20)      755 2024-05-01 15:42:03.000000 pyslth-0.2.4/slth/static/js/index.min.js
--rw-r--r--   0 breno      (501) staff       (20)    82972 2024-05-01 15:42:03.000000 pyslth-0.2.4/slth/static/js/lib.min.js
--rw-r--r--   0 breno      (501) staff       (20)   117723 2024-04-27 15:01:32.000000 pyslth-0.2.4/slth/static/js/peerjs.min.js
--rw-r--r--   0 breno      (501) staff       (20)    19927 2024-04-27 15:01:32.000000 pyslth-0.2.4/slth/static/js/qrcode.min.js
--rw-r--r--   0 breno      (501) staff       (20)     6176 2024-04-27 15:01:32.000000 pyslth-0.2.4/slth/static/js/react-trigger-change.js
--rw-r--r--   0 breno      (501) staff       (20)   141870 2024-05-01 15:42:03.000000 pyslth-0.2.4/slth/static/js/react.min.js
--rw-rw-r--   0 breno      (501) staff       (20)     7401 2024-04-27 15:01:32.000000 pyslth-0.2.4/slth/static/js/vanilla-masker.js
--rw-r--r--   0 breno      (501) staff       (20)     5720 2024-04-27 15:01:32.000000 pyslth-0.2.4/slth/static/js/vanilla-masker.min.js
--rw-r--r--   0 breno      (501) staff       (20)     6319 2024-04-09 12:56:09.000000 pyslth-0.2.4/slth/statistics.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-01 15:42:18.843583 pyslth-0.2.4/slth/templates/
--rw-r--r--   0 breno      (501) staff       (20)     2281 2024-05-01 12:46:57.000000 pyslth-0.2.4/slth/templates/index.html
--rw-r--r--   0 breno      (501) staff       (20)      660 2024-04-27 15:01:32.000000 pyslth-0.2.4/slth/templates/service-worker.js
--rw-r--r--   0 breno      (501) staff       (20)     5528 2024-04-16 18:07:11.000000 pyslth-0.2.4/slth/tests.py
--rw-r--r--   0 breno      (501) staff       (20)      797 2024-04-29 14:21:39.000000 pyslth-0.2.4/slth/urls.py
--rw-r--r--   0 breno      (501) staff       (20)     1000 2024-04-27 19:14:01.000000 pyslth-0.2.4/slth/utils.py
--rw-r--r--   0 breno      (501) staff       (20)     2425 2024-05-01 13:07:02.000000 pyslth-0.2.4/slth/views.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-01 17:49:31.895048 pyslth-0.2.5/
+-rw-r--r--   0 breno      (501) staff       (20)       96 2024-04-27 20:11:05.000000 pyslth-0.2.5/MANIFEST.in
+-rw-r--r--   0 breno      (501) staff       (20)      590 2024-05-01 17:49:31.894636 pyslth-0.2.5/PKG-INFO
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-01 17:49:31.850502 pyslth-0.2.5/pyslth.egg-info/
+-rw-r--r--   0 breno      (501) staff       (20)      590 2024-05-01 17:49:31.000000 pyslth-0.2.5/pyslth.egg-info/PKG-INFO
+-rw-r--r--   0 breno      (501) staff       (20)     1784 2024-05-01 17:49:31.000000 pyslth-0.2.5/pyslth.egg-info/SOURCES.txt
+-rw-r--r--   0 breno      (501) staff       (20)        1 2024-05-01 17:49:31.000000 pyslth-0.2.5/pyslth.egg-info/dependency_links.txt
+-rw-r--r--   0 breno      (501) staff       (20)      163 2024-05-01 17:49:31.000000 pyslth-0.2.5/pyslth.egg-info/requires.txt
+-rw-r--r--   0 breno      (501) staff       (20)        5 2024-05-01 17:49:31.000000 pyslth-0.2.5/pyslth.egg-info/top_level.txt
+-rw-r--r--   0 breno      (501) staff       (20)      155 2024-04-27 19:55:48.000000 pyslth-0.2.5/requirements.txt
+-rw-r--r--   0 breno      (501) staff       (20)       38 2024-05-01 17:49:31.895332 pyslth-0.2.5/setup.cfg
+-rw-r--r--   0 breno      (501) staff       (20)      929 2024-05-01 17:47:12.000000 pyslth-0.2.5/setup.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-01 17:49:31.856976 pyslth-0.2.5/slth/
+-rw-r--r--   0 breno      (501) staff       (20)     3774 2024-04-28 09:42:58.000000 pyslth-0.2.5/slth/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     6945 2024-04-30 16:46:55.000000 pyslth-0.2.5/slth/components.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-01 17:49:31.857639 pyslth-0.2.5/slth/db/
+-rw-r--r--   0 breno      (501) staff       (20)       46 2024-04-21 03:07:00.000000 pyslth-0.2.5/slth/db/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     4817 2024-04-23 11:29:24.000000 pyslth-0.2.5/slth/db/models.py
+-rw-r--r--   0 breno      (501) staff       (20)    20556 2024-05-01 15:37:13.000000 pyslth-0.2.5/slth/endpoints.py
+-rw-r--r--   0 breno      (501) staff       (20)      156 2024-04-09 12:56:09.000000 pyslth-0.2.5/slth/exceptions.py
+-rw-r--r--   0 breno      (501) staff       (20)     2527 2024-05-01 13:30:46.000000 pyslth-0.2.5/slth/factory.py
+-rw-r--r--   0 breno      (501) staff       (20)    25521 2024-05-01 15:36:17.000000 pyslth-0.2.5/slth/forms.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-01 17:49:31.857976 pyslth-0.2.5/slth/management/
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.2.5/slth/management/__init__.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-01 17:49:31.858643 pyslth-0.2.5/slth/management/commands/
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.2.5/slth/management/commands/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     1599 2024-04-13 14:42:59.000000 pyslth-0.2.5/slth/management/commands/integration_test.py
+-rw-r--r--   0 breno      (501) staff       (20)     1276 2024-04-09 17:55:35.000000 pyslth-0.2.5/slth/management/commands/sync.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-01 17:49:31.862043 pyslth-0.2.5/slth/migrations/
+-rw-r--r--   0 breno      (501) staff       (20)     1392 2024-05-01 14:04:01.000000 pyslth-0.2.5/slth/migrations/0001_initial.py
+-rw-r--r--   0 breno      (501) staff       (20)     3513 2024-04-19 09:33:48.000000 pyslth-0.2.5/slth/migrations/0002_email_role_pushsubscription_error.py
+-rw-r--r--   0 breno      (501) staff       (20)      601 2024-05-01 14:04:01.000000 pyslth-0.2.5/slth/migrations/0003_rename_photo_profile_alter_profile_options.py
+-rw-r--r--   0 breno      (501) staff       (20)      451 2024-05-01 14:04:01.000000 pyslth-0.2.5/slth/migrations/0004_alter_profile_photo.py
+-rw-r--r--   0 breno      (501) staff       (20)      450 2024-05-01 14:04:01.000000 pyslth-0.2.5/slth/migrations/0005_alter_profile_photo.py
+-rw-r--r--   0 breno      (501) staff       (20)      854 2024-04-28 09:44:45.000000 pyslth-0.2.5/slth/migrations/0006_user.py
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.2.5/slth/migrations/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     6441 2024-05-01 14:04:01.000000 pyslth-0.2.5/slth/models.py
+-rw-r--r--   0 breno      (501) staff       (20)      394 2024-04-13 09:58:46.000000 pyslth-0.2.5/slth/notifications.py
+-rw-r--r--   0 breno      (501) staff       (20)     1906 2024-04-09 12:56:09.000000 pyslth-0.2.5/slth/permissions.py
+-rw-r--r--   0 breno      (501) staff       (20)    19351 2024-05-01 11:31:08.000000 pyslth-0.2.5/slth/queryset.py
+-rw-r--r--   0 breno      (501) staff       (20)     4724 2024-04-19 09:29:01.000000 pyslth-0.2.5/slth/roles.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-01 17:49:31.862807 pyslth-0.2.5/slth/selenium/
+-rw-r--r--   0 breno      (501) staff       (20)     9095 2024-04-28 09:44:40.000000 pyslth-0.2.5/slth/selenium/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)    11350 2024-04-30 08:48:10.000000 pyslth-0.2.5/slth/selenium/browser.py
+-rw-r--r--   0 breno      (501) staff       (20)    14408 2024-05-01 13:49:16.000000 pyslth-0.2.5/slth/serializer.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-01 17:49:31.863366 pyslth-0.2.5/slth/static/
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-01 17:49:31.866807 pyslth-0.2.5/slth/static/css/
+-rw-r--r--   0 breno      (501) staff       (20)     6148 2024-04-29 19:56:09.000000 pyslth-0.2.5/slth/static/css/.DS_Store
+-rw-r--r--   0 breno      (501) staff       (20)    80823 2024-04-27 15:01:32.000000 pyslth-0.2.5/slth/static/css/fontawesome.min.css
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-01 17:49:31.872744 pyslth-0.2.5/slth/static/css/fonts/
+-rw-r--r--   0 breno      (501) staff       (20)     6148 2024-04-29 19:36:17.000000 pyslth-0.2.5/slth/static/css/fonts/.DS_Store
+-rw-r--r--   0 breno      (501) staff       (20)   150020 2024-04-27 15:01:32.000000 pyslth-0.2.5/slth/static/css/fonts/fa-solid-900.woff2
+-rw-r--r--   0 breno      (501) staff       (20)   115080 2024-04-29 19:28:27.000000 pyslth-0.2.5/slth/static/css/fonts/rawline-400.woff
+-rw-r--r--   0 breno      (501) staff       (20)   117252 2024-04-29 19:29:24.000000 pyslth-0.2.5/slth/static/css/fonts/rawline-500i.woff
+-rw-r--r--   0 breno      (501) staff       (20)   117076 2024-04-29 19:36:27.000000 pyslth-0.2.5/slth/static/css/fonts/rawline-700.woff
+-rw-r--r--   0 breno      (501) staff       (20)      752 2024-05-01 13:59:41.000000 pyslth-0.2.5/slth/static/css/slth.css
+-rw-r--r--   0 breno      (501) staff       (20)      515 2024-04-27 15:44:29.000000 pyslth-0.2.5/slth/static/css/solid.min.css
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-01 17:49:31.874314 pyslth-0.2.5/slth/static/images/
+-rw-r--r--   0 breno      (501) staff       (20)    10828 2024-04-15 11:56:33.000000 pyslth-0.2.5/slth/static/images/logo.png
+-rw-r--r--   0 breno      (501) staff       (20)     2432 2024-04-13 03:35:59.000000 pyslth-0.2.5/slth/static/images/logo.svg
+-rw-r--r--   0 breno      (501) staff       (20)    16754 2024-04-16 09:42:03.000000 pyslth-0.2.5/slth/static/images/user.png
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-27 17:47:02.000000 pyslth-0.2.5/slth/static/index.html
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-01 17:49:31.892283 pyslth-0.2.5/slth/static/js/
+-rw-r--r--   0 breno      (501) staff       (20)  1112414 2024-04-27 15:01:32.000000 pyslth-0.2.5/slth/static/js/echarts.min.js
+-rw-r--r--   0 breno      (501) staff       (20)      756 2024-05-01 17:47:42.000000 pyslth-0.2.5/slth/static/js/index.min.js
+-rw-r--r--   0 breno      (501) staff       (20)    83233 2024-05-01 17:36:19.000000 pyslth-0.2.5/slth/static/js/lib.min.js
+-rw-r--r--   0 breno      (501) staff       (20)   117723 2024-04-27 15:01:32.000000 pyslth-0.2.5/slth/static/js/peerjs.min.js
+-rw-r--r--   0 breno      (501) staff       (20)    19927 2024-04-27 15:01:32.000000 pyslth-0.2.5/slth/static/js/qrcode.min.js
+-rw-r--r--   0 breno      (501) staff       (20)     6176 2024-04-27 15:01:32.000000 pyslth-0.2.5/slth/static/js/react-trigger-change.js
+-rw-r--r--   0 breno      (501) staff       (20)   141870 2024-05-01 17:47:42.000000 pyslth-0.2.5/slth/static/js/react.min.js
+-rw-r--r--   0 breno      (501) staff       (20)    83233 2024-05-01 17:47:42.000000 pyslth-0.2.5/slth/static/js/slth.min.js
+-rw-rw-r--   0 breno      (501) staff       (20)     7401 2024-04-27 15:01:32.000000 pyslth-0.2.5/slth/static/js/vanilla-masker.js
+-rw-r--r--   0 breno      (501) staff       (20)     5720 2024-04-27 15:01:32.000000 pyslth-0.2.5/slth/static/js/vanilla-masker.min.js
+-rw-r--r--   0 breno      (501) staff       (20)     6319 2024-04-09 12:56:09.000000 pyslth-0.2.5/slth/statistics.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-01 17:49:31.893416 pyslth-0.2.5/slth/templates/
+-rw-r--r--   0 breno      (501) staff       (20)     2282 2024-05-01 17:36:48.000000 pyslth-0.2.5/slth/templates/index.html
+-rw-r--r--   0 breno      (501) staff       (20)      660 2024-04-27 15:01:32.000000 pyslth-0.2.5/slth/templates/service-worker.js
+-rw-r--r--   0 breno      (501) staff       (20)     5528 2024-04-16 18:07:11.000000 pyslth-0.2.5/slth/tests.py
+-rw-r--r--   0 breno      (501) staff       (20)      797 2024-04-29 14:21:39.000000 pyslth-0.2.5/slth/urls.py
+-rw-r--r--   0 breno      (501) staff       (20)     1000 2024-04-27 19:14:01.000000 pyslth-0.2.5/slth/utils.py
+-rw-r--r--   0 breno      (501) staff       (20)     2425 2024-05-01 13:07:02.000000 pyslth-0.2.5/slth/views.py
```

### Comparing `pyslth-0.2.4/PKG-INFO` & `pyslth-0.2.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyslth
-Version: 0.2.4
+Version: 0.2.5
 Summary: API generator based on yml file
 Home-page: https://github.com/brenokcc
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `pyslth-0.2.4/pyslth.egg-info/PKG-INFO` & `pyslth-0.2.5/pyslth.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyslth
-Version: 0.2.4
+Version: 0.2.5
 Summary: API generator based on yml file
 Home-page: https://github.com/brenokcc
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `pyslth-0.2.4/pyslth.egg-info/SOURCES.txt` & `pyslth-0.2.5/pyslth.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -54,11 +54,12 @@
 slth/static/js/echarts.min.js
 slth/static/js/index.min.js
 slth/static/js/lib.min.js
 slth/static/js/peerjs.min.js
 slth/static/js/qrcode.min.js
 slth/static/js/react-trigger-change.js
 slth/static/js/react.min.js
+slth/static/js/slth.min.js
 slth/static/js/vanilla-masker.js
 slth/static/js/vanilla-masker.min.js
 slth/templates/index.html
 slth/templates/service-worker.js
```

### Comparing `pyslth-0.2.4/setup.py` & `pyslth-0.2.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from setuptools import find_packages, setup
 
 install_requires = open('requirements.txt').read().splitlines()
 
 setup(
     name='pyslth',
-    version='0.2.4',
+    version='0.2.5',
     packages=find_packages(exclude=('xxx', 'xxx.*')),
     install_requires=install_requires,
     extras_require={
         'dev': []
     },
     include_package_data=True,
     license='BSD License',
```

### Comparing `pyslth-0.2.4/slth/__init__.py` & `pyslth-0.2.5/slth/__init__.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.4/slth/components.py` & `pyslth-0.2.5/slth/components.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.4/slth/db/models.py` & `pyslth-0.2.5/slth/db/models.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.4/slth/endpoints.py` & `pyslth-0.2.5/slth/endpoints.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.4/slth/factory.py` & `pyslth-0.2.5/slth/factory.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.4/slth/forms.py` & `pyslth-0.2.5/slth/forms.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.4/slth/management/commands/integration_test.py` & `pyslth-0.2.5/slth/management/commands/integration_test.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.4/slth/management/commands/sync.py` & `pyslth-0.2.5/slth/management/commands/sync.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.4/slth/migrations/0001_initial.py` & `pyslth-0.2.5/slth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.4/slth/migrations/0002_email_role_pushsubscription_error.py` & `pyslth-0.2.5/slth/migrations/0002_email_role_pushsubscription_error.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.4/slth/migrations/0003_rename_photo_profile_alter_profile_options.py` & `pyslth-0.2.5/slth/migrations/0003_rename_photo_profile_alter_profile_options.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.4/slth/migrations/0006_user.py` & `pyslth-0.2.5/slth/migrations/0006_user.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.4/slth/models.py` & `pyslth-0.2.5/slth/models.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.4/slth/permissions.py` & `pyslth-0.2.5/slth/permissions.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.4/slth/queryset.py` & `pyslth-0.2.5/slth/queryset.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.4/slth/roles.py` & `pyslth-0.2.5/slth/roles.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.4/slth/selenium/__init__.py` & `pyslth-0.2.5/slth/selenium/__init__.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.4/slth/selenium/browser.py` & `pyslth-0.2.5/slth/selenium/browser.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.4/slth/serializer.py` & `pyslth-0.2.5/slth/serializer.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.4/slth/static/css/.DS_Store` & `pyslth-0.2.5/slth/static/css/.DS_Store`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.4/slth/static/css/fontawesome.min.css` & `pyslth-0.2.5/slth/static/css/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.4/slth/static/css/fonts/.DS_Store` & `pyslth-0.2.5/slth/static/css/fonts/.DS_Store`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.4/slth/static/css/fonts/fa-solid-900.woff2` & `pyslth-0.2.5/slth/static/css/fonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.4/slth/static/css/fonts/rawline-400.woff` & `pyslth-0.2.5/slth/static/css/fonts/rawline-400.woff`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.4/slth/static/css/fonts/rawline-500i.woff` & `pyslth-0.2.5/slth/static/css/fonts/rawline-500i.woff`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.4/slth/static/css/fonts/rawline-700.woff` & `pyslth-0.2.5/slth/static/css/fonts/rawline-700.woff`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.4/slth/static/css/slth.css` & `pyslth-0.2.5/slth/static/css/slth.css`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.4/slth/static/css/solid.min.css` & `pyslth-0.2.5/slth/static/css/solid.min.css`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.4/slth/static/images/logo.png` & `pyslth-0.2.5/slth/static/images/logo.png`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.4/slth/static/images/logo.svg` & `pyslth-0.2.5/slth/static/images/logo.svg`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.4/slth/static/images/user.png` & `pyslth-0.2.5/slth/static/images/user.png`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.4/slth/static/js/echarts.min.js` & `pyslth-0.2.5/slth/static/js/echarts.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.4/slth/static/js/index.min.js` & `pyslth-0.2.5/slth/static/js/index.min.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-import "./lib.min.js";
+import "./slth.min.js";
 import "./react.min.js";
 (function() {
     const t = document.createElement("link").relList;
     if (t && t.supports && t.supports("modulepreload")) return;
     for (const e of document.querySelectorAll('link[rel="modulepreload"]')) i(e);
     new MutationObserver(e => {
         for (const r of e)
```

### Comparing `pyslth-0.2.4/slth/static/js/lib.min.js` & `pyslth-0.2.5/slth/static/js/lib.min.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,43 +1,43 @@
 import {
     j as t,
-    c as P,
+    c as W,
     r as C,
-    R as De
+    R as Ie
 } from "./react.min.js";
 
-function Ie(e) {
+function De(e) {
     function n(r) {
         navigator.clipboard.writeText(r), ee('Icon "' + r + '" copied to clipboard!')
     }
     const a = {
         display: "inline-block",
         width: 150,
         textAlign: "center",
         cursor: "pointer"
     };
     return t.jsx("div", {
         style: {
             marginTop: 30
         },
-        children: Be.map(r => t.jsxs("div", {
+        children: qe.map(r => t.jsxs("div", {
             className: "icon-box",
             onClick: () => n(r),
             style: a,
             children: [t.jsx("i", {
                 className: "fa-solid fa-fw fa-" + r
             }), t.jsx("div", {
                 className: "icon-text",
                 children: r
             })]
         }, Math.random()))
     })
 }
 
-function qe(e) {
+function Be(e) {
     function n() {
         return t.jsx("i", {
             style: e.style,
             className: "fa-solid fa-circle-notch fa-spin fa-1x spin"
         })
     }
     return n()
@@ -72,15 +72,15 @@
             children: t.jsx(b, {
                 icon: e.icon
             })
         })
     }
     return n()
 }
-const Be = ["1", "2", "3", "4", "5", "6", "7", "8", "9", "fill-drip", "arrows-to-circle", "circle-chevron-right", "at", "trash-can", "text-height", "user-xmark", "stethoscope", "message", "info", "down-left-and-up-right-to-center", "explosion", "file-text", "wave-square", "ring", "building-un", "dice-three", "calendar-days", "anchor-circle-check", "building-circle-arrow-right", "volleyball", "arrows-up-to-line", "sort-down", "minus-circle", "door-open", "sign-out-alt", "atom", "soap", "icons", "microphone-lines-slash", "bridge-circle-check", "pump-medical", "fingerprint", "hand-point-right", "search-location", "step-forward", "smile-beam", "flag-checkered", "football", "school-circle-exclamation", "crop", "angles-down", "users-rectangle", "people-roof", "people-line", "beer", "diagram-predecessor", "long-arrow-up", "fire-flame-simple", "person", "laptop", "file-csv", "menorah", "truck-plane", "record-vinyl", "grin-stars", "bong", "spaghetti-monster-flying", "arrow-down-up-across-line", "utensil-spoon", "jar-wheat", "mail-bulk", "file-circle-exclamation", "hospital-symbol", "pager", "contact-book", "strikethrough", "k", "landmark-flag", "pencil", "backward", "caret-right", "comments", "paste", "code-pull-request", "clipboard-list", "truck-ramp-box", "user-check", "vial-virus", "sheet-plastic", "blog", "user-ninja", "person-arrow-up-from-line", "torah", "quidditch", "toggle-off", "box-archive", "person-drowning", "sort-numeric-down-alt", "grin-tongue-squint", "spray-can", "truck-monster", "w", "globe-africa", "rainbow", "circle-notch", "tablet-screen-button", "paw", "cloud", "trowel-bricks", "flushed", "hospital-user", "tent-arrow-left-right", "legal", "binoculars", "microphone-slash", "box-tissue", "motorcycle", "concierge-bell", "pencil-ruler", "people-arrows", "mars-and-venus-burst", "square-caret-right", "scissors", "sun-plant-wilt", "toilets-portable", "hockey-puck", "table", "magnifying-glass-arrow-right", "tachograph-digital", "users-slash", "clover", "reply", "star-and-crescent", "house-fire", "square-minus", "helicopter", "compass", "square-caret-down", "file-circle-question", "laptop-code", "swatchbook", "prescription-bottle", "navicon", "people-group", "hourglass-end", "heart-crack", "square-up-right", "kiss-beam", "film", "ruler-horizontal", "people-robbery", "lightbulb", "caret-left", "exclamation-circle", "school-circle-xmark", "sign-out", "circle-chevron-down", "unlock-keyhole", "cloud-showers-heavy", "headphones-simple", "sitemap", "donate", "memory", "road-spikes", "fire-burner", "flag", "hanukiah", "feather", "volume-low", "comment-slash", "cloud-sun-rain", "compress", "wheat-awn", "ankh", "hands-holding-child", "asterisk", "square-check", "peseta-sign", "heading", "ghost", "list", "square-phone-flip", "cart-plus", "gamepad", "dot-circle", "face-dizzy", "egg", "house-medical-circle-xmark", "campground", "folder-plus", "soccer-ball", "paintbrush", "lock", "gas-pump", "hot-tub", "map-marked", "house-flood-water", "tree", "bridge-lock", "sack-dollar", "pen-to-square", "car-side", "share-nodes", "heart-circle-minus", "hourglass-half", "microscope", "sink", "shopping-bag", "sort-alpha-down-alt", "mitten", "person-rays", "users", "eye-slash", "flask-vial", "hand", "om", "worm", "house-circle-xmark", "plug", "chevron-up", "hand-spock", "stopwatch", "kiss", "bridge-circle-xmark", "grin-tongue", "chess-bishop", "grin-wink", "hard-of-hearing", "road-circle-check", "dice-five", "square-rss", "land-mine-on", "i-cursor", "stamp", "stairs", "i", "hryvnia", "pills", "grin-alt", "tooth", "v", "bangladeshi-taka-sign", "bicycle", "staff-snake", "head-side-cough-slash", "truck-medical", "wheat-awn-circle-exclamation", "snowman", "mortar-pestle", "road-barrier", "school", "igloo", "joint", "angle-right", "horse", "q", "g", "notes-medical", "thermometer-half", "dong-sign", "capsules", "poo-storm", "frown-open", "hand-point-up", "money-bill", "bookmark", "align-justify", "umbrella-beach", "helmet-un", "bullseye", "bacon", "hand-point-down", "arrow-up-from-bracket", "folder", "file-waveform", "radiation", "chart-simple", "mars-stroke", "vial", "tachometer-alt-average", "wand-magic-sparkles", "e", "pen-clip", "bridge-circle-exclamation", "user", "school-circle-check", "dumpster", "van-shuttle", "building-user", "square-caret-left", "highlighter", "key", "bullhorn", "globe", "synagogue", "person-half-dress", "road-bridge", "location-arrow", "c", "tablet-button", "building-lock", "pizza-slice", "money-bill-wave", "chart-area", "house-flag", "person-circle-minus", "cancel", "camera-rotate", "spray-can-sparkles", "star", "repeat", "cross", "box", "venus-mars", "mouse-pointer", "maximize", "charging-station", "triangle-circle-square", "shuffle", "running", "mobile-retro", "grip-lines-vertical", "spider", "hands-bound", "file-invoice-dollar", "plane-circle-exclamation", "x-ray", "spell-check", "slash", "mouse", "sign-in", "store-alt-slash", "server", "virus-covid-slash", "shop-lock", "hourglass-start", "blender-phone", "building-wheat", "person-breastfeeding", "sign-in-alt", "venus", "passport", "heartbeat", "people-carry", "temperature-high", "microchip", "crown", "weight-hanging", "xmarks-lines", "file-prescription", "weight", "user-group", "sort-alpha-up", "chess-knight", "laugh-squint", "wheelchair", "circle-arrow-up", "toggle-on", "walking", "l", "fire", "procedures", "space-shuttle", "laugh", "folder-open", "heart-circle-plus", "code-fork", "city", "microphone-lines", "pepper-hot", "unlock", "colon-sign", "headset", "store-slash", "road-circle-xmark", "user-minus", "mars-stroke-v", "glass-cheers", "clipboard", "house-circle-exclamation", "file-upload", "wifi", "bathtub", "underline", "user-pen", "signature", "stroopwafel", "bold", "anchor-lock", "building-ngo", "manat-sign", "not-equal", "border-top-left", "map-marked-alt", "jedi", "square-poll-vertical", "mug-hot", "car-battery", "gift", "dice-two", "chess-queen", "glasses", "chess-board", "building-circle-check", "person-chalkboard", "mars-stroke-right", "hand-rock", "square-caret-up", "cloud-showers-water", "chart-bar", "hands-wash", "less-than-equal", "train", "low-vision", "crow", "sailboat", "window-restore", "square-plus", "torii-gate", "frog", "bucket", "image", "microphone", "cow", "caret-up", "screwdriver", "folder-closed", "house-tsunami", "square-nfi", "arrow-up-from-ground-water", "martini-glass", "undo-alt", "table-columns", "lemon", "head-side-mask", "handshake", "gem", "dolly", "smoking", "minimize", "monument", "snowplow", "angles-right", "cannabis", "play-circle", "tablets", "ethernet", "euro", "chair", "circle-check", "stop-circle", "drafting-compass", "plate-wheat", "icicles", "person-shelter", "neuter", "id-badge", "marker", "laugh-beam", "helicopter-symbol", "universal-access", "circle-chevron-up", "lari-sign", "volcano", "person-walking-dashed-line-arrow-right", "sterling-sign", "viruses", "square-person-confined", "user-tie", "long-arrow-down", "tent-arrow-down-to-line", "certificate", "reply-all", "suitcase", "skating", "funnel-dollar", "camera-retro", "circle-arrow-down", "file-import", "square-arrow-up-right", "box-open", "scroll", "spa", "location-pin-lock", "pause", "hill-avalanche", "thermometer-empty", "bomb", "registered", "vcard", "scale-unbalanced-flip", "subscript", "directions", "burst", "laptop-house", "tired", "money-bills", "smog", "crutch", "cloud-upload", "palette", "arrows-turn-right", "vest", "ferry", "arrows-down-to-people", "sprout", "left-right", "boxes-packing", "circle-arrow-left", "group-arrows-rotate", "bowl-food", "candy-cane", "sort-amount-down", "thunderstorm", "text-slash", "smile-wink", "file-word", "file-powerpoint", "arrows-left-right", "house-lock", "cloud-download", "children", "chalkboard", "user-large-slash", "envelope-open", "handshake-simple-slash", "mattress-pillow", "guarani-sign", "sync", "fire-extinguisher", "cruzeiro-sign", "greater-than-equal", "shield-halved", "book-atlas", "virus", "envelope-circle-check", "layer-group", "arrows-to-dot", "archway", "heart-circle-check", "house-damage", "file-zipper", "square", "martini-glass-empty", "couch", "cedi-sign", "italic", "church", "comments-dollar", "democrat", "z", "skiing", "road-lock", "a", "temperature-down", "feather-pointed", "p", "snowflake", "newspaper", "rectangle-ad", "circle-arrow-right", "filter-circle-xmark", "locust", "unsorted", "list-ol", "person-dress-burst", "money-check-dollar", "vector-square", "bread-slice", "language", "kiss-wink-heart", "filter", "question", "file-signature", "up-down-left-right", "house-chimney-user", "hand-holding-heart", "puzzle-piece", "money-check", "star-half-stroke", "code", "whiskey-glass", "building-circle-exclamation", "magnifying-glass-chart", "external-link", "cubes-stacked", "won", "virus-covid", "austral-sign", "f", "leaf", "road", "taxi", "person-circle-plus", "pie-chart", "bolt-lightning", "sack-xmark", "file-excel", "file-contract", "fish-fins", "building-flag", "grin-beam", "object-ungroup", "poop", "map-marker", "kaaba", "toilet-paper", "helmet-safety", "eject", "circle-right", "plane-circle-check", "meh-rolling-eyes", "object-group", "line-chart", "mask-ventilator", "arrow-right", "signs-post", "cash-register", "person-circle-question", "h", "tarp", "tools", "arrows-to-eye", "plug-circle-bolt", "heart", "mars-and-venus", "house-user", "dumpster-fire", "house-crack", "martini-glass-citrus", "surprise", "bottle-water", "pause-circle", "toilet-paper-slash", "apple-whole", "kitchen-set", "r", "thermometer-quarter", "cube", "bitcoin-sign", "shield-dog", "solar-panel", "lock-open", "elevator", "money-bill-transfer", "money-bill-trend-up", "house-flood-water-circle-arrow-right", "square-poll-horizontal", "circle", "fast-backward", "recycle", "user-astronaut", "plane-slash", "trademark", "basketball", "satellite-dish", "circle-up", "mobile-screen-button", "volume-up", "users-rays", "wallet", "clipboard-check", "file-audio", "hamburger", "wrench", "bugs", "rupee", "file-image", "question-circle", "plane-departure", "handshake-slash", "book-bookmark", "code-branch", "hat-cowboy", "bridge", "phone-flip", "truck-front", "cat", "anchor-circle-exclamation", "truck-field", "route", "clipboard-question", "panorama", "comment-medical", "teeth-open", "file-circle-minus", "tags", "wine-glass", "fast", "meh-blank", "square-parking", "house-signal", "tasks-alt", "faucet-drip", "dolly-flatbed", "smoking-ban", "terminal", "mobile-button", "house-medical-flag", "shopping-basket", "tape", "bus-simple", "eye", "sad-cry", "audio-description", "person-military-to-person", "file-shield", "user-slash", "pen", "tower-observation", "file-code", "signal", "bus", "heart-circle-xmark", "house-chimney", "window-maximize", "frown", "prescription", "store-alt", "save", "vihara", "scale-unbalanced", "sort-up", "commenting", "plant-wilt", "diamond", "grin-squint", "hand-holding-usd", "bacterium", "hand-pointer", "drum-steelpan", "hand-scissors", "praying-hands", "redo", "biohazard", "location", "mars-double", "child-dress", "users-between-lines", "lungs-virus", "grin-tears", "phone", "calendar-xmark", "child-reaching", "head-side-virus", "user-gear", "sort-numeric-up", "door-closed", "shield-virus", "dice-six", "mosquito-net", "bridge-water", "person-booth", "text-width", "hat-wizard", "fancy", "person-digging", "trash", "tachometer-average", "book-medical", "poo", "quote-right", "tshirt", "cubes", "divide", "tenge", "headphones", "hands-holding", "hands-clapping", "republican", "arrow-left", "person-circle-xmark", "ruler", "align-left", "dice-d6", "restroom", "j", "users-viewfinder", "file-video", "up-right-from-square", "th", "file-pdf", "book-bible", "o", "suitcase-medical", "user-secret", "otter", "person-dress", "comment-dollar", "business-time", "th-large", "tanakh", "volume-control-phone", "hat-cowboy-side", "clipboard-user", "child", "lira-sign", "satellite", "plane-lock", "tag", "comment", "cake", "envelope", "angles-up", "paperclip", "arrow-right-to-city", "ribbon", "lungs", "sort-numeric-up-alt", "litecoin-sign", "border-none", "circle-nodes", "parachute-box", "indent", "truck-field-un", "hourglass", "mountain", "user-md", "info-circle", "cloud-meatball", "camera", "square-virus", "meteor", "car-on", "sleigh", "sort-numeric-down", "hand-holding-water", "water", "calendar-check", "braille", "prescription-bottle-medical", "landmark", "truck", "crosshairs", "person-cane", "tent", "vest-patches", "check-double", "sort-alpha-down", "money-bill-wheat", "cookie", "undo", "hdd", "grin-squint-tears", "dumbbell", "rectangle-list", "tarp-droplet", "house-medical-circle-check", "skiing-nordic", "calendar-plus", "plane-arrival", "circle-left", "train-subway", "chart-gantt", "inr", "crop-simple", "money-bill-alt", "long-arrow-alt-left", "dna", "virus-slash", "subtract", "chess", "long-arrow-left", "plug-circle-check", "street-view", "franc-sign", "volume-off", "hands-asl-interpreting", "gear", "tint-slash", "mosque", "mosquito", "star-of-david", "person-military-rifle", "shopping-cart", "vials", "plug-circle-plus", "place-of-worship", "grip-vertical", "level-up", "u", "square-root-variable", "clock", "step-backward", "pallet", "faucet", "baseball-bat-ball", "s", "timeline", "keyboard", "caret-down", "house-chimney-medical", "thermometer-three-quarters", "mobile-screen", "plane-up", "piggy-bank", "battery-half", "mountain-city", "coins", "khanda", "sliders", "folder-tree", "network-wired", "map-pin", "hamsa", "cent-sign", "flask", "person-pregnant", "wand-sparkles", "ellipsis-vertical", "ticket", "power-off", "right-long", "flag-usa", "laptop-file", "tty", "diagram-next", "person-rifle", "house-medical-circle-exclamation", "closed-captioning", "person-hiking", "venus-double", "images", "calculator", "people-pulling", "n", "tram", "cloud-rain", "building-circle-xmark", "ship", "arrows-down-to-line", "download", "grin", "delete-left", "eyedropper", "file-circle-check", "forward", "mobile", "meh", "align-center", "book-skull", "id-card", "outdent", "heart-circle-exclamation", "house", "calendar-week", "laptop-medical", "b", "file-medical", "dice-one", "kiwi-bird", "exchange", "rotate-right", "utensils", "sort-amount-up", "mill-sign", "bowl-rice", "skull", "tower-broadcast", "truck-pickup", "up-long", "stop", "code-merge", "upload", "hurricane", "mound", "toilet-portable", "compact-disc", "file-download", "caravan", "shield-cat", "zap", "glass-water", "oil-well", "vault", "mars", "toilet", "plane-circle-xmark", "yen", "ruble", "sun", "guitar", "laugh-wink", "horse-head", "bore-hole", "industry", "circle-down", "arrows-turn-to-dots", "florin-sign", "sort-amount-down-alt", "less-than", "angle-down", "car-tunnel", "head-side-cough", "grip-lines", "thumbs-down", "user-lock", "long-arrow-right", "anchor-circle-xmark", "ellipsis", "chess-pawn", "kit-medical", "person-through-window", "toolbox", "hands-holding-circle", "bug", "credit-card", "car", "hand-holding-hand", "book-reader", "mountain-sun", "arrows-left-right-to-line", "dice-d20", "truck-droplet", "file-circle-xmark", "temperature-up", "medal", "bed", "square-h", "podcast", "thermometer-full", "bell", "superscript", "plug-circle-xmark", "star-of-life", "phone-slash", "paint-roller", "handshake-angle", "map-marker-alt", "file", "greater-than", "swimmer", "arrow-down", "tint", "eraser", "globe-americas", "person-burst", "dove", "battery-empty", "socks", "inbox", "section", "tachometer-alt", "envelope-open-text", "hospital", "wine-bottle", "chess-rook", "stream", "dharmachakra", "hotdog", "person-walking-with-cane", "drum", "ice-cream", "heart-circle-bolt", "fax", "paragraph", "vote-yea", "star-half", "boxes", "link", "ear-listen", "tree-city", "play", "font", "rupiah-sign", "search", "table-tennis", "person-dots-from-line", "trash-restore-alt", "naira-sign", "cart-arrow-down", "walkie-talkie", "file-pen", "receipt", "square-pen", "suitcase-rolling", "person-circle-exclamation", "chevron-down", "battery", "skull-crossbones", "code-compare", "list-ul", "school-lock", "tower-cell", "long-arrow-alt-down", "ranking-star", "chess-king", "person-harassing", "brazilian-real-sign", "landmark-dome", "arrow-up", "tv", "shrimp", "tasks", "jug-detergent", "user-circle", "user-shield", "wind", "car-crash", "y", "snowboarding", "fast", "fish", "user-graduate", "circle-half-stroke", "clapperboard", "radiation-alt", "baseball", "jet-fighter-up", "project-diagram", "copy", "volume-xmark", "hand-sparkles", "grip", "share-square", "child-rifle", "gun", "square-phone", "plus", "expand", "computer", "xmark", "arrows", "chalkboard-user", "peso-sign", "building-shield", "baby", "users-line", "quote-left", "tractor", "trash-restore", "arrow-down-up-lock", "lines-leaning", "ruler-combined", "copyright", "equals", "blender", "teeth", "sheqel", "map", "rocket", "photo-video", "folder-minus", "store", "arrow-trend-up", "plug-circle-minus", "sign", "bezier-curve", "bell-slash", "tablet", "school-flag", "fill", "angle-up", "drumstick-bite", "holly-berry", "chevron-left", "bacteria", "hand-lizard", "notdef", "disease", "briefcase-medical", "genderless", "chevron-right", "retweet", "car-rear", "pump-soap", "video-slash", "battery-quarter", "radio", "carriage-baby", "traffic-light", "thermometer", "vr-cardboard", "hand-middle-finger", "percentage", "truck-moving", "glass-water-droplet", "display", "smile", "thumbtack", "trophy", "pray", "hammer", "hand-peace", "sync-alt", "spinner", "robot", "peace", "gears", "warehouse", "arrow-up-right-dots", "splotch", "grin-hearts", "dice-four", "sim-card", "transgender", "mercury", "level-down", "falling-burst", "award", "ticket-simple", "building", "angles-left", "qrcode", "history", "grin-beam-sweat", "file-export", "shield", "sort-amount-up-alt", "house-medical", "golf-ball", "circle-chevron-left", "house-chimney-window", "pen-nib", "tent-arrow-turn-left", "tents", "wand-magic", "dog", "carrot", "moon", "wine-glass-empty", "cheese", "yin-yang", "music", "code-commit", "temperature-low", "person-biking", "broom", "shield-heart", "gopuram", "globe-oceania", "xmark-square", "hashtag", "up-right-and-down-left-from-center", "oil-can", "t", "hippo", "chart-column", "infinity", "vial-circle-check", "person-arrow-down-to-line", "voicemail", "fan", "person-walking-luggage", "up-down", "cloud-moon-rain", "calendar", "trailer", "haykal", "sd-card", "dragon", "shoe-prints", "plus-circle", "grin-tongue-wink", "hand-holding", "plug-circle-exclamation", "unlink", "clone", "person-walking-arrow-loop-left", "sort-alpha-up-alt", "fire-flame-curved", "tornado", "file-circle-plus", "quran", "anchor", "border-all", "face-angry", "cookie-bite", "arrow-trend-down", "rss", "draw-polygon", "scale-balanced", "tachometer", "shower", "desktop", "m", "th-list", "sms", "book", "user-plus", "check", "battery-three-quarters", "house-circle-check", "angle-left", "diagram-successor", "truck-arrow-right", "arrows-split-up-and-left", "hand-fist", "cloud-moon", "briefcase", "falling", "portrait", "user-tag", "rug", "globe-europe", "luggage-cart", "window-close", "baht-sign", "book-open", "journal-whills", "handcuffs", "warning", "database", "share", "bottle-droplet", "face", "hill-rockslide", "right-left", "paper-plane", "road-circle-exclamation", "dungeon", "align-right", "money-bill-wave-alt", "life-ring", "signing", "calendar-day", "water-ladder", "arrows-v", "grimace", "wheelchair-move", "turn-down", "person-walking-arrow-right", "square-envelope", "dice", "bowling-ball", "brain", "bandage", "calendar-minus", "xmark-circle", "gifts", "hotel", "globe-asia", "id-card-clip", "search-plus", "thumbs-up", "user-clock", "hand-dots", "file-invoice", "window-minimize", "mug-saucer", "brush", "mask", "search-minus", "ruler-vertical", "user-large", "train-tram", "user-nurse", "syringe", "cloud-sun", "stopwatch-20", "square-full", "magnet", "jar", "sticky-note", "bug-slash", "arrow-up-from-water-pump", "bone", "user-injured", "sad-tear", "plane", "tent-arrows-down", "exclamation", "arrows-spin", "print", "turkish-lira", "usd", "x", "search-dollar", "users-gear", "person-military-pointing", "university", "umbrella", "trowel", "d", "stapler", "theater-masks", "kip-sign", "hand-point-left", "handshake-simple", "jet-fighter", "square-share-nodes", "barcode", "plus-minus", "video", "mortar-board", "hand-holding-medical", "person-circle-check", "turn-up"];
+const qe = ["1", "2", "3", "4", "5", "6", "7", "8", "9", "fill-drip", "arrows-to-circle", "circle-chevron-right", "at", "trash-can", "text-height", "user-xmark", "stethoscope", "message", "info", "down-left-and-up-right-to-center", "explosion", "file-text", "wave-square", "ring", "building-un", "dice-three", "calendar-days", "anchor-circle-check", "building-circle-arrow-right", "volleyball", "arrows-up-to-line", "sort-down", "minus-circle", "door-open", "sign-out-alt", "atom", "soap", "icons", "microphone-lines-slash", "bridge-circle-check", "pump-medical", "fingerprint", "hand-point-right", "search-location", "step-forward", "smile-beam", "flag-checkered", "football", "school-circle-exclamation", "crop", "angles-down", "users-rectangle", "people-roof", "people-line", "beer", "diagram-predecessor", "long-arrow-up", "fire-flame-simple", "person", "laptop", "file-csv", "menorah", "truck-plane", "record-vinyl", "grin-stars", "bong", "spaghetti-monster-flying", "arrow-down-up-across-line", "utensil-spoon", "jar-wheat", "mail-bulk", "file-circle-exclamation", "hospital-symbol", "pager", "contact-book", "strikethrough", "k", "landmark-flag", "pencil", "backward", "caret-right", "comments", "paste", "code-pull-request", "clipboard-list", "truck-ramp-box", "user-check", "vial-virus", "sheet-plastic", "blog", "user-ninja", "person-arrow-up-from-line", "torah", "quidditch", "toggle-off", "box-archive", "person-drowning", "sort-numeric-down-alt", "grin-tongue-squint", "spray-can", "truck-monster", "w", "globe-africa", "rainbow", "circle-notch", "tablet-screen-button", "paw", "cloud", "trowel-bricks", "flushed", "hospital-user", "tent-arrow-left-right", "legal", "binoculars", "microphone-slash", "box-tissue", "motorcycle", "concierge-bell", "pencil-ruler", "people-arrows", "mars-and-venus-burst", "square-caret-right", "scissors", "sun-plant-wilt", "toilets-portable", "hockey-puck", "table", "magnifying-glass-arrow-right", "tachograph-digital", "users-slash", "clover", "reply", "star-and-crescent", "house-fire", "square-minus", "helicopter", "compass", "square-caret-down", "file-circle-question", "laptop-code", "swatchbook", "prescription-bottle", "navicon", "people-group", "hourglass-end", "heart-crack", "square-up-right", "kiss-beam", "film", "ruler-horizontal", "people-robbery", "lightbulb", "caret-left", "exclamation-circle", "school-circle-xmark", "sign-out", "circle-chevron-down", "unlock-keyhole", "cloud-showers-heavy", "headphones-simple", "sitemap", "donate", "memory", "road-spikes", "fire-burner", "flag", "hanukiah", "feather", "volume-low", "comment-slash", "cloud-sun-rain", "compress", "wheat-awn", "ankh", "hands-holding-child", "asterisk", "square-check", "peseta-sign", "heading", "ghost", "list", "square-phone-flip", "cart-plus", "gamepad", "dot-circle", "face-dizzy", "egg", "house-medical-circle-xmark", "campground", "folder-plus", "soccer-ball", "paintbrush", "lock", "gas-pump", "hot-tub", "map-marked", "house-flood-water", "tree", "bridge-lock", "sack-dollar", "pen-to-square", "car-side", "share-nodes", "heart-circle-minus", "hourglass-half", "microscope", "sink", "shopping-bag", "sort-alpha-down-alt", "mitten", "person-rays", "users", "eye-slash", "flask-vial", "hand", "om", "worm", "house-circle-xmark", "plug", "chevron-up", "hand-spock", "stopwatch", "kiss", "bridge-circle-xmark", "grin-tongue", "chess-bishop", "grin-wink", "hard-of-hearing", "road-circle-check", "dice-five", "square-rss", "land-mine-on", "i-cursor", "stamp", "stairs", "i", "hryvnia", "pills", "grin-alt", "tooth", "v", "bangladeshi-taka-sign", "bicycle", "staff-snake", "head-side-cough-slash", "truck-medical", "wheat-awn-circle-exclamation", "snowman", "mortar-pestle", "road-barrier", "school", "igloo", "joint", "angle-right", "horse", "q", "g", "notes-medical", "thermometer-half", "dong-sign", "capsules", "poo-storm", "frown-open", "hand-point-up", "money-bill", "bookmark", "align-justify", "umbrella-beach", "helmet-un", "bullseye", "bacon", "hand-point-down", "arrow-up-from-bracket", "folder", "file-waveform", "radiation", "chart-simple", "mars-stroke", "vial", "tachometer-alt-average", "wand-magic-sparkles", "e", "pen-clip", "bridge-circle-exclamation", "user", "school-circle-check", "dumpster", "van-shuttle", "building-user", "square-caret-left", "highlighter", "key", "bullhorn", "globe", "synagogue", "person-half-dress", "road-bridge", "location-arrow", "c", "tablet-button", "building-lock", "pizza-slice", "money-bill-wave", "chart-area", "house-flag", "person-circle-minus", "cancel", "camera-rotate", "spray-can-sparkles", "star", "repeat", "cross", "box", "venus-mars", "mouse-pointer", "maximize", "charging-station", "triangle-circle-square", "shuffle", "running", "mobile-retro", "grip-lines-vertical", "spider", "hands-bound", "file-invoice-dollar", "plane-circle-exclamation", "x-ray", "spell-check", "slash", "mouse", "sign-in", "store-alt-slash", "server", "virus-covid-slash", "shop-lock", "hourglass-start", "blender-phone", "building-wheat", "person-breastfeeding", "sign-in-alt", "venus", "passport", "heartbeat", "people-carry", "temperature-high", "microchip", "crown", "weight-hanging", "xmarks-lines", "file-prescription", "weight", "user-group", "sort-alpha-up", "chess-knight", "laugh-squint", "wheelchair", "circle-arrow-up", "toggle-on", "walking", "l", "fire", "procedures", "space-shuttle", "laugh", "folder-open", "heart-circle-plus", "code-fork", "city", "microphone-lines", "pepper-hot", "unlock", "colon-sign", "headset", "store-slash", "road-circle-xmark", "user-minus", "mars-stroke-v", "glass-cheers", "clipboard", "house-circle-exclamation", "file-upload", "wifi", "bathtub", "underline", "user-pen", "signature", "stroopwafel", "bold", "anchor-lock", "building-ngo", "manat-sign", "not-equal", "border-top-left", "map-marked-alt", "jedi", "square-poll-vertical", "mug-hot", "car-battery", "gift", "dice-two", "chess-queen", "glasses", "chess-board", "building-circle-check", "person-chalkboard", "mars-stroke-right", "hand-rock", "square-caret-up", "cloud-showers-water", "chart-bar", "hands-wash", "less-than-equal", "train", "low-vision", "crow", "sailboat", "window-restore", "square-plus", "torii-gate", "frog", "bucket", "image", "microphone", "cow", "caret-up", "screwdriver", "folder-closed", "house-tsunami", "square-nfi", "arrow-up-from-ground-water", "martini-glass", "undo-alt", "table-columns", "lemon", "head-side-mask", "handshake", "gem", "dolly", "smoking", "minimize", "monument", "snowplow", "angles-right", "cannabis", "play-circle", "tablets", "ethernet", "euro", "chair", "circle-check", "stop-circle", "drafting-compass", "plate-wheat", "icicles", "person-shelter", "neuter", "id-badge", "marker", "laugh-beam", "helicopter-symbol", "universal-access", "circle-chevron-up", "lari-sign", "volcano", "person-walking-dashed-line-arrow-right", "sterling-sign", "viruses", "square-person-confined", "user-tie", "long-arrow-down", "tent-arrow-down-to-line", "certificate", "reply-all", "suitcase", "skating", "funnel-dollar", "camera-retro", "circle-arrow-down", "file-import", "square-arrow-up-right", "box-open", "scroll", "spa", "location-pin-lock", "pause", "hill-avalanche", "thermometer-empty", "bomb", "registered", "vcard", "scale-unbalanced-flip", "subscript", "directions", "burst", "laptop-house", "tired", "money-bills", "smog", "crutch", "cloud-upload", "palette", "arrows-turn-right", "vest", "ferry", "arrows-down-to-people", "sprout", "left-right", "boxes-packing", "circle-arrow-left", "group-arrows-rotate", "bowl-food", "candy-cane", "sort-amount-down", "thunderstorm", "text-slash", "smile-wink", "file-word", "file-powerpoint", "arrows-left-right", "house-lock", "cloud-download", "children", "chalkboard", "user-large-slash", "envelope-open", "handshake-simple-slash", "mattress-pillow", "guarani-sign", "sync", "fire-extinguisher", "cruzeiro-sign", "greater-than-equal", "shield-halved", "book-atlas", "virus", "envelope-circle-check", "layer-group", "arrows-to-dot", "archway", "heart-circle-check", "house-damage", "file-zipper", "square", "martini-glass-empty", "couch", "cedi-sign", "italic", "church", "comments-dollar", "democrat", "z", "skiing", "road-lock", "a", "temperature-down", "feather-pointed", "p", "snowflake", "newspaper", "rectangle-ad", "circle-arrow-right", "filter-circle-xmark", "locust", "unsorted", "list-ol", "person-dress-burst", "money-check-dollar", "vector-square", "bread-slice", "language", "kiss-wink-heart", "filter", "question", "file-signature", "up-down-left-right", "house-chimney-user", "hand-holding-heart", "puzzle-piece", "money-check", "star-half-stroke", "code", "whiskey-glass", "building-circle-exclamation", "magnifying-glass-chart", "external-link", "cubes-stacked", "won", "virus-covid", "austral-sign", "f", "leaf", "road", "taxi", "person-circle-plus", "pie-chart", "bolt-lightning", "sack-xmark", "file-excel", "file-contract", "fish-fins", "building-flag", "grin-beam", "object-ungroup", "poop", "map-marker", "kaaba", "toilet-paper", "helmet-safety", "eject", "circle-right", "plane-circle-check", "meh-rolling-eyes", "object-group", "line-chart", "mask-ventilator", "arrow-right", "signs-post", "cash-register", "person-circle-question", "h", "tarp", "tools", "arrows-to-eye", "plug-circle-bolt", "heart", "mars-and-venus", "house-user", "dumpster-fire", "house-crack", "martini-glass-citrus", "surprise", "bottle-water", "pause-circle", "toilet-paper-slash", "apple-whole", "kitchen-set", "r", "thermometer-quarter", "cube", "bitcoin-sign", "shield-dog", "solar-panel", "lock-open", "elevator", "money-bill-transfer", "money-bill-trend-up", "house-flood-water-circle-arrow-right", "square-poll-horizontal", "circle", "fast-backward", "recycle", "user-astronaut", "plane-slash", "trademark", "basketball", "satellite-dish", "circle-up", "mobile-screen-button", "volume-up", "users-rays", "wallet", "clipboard-check", "file-audio", "hamburger", "wrench", "bugs", "rupee", "file-image", "question-circle", "plane-departure", "handshake-slash", "book-bookmark", "code-branch", "hat-cowboy", "bridge", "phone-flip", "truck-front", "cat", "anchor-circle-exclamation", "truck-field", "route", "clipboard-question", "panorama", "comment-medical", "teeth-open", "file-circle-minus", "tags", "wine-glass", "fast", "meh-blank", "square-parking", "house-signal", "tasks-alt", "faucet-drip", "dolly-flatbed", "smoking-ban", "terminal", "mobile-button", "house-medical-flag", "shopping-basket", "tape", "bus-simple", "eye", "sad-cry", "audio-description", "person-military-to-person", "file-shield", "user-slash", "pen", "tower-observation", "file-code", "signal", "bus", "heart-circle-xmark", "house-chimney", "window-maximize", "frown", "prescription", "store-alt", "save", "vihara", "scale-unbalanced", "sort-up", "commenting", "plant-wilt", "diamond", "grin-squint", "hand-holding-usd", "bacterium", "hand-pointer", "drum-steelpan", "hand-scissors", "praying-hands", "redo", "biohazard", "location", "mars-double", "child-dress", "users-between-lines", "lungs-virus", "grin-tears", "phone", "calendar-xmark", "child-reaching", "head-side-virus", "user-gear", "sort-numeric-up", "door-closed", "shield-virus", "dice-six", "mosquito-net", "bridge-water", "person-booth", "text-width", "hat-wizard", "fancy", "person-digging", "trash", "tachometer-average", "book-medical", "poo", "quote-right", "tshirt", "cubes", "divide", "tenge", "headphones", "hands-holding", "hands-clapping", "republican", "arrow-left", "person-circle-xmark", "ruler", "align-left", "dice-d6", "restroom", "j", "users-viewfinder", "file-video", "up-right-from-square", "th", "file-pdf", "book-bible", "o", "suitcase-medical", "user-secret", "otter", "person-dress", "comment-dollar", "business-time", "th-large", "tanakh", "volume-control-phone", "hat-cowboy-side", "clipboard-user", "child", "lira-sign", "satellite", "plane-lock", "tag", "comment", "cake", "envelope", "angles-up", "paperclip", "arrow-right-to-city", "ribbon", "lungs", "sort-numeric-up-alt", "litecoin-sign", "border-none", "circle-nodes", "parachute-box", "indent", "truck-field-un", "hourglass", "mountain", "user-md", "info-circle", "cloud-meatball", "camera", "square-virus", "meteor", "car-on", "sleigh", "sort-numeric-down", "hand-holding-water", "water", "calendar-check", "braille", "prescription-bottle-medical", "landmark", "truck", "crosshairs", "person-cane", "tent", "vest-patches", "check-double", "sort-alpha-down", "money-bill-wheat", "cookie", "undo", "hdd", "grin-squint-tears", "dumbbell", "rectangle-list", "tarp-droplet", "house-medical-circle-check", "skiing-nordic", "calendar-plus", "plane-arrival", "circle-left", "train-subway", "chart-gantt", "inr", "crop-simple", "money-bill-alt", "long-arrow-alt-left", "dna", "virus-slash", "subtract", "chess", "long-arrow-left", "plug-circle-check", "street-view", "franc-sign", "volume-off", "hands-asl-interpreting", "gear", "tint-slash", "mosque", "mosquito", "star-of-david", "person-military-rifle", "shopping-cart", "vials", "plug-circle-plus", "place-of-worship", "grip-vertical", "level-up", "u", "square-root-variable", "clock", "step-backward", "pallet", "faucet", "baseball-bat-ball", "s", "timeline", "keyboard", "caret-down", "house-chimney-medical", "thermometer-three-quarters", "mobile-screen", "plane-up", "piggy-bank", "battery-half", "mountain-city", "coins", "khanda", "sliders", "folder-tree", "network-wired", "map-pin", "hamsa", "cent-sign", "flask", "person-pregnant", "wand-sparkles", "ellipsis-vertical", "ticket", "power-off", "right-long", "flag-usa", "laptop-file", "tty", "diagram-next", "person-rifle", "house-medical-circle-exclamation", "closed-captioning", "person-hiking", "venus-double", "images", "calculator", "people-pulling", "n", "tram", "cloud-rain", "building-circle-xmark", "ship", "arrows-down-to-line", "download", "grin", "delete-left", "eyedropper", "file-circle-check", "forward", "mobile", "meh", "align-center", "book-skull", "id-card", "outdent", "heart-circle-exclamation", "house", "calendar-week", "laptop-medical", "b", "file-medical", "dice-one", "kiwi-bird", "exchange", "rotate-right", "utensils", "sort-amount-up", "mill-sign", "bowl-rice", "skull", "tower-broadcast", "truck-pickup", "up-long", "stop", "code-merge", "upload", "hurricane", "mound", "toilet-portable", "compact-disc", "file-download", "caravan", "shield-cat", "zap", "glass-water", "oil-well", "vault", "mars", "toilet", "plane-circle-xmark", "yen", "ruble", "sun", "guitar", "laugh-wink", "horse-head", "bore-hole", "industry", "circle-down", "arrows-turn-to-dots", "florin-sign", "sort-amount-down-alt", "less-than", "angle-down", "car-tunnel", "head-side-cough", "grip-lines", "thumbs-down", "user-lock", "long-arrow-right", "anchor-circle-xmark", "ellipsis", "chess-pawn", "kit-medical", "person-through-window", "toolbox", "hands-holding-circle", "bug", "credit-card", "car", "hand-holding-hand", "book-reader", "mountain-sun", "arrows-left-right-to-line", "dice-d20", "truck-droplet", "file-circle-xmark", "temperature-up", "medal", "bed", "square-h", "podcast", "thermometer-full", "bell", "superscript", "plug-circle-xmark", "star-of-life", "phone-slash", "paint-roller", "handshake-angle", "map-marker-alt", "file", "greater-than", "swimmer", "arrow-down", "tint", "eraser", "globe-americas", "person-burst", "dove", "battery-empty", "socks", "inbox", "section", "tachometer-alt", "envelope-open-text", "hospital", "wine-bottle", "chess-rook", "stream", "dharmachakra", "hotdog", "person-walking-with-cane", "drum", "ice-cream", "heart-circle-bolt", "fax", "paragraph", "vote-yea", "star-half", "boxes", "link", "ear-listen", "tree-city", "play", "font", "rupiah-sign", "search", "table-tennis", "person-dots-from-line", "trash-restore-alt", "naira-sign", "cart-arrow-down", "walkie-talkie", "file-pen", "receipt", "square-pen", "suitcase-rolling", "person-circle-exclamation", "chevron-down", "battery", "skull-crossbones", "code-compare", "list-ul", "school-lock", "tower-cell", "long-arrow-alt-down", "ranking-star", "chess-king", "person-harassing", "brazilian-real-sign", "landmark-dome", "arrow-up", "tv", "shrimp", "tasks", "jug-detergent", "user-circle", "user-shield", "wind", "car-crash", "y", "snowboarding", "fast", "fish", "user-graduate", "circle-half-stroke", "clapperboard", "radiation-alt", "baseball", "jet-fighter-up", "project-diagram", "copy", "volume-xmark", "hand-sparkles", "grip", "share-square", "child-rifle", "gun", "square-phone", "plus", "expand", "computer", "xmark", "arrows", "chalkboard-user", "peso-sign", "building-shield", "baby", "users-line", "quote-left", "tractor", "trash-restore", "arrow-down-up-lock", "lines-leaning", "ruler-combined", "copyright", "equals", "blender", "teeth", "sheqel", "map", "rocket", "photo-video", "folder-minus", "store", "arrow-trend-up", "plug-circle-minus", "sign", "bezier-curve", "bell-slash", "tablet", "school-flag", "fill", "angle-up", "drumstick-bite", "holly-berry", "chevron-left", "bacteria", "hand-lizard", "notdef", "disease", "briefcase-medical", "genderless", "chevron-right", "retweet", "car-rear", "pump-soap", "video-slash", "battery-quarter", "radio", "carriage-baby", "traffic-light", "thermometer", "vr-cardboard", "hand-middle-finger", "percentage", "truck-moving", "glass-water-droplet", "display", "smile", "thumbtack", "trophy", "pray", "hammer", "hand-peace", "sync-alt", "spinner", "robot", "peace", "gears", "warehouse", "arrow-up-right-dots", "splotch", "grin-hearts", "dice-four", "sim-card", "transgender", "mercury", "level-down", "falling-burst", "award", "ticket-simple", "building", "angles-left", "qrcode", "history", "grin-beam-sweat", "file-export", "shield", "sort-amount-up-alt", "house-medical", "golf-ball", "circle-chevron-left", "house-chimney-window", "pen-nib", "tent-arrow-turn-left", "tents", "wand-magic", "dog", "carrot", "moon", "wine-glass-empty", "cheese", "yin-yang", "music", "code-commit", "temperature-low", "person-biking", "broom", "shield-heart", "gopuram", "globe-oceania", "xmark-square", "hashtag", "up-right-and-down-left-from-center", "oil-can", "t", "hippo", "chart-column", "infinity", "vial-circle-check", "person-arrow-down-to-line", "voicemail", "fan", "person-walking-luggage", "up-down", "cloud-moon-rain", "calendar", "trailer", "haykal", "sd-card", "dragon", "shoe-prints", "plus-circle", "grin-tongue-wink", "hand-holding", "plug-circle-exclamation", "unlink", "clone", "person-walking-arrow-loop-left", "sort-alpha-up-alt", "fire-flame-curved", "tornado", "file-circle-plus", "quran", "anchor", "border-all", "face-angry", "cookie-bite", "arrow-trend-down", "rss", "draw-polygon", "scale-balanced", "tachometer", "shower", "desktop", "m", "th-list", "sms", "book", "user-plus", "check", "battery-three-quarters", "house-circle-check", "angle-left", "diagram-successor", "truck-arrow-right", "arrows-split-up-and-left", "hand-fist", "cloud-moon", "briefcase", "falling", "portrait", "user-tag", "rug", "globe-europe", "luggage-cart", "window-close", "baht-sign", "book-open", "journal-whills", "handcuffs", "warning", "database", "share", "bottle-droplet", "face", "hill-rockslide", "right-left", "paper-plane", "road-circle-exclamation", "dungeon", "align-right", "money-bill-wave-alt", "life-ring", "signing", "calendar-day", "water-ladder", "arrows-v", "grimace", "wheelchair-move", "turn-down", "person-walking-arrow-right", "square-envelope", "dice", "bowling-ball", "brain", "bandage", "calendar-minus", "xmark-circle", "gifts", "hotel", "globe-asia", "id-card-clip", "search-plus", "thumbs-up", "user-clock", "hand-dots", "file-invoice", "window-minimize", "mug-saucer", "brush", "mask", "search-minus", "ruler-vertical", "user-large", "train-tram", "user-nurse", "syringe", "cloud-sun", "stopwatch-20", "square-full", "magnet", "jar", "sticky-note", "bug-slash", "arrow-up-from-water-pump", "bone", "user-injured", "sad-tear", "plane", "tent-arrows-down", "exclamation", "arrows-spin", "print", "turkish-lira", "usd", "x", "search-dollar", "users-gear", "person-military-pointing", "university", "umbrella", "trowel", "d", "stapler", "theater-masks", "kip-sign", "hand-point-left", "handshake-simple", "jet-fighter", "square-share-nodes", "barcode", "plus-minus", "video", "mortar-board", "hand-holding-medical", "person-circle-check", "turn-up"];
 
 function Ae(e) {
     function n() {
         const a = {
             position: "fixed",
             color: "white",
             backgroundColor: e.isError ? "#e52207" : "#1151b3",
@@ -100,15 +100,15 @@
         })
     }
     return n()
 }
 
 function ee(e, n = !1) {
     const a = document.createElement("div");
-    a.classList.add("message"), P.createRoot(document.body.appendChild(a)).render(t.jsx(Ae, {
+    a.classList.add("message"), W.createRoot(document.body.appendChild(a)).render(t.jsx(Ae, {
         text: e,
         isError: n
     })), setTimeout(function() {
         a.remove()
     }, 3e3)
 }
 
@@ -226,41 +226,41 @@
                 children: d
             }, Math.random())
         })
     }) : typeof e == "object" && JSON.stringify(Object.keys(e)) == JSON.stringify(["id", "text"]) ? e.text : JSON.stringify(e)
 }
 
 function pe() {
-    document.querySelector(".layer") == null && P.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(Re, {}))
+    document.querySelector(".layer") == null && W.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(Ne, {}))
 }
 
 function ve(e, n) {
     xe(), pe(), window.reloader = n;
     for (var a = document.getElementsByTagName("dialog"), r = 0; r < a.length; r++) a[r].style.display = "none";
-    P.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(Oe, {
+    W.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(Oe, {
         url: A(e)
     }))
 }
 
-function Ne(e) {
-    xe(), pe(), P.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(_e, {
+function Re(e) {
+    xe(), pe(), W.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(_e, {
         url: A(e)
     }))
 }
 
 function V(e) {
     e != null && showMessage(e);
     for (var n = document.getElementsByTagName("dialog"), a = 0; a < n.length; a++)
         if (a == n.length - 1) {
             var r = n[a];
             r.close(), r.classList.remove("opened"), r.remove(), a == 0 ? (document.querySelector(".layer").style.display = "none", window.reloader && window.reloader()) : n[a - 1].style.display = "block"
         }
 }
 
-function Re(e) {
+function Ne(e) {
     const n = {
         backgroundColor: "black",
         bottom: 0,
         left: 0,
         position: "fixed",
         right: 0,
         top: 0,
@@ -363,15 +363,15 @@
     return a()
 }
 
 function w(e) {
     return e != null && (e = e.toString().replace("-", "").normalize("NFD").replace("_", "").toLowerCase()), e
 }
 
-function R(e) {
+function N(e) {
     const n = e.id || Math.random(),
         [a, r] = C.useState(e.data.name);
 
     function d(s) {
         s.preventDefault(), e.onClick ? (a && r("Aguarde...."), e.onClick(s)) : e.data.modal == !1 ? window.load(H(e.data.url)) : ve(e.data.url)
     }
 
@@ -405,15 +405,15 @@
             "data-label": w(e.data.name),
             children: i()
         })
     }
     return o()
 }
 
-function Q(e) {
+function X(e) {
     function n(i) {
         var o = i.target.parentNode.querySelector(".dropdown");
         return o == null && (o = i.target.parentNode.parentNode.querySelector(".dropdown")), o == null && (o = i.target.parentNode.parentNode.parentNode.querySelector(".dropdown")), o
     }
 
     function a(i) {
         const o = i.target.getBoundingClientRect(),
@@ -451,41 +451,41 @@
                 children: e.children
             }), e.actions && e.actions.length > 0 && t.jsx("ul", {
                 style: i,
                 onMouseLeave: r,
                 className: "dropdown",
                 children: e.actions.map(s => t.jsx("li", {
                     style: o,
-                    children: t.jsx(R, {
+                    children: t.jsx(N, {
                         data: s,
                         style: {
                             padding: 0
                         }
                     })
                 }, Math.random()))
             })]
         })
     }
     return d()
 }
 
-function W({
+function P({
     id: e,
     href: n,
     modal: a,
     imodal: r,
     children: d,
     onClick: i,
     dataLabel: o,
     style: s
 }) {
     const c = n && n.indexOf("/media/") < 0 ? H(n) : n;
 
     function u(m) {
-        m.preventDefault(), a ? ve(c) : r ? Ne(c) : window.load(c)
+        m.preventDefault(), a ? ve(c) : r ? Re(c) : window.load(c)
     }
 
     function l() {
         return t.jsx("a", {
             id: e,
             onClick: i || u,
             href: c || "#",
@@ -569,15 +569,15 @@
         return t.jsx("div", {
             style: {
                 verticalAlign: "center",
                 textAlign: "right",
                 lineHeight: "3rem"
             },
             children: e.data.map(function(a) {
-                return t.jsx(R, {
+                return t.jsx(N, {
                     data: a,
                     default: !0,
                     compact: !0
                 }, Math.random())
             })
         })
     }
@@ -722,15 +722,15 @@
                 children: [n(), a(), d()]
             })]
         })
     }
     return i()
 }
 
-function We(e) {
+function Pe(e) {
     const n = Math.random(),
         [a, r] = C.useState(e.data);
 
     function d() {
         return t.jsx(ke, {
             data: a
         })
@@ -783,15 +783,15 @@
         })) : t.jsxs("div", {
             children: [d(), i()]
         })
     }
     return c()
 }
 
-function Pe(e) {
+function We(e) {
     const n = Math.random(),
         [a, r] = C.useState(e.data.actions);
 
     function d() {
         const s = e.data.url.indexOf("?") < 0 ? "?" : "&";
         return e.data.url + s + "only=actions"
     }
@@ -803,15 +803,15 @@
     }
 
     function o() {
         return window[n] = () => i(), t.jsx("div", {
             className: "reloadable",
             id: n,
             children: a.map(function(s) {
-                return t.jsx(R, {
+                return t.jsx(N, {
                     data: s,
                     default: !0
                 }, Math.random())
             })
         })
     }
     return o()
@@ -829,15 +829,15 @@
             };
         return t.jsxs("div", {
             style: a,
             children: [e.data.title && t.jsx("h1", {
                 style: r,
                 "data-label": w(e.data.title),
                 children: e.data.title
-            }), t.jsx(Pe, {
+            }), t.jsx(We, {
                 data: e.data
             })]
         })
     }
     return n()
 }
 
@@ -856,15 +856,15 @@
             style: a,
             children: [e.data.title && t.jsx("h2", {
                 style: r,
                 "data-label": w(e.data.title),
                 children: e.data.title
             }), e.data.actions.length > 0 && t.jsx("div", {
                 children: e.data.actions.map(function(d) {
-                    return t.jsx(R, {
+                    return t.jsx(N, {
                         data: d,
                         default: !0
                     }, Math.random())
                 })
             })]
         })
     }
@@ -932,15 +932,15 @@
                 display: "inline-block",
                 textAlign: "center",
                 width: "100%",
                 margin: "auto",
                 marginBottom: 20
             },
             children: e.data.map(function(d, i) {
-                return t.jsx(W, {
+                return t.jsx(P, {
                     href: d.url,
                     style: {
                         padding: 5,
                         fontWeight: n == i ? "bold" : "normal",
                         borderBottom: n == i ? "solid 3px #2670e8" : "solid 3px inherite",
                         textDecoration: "none",
                         color: "#0c326f",
@@ -1023,29 +1023,29 @@
 
 function Ye() {
     document.querySelectorAll(".reloadable").forEach(function(e) {
         window[e.id]()
     })
 }
 
-function q({
+function B({
     id: e,
     onClick: n,
     icon: a,
     label: r,
     display: d,
     primary: i,
     compact: o,
     spin: s
 }) {
     function c() {
         return a ? o || !r ? t.jsx(b, {
             icon: a
         }) : t.jsxs(t.Fragment, {
-            children: [t.jsx(qe, {
+            children: [t.jsx(Be, {
                 style: {
                     marginRight: 10,
                     display: "none"
                 }
             }), t.jsx(b, {
                 icon: a,
                 style: {
@@ -1075,15 +1075,15 @@
                 m.preventDefault(), a && s && (m.target.dataset.spinning = a, m.target.querySelector("i.fa-spin").style.display = "inline-block", m.target.querySelector("i.fa-" + a).style.display = "none"), n(m)
             },
             children: c()
         })
     }
     return u()
 }
-const Xe = ["text", "password", "email", "number", "date", "datetime-local", "file", "image", "range", "search", "tel", "time", "url", "week", "hidden", "color"],
+const Qe = ["text", "password", "email", "number", "date", "datetime-local", "file", "image", "range", "search", "tel", "time", "url", "week", "hidden", "color"],
     Y = {
         padding: 15,
         border: "solid 1px #d9d9d9",
         borderRadius: 5
     };
 
 function re(e) {
@@ -1095,15 +1095,15 @@
 }
 
 function Se(e, n) {
     var a = new FormData(e);
     E("POST", n, et, a)
 }
 
-function Qe(e) {
+function Xe(e) {
     if (e) {
         var n = document.querySelector(".form-fieldset." + e);
         n && (n.style.display = "none");
         var a = document.querySelector(".form-group." + e);
         a && (a.style.display = "none")
     }
 }
@@ -1134,15 +1134,15 @@
                     break
                 }
     }
 }
 
 function et(e) {
     if (e) {
-        for (var n = 0; n < e.hide.length; n++) Qe(e.hide[n]);
+        for (var n = 0; n < e.hide.length; n++) Xe(e.hide[n]);
         for (var n = 0; n < e.show.length; n++) Ke(e.show[n]);
         for (var a in e.set) Ze(a, e.set[a])
     }
 }
 
 function tt(e) {
     function n() {
@@ -1224,25 +1224,25 @@
             alignItems: "baseline"
         };
         return e.data.action && (e.data.action.modal = !0), t.jsxs("div", {
             style: s,
             children: [t.jsx("label", {
                 className: e.data.required ? "bold" : "",
                 children: e.data.label
-            }), e.data.action && t.jsx(R, {
+            }), e.data.action && t.jsx(N, {
                 data: e.data.action,
                 style: {
                     padding: 0
                 }
             })]
         })
     }
 
     function r() {
-        return e.data.type == "datetime" && (e.data.type = "datetime-local"), Xe.indexOf(e.data.type) >= 0 ? t.jsx(he, {
+        return e.data.type == "datetime" && (e.data.type = "datetime-local"), Qe.indexOf(e.data.type) >= 0 ? t.jsx(he, {
             data: e.data
         }) : e.data.type == "choice" && Array.isArray(e.data.choices) ? e.data.pick ? Array.isArray(e.data.value) ? t.jsx(me, {
             data: e.data
         }) : t.jsx(ie, {
             data: e.data
         }) : t.jsx(lt, {
             data: e.data
@@ -1326,26 +1326,26 @@
             let c = o.target.files[0];
             var s = new FileReader;
             s.onload = function(u) {
                 if (re(c.name)) {
                     const v = "display" + a;
                     var l = document.createElement("img");
                     l.id = o.target.id + "img", l.style.width = "200px", l.style.display = "block", l.style.margin = "auto", l.style.marginTop = "20px", l.onload = function(j) {
-                        const D = e.data.width > e.data.height ? e.data.width / l.width : e.data.height / l.height;
+                        const I = e.data.width > e.data.height ? e.data.width / l.width : e.data.height / l.height;
                         var M = document.createElement("canvas");
-                        const B = M.getContext("2d");
+                        const q = M.getContext("2d");
                         M.height = M.width * (l.height / l.width);
                         const S = document.createElement("canvas"),
                             F = S.getContext("2d");
-                        S.width = l.width * D, S.height = l.height * D, F.drawImage(l, 0, 0, S.width, S.height), B.drawImage(S, 0, 0, S.width * D, S.height * D, 0, 0, M.width, M.height), S.toBlob(function(h) {
+                        S.width = l.width * I, S.height = l.height * I, F.drawImage(l, 0, 0, S.width, S.height), q.drawImage(S, 0, 0, S.width * I, S.height * I, 0, 0, M.width, M.height), S.toBlob(function(h) {
                             const f = new DataTransfer;
                             f.items.add(new File([h], c.name)), o.target.files = f.files
                         });
-                        var I = document.getElementById(v);
-                        I == null ? (I = document.createElement("div"), I.id = v) : I.removeChild(I.childNodes[0]), I.appendChild(l), o.target.parentNode.appendChild(I)
+                        var D = document.getElementById(v);
+                        D == null ? (D = document.createElement("div"), D.id = v) : D.removeChild(D.childNodes[0]), D.appendChild(l), o.target.parentNode.appendChild(D)
                     }, l.src = u.target.result
                 }
                 const m = document.getElementById("fileinfo" + a);
                 var x = c.size / 1024;
                 x < 1024 ? x = parseInt(x) + " Kb" : x = (x / 1024).toFixed(2) + " Mb", m.innerHTML = c.name + " / " + x, e.data.max_size && c.size / 1024 / 1024 > e.data.max_size && alert("O limite de tamanho é " + e.data.max_size + "Mb. O arquivo informado possui " + x + ". Por favor, adicione um arquivo menor.")
             }, s.readAsDataURL(c)
         }
@@ -1400,15 +1400,15 @@
                             className: "bold",
                             id: "fileinfo" + a,
                             children: ["O arquivo", e.data.max_size && "deve possuir até " + e.data.max_size + " Mb e ", "deve ter extensão", " ", e.data.extensions.map(l => "." + l).join(" ou "), "."]
                         })]
                     }), t.jsx("div", {
                         style: u,
                         align: "center",
-                        children: t.jsx(q, {
+                        children: t.jsx(B, {
                             label: "Selecionar Arquivo",
                             onClick: () => document.getElementById(a).click()
                         })
                     })]
                 }), t.jsx("input", {
                     className: "form-control " + n,
                     type: o,
@@ -1481,28 +1481,28 @@
                     cursor: "pointer",
                     marginRight: 5
                 },
                 p = {
                     fontSize: "0.8rem"
                 };
             return t.jsxs("div", {
-                children: [h == null && n.map((k, N) => t.jsxs("div", {
+                children: [h == null && n.map((k, R) => t.jsxs("div", {
                     style: f,
                     children: [t.jsx("span", {
-                        onClick: () => F(N),
+                        onClick: () => F(R),
                         style: g,
                         children: t.jsx(b, {
                             icon: "trash-can",
                             style: p
                         })
                     }), k.value]
-                }, Math.random())), h != null && Array.from(h.options).map((k, N) => t.jsxs("div", {
+                }, Math.random())), h != null && Array.from(h.options).map((k, R) => t.jsxs("div", {
                     style: f,
                     children: [t.jsx("span", {
-                        onClick: () => F(N),
+                        onClick: () => F(R),
                         style: g,
                         children: t.jsx(b, {
                             icon: "trash-can",
                             style: p
                         })
                     }), k.innerHTML]
                 }, Math.random()))]
@@ -1549,74 +1549,74 @@
                 G = null;
             for (; !G && (z = z.parentElement) instanceof HTMLElement;) z.matches("dialog") && (G = z);
             T = G;
             const O = g.getBoundingClientRect();
             var p = O.top + O.height,
                 k = O.left;
             if (T) {
-                const X = T.getBoundingClientRect();
-                p = p - X.top, k = k - X.left
+                const Q = T.getBoundingClientRect();
+                p = p - Q.top, k = k - Q.left
             } else p += window.scrollY, k += window.scrollX;
             f.width = O.width, f.top = p, f.left = k
         }
-        const N = {
+        const R = {
                 cursor: "pointer",
                 padding: 10
             },
             ne = !d && n.length > 0 && n[0].value || "";
         return t.jsxs(t.Fragment, {
             children: [t.jsx("input", {
                 id: r,
                 name: e.data.name + "__autocomplete",
                 type: "text",
                 className: "form-control",
                 onFocus: T => {
-                    T.target.select(), B(T)
+                    T.target.select(), q(T)
                 },
-                onChange: B,
-                onMouseLeave: D,
-                onBlur: D,
+                onChange: q,
+                onMouseLeave: I,
+                onBlur: I,
                 defaultValue: ne,
                 style: h,
                 "data-label": w(e.data.label)
             }), s && i && t.jsxs("ul", {
                 style: f,
                 onMouseLeave: M,
                 onMouseEnter: function(T) {
                     u = !0
                 },
                 children: [s.length == 0 && t.jsx("li", {
-                    style: N,
+                    style: R,
                     children: "Nenhuma opção encontrada."
                 }), s.map(T => t.jsx("li", {
                     onClick: () => {
                         o(!1), e.onSelect ? e.onSelect(T) : S(T)
                     },
-                    style: N,
+                    style: R,
                     className: "autocomplete-item",
                     "data-label": w(T.value),
                     children: T.value
                 }, Math.random()))]
             })]
         })
     }
 
-    function D(h) {
+    function I(h) {
         u = !1, setTimeout(function() {
             M(h)
         }, 250)
     }
 
     function M(h) {
         const f = document.getElementById(a),
             g = document.getElementById(r);
         d || f.options.length > 0 && g.value != f.options[0].innerHTML && (f.innerHTML = "", g.value = "", o(!1)), h.target.tagName == "UL" ? o(!1) : u || o(!1)
     }
 
-    function B(h) {
+    function q(h) {
         clearTimeout(l), l = setTimeout(function() {
             const f = e.data.choices.indexOf("?") < 0 ? "?" : "&";
             o(!0), E("GET", e.data.choices + f + "term=" + h.target.value, function(p) {
                 c(p)
             })
         }, 1e3)
     }
@@ -1629,20 +1629,20 @@
 
     function F(h) {
         const f = document.getElementById(a);
         var g = Array.from(f.options);
         f.innerHTML = g.slice(0, h).concat(g.slice(h + 1)).map(p => `<option selected value="${p.value}">${p.innerHTML}</option>`).join(""), c([])
     }
 
-    function I() {
+    function D() {
         return t.jsxs(t.Fragment, {
             children: [m(), v(), j()]
         })
     }
-    return I()
+    return D()
 }
 
 function rt(e) {
     function n() {
         var a = {
             ...Y
         };
@@ -1783,21 +1783,21 @@
     function d() {
         return !e.data.required && t.jsx("div", {
             id: "info-" + n,
             children: t.jsxs(le, {
                 data: {
                     text: "Esta informação é opcional. Controle seu preenchimento com o botão ao lado."
                 },
-                children: [t.jsx(q, {
+                children: [t.jsx(B, {
                     primary: !0,
                     icon: "pen-clip",
                     onClick: () => i(!0),
                     id: "show-" + n,
                     display: r.value ? "none" : "inline"
-                }), t.jsx(q, {
+                }), t.jsx(B, {
                     primary: !0,
                     icon: "trash",
                     onClick: () => i(!1),
                     id: "hide-" + n,
                     display: r.value ? "inline" : "none"
                 })]
             })
@@ -1860,21 +1860,21 @@
                 data: l
             }), t.jsxs("div", {
                 style: {
                     textAlign: "center",
                     marginTop: 10,
                     marginBottom: 10
                 },
-                children: [t.jsx(q, {
+                children: [t.jsx(B, {
                     primary: !0,
                     icon: "plus",
                     onClick: () => i(),
                     id: "extra-add-" + x + "-",
                     display: m
-                }), t.jsx(q, {
+                }), t.jsx(B, {
                     primary: !0,
                     icon: "trash",
                     onClick: () => o(x),
                     display: "inline"
                 })]
             })]
         }, Math.random())
@@ -1901,15 +1901,15 @@
             m.name = m.name.replace("__n__", "__" + n + "__")
         }), l.fields[0].value = 0) : l.fieldsets.map(function(m) {
             m.fields.map(function(x) {
                 x.map(function(v) {
                     v.name = v.name.replace("__n__", "__" + n + "__")
                 }), x[0].value = 0
             })
-        }), P.createRoot(document.getElementById(a).appendChild(document.createElement("div"))).render(r(l, "inline")), setTimeout(d, 100)
+        }), W.createRoot(document.getElementById(a).appendChild(document.createElement("div"))).render(r(l, "inline")), setTimeout(d, 100)
     }
 
     function o(l) {
         const m = e.data.template,
             v = (m.fields ? m.fields[0] : m.fieldsets[0].fields[0][0]).name.replace("__n__", "__" + l + "__"),
             j = document.querySelector("input[name=" + v + "]");
         parseInt(j.value) == 0 ? j.value = "" : j.value = -parseInt(j.value), document.getElementById("form-" + l + "-" + a).style.display = "none", d()
@@ -1923,15 +1923,15 @@
     function c() {
         return t.jsx("div", {
             id: "info-" + a,
             children: t.jsx(le, {
                 data: {
                     text: 'Clique no botão com o ícone de "+" para adicionar e com o ícone da "lixeira" para remover.'
                 },
-                children: t.jsx(q, {
+                children: t.jsx(B, {
                     primary: !0,
                     icon: "add",
                     onClick: () => i(),
                     id: "add-" + a,
                     display: e.data.value.length > 0 ? "none" : "inline"
                 })
             })
@@ -2046,20 +2046,20 @@
 
     function o() {
         return t.jsxs("div", {
             style: {
                 marginTop: 20,
                 textAlign: "right"
             },
-            children: [t.jsx(q, {
+            children: [t.jsx(B, {
                 onClick: c,
                 label: "Cancelar",
                 default: !0,
                 display: "inline"
-            }), t.jsx(q, {
+            }), t.jsx(B, {
                 onClick: u,
                 label: "Enviar",
                 primary: !0,
                 display: "inline",
                 icon: "chevron-right",
                 spin: !0
             })]
@@ -2092,22 +2092,22 @@
 
     function u(l) {
         l.preventDefault();
         var m = document.getElementById(n),
             x = new FormData(m);
         E("POST", e.data.url, function(j) {
             if (l.target.dataset.spinning && (l.target.querySelector("i.fa-spin").style.display = "none", l.target.querySelector("i.fa-" + l.target.dataset.spinning).style.display = "inline-block"), j.type == "response") return V(), Ye(), ye(j);
-            var D = j.text;
+            var I = j.text;
             console.log(j), Object.keys(j.errors).map(function(M) {
-                if (M == "__all__") D = j.errors[M];
+                if (M == "__all__") I = j.errors[M];
                 else {
-                    const B = m.querySelector("#" + M + "_error");
-                    B.querySelector("span").innerHTML = j.errors[M], B.style.display = "block"
+                    const q = m.querySelector("#" + M + "_error");
+                    q.querySelector("span").innerHTML = j.errors[M], q.style.display = "block"
                 }
-            }), ee(D, !0)
+            }), ee(I, !0)
         }, x)
     }
     return s()
 }
 
 function ct(e) {
     function n() {
@@ -2180,15 +2180,15 @@
                 width: "100%",
                 margin: "auto",
                 paddingBottom: 20,
                 lineHeight: "2.5rem"
             },
             children: n.subsets.map(function(h, f) {
                 var g = n.subset === h.name || !n.subset && f == 0;
-                return t.jsxs(W, {
+                return t.jsxs(P, {
                     href: "#",
                     style: {
                         paddingBottom: 5,
                         paddingLeft: 15,
                         paddingRight: 15,
                         fontWeight: g ? "bold" : "normal",
                         borderBottom: g ? "solid 3px #2670e8" : 0,
@@ -2216,15 +2216,15 @@
         const p = document.getElementById("form-" + e.data.id);
         p.querySelector("input[name=" + n.calendar.field + "__day]").value = h || "", p.querySelector("input[name=" + n.calendar.field + "__month]").value = f || "", p.querySelector("input[name=" + n.calendar.field + "__year]").value = g || "", S()
     }
 
     function u() {
         if (n.calendar) {
             const k = ["SEG", "TER", "QUA", "QUI", "SEX", "SAB", "DOM"],
-                N = ["JANEIRO", "FEVEVEIRO", "MARÇO", "ABRIL", "MAIO", "JUNHO", "JULHO", "AGOSTO", "SETEMRO", "OUTUBRO", "NOVEMBRO", "DEZEMBRO"],
+                R = ["JANEIRO", "FEVEVEIRO", "MARÇO", "ABRIL", "MAIO", "JUNHO", "JULHO", "AGOSTO", "SETEMRO", "OUTUBRO", "NOVEMBRO", "DEZEMBRO"],
                 ne = {
                     width: "100%",
                     borderSpacing: 0,
                     borderCollapse: "collapse",
                     marginTop: 15,
                     marginBottom: 15
                 },
@@ -2253,15 +2253,15 @@
                     cursor: "pointer",
                     lineHeight: "2rem"
                 },
                 O = {
                     padding: 10,
                     textAlign: "center"
                 },
-                X = {
+                Q = {
                     display: "flex",
                     justifyContent: "space-between",
                     alignItems: "baseline"
                 },
                 Ee = new Date,
                 ce = n.calendar.day ? new Date(n.calendar.year, n.calendar.month - 1, n.calendar.day) : null;
             for (var h = [
@@ -2278,28 +2278,28 @@
                 total: n.calendar.total[g.toLocaleDateString("pt-BR")],
                 today: g.getDate() === Ee.getDate(),
                 selected: ce ? g.getDate() == ce.getDate() : !1
             }), g.setDate(g.getDate() + 1);
             return t.jsxs("div", {
                 className: "calendar",
                 children: [t.jsxs("div", {
-                    style: X,
+                    style: Q,
                     children: [t.jsx("div", {
                         children: t.jsx(ue, {
                             default: !0,
                             icon: "arrow-left",
                             onClick: () => c(null, n.calendar.previous.month, n.calendar.previous.year)
                         })
                     }), t.jsxs("div", {
                         children: [t.jsxs("h3", {
                             align: "center",
                             style: {
                                 margin: 0
                             },
-                            children: [N[n.calendar.month - 1], " ", n.calendar.year]
+                            children: [R[n.calendar.month - 1], " ", n.calendar.year]
                         }), n.calendar.day && t.jsxs("div", {
                             align: "center",
                             className: T,
                             children: [new Date(n.calendar.year, n.calendar.month - 1, n.calendar.day).toLocaleDateString("pt-BR"), t.jsx(b, {
                                 default: !0,
                                 icon: "x",
                                 onClick: () => c(null, n.calendar.month, n.calendar.year),
@@ -2398,15 +2398,15 @@
             }, Math.random()), t.jsx("td", {
                 style: g,
                 children: t.jsx("div", {
                     style: {
                         verticalAlign: "center"
                     },
                     children: h.actions.map(function(p) {
-                        return t.jsx(R, {
+                        return t.jsx(N, {
                             data: p,
                             default: !0,
                             compact: !0
                         }, Math.random())
                     })
                 })
             })]
@@ -2419,15 +2419,15 @@
             }), t.jsx("td", {
                 style: g,
                 children: t.jsx("div", {
                     style: {
                         verticalAlign: "center"
                     },
                     children: h.actions.map(function(p) {
-                        return t.jsx(R, {
+                        return t.jsx(N, {
                             data: p,
                             default: !0,
                             compact: !0
                         }, Math.random())
                     })
                 })
             })]
@@ -2477,15 +2477,15 @@
     }
 
     function j(h) {
         const g = document.getElementById("form-" + e.data.id).querySelector("input[name=page]");
         g.value = h, S()
     }
 
-    function D() {
+    function I() {
         const h = document.getElementById("form-" + e.data.id);
         if (h) {
             const k = h.querySelector("input[name=page]");
             k && (k.value = n.pagination.page.current)
         }
         const f = {
                 display: "flex",
@@ -2546,20 +2546,20 @@
                         },
                         onKeyDown: function(k) {
                             k.key == "Enter" && (k.preventDefault(), j(k.target.value < 0 ? 1 : Math.min(k.target.value, n.pagination.page.total)))
                         }
                     }), t.jsx("div", {
                         style: g,
                         children: "|"
-                    }), n.pagination.page.previous && t.jsx(q, {
+                    }), n.pagination.page.previous && t.jsx(B, {
                         icon: "chevron-left",
                         default: !0,
                         display: "inline",
                         onClick: () => j(n.pagination.page.previous)
-                    }), n.pagination.page.next && t.jsx(q, {
+                    }), n.pagination.page.next && t.jsx(B, {
                         icon: "chevron-right",
                         default: !0,
                         display: "inline",
                         onClick: () => j(n.pagination.page.next)
                     })]
                 })
             })]
@@ -2570,23 +2570,23 @@
         return t.jsx("div", {
             align: "right",
             style: {
                 marginTop: 20,
                 marginBottom: 20
             },
             children: n.actions.map(function(h) {
-                return t.jsx(R, {
+                return t.jsx(N, {
                     data: h,
                     primary: !0
                 }, Math.random())
             })
         })
     }
 
-    function B() {
+    function q() {
         const h = {
                 backgroundColor: "#f8f8f8",
                 borderBottom: "solid 1px #DDD",
                 marginBottom: 10,
                 padding: 10
             },
             f = n.search.length > 0,
@@ -2610,15 +2610,15 @@
                     }), g && n.filters.map(function(k) {
                         return k.type != "hidden" && t.jsx("div", {
                             children: t.jsx(K, {
                                 data: k
                             })
                         }, Math.random())
                     }), t.jsx("div", {
-                        children: t.jsx(q, {
+                        children: t.jsx(B, {
                             onClick: S,
                             label: "Filtrar",
                             icon: "filter",
                             primary: !0
                         })
                     })]
                 }), g && n.filters.map(function(k) {
@@ -2639,33 +2639,33 @@
         e.data.url.indexOf("?") > 0 ? h = e.data.url + "&" + f : h = e.data.url + "?" + f, E("GET", h, function(g) {
             a(g), i(!1)
         })
     }
 
     function F() {
         return n.bi ? t.jsxs(t.Fragment, {
-            children: [B(), n.bi.map(function(h) {
+            children: [q(), n.bi.map(function(h) {
                 return t.jsx($, {
                     width: 300,
                     alignItems: "start",
                     children: h.map(function(f) {
                         return t.jsx("div", {
                             children: t.jsx(y, {
                                 data: f
                             })
                         }, Math.random())
                     })
                 }, Math.random())
             })]
         }) : t.jsxs(t.Fragment, {
-            children: [M(), o(), B(), u(), x(), D()]
+            children: [M(), o(), q(), u(), x(), I()]
         })
     }
 
-    function I() {
+    function D() {
         window[e.data.id] = () => S();
         const h = {
             backgroundColor: "white",
             padding: 20
         };
         return t.jsx("div", {
             className: "reloadable",
@@ -2679,15 +2679,15 @@
                     type: "hidden",
                     name: "subset",
                     id: "subset-" + e.data.id
                 }), d(), F()]
             })
         })
     }
-    return I()
+    return D()
 }
 
 function te(e) {
     var n = Math.random();
 
     function a() {
         var r = document.getElementById(n);
@@ -3240,15 +3240,15 @@
             align: "center",
             children: [window.application.menu.image && t.jsx("div", {
                 children: t.jsx("img", {
                     src: window.application.menu.image,
                     style: i
                 })
             }), t.jsx("div", {
-                children: t.jsx(W, {
+                children: t.jsx(P, {
                     dataLabel: "Editar Perfil",
                     href: "/api/editprofile/",
                     style: {
                         textDecoration: "none"
                     },
                     children: window.application.menu.user
                 })
@@ -3287,15 +3287,15 @@
             c = {
                 padding: 5,
                 fontSize: "1.2rem"
             };
         return i.url ? t.jsx("li", {
             style: s,
             onClick: n,
-            children: t.jsxs(W, {
+            children: t.jsxs(P, {
                 href: i.url,
                 dataLabel: w(i.label),
                 style: {
                     textDecoration: "none"
                 },
                 children: [o == 0 && t.jsx(b, {
                     icon: i.icon || "dot-circle",
@@ -3536,15 +3536,15 @@
                     display: "flex",
                     alignItems: "center"
                 },
                 children: [e.data.navbar.adder.length > 0 && t.jsx("div", {
                     style: {
                         padding: 10
                     },
-                    children: t.jsx(Q, {
+                    children: t.jsx(X, {
                         actions: e.data.navbar.adder,
                         position: {},
                         dataLabel: "plus",
                         children: t.jsx(b, {
                             icon: "plus"
                         })
                     })
@@ -3553,27 +3553,27 @@
                         padding: 10
                     },
                     children: t.jsx(Ct, {})
                 }), e.data.navbar.tools.length > 0 && t.jsx("div", {
                     style: {
                         padding: 10
                     },
-                    children: t.jsx(Q, {
+                    children: t.jsx(X, {
                         actions: e.data.navbar.tools,
                         position: {},
                         dataLabel: "tools",
                         children: t.jsx(b, {
                             icon: "tools"
                         })
                     })
                 }), e.data.navbar.settings.length > 0 && t.jsx("div", {
                     style: {
                         padding: 10
                     },
-                    children: t.jsx(Q, {
+                    children: t.jsx(X, {
                         actions: e.data.navbar.settings,
                         position: {},
                         dataLabel: "gear",
                         children: t.jsx(b, {
                             icon: "gear"
                         })
                     })
@@ -3583,15 +3583,15 @@
                         padding: 10
                     },
                     onSelect: x => document.location.href = H(x.id)
                 }), e.data.navbar.usermenu.length > 0 && t.jsx("div", {
                     style: {
                         padding: 10
                     },
-                    children: t.jsx(Q, {
+                    children: t.jsx(X, {
                         actions: e.data.navbar.usermenu,
                         position: {},
                         dataLabel: w(e.data.navbar.user),
                         children: e.data.navbar.user
                     })
                 })]
             })]
@@ -3666,24 +3666,24 @@
                 children: [i(), s()]
             })]
         })
     }
     return u()
 }
 
-function Dt(e) {
+function It(e) {
     return t.jsx("img", {
         src: e.data.src,
         style: {
             width: "100%"
         }
     })
 }
 
-function It(e) {
+function Dt(e) {
     const n = {
         width: "100%",
         textAlign: "center"
     };
     return t.jsx("div", {
         style: n,
         children: t.jsx("img", {
@@ -3693,28 +3693,28 @@
                 height: e.data.height,
                 borderRadius: e.data.round ? "50%" : 0
             }
         })
     })
 }
 
-function qt(e) {
+function Bt(e) {
     return t.jsx("iframe", {
         width: e.data.width || "100%",
         height: e.data.height || "400px",
         id: "gmap_canvas",
         src: "https://maps.google.com/maps?q=" + e.data.latitude + "," + e.data.longitude + "&t=&z=13&ie=UTF8&iwloc=&output=embed",
         frameBorder: "0",
         scrolling: "no",
         marginHeight: "0",
         marginWidth: "0"
     })
 }
 
-function Bt(e) {
+function qt(e) {
     function n(i) {
         return e.data.icon ? i.done ? t.jsx(b, {
             style: {
                 marginTop: 6
             },
             icon: e.data.icon
         }) : t.jsx("span", {
@@ -3853,15 +3853,15 @@
             style: a,
             children: e.data.label
         })
     }
     return n()
 }
 
-function Nt(e) {
+function Rt(e) {
     function n() {
         const a = {
                 padding: 20,
                 marginLeft: -20,
                 marginRight: -20,
                 textAlign: "center",
                 backgroundColor: "#f8f8f8"
@@ -3892,15 +3892,15 @@
             };
         return e.data.items.length ? t.jsxs("div", {
             style: a,
             children: [t.jsx("h2", {
                 "data-label": w(e.data.title),
                 children: e.data.title
             }), t.jsx("div", {
-                children: e.data.items.map(o => t.jsxs(W, {
+                children: e.data.items.map(o => t.jsxs(P, {
                     href: o.url,
                     style: r,
                     dataLabel: o.label,
                     children: [t.jsx("div", {
                         children: t.jsx(b, {
                             style: d,
                             icon: o.icon
@@ -3912,15 +3912,15 @@
                 }, Math.random()))
             })]
         }) : null
     }
     return n()
 }
 
-function Rt(e) {
+function Nt(e) {
     function n() {
         return t.jsx("div", {
             style: {
                 backgroundColor: "black",
                 color: "white",
                 padding: "10px",
                 minHeight: "300px",
@@ -3934,15 +3934,15 @@
         })
     }
     return n()
 }
 
 function Ot(e) {
     function n() {
-        return e.data.url ? t.jsx(W, {
+        return e.data.url ? t.jsx(P, {
             href: e.data.url,
             imodal: !!e.data.modal,
             children: e.data.icon ? t.jsx(b, {
                 icon: e.data.icon
             }) : e.data.url
         }) : t.jsx("span", {
             children: "-"
@@ -4014,59 +4014,59 @@
                 children: e.data.value
             })]
         })
     }
     return n()
 }
 var Z, se = {};
-const Wt = "/api/application/",
+const Pt = "/api/application/",
     ge = localStorage.getItem("application");
 
 function y(e) {
     const n = se[e.data.type];
-    return n ? De.createElement(n, {
+    return n ? Ie.createElement(n, {
         data: e.data
     }) : t.jsx("div", {
         children: JSON.stringify(e.data)
     })
 }
-y.register = function(e) {
-    se[e.name.toLowerCase()] = e
+y.register = function(e, n) {
+    se[n.toLowerCase()] = e
 };
 y.render = function(e) {
     Z = e, document.location.pathname == "/" ? localStorage.getItem("token") ? window.reload("/app/dashboard/") : window.reload("/app/login/") : document.location.pathname == "/app/login/" && (localStorage.getItem("token") || localStorage.getItem("application")) ? (localStorage.removeItem("token"), localStorage.removeItem("application"), document.location.reload()) : window.reload(document.location.href)
 };
-y.register(Ht);
-y.register(st);
-y.register(ut);
-y.register(We);
-y.register(J);
-y.register(Ue);
-y.register(Ve);
-y.register(Je);
-y.register(jt);
-y.register(It);
-y.register(Dt);
-y.register(qt);
-y.register(Bt);
-y.register(Ft);
-y.register(Te);
-y.register(Lt);
-y.register(At);
-y.register(kt);
-y.register(Nt);
-y.register(Rt);
-y.register(Ot);
-y.register(_t);
-y.register(Le);
-y.register(Et);
-y.register(Ie);
-y.register(zt);
-y.register(ze);
-y.register(He);
+y.register(Ht, "Counter");
+y.register(st, "Form");
+y.register(ut, "QuerySet");
+y.register(Pe, "Fieldset");
+y.register(J, "Field");
+y.register(Ue, "Object");
+y.register(Ve, "Section");
+y.register(Je, "Group");
+y.register(jt, "Statistics");
+y.register(Dt, "Image");
+y.register(It, "Banner");
+y.register(Bt, "Map");
+y.register(qt, "Steps");
+y.register(Ft, "QrCode");
+y.register(Te, "Badge");
+y.register(Lt, "Status");
+y.register(At, "Progress");
+y.register(kt, "Color");
+y.register(Rt, "Boxes");
+y.register(Nt, "Shell");
+y.register(Ot, "FileLink");
+y.register(_t, "FilePreview");
+y.register(Le, "Response");
+y.register(Et, "Application");
+y.register(De, "IconSet");
+y.register(zt, "Grid");
+y.register(ze, "Rows");
+y.register(He, "Timeline");
 window.addEventListener("popstate", e => {
     window.reload(e.currentTarget.location.href)
 });
 window.reload = function(e) {
     const n = e.split("/app/")[1].split("/")[0];
     se[n] ? E("GET", A(e), function(a) {
         Z.render(t.jsx(y, {
@@ -4077,23 +4077,23 @@
         }))
     }) : (e != document.location.href && window.history.pushState({
         url: e
     }, "", e), ge ? (window.application = JSON.parse(ge), E("GET", A(e), function(a) {
         window.application.content = a, Z.render(t.jsx(y, {
             data: window.application
         }, Math.random()))
-    })) : E("GET", Wt, function(r) {
+    })) : E("GET", Pt, function(r) {
         window.application = r, localStorage.setItem("application", JSON.stringify(window.application)), E("GET", A(e), function(d) {
             window.application.content = d, Z.render(t.jsx(y, {
                 data: window.application
             }, Math.random()))
         })
     }))
 };
 window.load = function(e) {
     e.indexOf(window.origin) >= 0 || e.startsWith("/") ? (e != document.location.href && e != document.location.pathname && window.history.pushState({
         url: e
     }, "", e), E("GET", A(e), function(n) {
         window.loaddata(n)
     })) : document.location.href = e
 };
-y.render(P.createRoot(document.getElementById("root")));
+y.render(W.createRoot(document.getElementById("root")));
```

### Comparing `pyslth-0.2.4/slth/static/js/peerjs.min.js` & `pyslth-0.2.5/slth/static/js/peerjs.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.4/slth/static/js/qrcode.min.js` & `pyslth-0.2.5/slth/static/js/qrcode.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.4/slth/static/js/react-trigger-change.js` & `pyslth-0.2.5/slth/static/js/react-trigger-change.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.4/slth/static/js/react.min.js` & `pyslth-0.2.5/slth/static/js/react.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.4/slth/static/js/vanilla-masker.js` & `pyslth-0.2.5/slth/static/js/vanilla-masker.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.4/slth/static/js/vanilla-masker.min.js` & `pyslth-0.2.5/slth/static/js/vanilla-masker.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.4/slth/statistics.py` & `pyslth-0.2.5/slth/statistics.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.4/slth/templates/index.html` & `pyslth-0.2.5/slth/templates/index.html`

 * *Files 6% similar despite different names*

```diff
@@ -52,11 +52,11 @@
   <div id="root"></div>
 </body>
 
 {% if vite %}
   <script type="module" src="http://localhost:5173/src/main.jsx"></script>
 {% else %}
   <script type="module" src="/static/js/react.min.js"></script>
-  <script type="module" src="/static/js/lib.min.js"></script>
+  <script type="module" src="/static/js/slth.min.js"></script>
   <script type="module" src="/static/js/index.min.js"></script>
 {% endif %}
 </html>
```

### Comparing `pyslth-0.2.4/slth/templates/service-worker.js` & `pyslth-0.2.5/slth/templates/service-worker.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.4/slth/tests.py` & `pyslth-0.2.5/slth/tests.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.4/slth/urls.py` & `pyslth-0.2.5/slth/urls.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.4/slth/utils.py` & `pyslth-0.2.5/slth/utils.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.4/slth/views.py` & `pyslth-0.2.5/slth/views.py`

 * *Files identical despite different names*

