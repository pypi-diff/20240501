# Comparing `tmp/moodle_dl-2.3.8.tar.gz` & `tmp/moodle_dl-2.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moodle_dl-2.3.8.tar", last modified: Mon Apr 29 13:20:14 2024, max compression
+gzip compressed data, was "moodle_dl-2.3.9.tar", last modified: Wed May  1 17:41:32 2024, max compression
```

## Comparing `moodle_dl-2.3.8.tar` & `moodle_dl-2.3.9.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:20:14.362435 moodle_dl-2.3.8/
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10514 2024-04-29 13:20:14.362435 moodle_dl-2.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9022 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:20:14.350435 moodle_dl-2.3.8/moodle_dl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:20:14.350435 moodle_dl-2.3.8/moodle_dl/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27074 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/cli/config_wizard.py
--rw-r--r--   0 runner    (1001) docker     (127)     8153 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/cli/database_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6103 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/cli/moodle_wizard.py
--rw-r--r--   0 runner    (1001) docker     (127)     9268 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/cli/notifications_wizard.py
--rw-r--r--   0 runner    (1001) docker     (127)    11820 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    27774 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/database.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:20:14.354435 moodle_dl-2.3.8/moodle_dl/downloader/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5406 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/downloader/download_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:20:14.354435 moodle_dl-2.3.8/moodle_dl/downloader/extractors/
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/downloader/extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/downloader/extractors/echo360.py
--rw-r--r--   0 runner    (1001) docker     (127)    12660 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/downloader/extractors/googledrive.py
--rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/downloader/extractors/helixmedia_lti.py
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/downloader/extractors/kalvidres_lti.py
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/downloader/extractors/opencast_lti.py
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/downloader/extractors/owncloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/downloader/extractors/sharepoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/downloader/extractors/sharepointfiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/downloader/fake_download_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    41242 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/downloader/task.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    17840 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:20:14.354435 moodle_dl-2.3.8/moodle_dl/moodle/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/moodle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/moodle/cookie_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5814 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/moodle/core_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:20:14.358435 moodle_dl-2.3.8/moodle_dl/moodle/mods/
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/moodle/mods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10277 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/moodle/mods/assign.py
--rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/moodle/mods/book.py
--rw-r--r--   0 runner    (1001) docker     (127)     5408 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/moodle/mods/calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     8452 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/moodle/mods/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/moodle/mods/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/moodle/mods/folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     8440 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/moodle/mods/forum.py
--rw-r--r--   0 runner    (1001) docker     (127)     7648 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/moodle/mods/lesson.py
--rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/moodle/mods/page.py
--rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/moodle/mods/quiz.py
--rw-r--r--   0 runner    (1001) docker     (127)     8811 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/moodle/mods/workshop.py
--rw-r--r--   0 runner    (1001) docker     (127)    30746 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/moodle/moodle_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    12410 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/moodle/moodle_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    15855 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/moodle/request_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    17861 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/moodle/result_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:20:14.358435 moodle_dl-2.3.8/moodle_dl/notifications/
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/notifications/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:20:14.358435 moodle_dl-2.3.8/moodle_dl/notifications/console/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/notifications/console/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/notifications/console/console_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:20:14.358435 moodle_dl-2.3.8/moodle_dl/notifications/discord/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/notifications/discord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/notifications/discord/discord_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/notifications/discord/discord_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/notifications/discord/discord_shooter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:20:14.362435 moodle_dl-2.3.8/moodle_dl/notifications/mail/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/notifications/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36960 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/notifications/mail/header.png
--rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/notifications/mail/header_extender.png
--rw-r--r--   0 runner    (1001) docker     (127)    10237 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/notifications/mail/mail_formater.py
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/notifications/mail/mail_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/notifications/mail/mail_shooter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/notifications/notification_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:20:14.362435 moodle_dl-2.3.8/moodle_dl/notifications/telegram/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/notifications/telegram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/notifications/telegram/telegram_formater.py
--rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/notifications/telegram/telegram_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/notifications/telegram/telegram_shooter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:20:14.362435 moodle_dl-2.3.8/moodle_dl/notifications/xmpp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/notifications/xmpp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/notifications/xmpp/xmpp_formater.py
--rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/notifications/xmpp/xmpp_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/notifications/xmpp/xmpp_shooter.py
--rw-r--r--   0 runner    (1001) docker     (127)    11664 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    54399 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/moodle_dl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:20:14.362435 moodle_dl-2.3.8/moodle_dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10514 2024-04-29 13:20:14.000000 moodle_dl-2.3.8/moodle_dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-04-29 13:20:14.000000 moodle_dl-2.3.8/moodle_dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 13:20:14.000000 moodle_dl-2.3.8/moodle_dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-29 13:20:14.000000 moodle_dl-2.3.8/moodle_dl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 13:20:14.000000 moodle_dl-2.3.8/moodle_dl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-29 13:20:14.000000 moodle_dl-2.3.8/moodle_dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-29 13:20:14.000000 moodle_dl-2.3.8/moodle_dl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 13:20:14.362435 moodle_dl-2.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-04-29 13:20:06.000000 moodle_dl-2.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:41:32.966950 moodle_dl-2.3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10514 2024-05-01 17:41:32.966950 moodle_dl-2.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9022 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:41:32.954950 moodle_dl-2.3.9/moodle_dl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:41:32.958950 moodle_dl-2.3.9/moodle_dl/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27074 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/cli/config_wizard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8153 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/cli/database_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6103 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/cli/moodle_wizard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9268 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/cli/notifications_wizard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11820 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27774 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/database.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:41:32.958950 moodle_dl-2.3.9/moodle_dl/downloader/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5406 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/downloader/download_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:41:32.958950 moodle_dl-2.3.9/moodle_dl/downloader/extractors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/downloader/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/downloader/extractors/echo360.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12660 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/downloader/extractors/googledrive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/downloader/extractors/helixmedia_lti.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/downloader/extractors/kalvidres_lti.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/downloader/extractors/opencast_lti.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/downloader/extractors/owncloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/downloader/extractors/sharepoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/downloader/extractors/sharepointfiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/downloader/fake_download_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41370 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/downloader/task.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18169 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:41:32.958950 moodle_dl-2.3.9/moodle_dl/moodle/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/moodle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/moodle/cookie_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5814 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/moodle/core_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:41:32.962950 moodle_dl-2.3.9/moodle_dl/moodle/mods/
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/moodle/mods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10277 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/moodle/mods/assign.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/moodle/mods/book.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5408 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/moodle/mods/calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8452 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/moodle/mods/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/moodle/mods/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/moodle/mods/folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8440 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/moodle/mods/forum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7648 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/moodle/mods/lesson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/moodle/mods/page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/moodle/mods/quiz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8811 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/moodle/mods/workshop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30746 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/moodle/moodle_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12410 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/moodle/moodle_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16100 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/moodle/request_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17861 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/moodle/result_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:41:32.962950 moodle_dl-2.3.9/moodle_dl/notifications/
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/notifications/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:41:32.962950 moodle_dl-2.3.9/moodle_dl/notifications/console/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/notifications/console/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/notifications/console/console_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:41:32.962950 moodle_dl-2.3.9/moodle_dl/notifications/discord/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/notifications/discord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/notifications/discord/discord_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/notifications/discord/discord_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/notifications/discord/discord_shooter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:41:32.962950 moodle_dl-2.3.9/moodle_dl/notifications/mail/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/notifications/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36960 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/notifications/mail/header.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/notifications/mail/header_extender.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10237 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/notifications/mail/mail_formater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/notifications/mail/mail_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/notifications/mail/mail_shooter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/notifications/notification_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:41:32.966950 moodle_dl-2.3.9/moodle_dl/notifications/telegram/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/notifications/telegram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/notifications/telegram/telegram_formater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/notifications/telegram/telegram_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/notifications/telegram/telegram_shooter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:41:32.966950 moodle_dl-2.3.9/moodle_dl/notifications/xmpp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/notifications/xmpp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/notifications/xmpp/xmpp_formater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/notifications/xmpp/xmpp_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/notifications/xmpp/xmpp_shooter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11690 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54533 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/moodle_dl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:41:32.966950 moodle_dl-2.3.9/moodle_dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10514 2024-05-01 17:41:32.000000 moodle_dl-2.3.9/moodle_dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-05-01 17:41:32.000000 moodle_dl-2.3.9/moodle_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 17:41:32.000000 moodle_dl-2.3.9/moodle_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-01 17:41:32.000000 moodle_dl-2.3.9/moodle_dl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 17:41:32.000000 moodle_dl-2.3.9/moodle_dl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-01 17:41:32.000000 moodle_dl-2.3.9/moodle_dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-01 17:41:32.000000 moodle_dl-2.3.9/moodle_dl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 17:41:32.966950 moodle_dl-2.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-01 17:41:24.000000 moodle_dl-2.3.9/setup.py
```

### Comparing `moodle_dl-2.3.8/LICENSE` & `moodle_dl-2.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.8/PKG-INFO` & `moodle_dl-2.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moodle-dl
-Version: 2.3.8
+Version: 2.3.9
 Summary: Moodle-DL downloads course content fast from Moodle (eg. lecture pdfs)
 Home-page: https://github.com/C0D3D3V/Moodle-DL
 Author: C0D3D3V
 Author-email: moodle-dl@ist-ein-knaller.de
 License: GPL-3.0
 Project-URL: Documentation, https://github.com/C0D3D3V/Moodle-DL#readme
 Project-URL: Wiki, https://github.com/C0D3D3V/Moodle-DL/wiki
