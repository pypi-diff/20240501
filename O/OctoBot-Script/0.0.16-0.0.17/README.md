# Comparing `tmp/OctoBot-Script-0.0.16.tar.gz` & `tmp/OctoBot-Script-0.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OctoBot-Script-0.0.16.tar", last modified: Sun Jan 14 10:07:46 2024, max compression
+gzip compressed data, was "OctoBot-Script-0.0.17.tar", last modified: Wed May  1 20:12:22 2024, max compression
```

## Comparing `OctoBot-Script-0.0.16.tar` & `OctoBot-Script-0.0.17.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 10:07:46.376195 OctoBot-Script-0.0.16/
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-01-14 10:06:24.000000 OctoBot-Script-0.0.16/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-01-14 10:06:24.000000 OctoBot-Script-0.0.16/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-01-14 10:06:24.000000 OctoBot-Script-0.0.16/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 10:07:46.376195 OctoBot-Script-0.0.16/OctoBot_Script.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5137 2024-01-14 10:07:46.000000 OctoBot-Script-0.0.16/OctoBot_Script.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-01-14 10:07:46.000000 OctoBot-Script-0.0.16/OctoBot_Script.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-14 10:07:46.000000 OctoBot-Script-0.0.16/OctoBot_Script.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-01-14 10:07:46.000000 OctoBot-Script-0.0.16/OctoBot_Script.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-14 10:07:46.000000 OctoBot-Script-0.0.16/OctoBot_Script.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-01-14 10:07:46.000000 OctoBot-Script-0.0.16/OctoBot_Script.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-01-14 10:07:46.000000 OctoBot-Script-0.0.16/OctoBot_Script.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5137 2024-01-14 10:07:46.376195 OctoBot-Script-0.0.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4345 2024-01-14 10:06:24.000000 OctoBot-Script-0.0.16/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 10:07:46.368195 OctoBot-Script-0.0.16/octobot_script/
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-01-14 10:06:24.000000 OctoBot-Script-0.0.16/octobot_script/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 10:07:46.372195 OctoBot-Script-0.0.16/octobot_script/ai/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-01-14 10:06:24.000000 OctoBot-Script-0.0.16/octobot_script/ai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-01-14 10:06:24.000000 OctoBot-Script-0.0.16/octobot_script/ai/agents.py
--rw-r--r--   0 runner    (1001) docker     (127)     6341 2024-01-14 10:06:24.000000 OctoBot-Script-0.0.16/octobot_script/ai/environments.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-01-14 10:06:24.000000 OctoBot-Script-0.0.16/octobot_script/ai/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 10:07:46.372195 OctoBot-Script-0.0.16/octobot_script/api/
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-01-14 10:06:24.000000 OctoBot-Script-0.0.16/octobot_script/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-01-14 10:06:24.000000 OctoBot-Script-0.0.16/octobot_script/api/data_fetching.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-01-14 10:06:24.000000 OctoBot-Script-0.0.16/octobot_script/api/execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-01-14 10:06:24.000000 OctoBot-Script-0.0.16/octobot_script/api/ploting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-01-14 10:06:24.000000 OctoBot-Script-0.0.16/octobot_script/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 10:07:46.372195 OctoBot-Script-0.0.16/octobot_script/config/
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-01-14 10:06:24.000000 OctoBot-Script-0.0.16/octobot_script/config/config_mock.json
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-01-14 10:06:24.000000 OctoBot-Script-0.0.16/octobot_script/config/logging_config.ini
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-01-14 10:06:24.000000 OctoBot-Script-0.0.16/octobot_script/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 10:07:46.372195 OctoBot-Script-0.0.16/octobot_script/internal/
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-01-14 10:06:24.000000 OctoBot-Script-0.0.16/octobot_script/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-01-14 10:06:24.000000 OctoBot-Script-0.0.16/octobot_script/internal/backtester_trading_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-01-14 10:06:24.000000 OctoBot-Script-0.0.16/octobot_script/internal/logging_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-01-14 10:06:24.000000 OctoBot-Script-0.0.16/octobot_script/internal/octobot_mocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-01-14 10:06:24.000000 OctoBot-Script-0.0.16/octobot_script/internal/runners.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 10:07:46.372195 OctoBot-Script-0.0.16/octobot_script/model/
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-01-14 10:06:24.000000 OctoBot-Script-0.0.16/octobot_script/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-01-14 10:06:24.000000 OctoBot-Script-0.0.16/octobot_script/model/backtest_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-01-14 10:06:24.000000 OctoBot-Script-0.0.16/octobot_script/model/backtest_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-01-14 10:06:24.000000 OctoBot-Script-0.0.16/octobot_script/model/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-01-14 10:06:24.000000 OctoBot-Script-0.0.16/octobot_script/model/strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 10:07:46.372195 OctoBot-Script-0.0.16/octobot_script/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-01-14 10:06:24.000000 OctoBot-Script-0.0.16/octobot_script/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 10:07:46.372195 OctoBot-Script-0.0.16/octobot_script/resources/reports/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 10:07:46.376195 OctoBot-Script-0.0.16/octobot_script/resources/reports/css/
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-01-14 10:06:24.000000 OctoBot-Script-0.0.16/octobot_script/resources/reports/css/style.css
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-01-14 10:06:24.000000 OctoBot-Script-0.0.16/octobot_script/resources/reports/css/w2ui_template.css
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-01-14 10:06:24.000000 OctoBot-Script-0.0.16/octobot_script/resources/reports/default_report_template.html
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-01-14 10:06:24.000000 OctoBot-Script-0.0.16/octobot_script/resources/reports/header.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 10:07:46.376195 OctoBot-Script-0.0.16/octobot_script/resources/reports/js/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-01-14 10:06:24.000000 OctoBot-Script-0.0.16/octobot_script/resources/reports/js/common.js
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-14 10:06:24.000000 OctoBot-Script-0.0.16/octobot_script/resources/reports/js/data.js
--rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-01-14 10:06:24.000000 OctoBot-Script-0.0.16/octobot_script/resources/reports/js/graphs.js
--rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-01-14 10:06:24.000000 OctoBot-Script-0.0.16/octobot_script/resources/reports/js/tables.js
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-01-14 10:06:24.000000 OctoBot-Script-0.0.16/octobot_script/resources/reports/js/texts.js
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-01-14 10:06:24.000000 OctoBot-Script-0.0.16/octobot_script/resources/reports/scripts.html
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-01-14 10:06:24.000000 OctoBot-Script-0.0.16/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-14 10:07:46.376195 OctoBot-Script-0.0.16/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-01-14 10:06:24.000000 OctoBot-Script-0.0.16/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 10:07:46.364195 OctoBot-Script-0.0.16/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 10:07:46.376195 OctoBot-Script-0.0.16/tests/api/
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-01-14 10:06:24.000000 OctoBot-Script-0.0.16/tests/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-01-14 10:06:24.000000 OctoBot-Script-0.0.16/tests/api/test_data_fetching.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-01-14 10:06:24.000000 OctoBot-Script-0.0.16/tests/api/test_execution.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 10:07:46.376195 OctoBot-Script-0.0.16/tests/functionnal/
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-01-14 10:06:24.000000 OctoBot-Script-0.0.16/tests/functionnal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 10:07:46.376195 OctoBot-Script-0.0.16/tests/functionnal/example_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-01-14 10:06:24.000000 OctoBot-Script-0.0.16/tests/functionnal/example_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-01-14 10:06:24.000000 OctoBot-Script-0.0.16/tests/functionnal/example_scripts/test_precomputed_vs_iteration_rsi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:12:22.289240 OctoBot-Script-0.0.17/
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-01 20:11:06.000000 OctoBot-Script-0.0.17/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-05-01 20:11:06.000000 OctoBot-Script-0.0.17/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-01 20:11:06.000000 OctoBot-Script-0.0.17/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:12:22.285239 OctoBot-Script-0.0.17/OctoBot_Script.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5138 2024-05-01 20:12:22.000000 OctoBot-Script-0.0.17/OctoBot_Script.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-01 20:12:22.000000 OctoBot-Script-0.0.17/OctoBot_Script.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 20:12:22.000000 OctoBot-Script-0.0.17/OctoBot_Script.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-01 20:12:22.000000 OctoBot-Script-0.0.17/OctoBot_Script.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 20:12:22.000000 OctoBot-Script-0.0.17/OctoBot_Script.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-01 20:12:22.000000 OctoBot-Script-0.0.17/OctoBot_Script.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-01 20:12:22.000000 OctoBot-Script-0.0.17/OctoBot_Script.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5138 2024-05-01 20:12:22.289240 OctoBot-Script-0.0.17/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4345 2024-05-01 20:11:06.000000 OctoBot-Script-0.0.17/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:12:22.281239 OctoBot-Script-0.0.17/octobot_script/
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-01 20:11:06.000000 OctoBot-Script-0.0.17/octobot_script/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:12:22.281239 OctoBot-Script-0.0.17/octobot_script/ai/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-01 20:11:06.000000 OctoBot-Script-0.0.17/octobot_script/ai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-01 20:11:06.000000 OctoBot-Script-0.0.17/octobot_script/ai/agents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6341 2024-05-01 20:11:06.000000 OctoBot-Script-0.0.17/octobot_script/ai/environments.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-01 20:11:06.000000 OctoBot-Script-0.0.17/octobot_script/ai/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:12:22.281239 OctoBot-Script-0.0.17/octobot_script/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-01 20:11:06.000000 OctoBot-Script-0.0.17/octobot_script/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-05-01 20:11:06.000000 OctoBot-Script-0.0.17/octobot_script/api/data_fetching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-01 20:11:06.000000 OctoBot-Script-0.0.17/octobot_script/api/execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-01 20:11:06.000000 OctoBot-Script-0.0.17/octobot_script/api/ploting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-01 20:11:06.000000 OctoBot-Script-0.0.17/octobot_script/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:12:22.281239 OctoBot-Script-0.0.17/octobot_script/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-01 20:11:06.000000 OctoBot-Script-0.0.17/octobot_script/config/config_mock.json
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-01 20:11:06.000000 OctoBot-Script-0.0.17/octobot_script/config/logging_config.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-01 20:11:06.000000 OctoBot-Script-0.0.17/octobot_script/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:12:22.281239 OctoBot-Script-0.0.17/octobot_script/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-01 20:11:06.000000 OctoBot-Script-0.0.17/octobot_script/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-01 20:11:06.000000 OctoBot-Script-0.0.17/octobot_script/internal/backtester_trading_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-01 20:11:06.000000 OctoBot-Script-0.0.17/octobot_script/internal/logging_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-05-01 20:11:06.000000 OctoBot-Script-0.0.17/octobot_script/internal/octobot_mocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-05-01 20:11:06.000000 OctoBot-Script-0.0.17/octobot_script/internal/runners.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:12:22.285239 OctoBot-Script-0.0.17/octobot_script/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-01 20:11:06.000000 OctoBot-Script-0.0.17/octobot_script/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-05-01 20:11:06.000000 OctoBot-Script-0.0.17/octobot_script/model/backtest_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-05-01 20:11:06.000000 OctoBot-Script-0.0.17/octobot_script/model/backtest_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-01 20:11:06.000000 OctoBot-Script-0.0.17/octobot_script/model/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-01 20:11:06.000000 OctoBot-Script-0.0.17/octobot_script/model/strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:12:22.285239 OctoBot-Script-0.0.17/octobot_script/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-01 20:11:06.000000 OctoBot-Script-0.0.17/octobot_script/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:12:22.285239 OctoBot-Script-0.0.17/octobot_script/resources/reports/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:12:22.285239 OctoBot-Script-0.0.17/octobot_script/resources/reports/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-01 20:11:06.000000 OctoBot-Script-0.0.17/octobot_script/resources/reports/css/style.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-01 20:11:06.000000 OctoBot-Script-0.0.17/octobot_script/resources/reports/css/w2ui_template.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-01 20:11:06.000000 OctoBot-Script-0.0.17/octobot_script/resources/reports/default_report_template.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-01 20:11:06.000000 OctoBot-Script-0.0.17/octobot_script/resources/reports/header.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:12:22.285239 OctoBot-Script-0.0.17/octobot_script/resources/reports/js/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-01 20:11:06.000000 OctoBot-Script-0.0.17/octobot_script/resources/reports/js/common.js
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-01 20:11:06.000000 OctoBot-Script-0.0.17/octobot_script/resources/reports/js/data.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-05-01 20:11:06.000000 OctoBot-Script-0.0.17/octobot_script/resources/reports/js/graphs.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-05-01 20:11:06.000000 OctoBot-Script-0.0.17/octobot_script/resources/reports/js/tables.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-01 20:11:06.000000 OctoBot-Script-0.0.17/octobot_script/resources/reports/js/texts.js
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-01 20:11:06.000000 OctoBot-Script-0.0.17/octobot_script/resources/reports/scripts.html
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-01 20:11:06.000000 OctoBot-Script-0.0.17/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 20:12:22.289240 OctoBot-Script-0.0.17/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-05-01 20:11:06.000000 OctoBot-Script-0.0.17/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:12:22.277239 OctoBot-Script-0.0.17/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:12:22.285239 OctoBot-Script-0.0.17/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-01 20:11:06.000000 OctoBot-Script-0.0.17/tests/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-05-01 20:11:06.000000 OctoBot-Script-0.0.17/tests/api/test_data_fetching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-01 20:11:06.000000 OctoBot-Script-0.0.17/tests/api/test_execution.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:12:22.285239 OctoBot-Script-0.0.17/tests/functionnal/
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-01 20:11:06.000000 OctoBot-Script-0.0.17/tests/functionnal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:12:22.285239 OctoBot-Script-0.0.17/tests/functionnal/example_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-01 20:11:06.000000 OctoBot-Script-0.0.17/tests/functionnal/example_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-05-01 20:11:06.000000 OctoBot-Script-0.0.17/tests/functionnal/example_scripts/test_precomputed_vs_iteration_rsi.py
```

### Comparing `OctoBot-Script-0.0.16/CHANGELOG.md` & `OctoBot-Script-0.0.17/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.0.17] - 2024-05-01
+### Updated
+- OctoBot to 1.0.10
+
 ## [0.0.16] - 2023-01-14
 ### Updated
 - OctoBot to 1.0.6
 
 ## [0.0.15] - 2023-12-15
 ### Updated
 - OctoBot to 1.0.4
