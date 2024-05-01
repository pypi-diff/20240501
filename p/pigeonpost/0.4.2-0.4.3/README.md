# Comparing `tmp/pigeonpost-0.4.2.tar.gz` & `tmp/pigeonpost-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pigeonpost-0.4.2.tar", last modified: Tue Apr  9 16:20:48 2024, max compression
+gzip compressed data, was "pigeonpost-0.4.3.tar", last modified: Wed May  1 16:23:57 2024, max compression
```

## Comparing `pigeonpost-0.4.2.tar` & `pigeonpost-0.4.3.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:20:48.004715 pigeonpost-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-09 16:20:48.004715 pigeonpost-0.4.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:20:47.992715 pigeonpost-0.4.2/pigeon/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:20:47.992715 pigeonpost-0.4.2/pigeon/conf/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/conf/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/conf/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/conf/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:20:47.996714 pigeonpost-0.4.2/pigeon/core/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/core/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/core/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/core/secure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/core/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:20:47.996714 pigeonpost-0.4.2/pigeon/default/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/default/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:20:47.996714 pigeonpost-0.4.2/pigeon/files/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/files/media.py
--rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/files/static.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:20:47.996714 pigeonpost-0.4.2/pigeon/http/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/http/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/http/message.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/http/request.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/http/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:20:47.996714 pigeonpost-0.4.2/pigeon/middleware/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/middleware/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:20:48.000715 pigeonpost-0.4.2/pigeon/middleware/components/
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/middleware/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/middleware/components/cache_control.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/middleware/components/component.py
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/middleware/components/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4214 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/middleware/components/content_negotiation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/middleware/components/cors.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/middleware/components/date.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/middleware/components/host.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/middleware/components/mediafiles.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/middleware/components/method.py
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/middleware/components/server.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/middleware/components/staticfiles.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:20:48.000715 pigeonpost-0.4.2/pigeon/middleware/conversion/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/middleware/conversion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/middleware/conversion/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:20:48.000715 pigeonpost-0.4.2/pigeon/middleware/conversion/mime/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/middleware/conversion/mime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/middleware/conversion/mime/generators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/middleware/conversion/mime/parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/middleware/pipe.py
--rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/middleware/processing.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/middleware/tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/middleware/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/shortcuts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:20:48.000715 pigeonpost-0.4.2/pigeon/templating/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/templating/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/templating/templater.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:20:48.000715 pigeonpost-0.4.2/pigeon/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/utils/common.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3227 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/utils/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:20:48.000715 pigeonpost-0.4.2/pigeonpost.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-09 16:20:47.000000 pigeonpost-0.4.2/pigeonpost.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-09 16:20:47.000000 pigeonpost-0.4.2/pigeonpost.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 16:20:47.000000 pigeonpost-0.4.2/pigeonpost.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-09 16:20:47.000000 pigeonpost-0.4.2/pigeonpost.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-09 16:20:47.000000 pigeonpost-0.4.2/pigeonpost.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-09 16:20:47.000000 pigeonpost-0.4.2/pigeonpost.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-09 16:20:48.004715 pigeonpost-0.4.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)       37 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:23:57.546938 pigeonpost-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-01 16:23:57.546938 pigeonpost-0.4.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:23:57.538938 pigeonpost-0.4.3/pigeon/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:23:57.538938 pigeonpost-0.4.3/pigeon/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/conf/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/conf/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/conf/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:23:57.542938 pigeonpost-0.4.3/pigeon/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/core/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/core/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/core/secure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/core/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:23:57.542938 pigeonpost-0.4.3/pigeon/default/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/default/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:23:57.542938 pigeonpost-0.4.3/pigeon/files/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/files/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/files/static.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:23:57.542938 pigeonpost-0.4.3/pigeon/http/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/http/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/http/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/http/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/http/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:23:57.542938 pigeonpost-0.4.3/pigeon/middleware/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/middleware/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:23:57.546938 pigeonpost-0.4.3/pigeon/middleware/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/middleware/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/middleware/components/cache_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/middleware/components/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/middleware/components/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4214 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/middleware/components/content_negotiation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/middleware/components/cors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/middleware/components/date.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/middleware/components/host.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/middleware/components/mediafiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/middleware/components/method.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/middleware/components/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/middleware/components/staticfiles.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:23:57.546938 pigeonpost-0.4.3/pigeon/middleware/conversion/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/middleware/conversion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/middleware/conversion/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:23:57.546938 pigeonpost-0.4.3/pigeon/middleware/conversion/mime/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/middleware/conversion/mime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/middleware/conversion/mime/generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/middleware/conversion/mime/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/middleware/pipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/middleware/processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/middleware/tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/middleware/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/shortcuts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:23:57.546938 pigeonpost-0.4.3/pigeon/templating/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/templating/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/templating/templater.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:23:57.546938 pigeonpost-0.4.3/pigeon/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/utils/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3227 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/utils/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:23:57.546938 pigeonpost-0.4.3/pigeonpost.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-01 16:23:57.000000 pigeonpost-0.4.3/pigeonpost.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-01 16:23:57.000000 pigeonpost-0.4.3/pigeonpost.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 16:23:57.000000 pigeonpost-0.4.3/pigeonpost.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-01 16:23:57.000000 pigeonpost-0.4.3/pigeonpost.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-01 16:23:57.000000 pigeonpost-0.4.3/pigeonpost.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-01 16:23:57.000000 pigeonpost-0.4.3/pigeonpost.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-01 16:23:57.550938 pigeonpost-0.4.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)       37 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/setup.py
```

### Comparing `pigeonpost-0.4.2/pigeon/conf/manager.py` & `pigeonpost-0.4.3/pigeon/conf/manager.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.2/pigeon/conf/settings.py` & `pigeonpost-0.4.3/pigeon/conf/settings.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.2/pigeon/core/app.py` & `pigeonpost-0.4.3/pigeon/core/app.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.2/pigeon/core/handler.py` & `pigeonpost-0.4.3/pigeon/core/handler.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.2/pigeon/core/secure.py` & `pigeonpost-0.4.3/pigeon/core/secure.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.2/pigeon/core/server.py` & `pigeonpost-0.4.3/pigeon/core/server.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.2/pigeon/files/media.py` & `pigeonpost-0.4.3/pigeon/files/media.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.2/pigeon/files/static.py` & `pigeonpost-0.4.3/pigeon/files/static.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.2/pigeon/http/message.py` & `pigeonpost-0.4.3/pigeon/http/message.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.2/pigeon/http/request.py` & `pigeonpost-0.4.3/pigeon/http/request.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.2/pigeon/http/response.py` & `pigeonpost-0.4.3/pigeon/http/response.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.2/pigeon/middleware/auth.py` & `pigeonpost-0.4.3/pigeon/middleware/auth.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.2/pigeon/middleware/components/__init__.py` & `pigeonpost-0.4.3/pigeon/middleware/components/__init__.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.2/pigeon/middleware/components/cache_control.py` & `pigeonpost-0.4.3/pigeon/middleware/components/cache_control.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.2/pigeon/middleware/components/component.py` & `pigeonpost-0.4.3/pigeon/middleware/components/component.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.2/pigeon/middleware/components/connection.py` & `pigeonpost-0.4.3/pigeon/middleware/components/connection.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.2/pigeon/middleware/components/content_negotiation.py` & `pigeonpost-0.4.3/pigeon/middleware/components/content_negotiation.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.2/pigeon/middleware/components/cors.py` & `pigeonpost-0.4.3/pigeon/middleware/components/cors.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.2/pigeon/middleware/components/host.py` & `pigeonpost-0.4.3/pigeon/middleware/components/host.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.2/pigeon/middleware/components/mediafiles.py` & `pigeonpost-0.4.3/pigeon/middleware/components/mediafiles.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.2/pigeon/middleware/components/method.py` & `pigeonpost-0.4.3/pigeon/middleware/components/method.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.2/pigeon/middleware/components/staticfiles.py` & `pigeonpost-0.4.3/pigeon/middleware/components/staticfiles.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.2/pigeon/middleware/conversion/converter.py` & `pigeonpost-0.4.3/pigeon/middleware/conversion/converter.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.2/pigeon/middleware/conversion/mime/parsers.py` & `pigeonpost-0.4.3/pigeon/middleware/conversion/mime/parsers.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.2/pigeon/middleware/pipe.py` & `pigeonpost-0.4.3/pigeon/middleware/pipe.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.2/pigeon/middleware/processing.py` & `pigeonpost-0.4.3/pigeon/middleware/processing.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.2/pigeon/middleware/tags.py` & `pigeonpost-0.4.3/pigeon/middleware/tags.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.2/pigeon/middleware/views.py` & `pigeonpost-0.4.3/pigeon/middleware/views.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.2/pigeon/templating/templater.py` & `pigeonpost-0.4.3/pigeon/templating/templater.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.2/pigeon/utils/common.py` & `pigeonpost-0.4.3/pigeon/utils/common.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.2/pigeon/utils/logger.py` & `pigeonpost-0.4.3/pigeon/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.2/pigeonpost.egg-info/SOURCES.txt` & `pigeonpost-0.4.3/pigeonpost.egg-info/SOURCES.txt`

 * *Files identical despite different names*

