# Comparing `tmp/cobib-5.0.0.tar.gz` & `tmp/cobib-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cobib-5.0.0.tar", last modified: Sun Apr 28 12:09:56 2024, max compression
+gzip compressed data, was "cobib-5.0.1.tar", last modified: Wed May  1 13:46:22 2024, max compression
```

## Comparing `cobib-5.0.0.tar` & `cobib-5.0.1.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-28 12:09:56.750714 cobib-5.0.0/
--rw-r--r--   0 max       (1000) max       (1000)    41947 2024-04-28 12:08:28.000000 cobib-5.0.0/CHANGELOG.md
--rw-r--r--   0 max       (1000) max       (1000)     1076 2024-01-18 21:03:08.000000 cobib-5.0.0/LICENSE.txt
--rw-r--r--   0 max       (1000) max       (1000)      100 2023-06-12 19:22:05.000000 cobib-5.0.0/MANIFEST.in
--rw-r--r--   0 max       (1000) max       (1000)    51364 2024-04-28 12:09:56.750714 cobib-5.0.0/PKG-INFO
--rw-r--r--   0 max       (1000) max       (1000)     8035 2024-03-17 16:27:49.000000 cobib-5.0.0/README.md
--rw-r--r--   0 max       (1000) max       (1000)    35143 2024-04-28 12:07:47.000000 cobib-5.0.0/cobib.1
--rw-r--r--   0 max       (1000) max       (1000)     4580 2024-04-28 11:19:47.000000 cobib-5.0.0/pyproject.toml
--rw-r--r--   0 max       (1000) max       (1000)      135 2024-02-03 16:58:09.000000 cobib-5.0.0/requirements.txt
--rw-r--r--   0 max       (1000) max       (1000)       38 2024-04-28 12:09:56.750714 cobib-5.0.0/setup.cfg
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-28 12:09:56.724048 cobib-5.0.0/src/
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-28 12:09:56.730714 cobib-5.0.0/src/cobib/
--rw-r--r--   0 max       (1000) max       (1000)      474 2024-04-28 12:07:29.000000 cobib-5.0.0/src/cobib/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)      445 2024-03-17 16:27:49.000000 cobib-5.0.0/src/cobib/__main__.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-28 12:09:56.737381 cobib-5.0.0/src/cobib/commands/
--rw-r--r--   0 max       (1000) max       (1000)     1108 2024-03-17 16:27:49.000000 cobib-5.0.0/src/cobib/commands/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)    23338 2024-04-28 11:19:47.000000 cobib-5.0.0/src/cobib/commands/add.py
--rw-r--r--   0 max       (1000) max       (1000)     7015 2024-04-28 11:19:47.000000 cobib-5.0.0/src/cobib/commands/base_command.py
--rw-r--r--   0 max       (1000) max       (1000)     4633 2024-04-28 11:19:47.000000 cobib-5.0.0/src/cobib/commands/delete.py
--rw-r--r--   0 max       (1000) max       (1000)     8699 2024-04-28 11:19:47.000000 cobib-5.0.0/src/cobib/commands/edit.py
--rw-r--r--   0 max       (1000) max       (1000)     7477 2024-04-28 11:19:47.000000 cobib-5.0.0/src/cobib/commands/export.py
--rw-r--r--   0 max       (1000) max       (1000)     3179 2024-04-28 11:19:47.000000 cobib-5.0.0/src/cobib/commands/git.py
--rw-r--r--   0 max       (1000) max       (1000)     7264 2024-04-28 11:19:47.000000 cobib-5.0.0/src/cobib/commands/import_.py
--rw-r--r--   0 max       (1000) max       (1000)     4548 2024-04-28 11:19:47.000000 cobib-5.0.0/src/cobib/commands/init.py
--rw-r--r--   0 max       (1000) max       (1000)     4607 2024-04-28 11:19:47.000000 cobib-5.0.0/src/cobib/commands/lint.py
--rw-r--r--   0 max       (1000) max       (1000)    14510 2024-04-28 11:19:47.000000 cobib-5.0.0/src/cobib/commands/list_.py
--rw-r--r--   0 max       (1000) max       (1000)    21161 2024-04-28 11:19:47.000000 cobib-5.0.0/src/cobib/commands/modify.py
--rw-r--r--   0 max       (1000) max       (1000)    10356 2024-04-28 11:19:47.000000 cobib-5.0.0/src/cobib/commands/open.py
--rw-r--r--   0 max       (1000) max       (1000)     4578 2024-04-28 11:19:47.000000 cobib-5.0.0/src/cobib/commands/redo.py
--rw-r--r--   0 max       (1000) max       (1000)    19498 2024-04-28 11:19:47.000000 cobib-5.0.0/src/cobib/commands/review.py
--rw-r--r--   0 max       (1000) max       (1000)    11513 2024-04-28 11:19:47.000000 cobib-5.0.0/src/cobib/commands/search.py
--rw-r--r--   0 max       (1000) max       (1000)     2211 2024-04-28 11:19:47.000000 cobib-5.0.0/src/cobib/commands/show.py
--rw-r--r--   0 max       (1000) max       (1000)     5275 2024-04-28 11:19:47.000000 cobib-5.0.0/src/cobib/commands/undo.py
--rw-r--r--   0 max       (1000) max       (1000)     2578 2024-04-28 11:19:47.000000 cobib-5.0.0/src/cobib/commands/unify_labels.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-28 12:09:56.740714 cobib-5.0.0/src/cobib/config/
--rw-r--r--   0 max       (1000) max       (1000)     1302 2023-11-12 10:49:04.000000 cobib-5.0.0/src/cobib/config/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     1521 2024-04-28 11:19:47.000000 cobib-5.0.0/src/cobib/config/command.py
--rw-r--r--   0 max       (1000) max       (1000)    42596 2024-04-28 11:19:47.000000 cobib-5.0.0/src/cobib/config/config.py
--rw-r--r--   0 max       (1000) max       (1000)    31459 2024-01-21 19:11:03.000000 cobib-5.0.0/src/cobib/config/event.py
--rw-r--r--   0 max       (1000) max       (1000)    11469 2023-12-12 08:31:55.000000 cobib-5.0.0/src/cobib/config/example.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-28 12:09:56.740714 cobib-5.0.0/src/cobib/database/
--rw-r--r--   0 max       (1000) max       (1000)     1413 2023-11-13 21:18:22.000000 cobib-5.0.0/src/cobib/database/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     4164 2024-04-28 11:19:47.000000 cobib-5.0.0/src/cobib/database/author.py
--rw-r--r--   0 max       (1000) max       (1000)    18110 2024-04-28 11:19:47.000000 cobib-5.0.0/src/cobib/database/database.py
--rw-r--r--   0 max       (1000) max       (1000)    24383 2024-01-21 19:11:03.000000 cobib-5.0.0/src/cobib/database/entry.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-28 12:09:56.740714 cobib-5.0.0/src/cobib/importers/
--rw-r--r--   0 max       (1000) max       (1000)      275 2023-06-12 19:22:05.000000 cobib-5.0.0/src/cobib/importers/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     3051 2024-04-28 11:19:47.000000 cobib-5.0.0/src/cobib/importers/base_importer.py
--rw-r--r--   0 max       (1000) max       (1000)    12895 2024-04-28 11:19:47.000000 cobib-5.0.0/src/cobib/importers/zotero.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-28 12:09:56.744047 cobib-5.0.0/src/cobib/parsers/
--rw-r--r--   0 max       (1000) max       (1000)      520 2023-06-12 19:22:05.000000 cobib-5.0.0/src/cobib/parsers/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     5317 2024-04-28 11:19:47.000000 cobib-5.0.0/src/cobib/parsers/arxiv.py
--rw-r--r--   0 max       (1000) max       (1000)     2034 2023-08-27 11:42:15.000000 cobib-5.0.0/src/cobib/parsers/base_parser.py
--rw-r--r--   0 max       (1000) max       (1000)     3522 2023-11-12 10:49:04.000000 cobib-5.0.0/src/cobib/parsers/bibtex.py
--rw-r--r--   0 max       (1000) max       (1000)     3815 2023-08-27 11:42:15.000000 cobib-5.0.0/src/cobib/parsers/doi.py
--rw-r--r--   0 max       (1000) max       (1000)     4731 2023-12-17 17:15:09.000000 cobib-5.0.0/src/cobib/parsers/isbn.py
--rw-r--r--   0 max       (1000) max       (1000)     3593 2023-12-17 17:15:09.000000 cobib-5.0.0/src/cobib/parsers/url.py
--rw-r--r--   0 max       (1000) max       (1000)     3852 2024-01-21 19:11:03.000000 cobib-5.0.0/src/cobib/parsers/yaml.py
--rw-r--r--   0 max       (1000) max       (1000)        0 2023-06-12 19:22:05.000000 cobib-5.0.0/src/cobib/py.typed
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-28 12:09:56.744047 cobib-5.0.0/src/cobib/ui/
--rw-r--r--   0 max       (1000) max       (1000)      236 2024-03-17 16:27:49.000000 cobib-5.0.0/src/cobib/ui/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     4094 2024-03-17 16:27:49.000000 cobib-5.0.0/src/cobib/ui/cli.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-28 12:09:56.747381 cobib-5.0.0/src/cobib/ui/components/
--rw-r--r--   0 max       (1000) max       (1000)     1043 2024-04-28 11:19:47.000000 cobib-5.0.0/src/cobib/ui/components/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     1911 2024-03-17 16:27:49.000000 cobib-5.0.0/src/cobib/ui/components/entry_points.py
--rw-r--r--   0 max       (1000) max       (1000)      705 2023-06-12 19:22:05.000000 cobib-5.0.0/src/cobib/ui/components/entry_view.py
--rw-r--r--   0 max       (1000) max       (1000)     3287 2023-12-17 17:15:09.000000 cobib-5.0.0/src/cobib/ui/components/help_screen.py
--rw-r--r--   0 max       (1000) max       (1000)     2566 2024-01-14 16:13:13.000000 cobib-5.0.0/src/cobib/ui/components/input_screen.py
--rw-r--r--   0 max       (1000) max       (1000)     4649 2023-12-17 17:15:09.000000 cobib-5.0.0/src/cobib/ui/components/list_view.py
--rw-r--r--   0 max       (1000) max       (1000)     1564 2024-01-14 16:13:13.000000 cobib-5.0.0/src/cobib/ui/components/log_screen.py
--rw-r--r--   0 max       (1000) max       (1000)     2257 2024-01-21 19:11:03.000000 cobib-5.0.0/src/cobib/ui/components/logging_handler.py
--rw-r--r--   0 max       (1000) max       (1000)     2891 2023-12-11 20:47:52.000000 cobib-5.0.0/src/cobib/ui/components/main_content.py
--rw-r--r--   0 max       (1000) max       (1000)      565 2023-06-12 19:22:05.000000 cobib-5.0.0/src/cobib/ui/components/motion_key.py
--rw-r--r--   0 max       (1000) max       (1000)     2731 2023-12-17 17:15:09.000000 cobib-5.0.0/src/cobib/ui/components/preset_filter_screen.py
--rw-r--r--   0 max       (1000) max       (1000)     3908 2023-12-17 17:15:09.000000 cobib-5.0.0/src/cobib/ui/components/search_view.py
--rw-r--r--   0 max       (1000) max       (1000)     1373 2023-12-17 17:15:09.000000 cobib-5.0.0/src/cobib/ui/components/selection_filter.py
--rw-r--r--   0 max       (1000) max       (1000)    21173 2024-03-17 16:27:49.000000 cobib-5.0.0/src/cobib/ui/tui.py
--rw-r--r--   0 max       (1000) max       (1000)     4311 2024-04-28 11:19:47.000000 cobib-5.0.0/src/cobib/ui/ui.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-28 12:09:56.747381 cobib-5.0.0/src/cobib/utils/
--rw-r--r--   0 max       (1000) max       (1000)      242 2023-06-12 19:22:05.000000 cobib-5.0.0/src/cobib/utils/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)      460 2024-01-21 19:11:03.000000 cobib-5.0.0/src/cobib/utils/context.py
--rw-r--r--   0 max       (1000) max       (1000)     6731 2023-06-12 19:22:05.000000 cobib-5.0.0/src/cobib/utils/diff_renderer.py
--rw-r--r--   0 max       (1000) max       (1000)     7574 2024-04-28 11:21:44.000000 cobib-5.0.0/src/cobib/utils/file_downloader.py
--rw-r--r--   0 max       (1000) max       (1000)     4615 2023-12-17 17:15:09.000000 cobib-5.0.0/src/cobib/utils/journal_abbreviations.py
--rw-r--r--   0 max       (1000) max       (1000)     4776 2023-12-17 17:15:09.000000 cobib-5.0.0/src/cobib/utils/logging.py
--rw-r--r--   0 max       (1000) max       (1000)     2998 2024-01-21 19:11:03.000000 cobib-5.0.0/src/cobib/utils/progress.py
--rw-r--r--   0 max       (1000) max       (1000)     9017 2024-04-28 11:19:47.000000 cobib-5.0.0/src/cobib/utils/prompt.py
--rw-r--r--   0 max       (1000) max       (1000)     1860 2023-08-27 11:42:15.000000 cobib-5.0.0/src/cobib/utils/rel_path.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-28 12:09:56.750714 cobib-5.0.0/src/cobib.egg-info/
--rw-r--r--   0 max       (1000) max       (1000)    51364 2024-04-28 12:09:56.000000 cobib-5.0.0/src/cobib.egg-info/PKG-INFO
--rw-r--r--   0 max       (1000) max       (1000)     2366 2024-04-28 12:09:56.000000 cobib-5.0.0/src/cobib.egg-info/SOURCES.txt
--rw-r--r--   0 max       (1000) max       (1000)        1 2024-04-28 12:09:56.000000 cobib-5.0.0/src/cobib.egg-info/dependency_links.txt
--rw-r--r--   0 max       (1000) max       (1000)     1151 2024-04-28 12:09:56.000000 cobib-5.0.0/src/cobib.egg-info/entry_points.txt
--rw-r--r--   0 max       (1000) max       (1000)      135 2024-04-28 12:09:56.000000 cobib-5.0.0/src/cobib.egg-info/requires.txt
--rw-r--r--   0 max       (1000) max       (1000)        6 2024-04-28 12:09:56.000000 cobib-5.0.0/src/cobib.egg-info/top_level.txt
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-28 12:09:56.747381 cobib-5.0.0/tests/
--rw-r--r--   0 max       (1000) max       (1000)     4314 2024-04-28 11:19:47.000000 cobib-5.0.0/tests/test_main.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-01 13:46:22.433230 cobib-5.0.1/
+-rw-r--r--   0 max       (1000) max       (1000)    42185 2024-05-01 13:44:24.000000 cobib-5.0.1/CHANGELOG.md
+-rw-r--r--   0 max       (1000) max       (1000)     1076 2024-01-18 21:03:08.000000 cobib-5.0.1/LICENSE.txt
+-rw-r--r--   0 max       (1000) max       (1000)      100 2023-06-12 19:22:05.000000 cobib-5.0.1/MANIFEST.in
+-rw-r--r--   0 max       (1000) max       (1000)    51602 2024-05-01 13:46:22.433230 cobib-5.0.1/PKG-INFO
+-rw-r--r--   0 max       (1000) max       (1000)     8035 2024-03-17 16:27:49.000000 cobib-5.0.1/README.md
+-rw-r--r--   0 max       (1000) max       (1000)    35143 2024-05-01 13:43:45.000000 cobib-5.0.1/cobib.1
+-rw-r--r--   0 max       (1000) max       (1000)     4580 2024-04-28 11:19:47.000000 cobib-5.0.1/pyproject.toml
+-rw-r--r--   0 max       (1000) max       (1000)      135 2024-02-03 16:58:09.000000 cobib-5.0.1/requirements.txt
+-rw-r--r--   0 max       (1000) max       (1000)       38 2024-05-01 13:46:22.436564 cobib-5.0.1/setup.cfg
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-01 13:46:22.399897 cobib-5.0.1/src/
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-01 13:46:22.403231 cobib-5.0.1/src/cobib/
+-rw-r--r--   0 max       (1000) max       (1000)      474 2024-05-01 13:43:53.000000 cobib-5.0.1/src/cobib/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)      445 2024-03-17 16:27:49.000000 cobib-5.0.1/src/cobib/__main__.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-01 13:46:22.413231 cobib-5.0.1/src/cobib/commands/
+-rw-r--r--   0 max       (1000) max       (1000)     1108 2024-03-17 16:27:49.000000 cobib-5.0.1/src/cobib/commands/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)    23338 2024-04-28 11:19:47.000000 cobib-5.0.1/src/cobib/commands/add.py
+-rw-r--r--   0 max       (1000) max       (1000)     7015 2024-04-28 11:19:47.000000 cobib-5.0.1/src/cobib/commands/base_command.py
+-rw-r--r--   0 max       (1000) max       (1000)     4633 2024-04-28 11:19:47.000000 cobib-5.0.1/src/cobib/commands/delete.py
+-rw-r--r--   0 max       (1000) max       (1000)     8699 2024-04-28 11:19:47.000000 cobib-5.0.1/src/cobib/commands/edit.py
+-rw-r--r--   0 max       (1000) max       (1000)     7477 2024-04-28 11:19:47.000000 cobib-5.0.1/src/cobib/commands/export.py
+-rw-r--r--   0 max       (1000) max       (1000)     3179 2024-04-28 11:19:47.000000 cobib-5.0.1/src/cobib/commands/git.py
+-rw-r--r--   0 max       (1000) max       (1000)     7264 2024-04-28 11:19:47.000000 cobib-5.0.1/src/cobib/commands/import_.py
+-rw-r--r--   0 max       (1000) max       (1000)     4548 2024-04-28 11:19:47.000000 cobib-5.0.1/src/cobib/commands/init.py
+-rw-r--r--   0 max       (1000) max       (1000)     4607 2024-04-28 11:19:47.000000 cobib-5.0.1/src/cobib/commands/lint.py
+-rw-r--r--   0 max       (1000) max       (1000)    14510 2024-04-28 11:19:47.000000 cobib-5.0.1/src/cobib/commands/list_.py
+-rw-r--r--   0 max       (1000) max       (1000)    21161 2024-04-28 11:19:47.000000 cobib-5.0.1/src/cobib/commands/modify.py
+-rw-r--r--   0 max       (1000) max       (1000)    10356 2024-04-28 11:19:47.000000 cobib-5.0.1/src/cobib/commands/open.py
+-rw-r--r--   0 max       (1000) max       (1000)     4578 2024-04-28 11:19:47.000000 cobib-5.0.1/src/cobib/commands/redo.py
+-rw-r--r--   0 max       (1000) max       (1000)    19498 2024-04-28 11:19:47.000000 cobib-5.0.1/src/cobib/commands/review.py
+-rw-r--r--   0 max       (1000) max       (1000)    11513 2024-04-28 11:19:47.000000 cobib-5.0.1/src/cobib/commands/search.py
+-rw-r--r--   0 max       (1000) max       (1000)     2211 2024-04-28 11:19:47.000000 cobib-5.0.1/src/cobib/commands/show.py
+-rw-r--r--   0 max       (1000) max       (1000)     5275 2024-04-28 11:19:47.000000 cobib-5.0.1/src/cobib/commands/undo.py
+-rw-r--r--   0 max       (1000) max       (1000)     2578 2024-04-28 11:19:47.000000 cobib-5.0.1/src/cobib/commands/unify_labels.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-01 13:46:22.413231 cobib-5.0.1/src/cobib/config/
+-rw-r--r--   0 max       (1000) max       (1000)     1302 2023-11-12 10:49:04.000000 cobib-5.0.1/src/cobib/config/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     1521 2024-04-28 11:19:47.000000 cobib-5.0.1/src/cobib/config/command.py
+-rw-r--r--   0 max       (1000) max       (1000)    42794 2024-05-01 13:42:08.000000 cobib-5.0.1/src/cobib/config/config.py
+-rw-r--r--   0 max       (1000) max       (1000)    31459 2024-01-21 19:11:03.000000 cobib-5.0.1/src/cobib/config/event.py
+-rw-r--r--   0 max       (1000) max       (1000)    11469 2023-12-12 08:31:55.000000 cobib-5.0.1/src/cobib/config/example.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-01 13:46:22.416564 cobib-5.0.1/src/cobib/database/
+-rw-r--r--   0 max       (1000) max       (1000)     1413 2023-11-13 21:18:22.000000 cobib-5.0.1/src/cobib/database/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     4164 2024-04-28 11:19:47.000000 cobib-5.0.1/src/cobib/database/author.py
+-rw-r--r--   0 max       (1000) max       (1000)    18110 2024-04-28 11:19:47.000000 cobib-5.0.1/src/cobib/database/database.py
+-rw-r--r--   0 max       (1000) max       (1000)    24383 2024-01-21 19:11:03.000000 cobib-5.0.1/src/cobib/database/entry.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-01 13:46:22.419897 cobib-5.0.1/src/cobib/importers/
+-rw-r--r--   0 max       (1000) max       (1000)      275 2023-06-12 19:22:05.000000 cobib-5.0.1/src/cobib/importers/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     3051 2024-04-28 11:19:47.000000 cobib-5.0.1/src/cobib/importers/base_importer.py
+-rw-r--r--   0 max       (1000) max       (1000)    12895 2024-04-28 11:19:47.000000 cobib-5.0.1/src/cobib/importers/zotero.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-01 13:46:22.423231 cobib-5.0.1/src/cobib/parsers/
+-rw-r--r--   0 max       (1000) max       (1000)      520 2023-06-12 19:22:05.000000 cobib-5.0.1/src/cobib/parsers/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     5317 2024-04-28 11:19:47.000000 cobib-5.0.1/src/cobib/parsers/arxiv.py
+-rw-r--r--   0 max       (1000) max       (1000)     2034 2023-08-27 11:42:15.000000 cobib-5.0.1/src/cobib/parsers/base_parser.py
+-rw-r--r--   0 max       (1000) max       (1000)     3522 2023-11-12 10:49:04.000000 cobib-5.0.1/src/cobib/parsers/bibtex.py
+-rw-r--r--   0 max       (1000) max       (1000)     3815 2023-08-27 11:42:15.000000 cobib-5.0.1/src/cobib/parsers/doi.py
+-rw-r--r--   0 max       (1000) max       (1000)     4731 2023-12-17 17:15:09.000000 cobib-5.0.1/src/cobib/parsers/isbn.py
+-rw-r--r--   0 max       (1000) max       (1000)     3593 2023-12-17 17:15:09.000000 cobib-5.0.1/src/cobib/parsers/url.py
+-rw-r--r--   0 max       (1000) max       (1000)     3852 2024-01-21 19:11:03.000000 cobib-5.0.1/src/cobib/parsers/yaml.py
+-rw-r--r--   0 max       (1000) max       (1000)        0 2023-06-12 19:22:05.000000 cobib-5.0.1/src/cobib/py.typed
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-01 13:46:22.426564 cobib-5.0.1/src/cobib/ui/
+-rw-r--r--   0 max       (1000) max       (1000)      236 2024-03-17 16:27:49.000000 cobib-5.0.1/src/cobib/ui/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     4094 2024-03-17 16:27:49.000000 cobib-5.0.1/src/cobib/ui/cli.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-01 13:46:22.429897 cobib-5.0.1/src/cobib/ui/components/
+-rw-r--r--   0 max       (1000) max       (1000)     1043 2024-04-28 11:19:47.000000 cobib-5.0.1/src/cobib/ui/components/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     1911 2024-03-17 16:27:49.000000 cobib-5.0.1/src/cobib/ui/components/entry_points.py
+-rw-r--r--   0 max       (1000) max       (1000)      705 2023-06-12 19:22:05.000000 cobib-5.0.1/src/cobib/ui/components/entry_view.py
+-rw-r--r--   0 max       (1000) max       (1000)     3287 2023-12-17 17:15:09.000000 cobib-5.0.1/src/cobib/ui/components/help_screen.py
+-rw-r--r--   0 max       (1000) max       (1000)     2566 2024-01-14 16:13:13.000000 cobib-5.0.1/src/cobib/ui/components/input_screen.py
+-rw-r--r--   0 max       (1000) max       (1000)     4649 2023-12-17 17:15:09.000000 cobib-5.0.1/src/cobib/ui/components/list_view.py
+-rw-r--r--   0 max       (1000) max       (1000)     1564 2024-01-14 16:13:13.000000 cobib-5.0.1/src/cobib/ui/components/log_screen.py
+-rw-r--r--   0 max       (1000) max       (1000)     2257 2024-01-21 19:11:03.000000 cobib-5.0.1/src/cobib/ui/components/logging_handler.py
+-rw-r--r--   0 max       (1000) max       (1000)     2891 2023-12-11 20:47:52.000000 cobib-5.0.1/src/cobib/ui/components/main_content.py
+-rw-r--r--   0 max       (1000) max       (1000)      565 2023-06-12 19:22:05.000000 cobib-5.0.1/src/cobib/ui/components/motion_key.py
+-rw-r--r--   0 max       (1000) max       (1000)     2731 2023-12-17 17:15:09.000000 cobib-5.0.1/src/cobib/ui/components/preset_filter_screen.py
+-rw-r--r--   0 max       (1000) max       (1000)     3908 2023-12-17 17:15:09.000000 cobib-5.0.1/src/cobib/ui/components/search_view.py
+-rw-r--r--   0 max       (1000) max       (1000)     1373 2023-12-17 17:15:09.000000 cobib-5.0.1/src/cobib/ui/components/selection_filter.py
+-rw-r--r--   0 max       (1000) max       (1000)    21173 2024-03-17 16:27:49.000000 cobib-5.0.1/src/cobib/ui/tui.py
+-rw-r--r--   0 max       (1000) max       (1000)     4311 2024-04-28 11:19:47.000000 cobib-5.0.1/src/cobib/ui/ui.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-01 13:46:22.433230 cobib-5.0.1/src/cobib/utils/
+-rw-r--r--   0 max       (1000) max       (1000)      242 2023-06-12 19:22:05.000000 cobib-5.0.1/src/cobib/utils/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)      460 2024-01-21 19:11:03.000000 cobib-5.0.1/src/cobib/utils/context.py
+-rw-r--r--   0 max       (1000) max       (1000)     6731 2023-06-12 19:22:05.000000 cobib-5.0.1/src/cobib/utils/diff_renderer.py
+-rw-r--r--   0 max       (1000) max       (1000)     7574 2024-04-28 11:21:44.000000 cobib-5.0.1/src/cobib/utils/file_downloader.py
+-rw-r--r--   0 max       (1000) max       (1000)     4615 2023-12-17 17:15:09.000000 cobib-5.0.1/src/cobib/utils/journal_abbreviations.py
+-rw-r--r--   0 max       (1000) max       (1000)     4776 2023-12-17 17:15:09.000000 cobib-5.0.1/src/cobib/utils/logging.py
+-rw-r--r--   0 max       (1000) max       (1000)     2998 2024-01-21 19:11:03.000000 cobib-5.0.1/src/cobib/utils/progress.py
+-rw-r--r--   0 max       (1000) max       (1000)     9017 2024-04-28 11:19:47.000000 cobib-5.0.1/src/cobib/utils/prompt.py
+-rw-r--r--   0 max       (1000) max       (1000)     1860 2023-08-27 11:42:15.000000 cobib-5.0.1/src/cobib/utils/rel_path.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-01 13:46:22.433230 cobib-5.0.1/src/cobib.egg-info/
+-rw-r--r--   0 max       (1000) max       (1000)    51602 2024-05-01 13:46:22.000000 cobib-5.0.1/src/cobib.egg-info/PKG-INFO
+-rw-r--r--   0 max       (1000) max       (1000)     2366 2024-05-01 13:46:22.000000 cobib-5.0.1/src/cobib.egg-info/SOURCES.txt
+-rw-r--r--   0 max       (1000) max       (1000)        1 2024-05-01 13:46:22.000000 cobib-5.0.1/src/cobib.egg-info/dependency_links.txt
+-rw-r--r--   0 max       (1000) max       (1000)     1151 2024-05-01 13:46:22.000000 cobib-5.0.1/src/cobib.egg-info/entry_points.txt
+-rw-r--r--   0 max       (1000) max       (1000)      135 2024-05-01 13:46:22.000000 cobib-5.0.1/src/cobib.egg-info/requires.txt
+-rw-r--r--   0 max       (1000) max       (1000)        6 2024-05-01 13:46:22.000000 cobib-5.0.1/src/cobib.egg-info/top_level.txt
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-01 13:46:22.433230 cobib-5.0.1/tests/
+-rw-r--r--   0 max       (1000) max       (1000)     4314 2024-04-28 11:19:47.000000 cobib-5.0.1/tests/test_main.py
```

### Comparing `cobib-5.0.0/CHANGELOG.md` & `cobib-5.0.1/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,22 @@
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
 