```

### Comparing `OctoBot-Script-0.0.16/LICENSE` & `OctoBot-Script-0.0.17/LICENSE`

 * *Files identical despite different names*

### Comparing `OctoBot-Script-0.0.16/OctoBot_Script.egg-info/PKG-INFO` & `OctoBot-Script-0.0.17/OctoBot_Script.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: OctoBot-Script
-Version: 0.0.16
+Version: 0.0.17
 Summary: Backtesting framework of the OctoBot Ecosystem
 Home-page: https://github.com/Drakkar-Software/OctoBot-Script
 Author: Drakkar-Software
 Author-email: contact@drakkar.software
 License: GPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: OctoBot==1.0.6
+Requires-Dist: OctoBot==1.0.10
 Requires-Dist: appdirs==1.4.4
 Requires-Dist: click==8.1.3
 Requires-Dist: jinja2
 Requires-Dist: aiohttp
 Requires-Dist: wheel
 
-# OctoBot-Script [0.0.16](https://github.com/Drakkar-Software/OctoBot-Script/tree/master/CHANGELOG.md)
+# OctoBot-Script [0.0.17](https://github.com/Drakkar-Software/OctoBot-Script/tree/master/CHANGELOG.md)
 [![PyPI](https://img.shields.io/pypi/v/OctoBot-Script.svg?logo=pypi)](https://pypi.python.org/pypi/octobot-script/)
 [![Downloads](https://static.pepy.tech/badge/OctoBot-Script/month)](https://pepy.tech/project/octobot-script)
 [![Dockerhub](https://img.shields.io/docker/pulls/drakkarsoftware/OctoBot-Script.svg?logo=docker)](https://hub.docker.com/r/drakkarsoftware/octobot-script)
 [![Github-Action-CI](https://github.com/Drakkar-Software/OctoBot-Script/actions/workflows/main.yml/badge.svg)](https://github.com/Drakkar-Software/OctoBot-Script/actions/workflows/main.yml)
 
 ## OctoBot-Script Community
 [![Telegram Chat](https://img.shields.io/badge/telegram-chat-green.svg?logo=telegram&label=Telegram)](https://octobot.click/readme-telegram-OctoBot-Script)
```

### Comparing `OctoBot-Script-0.0.16/OctoBot_Script.egg-info/SOURCES.txt` & `OctoBot-Script-0.0.17/OctoBot_Script.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OctoBot-Script-0.0.16/PKG-INFO` & `OctoBot-Script-0.0.17/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: OctoBot-Script
-Version: 0.0.16
+Version: 0.0.17
 Summary: Backtesting framework of the OctoBot Ecosystem
 Home-page: https://github.com/Drakkar-Software/OctoBot-Script
 Author: Drakkar-Software
 Author-email: contact@drakkar.software
 License: GPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: OctoBot==1.0.6
+Requires-Dist: OctoBot==1.0.10
 Requires-Dist: appdirs==1.4.4
 Requires-Dist: click==8.1.3
 Requires-Dist: jinja2
 Requires-Dist: aiohttp
 Requires-Dist: wheel
 
-# OctoBot-Script [0.0.16](https://github.com/Drakkar-Software/OctoBot-Script/tree/master/CHANGELOG.md)
+# OctoBot-Script [0.0.17](https://github.com/Drakkar-Software/OctoBot-Script/tree/master/CHANGELOG.md)
 [![PyPI](https://img.shields.io/pypi/v/OctoBot-Script.svg?logo=pypi)](https://pypi.python.org/pypi/octobot-script/)
 [![Downloads](https://static.pepy.tech/badge/OctoBot-Script/month)](https://pepy.tech/project/octobot-script)
 [![Dockerhub](https://img.shields.io/docker/pulls/drakkarsoftware/OctoBot-Script.svg?logo=docker)](https://hub.docker.com/r/drakkarsoftware/octobot-script)
 [![Github-Action-CI](https://github.com/Drakkar-Software/OctoBot-Script/actions/workflows/main.yml/badge.svg)](https://github.com/Drakkar-Software/OctoBot-Script/actions/workflows/main.yml)
 
 ## OctoBot-Script Community
 [![Telegram Chat](https://img.shields.io/badge/telegram-chat-green.svg?logo=telegram&label=Telegram)](https://octobot.click/readme-telegram-OctoBot-Script)
```

### Comparing `OctoBot-Script-0.0.16/README.md` & `OctoBot-Script-0.0.17/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# OctoBot-Script [0.0.16](https://github.com/Drakkar-Software/OctoBot-Script/tree/master/CHANGELOG.md)
+# OctoBot-Script [0.0.17](https://github.com/Drakkar-Software/OctoBot-Script/tree/master/CHANGELOG.md)
 [![PyPI](https://img.shields.io/pypi/v/OctoBot-Script.svg?logo=pypi)](https://pypi.python.org/pypi/octobot-script/)
 [![Downloads](https://static.pepy.tech/badge/OctoBot-Script/month)](https://pepy.tech/project/octobot-script)
 [![Dockerhub](https://img.shields.io/docker/pulls/drakkarsoftware/OctoBot-Script.svg?logo=docker)](https://hub.docker.com/r/drakkarsoftware/octobot-script)
 [![Github-Action-CI](https://github.com/Drakkar-Software/OctoBot-Script/actions/workflows/main.yml/badge.svg)](https://github.com/Drakkar-Software/OctoBot-Script/actions/workflows/main.yml)
 
 ## OctoBot-Script Community
 [![Telegram Chat](https://img.shields.io/badge/telegram-chat-green.svg?logo=telegram&label=Telegram)](https://octobot.click/readme-telegram-OctoBot-Script)
```

### Comparing `OctoBot-Script-0.0.16/octobot_script/__init__.py` & `OctoBot-Script-0.0.17/octobot_script/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #  General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public
 #  License along with OctoBot-Script. If not, see <https://www.gnu.org/licenses/>.
 
 PROJECT_NAME = "OctoBot-Script"
 AUTHOR = "Drakkar-Software"
-VERSION = "0.0.16"  # major.minor.revision => don't forget to also update the setup.py version
+VERSION = "0.0.17"  # major.minor.revision => don't forget to also update the setup.py version
 
 
 def _use_module_local_tentacles():
     import sys
     import os
     import appdirs
     if os.getenv("USE_CUSTOM_TENTACLES", "").lower() == "true":
```

### Comparing `OctoBot-Script-0.0.16/octobot_script/ai/agents.py` & `OctoBot-Script-0.0.17/octobot_script/ai/agents.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Script-0.0.16/octobot_script/ai/environments.py` & `OctoBot-Script-0.0.17/octobot_script/ai/environments.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Script-0.0.16/octobot_script/ai/models.py` & `OctoBot-Script-0.0.17/octobot_script/ai/models.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Script-0.0.16/octobot_script/api/__init__.py` & `OctoBot-Script-0.0.17/octobot_script/api/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Script-0.0.16/octobot_script/api/data_fetching.py` & `OctoBot-Script-0.0.17/octobot_script/api/data_fetching.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Script-0.0.16/octobot_script/api/execution.py` & `OctoBot-Script-0.0.17/octobot_script/api/execution.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Script-0.0.16/octobot_script/api/ploting.py` & `OctoBot-Script-0.0.17/octobot_script/api/ploting.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Script-0.0.16/octobot_script/cli.py` & `OctoBot-Script-0.0.17/octobot_script/cli.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Script-0.0.16/octobot_script/config/config_mock.json` & `OctoBot-Script-0.0.17/octobot_script/config/config_mock.json`

 * *Files identical despite different names*

### Comparing `OctoBot-Script-0.0.16/octobot_script/config/logging_config.ini` & `OctoBot-Script-0.0.17/octobot_script/config/logging_config.ini`

 * *Files identical despite different names*

### Comparing `OctoBot-Script-0.0.16/octobot_script/constants.py` & `OctoBot-Script-0.0.17/octobot_script/constants.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Script-0.0.16/octobot_script/internal/__init__.py` & `OctoBot-Script-0.0.17/octobot_script/internal/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Script-0.0.16/octobot_script/internal/backtester_trading_mode.py` & `OctoBot-Script-0.0.17/octobot_script/internal/backtester_trading_mode.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Script-0.0.16/octobot_script/internal/logging_util.py` & `OctoBot-Script-0.0.17/octobot_script/internal/logging_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Script-0.0.16/octobot_script/internal/octobot_mocks.py` & `OctoBot-Script-0.0.17/octobot_script/internal/octobot_mocks.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Script-0.0.16/octobot_script/internal/runners.py` & `OctoBot-Script-0.0.17/octobot_script/internal/runners.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Script-0.0.16/octobot_script/model/__init__.py` & `OctoBot-Script-0.0.17/octobot_script/model/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Script-0.0.16/octobot_script/model/backtest_plot.py` & `OctoBot-Script-0.0.17/octobot_script/model/backtest_plot.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Script-0.0.16/octobot_script/model/backtest_result.py` & `OctoBot-Script-0.0.17/octobot_script/model/backtest_result.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Script-0.0.16/octobot_script/model/errors.py` & `OctoBot-Script-0.0.17/octobot_script/model/errors.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Script-0.0.16/octobot_script/model/strategy.py` & `OctoBot-Script-0.0.17/octobot_script/model/strategy.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Script-0.0.16/octobot_script/resources/__init__.py` & `OctoBot-Script-0.0.17/octobot_script/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Script-0.0.16/octobot_script/resources/reports/css/style.css` & `OctoBot-Script-0.0.17/octobot_script/resources/reports/css/style.css`

 * *Files identical despite different names*

### Comparing `OctoBot-Script-0.0.16/octobot_script/resources/reports/css/w2ui_template.css` & `OctoBot-Script-0.0.17/octobot_script/resources/reports/css/w2ui_template.css`

 * *Files identical despite different names*

### Comparing `OctoBot-Script-0.0.16/octobot_script/resources/reports/default_report_template.html` & `OctoBot-Script-0.0.17/octobot_script/resources/reports/default_report_template.html`

 * *Files identical despite different names*

### Comparing `OctoBot-Script-0.0.16/octobot_script/resources/reports/header.html` & `OctoBot-Script-0.0.17/octobot_script/resources/reports/header.html`

 * *Files identical despite different names*

### Comparing `OctoBot-Script-0.0.16/octobot_script/resources/reports/js/graphs.js` & `OctoBot-Script-0.0.17/octobot_script/resources/reports/js/graphs.js`

 * *Files identical despite different names*

### Comparing `OctoBot-Script-0.0.16/octobot_script/resources/reports/js/tables.js` & `OctoBot-Script-0.0.17/octobot_script/resources/reports/js/tables.js`

 * *Files identical despite different names*

### Comparing `OctoBot-Script-0.0.16/octobot_script/resources/reports/js/texts.js` & `OctoBot-Script-0.0.17/octobot_script/resources/reports/js/texts.js`

 * *Files identical despite different names*

### Comparing `OctoBot-Script-0.0.16/octobot_script/resources/reports/scripts.html` & `OctoBot-Script-0.0.17/octobot_script/resources/reports/scripts.html`

 * *Files identical despite different names*

### Comparing `OctoBot-Script-0.0.16/setup.py` & `OctoBot-Script-0.0.17/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import setup
 from distutils.command.install import install
 
 
 # from octobot_script import PROJECT_NAME, VERSION
 # todo figure out how not to import octobot_script.__init__.py here
 PROJECT_NAME = "OctoBot-Script"
-VERSION = "0.0.16"  # major.minor.revision
+VERSION = "0.0.17"  # major.minor.revision
 
 
 def _post_install():
     import octobot_script.cli
     asyncio.run(octobot_script.cli.install_all_tentacles(True))
```

### Comparing `OctoBot-Script-0.0.16/tests/api/__init__.py` & `OctoBot-Script-0.0.17/tests/api/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Script-0.0.16/tests/api/test_data_fetching.py` & `OctoBot-Script-0.0.17/tests/api/test_data_fetching.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Script-0.0.16/tests/api/test_execution.py` & `OctoBot-Script-0.0.17/tests/api/test_execution.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Script-0.0.16/tests/functionnal/__init__.py` & `OctoBot-Script-0.0.17/tests/functionnal/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Script-0.0.16/tests/functionnal/example_scripts/__init__.py` & `OctoBot-Script-0.0.17/tests/functionnal/example_scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Script-0.0.16/tests/functionnal/example_scripts/test_precomputed_vs_iteration_rsi.py` & `OctoBot-Script-0.0.17/tests/functionnal/example_scripts/test_precomputed_vs_iteration_rsi.py`

 * *Files identical despite different names*

