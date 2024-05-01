# Comparing `tmp/django-deovi-0.6.1.tar.gz` & `tmp/django-deovi-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-deovi-0.6.1.tar", last modified: Mon Nov  6 00:46:16 2023, max compression
+gzip compressed data, was "django-deovi-0.6.2.tar", last modified: Wed May  1 20:42:59 2024, max compression
```

## Comparing `django-deovi-0.6.1.tar` & `django-deovi-0.6.2.tar`

### file list

```diff
@@ -1,78 +1,82 @@
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-11-06 00:46:16.246878 django-deovi-0.6.1/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1070 2022-01-22 01:32:29.000000 django-deovi-0.6.1/LICENCE.txt
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      289 2023-11-06 00:43:37.000000 django-deovi-0.6.1/MANIFEST.in
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1478 2023-11-06 00:46:16.246878 django-deovi-0.6.1/PKG-INFO
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      597 2023-05-01 00:28:15.000000 django-deovi-0.6.1/README.rst
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-11-06 00:46:16.242878 django-deovi-0.6.1/django_deovi/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      705 2022-08-28 00:57:38.000000 django-deovi-0.6.1/django_deovi/__init__.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-11-06 00:46:16.242878 django-deovi-0.6.1/django_deovi/admin/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      183 2022-09-01 01:11:10.000000 django-deovi-0.6.1/django_deovi/admin/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      217 2023-05-27 14:18:52.000000 django-deovi-0.6.1/django_deovi/admin/device.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      223 2023-08-16 21:41:47.000000 django-deovi-0.6.1/django_deovi/admin/directory.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      228 2022-09-01 01:11:10.000000 django-deovi-0.6.1/django_deovi/admin/media.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      187 2022-01-22 01:32:29.000000 django-deovi-0.6.1/django_deovi/apps.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     5594 2023-08-16 21:41:47.000000 django-deovi-0.6.1/django_deovi/dump.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      418 2022-08-28 00:57:38.000000 django-deovi-0.6.1/django_deovi/exceptions.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-11-06 00:46:16.242878 django-deovi-0.6.1/django_deovi/factories/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      305 2022-09-01 01:11:10.000000 django-deovi-0.6.1/django_deovi/factories/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      327 2022-09-01 01:11:10.000000 django-deovi-0.6.1/django_deovi/factories/device.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1237 2023-08-16 21:41:47.000000 django-deovi-0.6.1/django_deovi/factories/directory.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     2977 2023-08-16 21:41:47.000000 django-deovi-0.6.1/django_deovi/factories/dump.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     2184 2023-08-16 21:41:47.000000 django-deovi-0.6.1/django_deovi/factories/media.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1838 2022-01-22 01:32:29.000000 django-deovi-0.6.1/django_deovi/factories/user.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)    14459 2023-08-16 21:41:47.000000 django-deovi-0.6.1/django_deovi/loader.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-11-06 00:46:16.238878 django-deovi-0.6.1/django_deovi/management/
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-11-06 00:46:16.242878 django-deovi-0.6.1/django_deovi/management/commands/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2022-08-28 00:57:38.000000 django-deovi-0.6.1/django_deovi/management/commands/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1943 2023-08-16 21:41:47.000000 django-deovi-0.6.1/django_deovi/management/commands/load_medias.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-11-06 00:46:16.242878 django-deovi-0.6.1/django_deovi/migrations/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     4538 2022-09-01 01:11:10.000000 django-deovi-0.6.1/django_deovi/migrations/0001_initial.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     3473 2023-08-16 21:41:47.000000 django-deovi-0.6.1/django_deovi/migrations/0002_alter_directory_options_alter_mediafile_options_and_more.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2022-08-30 01:37:59.000000 django-deovi-0.6.1/django_deovi/migrations/__init__.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-11-06 00:46:16.246878 django-deovi-0.6.1/django_deovi/models/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      153 2022-09-01 01:11:10.000000 django-deovi-0.6.1/django_deovi/models/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     4375 2023-08-16 21:41:47.000000 django-deovi-0.6.1/django_deovi/models/device.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     7440 2023-08-16 21:41:47.000000 django-deovi-0.6.1/django_deovi/models/directory.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     4911 2023-08-16 21:41:47.000000 django-deovi-0.6.1/django_deovi/models/media.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1663 2023-08-16 21:41:47.000000 django-deovi-0.6.1/django_deovi/outputs.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      237 2022-08-28 00:57:38.000000 django-deovi-0.6.1/django_deovi/routers.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-11-06 00:46:16.246878 django-deovi-0.6.1/django_deovi/serializers/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)       82 2022-08-28 00:57:38.000000 django-deovi-0.6.1/django_deovi/serializers/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      652 2022-09-01 01:11:10.000000 django-deovi-0.6.1/django_deovi/serializers/media.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      568 2023-08-16 21:41:47.000000 django-deovi-0.6.1/django_deovi/settings.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-11-06 00:46:16.238878 django-deovi-0.6.1/django_deovi/templates/
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-11-06 00:46:16.246878 django-deovi-0.6.1/django_deovi/templates/django_deovi/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      128 2022-09-12 22:58:38.000000 django-deovi-0.6.1/django_deovi/templates/django_deovi/base.html
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-11-06 00:46:16.246878 django-deovi-0.6.1/django_deovi/templates/django_deovi/device/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1598 2023-08-16 21:41:47.000000 django-deovi-0.6.1/django_deovi/templates/django_deovi/device/_tree-item.html
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     5053 2023-08-16 21:41:47.000000 django-deovi-0.6.1/django_deovi/templates/django_deovi/device/detail.html
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     3073 2022-09-12 22:58:38.000000 django-deovi-0.6.1/django_deovi/templates/django_deovi/device/index.html
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     6457 2023-08-16 21:41:47.000000 django-deovi-0.6.1/django_deovi/templates/django_deovi/device/tree.html
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-11-06 00:46:16.246878 django-deovi-0.6.1/django_deovi/templates/django_deovi/directory/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     6405 2023-08-16 21:41:47.000000 django-deovi-0.6.1/django_deovi/templates/django_deovi/directory/detail.html
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      292 2022-08-28 00:57:38.000000 django-deovi-0.6.1/django_deovi/templates/django_deovi/mediafile_detail.html
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      557 2022-09-12 22:58:38.000000 django-deovi-0.6.1/django_deovi/templates/django_deovi/pagination.html
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-11-06 00:46:16.246878 django-deovi-0.6.1/django_deovi/templatetags/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2022-09-12 22:58:38.000000 django-deovi-0.6.1/django_deovi/templatetags/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      444 2023-08-16 21:41:47.000000 django-deovi-0.6.1/django_deovi/templatetags/deovi.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      790 2023-08-16 21:41:47.000000 django-deovi-0.6.1/django_deovi/urls.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-11-06 00:46:16.246878 django-deovi-0.6.1/django_deovi/utils/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2023-08-16 21:41:47.000000 django-deovi-0.6.1/django_deovi/utils/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)    13246 2023-08-16 21:41:47.000000 django-deovi-0.6.1/django_deovi/utils/imaging.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     6295 2023-08-16 21:41:47.000000 django-deovi-0.6.1/django_deovi/utils/tests.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1039 2023-08-16 21:41:47.000000 django-deovi-0.6.1/django_deovi/utils/tree.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-11-06 00:46:16.246878 django-deovi-0.6.1/django_deovi/views/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      349 2023-08-16 21:41:47.000000 django-deovi-0.6.1/django_deovi/views/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     8872 2023-08-16 21:41:47.000000 django-deovi-0.6.1/django_deovi/views/device.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     2288 2023-08-16 21:41:47.000000 django-deovi-0.6.1/django_deovi/views/directory.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      726 2023-08-16 21:41:47.000000 django-deovi-0.6.1/django_deovi/views/media.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      419 2022-09-12 22:58:38.000000 django-deovi-0.6.1/django_deovi/views/mixins.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-11-06 00:46:16.242878 django-deovi-0.6.1/django_deovi.egg-info/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1478 2023-11-06 00:46:16.000000 django-deovi-0.6.1/django_deovi.egg-info/PKG-INFO
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     2018 2023-11-06 00:46:16.000000 django-deovi-0.6.1/django_deovi.egg-info/SOURCES.txt
--rw-rw-r--   0 emencia   (1001) emencia   (1001)        1 2023-11-06 00:46:16.000000 django-deovi-0.6.1/django_deovi.egg-info/dependency_links.txt
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      264 2023-11-06 00:46:16.000000 django-deovi-0.6.1/django_deovi.egg-info/requires.txt
--rw-rw-r--   0 emencia   (1001) emencia   (1001)       21 2023-11-06 00:46:16.000000 django-deovi-0.6.1/django_deovi.egg-info/top_level.txt
--rw-rw-r--   0 emencia   (1001) emencia   (1001)        1 2023-08-14 14:08:52.000000 django-deovi-0.6.1/django_deovi.egg-info/zip-safe
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1604 2023-11-06 00:46:16.250878 django-deovi-0.6.1/setup.cfg
--rw-rw-r--   0 emencia   (1001) emencia   (1001)       84 2022-01-22 01:32:29.000000 django-deovi-0.6.1/setup.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2024-05-01 20:42:59.946226 django-deovi-0.6.2/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1070 2022-01-22 01:32:29.000000 django-deovi-0.6.2/LICENCE.txt
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      289 2023-11-06 00:43:37.000000 django-deovi-0.6.2/MANIFEST.in
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1528 2024-05-01 20:42:59.946226 django-deovi-0.6.2/PKG-INFO
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      647 2024-05-01 20:42:48.000000 django-deovi-0.6.2/README.rst
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2024-05-01 20:42:59.938226 django-deovi-0.6.2/django_deovi/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      705 2022-08-28 00:57:38.000000 django-deovi-0.6.2/django_deovi/__init__.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2024-05-01 20:42:59.938226 django-deovi-0.6.2/django_deovi/admin/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      183 2022-09-01 01:11:10.000000 django-deovi-0.6.2/django_deovi/admin/__init__.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      327 2024-05-01 20:42:48.000000 django-deovi-0.6.2/django_deovi/admin/device.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      437 2024-05-01 20:42:48.000000 django-deovi-0.6.2/django_deovi/admin/directory.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      402 2024-05-01 20:42:48.000000 django-deovi-0.6.2/django_deovi/admin/media.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      187 2022-01-22 01:32:29.000000 django-deovi-0.6.2/django_deovi/apps.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     5587 2024-05-01 20:42:48.000000 django-deovi-0.6.2/django_deovi/dump.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      418 2022-08-28 00:57:38.000000 django-deovi-0.6.2/django_deovi/exceptions.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2024-05-01 20:42:59.942226 django-deovi-0.6.2/django_deovi/factories/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      305 2022-09-01 01:11:10.000000 django-deovi-0.6.2/django_deovi/factories/__init__.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      382 2024-05-01 20:42:48.000000 django-deovi-0.6.2/django_deovi/factories/device.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1237 2023-08-16 21:41:47.000000 django-deovi-0.6.2/django_deovi/factories/directory.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     2977 2023-08-16 21:41:47.000000 django-deovi-0.6.2/django_deovi/factories/dump.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     2184 2023-08-16 21:41:47.000000 django-deovi-0.6.2/django_deovi/factories/media.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1838 2022-01-22 01:32:29.000000 django-deovi-0.6.2/django_deovi/factories/user.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)    16285 2024-05-01 20:42:48.000000 django-deovi-0.6.2/django_deovi/loader.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2024-05-01 20:42:59.934226 django-deovi-0.6.2/django_deovi/management/
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2024-05-01 20:42:59.942226 django-deovi-0.6.2/django_deovi/management/commands/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2022-08-28 00:57:38.000000 django-deovi-0.6.2/django_deovi/management/commands/__init__.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1943 2024-03-31 20:55:51.000000 django-deovi-0.6.2/django_deovi/management/commands/load_medias.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2024-05-01 20:42:59.942226 django-deovi-0.6.2/django_deovi/migrations/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     4538 2022-09-01 01:11:10.000000 django-deovi-0.6.2/django_deovi/migrations/0001_initial.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     3473 2023-08-16 21:41:47.000000 django-deovi-0.6.2/django_deovi/migrations/0002_alter_directory_options_alter_mediafile_options_and_more.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      580 2024-05-01 20:42:48.000000 django-deovi-0.6.2/django_deovi/migrations/0003_device_last_update.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1370 2024-05-01 20:42:48.000000 django-deovi-0.6.2/django_deovi/migrations/0004_add_device_disk_usage_fields.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2022-08-30 01:37:59.000000 django-deovi-0.6.2/django_deovi/migrations/__init__.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2024-05-01 20:42:59.942226 django-deovi-0.6.2/django_deovi/models/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      153 2022-09-01 01:11:10.000000 django-deovi-0.6.2/django_deovi/models/__init__.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     6427 2024-05-01 20:42:48.000000 django-deovi-0.6.2/django_deovi/models/device.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     7440 2023-08-16 21:41:47.000000 django-deovi-0.6.2/django_deovi/models/directory.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     4911 2023-08-16 21:41:47.000000 django-deovi-0.6.2/django_deovi/models/media.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1663 2023-08-16 21:41:47.000000 django-deovi-0.6.2/django_deovi/outputs.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      237 2022-08-28 00:57:38.000000 django-deovi-0.6.2/django_deovi/routers.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2024-05-01 20:42:59.942226 django-deovi-0.6.2/django_deovi/serializers/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)       82 2022-08-28 00:57:38.000000 django-deovi-0.6.2/django_deovi/serializers/__init__.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      652 2022-09-01 01:11:10.000000 django-deovi-0.6.2/django_deovi/serializers/media.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      703 2024-05-01 20:42:48.000000 django-deovi-0.6.2/django_deovi/settings.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2024-05-01 20:42:59.934226 django-deovi-0.6.2/django_deovi/templates/
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2024-05-01 20:42:59.942226 django-deovi-0.6.2/django_deovi/templates/django_deovi/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      128 2022-09-12 22:58:38.000000 django-deovi-0.6.2/django_deovi/templates/django_deovi/base.html
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2024-05-01 20:42:59.942226 django-deovi-0.6.2/django_deovi/templates/django_deovi/device/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1117 2024-05-01 20:42:48.000000 django-deovi-0.6.2/django_deovi/templates/django_deovi/device/_occupancy.svg
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1598 2023-08-16 21:41:47.000000 django-deovi-0.6.2/django_deovi/templates/django_deovi/device/_tree-item.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     6135 2024-05-01 20:42:48.000000 django-deovi-0.6.2/django_deovi/templates/django_deovi/device/detail.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     3260 2024-05-01 20:42:48.000000 django-deovi-0.6.2/django_deovi/templates/django_deovi/device/index.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     6927 2024-05-01 20:42:48.000000 django-deovi-0.6.2/django_deovi/templates/django_deovi/device/tree.html
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2024-05-01 20:42:59.942226 django-deovi-0.6.2/django_deovi/templates/django_deovi/directory/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     6405 2023-08-16 21:41:47.000000 django-deovi-0.6.2/django_deovi/templates/django_deovi/directory/detail.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      292 2022-08-28 00:57:38.000000 django-deovi-0.6.2/django_deovi/templates/django_deovi/mediafile_detail.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      557 2022-09-12 22:58:38.000000 django-deovi-0.6.2/django_deovi/templates/django_deovi/pagination.html
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2024-05-01 20:42:59.942226 django-deovi-0.6.2/django_deovi/templatetags/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2022-09-12 22:58:38.000000 django-deovi-0.6.2/django_deovi/templatetags/__init__.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     2084 2024-05-01 20:42:48.000000 django-deovi-0.6.2/django_deovi/templatetags/deovi.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      790 2023-08-16 21:41:47.000000 django-deovi-0.6.2/django_deovi/urls.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2024-05-01 20:42:59.946226 django-deovi-0.6.2/django_deovi/utils/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2023-08-16 21:41:47.000000 django-deovi-0.6.2/django_deovi/utils/__init__.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      690 2024-05-01 20:42:48.000000 django-deovi-0.6.2/django_deovi/utils/formatters.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)    13246 2023-08-16 21:41:47.000000 django-deovi-0.6.2/django_deovi/utils/imaging.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     6295 2023-08-16 21:41:47.000000 django-deovi-0.6.2/django_deovi/utils/tests.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1039 2023-08-16 21:41:47.000000 django-deovi-0.6.2/django_deovi/utils/tree.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2024-05-01 20:42:59.946226 django-deovi-0.6.2/django_deovi/views/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      349 2023-08-16 21:41:47.000000 django-deovi-0.6.2/django_deovi/views/__init__.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)    10317 2024-05-01 20:42:48.000000 django-deovi-0.6.2/django_deovi/views/device.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     2288 2023-08-16 21:41:47.000000 django-deovi-0.6.2/django_deovi/views/directory.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      726 2023-08-16 21:41:47.000000 django-deovi-0.6.2/django_deovi/views/media.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      419 2022-09-12 22:58:38.000000 django-deovi-0.6.2/django_deovi/views/mixins.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2024-05-01 20:42:59.938226 django-deovi-0.6.2/django_deovi.egg-info/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1528 2024-05-01 20:42:59.000000 django-deovi-0.6.2/django_deovi.egg-info/PKG-INFO
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     2221 2024-05-01 20:42:59.000000 django-deovi-0.6.2/django_deovi.egg-info/SOURCES.txt
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)        1 2024-05-01 20:42:59.000000 django-deovi-0.6.2/django_deovi.egg-info/dependency_links.txt
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      272 2024-05-01 20:42:59.000000 django-deovi-0.6.2/django_deovi.egg-info/requires.txt
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)       21 2024-05-01 20:42:59.000000 django-deovi-0.6.2/django_deovi.egg-info/top_level.txt
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)        1 2023-08-14 14:08:52.000000 django-deovi-0.6.2/django_deovi.egg-info/zip-safe
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1612 2024-05-01 20:42:59.946226 django-deovi-0.6.2/setup.cfg
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)       84 2022-01-22 01:32:29.000000 django-deovi-0.6.2/setup.py
```

### Comparing `django-deovi-0.6.1/LICENCE.txt` & `django-deovi-0.6.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `django-deovi-0.6.1/PKG-INFO` & `django-deovi-0.6.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-deovi
-Version: 0.6.1
+Version: 0.6.2
 Summary: A Django application around Deovi
 Home-page: https://github.com/sveetch/django-deovi
 Author: David Thenon
 Author-email: sveetch@gmail.com
 License: MIT
 Keywords: Python Django
 Classifier: Development Status :: 5 - Production/Stable
@@ -24,27 +24,33 @@
 Provides-Extra: doc
 Provides-Extra: release
 License-File: LICENCE.txt
 
 .. _Python: https://www.python.org/
 .. _Django: https://www.djangoproject.com/
 .. _Django REST framework: https://www.django-rest-framework.org/
+.. _bigtree: https://bigtree.readthedocs.io/
+.. _Deovi: https://deovi.readthedocs.io/
+
 
 ============
 Django Deovi
 ============
 
-A Django application around Deovi
+A Django interface to load `Deovi`_ dumps and browse data.
+
 
 Dependancies
 ************
 
 * `Python`_>=3.8;
 * `Django`_>=4.0;
 * `Django REST framework`_>=3.13.0;
+* `bigtree`_>=0.10.3;
+* `Deovi`_>=0.7.0;
+
 
 Links
 *****
 
-* (Not yet) Read the documentation on `Read the docs <https://django-deovi.readthedocs.io/>`_;
-* (Not yet) Download its `PyPi package <https://pypi.python.org/pypi/django-deovi>`_;
+* Download its `PyPi package <https://pypi.python.org/pypi/django-deovi>`_;
 * Clone it on its `Github repository <https://github.com/sveetch/django-deovi>`_;
