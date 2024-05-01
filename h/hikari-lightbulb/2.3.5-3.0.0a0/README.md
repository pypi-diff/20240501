# Comparing `tmp/hikari-lightbulb-2.3.5.tar.gz` & `tmp/hikari_lightbulb-3.0.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hikari-lightbulb-2.3.5.tar", last modified: Fri Dec  8 20:17:29 2023, max compression
+gzip compressed data, was "hikari_lightbulb-3.0.0a0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `hikari-lightbulb-2.3.5.tar` & `hikari_lightbulb-3.0.0a0.tar`

### file list

```diff
@@ -1,63 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 20:17:29.855943 hikari-lightbulb-2.3.5/
--rw-r--r--   0 runner    (1001) docker     (127)     7642 2023-12-08 20:17:21.000000 hikari-lightbulb-2.3.5/COPYING.LESSER.md
--rw-r--r--   0 runner    (1001) docker     (127)    34915 2023-12-08 20:17:21.000000 hikari-lightbulb-2.3.5/COPYING.md
--rw-r--r--   0 runner    (1001) docker     (127)      161 2023-12-08 20:17:21.000000 hikari-lightbulb-2.3.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3714 2023-12-08 20:17:29.855943 hikari-lightbulb-2.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2023-12-08 20:17:21.000000 hikari-lightbulb-2.3.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-12-08 20:17:21.000000 hikari-lightbulb-2.3.5/crontrigger_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 20:17:29.855943 hikari-lightbulb-2.3.5/hikari_lightbulb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3714 2023-12-08 20:17:29.000000 hikari-lightbulb-2.3.5/hikari_lightbulb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2023-12-08 20:17:29.000000 hikari-lightbulb-2.3.5/hikari_lightbulb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-08 20:17:29.000000 hikari-lightbulb-2.3.5/hikari_lightbulb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-08 20:17:29.000000 hikari-lightbulb-2.3.5/hikari_lightbulb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       74 2023-12-08 20:17:29.000000 hikari-lightbulb-2.3.5/hikari_lightbulb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-12-08 20:17:29.000000 hikari-lightbulb-2.3.5/hikari_lightbulb.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 20:17:29.851943 hikari-lightbulb-2.3.5/lightbulb/
--rw-r--r--   0 runner    (1001) docker     (127)     5027 2023-12-08 20:17:21.000000 hikari-lightbulb-2.3.5/lightbulb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2023-12-08 20:17:21.000000 hikari-lightbulb-2.3.5/lightbulb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    53971 2023-12-08 20:17:21.000000 hikari-lightbulb-2.3.5/lightbulb/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     5186 2023-12-08 20:17:21.000000 hikari-lightbulb-2.3.5/lightbulb/buckets.py
--rw-r--r--   0 runner    (1001) docker     (127)    25446 2023-12-08 20:17:21.000000 hikari-lightbulb-2.3.5/lightbulb/checks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 20:17:29.851943 hikari-lightbulb-2.3.5/lightbulb/commands/
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2023-12-08 20:17:21.000000 hikari-lightbulb-2.3.5/lightbulb/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35937 2023-12-08 20:17:21.000000 hikari-lightbulb-2.3.5/lightbulb/commands/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2023-12-08 20:17:21.000000 hikari-lightbulb-2.3.5/lightbulb/commands/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     8966 2023-12-08 20:17:21.000000 hikari-lightbulb-2.3.5/lightbulb/commands/prefix.py
--rw-r--r--   0 runner    (1001) docker     (127)    10093 2023-12-08 20:17:21.000000 hikari-lightbulb-2.3.5/lightbulb/commands/slash.py
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2023-12-08 20:17:21.000000 hikari-lightbulb-2.3.5/lightbulb/commands/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 20:17:29.855943 hikari-lightbulb-2.3.5/lightbulb/context/
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2023-12-08 20:17:21.000000 hikari-lightbulb-2.3.5/lightbulb/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23693 2023-12-08 20:17:21.000000 hikari-lightbulb-2.3.5/lightbulb/context/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2023-12-08 20:17:21.000000 hikari-lightbulb-2.3.5/lightbulb/context/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     6256 2023-12-08 20:17:21.000000 hikari-lightbulb-2.3.5/lightbulb/context/prefix.py
--rw-r--r--   0 runner    (1001) docker     (127)     5090 2023-12-08 20:17:21.000000 hikari-lightbulb-2.3.5/lightbulb/context/slash.py
--rw-r--r--   0 runner    (1001) docker     (127)     2752 2023-12-08 20:17:21.000000 hikari-lightbulb-2.3.5/lightbulb/context/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 20:17:29.855943 hikari-lightbulb-2.3.5/lightbulb/converters/
--rw-r--r--   0 runner    (1001) docker     (127)     2292 2023-12-08 20:17:21.000000 hikari-lightbulb-2.3.5/lightbulb/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2023-12-08 20:17:21.000000 hikari-lightbulb-2.3.5/lightbulb/converters/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    12242 2023-12-08 20:17:21.000000 hikari-lightbulb-2.3.5/lightbulb/converters/special.py
--rw-r--r--   0 runner    (1001) docker     (127)     4573 2023-12-08 20:17:21.000000 hikari-lightbulb-2.3.5/lightbulb/cooldown_algorithms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3817 2023-12-08 20:17:21.000000 hikari-lightbulb-2.3.5/lightbulb/cooldowns.py
--rw-r--r--   0 runner    (1001) docker     (127)    20784 2023-12-08 20:17:21.000000 hikari-lightbulb-2.3.5/lightbulb/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    10707 2023-12-08 20:17:21.000000 hikari-lightbulb-2.3.5/lightbulb/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     6282 2023-12-08 20:17:21.000000 hikari-lightbulb-2.3.5/lightbulb/events.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 20:17:29.847943 hikari-lightbulb-2.3.5/lightbulb/ext/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 20:17:29.855943 hikari-lightbulb-2.3.5/lightbulb/ext/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)    16770 2023-12-08 20:17:21.000000 hikari-lightbulb-2.3.5/lightbulb/ext/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4975 2023-12-08 20:17:21.000000 hikari-lightbulb-2.3.5/lightbulb/ext/tasks/triggers.py
--rw-r--r--   0 runner    (1001) docker     (127)    13862 2023-12-08 20:17:21.000000 hikari-lightbulb-2.3.5/lightbulb/help_command.py
--rw-r--r--   0 runner    (1001) docker     (127)    12784 2023-12-08 20:17:21.000000 hikari-lightbulb-2.3.5/lightbulb/internal.py
--rw-r--r--   0 runner    (1001) docker     (127)    10459 2023-12-08 20:17:21.000000 hikari-lightbulb-2.3.5/lightbulb/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    13185 2023-12-08 20:17:21.000000 hikari-lightbulb-2.3.5/lightbulb/plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-08 20:17:21.000000 hikari-lightbulb-2.3.5/lightbulb/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 20:17:29.855943 hikari-lightbulb-2.3.5/lightbulb/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2023-12-08 20:17:21.000000 hikari-lightbulb-2.3.5/lightbulb/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2023-12-08 20:17:21.000000 hikari-lightbulb-2.3.5/lightbulb/utils/data_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    19662 2023-12-08 20:17:21.000000 hikari-lightbulb-2.3.5/lightbulb/utils/nav.py
--rw-r--r--   0 runner    (1001) docker     (127)    11384 2023-12-08 20:17:21.000000 hikari-lightbulb-2.3.5/lightbulb/utils/pag.py
--rw-r--r--   0 runner    (1001) docker     (127)     3348 2023-12-08 20:17:21.000000 hikari-lightbulb-2.3.5/lightbulb/utils/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2666 2023-12-08 20:17:21.000000 hikari-lightbulb-2.3.5/lightbulb/utils/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2023-12-08 20:17:21.000000 hikari-lightbulb-2.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-12-08 20:17:21.000000 hikari-lightbulb-2.3.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-08 20:17:29.855943 hikari-lightbulb-2.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3148 2023-12-08 20:17:21.000000 hikari-lightbulb-2.3.5/setup.py
+-rw-r--r--   0        0        0     2120 2023-12-23 18:35:18.886800 hikari_lightbulb-3.0.0a0/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      153 2023-12-23 18:35:18.886881 hikari_lightbulb-3.0.0a0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     1019 2023-12-23 18:35:18.886949 hikari_lightbulb-3.0.0a0/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0        0        0      225 2023-12-23 18:35:18.887008 hikari_lightbulb-3.0.0a0/.github/dependabot.yml
+-rw-r--r--   0        0        0      443 2023-12-23 18:35:18.887085 hikari_lightbulb-3.0.0a0/.github/pull_request_template.md
+-rw-r--r--   0        0        0     1125 2024-02-16 18:45:30.187132 hikari_lightbulb-3.0.0a0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1609 2024-05-01 09:27:21.756678 hikari_lightbulb-3.0.0a0/.github/workflows/deploy.yml
+-rw-r--r--   0        0        0      533 2024-03-30 14:04:16.542574 hikari_lightbulb-3.0.0a0/.gitignore
+-rw-r--r--   0        0        0      594 2024-02-25 11:02:00.204228 hikari_lightbulb-3.0.0a0/.readthedocs.yml
+-rw-r--r--   0        0        0     1062 2023-12-29 22:20:58.590560 hikari_lightbulb-3.0.0a0/LICENSE
+-rw-r--r--   0        0        0       98 2024-02-27 11:58:55.083188 hikari_lightbulb-3.0.0a0/MANIFEST.in
+-rw-r--r--   0        0        0     2453 2024-02-16 21:07:59.938513 hikari_lightbulb-3.0.0a0/README.md
+-rw-r--r--   0        0        0      224 2023-12-23 18:35:18.888203 hikari_lightbulb-3.0.0a0/docs/source/_static/theme_overrides.css
+-rw-r--r--   0        0        0      361 2023-12-23 18:35:18.889078 hikari_lightbulb-3.0.0a0/docs/source/changelog.rst
+-rw-r--r--   0        0        0     7715 2023-12-23 18:35:18.889256 hikari_lightbulb-3.0.0a0/docs/source/changelogs/v0-changelog.rst
+-rw-r--r--   0        0        0     6491 2023-12-23 18:35:18.889366 hikari_lightbulb-3.0.0a0/docs/source/changelogs/v1-changelog.rst
+-rw-r--r--   0        0        0    11582 2023-12-23 18:35:18.889481 hikari_lightbulb-3.0.0a0/docs/source/changelogs/v2-changelog.rst
+-rw-r--r--   0        0        0     2356 2023-12-23 18:35:18.889551 hikari_lightbulb-3.0.0a0/docs/source/conf.py
+-rw-r--r--   0        0        0     2981 2024-03-31 11:50:42.789192 hikari_lightbulb-3.0.0a0/docs/source/getting-started.rst
+-rw-r--r--   0        0        0      479 2024-03-31 22:57:23.557826 hikari_lightbulb-3.0.0a0/docs/source/guide.rst
+-rw-r--r--   0        0        0     5198 2024-03-31 22:57:23.558721 hikari_lightbulb-3.0.0a0/docs/source/guides/application-commands.rst
+-rw-r--r--   0        0        0     5698 2024-03-31 22:57:23.559968 hikari_lightbulb-3.0.0a0/docs/source/guides/command-groups.rst
+-rw-r--r--   0        0        0     9958 2024-03-31 22:57:23.560793 hikari_lightbulb-3.0.0a0/docs/source/guides/commands.rst
+-rw-r--r--   0        0        0     3221 2024-03-31 22:57:23.561081 hikari_lightbulb-3.0.0a0/docs/source/guides/custom-help.rst
+-rw-r--r--   0        0        0     3938 2024-03-31 22:57:23.561365 hikari_lightbulb-3.0.0a0/docs/source/guides/error-handling.rst
+-rw-r--r--   0        0        0     2660 2024-03-31 22:57:23.561606 hikari_lightbulb-3.0.0a0/docs/source/guides/extensions.rst
+-rw-r--r--   0        0        0     5840 2024-03-31 22:57:23.561852 hikari_lightbulb-3.0.0a0/docs/source/guides/plugins.rst
+-rw-r--r--   0        0        0      529 2024-02-16 16:32:16.354005 hikari_lightbulb-3.0.0a0/docs/source/hikari-basics.rst
+-rw-r--r--   0        0        0       45 2023-12-23 18:35:18.890360 hikari_lightbulb-3.0.0a0/docs/source/hikari_basics/api-requests.rst
+-rw-r--r--   0        0        0       24 2023-12-23 18:35:18.890406 hikari_lightbulb-3.0.0a0/docs/source/hikari_basics/cache.rst
+-rw-r--r--   0        0        0     4642 2023-12-23 18:35:18.890472 hikari_lightbulb-3.0.0a0/docs/source/hikari_basics/components.rst
+-rw-r--r--   0        0        0     2477 2023-12-23 18:35:18.890527 hikari_lightbulb-3.0.0a0/docs/source/hikari_basics/embeds.rst
+-rw-r--r--   0        0        0     2818 2023-12-23 18:35:18.890583 hikari_lightbulb-3.0.0a0/docs/source/hikari_basics/intents.rst
+-rw-r--r--   0        0        0     2596 2024-03-31 22:57:23.562285 hikari_lightbulb-3.0.0a0/docs/source/index.rst
+-rw-r--r--   0        0        0     1940 2023-12-23 18:35:18.890772 hikari_lightbulb-3.0.0a0/examples/basic_bot_example.py
+-rw-r--r--   0        0        0     1322 2023-12-23 18:35:18.890832 hikari_lightbulb-3.0.0a0/examples/basic_slash_command_bot_example.py
+-rw-r--r--   0        0        0     1201 2023-12-23 18:35:18.890940 hikari_lightbulb-3.0.0a0/examples/extension_example.py
+-rw-r--r--   0        0        0     7819 2023-12-23 18:35:18.891014 hikari_lightbulb-3.0.0a0/examples/in_depth_component_example.py
+-rw-r--r--   0        0        0     3040 2023-12-23 18:35:18.891075 hikari_lightbulb-3.0.0a0/examples/moderation_example.py
+-rw-r--r--   0        0        0     1203 2023-12-23 18:35:18.891123 hikari_lightbulb-3.0.0a0/examples/plugin_example.py
+-rw-r--r--   0        0        0     2265 2024-05-01 09:25:32.372131 hikari_lightbulb-3.0.0a0/lightbulb/__init__.py
+-rw-r--r--   0        0        0     1277 2024-02-16 09:16:24.536640 hikari_lightbulb-3.0.0a0/lightbulb/__main__.py
+-rw-r--r--   0        0        0    37462 2024-05-01 09:04:31.448804 hikari_lightbulb-3.0.0a0/lightbulb/client.py
+-rw-r--r--   0        0        0     1730 2024-02-19 22:58:21.810870 hikari_lightbulb-3.0.0a0/lightbulb/commands/__init__.py
+-rw-r--r--   0        0        0    23253 2024-03-21 20:35:15.382501 hikari_lightbulb-3.0.0a0/lightbulb/commands/commands.py
+-rw-r--r--   0        0        0    13156 2024-04-28 18:39:43.776876 hikari_lightbulb-3.0.0a0/lightbulb/commands/execution.py
+-rw-r--r--   0        0        0     9264 2024-03-21 20:35:15.382368 hikari_lightbulb-3.0.0a0/lightbulb/commands/groups.py
+-rw-r--r--   0        0        0    25750 2024-04-12 18:17:10.714475 hikari_lightbulb-3.0.0a0/lightbulb/commands/options.py
+-rw-r--r--   0        0        0     2628 2024-03-21 20:34:17.621001 hikari_lightbulb-3.0.0a0/lightbulb/commands/utils.py
+-rw-r--r--   0        0        0    24390 2024-03-10 17:35:04.283324 hikari_lightbulb-3.0.0a0/lightbulb/context.py
+-rw-r--r--   0        0        0     3248 2024-04-14 14:34:30.540538 hikari_lightbulb-3.0.0a0/lightbulb/exceptions.py
+-rw-r--r--   0        0        0     1259 2024-03-19 09:53:20.890938 hikari_lightbulb-3.0.0a0/lightbulb/internal/__init__.py
+-rw-r--r--   0        0        0     1346 2024-03-07 11:49:30.419107 hikari_lightbulb-3.0.0a0/lightbulb/internal/constants.py
+-rw-r--r--   0        0        0     9166 2024-03-30 13:59:30.625614 hikari_lightbulb-3.0.0a0/lightbulb/internal/di.py
+-rw-r--r--   0        0        0     8327 2024-03-21 20:34:17.631935 hikari_lightbulb-3.0.0a0/lightbulb/internal/sync.py
+-rw-r--r--   0        0        0     1218 2024-03-19 09:53:20.859314 hikari_lightbulb-3.0.0a0/lightbulb/internal/types.py
+-rw-r--r--   0        0        0     2343 2024-03-21 21:40:49.069734 hikari_lightbulb-3.0.0a0/lightbulb/internal/utils.py
+-rw-r--r--   0        0        0    11288 2024-04-14 15:21:31.545705 hikari_lightbulb-3.0.0a0/lightbulb/loaders.py
+-rw-r--r--   0        0        0     5240 2024-03-29 10:53:40.891687 hikari_lightbulb-3.0.0a0/lightbulb/localization.py
+-rw-r--r--   0        0        0        0 2024-02-16 14:14:10.382578 hikari_lightbulb-3.0.0a0/lightbulb/py.typed
+-rw-r--r--   0        0        0     4940 2024-03-10 17:35:21.236647 hikari_lightbulb-3.0.0a0/lightbulb/utils.py
+-rw-r--r--   0        0        0     2466 2024-03-06 10:38:16.235164 hikari_lightbulb-3.0.0a0/noxfile.py
+-rw-r--r--   0        0        0     4593 2024-05-01 08:56:08.766749 hikari_lightbulb-3.0.0a0/pyproject.toml
+-rw-r--r--   0        0        0     2907 2024-05-01 09:27:21.750262 hikari_lightbulb-3.0.0a0/scripts/deploy/update_version.py
+-rw-r--r--   0        0        0     5417 2024-04-04 00:41:01.681666 hikari_lightbulb-3.0.0a0/scripts/docs/api_reference_generator.py
+-rw-r--r--   0        0        0     4539 1970-01-01 00:00:00.000000 hikari_lightbulb-3.0.0a0/PKG-INFO
```