```

### Comparing `moodle_dl-2.3.8/README.md` & `moodle_dl-2.3.9/README.md`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.8/moodle_dl/cli/__init__.py` & `moodle_dl-2.3.9/moodle_dl/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.8/moodle_dl/cli/config_wizard.py` & `moodle_dl-2.3.9/moodle_dl/cli/config_wizard.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.8/moodle_dl/cli/database_manager.py` & `moodle_dl-2.3.9/moodle_dl/cli/database_manager.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.8/moodle_dl/cli/moodle_wizard.py` & `moodle_dl-2.3.9/moodle_dl/cli/moodle_wizard.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.8/moodle_dl/cli/notifications_wizard.py` & `moodle_dl-2.3.9/moodle_dl/cli/notifications_wizard.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.8/moodle_dl/config.py` & `moodle_dl-2.3.9/moodle_dl/config.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.8/moodle_dl/database.py` & `moodle_dl-2.3.9/moodle_dl/database.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.8/moodle_dl/downloader/download_service.py` & `moodle_dl-2.3.9/moodle_dl/downloader/download_service.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.8/moodle_dl/downloader/extractors/__init__.py` & `moodle_dl-2.3.9/moodle_dl/downloader/extractors/__init__.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.8/moodle_dl/downloader/extractors/echo360.py` & `moodle_dl-2.3.9/moodle_dl/downloader/extractors/echo360.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.8/moodle_dl/downloader/extractors/googledrive.py` & `moodle_dl-2.3.9/moodle_dl/downloader/extractors/googledrive.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.8/moodle_dl/downloader/extractors/helixmedia_lti.py` & `moodle_dl-2.3.9/moodle_dl/downloader/extractors/helixmedia_lti.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.8/moodle_dl/downloader/extractors/kalvidres_lti.py` & `moodle_dl-2.3.9/moodle_dl/downloader/extractors/kalvidres_lti.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.8/moodle_dl/downloader/extractors/opencast_lti.py` & `moodle_dl-2.3.9/moodle_dl/downloader/extractors/opencast_lti.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.8/moodle_dl/downloader/extractors/owncloud.py` & `moodle_dl-2.3.9/moodle_dl/downloader/extractors/owncloud.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.8/moodle_dl/downloader/extractors/sharepoint.py` & `moodle_dl-2.3.9/moodle_dl/downloader/extractors/sharepoint.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.8/moodle_dl/downloader/extractors/sharepointfiles.py` & `moodle_dl-2.3.9/moodle_dl/downloader/extractors/sharepointfiles.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.8/moodle_dl/downloader/fake_download_service.py` & `moodle_dl-2.3.9/moodle_dl/downloader/fake_download_service.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.8/moodle_dl/downloader/task.py` & `moodle_dl-2.3.9/moodle_dl/downloader/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -307,15 +307,17 @@
 
     async def get_head_infos(self, dl_url: str) -> HeadInfo:
         """
         Do a Head request to collect some information about the URL
         @return: If download should be aborted then None; else HeadInfo
         """
         ssl_context = SslHelper.get_ssl_context(
-            self.opts.global_opts.skip_cert_verify, self.opts.global_opts.allow_insecure_ssl
+            self.opts.global_opts.skip_cert_verify,
+            self.opts.global_opts.allow_insecure_ssl,
+            self.opts.global_opts.use_all_ciphers,
         )
         async with aiohttp.ClientSession(cookie_jar=self.get_cookie_jar(), raise_for_status=True) as session:
             try:
                 async with session.request("HEAD", dl_url, headers=self.RQ_HEADER, ssl=ssl_context, timeout=20) as resp:
                     if resp.url != dl_url:
                         if resp.history and len(resp.history) > 0:
                             logging.debug('[%d] URL was %s time(s) redirected', self.task_id, len(resp.history))
@@ -815,15 +817,17 @@
     async def download_url(self, dl_url: str, dest_path: str, timeout: int = None):
         total_bytes_received = 0
         done_tries = 0
         can_continue_on_fail = False
         file_obj = None
         headers = self.RQ_HEADER.copy()
         ssl_context = SslHelper.get_ssl_context(
-            self.opts.global_opts.skip_cert_verify, self.opts.global_opts.allow_insecure_ssl
+            self.opts.global_opts.skip_cert_verify,
+            self.opts.global_opts.allow_insecure_ssl,
+            self.opts.global_opts.use_all_ciphers,
         )
         with Timer() as watch:
             async with aiohttp.ClientSession(cookie_jar=self.get_cookie_jar(), raise_for_status=True) as session:
                 while done_tries < self.MAX_DL_RETRIES:
                     try:
                         if done_tries > 0:
                             logging.debug(
```