```

### Comparing `django-deovi-0.6.1/README.rst` & `django-deovi-0.6.2/README.rst`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 .. _Python: https://www.python.org/
 .. _Django: https://www.djangoproject.com/
 .. _Django REST framework: https://www.django-rest-framework.org/
+.. _bigtree: https://bigtree.readthedocs.io/
+.. _Deovi: https://deovi.readthedocs.io/
+
 
 ============
 Django Deovi
 ============
 
-A Django application around Deovi
+A Django interface to load `Deovi`_ dumps and browse data.
+
 
 Dependancies
 ************
 
 * `Python`_>=3.8;
 * `Django`_>=4.0;
 * `Django REST framework`_>=3.13.0;
+* `bigtree`_>=0.10.3;
+* `Deovi`_>=0.7.0;
+
 
 Links
 *****
 
-* (Not yet) Read the documentation on `Read the docs <https://django-deovi.readthedocs.io/>`_;
-* (Not yet) Download its `PyPi package <https://pypi.python.org/pypi/django-deovi>`_;
+* Download its `PyPi package <https://pypi.python.org/pypi/django-deovi>`_;
 * Clone it on its `Github repository <https://github.com/sveetch/django-deovi>`_;
```

### Comparing `django-deovi-0.6.1/django_deovi/__init__.py` & `django-deovi-0.6.2/django_deovi/__init__.py`

 * *Files identical despite different names*

### Comparing `django-deovi-0.6.1/django_deovi/dump.py` & `django-deovi-0.6.2/django_deovi/dump.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,15 @@
         return {
             item: getattr(self, item)
             for item in self.FIELDNAMES
         }
 
     def _convert_type(self, modelname, value):
         """
-        Should convert value type to the right one according to the field.
+        Convert value type to the right one according to the field.
 
         stored_date
             If a string it will be converted to a datetime else it is assumed to
             already be a datetime object. Finally the returned datetime will be
             timezone aware, if the source already have it, it will stay unchanged else
             the default timezone (as from Django settings) will be added.
```

### Comparing `django-deovi-0.6.1/django_deovi/factories/directory.py` & `django-deovi-0.6.2/django_deovi/factories/directory.py`

 * *Files identical despite different names*

### Comparing `django-deovi-0.6.1/django_deovi/factories/dump.py` & `django-deovi-0.6.2/django_deovi/factories/dump.py`

 * *Files identical despite different names*

### Comparing `django-deovi-0.6.1/django_deovi/factories/media.py` & `django-deovi-0.6.2/django_deovi/factories/media.py`

 * *Files identical despite different names*

### Comparing `django-deovi-0.6.1/django_deovi/factories/user.py` & `django-deovi-0.6.2/django_deovi/factories/user.py`

 * *Files identical despite different names*

### Comparing `django-deovi-0.6.1/django_deovi/loader.py` & `django-deovi-0.6.2/django_deovi/loader.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 ==================
 
 """
 import json
 
 from pathlib import Path
 
+from django.core.exceptions import ValidationError
 from django.core.files import File
+from django.core.validators import validate_slug
 from django.utils import timezone
 
 from .dump import DumpedFile
 from .models import Device, Directory, MediaFile
 from .outputs import BaseOutput
 
 
@@ -338,14 +340,47 @@
                 self.edit_files(to_edit, batch_date=batch_date)
 
             if len(to_create) > 0 or len(to_edit) > 0:
                 saved.append((directory, created))
 
         return saved
 
+    def set_device_stats(self, device, stats):
+        """
+        Set device disk usage values.
+
+        This will try to no update the device if no usage values have changed to avoid
+        triggering ``Device.last_update`` date change.
+
+        Arguments:
+            device (django_deovi.models.Device): Device object to update.
+            stats (dict): Dictionnary of disk usage items from dump.
+
+        Returns:
+            bool: True if device has been updated else False.
+        """
+        changed = False
+
+        if device.disk_total != stats["total"]:
+            device.disk_total = stats["total"]
+            changed = True
+
+        if device.disk_used != stats["used"]:
+            device.disk_used = stats["used"]
+            changed = True
+
+        if device.disk_free != stats["free"]:
+            device.disk_free = stats["free"]
+            changed = True
+
+        if changed:
+            device.save()
+
+        return changed
+
     def load(self, device_slug, dump, covers_basepath=None):
         """
         Load a Deovi dump to create and update MediaFile objects for the dump directory
         and files.
 
         Arguments:
             device_slug (string): Slug name for the Device object to attach all the
@@ -354,23 +389,44 @@
 
         Keyword Arguments:
             covers_basepath (pathlib.Path): A path object to use to resolve cover
                 filepath. If empty, the current working directory is used. Finally
                 every cover files paths are resolved from this base dir.
         """
         self.log.info("🏷️Using device slug: {}".format(device_slug))
+
+        try:
+            validate_slug(device_slug)
+        except ValidationError as e:
+            self.log.critical("Invalid device slug: {}".format("; ".join(e)))
+
+        # Get existing device from slug if any else create a new one using slug as the
+        # default title
         device, created = Device.objects.get_or_create(
             slug=device_slug,
+            defaults={"title": device_slug},
         )
 
         if created:
             msg = "- New device created for given slug"
         else:
             msg = "- Got an existing device for given slug"
         self.log.debug(msg)
 
         covers_basepath = covers_basepath or Path.cwd()
         self.log.info("🏷️Using cover basepath: {}".format(covers_basepath))
 
-        dump_content = self.open_dump(dump)
+        dump_payload = self.open_dump(dump)
+        try:
+            device_stats = dump_payload["device"]
+            registry = dump_payload["registry"]
+        except KeyError:
+            self.log.critical(
+                "The JSON dump structure does not fit to Deovi>=0.7.0, it must "
+                "have a 'device' and 'registry'."
+            )
+
+        # Update device with disk usage
+        self.set_device_stats(device, device_stats)
 