### Comparing `hikari-lightbulb-2.3.5/README.md` & `hikari_lightbulb-3.0.0a0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -12,31 +12,37 @@
 
 ```bash
 pip install hikari-lightbulb
 ```
 
 ## Usage
 ```python
-# Import the command handler
+# Import the libraries
+import hikari
 import lightbulb
 
-# Instantiate a Bot instance
-bot = lightbulb.BotApp(token="your_token_here", prefix="your_prefix_here")
-
-# Register the command to the bot
-@bot.command
-# Use the command decorator to convert the function into a command
-@lightbulb.command("ping", "checks the bot is alive")
-# Define the command type(s) that this command implements
-@lightbulb.implements(lightbulb.PrefixCommand)
-# Define the command's callback. The callback should take a single argument which will be
-# an instance of a subclass of lightbulb.context.Context when passed in
-async def ping(ctx: lightbulb.Context) -> None:
-    # Send a message to the channel the command was used in
-    await ctx.respond("Pong!")
+# Create a GatewayBot instance
+bot = hikari.GatewayBot("your_token_here")
+client = lightbulb.client_from_app(bot)
+
+# Register the command with the client
+@client.register()
+class Ping(
+    # Command type - builtins include SlashCommand, UserCommand, and MessageCommand
+    lightbulb.SlashCommand,
+    # Command declaration parameters
+    name="ping",
+    description="checks the bot is alive",
+):
+    # Define the command's invocation method. This method must take the context as the first
+    # argument (excluding self) which contains information about the command invocation.
+    @lightbulb.invoke
+    async def invoke(self, ctx: lightbulb.Context) -> None:
+        # Send a message to the channel the command was used in
+        await ctx.respond("Pong!")
 
 # Run the bot
 # Note that this is blocking meaning no code after this line will run
 # until the bot is shut off
 bot.run()
 ```
 
@@ -51,10 +57,10 @@
 Please try to update tests as appropriate and ensure that documentation is updated if
 you add any features accessible through the public API.
 
 If you use this library and like it, feel free to sign up to GitHub and star the project,
 it is greatly appreciated and lets me know that I'm going in the right direction!
 
 ## Links