### Comparing `moodle_dl-2.3.8/moodle_dl/main.py` & `moodle_dl-2.3.9/moodle_dl/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -456,14 +456,25 @@
         '--allow-insecure-ssl',
         dest='allow_insecure_ssl',
         default=False,
         action='store_true',
         help='Allow connections to unpatched servers. Use this option if your server uses a very old SSL version.',
     )
     parser.add_argument(
+        '-uac',
+        '--use-all-ciphers',
+        dest='use_all_ciphers',
+        default=False,
+        action='store_true',
+        help=(
+            'Allow connections to servers that use insecure ciphers.'
+            + ' Use this option if your server uses an insecure cipher.'
+        ),
+    )
+    parser.add_argument(
         '-scv',
         '--skip-cert-verify',
         dest='skip_cert_verify',
         default=False,
         action='store_true',
         help='Don\'t verify TLS certificates. This option should only be used in non production environments.',
     )
```

### Comparing `moodle_dl-2.3.8/moodle_dl/moodle/cookie_handler.py` & `moodle_dl-2.3.9/moodle_dl/moodle/cookie_handler.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.8/moodle_dl/moodle/core_handler.py` & `moodle_dl-2.3.9/moodle_dl/moodle/core_handler.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.8/moodle_dl/moodle/mods/__init__.py` & `moodle_dl-2.3.9/moodle_dl/moodle/mods/__init__.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.8/moodle_dl/moodle/mods/assign.py` & `moodle_dl-2.3.9/moodle_dl/moodle/mods/assign.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.8/moodle_dl/moodle/mods/book.py` & `moodle_dl-2.3.9/moodle_dl/moodle/mods/book.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.8/moodle_dl/moodle/mods/calendar.py` & `moodle_dl-2.3.9/moodle_dl/moodle/mods/calendar.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.8/moodle_dl/moodle/mods/common.py` & `moodle_dl-2.3.9/moodle_dl/moodle/mods/common.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.8/moodle_dl/moodle/mods/data.py` & `moodle_dl-2.3.9/moodle_dl/moodle/mods/data.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.8/moodle_dl/moodle/mods/folder.py` & `moodle_dl-2.3.9/moodle_dl/moodle/mods/folder.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.8/moodle_dl/moodle/mods/forum.py` & `moodle_dl-2.3.9/moodle_dl/moodle/mods/forum.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.8/moodle_dl/moodle/mods/lesson.py` & `moodle_dl-2.3.9/moodle_dl/moodle/mods/lesson.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.8/moodle_dl/moodle/mods/page.py` & `moodle_dl-2.3.9/moodle_dl/moodle/mods/page.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.8/moodle_dl/moodle/mods/quiz.py` & `moodle_dl-2.3.9/moodle_dl/moodle/mods/quiz.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.8/moodle_dl/moodle/mods/workshop.py` & `moodle_dl-2.3.9/moodle_dl/moodle/mods/workshop.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.8/moodle_dl/moodle/moodle_constants.py` & `moodle_dl-2.3.9/moodle_dl/moodle/moodle_constants.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.8/moodle_dl/moodle/moodle_service.py` & `moodle_dl-2.3.9/moodle_dl/moodle/moodle_service.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.8/moodle_dl/moodle/request_helper.py` & `moodle_dl-2.3.9/moodle_dl/moodle/request_helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,15 +58,17 @@
         @return: The resulting response object and the session object.
         """
 
         data_urlencoded = ""
         if data is not None:
             data_urlencoded = self.recursive_urlencode(data)
 
-        session = SslHelper.custom_requests_session(self.opts.skip_cert_verify, self.opts.allow_insecure_ssl)
+        session = SslHelper.custom_requests_session(
+            self.opts.skip_cert_verify, self.opts.allow_insecure_ssl, self.opts.use_all_ciphers
+        )
         if cookie_jar_path is not None:
             session.cookies = MoodleDLCookieJar(cookie_jar_path)
 
             if os.path.exists(cookie_jar_path):
                 session.cookies.load(ignore_discard=True, ignore_expires=True)
         try:
             response = session.post(url, data=data_urlencoded, headers=self.RQ_HEADER, timeout=60)
@@ -87,15 +89,17 @@
         Sends a GET request to a specific URL of the Moodle system, including additional cookies
         (cookies are updated after the request)
         @param url: The url to which the request is sent. (the moodle base url is not added to the given URL)
         @param cookie_jar_path: The optional cookies to add to the request
         @return: The resulting Response object.
         """
 