-        self.process_directory(device, dump_content, covers_basepath)
+        # Go collecting into device directories
+        self.process_directory(device, registry, covers_basepath)
```

### Comparing `django-deovi-0.6.1/django_deovi/management/commands/load_medias.py` & `django-deovi-0.6.2/django_deovi/management/commands/load_medias.py`

 * *Files identical despite different names*

### Comparing `django-deovi-0.6.1/django_deovi/migrations/0001_initial.py` & `django-deovi-0.6.2/django_deovi/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-deovi-0.6.1/django_deovi/migrations/0002_alter_directory_options_alter_mediafile_options_and_more.py` & `django-deovi-0.6.2/django_deovi/migrations/0002_alter_directory_options_alter_mediafile_options_and_more.py`

 * *Files identical despite different names*

### Comparing `django-deovi-0.6.1/django_deovi/models/device.py` & `django-deovi-0.6.2/django_deovi/models/device.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,25 @@
+from django.core.validators import MinValueValidator
 from django.db import models
 from django.utils import timezone
 from django.utils.translation import gettext_lazy as _
 from django.urls import reverse
 
 from bigtree import dict_to_tree, tree_to_nested_dict
 
 from ..utils.tree import DirectoryInfosNode
 
 
 class Device(models.Model):
     """
     A device container to hold Directory objects.
+
+    Even through it is called a device (because it is should be the common usage), it
+    may be a simple directory path, therefore the disk usage will not be accurate to
+    the path itself.
     """
     title = models.CharField(
         _("title"),
         max_length=150,
         default="",
     )
     """
@@ -29,23 +34,75 @@
             "Used to build the URL and as an argument to the loader command."
         ),
     )
     """
     Required unique slug string.
     """
 
+    disk_total = models.BigIntegerField(
+        _("filesize"),
+        blank=False,
+        default=0,
+        validators=[MinValueValidator(0)],
+        help_text="Total available disk size of which the device belong to.",
+    )
+    """
+    Required file size integer.
+    """
+
+    disk_used = models.BigIntegerField(
+        _("filesize"),
+        blank=False,
+        default=0,
+        validators=[MinValueValidator(0)],
+        help_text=(
+            "Total used disk size of which the device belong to. This will includes"
+            "the device size and everything else that belong onto the same disk."
+        ),
+    )
+    """
+    Required file size integer.
+    """
+
+    disk_free = models.BigIntegerField(
+        _("filesize"),
+        blank=False,
+        default=0,
+        validators=[MinValueValidator(0)],
+        help_text=(
+            "Free space size on disk of which the device belong to. This will be"
+            "computed from the device size and everything else that belong onto the "
+            "same disk."
+        ),
+    )
+    """
+    Required file size integer.
+    """
+
     created_date = models.DateTimeField(
         _("created date"),
         db_index=True,
         default=timezone.now,
     )
     """
     Required datetime for when the file has been loaded.
     """
 
+    last_update = models.DateTimeField(
+        _("last update"),
+        db_index=True,
+        default=timezone.now,
+        help_text=_(
+            "The last update date for this device."
+        ),
+    )
+    """
+    Last device change date.
+    """
+
     COMMON_ORDER_BY = ["title"]
     """
     List of field order commonly used in frontend view/api
     """
 
     class Meta:
         verbose_name = _("Device")
@@ -84,14 +141,21 @@
         last_media_update = sorted([item.last_media_update for item in directories])
         if last_media_update:
             last_media_update = last_media_update[-1]
         else:
             last_media_update = None
 
         return {
+            "disk_total": self.disk_total,
+            "disk_used": self.disk_used,
+            "disk_free": self.disk_free,
+            "disk_occupancy": (
+                (self.disk_used / self.disk_total) * 100
+                if self.disk_total else 0.0
+            ),
             "directories": len(directories),
             "mediafiles": sum([item.num_mediafiles for item in directories]),
             "filesize": sum([item.total_filesize for item in directories]),
             "last_media_update": last_media_update,
         }
 
     def get_directory_tree(self):
@@ -135,7 +199,13 @@
         return tree_to_nested_dict(tree, attr_dict={
             "filepath": "filepath",
             "total_files": "total_files",
             "total_filesize": "total_filesize",
             "recursive_files": "recursive_files",
             "recursive_filesize": "recursive_filesize",
         })
+
+    def save(self, *args, **kwargs):
+        # Auto update 'last_update' value on each save
+        self.last_update = timezone.now()
+
+        super().save(*args, **kwargs)
```

### Comparing `django-deovi-0.6.1/django_deovi/models/directory.py` & `django-deovi-0.6.2/django_deovi/models/directory.py`

 * *Files identical despite different names*

### Comparing `django-deovi-0.6.1/django_deovi/models/media.py` & `django-deovi-0.6.2/django_deovi/models/media.py`

 * *Files identical despite different names*

### Comparing `django-deovi-0.6.1/django_deovi/outputs.py` & `django-deovi-0.6.2/django_deovi/outputs.py`

 * *Files identical despite different names*

### Comparing `django-deovi-0.6.1/django_deovi/serializers/media.py` & `django-deovi-0.6.2/django_deovi/serializers/media.py`

 * *Files identical despite different names*

### Comparing `django-deovi-0.6.1/django_deovi/templates/django_deovi/device/_tree-item.html` & `django-deovi-0.6.2/django_deovi/templates/django_deovi/device/_tree-item.html`

 * *Files identical despite different names*

### Comparing `django-deovi-0.6.1/django_deovi/templates/django_deovi/device/detail.html` & `django-deovi-0.6.2/django_deovi/templates/django_deovi/device/detail.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,316 +1,384 @@
 00000000: 7b25 2065 7874 656e 6473 2022 646a 616e  {% extends "djan
 00000010: 676f 5f64 656f 7669 2f62 6173 652e 6874  go_deovi/base.ht
 00000020: 6d6c 2220 257d 0a7b 2520 6c6f 6164 2069  ml" %}.{% load i
 00000030: 3138 6e20 736d 6172 745f 696d 6167 6520  18n smart_image 
-00000040: 257d 0a0a 7b25 2062 6c6f 636b 2068 6561  %}..{% block hea
-00000050: 645f 7469 746c 6520 257d 7b7b 2064 6576  d_title %}{{ dev
-00000060: 6963 655f 6f62 6a65 6374 207d 7d20 2d20  ice_object }} - 
-00000070: 7b7b 2062 6c6f 636b 2e73 7570 6572 207d  {{ block.super }
-00000080: 7d7b 2520 656e 6462 6c6f 636b 2068 6561  }{% endblock hea
-00000090: 645f 7469 746c 6520 257d 0a0a 7b25 2062  d_title %}..{% b
-000000a0: 6c6f 636b 2061 7070 5f63 6f6e 7465 6e74  lock app_content
-000000b0: 2025 7d7b 2520 7370 6163 656c 6573 7320   %}{% spaceless 
-000000c0: 257d 0a3c 6469 7620 636c 6173 733d 2264  %}.<div class="d
-000000d0: 6576 6963 652d 6465 7461 696c 223e 0a20  evice-detail">. 
-000000e0: 2020 203c 6469 7620 636c 6173 733d 2264     <div class="d
-000000f0: 6576 6963 652d 6465 7461 696c 5f5f 6865  evice-detail__he
-00000100: 6164 223e 0a20 2020 2020 2020 203c 6832  ad">.        <h2
-00000110: 2063 6c61 7373 3d22 6465 7669 6365 2d64   class="device-d
-00000120: 6574 6169 6c5f 5f74 6974 6c65 223e 7b7b  etail__title">{{
-00000130: 2064 6576 6963 655f 6f62 6a65 6374 207d   device_object }
-00000140: 7d3c 2f68 323e 0a20 2020 2020 2020 207b  }</h2>.        {
-00000150: 2520 7769 7468 2064 6576 6963 655f 6f62  % with device_ob
-00000160: 6a65 6374 2e72 6573 756d 6520 6173 2072  ject.resume as r
-00000170: 6573 756d 6520 257d 0a20 2020 2020 2020  esume %}.       
-00000180: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-00000190: 2264 6576 6963 652d 6465 7461 696c 5f5f  "device-detail__
-000001a0: 7374 6174 7320 7374 6174 7322 3e0a 2020  stats stats">.  
-000001b0: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-000001c0: 6976 2063 6c61 7373 3d22 7374 6174 735f  iv class="stats_
-000001d0: 5f63 656c 6c22 3e0a 2020 2020 2020 2020  _cell">.        
-000001e0: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
-000001f0: 3e3c 6920 636c 6173 733d 2268 3520 6269  ><i class="h5 bi
-00000200: 2062 692d 6261 722d 6368 6172 742d 6669   bi-bar-chart-fi
-00000210: 6c6c 223e 3c2f 693e 3c2f 6469 763e 0a20  ll"></i></div>. 
-00000220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000230: 2020 203c 6469 763e 3c73 6d61 6c6c 2063     <div><small c
-00000240: 6c61 7373 3d22 7465 7874 2d6d 7574 6564  lass="text-muted
-00000250: 2073 6d2d 3220 6677 2d6e 6f72 6d61 6c22   sm-2 fw-normal"
-00000260: 3e7b 2520 7472 616e 7320 2254 6f74 616c  >{% trans "Total
-00000270: 2073 697a 6522 2025 7d3c 2f73 6d61 6c6c   size" %}</small
-00000280: 3e3c 2f64 6976 3e0a 2020 2020 2020 2020  ></div>.        
-00000290: 2020 2020 2020 2020 2020 2020 3c68 3320              <h3 
-000002a0: 636c 6173 733d 2266 772d 626f 6c64 206d  class="fw-bold m
-000002b0: 622d 3020 6673 2d35 223e 7b7b 2072 6573  b-0 fs-5">{{ res
-000002c0: 756d 652e 6669 6c65 7369 7a65 7c66 696c  ume.filesize|fil
-000002d0: 6573 697a 6566 6f72 6d61 7420 7d7d 3c2f  esizeformat }}</
-000002e0: 6833 3e0a 2020 2020 2020 2020 2020 2020  h3>.            
-000002f0: 2020 2020 3c2f 6469 763e 0a20 2020 2020      </div>.     
-00000300: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
-00000310: 636c 6173 733d 2273 7461 7473 5f5f 6365  class="stats__ce
-00000320: 6c6c 223e 0a20 2020 2020 2020 2020 2020  ll">.           
-00000330: 2020 2020 2020 2020 203c 6469 763e 3c69           <div><i
-00000340: 2063 6c61 7373 3d22 6835 2062 6920 6269   class="h5 bi bi
-00000350: 2d66 6f6c 6465 7222 3e3c 2f69 3e3c 2f64  -folder"></i></d
-00000360: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
-00000370: 2020 2020 2020 2020 3c64 6976 3e3c 736d          <div><sm
-00000380: 616c 6c20 636c 6173 733d 2274 6578 742d  all class="text-
-00000390: 6d75 7465 6420 736d 2d32 2066 772d 6e6f  muted sm-2 fw-no
-000003a0: 726d 616c 223e 7b25 2074 7261 6e73 2022  rmal">{% trans "
-000003b0: 4469 7265 6374 6f72 6965 7322 2025 7d3c  Directories" %}<
-000003c0: 2f73 6d61 6c6c 3e3c 2f64 6976 3e0a 2020  /small></div>.  
-000003d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000003e0: 2020 3c68 3320 636c 6173 733d 2266 772d    <h3 class="fw-
-000003f0: 626f 6c64 206d 622d 3020 6673 2d35 223e  bold mb-0 fs-5">
-00000400: 7b7b 2072 6573 756d 652e 6469 7265 6374  {{ resume.direct
-00000410: 6f72 6965 7320 7d7d 3c2f 6833 3e0a 2020  ories }}</h3>.  
-00000420: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-00000430: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
-00000440: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-00000450: 2273 7461 7473 5f5f 6365 6c6c 223e 0a20  "stats__cell">. 
-00000460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000470: 2020 203c 6469 763e 3c69 2063 6c61 7373     <div><i class
-00000480: 3d22 6835 2062 6920 6269 2d66 696c 6d22  ="h5 bi bi-film"
-00000490: 3e3c 2f69 3e3c 2f64 6976 3e0a 2020 2020  ></i></div>.    
-000004a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000004b0: 3c64 6976 3e3c 736d 616c 6c20 636c 6173  <div><small clas
-000004c0: 733d 2274 6578 742d 6d75 7465 6420 736d  s="text-muted sm
-000004d0: 2d32 2066 772d 6e6f 726d 616c 223e 7b25  -2 fw-normal">{%
-000004e0: 2074 7261 6e73 2022 4d65 6469 6173 2220   trans "Medias" 
-000004f0: 257d 3c2f 736d 616c 6c3e 3c2f 6469 763e  %}</small></div>
-00000500: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000510: 2020 2020 203c 6833 2063 6c61 7373 3d22       <h3 class="
-00000520: 6677 2d62 6f6c 6420 6d62 2d30 2066 732d  fw-bold mb-0 fs-
-00000530: 3522 3e7b 7b20 7265 7375 6d65 2e6d 6564  5">{{ resume.med
-00000540: 6961 6669 6c65 7320 7d7d 3c2f 6833 3e0a  iafiles }}</h3>.
-00000550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000560: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
-00000570: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-00000580: 733d 2273 7461 7473 5f5f 6365 6c6c 223e  s="stats__cell">
-00000590: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000005a0: 2020 2020 203c 6469 763e 3c69 2063 6c61       <div><i cla
-000005b0: 7373 3d22 6835 2062 6920 6269 2d62 616c  ss="h5 bi bi-bal
-000005c0: 6c6f 6f6e 223e 3c2f 693e 3c2f 6469 763e  loon"></i></div>
-000005d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000005e0: 2020 2020 203c 6469 763e 3c73 6d61 6c6c       <div><small
-000005f0: 2063 6c61 7373 3d22 7465 7874 2d6d 7574   class="text-mut
-00000600: 6564 2073 6d2d 3220 6677 2d6e 6f72 6d61  ed sm-2 fw-norma
-00000610: 6c22 3e7b 2520 7472 616e 7320 2243 7265  l">{% trans "Cre
-00000620: 6174 6564 2220 257d 3c2f 736d 616c 6c3e  ated" %}</small>
-00000630: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
-00000640: 2020 2020 2020 2020 2020 203c 6833 2063             <h3 c
-00000650: 6c61 7373 3d22 6677 2d62 6f6c 6420 6d62  lass="fw-bold mb
-00000660: 2d30 2066 732d 3522 3e0a 2020 2020 2020  -0 fs-5">.      
-00000670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000680: 2020 3c61 6262 7220 636c 6173 733d 2274    <abbr class="t
-00000690: 6578 742d 6465 636f 7261 7469 6f6e 2d6e  ext-decoration-n
-000006a0: 6f6e 6522 2074 6974 6c65 3d22 7b7b 2064  one" title="{{ d
-000006b0: 6576 6963 655f 6f62 6a65 6374 2e63 7265  evice_object.cre
-000006c0: 6174 6564 5f64 6174 6520 7d7d 223e 0a20  ated_date }}">. 
-000006d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000006e0: 2020 2020 2020 2020 2020 207b 7b20 6465             {{ de
-000006f0: 7669 6365 5f6f 626a 6563 742e 6372 6561  vice_object.crea
-00000700: 7465 645f 6461 7465 7c64 6174 653a 2253  ted_date|date:"S
-00000710: 484f 5254 5f44 4154 455f 464f 524d 4154  HORT_DATE_FORMAT
-00000720: 2220 7d7d 0a20 2020 2020 2020 2020 2020  " }}.           
-00000730: 2020 2020 2020 2020 2020 2020 203c 2f61               </a
-00000740: 6262 723e 0a20 2020 2020 2020 2020 2020  bbr>.           
-00000750: 2020 2020 2020 2020 203c 2f68 333e 0a20           </h3>. 
-00000760: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00000770: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
-00000780: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-00000790: 3d22 7374 6174 735f 5f63 656c 6c22 3e0a  ="stats__cell">.
-000007a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000007b0: 2020 2020 3c64 6976 3e3c 6920 636c 6173      <div><i clas
-000007c0: 733d 2268 3520 6269 2062 692d 6163 7469  s="h5 bi bi-acti
-000007d0: 7669 7479 223e 3c2f 693e 3c2f 6469 763e  vity"></i></div>
-000007e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000007f0: 2020 2020 203c 6469 763e 3c73 6d61 6c6c       <div><small
-00000800: 2063 6c61 7373 3d22 7465 7874 2d6d 7574   class="text-mut
-00000810: 6564 2073 6d2d 3220 6677 2d6e 6f72 6d61  ed sm-2 fw-norma
-00000820: 6c22 3e7b 2520 7472 616e 7320 224c 6173  l">{% trans "Las
-00000830: 7420 7570 6461 7465 2220 257d 3c2f 736d  t update" %}</sm
-00000840: 616c 6c3e 3c2f 6469 763e 0a20 2020 2020  all></div>.     
-00000850: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00000860: 6833 2063 6c61 7373 3d22 6677 2d62 6f6c  h3 class="fw-bol
-00000870: 6420 6d62 2d30 2066 732d 3522 3e0a 2020  d mb-0 fs-5">.  
-00000880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000890: 2020 2020 2020 3c61 6262 7220 636c 6173        <abbr clas
-000008a0: 733d 2274 6578 742d 6465 636f 7261 7469  s="text-decorati
-000008b0: 6f6e 2d6e 6f6e 6522 2074 6974 6c65 3d22  on-none" title="
-000008c0: 7b7b 2072 6573 756d 652e 6c61 7374 5f6d  {{ resume.last_m
-000008d0: 6564 6961 5f75 7064 6174 6520 7d7d 223e  edia_update }}">
-000008e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000008f0: 2020 2020 2020 2020 2020 2020 207b 7b20               {{ 
-00000900: 7265 7375 6d65 2e6c 6173 745f 6d65 6469  resume.last_medi
-00000910: 615f 7570 6461 7465 7c64 6174 653a 2253  a_update|date:"S
-00000920: 484f 5254 5f44 4154 455f 464f 524d 4154  HORT_DATE_FORMAT
-00000930: 2220 7d7d 0a20 2020 2020 2020 2020 2020  " }}.           
-00000940: 2020 2020 2020 2020 2020 2020 203c 2f61               </a
-00000950: 6262 723e 0a20 2020 2020 2020 2020 2020  bbr>.           
-00000960: 2020 2020 2020 2020 203c 2f68 333e 0a20           </h3>. 
-00000970: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00000980: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
-00000990: 2020 3c2f 6469 763e 0a20 2020 2020 2020    </div>.       
-000009a0: 207b 2520 656e 6477 6974 6820 257d 0a20   {% endwith %}. 
-000009b0: 2020 203c 2f64 6976 3e0a 2020 2020 3c64     </div>.    <d
-000009c0: 6976 2063 6c61 7373 3d22 6465 7669 6365  iv class="device
-000009d0: 2d64 6574 6169 6c5f 5f64 6972 6563 746f  -detail__directo
-000009e0: 7269 6573 2064 6972 6563 746f 7279 2d6c  ries directory-l
-000009f0: 6973 7422 3e0a 2020 2020 2020 2020 3c64  ist">.        <d
-00000a00: 6976 2063 6c61 7373 3d22 6274 6e2d 746f  iv class="btn-to
-00000a10: 6f6c 6261 7220 772d 3130 3020 6a75 7374  olbar w-100 just
-00000a20: 6966 792d 636f 6e74 656e 742d 6265 7477  ify-content-betw
-00000a30: 6565 6e20 7062 2d32 206d 622d 3222 0a20  een pb-2 mb-2". 
-00000a40: 2020 2020 2020 2020 2020 2020 726f 6c65              role
-00000a50: 3d22 746f 6f6c 6261 7222 2061 7269 612d  ="toolbar" aria-
-00000a60: 6c61 6265 6c3d 2244 6576 6963 6520 746f  label="Device to
-00000a70: 6f6c 6261 7222 3e0a 2020 2020 2020 2020  olbar">.        
-00000a80: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-00000a90: 6274 6e2d 6772 6f75 7020 6274 6e2d 6772  btn-group btn-gr
-00000aa0: 6f75 702d 736d 2220 726f 6c65 3d22 6772  oup-sm" role="gr
-00000ab0: 6f75 7022 0a20 2020 2020 2020 2020 2020  oup".           
-00000ac0: 2020 2020 2020 6172 6961 2d6c 6162 656c        aria-label
-00000ad0: 3d22 4465 7669 6365 206e 6176 6967 6174  ="Device navigat
-00000ae0: 696f 6e22 3e0a 2020 2020 2020 2020 2020  ion">.          
-00000af0: 2020 2020 2020 3c61 2063 6c61 7373 3d22        <a class="
-00000b00: 6274 6e20 6274 6e2d 7365 636f 6e64 6172  btn btn-secondar
-00000b10: 7922 0a20 2020 2020 2020 2020 2020 2020  y".             
-00000b20: 2020 2020 2020 6872 6566 3d22 7b25 2075        href="{% u
-00000b30: 726c 2022 646a 616e 676f 5f64 656f 7669  rl "django_deovi
-00000b40: 3a64 6576 6963 652d 7472 6565 2220 6465  :device-tree" de
-00000b50: 7669 6365 5f73 6c75 673d 6465 7669 6365  vice_slug=device
-00000b60: 5f6f 626a 6563 742e 736c 7567 2025 7d22  _object.slug %}"
-00000b70: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00000b80: 2020 2020 2020 3c69 2063 6c61 7373 3d22        <i class="
-00000b90: 6269 2062 692d 666f 6c64 6572 206d 652d  bi bi-folder me-
-00000ba0: 3122 3e3c 2f69 3e0a 2020 2020 2020 2020  1"></i>.        
-00000bb0: 2020 2020 2020 2020 2020 2020 4465 7669              Devi
-00000bc0: 6365 2074 7265 650a 2020 2020 2020 2020  ce tree.        
-00000bd0: 2020 2020 2020 2020 3c2f 613e 0a20 2020          </a>.   
-00000be0: 2020 2020 2020 2020 203c 2f64 6976 3e0a           </div>.
-00000bf0: 2020 2020 2020 2020 3c2f 6469 763e 0a0a          </div>..
-00000c00: 2020 2020 2020 2020 7b25 2066 6f72 2064          {% for d
-00000c10: 6972 6563 746f 7279 5f6f 626a 6563 7420  irectory_object 
-00000c20: 696e 206f 626a 6563 745f 6c69 7374 2025  in object_list %
-00000c30: 7d0a 2020 2020 2020 2020 3c64 6976 2063  }.        <div c
-00000c40: 6c61 7373 3d22 6469 7265 6374 6f72 792d  lass="directory-
-00000c50: 6c69 7374 5f5f 6974 656d 223e 0a20 2020  list__item">.   
-00000c60: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
-00000c70: 6173 733d 2263 6172 6422 3e0a 2020 2020  ass="card">.    
-00000c80: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
-00000c90: 2063 6c61 7373 3d22 6361 7264 2d62 6f64   class="card-bod
-00000ca0: 7922 3e0a 2020 2020 2020 2020 2020 2020  y">.            
-00000cb0: 2020 2020 2020 2020 3c61 2068 7265 663d          <a href=
-00000cc0: 227b 7b20 6469 7265 6374 6f72 795f 6f62  "{{ directory_ob
-00000cd0: 6a65 6374 2e67 6574 5f61 6273 6f6c 7574  ject.get_absolut
-00000ce0: 655f 7572 6c20 7d7d 220a 2020 2020 2020  e_url }}".      
-00000cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d00: 2020 636c 6173 733d 2264 6972 6563 746f    class="directo
-00000d10: 7279 2d6c 6973 745f 5f74 6974 6c65 2073  ry-list__title s
-00000d20: 7472 6574 6368 6564 2d6c 696e 6b22 3e0a  tretched-link">.
+00000040: 6465 6f76 6920 257d 0a0a 7b25 2062 6c6f  deovi %}..{% blo
+00000050: 636b 2068 6561 645f 7469 746c 6520 257d  ck head_title %}
+00000060: 7b7b 2064 6576 6963 655f 6f62 6a65 6374  {{ device_object
+00000070: 207d 7d20 2d20 7b7b 2062 6c6f 636b 2e73   }} - {{ block.s
+00000080: 7570 6572 207d 7d7b 2520 656e 6462 6c6f  uper }}{% endblo
+00000090: 636b 2068 6561 645f 7469 746c 6520 257d  ck head_title %}
+000000a0: 0a0a 7b25 2062 6c6f 636b 2061 7070 5f63  ..{% block app_c
+000000b0: 6f6e 7465 6e74 2025 7d7b 2520 7370 6163  ontent %}{% spac
+000000c0: 656c 6573 7320 257d 0a3c 6469 7620 636c  eless %}.<div cl
+000000d0: 6173 733d 2264 6576 6963 652d 6465 7461  ass="device-deta
+000000e0: 696c 223e 0a20 2020 203c 6469 7620 636c  il">.    <div cl
+000000f0: 6173 733d 2264 6576 6963 652d 6465 7461  ass="device-deta
+00000100: 696c 5f5f 6865 6164 223e 0a20 2020 2020  il__head">.     
+00000110: 2020 203c 6832 2063 6c61 7373 3d22 6465     <h2 class="de
+00000120: 7669 6365 2d64 6574 6169 6c5f 5f74 6974  vice-detail__tit
+00000130: 6c65 223e 7b7b 2064 6576 6963 655f 6f62  le">{{ device_ob
+00000140: 6a65 6374 207d 7d3c 2f68 323e 0a20 2020  ject }}</h2>.   
+00000150: 2020 2020 207b 2520 7769 7468 2064 6576       {% with dev
+00000160: 6963 655f 6f62 6a65 6374 2e72 6573 756d  ice_object.resum
+00000170: 6520 6173 2072 6573 756d 6520 257d 0a20  e as resume %}. 
+00000180: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
+00000190: 636c 6173 733d 2264 6576 6963 652d 6465  class="device-de
+000001a0: 7461 696c 5f5f 7374 6174 7320 7374 6174  tail__stats stat
+000001b0: 7322 3e0a 2020 2020 2020 2020 2020 2020  s">.            
+000001c0: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+000001d0: 7374 6174 735f 5f63 656c 6c22 3e0a 2020  stats__cell">.  
+000001e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000001f0: 2020 3c64 6976 3e3c 6920 636c 6173 733d    <div><i class=
+00000200: 2268 3520 6269 2062 692d 6261 722d 6368  "h5 bi bi-bar-ch
+00000210: 6172 742d 6669 6c6c 223e 3c2f 693e 3c2f  art-fill"></i></
+00000220: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
+00000230: 2020 2020 2020 2020 203c 6469 763e 3c73           <div><s
+00000240: 6d61 6c6c 2063 6c61 7373 3d22 7465 7874  mall class="text
+00000250: 2d6d 7574 6564 2073 6d2d 3220 6677 2d6e  -muted sm-2 fw-n
+00000260: 6f72 6d61 6c22 3e7b 2520 7472 616e 7320  ormal">{% trans 
+00000270: 2254 6f74 616c 2066 696c 6520 7369 7a65  "Total file size
+00000280: 2220 257d 3c2f 736d 616c 6c3e 3c2f 6469  " %}</small></di
+00000290: 763e 0a20 2020 2020 2020 2020 2020 2020  v>.             
+000002a0: 2020 2020 2020 203c 6833 2063 6c61 7373         <h3 class
+000002b0: 3d22 6677 2d62 6f6c 6420 6d62 2d30 2066  ="fw-bold mb-0 f
+000002c0: 732d 3522 3e7b 7b20 7265 7375 6d65 2e66  s-5">{{ resume.f
+000002d0: 696c 6573 697a 657c 6669 6c65 7369 7a65  ilesize|filesize
+000002e0: 666f 726d 6174 207d 7d3c 2f68 333e 0a20  format }}</h3>. 
+000002f0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00000300: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
+00000310: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+00000320: 3d22 7374 6174 735f 5f63 656c 6c22 3e0a  ="stats__cell">.
+00000330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000340: 2020 2020 3c64 6976 3e3c 6920 636c 6173      <div><i clas
+00000350: 733d 2268 3520 6269 2062 692d 666f 6c64  s="h5 bi bi-fold
+00000360: 6572 223e 3c2f 693e 3c2f 6469 763e 0a20  er"></i></div>. 
+00000370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000380: 2020 203c 6469 763e 3c73 6d61 6c6c 2063     <div><small c
+00000390: 6c61 7373 3d22 7465 7874 2d6d 7574 6564  lass="text-muted
+000003a0: 2073 6d2d 3220 6677 2d6e 6f72 6d61 6c22   sm-2 fw-normal"
+000003b0: 3e7b 2520 7472 616e 7320 2244 6972 6563  >{% trans "Direc
+000003c0: 746f 7269 6573 2220 257d 3c2f 736d 616c  tories" %}</smal
+000003d0: 6c3e 3c2f 6469 763e 0a20 2020 2020 2020  l></div>.       
+000003e0: 2020 2020 2020 2020 2020 2020 203c 6833               <h3
+000003f0: 2063 6c61 7373 3d22 6677 2d62 6f6c 6420   class="fw-bold 
+00000400: 6d62 2d30 2066 732d 3522 3e7b 7b20 7265  mb-0 fs-5">{{ re
+00000410: 7375 6d65 2e64 6972 6563 746f 7269 6573  sume.directories
+00000420: 207d 7d3c 2f68 333e 0a20 2020 2020 2020   }}</h3>.       
+00000430: 2020 2020 2020 2020 203c 2f64 6976 3e0a           </div>.
+00000440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000450: 3c64 6976 2063 6c61 7373 3d22 7374 6174  <div class="stat
+00000460: 735f 5f63 656c 6c22 3e0a 2020 2020 2020  s__cell">.      
+00000470: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
+00000480: 6976 3e3c 6920 636c 6173 733d 2268 3520  iv><i class="h5 
+00000490: 6269 2062 692d 6669 6c6d 223e 3c2f 693e  bi bi-film"></i>
+000004a0: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
+000004b0: 2020 2020 2020 2020 2020 203c 6469 763e             <div>
+000004c0: 3c73 6d61 6c6c 2063 6c61 7373 3d22 7465  <small class="te
+000004d0: 7874 2d6d 7574 6564 2073 6d2d 3220 6677  xt-muted sm-2 fw
+000004e0: 2d6e 6f72 6d61 6c22 3e7b 2520 7472 616e  -normal">{% tran
+000004f0: 7320 224d 6564 6961 7322 2025 7d3c 2f73  s "Medias" %}</s
+00000500: 6d61 6c6c 3e3c 2f64 6976 3e0a 2020 2020  mall></div>.    
+00000510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000520: 3c68 3320 636c 6173 733d 2266 772d 626f  <h3 class="fw-bo
+00000530: 6c64 206d 622d 3020 6673 2d35 223e 7b7b  ld mb-0 fs-5">{{
+00000540: 2072 6573 756d 652e 6d65 6469 6166 696c   resume.mediafil
+00000550: 6573 207d 7d3c 2f68 333e 0a20 2020 2020  es }}</h3>.     
+00000560: 2020 2020 2020 2020 2020 203c 2f64 6976             </div
+00000570: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00000580: 2020 3c64 6976 2063 6c61 7373 3d22 7374    <div class="st
+00000590: 6174 735f 5f63 656c 6c22 3e0a 2020 2020  ats__cell">.    
+000005a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000005b0: 3c64 6976 3e3c 6920 636c 6173 733d 2268  <div><i class="h
+000005c0: 3520 6269 2062 692d 6261 6c6c 6f6f 6e22  5 bi bi-balloon"
+000005d0: 3e3c 2f69 3e3c 2f64 6976 3e0a 2020 2020  ></i></div>.    
+000005e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000005f0: 3c64 6976 3e3c 736d 616c 6c20 636c 6173  <div><small clas
+00000600: 733d 2274 6578 742d 6d75 7465 6420 736d  s="text-muted sm
+00000610: 2d32 2066 772d 6e6f 726d 616c 223e 7b25  -2 fw-normal">{%
+00000620: 2074 7261 6e73 2022 4372 6561 7465 6422   trans "Created"
+00000630: 2025 7d3c 2f73 6d61 6c6c 3e3c 2f64 6976   %}</small></div
+00000640: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00000650: 2020 2020 2020 3c68 3320 636c 6173 733d        <h3 class=
+00000660: 2266 772d 626f 6c64 206d 622d 3020 6673  "fw-bold mb-0 fs
+00000670: 2d35 223e 0a20 2020 2020 2020 2020 2020  -5">.           
+00000680: 2020 2020 2020 2020 2020 2020 203c 6162               <ab
+00000690: 6272 2063 6c61 7373 3d22 7465 7874 2d64  br class="text-d
+000006a0: 6563 6f72 6174 696f 6e2d 6e6f 6e65 2220  ecoration-none" 
+000006b0: 7469 746c 653d 227b 7b20 6465 7669 6365  title="{{ device
+000006c0: 5f6f 626a 6563 742e 6372 6561 7465 645f  _object.created_
+000006d0: 6461 7465 207d 7d22 3e0a 2020 2020 2020  date }}">.      
+000006e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000006f0: 2020 2020 2020 7b7b 2064 6576 6963 655f        {{ device_
+00000700: 6f62 6a65 6374 2e63 7265 6174 6564 5f64  object.created_d
+00000710: 6174 657c 6461 7465 3a22 5348 4f52 545f  ate|date:"SHORT_
+00000720: 4441 5445 5f46 4f52 4d41 5422 207d 7d0a  DATE_FORMAT" }}.
+00000730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000740: 2020 2020 2020 2020 3c2f 6162 6272 3e0a          </abbr>.
+00000750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000760: 2020 2020 3c2f 6833 3e0a 2020 2020 2020      </h3>.      
+00000770: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
+00000780: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000790: 203c 6469 7620 636c 6173 733d 2273 7461   <div class="sta
+000007a0: 7473 5f5f 6365 6c6c 223e 0a20 2020 2020  ts__cell">.     
+000007b0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+000007c0: 6469 763e 3c69 2063 6c61 7373 3d22 6835  div><i class="h5
+000007d0: 2062 6920 6269 2d61 6374 6976 6974 7922   bi bi-activity"
+000007e0: 3e3c 2f69 3e3c 2f64 6976 3e0a 2020 2020  ></i></div>.    
+000007f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000800: 3c64 6976 3e3c 736d 616c 6c20 636c 6173  <div><small clas
+00000810: 733d 2274 6578 742d 6d75 7465 6420 736d  s="text-muted sm
+00000820: 2d32 2066 772d 6e6f 726d 616c 223e 7b25  -2 fw-normal">{%
+00000830: 2074 7261 6e73 2022 4c61 7374 2075 7064   trans "Last upd
+00000840: 6174 6522 2025 7d3c 2f73 6d61 6c6c 3e3c  ate" %}</small><
+00000850: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
+00000860: 2020 2020 2020 2020 2020 3c68 3320 636c            <h3 cl
+00000870: 6173 733d 2266 772d 626f 6c64 206d 622d  ass="fw-bold mb-
+00000880: 3020 6673 2d35 223e 0a20 2020 2020 2020  0 fs-5">.       
+00000890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000008a0: 203c 6162 6272 2063 6c61 7373 3d22 7465   <abbr class="te
+000008b0: 7874 2d64 6563 6f72 6174 696f 6e2d 6e6f  xt-decoration-no
+000008c0: 6e65 2220 7469 746c 653d 227b 7b20 7265  ne" title="{{ re
+000008d0: 7375 6d65 2e6c 6173 745f 6d65 6469 615f  sume.last_media_
+000008e0: 7570 6461 7465 207d 7d22 3e0a 2020 2020  update }}">.    
+000008f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000900: 2020 2020 2020 2020 7b7b 2072 6573 756d          {{ resum
+00000910: 652e 6c61 7374 5f6d 6564 6961 5f75 7064  e.last_media_upd
+00000920: 6174 657c 6461 7465 3a22 5348 4f52 545f  ate|date:"SHORT_
+00000930: 4441 5445 5f46 4f52 4d41 5422 207d 7d0a  DATE_FORMAT" }}.
+00000940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000950: 2020 2020 2020 2020 3c2f 6162 6272 3e0a          </abbr>.
+00000960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000970: 2020 2020 3c2f 6833 3e0a 2020 2020 2020      </h3>.      
+00000980: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
+00000990: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000009a0: 203c 6469 7620 636c 6173 733d 2273 7461   <div class="sta
+000009b0: 7473 5f5f 6365 6c6c 223e 0a20 2020 2020  ts__cell">.     
+000009c0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+000009d0: 6469 763e 3c69 2063 6c61 7373 3d22 6835  div><i class="h5
+000009e0: 2062 6920 6269 2d68 6464 2d66 696c 6c22   bi bi-hdd-fill"
+000009f0: 3e3c 2f69 3e3c 2f64 6976 3e0a 2020 2020  ></i></div>.    
+00000a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a10: 3c64 6976 3e3c 736d 616c 6c20 636c 6173  <div><small clas
+00000a20: 733d 2274 6578 742d 6d75 7465 6420 736d  s="text-muted sm
+00000a30: 2d32 2066 772d 6e6f 726d 616c 223e 7b25  -2 fw-normal">{%
+00000a40: 2074 7261 6e73 2022 4469 736b 2074 6f74   trans "Disk tot
+00000a50: 616c 2220 257d 3c2f 736d 616c 6c3e 3c2f  al" %}</small></
+00000a60: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
+00000a70: 2020 2020 2020 2020 203c 6833 2063 6c61           <h3 cla
+00000a80: 7373 3d22 6677 2d62 6f6c 6420 6d62 2d30  ss="fw-bold mb-0
+00000a90: 2066 732d 3522 3e7b 7b20 7265 7375 6d65   fs-5">{{ resume
+00000aa0: 2e64 6973 6b5f 746f 7461 6c7c 6669 6c65  .disk_total|file
+00000ab0: 7369 7a65 666f 726d 6174 207d 7d3c 2f68  sizeformat }}</h
+00000ac0: 333e 0a20 2020 2020 2020 2020 2020 2020  3>.             
+00000ad0: 2020 203c 2f64 6976 3e0a 2020 2020 2020     </div>.      
+00000ae0: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+00000af0: 6c61 7373 3d22 7374 6174 735f 5f63 656c  lass="stats__cel
+00000b00: 6c22 3e0a 2020 2020 2020 2020 2020 2020  l">.            
+00000b10: 2020 2020 2020 2020 3c64 6976 3e3c 6920          <div><i 
+00000b20: 636c 6173 733d 2268 3520 6269 2062 692d  class="h5 bi bi-
+00000b30: 6864 6422 3e3c 2f69 3e3c 2f64 6976 3e0a  hdd"></i></div>.
+00000b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b50: 2020 2020 3c64 6976 3e3c 736d 616c 6c20      <div><small 
+00000b60: 636c 6173 733d 2274 6578 742d 6d75 7465  class="text-mute
+00000b70: 6420 736d 2d32 2066 772d 6e6f 726d 616c  d sm-2 fw-normal
+00000b80: 223e 7b25 2074 7261 6e73 2022 4469 736b  ">{% trans "Disk
+00000b90: 2066 7265 6522 2025 7d3c 2f73 6d61 6c6c   free" %}</small
+00000ba0: 3e3c 2f64 6976 3e0a 2020 2020 2020 2020  ></div>.        
+00000bb0: 2020 2020 2020 2020 2020 2020 3c68 3320              <h3 
+00000bc0: 636c 6173 733d 2266 772d 626f 6c64 206d  class="fw-bold m
+00000bd0: 622d 3020 6673 2d35 223e 7b7b 2072 6573  b-0 fs-5">{{ res
+00000be0: 756d 652e 6469 736b 5f66 7265 657c 6669  ume.disk_free|fi
+00000bf0: 6c65 7369 7a65 666f 726d 6174 207d 7d3c  lesizeformat }}<
+00000c00: 2f68 333e 0a20 2020 2020 2020 2020 2020  /h3>.           
+00000c10: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
+00000c20: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+00000c30: 2063 6c61 7373 3d22 7374 6174 735f 5f63   class="stats__c
+00000c40: 656c 6c22 3e0a 2020 2020 2020 2020 2020  ell">.          
+00000c50: 2020 2020 2020 2020 2020 3c64 6976 3e0a            <div>.
+00000c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c70: 2020 2020 2020 2020 7b25 2073 686f 775f          {% show_
+00000c80: 6f63 6375 7061 6e63 795f 7376 6720 6465  occupancy_svg de
+00000c90: 7669 6365 5f6f 626a 6563 7420 7265 7375  vice_object resu
+00000ca0: 6d65 3d72 6573 756d 6520 257d 0a20 2020  me=resume %}.   
+00000cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000cc0: 203c 2f64 6976 3e0a 2020 2020 2020 2020   </div>.        
+00000cd0: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+00000ce0: 3e3c 736d 616c 6c20 636c 6173 733d 2274  ><small class="t
+00000cf0: 6578 742d 6d75 7465 6420 736d 2d32 2066  ext-muted sm-2 f
+00000d00: 772d 6e6f 726d 616c 223e 7b25 2074 7261  w-normal">{% tra
+00000d10: 6e73 2022 4f63 6375 7061 6e63 7922 2025  ns "Occupancy" %
+00000d20: 7d3c 2f73 6d61 6c6c 3e3c 2f64 6976 3e0a  }</small></div>.
 00000d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d40: 2020 2020 2020 2020 7b25 2069 6620 6469          {% if di
-00000d50: 7265 6374 6f72 795f 6f62 6a65 6374 2e74  rectory_object.t
-00000d60: 6974 6c65 2025 7d0a 2020 2020 2020 2020  itle %}.        
-00000d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d80: 2020 2020 7b7b 2064 6972 6563 746f 7279      {{ directory
-00000d90: 5f6f 626a 6563 742e 7469 746c 6520 7d7d  _object.title }}
-00000da0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000db0: 2020 2020 2020 2020 207b 2520 656c 7365           {% else
-00000dc0: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
-00000dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000de0: 7b7b 2064 6972 6563 746f 7279 5f6f 626a  {{ directory_obj
-00000df0: 6563 742e 6469 7265 6374 6f72 795f 6e61  ect.directory_na
-00000e00: 6d65 207d 7d0a 2020 2020 2020 2020 2020  me }}.          
-00000e10: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
-00000e20: 2065 6e64 6966 2025 7d0a 2020 2020 2020   endif %}.      
-00000e30: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-00000e40: 613e 0a20 2020 2020 2020 2020 2020 2020  a>.             
-00000e50: 2020 203c 2f64 6976 3e0a 0a20 2020 2020     </div>..     
-00000e60: 2020 2020 2020 2020 2020 207b 2520 7769             {% wi
-00000e70: 7468 2064 6972 6563 746f 7279 5f6f 626a  th directory_obj
-00000e80: 6563 742e 7265 7375 6d65 2061 7320 7265  ect.resume as re
-00000e90: 7375 6d65 2025 7d0a 2020 2020 2020 2020  sume %}.        
-00000ea0: 2020 2020 2020 2020 2020 2020 7b25 2069              {% i
-00000eb0: 6620 6469 7265 6374 6f72 795f 6f62 6a65  f directory_obje
-00000ec0: 6374 2e63 6f76 6572 2025 7d0a 2020 2020  ct.cover %}.    
-00000ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ee0: 2020 2020 7b25 206d 6564 6961 5f74 6875      {% media_thu
-00000ef0: 6d62 2064 6972 6563 746f 7279 5f6f 626a  mb directory_obj
-00000f00: 6563 742e 636f 7665 7220 2232 3030 7832  ect.cover "200x2
-00000f10: 3936 2220 666f 726d 6174 3d22 4a50 4547  96" format="JPEG
-00000f20: 2220 6173 2063 6f76 6572 5f74 6875 6d62  " as cover_thumb
-00000f30: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
-00000f40: 2020 2020 2020 2020 2020 2020 3c69 6d67              <img
-00000f50: 2063 6c61 7373 3d22 6361 7264 2d69 6d67   class="card-img
-00000f60: 2d74 6f70 2220 7372 633d 227b 7b20 636f  -top" src="{{ co
-00000f70: 7665 725f 7468 756d 622e 7572 6c20 7d7d  ver_thumb.url }}
-00000f80: 2220 616c 743d 2222 3e0a 2020 2020 2020  " alt="">.      
-00000f90: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
-00000fa0: 2065 6c73 6520 257d 0a20 2020 2020 2020   else %}.       
+00000d40: 2020 2020 7b25 2063 6f6d 6d65 6e74 2025      {% comment %
+00000d50: 7d3c 6833 2063 6c61 7373 3d22 6677 2d62  }<h3 class="fw-b
+00000d60: 6f6c 6420 6d62 2d30 2066 732d 3522 3e7b  old mb-0 fs-5">{
+00000d70: 7b20 7265 7375 6d65 2e66 696c 6573 697a  { resume.filesiz
+00000d80: 657c 6669 6c65 7369 7a65 666f 726d 6174  e|filesizeformat
+00000d90: 207d 7d3c 2f68 333e 7b25 2065 6e64 636f   }}</h3>{% endco
+00000da0: 6d6d 656e 7420 257d 0a20 2020 2020 2020  mment %}.       
+00000db0: 2020 2020 2020 2020 203c 2f64 6976 3e0a           </div>.
+00000dc0: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
+00000dd0: 763e 0a20 2020 2020 2020 207b 2520 656e  v>.        {% en
+00000de0: 6477 6974 6820 257d 0a20 2020 203c 2f64  dwith %}.    </d
+00000df0: 6976 3e0a 2020 2020 3c64 6976 2063 6c61  iv>.    <div cla
+00000e00: 7373 3d22 6465 7669 6365 2d64 6574 6169  ss="device-detai
+00000e10: 6c5f 5f64 6972 6563 746f 7269 6573 2064  l__directories d
+00000e20: 6972 6563 746f 7279 2d6c 6973 7422 3e0a  irectory-list">.
+00000e30: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+00000e40: 7373 3d22 6274 6e2d 746f 6f6c 6261 7220  ss="btn-toolbar 
+00000e50: 772d 3130 3020 6a75 7374 6966 792d 636f  w-100 justify-co
+00000e60: 6e74 656e 742d 6265 7477 6565 6e20 7062  ntent-between pb
+00000e70: 2d32 206d 622d 3222 0a20 2020 2020 2020  -2 mb-2".       
+00000e80: 2020 2020 2020 726f 6c65 3d22 746f 6f6c        role="tool
+00000e90: 6261 7222 2061 7269 612d 6c61 6265 6c3d  bar" aria-label=
+00000ea0: 2244 6576 6963 6520 746f 6f6c 6261 7222  "Device toolbar"
+00000eb0: 3e0a 2020 2020 2020 2020 2020 2020 3c64  >.            <d
+00000ec0: 6976 2063 6c61 7373 3d22 6274 6e2d 6772  iv class="btn-gr
+00000ed0: 6f75 7020 6274 6e2d 6772 6f75 702d 736d  oup btn-group-sm
+00000ee0: 2220 726f 6c65 3d22 6772 6f75 7022 0a20  " role="group". 
+00000ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f00: 6172 6961 2d6c 6162 656c 3d22 4465 7669  aria-label="Devi
+00000f10: 6365 206e 6176 6967 6174 696f 6e22 3e0a  ce navigation">.
+00000f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f30: 3c61 2063 6c61 7373 3d22 6274 6e20 6274  <a class="btn bt
+00000f40: 6e2d 7365 636f 6e64 6172 7922 0a20 2020  n-secondary".   
+00000f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f60: 6872 6566 3d22 7b25 2075 726c 2022 646a  href="{% url "dj
+00000f70: 616e 676f 5f64 656f 7669 3a64 6576 6963  ango_deovi:devic
+00000f80: 652d 7472 6565 2220 6465 7669 6365 5f73  e-tree" device_s
+00000f90: 6c75 673d 6465 7669 6365 5f6f 626a 6563  lug=device_objec
+00000fa0: 742e 736c 7567 2025 7d22 3e0a 2020 2020  t.slug %}">.    
 00000fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000fc0: 203c 7376 6720 636c 6173 733d 2263 6172   <svg class="car
-00000fd0: 642d 696d 672d 746f 7022 2077 6964 7468  d-img-top" width
-00000fe0: 3d22 3139 3722 2068 6569 6768 743d 2231  ="197" height="1
-00000ff0: 3030 2522 2078 6d6c 6e73 3d22 6874 7470  00%" xmlns="http
-00001000: 3a2f 2f77 7777 2e77 332e 6f72 672f 3230  ://www.w3.org/20
-00001010: 3030 2f73 7667 2220 726f 6c65 3d22 696d  00/svg" role="im
-00001020: 6722 2061 7269 612d 6c61 6265 6c3d 2243  g" aria-label="C
-00001030: 6172 6420 696d 6167 6520 6361 7022 2070  ard image cap" p
-00001040: 7265 7365 7276 6541 7370 6563 7452 6174  reserveAspectRat
-00001050: 696f 3d22 784d 6964 594d 6964 2073 6c69  io="xMidYMid sli
-00001060: 6365 2220 666f 6375 7361 626c 653d 2266  ce" focusable="f
-00001070: 616c 7365 223e 3c74 6974 6c65 3e43 6172  alse"><title>Car
-00001080: 6420 696d 6167 6520 6361 703c 2f74 6974  d image cap</tit
-00001090: 6c65 3e3c 7265 6374 2077 6964 7468 3d22  le><rect width="
-000010a0: 3130 3025 2220 6865 6967 6874 3d22 3130  100%" height="10
-000010b0: 3025 2220 6669 6c6c 3d22 2338 3638 6539  0%" fill="#868e9
-000010c0: 3622 3e3c 2f72 6563 743e 3c2f 7376 673e  6"></rect></svg>
-000010d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000010e0: 2020 2020 207b 2520 656e 6469 6620 257d       {% endif %}
-000010f0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001100: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-00001110: 3d22 6361 7264 2d66 6f6f 7465 7222 3e0a  ="card-footer">.
-00001120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001130: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-00001140: 7373 3d22 6469 7265 6374 6f72 792d 6c69  ss="directory-li
-00001150: 7374 5f5f 6d65 6469 6173 2063 6f6c 2d6d  st__medias col-m
-00001160: 642d 6175 746f 223e 0a20 2020 2020 2020  d-auto">.       
+00000fc0: 3c69 2063 6c61 7373 3d22 6269 2062 692d  <i class="bi bi-
+00000fd0: 666f 6c64 6572 206d 652d 3122 3e3c 2f69  folder me-1"></i
+00000fe0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00000ff0: 2020 2020 2020 4465 7669 6365 2074 7265        Device tre
+00001000: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+00001010: 2020 3c2f 613e 0a20 2020 2020 2020 2020    </a>.         
+00001020: 2020 203c 2f64 6976 3e0a 2020 2020 2020     </div>.      
+00001030: 2020 3c2f 6469 763e 0a0a 2020 2020 2020    </div>..      
+00001040: 2020 7b25 2066 6f72 2064 6972 6563 746f    {% for directo
+00001050: 7279 5f6f 626a 6563 7420 696e 206f 626a  ry_object in obj
+00001060: 6563 745f 6c69 7374 2025 7d0a 2020 2020  ect_list %}.    
+00001070: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+00001080: 6469 7265 6374 6f72 792d 6c69 7374 5f5f  directory-list__
+00001090: 6974 656d 223e 0a20 2020 2020 2020 2020  item">.         
+000010a0: 2020 203c 6469 7620 636c 6173 733d 2263     <div class="c
+000010b0: 6172 6422 3e0a 2020 2020 2020 2020 2020  ard">.          
+000010c0: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+000010d0: 3d22 6361 7264 2d62 6f64 7922 3e0a 2020  ="card-body">.  
+000010e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000010f0: 2020 3c61 2068 7265 663d 227b 7b20 6469    <a href="{{ di
+00001100: 7265 6374 6f72 795f 6f62 6a65 6374 2e67  rectory_object.g
+00001110: 6574 5f61 6273 6f6c 7574 655f 7572 6c20  et_absolute_url 
+00001120: 7d7d 220a 2020 2020 2020 2020 2020 2020  }}".            
+00001130: 2020 2020 2020 2020 2020 2020 636c 6173              clas
+00001140: 733d 2264 6972 6563 746f 7279 2d6c 6973  s="directory-lis
+00001150: 745f 5f74 6974 6c65 2073 7472 6574 6368  t__title stretch
+00001160: 6564 2d6c 696e 6b22 3e0a 2020 2020 2020  ed-link">.      
 00001170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001180: 2020 2020 203c 6920 636c 6173 733d 2262       <i class="b
-00001190: 6920 6269 2d66 696c 6d20 6d65 2d31 223e  i bi-film me-1">
-000011a0: 3c2f 693e 0a20 2020 2020 2020 2020 2020  </i>.           
-000011b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000011c0: 207b 7b20 7265 7375 6d65 2e6d 6564 6961   {{ resume.media
-000011d0: 6669 6c65 7320 7d7d 0a20 2020 2020 2020  files }}.       
+00001180: 2020 7b25 2069 6620 6469 7265 6374 6f72    {% if director
+00001190: 795f 6f62 6a65 6374 2e74 6974 6c65 2025  y_object.title %
+000011a0: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+000011b0: 2020 2020 2020 2020 2020 2020 2020 7b7b                {{
+000011c0: 2064 6972 6563 746f 7279 5f6f 626a 6563   directory_objec
+000011d0: 742e 7469 746c 6520 7d7d 0a20 2020 2020  t.title }}.     
 000011e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000011f0: 203c 2f64 6976 3e0a 2020 2020 2020 2020   </div>.        
+000011f0: 2020 207b 2520 656c 7365 2025 7d0a 2020     {% else %}.  
 00001200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001210: 3c64 6976 2063 6c61 7373 3d22 6469 7265  <div class="dire
-00001220: 6374 6f72 792d 6c69 7374 5f5f 7369 7a65  ctory-list__size
-00001230: 2063 6f6c 223e 0a20 2020 2020 2020 2020   col">.         
+00001210: 2020 2020 2020 2020 2020 7b7b 2064 6972            {{ dir
+00001220: 6563 746f 7279 5f6f 626a 6563 742e 6469  ectory_object.di
+00001230: 7265 6374 6f72 795f 6e61 6d65 207d 7d0a  rectory_name }}.
 00001240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001250: 2020 207b 7b20 7265 7375 6d65 2e66 696c     {{ resume.fil
-00001260: 6573 697a 657c 6669 6c65 7369 7a65 666f  esize|filesizefo
-00001270: 726d 6174 207d 7d0a 2020 2020 2020 2020  rmat }}.        
-00001280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001290: 2020 2020 3c69 2063 6c61 7373 3d22 6269      <i class="bi
-000012a0: 2062 692d 6261 722d 6368 6172 742d 6669   bi-bar-chart-fi
-000012b0: 6c6c 206d 732d 3122 3e3c 2f69 3e0a 2020  ll ms-1"></i>.  
-000012c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012d0: 2020 2020 2020 3c2f 6469 763e 0a20 2020        </div>.   
-000012e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012f0: 203c 2f64 6976 3e0a 2020 2020 2020 2020   </div>.        
-00001300: 2020 2020 2020 2020 7b25 2065 6e64 7769          {% endwi
-00001310: 7468 2025 7d0a 2020 2020 2020 2020 2020  th %}.          
-00001320: 2020 3c2f 6469 763e 0a20 2020 2020 2020    </div>.       
-00001330: 203c 2f64 6976 3e0a 2020 2020 2020 2020   </div>.        
-00001340: 7b25 2065 6e64 666f 7220 257d 0a20 2020  {% endfor %}.   
-00001350: 203c 2f64 6976 3e0a 2020 2020 7b25 2069   </div>.    {% i
-00001360: 6e63 6c75 6465 2022 646a 616e 676f 5f64  nclude "django_d
-00001370: 656f 7669 2f70 6167 696e 6174 696f 6e2e  eovi/pagination.
-00001380: 6874 6d6c 2220 257d 0a3c 2f64 6976 3e0a  html" %}.</div>.
-00001390: 7b25 2065 6e64 7370 6163 656c 6573 7320  {% endspaceless 
-000013a0: 257d 7b25 2065 6e64 626c 6f63 6b20 6170  %}{% endblock ap
-000013b0: 705f 636f 6e74 656e 7420 257d 0a         p_content %}.
+00001250: 2020 2020 2020 2020 7b25 2065 6e64 6966          {% endif
+00001260: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
+00001270: 2020 2020 2020 2020 3c2f 613e 0a20 2020          </a>.   
+00001280: 2020 2020 2020 2020 2020 2020 203c 2f64               </d
+00001290: 6976 3e0a 0a20 2020 2020 2020 2020 2020  iv>..           
+000012a0: 2020 2020 207b 2520 7769 7468 2064 6972       {% with dir
+000012b0: 6563 746f 7279 5f6f 626a 6563 742e 7265  ectory_object.re
+000012c0: 7375 6d65 2061 7320 7265 7375 6d65 2025  sume as resume %
+000012d0: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+000012e0: 2020 2020 2020 7b25 2069 6620 6469 7265        {% if dire
+000012f0: 6374 6f72 795f 6f62 6a65 6374 2e63 6f76  ctory_object.cov
+00001300: 6572 2025 7d0a 2020 2020 2020 2020 2020  er %}.          
+00001310: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
+00001320: 206d 6564 6961 5f74 6875 6d62 2064 6972   media_thumb dir
+00001330: 6563 746f 7279 5f6f 626a 6563 742e 636f  ectory_object.co
+00001340: 7665 7220 2232 3030 7832 3936 2220 666f  ver "200x296" fo
+00001350: 726d 6174 3d22 4a50 4547 2220 6173 2063  rmat="JPEG" as c
+00001360: 6f76 6572 5f74 6875 6d62 2025 7d0a 2020  over_thumb %}.  
+00001370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001380: 2020 2020 2020 3c69 6d67 2063 6c61 7373        <img class
+00001390: 3d22 6361 7264 2d69 6d67 2d74 6f70 2220  ="card-img-top" 
+000013a0: 7372 633d 227b 7b20 636f 7665 725f 7468  src="{{ cover_th
+000013b0: 756d 622e 7572 6c20 7d7d 2220 616c 743d  umb.url }}" alt=
+000013c0: 2222 3e0a 2020 2020 2020 2020 2020 2020  "">.            
+000013d0: 2020 2020 2020 2020 7b25 2065 6c73 6520          {% else 
+000013e0: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
+000013f0: 2020 2020 2020 2020 2020 203c 7376 6720             <svg 
+00001400: 636c 6173 733d 2263 6172 642d 696d 672d  class="card-img-
+00001410: 746f 7022 2077 6964 7468 3d22 3139 3722  top" width="197"
+00001420: 2068 6569 6768 743d 2231 3030 2522 2078   height="100%" x
+00001430: 6d6c 6e73 3d22 6874 7470 3a2f 2f77 7777  mlns="http://www
+00001440: 2e77 332e 6f72 672f 3230 3030 2f73 7667  .w3.org/2000/svg
+00001450: 2220 726f 6c65 3d22 696d 6722 2061 7269  " role="img" ari
+00001460: 612d 6c61 6265 6c3d 2243 6172 6420 696d  a-label="Card im
+00001470: 6167 6520 6361 7022 2070 7265 7365 7276  age cap" preserv
+00001480: 6541 7370 6563 7452 6174 696f 3d22 784d  eAspectRatio="xM
+00001490: 6964 594d 6964 2073 6c69 6365 2220 666f  idYMid slice" fo
+000014a0: 6375 7361 626c 653d 2266 616c 7365 223e  cusable="false">
+000014b0: 3c74 6974 6c65 3e43 6172 6420 696d 6167  <title>Card imag
+000014c0: 6520 6361 703c 2f74 6974 6c65 3e3c 7265  e cap</title><re
+000014d0: 6374 2077 6964 7468 3d22 3130 3025 2220  ct width="100%" 
+000014e0: 6865 6967 6874 3d22 3130 3025 2220 6669  height="100%" fi
+000014f0: 6c6c 3d22 2338 3638 6539 3622 3e3c 2f72  ll="#868e96"></r
+00001500: 6563 743e 3c2f 7376 673e 0a20 2020 2020  ect></svg>.     
+00001510: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+00001520: 2520 656e 6469 6620 257d 0a0a 2020 2020  % endif %}..    
+00001530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001540: 3c64 6976 2063 6c61 7373 3d22 6361 7264  <div class="card
+00001550: 2d66 6f6f 7465 7222 3e0a 2020 2020 2020  -footer">.      
+00001560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001570: 2020 3c64 6976 2063 6c61 7373 3d22 6469    <div class="di
+00001580: 7265 6374 6f72 792d 6c69 7374 5f5f 6d65  rectory-list__me
+00001590: 6469 6173 2063 6f6c 2d6d 642d 6175 746f  dias col-md-auto
+000015a0: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
+000015b0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+000015c0: 6920 636c 6173 733d 2262 6920 6269 2d66  i class="bi bi-f
+000015d0: 696c 6d20 6d65 2d31 223e 3c2f 693e 0a20  ilm me-1"></i>. 
+000015e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000015f0: 2020 2020 2020 2020 2020 207b 7b20 7265             {{ re
+00001600: 7375 6d65 2e6d 6564 6961 6669 6c65 7320  sume.mediafiles 
+00001610: 7d7d 0a20 2020 2020 2020 2020 2020 2020  }}.             
+00001620: 2020 2020 2020 2020 2020 203c 2f64 6976             </div
+00001630: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00001640: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+00001650: 6c61 7373 3d22 6469 7265 6374 6f72 792d  lass="directory-
+00001660: 6c69 7374 5f5f 7369 7a65 2063 6f6c 223e  list__size col">
+00001670: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001680: 2020 2020 2020 2020 2020 2020 207b 7b20               {{ 
+00001690: 7265 7375 6d65 2e66 696c 6573 697a 657c  resume.filesize|
+000016a0: 6669 6c65 7369 7a65 666f 726d 6174 207d  filesizeformat }
+000016b0: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+000016c0: 2020 2020 2020 2020 2020 2020 2020 3c69                <i
+000016d0: 2063 6c61 7373 3d22 6269 2062 692d 6261   class="bi bi-ba
+000016e0: 722d 6368 6172 742d 6669 6c6c 206d 732d  r-chart-fill ms-
+000016f0: 3122 3e3c 2f69 3e0a 2020 2020 2020 2020  1"></i>.        
+00001700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001710: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
+00001720: 2020 2020 2020 2020 2020 203c 2f64 6976             </div
+00001730: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00001740: 2020 7b25 2065 6e64 7769 7468 2025 7d0a    {% endwith %}.
+00001750: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
+00001760: 763e 0a20 2020 2020 2020 203c 2f64 6976  v>.        </div
+00001770: 3e0a 2020 2020 2020 2020 7b25 2065 6e64  >.        {% end
+00001780: 666f 7220 257d 0a20 2020 203c 2f64 6976  for %}.    </div
+00001790: 3e0a 2020 2020 7b25 2069 6e63 6c75 6465  >.    {% include
+000017a0: 2022 646a 616e 676f 5f64 656f 7669 2f70   "django_deovi/p
+000017b0: 6167 696e 6174 696f 6e2e 6874 6d6c 2220  agination.html" 
+000017c0: 257d 0a3c 2f64 6976 3e0a 7b25 2065 6e64  %}.</div>.{% end
+000017d0: 7370 6163 656c 6573 7320 257d 7b25 2065  spaceless %}{% e
+000017e0: 6e64 626c 6f63 6b20 6170 705f 636f 6e74  ndblock app_cont
+000017f0: 656e 7420 257d 0a                        ent %}.
```

### Comparing `django-deovi-0.6.1/django_deovi/templates/django_deovi/device/index.html` & `django-deovi-0.6.2/django_deovi/templates/django_deovi/device/index.html`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 {% extends "django_deovi/base.html" %}
-{% load i18n %}
+{% load i18n deovi %}
 
 {% block head_title %}{% trans "Devices" %} - {{ block.super }}{% endblock head_title %}
 
 {% block app_content %}{% spaceless %}
 <div class="device-index">
     <h2 class="mt-4 mb-5 display-1 text-center">{% trans "Devices" %}</h2>
     <div class="container px-4">
@@ -13,38 +13,41 @@
                 <div class="card h-100">
                     <h3 class="card-header h5 device-title">
                         {{ device_object }}
                     </h3>
                     <div class="card-body">
                         {% with device_object.resume as resume %}
                         <div class="row gx-1 mt-3 mb-1">
-                            <div class="device-directories col-3 text-center">
+                            <div class="device-directories col-5 text-center">
                                 <div><i class="h4 bi bi-folder"></i></div>
                                 <div><small class="sm-2">{% trans "Directories" %}</small></div>
                                 <div class="h3">{{ resume.directories }}</div>
-                            </div>
-                            <div class="device-medias col-3 text-center">
-                                <div><i class="h4 bi bi-film"></i></div>
+                                <div class="mt-4"><i class="h4 bi bi-film"></i></div>
                                 <div><small class="sm-2">{% trans "Medias" %}</small></div>
                                 <div class="h3">{{ resume.mediafiles }}</div>
                             </div>
-                            <div class="device-size col-6 text-center">
-                                <div><i class="h4 bi bi-bar-chart-fill"></i></div>
-                                <div><small class="sm-2">{% trans "Total size" %}</small></div>
-                                <div class="h3">{{ resume.filesize|filesizeformat }}</div>
+                            <div class="device-occupancy col-7 text-center">
+                                {% show_occupancy_svg device_object resume=resume %}
+                            </div>
+                            <div class="col-4"></div>
+                            <div class="device-occupancy col-8 text-center">
+                                <div class="index-devices row g-0 row-cols-3">
+                                    <div class="col">Used<br>{{ resume.disk_used|filesizeformat }}</div>
+                                    <div class="col">Free<br>{{ resume.disk_free|filesizeformat }}</div>
+                                    <div class="col">Total<br>{{ resume.disk_total|filesizeformat }}</div>
+                                </div>
                             </div>
                         </div>
                         {% endwith %}
                     </div>
                     <div class="card-footer">
                         <div class="row">
                             <div class="col align-middle">
                                 <small class="text-muted">
-                                    {% comment %}TODO: This should be the last update directory or a new Device.modified field{% endcomment %}
-                                    Last updated {{ device_object.created_date|timesince }}
+                                    Last updated {{ device_object.last_update|timesince }}
                                 </small>
                             </div>
                             <div class="col-md-auto text-end">
                                 <a href="{{ device_object.get_absolute_url }}" class="device-link stretched-link btn btn-outline-dark">
                                     <i class="bi bi-arrow-right"></i>
                                 </a>
                             </div>
```

#### html2text {}

```diff
@@ -1,19 +1,22 @@
-{% extends "django_deovi/base.html" %} {% load i18n %} {% block head_title %}{%
-trans "Devices" %} - {{ block.super }}{% endblock head_title %} {% block
-app_content %}{% spaceless %}
+{% extends "django_deovi/base.html" %} {% load i18n deovi %} {% block
+head_title %}{% trans "Devices" %} - {{ block.super }}{% endblock head_title %}
+{% block app_content %}{% spaceless %}
 ********** {{%% ttrraannss ""DDeevviicceess"" %%}} **********
 {% for device_object in device_list %}
 ******** {{{{ ddeevviiccee__oobbjjeecctt }}}} ********
 {% with device_object.resume as resume %}
 {% trans "Directories" %}
 {{ resume.directories }}
 {% trans "Medias" %}
 {{ resume.mediafiles }}
-{% trans "Total size" %}
-{{ resume.filesize|filesizeformat }}
+{% show_occupancy_svg device_object resume=resume %}
+Used
+{{ resume.disk_used|filesizeformat }}
+Free
+{{ resume.disk_free|filesizeformat }}
+Total
+{{ resume.disk_total|filesizeformat }}
 {% endwith %}
-{% comment %}TODO: This should be the last update directory or a new
-Device.modified field{% endcomment %} Last updated {
-{ device_object.created_date|timesince }}
+Last updated {{ device_object.last_update|timesince }}
 {% endfor %}
 {% endspaceless %}{% endblock app_content %}
```

### Comparing `django-deovi-0.6.1/django_deovi/templates/django_deovi/device/tree.html` & `django-deovi-0.6.2/django_deovi/templates/django_deovi/device/tree.html`

 * *Files 12% similar despite different names*

```diff
@@ -88,14 +88,23 @@
                                data-treegrid-form="#treegrid-form"
                                data-treegrid-action="details-json"
                                data-treegrid-title="Export selection details to JSON"
                                href="#">
                                 Path details as JSON
                             </a>
                         </li>
+                        <li>
+                            <a class="dropdown-item treegrid-export-action"
+                               data-treegrid-form="#treegrid-form"
+                               data-treegrid-action="size-sum"
+                               data-treegrid-title="Selected path sizes sum"
+                               href="#">
+                                Compute size to a sum
+                            </a>
+                        </li>
                     </ul>
                 </div>
             </div>
         </div>
 
         <div class="treegrid__directory treegrid__directory--headers">
             <div class="name">Name</div>
```

### Comparing `django-deovi-0.6.1/django_deovi/templates/django_deovi/directory/detail.html` & `django-deovi-0.6.2/django_deovi/templates/django_deovi/directory/detail.html`

 * *Files identical despite different names*

### Comparing `django-deovi-0.6.1/django_deovi/templates/django_deovi/pagination.html` & `django-deovi-0.6.2/django_deovi/templates/django_deovi/pagination.html`

 * *Files identical despite different names*

### Comparing `django-deovi-0.6.1/django_deovi/urls.py` & `django-deovi-0.6.2/django_deovi/urls.py`

 * *Files identical despite different names*

### Comparing `django-deovi-0.6.1/django_deovi/utils/imaging.py` & `django-deovi-0.6.2/django_deovi/utils/imaging.py`

 * *Files identical despite different names*

### Comparing `django-deovi-0.6.1/django_deovi/utils/tests.py` & `django-deovi-0.6.2/django_deovi/utils/tests.py`

 * *Files identical despite different names*

### Comparing `django-deovi-0.6.1/django_deovi/utils/tree.py` & `django-deovi-0.6.2/django_deovi/utils/tree.py`

 * *Files identical despite different names*

### Comparing `django-deovi-0.6.1/django_deovi/views/device.py` & `django-deovi-0.6.2/django_deovi/views/device.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 from django.conf import settings
 from django.http import JsonResponse, HttpResponseBadRequest
 from django.urls import reverse
 from django.utils.translation import gettext_lazy as _
 from django.views.generic import DetailView, ListView, View
 from django.views.generic.detail import SingleObjectMixin
+from django.template.defaultfilters import filesizeformat
+
 
 from .mixins import DeoviBreadcrumMixin
 from ..models import Device, Directory
 
 
 class DeviceIndexView(DeoviBreadcrumMixin, ListView):
     """