+## [5.0.1] - 2024-05-01
+
+Pypi: https://pypi.org/project/cobib/5.0.1/
+
+### Fixed
+- the ability to use an empty string as the separator in `config.database.format.label_suffix` (#138)
+
+
 ## [5.0.0] - 2024-04-28
 
 Pypi: https://pypi.org/project/cobib/5.0.0/
 
 ### Added
 
 - the ability to add custom `commands`, `importers`, and `parsers` through entry points (#135, !139)
@@ -988,15 +996,16 @@
 
 ## [0.1] - 2019-04-29
 
 ### Added
 - initial version with a basic `sqlite3`-based database
 
 
-[Unreleased]: https://gitlab.com/cobib/cobib/-/compare/v5.0.0...master
+[Unreleased]: https://gitlab.com/cobib/cobib/-/compare/v5.0.1...master
+[5.0.1]: https://gitlab.com/cobib/cobib/-/tags/v5.0.1
 [5.0.0]: https://gitlab.com/cobib/cobib/-/tags/v5.0.0
 [4.5.0]: https://gitlab.com/cobib/cobib/-/tags/v4.5.0
 [4.4.0]: https://gitlab.com/cobib/cobib/-/tags/v4.4.0
 [4.3.1]: https://gitlab.com/cobib/cobib/-/tags/v4.3.1
 [4.3.0]: https://gitlab.com/cobib/cobib/-/tags/v4.3.0
 [4.2.0]: https://gitlab.com/cobib/cobib/-/tags/v4.2.0
 [4.1.0]: https://gitlab.com/cobib/cobib/-/tags/v4.1.0
```

### Comparing `cobib-5.0.0/LICENSE.txt` & `cobib-5.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cobib-5.0.0/PKG-INFO` & `cobib-5.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cobib
-Version: 5.0.0
+Version: 5.0.1
 Summary: Console Bibliography
 Author-email: Max Rossmannek <max@rossmannek.de>
 License: MIT License
 Project-URL: Homepage, https://gitlab.com/cobib/cobib
 Project-URL: Documentation, https://cobib.gitlab.io/cobib/cobib.html
 Project-URL: Repository, https://gitlab.com/cobib/cobib
 Project-URL: Issues, https://gitlab.com/cobib/cobib/-/issues
@@ -307,14 +307,22 @@
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
 
+## [5.0.1] - 2024-05-01
+
+Pypi: https://pypi.org/project/cobib/5.0.1/
+
+### Fixed
+- the ability to use an empty string as the separator in `config.database.format.label_suffix` (#138)
+
+
 ## [5.0.0] - 2024-04-28
 
 Pypi: https://pypi.org/project/cobib/5.0.0/
 
 ### Added
 
 - the ability to add custom `commands`, `importers`, and `parsers` through entry points (#135, !139)
@@ -1292,15 +1300,16 @@
 
 ## [0.1] - 2019-04-29
 
 ### Added
 - initial version with a basic `sqlite3`-based database
 
 
-[Unreleased]: https://gitlab.com/cobib/cobib/-/compare/v5.0.0...master
+[Unreleased]: https://gitlab.com/cobib/cobib/-/compare/v5.0.1...master
+[5.0.1]: https://gitlab.com/cobib/cobib/-/tags/v5.0.1
 [5.0.0]: https://gitlab.com/cobib/cobib/-/tags/v5.0.0
 [4.5.0]: https://gitlab.com/cobib/cobib/-/tags/v4.5.0
 [4.4.0]: https://gitlab.com/cobib/cobib/-/tags/v4.4.0
 [4.3.1]: https://gitlab.com/cobib/cobib/-/tags/v4.3.1
 [4.3.0]: https://gitlab.com/cobib/cobib/-/tags/v4.3.0
 [4.2.0]: https://gitlab.com/cobib/cobib/-/tags/v4.2.0
 [4.1.0]: https://gitlab.com/cobib/cobib/-/tags/v4.1.0
```

### Comparing `cobib-5.0.0/README.md` & `cobib-5.0.1/README.md`

 * *Files identical despite different names*

### Comparing `cobib-5.0.0/cobib.1` & `cobib-5.0.1/cobib.1`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH COBIB 1 2024-04-28 v5.0.0
+.TH COBIB 1 2024-05-01 v5.0.1
 .SH NAME
 coBib \- Console-based Bibliography Management
 .SH SYNOPSIS
 .B cobib
 [\fB\-\-version\fR]
 [\fB\-h\fR|\fB\-\-help\fR]
 [\fB\-v\fR|\fB\-\-verbose\fR]
```

### Comparing `cobib-5.0.0/pyproject.toml` & `cobib-5.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cobib-5.0.0/src/cobib/commands/__init__.py` & `cobib-5.0.1/src/cobib/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.0/src/cobib/commands/add.py` & `cobib-5.0.1/src/cobib/commands/add.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.0/src/cobib/commands/base_command.py` & `cobib-5.0.1/src/cobib/commands/base_command.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.0/src/cobib/commands/delete.py` & `cobib-5.0.1/src/cobib/commands/delete.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.0/src/cobib/commands/edit.py` & `cobib-5.0.1/src/cobib/commands/edit.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.0/src/cobib/commands/export.py` & `cobib-5.0.1/src/cobib/commands/export.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.0/src/cobib/commands/git.py` & `cobib-5.0.1/src/cobib/commands/git.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.0/src/cobib/commands/import_.py` & `cobib-5.0.1/src/cobib/commands/import_.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.0/src/cobib/commands/init.py` & `cobib-5.0.1/src/cobib/commands/init.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.0/src/cobib/commands/lint.py` & `cobib-5.0.1/src/cobib/commands/lint.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.0/src/cobib/commands/list_.py` & `cobib-5.0.1/src/cobib/commands/list_.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.0/src/cobib/commands/modify.py` & `cobib-5.0.1/src/cobib/commands/modify.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.0/src/cobib/commands/open.py` & `cobib-5.0.1/src/cobib/commands/open.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.0/src/cobib/commands/redo.py` & `cobib-5.0.1/src/cobib/commands/redo.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.0/src/cobib/commands/review.py` & `cobib-5.0.1/src/cobib/commands/review.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.0/src/cobib/commands/search.py` & `cobib-5.0.1/src/cobib/commands/search.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.0/src/cobib/commands/show.py` & `cobib-5.0.1/src/cobib/commands/show.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.0/src/cobib/commands/undo.py` & `cobib-5.0.1/src/cobib/commands/undo.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.0/src/cobib/commands/unify_labels.py` & `cobib-5.0.1/src/cobib/commands/unify_labels.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.0/src/cobib/config/__init__.py` & `cobib-5.0.1/src/cobib/config/__init__.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.0/src/cobib/config/command.py` & `cobib-5.0.1/src/cobib/config/command.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.0/src/cobib/config/config.py` & `cobib-5.0.1/src/cobib/config/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -603,15 +603,20 @@
         Returns:
             The pair of the trimmed label and numeric value of its original suffix.
         """
         # initialize the counter of the suffix
         suffix_value = 0
 
         # try split the suffix from the label using the provided separator
-        *pieces, suffix = label.split(separator)
+        if separator:
+            *pieces, suffix = label.split(separator)
+        else:
+            # no character is used for separation, we simply fall back to using the last one
+            suffix = label[-1]
+            pieces = [label[:-1]]
 
         if pieces:
             # piece together the left-over raw label without its suffix
             raw_label = separator.join(pieces)
             # determine the suffix type of this label
             suffix_type = LabelSuffix.suffix_type(suffix)
```

### Comparing `cobib-5.0.0/src/cobib/config/event.py` & `cobib-5.0.1/src/cobib/config/event.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.0/src/cobib/config/example.py` & `cobib-5.0.1/src/cobib/config/example.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.0/src/cobib/database/__init__.py` & `cobib-5.0.1/src/cobib/database/__init__.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.0/src/cobib/database/author.py` & `cobib-5.0.1/src/cobib/database/author.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.0/src/cobib/database/database.py` & `cobib-5.0.1/src/cobib/database/database.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.0/src/cobib/database/entry.py` & `cobib-5.0.1/src/cobib/database/entry.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.0/src/cobib/importers/base_importer.py` & `cobib-5.0.1/src/cobib/importers/base_importer.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.0/src/cobib/importers/zotero.py` & `cobib-5.0.1/src/cobib/importers/zotero.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.0/src/cobib/parsers/__init__.py` & `cobib-5.0.1/src/cobib/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.0/src/cobib/parsers/arxiv.py` & `cobib-5.0.1/src/cobib/parsers/arxiv.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.0/src/cobib/parsers/base_parser.py` & `cobib-5.0.1/src/cobib/parsers/base_parser.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.0/src/cobib/parsers/bibtex.py` & `cobib-5.0.1/src/cobib/parsers/bibtex.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.0/src/cobib/parsers/doi.py` & `cobib-5.0.1/src/cobib/parsers/doi.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.0/src/cobib/parsers/isbn.py` & `cobib-5.0.1/src/cobib/parsers/isbn.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.0/src/cobib/parsers/url.py` & `cobib-5.0.1/src/cobib/parsers/url.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.0/src/cobib/parsers/yaml.py` & `cobib-5.0.1/src/cobib/parsers/yaml.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.0/src/cobib/ui/cli.py` & `cobib-5.0.1/src/cobib/ui/cli.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.0/src/cobib/ui/components/__init__.py` & `cobib-5.0.1/src/cobib/ui/components/__init__.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.0/src/cobib/ui/components/entry_points.py` & `cobib-5.0.1/src/cobib/ui/components/entry_points.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.0/src/cobib/ui/components/entry_view.py` & `cobib-5.0.1/src/cobib/ui/components/entry_view.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.0/src/cobib/ui/components/help_screen.py` & `cobib-5.0.1/src/cobib/ui/components/help_screen.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.0/src/cobib/ui/components/input_screen.py` & `cobib-5.0.1/src/cobib/ui/components/input_screen.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.0/src/cobib/ui/components/list_view.py` & `cobib-5.0.1/src/cobib/ui/components/list_view.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.0/src/cobib/ui/components/log_screen.py` & `cobib-5.0.1/src/cobib/ui/components/log_screen.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.0/src/cobib/ui/components/logging_handler.py` & `cobib-5.0.1/src/cobib/ui/components/logging_handler.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.0/src/cobib/ui/components/main_content.py` & `cobib-5.0.1/src/cobib/ui/components/main_content.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.0/src/cobib/ui/components/motion_key.py` & `cobib-5.0.1/src/cobib/ui/components/motion_key.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.0/src/cobib/ui/components/preset_filter_screen.py` & `cobib-5.0.1/src/cobib/ui/components/preset_filter_screen.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.0/src/cobib/ui/components/search_view.py` & `cobib-5.0.1/src/cobib/ui/components/search_view.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.0/src/cobib/ui/components/selection_filter.py` & `cobib-5.0.1/src/cobib/ui/components/selection_filter.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.0/src/cobib/ui/tui.py` & `cobib-5.0.1/src/cobib/ui/tui.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.0/src/cobib/ui/ui.py` & `cobib-5.0.1/src/cobib/ui/ui.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.0/src/cobib/utils/diff_renderer.py` & `cobib-5.0.1/src/cobib/utils/diff_renderer.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.0/src/cobib/utils/file_downloader.py` & `cobib-5.0.1/src/cobib/utils/file_downloader.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.0/src/cobib/utils/journal_abbreviations.py` & `cobib-5.0.1/src/cobib/utils/journal_abbreviations.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.0/src/cobib/utils/logging.py` & `cobib-5.0.1/src/cobib/utils/logging.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.0/src/cobib/utils/progress.py` & `cobib-5.0.1/src/cobib/utils/progress.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.0/src/cobib/utils/prompt.py` & `cobib-5.0.1/src/cobib/utils/prompt.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.0/src/cobib/utils/rel_path.py` & `cobib-5.0.1/src/cobib/utils/rel_path.py`

 * *Files identical despite different names*

### Comparing `cobib-5.0.0/src/cobib.egg-info/PKG-INFO` & `cobib-5.0.1/src/cobib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cobib
-Version: 5.0.0
+Version: 5.0.1
 Summary: Console Bibliography
 Author-email: Max Rossmannek <max@rossmannek.de>
 License: MIT License
 Project-URL: Homepage, https://gitlab.com/cobib/cobib
 Project-URL: Documentation, https://cobib.gitlab.io/cobib/cobib.html
 Project-URL: Repository, https://gitlab.com/cobib/cobib
 Project-URL: Issues, https://gitlab.com/cobib/cobib/-/issues
@@ -307,14 +307,22 @@
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
 
+## [5.0.1] - 2024-05-01
+
+Pypi: https://pypi.org/project/cobib/5.0.1/
+
+### Fixed
+- the ability to use an empty string as the separator in `config.database.format.label_suffix` (#138)
+
+
 ## [5.0.0] - 2024-04-28
 
 Pypi: https://pypi.org/project/cobib/5.0.0/
 
 ### Added
 
 - the ability to add custom `commands`, `importers`, and `parsers` through entry points (#135, !139)
@@ -1292,15 +1300,16 @@
 
 ## [0.1] - 2019-04-29
 
 ### Added
 - initial version with a basic `sqlite3`-based database
 
 
-[Unreleased]: https://gitlab.com/cobib/cobib/-/compare/v5.0.0...master
+[Unreleased]: https://gitlab.com/cobib/cobib/-/compare/v5.0.1...master
+[5.0.1]: https://gitlab.com/cobib/cobib/-/tags/v5.0.1
 [5.0.0]: https://gitlab.com/cobib/cobib/-/tags/v5.0.0
 [4.5.0]: https://gitlab.com/cobib/cobib/-/tags/v4.5.0
 [4.4.0]: https://gitlab.com/cobib/cobib/-/tags/v4.4.0
 [4.3.1]: https://gitlab.com/cobib/cobib/-/tags/v4.3.1
 [4.3.0]: https://gitlab.com/cobib/cobib/-/tags/v4.3.0
 [4.2.0]: https://gitlab.com/cobib/cobib/-/tags/v4.2.0
 [4.1.0]: https://gitlab.com/cobib/cobib/-/tags/v4.1.0
```

### Comparing `cobib-5.0.0/src/cobib.egg-info/SOURCES.txt` & `cobib-5.0.1/src/cobib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cobib-5.0.0/src/cobib.egg-info/entry_points.txt` & `cobib-5.0.1/src/cobib.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `cobib-5.0.0/tests/test_main.py` & `cobib-5.0.1/tests/test_main.py`

 * *Files identical despite different names*