-        session = SslHelper.custom_requests_session(self.opts.skip_cert_verify, self.opts.allow_insecure_ssl)
+        session = SslHelper.custom_requests_session(
+            self.opts.skip_cert_verify, self.opts.allow_insecure_ssl, self.opts.use_all_ciphers
+        )
         if cookie_jar_path is not None:
             session.cookies = MoodleDLCookieJar(cookie_jar_path)
 
             if os.path.exists(cookie_jar_path):
                 session.cookies.load(ignore_discard=True, ignore_expires=True)
             session.cookies = session.cookies
         try:
@@ -119,15 +123,17 @@
 
         if self.token is None:
             raise ValueError('The required token is not set!')
 
         data = self._get_POST_DATA(function, self.token, data)
         data_urlencoded = self.recursive_urlencode(data)
         url = self._get_REST_POST_URL(self.url_base, function)
-        ssl_context = SslHelper.get_ssl_context(self.opts.skip_cert_verify, self.opts.allow_insecure_ssl)
+        ssl_context = SslHelper.get_ssl_context(
+            self.opts.skip_cert_verify, self.opts.allow_insecure_ssl, self.opts.use_all_ciphers
+        )
 
         error_ctr = 0
         async with self.semaphore, aiohttp.ClientSession() as session:
             while error_ctr < self.MAX_RETRIES:
                 try:
                     async with session.post(
                         url,
@@ -177,15 +183,17 @@
         if self.token is None:
             raise ValueError('The required Token is not set!')
 
         data = self._get_POST_DATA(function, self.token, data)
         data_urlencoded = self.recursive_urlencode(data)
         url = self._get_REST_POST_URL(self.url_base, function)
 
-        session = SslHelper.custom_requests_session(self.opts.skip_cert_verify, self.opts.allow_insecure_ssl)
+        session = SslHelper.custom_requests_session(
+            self.opts.skip_cert_verify, self.opts.allow_insecure_ssl, self.opts.use_all_ciphers
+        )
         error_ctr = 0
         while error_ctr <= self.MAX_RETRIES:
             try:
                 response = session.post(url, data=data_urlencoded, headers=self.RQ_HEADER, timeout=timeout)
                 break
             except (requests.ConnectionError, requests.Timeout) as req_err:
                 # We treat requests.ConnectionErrors here specially, since they normally mean,
@@ -245,15 +253,17 @@
         Sends a POST request to the login endpoint of the Moodle system to
         obtain a token in JSON format.
         @param data: The data is inserted into the Post-Body as arguments. This
         should contain the login data.
         @return: The JSON response returned by the Moodle System, already
         checked for errors.
         """
-        session = SslHelper.custom_requests_session(self.opts.skip_cert_verify, self.opts.allow_insecure_ssl)
+        session = SslHelper.custom_requests_session(
+            self.opts.skip_cert_verify, self.opts.allow_insecure_ssl, self.opts.use_all_ciphers
+        )
         try:
             response = session.post(
                 f'{self.url_base}login/token.php',
                 data=urllib.parse.urlencode(data),
                 headers=self.RQ_HEADER,
                 timeout=60,
             )
```

### Comparing `moodle_dl-2.3.8/moodle_dl/moodle/result_builder.py` & `moodle_dl-2.3.9/moodle_dl/moodle/result_builder.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.8/moodle_dl/notifications/__init__.py` & `moodle_dl-2.3.9/moodle_dl/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.8/moodle_dl/notifications/console/console_service.py` & `moodle_dl-2.3.9/moodle_dl/notifications/console/console_service.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.8/moodle_dl/notifications/discord/discord_formatter.py` & `moodle_dl-2.3.9/moodle_dl/notifications/discord/discord_formatter.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.8/moodle_dl/notifications/discord/discord_service.py` & `moodle_dl-2.3.9/moodle_dl/notifications/discord/discord_service.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.8/moodle_dl/notifications/discord/discord_shooter.py` & `moodle_dl-2.3.9/moodle_dl/notifications/discord/discord_shooter.py`

 * *Files 15% similar despite different names*

```diff
@@ -33,15 +33,17 @@
                 'username': 'Moodle Notifications',
                 'avatar_url': 'https://i.imgur.com/J3Pxl41.png',
             }
         )
 
     def send_data(self, data: Dict):
 
-        session = SslHelper.custom_requests_session(skip_cert_verify=False, allow_insecure_ssl=False)
+        session = SslHelper.custom_requests_session(
+            skip_cert_verify=False, allow_insecure_ssl=False, use_all_ciphers=False
+        )
         for webhook_url in self.discord_webhooks:
             try:
                 response = session.post(webhook_url, data=json.dumps(data), headers=self.RQ_HEADER, timeout=60)
                 self._check_response_code(response)
             except RequestException as error:
                 raise ConnectionError(f"Connection error: {str(error)}") from None
```

### Comparing `moodle_dl-2.3.8/moodle_dl/notifications/mail/header.png` & `moodle_dl-2.3.9/moodle_dl/notifications/mail/header.png`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.8/moodle_dl/notifications/mail/header_extender.png` & `moodle_dl-2.3.9/moodle_dl/notifications/mail/header_extender.png`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.8/moodle_dl/notifications/mail/mail_formater.py` & `moodle_dl-2.3.9/moodle_dl/notifications/mail/mail_formater.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.8/moodle_dl/notifications/mail/mail_service.py` & `moodle_dl-2.3.9/moodle_dl/notifications/mail/mail_service.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.8/moodle_dl/notifications/mail/mail_shooter.py` & `moodle_dl-2.3.9/moodle_dl/notifications/mail/mail_shooter.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.8/moodle_dl/notifications/notification_service.py` & `moodle_dl-2.3.9/moodle_dl/notifications/notification_service.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.8/moodle_dl/notifications/telegram/telegram_formater.py` & `moodle_dl-2.3.9/moodle_dl/notifications/telegram/telegram_formater.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.8/moodle_dl/notifications/telegram/telegram_service.py` & `moodle_dl-2.3.9/moodle_dl/notifications/telegram/telegram_service.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.8/moodle_dl/notifications/telegram/telegram_shooter.py` & `moodle_dl-2.3.9/moodle_dl/notifications/telegram/telegram_shooter.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,17 @@
 
     def send(self, message: str):
         payload = {'chat_id': self.telegram_chatid, 'text': message, 'parse_mode': 'HTML'}
 
         url = f'https://api.telegram.org/bot{self.telegram_token}/sendMessage'
         data_urlencoded = urllib.parse.urlencode(payload)
 
-        session = SslHelper.custom_requests_session(skip_cert_verify=False, allow_insecure_ssl=False)
+        session = SslHelper.custom_requests_session(
+            skip_cert_verify=False, allow_insecure_ssl=False, use_all_ciphers=False
+        )
         try:
             response = session.post(url, data=data_urlencoded, headers=self.RQ_HEADER, timeout=60)
         except RequestException as error:
             raise ConnectionError(f"Connection error: {str(error)}") from None
 
         self._check_errors(response)
```

### Comparing `moodle_dl-2.3.8/moodle_dl/notifications/xmpp/xmpp_formater.py` & `moodle_dl-2.3.9/moodle_dl/notifications/xmpp/xmpp_formater.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.8/moodle_dl/notifications/xmpp/xmpp_service.py` & `moodle_dl-2.3.9/moodle_dl/notifications/xmpp/xmpp_service.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.8/moodle_dl/notifications/xmpp/xmpp_shooter.py` & `moodle_dl-2.3.9/moodle_dl/notifications/xmpp/xmpp_shooter.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.8/moodle_dl/types.py` & `moodle_dl-2.3.9/moodle_dl/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -268,14 +268,15 @@
     max_parallel_downloads: int
     max_parallel_yt_dlp: int
     download_chunk_size: int
     ignore_ytdl_errors: bool
     without_downloading_files: bool
     max_path_length_workaround: bool
     allow_insecure_ssl: bool
+    use_all_ciphers: bool
     skip_cert_verify: bool
     verbose: bool
     quiet: bool
     log_to_file: bool
     log_file_path: str
```

### Comparing `moodle_dl-2.3.8/moodle_dl/utils.py` & `moodle_dl-2.3.9/moodle_dl/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -782,27 +782,29 @@
             if not os.path.isdir(cert_loc):
                 ssl_context.load_verify_locations(cafile=cert_loc)
             else:
                 ssl_context.load_verify_locations(capath=cert_loc)
 
     @classmethod
     @lru_cache(maxsize=4)
-    def get_ssl_context(cls, skip_cert_verify: bool, allow_insecure_ssl: bool):
+    def get_ssl_context(cls, skip_cert_verify: bool, allow_insecure_ssl: bool, use_all_ciphers: bool):
         if not skip_cert_verify:
             ssl_context = ssl.create_default_context(ssl.Purpose.SERVER_AUTH)
             cls.load_default_certs(ssl_context)
         else:
             ssl_context = ssl._create_unverified_context()  # pylint: disable=protected-access
 
         if allow_insecure_ssl:
             # This allows connections to legacy insecure servers
             # https://www.openssl.org/docs/manmaster/man3/SSL_CTX_set_options.html#SECURE-RENEGOTIATION
             # Be warned the insecure renegotiation allows an attack, see:
             # https://nvd.nist.gov/vuln/detail/CVE-2009-3555
             ssl_context.options |= 0x4  # set ssl.OP_LEGACY_SERVER_CONNECT bit
+        if use_all_ciphers:
+            ssl_context.set_ciphers('ALL')
 
         return ssl_context
 
     class CustomHttpAdapter(requests.adapters.HTTPAdapter):
         '''
         Transport adapter that allows us to use custom ssl_context.
         See https://stackoverflow.com/a/71646353 for more details.
@@ -814,20 +816,20 @@
 
         def init_poolmanager(self, connections, maxsize, block=False, **pool_kwargs):
             self.poolmanager = urllib3.poolmanager.PoolManager(
                 num_pools=connections, maxsize=maxsize, block=block, ssl_context=self.ssl_context, **pool_kwargs
             )
 
     @classmethod
-    def custom_requests_session(cls, skip_cert_verify: bool, allow_insecure_ssl: bool):
+    def custom_requests_session(cls, skip_cert_verify: bool, allow_insecure_ssl: bool, use_all_ciphers: bool):
         """
         Return a new requests session with custom SSL context
         """
         session = requests.Session()
-        ssl_context = cls.get_ssl_context(skip_cert_verify, allow_insecure_ssl)
+        ssl_context = cls.get_ssl_context(skip_cert_verify, allow_insecure_ssl, use_all_ciphers)
         session.mount('https://', cls.CustomHttpAdapter(ssl_context))
         session.verify = not skip_cert_verify
         return session
 
 
 class ProcessLock:
     """
```

### Comparing `moodle_dl-2.3.8/moodle_dl.egg-info/PKG-INFO` & `moodle_dl-2.3.9/moodle_dl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moodle-dl
-Version: 2.3.8
+Version: 2.3.9
 Summary: Moodle-DL downloads course content fast from Moodle (eg. lecture pdfs)
 Home-page: https://github.com/C0D3D3V/Moodle-DL
 Author: C0D3D3V
 Author-email: moodle-dl@ist-ein-knaller.de
 License: GPL-3.0
 Project-URL: Documentation, https://github.com/C0D3D3V/Moodle-DL#readme
 Project-URL: Wiki, https://github.com/C0D3D3V/Moodle-DL/wiki
```

### Comparing `moodle_dl-2.3.8/moodle_dl.egg-info/SOURCES.txt` & `moodle_dl-2.3.9/moodle_dl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.8/setup.py` & `moodle_dl-2.3.9/setup.py`

 * *Files identical despite different names*