@@ -202,21 +204,21 @@
 
     Finally all success responses will return a payload alike: ::
 
         {
             "content": ...
         }
 
-    Where ``content`` will contains action output.
+    Where ``content`` will contains action output as a string.
 
     """
     model = Device
     http_method_names = ["post"]
     slug_url_kwarg = "device_slug"
-    task_actions = ["details-json", "list-text", "ping"]
+    task_actions = ["details-json", "list-text", "size-sum", "ping"]
 
     def get_queryset(self):
         """
         Build queryset base to get Device.
         """
         return self.model.objects.all()
 
@@ -281,11 +283,54 @@
         """
         Returns the selected paths details into a dumped JSON (carried in a string).
         """
         if "paths" not in payload:
             return HttpResponseBadRequest(
                 "Request data is invalid, details items must have a 'path' item"
             )
-        print(json.dumps(payload["paths"], indent=4))
+
         return JsonResponse({
             "content": json.dumps(payload["paths"], indent=4)
         })
+
+    def action_size_sum(self, request, payload):
+        """
+        Returns the sum of selected path sizes.
+        """
+        if "paths" not in payload:
+            return HttpResponseBadRequest(
+                "Request data is invalid, details items must have a 'path' item"
+            )
+
+        # Prepare lines from selections
+        lines = [
+            [
+                item["name"],
+                int(item["recursive_filesize"]),
+                filesizeformat(item["recursive_filesize"])
+            ]
+            for item in payload["paths"]
+        ]
+
+        # Get the max size of name and formatted size
+        name_column_width = max([len(k) for k, v, f in lines]) + 1
+        size_column_width = max([len(f) for k, v, f in lines]) + 2
+
+        # Push lines in output
+        output = []
+        for name, size, formatted in lines:
+            output.append(
+                name.ljust(name_column_width) + ":" +
+                formatted.rjust(size_column_width)
+            )
+
+        # Add final divider and total sum
+        output.append("-" * (name_column_width + size_column_width + 1))
+        size_sum = sum([size for name, size, formatted in lines])
+        output.append(
+            "Total".ljust(name_column_width) + ":" +
+            filesizeformat(size_sum).rjust(size_column_width)
+        )
+
+        return JsonResponse({
+            "content": "\n".join(output)
+        })
```

### Comparing `django-deovi-0.6.1/django_deovi/views/directory.py` & `django-deovi-0.6.2/django_deovi/views/directory.py`

 * *Files identical despite different names*

### Comparing `django-deovi-0.6.1/django_deovi/views/media.py` & `django-deovi-0.6.2/django_deovi/views/media.py`

 * *Files identical despite different names*

### Comparing `django-deovi-0.6.1/django_deovi.egg-info/PKG-INFO` & `django-deovi-0.6.2/django_deovi.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-deovi
-Version: 0.6.1
+Version: 0.6.2
 Summary: A Django application around Deovi
 Home-page: https://github.com/sveetch/django-deovi
 Author: David Thenon
 Author-email: sveetch@gmail.com
 License: MIT
 Keywords: Python Django
 Classifier: Development Status :: 5 - Production/Stable
@@ -24,27 +24,33 @@
 Provides-Extra: doc
 Provides-Extra: release
 License-File: LICENCE.txt
 
 .. _Python: https://www.python.org/
 .. _Django: https://www.djangoproject.com/
 .. _Django REST framework: https://www.django-rest-framework.org/
+.. _bigtree: https://bigtree.readthedocs.io/
+.. _Deovi: https://deovi.readthedocs.io/
+
 
 ============
 Django Deovi
 ============
 
-A Django application around Deovi
+A Django interface to load `Deovi`_ dumps and browse data.
+
 
 Dependancies
 ************
 
 * `Python`_>=3.8;
 * `Django`_>=4.0;
 * `Django REST framework`_>=3.13.0;
+* `bigtree`_>=0.10.3;
+* `Deovi`_>=0.7.0;
+
 
 Links
 *****
 
-* (Not yet) Read the documentation on `Read the docs <https://django-deovi.readthedocs.io/>`_;
-* (Not yet) Download its `PyPi package <https://pypi.python.org/pypi/django-deovi>`_;
+* Download its `PyPi package <https://pypi.python.org/pypi/django-deovi>`_;
 * Clone it on its `Github repository <https://github.com/sveetch/django-deovi>`_;
```

### Comparing `django-deovi-0.6.1/django_deovi.egg-info/SOURCES.txt` & `django-deovi-0.6.2/django_deovi.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -28,32 +28,36 @@
 django_deovi/factories/dump.py
 django_deovi/factories/media.py
 django_deovi/factories/user.py
 django_deovi/management/commands/__init__.py
 django_deovi/management/commands/load_medias.py
 django_deovi/migrations/0001_initial.py
 django_deovi/migrations/0002_alter_directory_options_alter_mediafile_options_and_more.py
+django_deovi/migrations/0003_device_last_update.py
+django_deovi/migrations/0004_add_device_disk_usage_fields.py
 django_deovi/migrations/__init__.py
 django_deovi/models/__init__.py
 django_deovi/models/device.py
 django_deovi/models/directory.py
 django_deovi/models/media.py
 django_deovi/serializers/__init__.py
 django_deovi/serializers/media.py
 django_deovi/templates/django_deovi/base.html
 django_deovi/templates/django_deovi/mediafile_detail.html
 django_deovi/templates/django_deovi/pagination.html
+django_deovi/templates/django_deovi/device/_occupancy.svg
 django_deovi/templates/django_deovi/device/_tree-item.html
 django_deovi/templates/django_deovi/device/detail.html
 django_deovi/templates/django_deovi/device/index.html
 django_deovi/templates/django_deovi/device/tree.html
 django_deovi/templates/django_deovi/directory/detail.html
 django_deovi/templatetags/__init__.py
 django_deovi/templatetags/deovi.py
 django_deovi/utils/__init__.py
+django_deovi/utils/formatters.py
 django_deovi/utils/imaging.py
 django_deovi/utils/tests.py
 django_deovi/utils/tree.py
 django_deovi/views/__init__.py
 django_deovi/views/device.py
 django_deovi/views/directory.py
 django_deovi/views/media.py
```

### Comparing `django-deovi-0.6.1/setup.cfg` & `django-deovi-0.6.2/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-deovi
-version = 0.6.1
+version = 0.6.2
 description = A Django application around Deovi
 long_description = file:README.rst
 long_description_content_type = text/x-rst
 author = David Thenon
 author_email = sveetch@gmail.com
 url = https://github.com/sveetch/django-deovi
 license = MIT
@@ -21,16 +21,16 @@
 	Framework :: Django
 	Framework :: Django :: 4.0
 
 [options]
 include_package_data = True
 install_requires = 
 	Django>=4.0,<4.1
-	deovi>=0.5.2
-	bigtree>=0.10.3
+	deovi>=0.7.0
+	bigtree[pandas]>=0.10.3
 	django-smart-media
 packages = find:
 zip_safe = True
 
 [options.extras_require]
 breadcrumbs = 
 	django-view-breadcrumbs>=2.2.4
```