-- **License:** [LGPLv3](https://choosealicense.com/licenses/lgpl-3.0/)
+- **License:** [MIT](https://choosealicense.com/licenses/mit/)
 - **Repository:** [GitHub](https://github.com/tandemdude/hikari-lightbulb)
 - **Documentation:** [ReadTheDocs](https://hikari-lightbulb.readthedocs.io/en/latest/)
```

### Comparing `hikari-lightbulb-2.3.5/lightbulb/__main__.py` & `hikari_lightbulb-3.0.0a0/examples/extension_example.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,14 +11,26 @@
 # Lightbulb is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with Lightbulb. If not, see <https://www.gnu.org/licenses/>.
-import importlib
-import sys
-
 import lightbulb
 
-sys.stderr.write(f"hikari-lightbulb ({lightbulb.__version__})\n")
-importlib.import_module("hikari.__main__")
+example_plugin = lightbulb.Plugin("ExamplePlugin")
+
+
+@example_plugin.command()
+@lightbulb.command("ping", "Checks that the bot is alive")
+@lightbulb.implements(lightbulb.PrefixCommand, lightbulb.SlashCommand)
+async def ping(ctx: lightbulb.Context) -> None:
+    """Checks that the bot is alive"""
+    await ctx.respond("Pong!")
+
+
+def load(bot):
+    bot.add_plugin(example_plugin)
+
+
+def unload(bot):
+    bot.remove_plugin(example_plugin)
```

### Comparing `hikari-lightbulb-2.3.5/lightbulb/commands/base.py` & `hikari_lightbulb-3.0.0a0/lightbulb/client.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,963 +1,888 @@
 # -*- coding: utf-8 -*-
-# Copyright © tandemdude 2020-present
+# Copyright (c) 2023-present tandemdude
 #
-# This file is part of Lightbulb.
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
 #
-# Lightbulb is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Lesser General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
 #
-# Lightbulb is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Lesser General Public License for more details.
-#
-# You should have received a copy of the GNU Lesser General Public License
-# along with Lightbulb. If not, see <https://www.gnu.org/licenses/>.
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
 from __future__ import annotations
 
-__all__ = ["OptionModifier", "OptionLike", "CommandLike", "Command", "ApplicationCommand", "SubCommandTrait"]
+__all__ = ["Client", "GatewayEnabledClient", "RestEnabledClient", "client_from_app"]
 
-import abc
 import asyncio
 import collections
-import datetime
-import enum
-import inspect
-import re
+import functools
+import importlib
+import logging
+import pathlib
 import typing as t
 
-import attrs
 import hikari
 
-from lightbulb import errors
+from lightbulb import context as context_
+from lightbulb import exceptions
+from lightbulb import loaders
+from lightbulb import localization
+from lightbulb.commands import commands
+from lightbulb.commands import execution
+from lightbulb.commands import groups
+from lightbulb.internal import constants
+from lightbulb.internal import di as di_
+from lightbulb.internal import sync
+from lightbulb.internal import utils
 
 if t.TYPE_CHECKING:
-    from lightbulb import app as app_
-    from lightbulb import buckets
-    from lightbulb import checks
-    from lightbulb import context as context_
-    from lightbulb import cooldowns
-    from lightbulb import events
-    from lightbulb import parser as parser_
-    from lightbulb import plugins
-
-_AutocompleteableOptionT = t.Union[str, int, float]
-AutocompleteCallbackT = t.TypeVar(
-    "AutocompleteCallbackT",
-    bound=t.Callable[
-        ...,
-        t.Coroutine[
-            t.Any,
-            t.Any,
-            t.Union[
-                _AutocompleteableOptionT,
-                hikari.api.AutocompleteChoiceBuilder,
-                t.Sequence[t.Union[_AutocompleteableOptionT, hikari.api.AutocompleteChoiceBuilder]],
-            ],
-        ],
-    ],
-)
-ErrorHandlerCallbackT = t.TypeVar(
-    "ErrorHandlerCallbackT", bound=t.Callable[..., t.Coroutine[t.Any, t.Any, t.Optional[bool]]]
-)
+    import types
 
+    from lightbulb.commands import options
+    from lightbulb.internal.types import MaybeAwaitable
 
-class CommandCallbackT(t.Protocol):
-    def __call__(self, context: context_.base.Context, **kwargs: t.Any) -> t.Coroutine[t.Any, t.Any, None]:
-        ...
-
-
-OPTION_TYPE_MAPPING = {
-    str: hikari.OptionType.STRING,
-    int: hikari.OptionType.INTEGER,
-    float: hikari.OptionType.FLOAT,
-    bool: hikari.OptionType.BOOLEAN,
-    hikari.User: hikari.OptionType.USER,
-    hikari.Member: hikari.OptionType.USER,
-    hikari.GuildChannel: hikari.OptionType.CHANNEL,
-    hikari.TextableGuildChannel: hikari.OptionType.CHANNEL,
-    hikari.TextableChannel: hikari.OptionType.CHANNEL,
-    hikari.GuildCategory: hikari.OptionType.CHANNEL,
-    hikari.GuildVoiceChannel: hikari.OptionType.CHANNEL,
-    hikari.Role: hikari.OptionType.ROLE,
-    hikari.Emoji: hikari.OptionType.STRING,
-    hikari.Guild: hikari.OptionType.STRING,
-    hikari.Message: hikari.OptionType.STRING,
-    hikari.Invite: hikari.OptionType.STRING,
-    hikari.Colour: hikari.OptionType.STRING,
-    hikari.Color: hikari.OptionType.STRING,
-    hikari.Snowflake: hikari.OptionType.STRING,
-    datetime.datetime: hikari.OptionType.STRING,
-    hikari.Attachment: hikari.OptionType.ATTACHMENT,
-}
-OPTION_NAME_REGEX: re.Pattern[str] = re.compile(r"^[\w-]{1,32}$", re.U)
-
-
-class _HasRecreateSubcommands(t.Protocol):
-    app: app_.BotApp
-
-    def recreate_subcommands(self, raw_cmds: t.Sequence[CommandLike], app: app_.BotApp) -> None:
-        ...
-
-
-class _SubcommandListProxy(collections.UserList):  # type: ignore
-    def __init__(self, *args: t.Any, parent: _HasRecreateSubcommands, **kwargs: t.Any) -> None:
-        super().__init__(*args, **kwargs)
-        self.parents = [parent]
-
-    def append(self, item: t.Any) -> None:
-        super().append(item)
-        for parent in self.parents:
-            parent.recreate_subcommands(self.data, parent.app)
-
-    def add_parent(self, parent: _HasRecreateSubcommands) -> _SubcommandListProxy:
-        self.parents.append(parent)
-        return self
-
-
-def _get_choice_objects_from_choices(
-    choices: t.Sequence[t.Union[str, int, float, hikari.CommandChoice]]
-) -> t.Sequence[hikari.CommandChoice]:
-    return [c if isinstance(c, hikari.CommandChoice) else hikari.CommandChoice(name=str(c), value=c) for c in choices]
-
-
-class OptionModifier(enum.Enum):
-    """Enum representing option modifiers that affect parsing for prefix commands."""
-
-    NONE = enum.auto()
-    """No modifier. This will be parsed as a normal argument."""
-    GREEDY = enum.auto()
-    """Greedy option. This will consume arguments until the string is exhausted or conversion fails."""
-    CONSUME_REST = enum.auto()
-    """Consume rest option. This will consume the entire remainder of the string."""
+T = t.TypeVar("T")
+CommandMap: t.TypeAlias = t.MutableMapping[hikari.Snowflakeish, t.MutableMapping[str, utils.CommandCollection]]
+CommandOrGroup: t.TypeAlias = t.Union[groups.Group, type[commands.CommandBase]]
+CommandOrGroupT = t.TypeVar("CommandOrGroupT", bound=CommandOrGroup)
+ErrorHandler: t.TypeAlias = t.Callable[
+    t.Concatenate[exceptions.ExecutionPipelineFailedException, ...], t.Awaitable[bool]
+]
+ErrorHandlerT = t.TypeVar("ErrorHandlerT", bound=ErrorHandler)
+OptionT = t.TypeVar("OptionT", bound=hikari.CommandInteractionOption)
+
+LOGGER = logging.getLogger("lightbulb.client")
+DEFAULT_EXECUTION_STEP_ORDER = (
+    execution.ExecutionSteps.MAX_CONCURRENCY,
+    execution.ExecutionSteps.CHECKS,
+    execution.ExecutionSteps.COOLDOWNS,
+    execution.ExecutionSteps.INVOKE,
+    execution.ExecutionSteps.POST_INVOKE,
+)
 
 
-@attrs.define(slots=True)
-class OptionLike:
-    """
-    Generic dataclass representing a command option. Compatible with both prefix and application commands.
-    """
+@t.runtime_checkable
+class GatewayClientAppT(hikari.EventManagerAware, hikari.RESTAware, t.Protocol):
+    """Protocol indicating an application supports gateway events."""
 
-    name: str
-    """The name of the option."""
-    description: str
-    """The description of the option"""
-    arg_type: t.Any = str
-    """The type of the option."""
-    required: bool = True
-    """Whether or not the option is required. This will be inferred from whether or not
-    a default value was provided if unspecified."""
-    choices: t.Optional[t.Sequence[t.Union[str, int, float, hikari.CommandChoice]]] = None
-    """The option's choices. This only affects slash commands."""
-    channel_types: t.Optional[t.Sequence[hikari.ChannelType]] = None
-    """The channel types for this option. This only affects slash commands."""
-    default: hikari.UndefinedOr[t.Any] = hikari.UNDEFINED
-    """The default value for this option."""
-    modifier: OptionModifier = OptionModifier.NONE
-    """Additional modifier controlling how the option should be parsed. This only affects prefix commands."""
-    min_value: t.Optional[t.Union[float, int]] = None
-    """
-    The minimum value permitted for this option (inclusive). The option must be ``INTEGER`` or ``FLOAT`` to use this.
 
-    .. versionadded:: 2.1.3
-    """
-    max_value: t.Optional[t.Union[float, int]] = None
-    """
-    The maximum value permitted for this option (inclusive). The option must be ``INTEGER`` or ``FLOAT`` to use this.
+@t.runtime_checkable
+class RestClientAppT(hikari.InteractionServerAware, hikari.RESTAware, t.Protocol):
+    """Protocol indicating an application supports an interaction server."""
 
-    .. versionadded:: 2.1.3
-    """
-    min_length: t.Optional[int] = None
-    """
-    The minimum length permitted for this option. The option must be ``STRING`` to use this.
 
-    .. versionadded:: 2.3.2
+class Client:
     """
-    max_length: t.Optional[int] = None
-    """
-    The maximum length permitted for this option. The option must be ``STRING`` to use this.
+    Base client implementation supporting generic application command handling.
 
-    .. versionadded:: 2.3.2
-    """
-    autocomplete: bool = False
-    """Whether the option should be autocompleted or not. This only affects slash commands."""
-    name_localizations: t.Mapping[t.Union[hikari.Locale, str], str] = attrs.field(factory=dict)
+    Args:
+        rest (:obj:`~hikari.api.RESTClient`): The rest client to use.
+        default_enabled_guilds (:obj:`~typing.Sequence` [ :obj:`~hikari.Snowflakeish` ]): The guilds that application
+            commands should be created in by default. Can be overridden on a per-command basis.
+        execution_step_order (:obj:`~typing.Sequence` [ :obj:`~lightbulb.commands.execution.ExecutionStep` ]): The
+            order that execution steps will be run in upon command processing.
+        default_locale (:obj:`~hikari.locales.Locale`): The default locale to use for command names and descriptions,
+            as well as option names and descriptions. Has no effect if localizations are not being used.
+        localization_provider: The localization provider function to use. This will be called whenever the client
+            needs to get the localizations for a key.
+        delete_unknown_commands (:obj:`bool`): Whether to delete existing commands that the client does not have
+            an implementation for during command syncing.
+        deferred_registration_callback: The callback to use to resolve which guilds a command should be created in
+            if a command is registered using :meth:`~Client.register_deferred`. Allows for commands to be
+            dynamically created in guilds, for example enabled on a per-guild basis using feature flags.
     """
-    A mapping of locale to name localizations for this option
 
-    .. versionadded:: 2.3.0
-    """
-    description_localizations: t.Mapping[t.Union[hikari.Locale, str], str] = attrs.field(factory=dict)
-    """
-    A mapping of locale to description localizations for this option
+    __slots__ = (
+        "rest",
+        "default_enabled_guilds",
+        "execution_step_order",
+        "default_locale",
+        "localization_provider",
+        "delete_unknown_commands",
+        "deferred_registration_callback",
+        "_di",
+        "_localization",
+        "_localized_commands",
+        "_deferred_commands",
+        "_commands",
+        "_error_handlers",
+        "_application",
+    )
 
-    .. versionadded:: 2.3.0
-    """
+    def __init__(
+        self,
+        rest: hikari.api.RESTClient,
+        default_enabled_guilds: t.Sequence[hikari.Snowflakeish],
+        execution_step_order: t.Sequence[execution.ExecutionStep],
+        default_locale: hikari.Locale,
+        localization_provider: localization.LocalizationProviderT,
+        delete_unknown_commands: bool,
+        deferred_registration_callback: t.Callable[
+            [CommandOrGroup], MaybeAwaitable[hikari.Snowflakeish | t.Sequence[hikari.Snowflakeish]]
+        ]
+        | None,
+    ) -> None:
+        super().__init__()
+
+        self.rest = rest
+        self.default_enabled_guilds = default_enabled_guilds
+        self.execution_step_order = execution_step_order
+        self.default_locale = default_locale
+        self.localization_provider = localization_provider
+        self.delete_unknown_commands = delete_unknown_commands
+        self.deferred_registration_callback = deferred_registration_callback
+
+        self._di = di_.DependencyInjectionManager()
+
+        self._localized_commands: list[tuple[t.Sequence[hikari.Snowflakeish], CommandOrGroup]] = []
+        self._deferred_commands: list[CommandOrGroup] = []
+
+        self._commands: CommandMap = collections.defaultdict(lambda: collections.defaultdict(utils.CommandCollection))
+        self._error_handlers: dict[int, list[ErrorHandler]] = {}
+        self._application: t.Optional[hikari.PartialApplication] = None
+
+        self.di.register_dependency(hikari.api.RESTClient, lambda: self.rest, enter=False)
+        self.di.register_dependency(Client, lambda: self)
 
-    def as_application_command_option(self) -> hikari.CommandOption:
+    @property
+    def di(self) -> di_.DependencyInjectionManager:
+        return self._di
+
+    async def start(self, _: t.Any = None) -> None:
         """
-        Convert this object into a :obj:`~hikari.commands.CommandOption`.
+        Starts the client. Ensures that commands are registered properly with the client, and that
+        commands have been synced with discord.
 
         Returns:
-            :obj:`~hikari.commands.CommandOption`: Created ``CommandOption`` object.
+            :obj:`None`
         """
-        if not OPTION_NAME_REGEX.fullmatch(self.name) or self.name != self.name.lower():
-            raise ValueError(
-                f"Application command option {self.name!r}: "
-                + "name must match regex '^[\\w-]{1, 32}$' and be all lowercase"
-            )
-        if len(self.description) < 1 or len(self.description) > 100:
-            raise ValueError(
-                f"Application command option {self.name!r}: description must be from 1-100 characters long"
-            )
+        if self._localized_commands and self.localization_provider is localization.localization_unsupported:
+            raise RuntimeError("some commands are marked as localized but no localization provider is available")
 
-        arg_type = OPTION_TYPE_MAPPING.get(self.arg_type, self.arg_type)
-        if not isinstance(arg_type, hikari.OptionType):
-            arg_type = hikari.OptionType.STRING
-
-        if (self.min_value is not None or self.max_value is not None) and arg_type not in (
-            hikari.OptionType.INTEGER,
-            hikari.OptionType.FLOAT,
-        ):
-            raise ValueError(
-                f"Application command option {self.name!r}: "
-                + "'min_value' or 'max_value' was provided but the option type is not numeric"
-            )
+        for guilds, command in self._localized_commands:
+            builder = await command.as_command_builder(self.default_locale, self.localization_provider)
 
-        if (self.min_length is not None or self.max_length is not None) and arg_type is not hikari.OptionType.STRING:
-            raise ValueError(
-                f"Application command option {self.name!r}: "
-                + "'min_length' or 'max_length' was provided but the option type is not string"
-            )
+            for guild in guilds:
+                self._commands[guild][builder.name].put(command)
 
-        if (
-            arg_type not in (hikari.OptionType.INTEGER, hikari.OptionType.FLOAT, hikari.OptionType.STRING)
-            and self.autocomplete
-        ):
-            raise ValueError(
-                f"Application command option {self.name!r}: "
-                + "'autocomplete' is True but the option type does not support choices"
-            )
+        if self._deferred_commands and self.deferred_registration_callback is None:
+            raise RuntimeError("some commands have deferred registration but no callback is available")
 
-        kwargs: t.MutableMapping[str, t.Any] = {
-            "type": arg_type,
-            "name": self.name,
-            "description": self.description,
-            "is_required": self.required,
-            "autocomplete": self.autocomplete,
-            "name_localizations": self.name_localizations,
-            "description_localizations": self.description_localizations,
-        }
-
-        if self.choices:
-            if len(self.choices) > 25:
-                raise ValueError("Application command options can have at most 25 choices")
-            kwargs["choices"] = _get_choice_objects_from_choices(self.choices)
-
-        if self.channel_types:
-            kwargs["channel_types"] = self.channel_types
-
-        if self.min_value is not None:
-            kwargs["min_value"] = (
-                int(self.min_value) if arg_type is hikari.OptionType.INTEGER else float(self.min_value)
-            )
+        for command in self._deferred_commands:
+            name = command.name if isinstance(command, groups.Group) else command._command_data.name
 
-        if self.max_value is not None:
-            kwargs["max_value"] = (
-                int(self.max_value) if arg_type is hikari.OptionType.INTEGER else float(self.max_value)
-            )
+            assert self.deferred_registration_callback is not None
+            guilds = await utils.maybe_await(self.deferred_registration_callback(command))
 
-        if self.min_length is not None:
-            kwargs["min_length"] = self.min_length
-        if self.max_length is not None:
-            kwargs["max_length"] = self.max_length
-
-        return hikari.CommandOption(**kwargs)
-
-
-@attrs.define(slots=True)
-class CommandLike:
-    """Generic dataclass representing a command. This can be converted into any command object."""
-
-    callback: CommandCallbackT
-    """The callback function for the command."""
-    name: str
-    """The name of the command."""
-    description: str
-    """The description of the command."""
-    options: t.MutableMapping[str, OptionLike] = attrs.field(factory=dict)
-    """The options for the command."""
-    checks: t.Sequence[t.Union[checks.Check, checks._ExclusiveCheck]] = attrs.field(factory=list)
-    """The checks for the command."""
-    error_handler: t.Optional[
-        t.Callable[[events.CommandErrorEvent], t.Coroutine[t.Any, t.Any, t.Optional[bool]]]
-    ] = None
-    """The error handler for the command."""
-    aliases: t.Sequence[str] = attrs.field(factory=list)
-    """The aliases for the command. This only affects prefix commands."""
-    guilds: hikari.UndefinedOr[t.Sequence[int]] = hikari.UNDEFINED
-    """The guilds for the command. This only affects application commands."""
-    subcommands: t.List[CommandLike] = attrs.field(factory=list)
-    """Subcommands for the command."""
-    parser: t.Optional[t.Type[parser_.BaseParser]] = None
-    """The argument parser to use for prefix commands."""
-    cooldown_manager: t.Optional[cooldowns.CooldownManager] = None
-    """The cooldown manager for the command."""
-    help_getter: t.Optional[t.Callable[[Command, context_.base.Context], str]] = None
-    """The function to call to get the command's long help text."""
-    auto_defer: bool = False
-    """Whether or not to automatically defer the response when the command is invoked."""
-    ephemeral: bool = False
-    """Whether or not to send responses from this command as ephemeral messages by default."""
-    check_exempt: t.Optional[t.Callable[[context_.base.Context], t.Union[bool, t.Coroutine[t.Any, t.Any, bool]]]] = None
-    """Check exempt predicate to use for the command."""
-    hidden: bool = False
-    """Whether or not the command should be hidden from the help command."""
-    inherit_checks: bool = False
-    """Whether or not the command should inherit checks from the parent group."""
-    pass_options: bool = False
-    """
-    Whether or not the command will have its options passed as keyword arguments when invoked.
+            if isinstance(guilds, int):
+                self._commands[guilds][name].put(command)
+                continue
 
-    .. versionadded:: 2.2.1
-    """
-    max_concurrency: t.Optional[t.Tuple[int, t.Type[buckets.Bucket]]] = None
-    """
-    The max concurrency rule for the command.
+            for guild in guilds:
+                self._commands[guild][name].put(command)
 
-    .. versionadded:: 2.2.1
-    """
-    app_command_default_member_permissions: t.Optional[hikari.Permissions] = None
-    """
-    The default member permissions for this command, if an application command.
+        await self.sync_application_commands()
 
-    .. versionadded:: 2.2.3
-    """
-    app_command_dm_enabled: bool = True
-    """
-    Whether this command will be enabled in DMs, if an application command.
+    @t.overload
+    def error_handler(self, *, priority: int = 0) -> t.Callable[[ErrorHandlerT], ErrorHandlerT]: ...
 
-    .. versionadded:: 2.2.3
-    """
-    app_command_bypass_author_permission_checks: bool = False
-    """
-    Whether invocations of this command will bypass author permission checks, if an application command.
+    @t.overload
+    def error_handler(self, func: ErrorHandlerT, *, priority: int = 0) -> ErrorHandlerT: ...
 
-    .. versionadded:: 2.2.3
-    """
-    name_localizations: t.Mapping[t.Union[hikari.Locale, str], str] = attrs.field(factory=dict)
-    """
-    A mapping of locale to name localizations for this command
+    def error_handler(
+        self, func: ErrorHandlerT | None = None, *, priority: int = 0
+    ) -> ErrorHandlerT | t.Callable[[ErrorHandlerT], ErrorHandlerT]:
+        """
+        Register an error handler function to call when an :obj:`~lightbulb.commands.execution.ExecutionPipeline` fails.
+        Also enables dependency injection for the error handler function.
 
-    .. versionadded:: 2.3.0
-    """
-    description_localizations: t.Mapping[t.Union[hikari.Locale, str], str] = attrs.field(factory=dict)
-    """
-    A mapping of locale to description localizations for this command
+        The function must take the exception as its first argument, which will be an instance of
+        :obj:`~lightbulb.exceptions.ExecutionPipelineFailedException`. The function **must** return a boolean
+        indicating whether the exception was successfully handled. Non-boolean return values will be cast to booleans.
 
-    .. versionadded:: 2.3.0
-    """
-    nsfw: bool = False
-    """
-    Whether the command should only be enabled in NSFW channels.
+        Args:
+            func: The function to register as a command error handler.
+            priority (:obj:`int`): The priority that this handler should be registered at. Higher priority handlers
+                will be executed first.
+        """
+        if func is not None:
+            wrapped = di_.with_di(func)
 
-    For prefix commands, this will add an NSFW-channel only check to the command automatically.
-    For slash commands, this will behave as specified in the Discord documentation.
+            handlers_with_same_priority = self._error_handlers.get(priority, [])
+            handlers_with_same_priority.append(wrapped)
+            self._error_handlers[priority] = handlers_with_same_priority
 
-    .. versionadded:: 2.3.1
-    """
-    _autocomplete_callbacks: t.Dict[
-        str,
-        t.Callable[
-            [hikari.CommandInteractionOption, hikari.AutocompleteInteraction],
-            t.Coroutine[
-                t.Any,
-                t.Any,
-                t.Union[
-                    _AutocompleteableOptionT,
-                    hikari.api.AutocompleteChoiceBuilder,
-                    t.Sequence[t.Union[_AutocompleteableOptionT, hikari.api.AutocompleteChoiceBuilder]],
-                ],
-            ],
-        ],
-    ] = attrs.field(factory=dict, init=False)
+            sorted_handlers = sorted(self._error_handlers.items(), key=lambda item: item[0], reverse=True)
+            self._error_handlers = {k: v for k, v in sorted_handlers}
+
+            return wrapped
 
-    async def __call__(self, context: context_.base.Context) -> None:
-        await self.callback(context)
+        def _inner(func_: ErrorHandlerT) -> ErrorHandlerT:
+            return self.error_handler(func_, priority=priority)
+
+        return _inner
 
     @t.overload
-    def set_error_handler(self) -> t.Callable[[ErrorHandlerCallbackT], ErrorHandlerCallbackT]:
-        ...
+    def register(
+        self, *, guilds: t.Sequence[hikari.Snowflakeish] | None = None
+    ) -> t.Callable[[CommandOrGroupT], CommandOrGroupT]: ...
 
     @t.overload
-    def set_error_handler(self, func: ErrorHandlerCallbackT) -> ErrorHandlerCallbackT:
-        ...
+    def register(
+        self, command: CommandOrGroupT, *, guilds: t.Sequence[hikari.Snowflakeish] | None = None
+    ) -> CommandOrGroupT: ...
 
-    def set_error_handler(
+    def register(
         self,
-        func: t.Optional[ErrorHandlerCallbackT] = None,
-    ) -> t.Union[ErrorHandlerCallbackT, t.Callable[[ErrorHandlerCallbackT], ErrorHandlerCallbackT]]:
-        """
-        Registers a coroutine function as an error handler for this command. This can be used as a first or second
-        order decorator, or called manually with the function to register.
+        command: CommandOrGroupT | None = None,
+        *,
+        guilds: t.Sequence[hikari.Snowflakeish] | None = None,
+    ) -> CommandOrGroupT | t.Callable[[CommandOrGroupT], CommandOrGroupT]:
+        """
+        Register a command or group with this client instance. Optionally, a sequence of guild ids can
+        be provided to make the commands created in specific guilds only - overriding the value for
+        default enabled guilds.
+
+        This method can be used as a function, or a first or second order decorator.
+
+        Args:
+            command (:obj:`~typing.Union` [ :obj:`~typing.Type` [ :obj:`~lightbulb.commands.commands.CommandBase ], :obj:`~lightbulb.commands.groups.Group` ]): The
+                command class or command group to register with the client.
+            guilds (:obj:`~typing.Optional` [ :obj:`~typing.Sequence` [ :obj:`~hikari.Snowflakeish` ]]): The guilds
+                to create the command or group in. If set to :obj:`None`, then this will fall back to the default
+                enabled guilds. To override default enabled guilds and make the command or group global, this should
+                be set to an empty sequence.
+
+        Returns:
+            The registered command or group, unchanged.
 
         Example:
 
             .. code-block:: python
 
-                @lightbulb.command(...)
-                @lightbulb.implements(...)
-                async def foo(ctx: lightbulb.Context) -> None:
-                    ...
-
-                # Valid
-                @foo.set_error_handler
-                async def foo_error_handler(event: lightbulb.CommandErrorEvent) -> bool:
-                    ...
+                client = lightbulb.client_from_app(...)
 
-                # Also valid
-                @foo.set_error_handler()
-                async def foo_error_handler(event: lightbulb.CommandErrorEvent) -> bool:
+                # valid
+                @client.register
+                # also valid
+                @client.register(guilds=[...])
+                class Example(
+                    lightbulb.SlashCommand,
                     ...
-
-                # Also valid
-                async def foo_error_handler(event: lightbulb.CommandErrorEvent) -> bool:
+                ):
                     ...
 
-                foo.set_error_handler(foo_error_handler)
-        """
-        if func is not None:
-            self.error_handler = func
-            return func
+                # also valid
+                client.register(Example, guilds=[...])
+        """  # noqa: E501
+        register_in: t.Sequence[hikari.Snowflakeish]
+        if not guilds and guilds is not None:
+            # commands should ignore default guilds and be global
+            register_in = (constants.GLOBAL_COMMAND_KEY,)
+        else:
+            # commands should either use the passed guilds, or if none passed, use default guilds
+            maybe_guilds = guilds or self.default_enabled_guilds
+            # pyright isn't happy about just using the above line even though it should be fine,
+            # so added the below just to remove the error
+            register_in = maybe_guilds if maybe_guilds is not hikari.UNDEFINED else ()
+
+        # Used as a function or first-order decorator
+        if command is not None:
+            name = command.name if isinstance(command, groups.Group) else command._command_data.name
+            localize = command.localize if isinstance(command, groups.Group) else command._command_data.localize
+
+            if localize:
+                # We need to handle localized commands separately because we don't know what their
+                # name is until we resolve it using the callback
+                self._localized_commands.append((register_in, command))
+            else:
+                for guild_id in register_in:
+                    self._commands[guild_id][name].put(command)
+
+            LOGGER.debug("command %r (%r) registered successfully", name, command)
+            return command
+
+        # Used as a second-order decorator
+        def _inner(command_: CommandOrGroupT) -> CommandOrGroupT:
+            return self.register(command_, guilds=register_in)
+
+        return _inner
+
+    def register_deferred(self, command: CommandOrGroupT) -> CommandOrGroupT:
+        if self.deferred_registration_callback is None:
+            raise ValueError("cannot defer registration if no deferred registration callback was provided")
 
-        def decorate(func_: ErrorHandlerCallbackT) -> ErrorHandlerCallbackT:
-            self.error_handler = func_
-            return func_
+        self._deferred_commands.append(command)
+        return command
 
-        return decorate
+    async def load_extensions(self, *import_paths: str) -> None:
+        """
+        Load extensions from the given import paths. If loading of a single extension fails it will be skipped
+        and any loaders already processed, as well as the one that caused the error will be removed.
 
-    @t.overload
-    def child(self) -> t.Callable[[CommandLike], CommandLike]:
-        ...
+        Args:
+            *import_paths (:obj:`str`): The import paths for the extensions to be loaded.
 
-    @t.overload
-    def child(self, cmd_like: CommandLike) -> CommandLike:
-        ...
+        Returns:
+            :obj:`None`
 
-    def child(
-        self, cmd_like: t.Optional[CommandLike] = None
-    ) -> t.Union[CommandLike, t.Callable[[CommandLike], CommandLike]]:
+        See Also:
+            :meth:`~Client.load_extensions_from_package`
         """
-        Registers a :obj:`~CommandLike` object as a child to this command. This can be used as a first or second
-        order decorator, or called manually with the :obj:`~CommandLike` instance to add as a child.
+        for path in import_paths:
+            try:
+                extension = importlib.import_module(path)
+            except ImportError as e:
+                LOGGER.error("could not import extension %r - skipping", path, exc_info=(type(e), e, e.__traceback__))
+                continue
 
-        Example:
+            loaded: list[loaders.Loader] = []
 
-            .. code-block:: python
+            maybe_loader: loaders.Loader | None = None
+            try:
+                for name in dir(extension):
+                    if isinstance(item := getattr(extension, name, None), loaders.Loader):
+                        maybe_loader = item
+                        await maybe_loader.add_to_client(self)
 
-                @lightbulb.command(...)
-                @lightbulb.implements(...)
-                async def foo(ctx: lightbulb.Context) -> None:
-                    ...
+                        loaded.append(maybe_loader)
+            except Exception as e:
+                LOGGER.error(
+                    "error while loading extension %r - skipping", path, exc_info=(type(e), e, e.__traceback__)
+                )
 
-                # Valid
-                @foo.child
-                @lightbulb.command(...)
-                @lightbulb.implements(...)
-                async def foo_child(event: lightbulb.Context) -> None:
-                    ...
+                if maybe_loader is not None and maybe_loader not in loaded:
+                    loaded.append(maybe_loader)
 
-                # Also valid
-                @foo.child()
-                @lightbulb.command(...)
-                @lightbulb.implements(...)
-                async def foo_child(event: lightbulb.Context) -> None:
-                    ...
+                for loader in loaded:
+                    await loader.remove_from_client(self)
 
-                # Also valid
-                @lightbulb.command(...)
-                @lightbulb.implements(...)
-                async def foo_child(event: lightbulb.Context) -> None:
-                    ...
+                continue
 
-                foo.child(foo_child)
-        """
-        if cmd_like is not None:
-            self.subcommands.append(cmd_like)
-            return cmd_like
+            LOGGER.info("extension %r loaded successfully", path)
 
-        def decorate(cmd_like_: CommandLike) -> CommandLike:
-            self.subcommands.append(cmd_like_)
-            return cmd_like_
+    async def load_extensions_from_package(self, package: types.ModuleType, *, recursive: bool = False) -> None:
+        """
+        Load all extension modules from the given package. Ignores any files with a name that starts with an underscore.
 
-        return decorate
+        Args:
+            package (:obj:`~types.ModuleType`): The package to load extensions from. Expects the imported module for
+                the ``__init__.py`` file in the package.
+            recursive (:obj:`bool`): Whether to recursively load extensions from subpackages. Defaults to :obj:`False`.
 
-    def autocomplete(self, opt1: str, *opts: str) -> t.Callable[[AutocompleteCallbackT], AutocompleteCallbackT]:
-        """
-        Second order decorator that registers a function as an autocomplete callback for this command.
+        Returns:
+            :obj:`None`
 
-        The autocomplete callback **must** be an asynchronous function that takes exactly two arguments: ``option``
-        (an instance of :obj:`hikari.interactions.command_interactions.AutocompleteInteractionOption`) which is
-        the option being autocompleted, and ``interaction`` (an instance of :obj:`hikari.interactions.command_interactions.AutocompleteInteraction`)
-        which is the interaction that triggered the autocomplete.
+        Raises:
+            :obj:`TypeError`: If the given module is not for the ``__init__.py`` file of a package.
 
-        Autocomplete can only be enabled for options with type :obj:`str`, :obj:`int`, or :obj:`float`.
+        Example:
 
-        The callback should return one of the following: a single item of the option type, a sequence of items of the
-        option type, a single :obj:`hikari.commands.CommandChoice`, or a sequence of :obj:`hikari.commands.CommandChoice`.
+            Given the following file structure:
 
-        Args:
-            opt1 (:obj:`str`): Option that this callback will do autocomplete for.
-            *opts (:obj:`str`): Additional options that this callback will do autocomplete for.
+            .. code-block:: bash
+                extensions/
+                ├── __init__.py
+                ├── extension1.py
+                └── extension2.py
+                bot.py
 
-        Example:
+            To load all extensions in the ``extensions`` package you should do the following:
 
             .. code-block:: python
 
-                @lightbulb.option("foo", "bar", autocomplete=True)
-                @lightbulb.command(...)
-                @lightbulb.implements(lightbulb.SlashCommand)
-                async def foo(ctx: lightbulb.Context) -> None
-                    ...
+                import extensions
 
-                @foo.autocomplete("foo")  # Name of the option you want to autocomplete
-                async def foo_autocomplete(
-                    opt: hikari.AutocompleteInteractionOption, inter: hikari.AutocompleteInteraction
-                ) -> Union[str, Sequence[str], hikari.api.AutocompleteChoiceBuilder, Sequence[hikari.api.AutocompleteChoiceBuilder]]:
-                    ...
-        """  # noqa: E501
+                await client.load_extensions_from_package(extensions)
 
-        def decorate(func: AutocompleteCallbackT) -> AutocompleteCallbackT:
-            for opt in [opt1, *opts]:
-                self._autocomplete_callbacks[opt] = func
-            return func
+        See Also:
+            :meth:`~Client.load_extensions`
+        """
+        if not (package.__file__ or "").endswith("__init__.py"):
+            raise TypeError("the given module does not appear to be a package")
 
-        return decorate
+        assert package.__file__ is not None
+        package_path = pathlib.Path(package.__file__).parent
+        package_import_path = package.__name__
 
+        extensions: list[str] = []
+        for item in package_path.iterdir():
+            if item.is_dir():
+                if not recursive:
+                    continue
 
-class SubCommandTrait(abc.ABC):
-    """
-    Trait that all subcommands and subgroups have.
+                # TODO - recursive extension loading
+                continue
 
-    You can check if any given command is a subcommand by checking ``issubclass``
-    on the command's class or ``isinstance`` if you have the object.
-    """
+            if item.name.startswith("_") or not item.name.endswith(".py"):
+                continue
 
-    __slots__ = ()
+            extensions.append(package_import_path + "." + item.name[:-3])
 
+        await self.load_extensions(*extensions)
 
-class Command(abc.ABC):
-    """
-    Abstract base class for all command types.
+    async def _ensure_application(self) -> hikari.PartialApplication:
+        if self._application is not None:
+            return self._application
 
-    Args:
-        app (:obj:`~.app.BotApp`): The ``BotApp`` instance that the command is registered to.
-        initialiser (:obj:`~CommandLike`): The ``CommandLike`` object to create the command from.
-    """
+        self._application = await self.rest.fetch_application()
+        return self._application
 
-    __slots__ = (
-        "_initialiser",
-        "app",
-        "parent",
-        "_plugin",
-        "_max_concurrency_semaphores",
-    )
+    async def sync_application_commands(self) -> None:
+        """
+        Sync all application commands registered to the bot with discord.
 
-    def __init__(self, app: app_.BotApp, initialiser: CommandLike) -> None:
-        self._initialiser = initialiser
-        self._plugin: t.Optional[plugins.Plugin] = None
-        self.app: app_.BotApp = app
-        """The ``BotApp`` instance the command is registered to."""
-        self.parent: t.Optional[Command] = None
-        """The parent for the command."""
-        self._max_concurrency_semaphores: t.Dict[t.Hashable, asyncio.Semaphore] = {}
+        Returns:
+            :obj:`None`
+        """
+        await sync.sync_application_commands(self)
 
-    @property
-    def _help_getter(self) -> t.Optional[t.Callable[[Command, context_.base.Context], str]]:
-        return self._initialiser.help_getter
+    @staticmethod
+    def _get_subcommand(
+        options: t.Sequence[OptionT],
+    ) -> OptionT | None:
+        subcommand = filter(
+            lambda o: o.type in (hikari.OptionType.SUB_COMMAND, hikari.OptionType.SUB_COMMAND_GROUP), options
+        )
+        return next(subcommand, None)
 
-    @property
-    def callback(self) -> CommandCallbackT:
-        """The callback function for the command."""
-        return self._initialiser.callback
+    @t.overload
+    def _resolve_options_and_command(
+        self, interaction: hikari.AutocompleteInteraction
+    ) -> tuple[t.Sequence[hikari.AutocompleteInteractionOption], type[commands.CommandBase]] | None: ...
 
-    @property
-    def name(self) -> str:
-        """The name of the command."""
-        return self._initialiser.name
+    @t.overload
+    def _resolve_options_and_command(
+        self, interaction: hikari.CommandInteraction
+    ) -> tuple[t.Sequence[hikari.CommandInteractionOption], type[commands.CommandBase]] | None: ...
+
+    def _resolve_options_and_command(
+        self, interaction: hikari.AutocompleteInteraction | hikari.CommandInteraction
+    ) -> (
+        tuple[
+            t.Sequence[hikari.AutocompleteInteractionOption] | t.Sequence[hikari.CommandInteractionOption],
+            type[commands.CommandBase],
+        ]
+        | None
+    ):
+        command_path = [interaction.command_name]
+
+        subcommand: hikari.CommandInteractionOption | hikari.AutocompleteInteractionOption | None
+        options = interaction.options or []  # TODO - check if this is hikari bug with interaction server
+        while (subcommand := self._get_subcommand(options or [])) is not None:
+            command_path.append(subcommand.name)
+            options = subcommand.options
+
+        global_commands = self._commands.get(constants.GLOBAL_COMMAND_KEY, {}).get(interaction.command_name)
+        guild_commands = self._commands.get(interaction.guild_id or constants.GLOBAL_COMMAND_KEY, {}).get(
+            interaction.command_name
+        )
+        # TODO - fix this when hikari adds the guild_id from interaction data to the model
+        root_commands = guild_commands or global_commands
+        if root_commands is None:
+            LOGGER.debug("ignoring interaction received for unknown command - %r", interaction.command_name)
+            return
 
-    @property
-    def description(self) -> str:
-        """The description of the command."""
-        return self._initialiser.description
+        root_command = {
+            int(hikari.CommandType.SLASH): root_commands.slash,
+            int(hikari.CommandType.USER): root_commands.user,
+            int(hikari.CommandType.MESSAGE): root_commands.message,
+        }[int(interaction.command_type)]
 
-    @property
-    def options(self) -> t.MutableMapping[str, OptionLike]:
-        """The options for the command."""
-        return self._initialiser.options
+        if root_command is None:
+            LOGGER.debug("ignoring interaction received for unknown command - %r", " ".join(command_path))
+            return
 
-    @property
-    def checks(self) -> t.Sequence[t.Union[checks.Check, checks._ExclusiveCheck]]:
-        """The checks for the command."""
-        return self._initialiser.checks
+        if isinstance(root_command, groups.Group):
+            command = root_command.resolve_subcommand(command_path[1:])
+            if command is None:
+                LOGGER.debug("ignoring interaction received for unknown command - %r", " ".join(command_path))
+                return
+        else:
+            command = root_command
 
-    @property
-    def aliases(self) -> t.Sequence[str]:
-        """The aliases for the command. This value means nothing for application commands."""
-        return self._initialiser.aliases
+        assert options is not None
+        return options, command
 
-    @property
-    def error_handler(
+    def build_autocomplete_context(
         self,
-    ) -> t.Optional[t.Callable[[events.CommandErrorEvent], t.Coroutine[t.Any, t.Any, t.Optional[bool]]]]:
-        """The error handler function for the command."""
-        return self._initialiser.error_handler
-
-    @property
-    def parser(self) -> t.Optional[t.Type[parser_.BaseParser]]:
-        """The argument parser to use for prefix commands."""
-        return self._initialiser.parser
+        interaction: hikari.AutocompleteInteraction,
+        options: t.Sequence[hikari.AutocompleteInteractionOption],
+        command_cls: type[commands.CommandBase],
+    ) -> context_.AutocompleteContext:
+        """
+        Build a context object from the given parameters.
 
-    @property
-    def cooldown_manager(self) -> t.Optional[cooldowns.CooldownManager]:
-        """The cooldown manager instance to use for the command."""
-        return self._initialiser.cooldown_manager
+        Args:
+            interaction (:obj:`~hikari.AutocompleteInteraction`): The interaction for the autocomplete invocation.
+            options (:obj:`~typing.Sequence` [ :obj:`hikari.CommandInteractionOption` ]): The options supplied with
+                the interaction.
+            command_cls (:obj:`~typing.Type` [ :obj:`~lightbulb.commands.commands.CommandBase` ]): The command class
+                that represents the command that has the option being autocompleted.
 
-    @property
-    def auto_defer(self) -> bool:
-        """Whether to automatically defer the response when the command is invoked."""
-        return self._initialiser.auto_defer
+        Returns:
+            :obj:`~lightbulb.context.AutocompleteContext`: The built context.
+        """
+        return context_.AutocompleteContext(self, interaction, options, command_cls)
 
-    @property
-    def default_ephemeral(self) -> bool:
-        """Whether to send responses from this command as ephemeral messages by default."""
-        return self._initialiser.ephemeral
+    async def _execute_autocomplete_context(
+        self, context: context_.AutocompleteContext, autocomplete_provider: options.AutocompleteProviderT
+    ) -> None:
+        with di_.ensure_di_context(self.di):
+            try:
+                await autocomplete_provider(context)
+            except Exception as e:
+                LOGGER.error(
+                    "Error encountered during invocation of autocomplete for command %r",
+                    context.command._command_data.qualified_name,
+                    exc_info=(type(e), e, e.__traceback__),
+                )
+
+    async def handle_autocomplete_interaction(self, interaction: hikari.AutocompleteInteraction) -> None:
+        out = self._resolve_options_and_command(interaction)
+        if out is None:
+            return
 
-    @property
-    def check_exempt(self) -> t.Callable[[context_.base.Context], t.Union[bool, t.Coroutine[t.Any, t.Any, bool]]]:
-        """Check exempt predicate to use for the command."""
-        return self._initialiser.check_exempt or (lambda _: False)
+        options, command = out
 
-    @property
-    def hidden(self) -> bool:
-        """Whether the command should be hidden from the help command."""
-        return self._initialiser.hidden
+        if not options:
+            LOGGER.debug("no options resolved from autocomplete interaction - ignoring")
+            return
 
-    @property
-    def inherit_checks(self) -> bool:
-        """Whether the command should inherit checks from the parent group."""
-        return self._initialiser.inherit_checks
+        context = self.build_autocomplete_context(interaction, options, command)
 
-    @property
-    def pass_options(self) -> bool:
-        """Whether the command will have its options passed as keyword arguments when invoked."""
-        return self._initialiser.pass_options
+        option = command._command_data.options.get(context.focused.name, None)
+        if option is None or not option.autocomplete:
+            LOGGER.debug("interaction appears to refer to option that has autocomplete disabled - ignoring")
+            return
 
-    @property
-    def max_concurrency(self) -> t.Optional[t.Tuple[int, t.Type[buckets.Bucket]]]:
-        """The max concurrency rule for the command."""
-        return self._initialiser.max_concurrency
+        LOGGER.debug("%r - invoking autocomplete", command._command_data.qualified_name)
 
-    @property
-    def app_command_default_member_permissions(self) -> t.Optional[hikari.Permissions]:
-        """The default member permissions for this command, as an application command."""
-        return self._initialiser.app_command_default_member_permissions
+        assert option.autocomplete_provider is not hikari.UNDEFINED
+        await self._execute_autocomplete_context(context, option.autocomplete_provider)
 
-    @property
-    def app_command_dm_enabled(self) -> bool:
-        """Whether this command, as an application command, is enabled in DMs."""
-        return self._initialiser.app_command_dm_enabled
+    def build_command_context(
+        self,
+        interaction: hikari.CommandInteraction,
+        options: t.Sequence[hikari.CommandInteractionOption],
+        command_cls: type[commands.CommandBase],
+    ) -> context_.Context:
+        """
+        Build a context object from the given parameters.
 
-    @property
-    def app_command_bypass_author_permission_checks(self) -> bool:
-        """Whether invocations of this command as an application command will bypass author permission checks."""
-        return self._initialiser.app_command_bypass_author_permission_checks
+        Args:
+            interaction (:obj:`~hikari.CommandInteraction`): The interaction for the command invocation.
+            options (:obj:`~typing.Sequence` [ :obj:`hikari.CommandInteractionOption` ]): The options to use to
+                invoke the command with.
+            command_cls (:obj:`~typing.Type` [ :obj:`~lightbulb.commands.commands.CommandBase` ]): The command class
+                that represents the command that should be invoked for the interaction.
 
-    @property
-    def name_localizations(self) -> t.Mapping[t.Union[hikari.Locale, str], str]:
+        Returns:
+            :obj:`~lightbulb.context.Context`: The built context.
         """
-        A mapping of locale to name localizations for this command
+        return context_.Context(
+            client=self,
+            interaction=interaction,
+            options=options,
+            command=command_cls(),
+        )
+
+    async def _execute_command_context(self, context: context_.Context) -> None:
+        with di_.ensure_di_context(self.di):
+            pipeline = execution.ExecutionPipeline(context, self.execution_step_order)
 
-        .. versionadded:: 2.3.0
-        """
-        return self._initialiser.name_localizations
+            try:
+                await pipeline._run()
+            except exceptions.ExecutionPipelineFailedException as ex:
+                all_handlers = [handler for handlers in self._error_handlers.values() for handler in handlers]
+
+                handled = False
+                while all_handlers and not handled:
+                    handled = await (all_handlers.pop(0))(ex)
+
+                if not handled:
+                    LOGGER.error(
+                        "Error encountered during invocation of command %r",
+                        context.command._command_data.qualified_name,
+                        exc_info=(type(ex), ex, ex.__traceback__),
+                    )
+
+    async def handle_application_command_interaction(self, interaction: hikari.CommandInteraction) -> None:
+        out = self._resolve_options_and_command(interaction)
+        if out is None:
+            return
 
-    @property
-    def description_localizations(self) -> t.Mapping[t.Union[hikari.Locale, str], str]:
-        """
-        A mapping of locale to description localizations for this command
+        options, command = out
+        context = self.build_command_context(interaction, options or [], command)
+        LOGGER.debug("invoking command - %r", command._command_data.qualified_name)
+        await self._execute_command_context(context)
 
-        .. versionadded:: 2.3.0
-        """
-        return self._initialiser.description_localizations
+    async def handle_interaction_create(self, interaction: hikari.PartialInteraction) -> None:
+        if isinstance(interaction, hikari.AutocompleteInteraction):
+            await self.handle_autocomplete_interaction(interaction)
+        elif isinstance(interaction, hikari.CommandInteraction):
+            await self.handle_application_command_interaction(interaction)
 
-    @property
-    def nsfw(self) -> bool:
-        """
-        Whether the command should only be enabled in NSFW channels.
 
-        For prefix commands, this will add an NSFW-channel only check to the command automatically.
-        For slash commands, this will behave as specified in the Discord documentation.
+class GatewayEnabledClient(Client):
+    """
+    Client implementation for applications that support gateway events.
 
-        .. versionadded:: 2.3.1
-        """
-        return self._initialiser.nsfw
+    Warning:
+        This client should not be instantiated manually. Use :func:`~client_from_app` instead.
 
-    def __hash__(self) -> int:
-        return hash(self.name)
+    Warning:
+        This client **will not** be started automatically (see: :meth:`~Client.start`). It is recommended
+        that you start the client in a listener for :obj:`~hikari.StartedEvent`. You should ensure that any
+        commands are registered and extensions have been loaded **before** starting the client - otherwise
+        command syncing may not work properly.
 
-    async def __call__(self, context: context_.base.Context, **kwargs: t.Any) -> None:
-        if self.pass_options:
-            for opt in context.raw_options:
-                kwargs.setdefault(opt, context.raw_options[opt])
-        return await self.callback(context, **kwargs)
+        For example:
 
-    def _validate_attributes(self) -> None:
-        pass
+        .. code-block:: python
 
-    def _set_plugin(self, pl: plugins.Plugin) -> None:
-        self._plugin = pl
+            bot = hikari.GatewayBot(...)
+            client = lightbulb.client_from_app(bot, ...)
 
-    @property
-    def plugin(self) -> t.Optional[plugins.Plugin]:
-        """The plugin that the command belongs to."""
-        return self._plugin
-
-    @plugin.setter
-    def plugin(self, pl: plugins.Plugin) -> None:
-        self._set_plugin(pl)
+            bot.subscribe(hikari.StartedEvent, client.start)
+    """
 
-    @property
-    def bot(self) -> app_.BotApp:
-        """Alias for :obj:`~Context.app`"""
-        return self.app
-
-    def get_help(self, context: context_.base.Context) -> str:
-        """
-        Get the help text for the command under the given context. This method calls the help getter
-        provided by the :obj:`~.decorators.set_help` decorator. An empty string will be returned
-        if no help getter function was set.
+    __slots__ = ("_app",)
 
-        Args:
-            context (:obj:`~.context.base.Context`): Context to get the help text under.
+    def __init__(self, app: GatewayClientAppT, *args: t.Any, **kwargs: t.Any) -> None:
+        super().__init__(app.rest, *args, **kwargs)
+        self._app = app
 
-        Returns:
-            :obj:`str`: Command's help text.
-        """
-        if self._help_getter is None:
-            return ""
-        return self._help_getter(self, context)
+        async def wrap_listener(
+            event: hikari.Event,
+            *,
+            func: t.Callable[..., t.Coroutine[t.Any, t.Any, None]],
+            arg_resolver: t.Callable[[hikari.Event], t.Sequence[t.Any]],
+        ) -> None:
+            return await func(*arg_resolver(event))
 
-    @property
-    def is_subcommand(self) -> bool:
-        """Boolean representing whether this object is a subcommand."""
-        return isinstance(self, SubCommandTrait)
+        app.event_manager.subscribe(
+            hikari.InteractionCreateEvent,
+            functools.partial(
+                wrap_listener,
+                func=self.handle_interaction_create,
+                arg_resolver=lambda e: (t.cast(hikari.InteractionCreateEvent, e).interaction,),
+            ),
+        )
 
-    @property
-    def qualname(self) -> str:
-        """The qualified name for the command."""
-        return self.name
+        if isinstance(app, hikari.GatewayBot):
+            self.di.register_dependency(hikari.GatewayBot, lambda: app)
 
-    @property
-    @abc.abstractmethod
-    def signature(self) -> str:
-        """The command's text signature."""
-        ...
+        self.di.register_dependency(hikari.api.EventManager, lambda: app.event_manager)
 
-    async def _evaluate_max_concurrency(self, context: context_.base.Context) -> None:
-        if self.max_concurrency is None:
-            return
-        bucket_hash = self.max_concurrency[1].extract_hash(context)
-        if bucket_hash not in self._max_concurrency_semaphores:
-            self._max_concurrency_semaphores[bucket_hash] = asyncio.Semaphore(self.max_concurrency[0])
-        if self._max_concurrency_semaphores[bucket_hash].locked():
-            assert context.invoked is not None
-            raise errors.MaxConcurrencyLimitReached(
-                f"Maximum concurrency limit for command '{context.invoked.qualname}' exceeded",
-                bucket=self.max_concurrency[1],
-            )
-        await self._max_concurrency_semaphores[bucket_hash].acquire()
 
-    def _release_max_concurrency(self, context: context_.base.Context) -> None:
-        if self.max_concurrency is None:
-            return
+class RestEnabledClient(Client):
+    """
+    Client implementation for applications that support an interaction server.
 
-        if sem := self._max_concurrency_semaphores.get(self.max_concurrency[1].extract_hash(context)):
-            sem.release()
+    Warning:
+        This client should not be instantiated manually. Use :func:`~client_from_app` instead.
 
-    async def invoke(self, context: context_.base.Context, **kwargs: t.Any) -> None:
-        """
-        Invokes the command under the given context. All checks, cooldowns and concurrency limits will be processed
-        prior to invocation.
-        """
-        context._invoked = self
+    Warning:
+        This client **will not** be started automatically (see: :meth:`~Client.start`). It is recommended
+        that you start the client in a :obj:`~hikari.impl.rest_bot.RESTBot` startup callback. You should ensure that any
+        commands are registered and extensions have been loaded **before** starting the client - otherwise
+        command syncing may not work properly.
 
-        await self._evaluate_max_concurrency(context)
-        try:
-            await self.evaluate_checks(context)
-            await self.evaluate_cooldowns(context)
-            await self(context, **kwargs)
-        except Exception:
-            raise
-        finally:
-            self._release_max_concurrency(context)
-
-    async def evaluate_checks(self, context: context_.base.Context) -> bool:
-        """
-        Evaluate the command's checks under the given context. This method will either return
-        ``True`` if all the checks passed, or it will raise :obj:`~.errors.CheckFailure`.
-        """
-        exempt = self.check_exempt(context)
-        if inspect.iscoroutine(exempt):
-            exempt = await exempt
-        if exempt:
-            return True
+        For example:
 
-        parent_checks = self.parent.checks if self.inherit_checks and self.parent is not None else []
+        .. code-block:: python
 
-        failed_checks: t.List[errors.CheckFailure] = []
-        for check in [*self.app._checks, *getattr(self.plugin, "_checks", []), *self.checks, *parent_checks]:
-            try:
-                result = check(context)
-                if inspect.iscoroutine(result):
-                    result = await result
-
-                if not result:
-                    failed_checks.append(errors.CheckFailure(f"Check {check.__name__} failed for command {self.name}"))
-            except Exception as ex:
-                if not isinstance(ex, errors.CheckFailure):
-                    error = errors.CheckFailure(str(ex))
-                    error.__cause__ = ex
-                else:
-                    error = ex
-                failed_checks.append(error)
-
-        if len(failed_checks) > 1:
-            raise errors.CheckFailure(
-                "Multiple checks failed: " + ", ".join(str(ex) for ex in failed_checks), causes=failed_checks
-            )
-        elif failed_checks:
-            raise failed_checks[0]
+            bot = hikari.RESTBot(...)
+            client = lightbulb.client_from_app(bot, ...)
 
-        return True
+            async def start_client() -> None:
+                # Load extensions here
+                await client.start()
+    """
 
-    async def evaluate_cooldowns(self, context: context_.base.Context) -> None:
-        """
-        Evaluate the command's cooldown under the given context. This method will either return
-        ``None`` if the command is not on cooldown or raise :obj:`.errors.CommandIsOnCooldown`.
-        """
-        if self.cooldown_manager is not None:
-            await self.cooldown_manager.add_cooldown(context)
+    __slots__ = ("_app",)
 
+    def __init__(self, app: RestClientAppT, *args: t.Any, **kwargs: t.Any) -> None:
+        super().__init__(app.rest, *args, **kwargs)
+        self._app = app
 
-class ApplicationCommand(Command, abc.ABC):
-    """Abstract base class for all application command types."""
+        app.interaction_server.set_listener(hikari.AutocompleteInteraction, self.handle_rest_autocomplete_interaction)
+        app.interaction_server.set_listener(hikari.CommandInteraction, self.handle_rest_application_command_interaction)
 
-    __slots__ = ("_guilds", "instances")
+        if isinstance(app, hikari.RESTBot):
+            self.di.register_dependency(hikari.RESTBot, lambda: app)
 
-    def __init__(self, app: app_.BotApp, initialiser: CommandLike) -> None:
-        super().__init__(app, initialiser)
-        self._guilds = initialiser.guilds
-        self.instances: t.Dict[t.Union[int, None], hikari.PartialCommand] = {}
-        """Mapping of guild ID to created hikari ``PartialCommand`` objects for this command."""
+        self.di.register_dependency(hikari.api.InteractionServer, lambda: app.interaction_server)
 
-    @property
-    def guilds(self) -> t.Sequence[int]:
-        """The guilds that this command is available in."""
-        return self.app.default_enabled_guilds if self._guilds is hikari.UNDEFINED else self._guilds
+    def build_rest_autocomplete_context(
+        self,
+        interaction: hikari.AutocompleteInteraction,
+        options: t.Sequence[hikari.AutocompleteInteractionOption],
+        command_cls: type[commands.CommandBase],
+        response_callback: t.Callable[[hikari.api.InteractionResponseBuilder], None],
+    ) -> context_.AutocompleteContext:
+        return context_.RestAutocompleteContext(self, interaction, options, command_cls, response_callback)
+
+    async def handle_rest_autocomplete_interaction(
+        self, interaction: hikari.AutocompleteInteraction
+    ) -> t.AsyncGenerator[hikari.api.InteractionAutocompleteBuilder, t.Any]:
+        out = self._resolve_options_and_command(interaction)
+        if out is None:
+            return
 
-    @property
-    def signature(self) -> str:
-        sig = self.qualname
-        if self.options:
-            sig += " " + " ".join(
-                f"<{o.name}>" if o.required else f"[{o.name}={o.default}]" for o in self.options.values()
-            )
-        return sig
+        options, command = out
 
-    async def create(self, guild: t.Optional[int] = None) -> hikari.PartialCommand:
-        """
-        Creates the command in the guild with the given ID, or globally if no
-        guild ID was provided.
+        if not options:
+            LOGGER.debug("no options resolved from autocomplete interaction - ignoring")
+            return
 
-        Args:
-            guild (Optional[:obj:`int`]): ID of the guild to create the command in, or ``None`` if to create globally.
+        initial_response_ready = asyncio.Event()
+        initial_response: t.Optional[hikari.api.InteractionResponseBuilder] = None
 
-        Returns:
-            :obj:`~hikari.commands.PartialCommand`: Created hikari ``Command`` object.
-        """
-        assert self.app.application is not None
-        kwargs = self.as_create_kwargs()
-        kwargs.update({"guild": guild} if guild is not None else {})
-        kwargs["nsfw"] = self.nsfw
-
-        if guild is None:
-            kwargs["dm_enabled"] = self.app_command_dm_enabled
-
-        if self.app_command_default_member_permissions is not None:
-            kwargs["default_member_permissions"] = self.app_command_default_member_permissions
-
-        if self.name_localizations:
-            kwargs["name_localizations"] = self.name_localizations
-
-        if self.description_localizations:
-            kwargs["description_localizations"] = self.description_localizations
-
-        cmd_type: hikari.CommandType = kwargs.pop("type")
-        created_cmd: hikari.PartialCommand
-        if cmd_type is hikari.CommandType.SLASH:
-            created_cmd = await self.app.rest.create_slash_command(
-                self.app.application,
-                **kwargs,
-            )
-        else:
-            created_cmd = await self.app.rest.create_context_menu_command(
-                self.app.application,
-                type=cmd_type,
-                **kwargs,
-            )
+        def set_response(response: hikari.api.InteractionResponseBuilder) -> None:
+            nonlocal initial_response, initial_response_ready
+            initial_response = response
+            initial_response_ready.set()
+
+        context = self.build_rest_autocomplete_context(interaction, options, command, set_response)
+
+        option = command._command_data.options.get(context.focused.name, None)
+        if option is None or not option.autocomplete:
+            LOGGER.debug("interaction appears to refer to option that has autocomplete disabled - ignoring")
+            return
 
-        self.instances[guild] = created_cmd
-        assert isinstance(created_cmd, hikari.PartialCommand)
-        return created_cmd
-
-    async def _auto_create(self) -> None:
-        if self.guilds:
-            for guild_id in self.guilds:
-                await self.create(guild_id)
-        else:
-            await self.create()
+        LOGGER.debug("%r - invoking autocomplete", command._command_data.qualified_name)
 
-    async def delete(self, guild: t.Optional[int]) -> None:
-        """
-        Deletes the command in the guild with the given ID, or globally if no
-        guild ID was provided.
+        assert option.autocomplete_provider is not hikari.UNDEFINED
+        task = asyncio.create_task(self._execute_autocomplete_context(context, option.autocomplete_provider))
+        try:
+            await asyncio.wait_for(initial_response_ready.wait(), timeout=5)
 
-        Args:
-            guild (Optional[:obj:`int`]): ID of the guild to delete the command in, or ``None`` if to delete globally.
+            if initial_response is not None:
+                yield initial_response
+        except asyncio.TimeoutError:
+            LOGGER.warning(
+                "Autocomplete for command %r took too long to create initial response",
+                command._command_data.qualified_name,
+            )
 
-        Returns:
-            ``None``
-        """
-        cmd = self.instances.pop(guild, None)
-        if cmd is None:
+        # Ensure the autocomplete provider completes
+        await task
+
+    def build_rest_command_context(
+        self,
+        interaction: hikari.CommandInteraction,
+        options: t.Sequence[hikari.CommandInteractionOption],
+        command_cls: type[commands.CommandBase],
+        response_callback: t.Callable[[hikari.api.InteractionResponseBuilder], None],
+    ) -> context_.Context:
+        return context_.RestContext(self, interaction, options, command_cls(), response_callback)
+
+    async def handle_rest_application_command_interaction(
+        self, interaction: hikari.CommandInteraction
+    ) -> t.AsyncGenerator[
+        hikari.api.InteractionDeferredBuilder
+        | hikari.api.InteractionMessageBuilder
+        | hikari.api.InteractionModalBuilder,
+        t.Any,
+    ]:
+        out = self._resolve_options_and_command(interaction)
+        if out is None:
             return
-        await cmd.delete()
 
-    async def _auto_delete(self) -> None:
-        for cmd in self.instances.values():
-            await cmd.delete()
-        self.instances.clear()
+        options, command = out
 
-    @abc.abstractmethod
-    def as_create_kwargs(self) -> t.Dict[str, t.Any]:
-        """
-        Converts this class into a dictionary of kwargs required by
-        :obj:`~hikari.api.rest.RESTClient.create_application_command`.
+        initial_response_ready = asyncio.Event()
+        initial_response: t.Optional[hikari.api.InteractionResponseBuilder] = None
 
-        Returns:
-            Dict[:obj:`str`, Any]: Kwargs required in order to create the command.
-        """
-        ...
+        def set_response(response: hikari.api.InteractionResponseBuilder) -> None:
+            nonlocal initial_response, initial_response_ready
+
+            initial_response = response
+            initial_response_ready.set()
+
+        context = self.build_rest_command_context(interaction, options or [], command, set_response)
+        LOGGER.debug("invoking command - %r", command._command_data.qualified_name)
+
+        task = asyncio.create_task(self._execute_command_context(context))
+        try:
+            await asyncio.wait_for(initial_response_ready.wait(), timeout=5)
+
+            if initial_response is not None:
+                yield initial_response
+        except asyncio.TimeoutError as e:
+            LOGGER.warning(
+                "Command %r took too long to create initial response",
+                command._command_data.qualified_name,
+                exc_info=(type(e), e, e.__traceback__),
+            )
+
+        # Ensure the command completes
+        await task
+
+
+def client_from_app(
+    app: GatewayClientAppT | RestClientAppT,
+    default_enabled_guilds: t.Sequence[hikari.Snowflakeish] = (constants.GLOBAL_COMMAND_KEY,),
+    execution_step_order: t.Sequence[execution.ExecutionStep] = DEFAULT_EXECUTION_STEP_ORDER,
+    default_locale: hikari.Locale = hikari.Locale.EN_US,
+    localization_provider: localization.LocalizationProviderT = localization.localization_unsupported,
+    delete_unknown_commands: bool = True,
+    deferred_registration_callback: t.Callable[
+        [CommandOrGroup], MaybeAwaitable[hikari.Snowflakeish | t.Sequence[hikari.Snowflakeish]]
+    ]
+    | None = None,
+) -> Client:
+    """
+    Create and return the appropriate client implementation from the given application.
+
+    Args:
+        app: Application that either supports gateway events, or an interaction server.
+        default_enabled_guilds (:obj:`~typing.Sequence` [ :obj:`~hikari.Snowflakeish` ]): The guilds that application
+            commands should be created in by default.
+        execution_step_order (:obj:`~typing.Sequence` [ :obj:`~lightbulb.commands.execution.ExecutionStep` ]): The
+            order that execution steps will be run in upon command processing.
+        default_locale: (:obj:`~hikari.locales.Locale`): The default locale to use for command names and descriptions,
+            as well as option names and descriptions. Has no effect if localizations are not being used.
+            Defaults to :obj:`hikari.locales.Locale.EN_US`.
+        localization_provider (:obj:`~typing.Callable` [ [ :obj:`str` ], :obj:`~typing.Mapping` [ :obj:`~hikari.locales.Locale`, :obj:`str` ] ]): The
+            localization provider function to use. This will be called whenever the client needs to get the
+            localizations for a key. Defaults to :obj:`~lightbulb.localization.localization_unsupported` - the client
+            does not support localizing commands. **Must** be passed if you intend
+            to support localizations.
+        delete_unknown_commands (:obj:`bool`): Whether to delete existing commands that the client does not have
+            an implementation for during command syncing. Defaults to :obj:`True`.
+        deferred_registration_callback: The callback to use to resolve which guilds a command should be created in
+            if a command is registered using :meth:`~Client.register_deferred`. Allows for commands to be
+            dynamically created in guilds, for example enabled on a per-guild basis using feature flags. Defaults
+            to :obj:`None`.
+
+    Returns:
+        :obj:`~Client`: The created client instance.
+    """  # noqa: E501
+    if isinstance(app, GatewayClientAppT):
+        LOGGER.debug("building gateway client from app")
+        cls = GatewayEnabledClient
+    else:
+        LOGGER.debug("building REST client from app")
+        cls = RestEnabledClient
+
+    return cls(
+        app,  # type: ignore[reportArgumentType]
+        default_enabled_guilds,
+        execution_step_order,
+        default_locale,
+        localization_provider,
+        delete_unknown_commands,
+        deferred_registration_callback,
+    )
```

### Comparing `hikari-lightbulb-2.3.5/lightbulb/commands/slash.py` & `hikari_lightbulb-3.0.0a0/lightbulb/commands/groups.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,248 +1,246 @@
 # -*- coding: utf-8 -*-
-# Copyright © tandemdude 2020-present
+# Copyright (c) 2023-present tandemdude
 #
-# This file is part of Lightbulb.
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
 #
-# Lightbulb is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Lesser General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
 #
-# Lightbulb is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Lesser General Public License for more details.
-#
-# You should have received a copy of the GNU Lesser General Public License
-# along with Lightbulb. If not, see <https://www.gnu.org/licenses/>.
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
 from __future__ import annotations
 
-__all__ = ["SlashCommand", "SlashCommandGroup", "SlashGroupMixin", "SlashSubGroup", "SlashSubCommand"]
+__all__ = ["SubGroup", "Group"]
 
 import abc
-import re
+import dataclasses
 import typing as t
 
 import hikari
 
-from lightbulb import context as context_
-from lightbulb import errors
-from lightbulb.commands import base
+from lightbulb.commands import utils
 
 if t.TYPE_CHECKING:
-    from lightbulb import app as app_
-    from lightbulb import plugins
-
-COMMAND_NAME_REGEX: re.Pattern[str] = re.compile(r"^[\w-]{1,32}$", re.U)
-
-
-class SlashGroupMixin(abc.ABC):
-    __slots__ = ()
-    _plugin: t.Optional[plugins.Plugin]
-    _subcommands: t.Dict[str, t.Union[SlashSubGroup, SlashSubCommand]]
-
-    @property
-    @abc.abstractmethod
-    def name(self) -> str:
-        ...
-
-    def create_subcommands(
-        self,
-        raw_cmds: t.Sequence[base.CommandLike],
-        app: app_.BotApp,
-        allowed_types: t.Union[t.Tuple[t.Type[SlashSubCommand], t.Type[SlashSubGroup]], t.Type[SlashSubCommand]],
-    ) -> None:
-        for raw_cmd in raw_cmds:
-            impls: t.List[t.Type[base.Command]] = getattr(raw_cmd.callback, "__cmd_types__", [])
-            for impl in impls:
-                if issubclass(impl, allowed_types):
-                    cmd = impl(app, raw_cmd)
-                    assert isinstance(cmd, (SlashSubCommand, SlashSubGroup))
-                    cmd.parent = self  # type: ignore
-                    cmd.plugin = self.plugin  # type: ignore
-
-                    if cmd.name in self._subcommands:
-                        raise errors.CommandAlreadyExists(
-                            f"A prefix subcommand with name or alias {cmd.name!r} "
-                            + f"already exists for group {self.name!r}"
-                        )
-                    self._subcommands[cmd.name] = cmd
-
-    def recreate_subcommands(self, raw_cmds: t.Sequence[base.CommandLike], app: app_.BotApp) -> None:
-        self._subcommands.clear()
-        self.create_subcommands(
-            raw_cmds, app, SlashSubCommand if isinstance(self, SlashSubGroup) else (SlashSubCommand, SlashSubGroup)
-        )
-
-    async def _invoke_subcommand(self, context: context_.base.Context) -> None:
-        assert isinstance(context, context_.slash.SlashContext)
-        cmd_option = context._raw_options[0]
-        context._raw_options = cmd_option.options or []
-        # Replace the invoked command prematurely so that _parse_options uses the correct command options
-        context._invoked = self._subcommands[cmd_option.name]
-        # Reparse the options for the subcommand
-        context._parse_options(cmd_option.options)
-        # Ensure we call _maybe_defer
-        await context._maybe_defer()
-        # Invoke the subcommand
-        await context._invoked.invoke(context)
-
-    def get_subcommand(self, name: str) -> t.Optional[t.Union[SlashSubGroup, SlashSubCommand]]:
-        """Get the group's subcommand with the given name."""
-        return self._subcommands.get(name)
-
-    @property
-    def subcommands(self) -> t.Dict[str, t.Union[SlashSubGroup, SlashSubCommand]]:
-        """Mapping of command name to command object containing the group's subcommands."""
-        return self._subcommands
-
-    def _set_plugin(self, pl: plugins.Plugin) -> None:
-        self._plugin = pl  # type: ignore[misc]
-        for command in self._subcommands.values():
-            if isinstance(command, SlashGroupMixin):
-                command._set_plugin(pl)
-            else:
-                command.plugin = pl
-
-
-class SlashCommand(base.ApplicationCommand):
-    """
-    An implementation of :obj:`~.commands.base.Command` representing a slash command.
-
-    See the `API Documentation <https://discord.com/developers/docs/interactions/application-commands#slash-commands>`_.
-    """
-
-    __slots__ = ()
+    from lightbulb import localization
+    from lightbulb.commands import commands
 
-    def as_create_kwargs(self) -> t.Dict[str, t.Any]:
-        sorted_opts = sorted(self.options.values(), key=lambda o: int(o.required), reverse=True)
-        return {
-            "type": hikari.CommandType.SLASH,
-            "name": self.name,
-            "description": self.description,
-            "options": [o.as_application_command_option() for o in sorted_opts],
-            "name_localizations": self.name_localizations,
-            "description_localizations": self.description_localizations,
-        }
-
-    def _validate_attributes(self) -> None:
-        if not COMMAND_NAME_REGEX.fullmatch(self.name) or self.name != self.name.lower():
-            raise ValueError(
-                f"Slash command {self.name!r}: name must match regex '^[\\w-]{1,32}$' and be all lowercase"
-            ) from None
-        if len(self.description) < 1 or len(self.description) > 100:
-            raise ValueError(f"Slash command {self.name!r}: description must be from 1-100 characters long") from None
-        if len(self.options) > 25:
-            raise ValueError(f"Slash command {self.name!r}: can at most have 25 options") from None
+CommandT = t.TypeVar("CommandT", bound=type["commands.CommandBase"])
+SubGroupCommandMappingT = dict[str, type["commands.CommandBase"]]
+GroupCommandMappingT = dict[str, t.Union["SubGroup", type["commands.CommandBase"]]]
 
 
-class SlashSubCommand(SlashCommand, base.SubCommandTrait):
-    """
-    Class representing a slash subcommand.
-    """
+class GroupMixin(abc.ABC):
+    """Base class for application command groups."""
 
     __slots__ = ()
 
-    @property
-    def qualname(self) -> str:
-        assert self.parent is not None
-        return f"{self.parent.qualname} {self.name}"
-
-    def as_option(self) -> hikari.CommandOption:
-        sorted_opts = sorted(self.options.values(), key=lambda o: int(o.required), reverse=True)
-        return hikari.CommandOption(
-            type=hikari.OptionType.SUB_COMMAND,
-            name=self.name,
-            description=self.description,
-            is_required=False,
-            options=[o.as_application_command_option() for o in sorted_opts],
-            name_localizations=self.name_localizations,
-            description_localizations=self.description_localizations,
-        )
+    _commands: SubGroupCommandMappingT | GroupCommandMappingT
 
+    @t.overload
+    def register(self) -> t.Callable[[CommandT], CommandT]: ...
 
-class SlashSubGroup(SlashCommand, SlashGroupMixin, base.SubCommandTrait):
-    """
-    Class representing a slash subgroup of commands.
-    """
+    @t.overload
+    def register(self, command: CommandT) -> CommandT: ...
 
-    __slots__ = ("_raw_subcommands", "_subcommands")
+    def register(self, command: CommandT | None = None) -> CommandT | t.Callable[[CommandT], CommandT]:
+        """
+        Register a command as a subcommand for this group. Can be used as a first or second order decorator,
+        or called with the command to register.
+
+        Args:
+            command (:obj:`~typing.Type` [ :obj:`~lightbulb.commands.commands.CommandBase` ]): The command to register
+                to the group as a subcommand.
+
+        Returns:
+            The passed command, with the parent set.
+
+        Example:
+
+            .. code-block:: python
+
+                group = lightbulb.Group("name", "description")
+
+                # valid
+                @group.register  # or @group.register()
+                class Example(
+                    lightbulb.SlashCommand,
+                    ...
+                ):
+                    ...
+
+                # also valid
+                group.register(Example)
+        """
+        if command is not None:
+            self._commands[command._command_data.name] = command
+            command._command_data.parent = self  # type: ignore[reportGeneralTypeIssues]
+            return command
+
+        def _inner(_command: CommandT) -> CommandT:
+            return self.register(_command)
+
+        return _inner
+
+    def resolve_subcommand(self, path: list[str]) -> type[commands.CommandBase] | None:
+        """
+        Resolve the subcommand for the given path - fully qualified command name.
+
+        Args:
+            path (:obj:`~typing.List` [ :obj:`str` ]): The path of the subcommand to resolve.
+
+        Returns:
+            The resolved command class, or :obj:`None` if one was not found.
+        """
+        if not path:
+            return None
+
+        maybe_command = self._commands.get(path.pop(0))
+        if maybe_command is None:
+            return None
+
+        if isinstance(maybe_command, GroupMixin):
+            return maybe_command.resolve_subcommand(path)
+
+        return maybe_command
+
+
+@dataclasses.dataclass(slots=True, frozen=True)
+class SubGroup(GroupMixin):
+    """
+    Dataclass representing a slash command subgroup.
+
+    Warning:
+        This **should not** be instantiated manually - you should instead create one using :meth:`Group.subgroup`.
+    """
+
+    name: str
+    """The name of the subgroup."""
+    description: str
+    """The description of the subgroup."""
+    localize: bool
+    """Whether the group name and description should be localized."""
+    parent: Group
+    """The parent group of the subgroup."""
+    _commands: SubGroupCommandMappingT = dataclasses.field(init=False, default_factory=dict)
+
+    async def to_command_option(
+        self, default_locale: hikari.Locale, localization_provider: localization.LocalizationProviderT
+    ) -> hikari.CommandOption:
+        """
+        Convert the subgroup into a subgroup command option.
+
+        Returns:
+            :obj:`hikari.CommandOption`: The subgroup option for this subgroup.
+        """
+        name, description = self.name, self.description
+        name_localizations: t.Mapping[hikari.Locale, str] = {}
+        description_localizations: t.Mapping[hikari.Locale, str] = {}
+
+        if self.localize:
+            (
+                name,
+                description,
+                name_localizations,
+                description_localizations,
+            ) = await utils.localize_name_and_description(name, description, default_locale, localization_provider)
 
-    def __init__(self, app: app_.BotApp, initialiser: base.CommandLike) -> None:
-        super().__init__(app, initialiser)
-        self._raw_subcommands = initialiser.subcommands
-        initialiser.subcommands = (
-            initialiser.subcommands.add_parent(self)  # type: ignore
-            if isinstance(initialiser.subcommands, base._SubcommandListProxy)  # type: ignore
-            else base._SubcommandListProxy(initialiser.subcommands, parent=self)
-        )
-        # Just to keep mypy happy we leave SlashSubGroup here
-        self._subcommands: t.Dict[str, t.Union[SlashSubGroup, SlashSubCommand]] = {}
-        self.create_subcommands(self._raw_subcommands, app, SlashSubCommand)
-
-    @property
-    def qualname(self) -> str:
-        assert self.parent is not None
-        return f"{self.parent.qualname} {self.name}"
-
-    def as_option(self) -> hikari.CommandOption:
         return hikari.CommandOption(
             type=hikari.OptionType.SUB_COMMAND_GROUP,
-            name=self.name,
-            description=self.description,
-            is_required=False,
-            options=[c.as_option() for c in self._subcommands.values()],
-            name_localizations=self.name_localizations,
-            description_localizations=self.description_localizations,
+            name=name,
+            name_localizations=name_localizations,  # type: ignore[reportArgumentType]
+            description=description,
+            description_localizations=description_localizations,  # type: ignore[reportArgumentType]
+            options=[
+                await command.to_command_option(default_locale, localization_provider)
+                for command in self._commands.values()
+            ],
         )
 
-    async def invoke(self, context: context_.base.Context, **_: t.Any) -> None:
-        await self._invoke_subcommand(context)
-
-    def _validate_attributes(self) -> None:
-        super()._validate_attributes()
-        if len(self._subcommands) > 25:
-            raise ValueError(f"Slash command {self.name!r}: group can have at most 25 subcommands") from None
-
-    def _set_plugin(self, pl: plugins.Plugin) -> None:
-        SlashGroupMixin._set_plugin(self, pl)
-
 
-class SlashCommandGroup(SlashCommand, SlashGroupMixin):
+@dataclasses.dataclass(slots=True, frozen=True)
+class Group(GroupMixin):
     """
-    Class representing a slash command group.
-    """
-
-    __slots__ = ("_raw_subcommands", "_subcommands")
+    Dataclass representing a slash command group.
 
-    def __init__(self, app: app_.BotApp, initialiser: base.CommandLike) -> None:
-        super().__init__(app, initialiser)
-        self._raw_subcommands = initialiser.subcommands
-        initialiser.subcommands = (
-            initialiser.subcommands.add_parent(self)  # type: ignore
-            if isinstance(initialiser.subcommands, base._SubcommandListProxy)  # type: ignore
-            else base._SubcommandListProxy(initialiser.subcommands, parent=self)
+    Note:
+        If ``localize`` is :obj:`True`, then ``name`` and ``description`` will instead be
+        interpreted as localization keys from which the actual name and description will be retrieved from.
+    """
+
+    name: str
+    """The name of the group."""
+    description: str
+    """The description of the group."""
+    localize: bool = False
+    """Whether the group name and description should be localized."""
+    nsfw: bool = False
+    """Whether the group should be marked as nsfw. Defaults to :obj:`False`."""
+    dm_enabled: bool = True
+    """Whether the group is enabled in direct messages."""
+    default_member_permissions: hikari.UndefinedOr[hikari.Permissions] = hikari.UNDEFINED
+    """The default permissions required to use the group in a guild."""
+
+    _commands: GroupCommandMappingT = dataclasses.field(init=False, default_factory=dict)
+
+    def subgroup(self, name: str, description: str, *, localize: bool = False) -> SubGroup:
+        """
+        Create a new subgroup as a child of this group.
+
+        Args:
+            name (:obj:`str`): The name of the subgroup.
+            description (:obj:`str`): The description of the subgroup.
+            localize (:obj:`bool`, optional): Whether to localize the group's name and description. If :obj:`true`,
+                then the ``name`` and ``description`` arguments will instead be interpreted as localization keys from
+                which the actual name and description will be retrieved from. Defaults to :obj:`False`.
+
+        Returns:
+            :obj:`~SubGroup`: The created subgroup.
+        """
+        new = SubGroup(name=name, description=description, localize=localize, parent=self)
+        self._commands[name] = new
+        return new
+
+    async def as_command_builder(
+        self, default_locale: hikari.Locale, localization_provider: localization.LocalizationProviderT
+    ) -> hikari.api.CommandBuilder:
+        """
+        Convert the group into a hikari command builder object.
+
+        Returns:
+            :obj:`hikari.api.CommandBuilder`: The builder object for this group.
+        """
+        name, description = self.name, self.description
+        name_localizations: t.Mapping[hikari.Locale, str] = {}
+        description_localizations: t.Mapping[hikari.Locale, str] = {}
+
+        if self.localize:
+            (
+                name,
+                description,
+                name_localizations,
+                description_localizations,
+            ) = await utils.localize_name_and_description(name, description, default_locale, localization_provider)
+
+        bld = (
+            hikari.impl.SlashCommandBuilder(name=name, description=description)
+            .set_name_localizations(name_localizations)  # type: ignore[reportArgumentType]
+            .set_description_localizations(description_localizations)  # type: ignore[reportArgumentType]
+            .set_is_nsfw(self.nsfw)
+            .set_is_dm_enabled(self.dm_enabled)
+            .set_default_member_permissions(self.default_member_permissions)
         )
-        self._subcommands: t.Dict[str, t.Union[SlashSubGroup, SlashSubCommand]] = {}
-        self.create_subcommands(self._raw_subcommands, app, (SlashSubCommand, SlashSubGroup))
-
-    async def invoke(self, context: context_.base.Context, **_: t.Any) -> None:
-        await self._invoke_subcommand(context)
 
-    def as_create_kwargs(self) -> t.Dict[str, t.Any]:
-        return {
-            "type": hikari.CommandType.SLASH,
-            "name": self.name,
-            "description": self.description,
-            "options": [c.as_option() for c in self._subcommands.values()],
-            "name_localizations": self.name_localizations,
-            "description_localizations": self.description_localizations,
-        }
-
-    def _validate_attributes(self) -> None:
-        super()._validate_attributes()
-        if len(self._subcommands) > 25:
-            raise ValueError(f"Slash command {self.name!r}: group can have at most 25 subcommands") from None
+        for command_or_group in self._commands.values():
+            bld.add_option(await command_or_group.to_command_option(default_locale, localization_provider))
 
-    def _set_plugin(self, pl: plugins.Plugin) -> None:
-        SlashGroupMixin._set_plugin(self, pl)
+        return bld
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `hikari-lightbulb-2.3.5/lightbulb/commands/user.py` & `hikari_lightbulb-3.0.0a0/examples/moderation_example.py`

 * *Files 27% similar despite different names*

```diff
@@ -11,49 +11,61 @@
 # Lightbulb is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with Lightbulb. If not, see <https://www.gnu.org/licenses/>.
-from __future__ import annotations
-
-__all__ = ["UserCommand"]
-
-import typing as t
+import datetime
 
 import hikari
 
-from lightbulb.commands import base
-
-
-class UserCommand(base.ApplicationCommand):
-    """
-    An implementation of :obj:`~.commands.base.Command` representing a user context menu command.
-
-    See the `API Documentation <https://discord.com/developers/docs/interactions/application-commands#user-commands>`_.
-
-    .. versionadded:: 2.2.0
-    """
-
-    __slots__ = ()
+import lightbulb
 
-    def __init__(self, *args: t.Any, **kwargs: t.Any) -> None:
-        super().__init__(*args, **kwargs)
+bot = lightbulb.BotApp(token="YOUR_TOKEN", intents=hikari.Intents.ALL_UNPRIVILEGED)
 
-    @property
-    def options(self) -> t.Dict[str, t.Any]:
-        return {}
 
-    @property
-    def description_localizations(self) -> t.Mapping[t.Union[hikari.Locale, str], str]:
-        return {}
+@bot.command()
+@lightbulb.option("reason", "Reason for the ban", required=False)
+@lightbulb.option("user", "The user to ban.", type=hikari.User)
+@lightbulb.command("ban", "Ban a user from the server.")
+@lightbulb.implements(lightbulb.SlashCommand)
+async def ban(ctx: lightbulb.SlashContext) -> None:
+    """Ban a user from the server with an optional reason."""
+    if not ctx.guild_id:
+        await ctx.respond("This command can only be used in a guild.")
+        return
+
+    # Create a deferred response as the ban may take longer than 3 seconds
+    await ctx.respond(hikari.ResponseType.DEFERRED_MESSAGE_CREATE)
+    # Perform the ban
+    await ctx.app.rest.ban_user(ctx.guild_id, ctx.options.user.id, reason=ctx.options.reason or hikari.UNDEFINED)
+    # Provide feedback to the moderator
+    await ctx.respond(f"Banned {ctx.options.user.mention}.\n**Reason:** {ctx.options.reason or 'No reason provided.'}")
+
+
+@bot.command()
+@lightbulb.option("count", "The amount of messages to purge.", type=int, max_value=100, min_value=1)
+# You may also use pass_options to pass the options directly to the function
+@lightbulb.command("purge", "Purge a certain amount of messages from a channel.", pass_options=True)
+@lightbulb.implements(lightbulb.SlashCommand)
+async def purge(ctx: lightbulb.SlashContext, count: int) -> None:
+    """Purge a certain amount of messages from a channel."""
+    if not ctx.guild_id:
+        await ctx.respond("This command can only be used in a server.")
+        return
+
+    # Fetch messages that are not older than 14 days in the channel the command is invoked in
+    # Messages older than 14 days cannot be deleted by bots, so this is a necessary precaution
+    messages = (
+        await ctx.app.rest.fetch_messages(ctx.channel_id)
+        .take_until(lambda m: datetime.datetime.now(datetime.timezone.utc) - datetime.timedelta(days=14) > m.created_at)
+        .limit(count)
+    )
+    if messages:
+        await ctx.app.rest.delete_messages(ctx.channel_id, messages)
+        await ctx.respond(f"Purged {len(messages)} messages.")
+    else:
+        await ctx.respond("Could not find any messages younger than 14 days!")
 
-    def _validate_attributes(self) -> None:
-        if len(self.name) < 1 or len(self.name) > 32:
-            raise ValueError(f"User command {self.name!r}: name must be from 1-32 characters long") from None
 
-    def as_create_kwargs(self) -> t.Dict[str, t.Any]:
-        return {
-            "type": hikari.CommandType.USER,
-            "name": self.name,
-        }
+bot.run()
```

### Comparing `hikari-lightbulb-2.3.5/lightbulb/plugins.py` & `hikari_lightbulb-3.0.0a0/lightbulb/loaders.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,350 +1,293 @@
 # -*- coding: utf-8 -*-
-# Copyright © tandemdude 2020-present
+# Copyright (c) 2023-present tandemdude
 #
-# This file is part of Lightbulb.
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
 #
-# Lightbulb is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Lesser General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
 #
-# Lightbulb is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Lesser General Public License for more details.
-#
-# You should have received a copy of the GNU Lesser General Public License
-# along with Lightbulb. If not, see <https://www.gnu.org/licenses/>.
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
 from __future__ import annotations
 
-__all__ = ["Plugin"]
+__all__ = ["Loadable", "Loader"]
 
+import abc
+import logging
 import typing as t
-from collections import defaultdict
 
 import hikari
+import svcs
 
-from lightbulb.utils import data_store
+from lightbulb import exceptions
+from lightbulb.commands import commands
+from lightbulb.commands import groups
+from lightbulb.internal import di
 
 if t.TYPE_CHECKING:
-    from lightbulb import app as app_
-    from lightbulb import checks as checks_
-    from lightbulb import commands
-    from lightbulb import events
-
-ListenerT = t.TypeVar("ListenerT", bound=t.Callable[..., t.Coroutine[t.Any, t.Any, None]])
-ErrorHandlerT = t.TypeVar(
-    "ErrorHandlerT",
-    bound=t.Callable[..., t.Coroutine[t.Any, t.Any, t.Optional[bool]]],
-)
-RemoveHookT = t.TypeVar("RemoveHookT", bound=t.Callable[..., t.Union[t.Coroutine[t.Any, t.Any, None], None]])
-
-
-class Plugin:
-    """
-    Container class for commands and listeners that can be loaded and unloaded from the bot
-    to allow for hot-swapping of commands.
-
-    Args:
-        name (:obj:`str`): The name of the plugin.
-        description (Optional[:obj:`str`]): Description of the plugin. Defaults to ``None``.
-        include_datastore (:obj:`bool`): Whether or not to create a :obj:`~.utils.data_store.DataStore` instance
-            internally for this plugin.
-        default_enabled_guilds (UndefinedOr[Union[:obj:`int`, Sequence[:obj:`int`]]]): The guilds to create application
-            commands registered to this plugin in by default. This overrides :obj:`~.app.BotApp.default_enabled_guilds`
-            but is overridden by :obj:`~.commands.base.CommandLike.guilds`.
-
-    .. versionadded:: 2.1.2
-        ``default_enabled_guilds`` arg.
-    """
-
-    __slots__ = (
-        "name",
-        "description",
-        "default_enabled_guilds",
-        "_d",
-        "_raw_commands",
-        "_all_commands",
-        "_listeners",
-        "_app",
-        "_checks",
-        "_error_handler",
-        "_remove_hook",
-    )
-
-    def __init__(
-        self,
-        name: str,
-        description: t.Optional[str] = None,
-        include_datastore: bool = False,
-        default_enabled_guilds: hikari.UndefinedOr[t.Union[int, t.Sequence[int]]] = hikari.UNDEFINED,
-    ) -> None:
-        self.name: str = name
-        """The plugin's name."""
-        self.description: str = description or ""
-        """The plugin's description."""
-        self.default_enabled_guilds: hikari.UndefinedOr[t.Sequence[int]] = (
-            (default_enabled_guilds,) if isinstance(default_enabled_guilds, int) else default_enabled_guilds
-        )
-        """The guilds that application commands registered to this plugin will be created in by default."""
-
-        self._d: t.Optional[data_store.DataStore] = None
-        if include_datastore:
-            self._d = data_store.DataStore()
-
-        self._raw_commands: t.List[commands.base.CommandLike] = []
-        self._all_commands: t.List[commands.base.Command] = []
-
-        self._listeners: t.MutableMapping[
-            t.Type[hikari.Event], t.List[t.Callable[[hikari.Event], t.Coroutine[t.Any, t.Any, None]]]
-        ] = defaultdict(list)
-
-        self._checks: t.List[t.Union[checks_.Check, checks_._ExclusiveCheck]] = []
-        self._error_handler: t.Optional[
-            t.Callable[[events.CommandErrorEvent], t.Coroutine[t.Any, t.Any, t.Optional[bool]]]
-        ] = None
-        self._remove_hook: t.Optional[t.Callable[[], t.Union[t.Coroutine[t.Any, t.Any, None], None]]] = None
-
-        self._app: t.Optional[app_.BotApp] = None
-
-    @property
-    def d(self) -> data_store.DataStore:
-        """
-        A :obj:`~.utils.data_store.DataStore` instance enabling storage of custom data without subclassing.
-        This will raise a :obj:`RuntimeError` unless you explicitly specify you want the data
-        storage instance included by passing the kwarg ``include_datastore=True`` to the constructor.
-        """
-        if self._d is None:
-            raise RuntimeError(
-                "'Plugin.d' cannot be accessed unless 'include_datastore=True' was provided during instantiation"
-            )
-
-        return self._d
-
-    @property
-    def app(self) -> app_.BotApp:
-        """The :obj:`~.app.BotApp` instance that the plugin is registered to."""
-        if self._app is None:
-            raise RuntimeError(
-                "'Plugin.app' cannot be accessed before the plugin has been added to a 'BotApp' instance"
-            )
-
-        return self._app
-
-    @app.setter
-    def app(self, val: app_.BotApp) -> None:
-        self._app = val
-        # Commands need the BotApp instance in order to be instantiated
-        # so we wait until the instance is injected in order to create the Command instanced
-        self.create_commands()
-
-    @property
-    def bot(self) -> app_.BotApp:
-        """Alias for :obj:`~Plugin.app`"""
-        return self.app
-
-    @property
-    def raw_commands(self) -> t.List[commands.base.CommandLike]:
-        """List of all the CommandLike objects registered to the plugin."""
-        return self._raw_commands
-
-    @property
-    def all_commands(self) -> t.List[commands.base.Command]:
-        """List of all created command objects registered to the plugin."""
-        return self._all_commands
-
-    @property
-    def listeners(
-        self,
-    ) -> t.Mapping[t.Type[hikari.Event], t.Collection[t.Callable[[hikari.Event], t.Coroutine[t.Any, t.Any, None]]]]:
-        """Mapping of event type to listeners registered to the plugin"""
-        return self._listeners
+    from lightbulb import client as client_
+
+CommandOrGroup: t.TypeAlias = t.Union[type[commands.CommandBase], groups.Group]
+CommandOrGroupT = t.TypeVar("CommandOrGroupT", bound=CommandOrGroup)
+ErrorHandler: t.TypeAlias = t.Callable[
+    t.Concatenate[exceptions.ExecutionPipelineFailedException, ...], t.Awaitable[bool]
+]
+ErrorHandlerT = t.TypeVar("ErrorHandlerT", bound=ErrorHandler)
+EventT = t.TypeVar("EventT", bound=type[hikari.Event])
+
+LOGGER = logging.getLogger("lightbulb.loaders")
+
+
+class Loadable(abc.ABC):
+    """Abstract class containing the logic required to add and remove a feature from a client instance."""
 
-    def create_commands(self) -> None:
+    __slots__ = ()
+
+    @abc.abstractmethod
+    async def load(self, client: client_.Client) -> None:
         """
-        Creates the command objects implemented by the :obj:`~.commands.base.CommandLike` objects registered
-        to the plugin.
+        Add the feature to the client instance.
+
+        Args:
+            client (:obj:`~lightbulb.client.Client`): The client instance to add the feature to.
 
         Returns:
-            ``None``
+            :obj:`None`
         """
-        assert self._app is not None
-        for command_like in self._raw_commands:
-            commands_to_impl: t.Sequence[t.Type[commands.base.Command]] = getattr(
-                command_like.callback, "__cmd_types__", []
-            )
-            for cmd_type in commands_to_impl:
-                cmd = cmd_type(self._app, command_like)
-
-                if cmd.is_subcommand:
-                    continue
-
-                cmd._validate_attributes()
-                cmd.plugin = self
-                self._all_commands.append(cmd)
 
-    @t.overload
-    def command(self, cmd_like: commands.base.CommandLike) -> commands.base.CommandLike:
-        ...
+    async def unload(self, client: client_.Client) -> None:
+        """
+        Remove the feature from the client instance.
 
-    @t.overload
-    def command(self) -> t.Callable[[commands.base.CommandLike], commands.base.CommandLike]:
-        ...
+        Args:
+            client (:obj:`~lightbulb.client.Client`): The client instance to remove the feature from.
 
-    def command(
-        self, cmd_like: t.Optional[commands.base.CommandLike] = None
-    ) -> t.Union[commands.base.CommandLike, t.Callable[[commands.base.CommandLike], commands.base.CommandLike]]:
+        Returns:
+            :obj:`None`
         """
-        Adds a :obj:`~.commands.base.CommandLike` object as a command to the plugin. This method can be used as a
-        first or second order decorator, or called manually with the :obj:`~.commands.CommandLike` instance to
-        add as a command.
-        """
-        if cmd_like is not None:
-            self._raw_commands.append(cmd_like)
-            if cmd_like.guilds is hikari.UNDEFINED:
-                cmd_like.guilds = self.default_enabled_guilds
-            return cmd_like
-
-        def decorate(cmd_like_: commands.base.CommandLike) -> commands.base.CommandLike:
-            self.command(cmd_like_)
-            return cmd_like_
 
-        return decorate
 
-    @t.overload
-    def listener(self, event: t.Type[hikari.Event], listener_func: ListenerT, *, bind: bool = False) -> ListenerT:
-        ...
+class _CommandLoadable(Loadable):
+    __slots__ = ("_command", "_guilds")
 
-    @t.overload
-    def listener(self, event: t.Type[hikari.Event], *, bind: bool = False) -> t.Callable[[ListenerT], ListenerT]:
-        ...
+    def __init__(self, command: CommandOrGroup, guilds: t.Sequence[hikari.Snowflakeish] | None) -> None:
+        self._command = command
+        self._guilds = guilds
 
-    def listener(
-        self,
-        event: t.Type[hikari.Event],
-        listener_func: t.Optional[ListenerT] = None,
-        *,
-        bind: bool = False,
-    ) -> t.Union[ListenerT, t.Callable[[ListenerT], ListenerT]]:
+    async def load(self, client: client_.Client) -> None:
+        client.register(self._command, guilds=self._guilds)
+
+
+class _ListenerLoadable(Loadable):
+    __slots__ = ("_callback", "_wrapped_callback", "_event_type")
+
+    def __init__(self, callback: t.Callable[[EventT], t.Awaitable[None]], event_type: EventT) -> None:
+        self._callback = callback
+        self._event_type = event_type
+
+        self._wrapped_callback: t.Callable[..., t.Awaitable[t.Any]] | None = None
+
+    async def load(self, client: client_.Client) -> None:
+        try:
+            event_manager = await client.di.get_dependency(hikari.api.EventManager)
+        except svcs.exceptions.ServiceNotFoundError as e:
+            raise RuntimeError("cannot load listeners as client does not support event dispatching") from e
+
+        async def _wrapped(*args: t.Any, **kwargs: t.Any) -> t.Any:
+            with di.ensure_di_context(client.di):
+                return await self._callback(*args, **kwargs)
+
+        self._wrapped_callback = _wrapped if di.DI_ENABLED else None
+        event_manager.subscribe(self._event_type, self._wrapped_callback or self._callback)  # type: ignore[reportArgumentType]
+
+    async def unload(self, client: client_.Client) -> None:
+        event_manager = await client.di.get_dependency(hikari.api.EventManager)
+        event_manager.unsubscribe(self._event_type, self._wrapped_callback or self._callback)  # type: ignore[reportArgumentType]
+
+
+class _ErrorHandlerLoadable(Loadable):
+    __slots__ = ("_callback", "_priority")
+
+    def __init__(self, callback: ErrorHandler, priority: int) -> None:
+        self._callback = callback
+        self._priority = priority
+
+    async def load(self, client: client_.Client) -> None:
+        client.error_handler(self._callback, priority=self._priority)
+
+
+class Loader:
+    """Class used for loading features into the client from extensions."""
+
+    __slots__ = ("_loadables",)
+
+    def __init__(self) -> None:
+        self._loadables: list[Loadable] = []
+
+    async def add_to_client(self, client: client_.Client) -> None:
         """
-        Adds a listener function to the plugin. This method can be used as a second order decorator, or called
-        manually with the event type and function to add to the plugin as a listener.
+        Add the features contained within this loader to the given client.
 
         Args:
-            event (Type[:obj:`~hikari.events.base_events.Event`): Event that the listener is for.
+            client (:obj:`~lightbulb.client.Client`): The client to add this loader's features to.
+
+        Returns:
+            :obj:`None`
+        """
+        for loadable in self._loadables:
+            await loadable.load(client)
 
-        Keyword Args:
-            bind (:obj:`bool`): Whether or not to bind the listener function to the plugin. If ``True``, the
-                function will be converted into a bound method and so will be called with the plugin as the
-                first argument, and the error event as the second argument. Defaults to ``False``.
-        """
-        if listener_func is not None:
-            if bind:
-                listener_func = listener_func.__get__(self)
-            assert listener_func is not None
-            self._listeners[event].append(listener_func)
-            return listener_func
-
-        def decorate(func: ListenerT) -> ListenerT:
-            # TODO - allow getting event type from type hint
-            if bind:
-                func = func.__get__(self)
-            self.listener(event, func)
-            return func
+    async def remove_from_client(self, client: client_.Client) -> None:
+        """
+        Remove the features contained within this loader from the given client. If any single
+        loadable's unload method raises an exception then the remaining loadables will still be unloaded.
+
+        Args:
+            client (:obj:`~lightbulb.client.Client`): The client to remove this loader's features from.
 
-        return decorate
+        Returns:
+            :obj:`None`
+        """
+        for loadable in self._loadables:
+            try:
+                await loadable.unload(client)
+            except Exception as e:
+                LOGGER.warning("error while unloading loadable %r", loadable, exc_info=(type(e), e, e.__traceback__))
 
     @t.overload
-    def set_error_handler(self, func: ErrorHandlerT, *, bind: bool = False) -> ErrorHandlerT:
-        ...
+    def command(
+        self, *, guilds: t.Sequence[hikari.Snowflakeish] | None = None
+    ) -> t.Callable[[CommandOrGroupT], CommandOrGroupT]: ...
 
     @t.overload
-    def set_error_handler(self, *, bind: bool = False) -> t.Callable[[ErrorHandlerT], ErrorHandlerT]:
-        ...
+    def command(
+        self, command: CommandOrGroupT, *, guilds: t.Sequence[hikari.Snowflakeish] | None = None
+    ) -> CommandOrGroupT: ...
 
-    def set_error_handler(
-        self,
-        func: t.Optional[ErrorHandlerT] = None,
-        *,
-        bind: bool = False,
-    ) -> t.Union[ErrorHandlerT, t.Callable[[ErrorHandlerT], ErrorHandlerT]]:
-        """
-        Sets the error handler function for the plugin. This method can be used as a second order decorator,
-        or called manually with the event type and function to set the plugin's error handler to.
-
-        Keyword Args:
-            bind (:obj:`bool`): Whether or not to bind the error handler function to the plugin. If ``True``, the
-                function will be converted into a bound method and so will be called with the plugin as the
-                first argument, and the error event as the second argument. Defaults to ``False``.
+    def command(
+        self, command: CommandOrGroupT | None = None, *, guilds: t.Sequence[hikari.Snowflakeish] | None = None
+    ) -> CommandOrGroupT | t.Callable[[CommandOrGroupT], CommandOrGroupT]:
         """
-        if func is not None:
-            if bind:
-                func = func.__get__(self)
-            assert func is not None
-            self._error_handler = func
-            return func
-
-        def decorate(func_: ErrorHandlerT) -> ErrorHandlerT:
-            if bind:
-                func_ = func_.__get__(self)
-            self._error_handler = func_
-            return func_
+        Register a command or group with this loader. Optionally, a sequence of guild ids can
+        be provided to make the commands created in specific guilds only - overriding the value for
+        default enabled guilds.
 
-        return decorate
+        This method can be used as a function, or a first or second order decorator.
 
-    @t.overload
-    def remove_hook(self, func: RemoveHookT, *, bind: bool = False) -> RemoveHookT:
-        ...
+        Args:
+            command (:obj:`~typing.Union` [ :obj:`~typing.Type` [ :obj:`~lightbulb.commands.commands.CommandBase ], :obj:`~lightbulb.commands.groups.Group` ]): The
+                command class or command group to register with the client.
+            guilds (:obj:`~typing.Optional` [ :obj:`~typing.Sequence` [ :obj:`~hikari.Snowflakeish` ]]): The guilds
+                to create the command or group in. If set to :obj:`None`, then this will fall back to the default
+                enabled guilds. To override default enabled guilds and make the command or group global, this should
+                be set to an empty sequence.
 
-    @t.overload
-    def remove_hook(self, *, bind: bool = False) -> t.Callable[[RemoveHookT], RemoveHookT]:
-        ...
+        Returns:
+            The registered command or group, unchanged.
 
-    def remove_hook(
-        self,
-        func: t.Optional[RemoveHookT] = None,
-        *,
-        bind: bool = False,
-    ) -> t.Union[RemoveHookT, t.Callable[[RemoveHookT], RemoveHookT]]:
-        """
-        Sets the remove hook function for the plugin. This method can be used as a second order decorator,
-        or called manually with the function to set the plugin's remove hook to. The registered function will
-        be called when the plugin is removed from the bot so may be useful for teardown.
-
-        This function will be called **after** all the members of the plugin (listeners and commands) have already
-        been removed from the bot.
-
-        Keyword Args:
-            bind (:obj:`bool`): Whether or not to bind the remove hook function to the plugin. If ``True``, the
-                function will be converted into a bound method and so will be called with the plugin as an
-                argument. Defaults to ``False``.
-        """
-        if func is not None:
-            if bind:
-                func = func.__get__(self)
-            assert func is not None
-            self._remove_hook = func
-            return func
-
-        def decorate(func_: RemoveHookT) -> RemoveHookT:
-            if bind:
-                func_ = func_.__get__(self)
-            self._remove_hook = func_
-            return func_
+        Example:
 
-        return decorate
+            .. code-block:: python
 
-    def add_checks(self, *checks: t.Union[checks_.Check, checks_._ExclusiveCheck]) -> None:
+                loader = lightbulb.Loader()
+
+                # valid
+                @loader.register
+                # also valid
+                @loader.register(guilds=[...])
+                class Example(
+                    lightbulb.SlashCommand,
+                    ...
+                ):
+                    ...
+
+                # also valid
+                loader.register(Example, guilds=[...])
+        """  # noqa: E501
+        # Used as a function or first-order decorator
+        if command is not None:
+            self._loadables.append(_CommandLoadable(command, guilds))
+            return command
+
+        # Used as a second-order decorator
+        def _inner(command_: CommandOrGroupT) -> CommandOrGroupT:
+            return self.command(command_, guilds=guilds)
+
+        return _inner
+
+    def listener(
+        self, event_type: EventT
+    ) -> t.Callable[
+        [t.Callable[t.Concatenate[EventT, ...], t.Awaitable[None]]], t.Callable[[EventT], t.Awaitable[None]]
+    ]:
         """
-        Adds one or more checks to the plugin object. These checks will be run for
-        all commands in the plugin.
+        Decorator to register a listener with this loader. Also enables dependency injection on the listener
+        callback.
+
+        If an :obj:`hikari.api.event_manager.EventManager` instance is not available through dependency
+        injection then adding this loader to the client will fail at runtime.
 
         Args:
-            *checks (:obj:`~.checks.Check`): Check object(s) to add to the command.
+            event_type (:obj:`~typing.Type` [ :obj:`hikari.Event` ]): The event class for the listener to listen to.
 
-        Returns:
-            ``None``
+        Example:
+
+            .. code-block:: python
+
+                loader = lightbulb.Loader()
+
+                @loader.listener(hikari.MessageCreateEvent)
+                async def message_create_listener(event: hikari.MessageCreateEvent) -> None:
+                    ...
+        """
+
+        def _inner(
+            callback: t.Callable[t.Concatenate[EventT, ...], t.Awaitable[None]],
+        ) -> t.Callable[[EventT], t.Awaitable[None]]:
+            wrapped = t.cast(t.Callable[[EventT], t.Awaitable[None]], di.with_di(callback))
+            self._loadables.append(_ListenerLoadable(wrapped, event_type))
+            return wrapped
+
+        return _inner
+
+    @t.overload
+    def error_handler(self, *, priority: int = 0) -> t.Callable[[ErrorHandlerT], ErrorHandlerT]: ...
+
+    @t.overload
+    def error_handler(self, func: ErrorHandlerT, *, priority: int = 0) -> ErrorHandlerT: ...
+
+    def error_handler(
+        self, func: ErrorHandlerT | None = None, *, priority: int = 0
+    ) -> ErrorHandlerT | t.Callable[[ErrorHandlerT], ErrorHandlerT]:
+        """
+        Register an error handler function to call when an :obj:`~lightbulb.commands.execution.ExecutionPipeline` fails.
+        Also enables dependency injection for the error handler function.
+
+        The function must take the exception as its first argument, which will be an instance of
+        :obj:`~lightbulb.exceptions.ExecutionPipelineFailedException`. The function **must** return a boolean
+        indicating whether the exception was successfully handled. Non-boolean return values will be cast to booleans.
+
+        Args:
+            func: The function to register as a command error handler.
+            priority (:obj:`int`): The priority that this handler should be registered at. Higher priority handlers
+                will be executed first.
         """
-        self._checks.extend(checks)
-        for check in checks:
-            check.add_to_object_hook(self)
+        if func is not None:
+            wrapped = di.with_di(func)
+            self._loadables.append(_ErrorHandlerLoadable(wrapped, priority))
+            return wrapped
+
+        def _inner(func_: ErrorHandlerT) -> ErrorHandlerT:
+            return self.error_handler(func_, priority=priority)
+
+        return _inner
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

