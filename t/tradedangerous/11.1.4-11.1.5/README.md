# Comparing `tmp/tradedangerous-11.1.4.tar.gz` & `tmp/tradedangerous-11.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tradedangerous-11.1.4.tar", last modified: Tue Apr 30 00:36:34 2024, max compression
+gzip compressed data, was "tradedangerous-11.1.5.tar", last modified: Wed May  1 10:27:03 2024, max compression
```

## Comparing `tradedangerous-11.1.4.tar` & `tradedangerous-11.1.5.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:36:34.551862 tradedangerous-11.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-04-30 00:36:34.551862 tradedangerous-11.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-30 00:36:34.551862 tradedangerous-11.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:36:34.535862 tradedangerous-11.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tests/test_bootstrap_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tests/test_bootstrap_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tests/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tests/test_peek.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tests/test_trade.py
--rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tests/test_trade_run.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/trade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:36:34.539862 tradedangerous-11.1.4/tradedangerous/
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36080 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     4559 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:36:34.543862 tradedangerous-11.1.4/tradedangerous/commands/
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/commands/TEMPLATE.py
--rw-r--r--   0 runner    (1001) docker     (127)     9516 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/commands/buildcache_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    13924 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/commands/buy_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     9462 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/commands/commandenv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/commands/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4405 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/commands/export_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/commands/import_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     8392 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/commands/local_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/commands/market_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     8460 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/commands/nav_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     7888 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/commands/olddata_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     6725 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/commands/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9207 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/commands/rares_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    47650 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/commands/run_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     7943 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/commands/sell_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     6918 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/commands/shipvendor_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    16219 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/commands/station_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/commands/trade_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    14551 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/commands/update_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    23318 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/commands/update_gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/corrections.py
--rw-r--r--   0 runner    (1001) docker     (127)     8653 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/csvexport.py
--rw-r--r--   0 runner    (1001) docker     (127)    17297 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/edscupdate.py
--rw-r--r--   0 runner    (1001) docker     (127)    14915 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/edsmupdate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6931 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/fs.py
--rw-r--r--   0 runner    (1001) docker     (127)    43676 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/jsonprices.py
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:36:34.543862 tradedangerous-11.1.4/tradedangerous/mfd/
--rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/mfd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:36:34.543862 tradedangerous-11.1.4/tradedangerous/mfd/saitek/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/mfd/saitek/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24840 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/mfd/saitek/directoutput.py
--rw-r--r--   0 runner    (1001) docker     (127)     5816 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/mfd/saitek/x52pro.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:36:34.547862 tradedangerous-11.1.4/tradedangerous/misc/
--rw-r--r--   0 runner    (1001) docker     (127)     8405 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/misc/checkpricebounds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/misc/clipboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/misc/coord64.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/misc/derp-sentinel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4931 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/misc/diff-system-csvs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/misc/eddb.py
--rw-r--r--   0 runner    (1001) docker     (127)    12149 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/misc/eddn.py
--rw-r--r--   0 runner    (1001) docker     (127)    14367 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/misc/edsc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/misc/edsm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/misc/importeddbstats.py
--rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/misc/prices-json-exp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/misc/progress.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:36:34.547862 tradedangerous-11.1.4/tradedangerous/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     7860 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42262 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/plugins/edapi_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)    14412 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/plugins/edcd_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)    22887 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/plugins/eddblink_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/plugins/edmc_batch_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)    23746 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/plugins/journal_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)    13469 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/plugins/netlog_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)    27048 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/plugins/spansh_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)     7425 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/prices.py
--rw-r--r--   0 runner    (1001) docker     (127)    11709 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/submit-distances.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:36:34.547862 tradedangerous-11.1.4/tradedangerous/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/templates/Added.csv
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/templates/Category.csv
--rw-r--r--   0 runner    (1001) docker     (127)    10483 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/templates/RareItem.csv
--rw-r--r--   0 runner    (1001) docker     (127)     7808 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/templates/TradeDangerous.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    42075 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/tradecalc.py
--rw-r--r--   0 runner    (1001) docker     (127)    72282 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/tradedb.py
--rw-r--r--   0 runner    (1001) docker     (127)    10576 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/tradeenv.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/tradeexcept.py
--rw-r--r--   0 runner    (1001) docker     (127)     8378 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/transfers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5186 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradedangerous/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-30 00:34:32.000000 tradedangerous-11.1.4/tradedangerous/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:36:34.547862 tradedangerous-11.1.4/tradedangerous.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-04-30 00:36:34.000000 tradedangerous-11.1.4/tradedangerous.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-04-30 00:36:34.000000 tradedangerous-11.1.4/tradedangerous.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 00:36:34.000000 tradedangerous-11.1.4/tradedangerous.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-30 00:36:34.000000 tradedangerous-11.1.4/tradedangerous.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 00:36:34.000000 tradedangerous-11.1.4/tradedangerous.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-30 00:36:34.000000 tradedangerous-11.1.4/tradedangerous.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-30 00:36:34.000000 tradedangerous-11.1.4/tradedangerous.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-30 00:33:50.000000 tradedangerous-11.1.4/tradegui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:27:03.040750 tradedangerous-11.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-01 10:27:03.040750 tradedangerous-11.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-01 10:27:03.040750 tradedangerous-11.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:27:03.028750 tradedangerous-11.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tests/test_bootstrap_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tests/test_bootstrap_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tests/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tests/test_peek.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tests/test_trade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tests/test_trade_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/trade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:27:03.032750 tradedangerous-11.1.5/tradedangerous/
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36080 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4559 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:27:03.036750 tradedangerous-11.1.5/tradedangerous/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/commands/TEMPLATE.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9516 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/commands/buildcache_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13924 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/commands/buy_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9462 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/commands/commandenv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/commands/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4405 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/commands/export_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/commands/import_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8392 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/commands/local_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/commands/market_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8460 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/commands/nav_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7888 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/commands/olddata_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6725 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/commands/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9207 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/commands/rares_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47650 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/commands/run_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7943 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/commands/sell_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6918 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/commands/shipvendor_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16219 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/commands/station_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/commands/trade_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14551 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/commands/update_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23318 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/commands/update_gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/corrections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8653 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/csvexport.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17297 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/edscupdate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14915 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/edsmupdate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6931 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43676 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/jsonprices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:27:03.036750 tradedangerous-11.1.5/tradedangerous/mfd/
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/mfd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:27:03.036750 tradedangerous-11.1.5/tradedangerous/mfd/saitek/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/mfd/saitek/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24840 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/mfd/saitek/directoutput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5816 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/mfd/saitek/x52pro.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:27:03.040750 tradedangerous-11.1.5/tradedangerous/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)     8405 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/misc/checkpricebounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/misc/clipboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/misc/coord64.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/misc/derp-sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4931 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/misc/diff-system-csvs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/misc/eddb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12149 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/misc/eddn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14367 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/misc/edsc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/misc/edsm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/misc/importeddbstats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/misc/prices-json-exp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/misc/progress.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:27:03.040750 tradedangerous-11.1.5/tradedangerous/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     7860 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42262 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/plugins/edapi_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14412 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/plugins/edcd_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21931 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/plugins/eddblink_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/plugins/edmc_batch_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23746 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/plugins/journal_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13469 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/plugins/netlog_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27048 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/plugins/spansh_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7425 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/prices.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11709 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/submit-distances.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:27:03.040750 tradedangerous-11.1.5/tradedangerous/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/templates/Added.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/templates/Category.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    10483 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/templates/RareItem.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     7808 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/templates/TradeDangerous.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42075 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/tradecalc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72282 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/tradedb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10576 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/tradeenv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/tradeexcept.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8378 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/transfers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5186 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradedangerous/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-01 10:26:11.000000 tradedangerous-11.1.5/tradedangerous/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:27:03.040750 tradedangerous-11.1.5/tradedangerous.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-01 10:27:03.000000 tradedangerous-11.1.5/tradedangerous.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-05-01 10:27:03.000000 tradedangerous-11.1.5/tradedangerous.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 10:27:03.000000 tradedangerous-11.1.5/tradedangerous.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-01 10:27:03.000000 tradedangerous-11.1.5/tradedangerous.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 10:27:03.000000 tradedangerous-11.1.5/tradedangerous.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-01 10:27:03.000000 tradedangerous-11.1.5/tradedangerous.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-01 10:27:03.000000 tradedangerous-11.1.5/tradedangerous.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-01 10:25:41.000000 tradedangerous-11.1.5/tradegui.py
```

### Comparing `tradedangerous-11.1.4/LICENSE` & `tradedangerous-11.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/PKG-INFO` & `tradedangerous-11.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tradedangerous
-Version: 11.1.4
+Version: 11.1.5
 Summary: Trade-Dangerous is a set of powerful trading tools for Elite Dangerous, organized around one of the most powerful trade run optimizers available.
 Home-page: https://github.com/eyeonus/Trade-Dangerous
 Author: eyeonus
 Author-email: eyeonus@gmail.com
 License: MPL
 Project-URL: Bug Tracker, https://github.com/eyeonus/Trade-Dangerous/issues
 Project-URL: Documentation, https://github.com/eyeonus/Trade-Dangerous/wiki
```

### Comparing `tradedangerous-11.1.4/README.md` & `tradedangerous-11.1.5/README.md`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/setup.py` & `tradedangerous-11.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tests/test_bootstrap_commands.py` & `tradedangerous-11.1.5/tests/test_bootstrap_commands.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tests/test_bootstrap_plugins.py` & `tradedangerous-11.1.5/tests/test_bootstrap_plugins.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tests/test_cache.py` & `tradedangerous-11.1.5/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tests/test_commands.py` & `tradedangerous-11.1.5/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tests/test_fs.py` & `tradedangerous-11.1.5/tests/test_fs.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tests/test_peek.py` & `tradedangerous-11.1.5/tests/test_peek.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tests/test_trade.py` & `tradedangerous-11.1.5/tests/test_trade.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tests/test_trade_run.py` & `tradedangerous-11.1.5/tests/test_trade_run.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tests/test_utils.py` & `tradedangerous-11.1.5/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/trade.py` & `tradedangerous-11.1.5/trade.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/__init__.py` & `tradedangerous-11.1.5/tradedangerous/__init__.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/cache.py` & `tradedangerous-11.1.5/tradedangerous/cache.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/cli.py` & `tradedangerous-11.1.5/tradedangerous/cli.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/commands/TEMPLATE.py` & `tradedangerous-11.1.5/tradedangerous/commands/TEMPLATE.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/commands/__init__.py` & `tradedangerous-11.1.5/tradedangerous/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/commands/buildcache_cmd.py` & `tradedangerous-11.1.5/tradedangerous/commands/buildcache_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/commands/buy_cmd.py` & `tradedangerous-11.1.5/tradedangerous/commands/buy_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/commands/commandenv.py` & `tradedangerous-11.1.5/tradedangerous/commands/commandenv.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/commands/exceptions.py` & `tradedangerous-11.1.5/tradedangerous/commands/exceptions.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/commands/export_cmd.py` & `tradedangerous-11.1.5/tradedangerous/commands/export_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/commands/import_cmd.py` & `tradedangerous-11.1.5/tradedangerous/commands/import_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/commands/local_cmd.py` & `tradedangerous-11.1.5/tradedangerous/commands/local_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/commands/market_cmd.py` & `tradedangerous-11.1.5/tradedangerous/commands/market_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/commands/nav_cmd.py` & `tradedangerous-11.1.5/tradedangerous/commands/nav_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/commands/olddata_cmd.py` & `tradedangerous-11.1.5/tradedangerous/commands/olddata_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/commands/parsing.py` & `tradedangerous-11.1.5/tradedangerous/commands/parsing.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/commands/rares_cmd.py` & `tradedangerous-11.1.5/tradedangerous/commands/rares_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/commands/run_cmd.py` & `tradedangerous-11.1.5/tradedangerous/commands/run_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/commands/sell_cmd.py` & `tradedangerous-11.1.5/tradedangerous/commands/sell_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/commands/shipvendor_cmd.py` & `tradedangerous-11.1.5/tradedangerous/commands/shipvendor_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/commands/station_cmd.py` & `tradedangerous-11.1.5/tradedangerous/commands/station_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/commands/trade_cmd.py` & `tradedangerous-11.1.5/tradedangerous/commands/trade_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/commands/update_cmd.py` & `tradedangerous-11.1.5/tradedangerous/commands/update_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/commands/update_gui.py` & `tradedangerous-11.1.5/tradedangerous/commands/update_gui.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/corrections.py` & `tradedangerous-11.1.5/tradedangerous/corrections.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/csvexport.py` & `tradedangerous-11.1.5/tradedangerous/csvexport.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/edscupdate.py` & `tradedangerous-11.1.5/tradedangerous/edscupdate.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/edsmupdate.py` & `tradedangerous-11.1.5/tradedangerous/edsmupdate.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/formatting.py` & `tradedangerous-11.1.5/tradedangerous/formatting.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/fs.py` & `tradedangerous-11.1.5/tradedangerous/fs.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/gui.py` & `tradedangerous-11.1.5/tradedangerous/gui.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/jsonprices.py` & `tradedangerous-11.1.5/tradedangerous/jsonprices.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/mapping.py` & `tradedangerous-11.1.5/tradedangerous/mapping.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/mfd/__init__.py` & `tradedangerous-11.1.5/tradedangerous/mfd/__init__.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/mfd/saitek/directoutput.py` & `tradedangerous-11.1.5/tradedangerous/mfd/saitek/directoutput.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/mfd/saitek/x52pro.py` & `tradedangerous-11.1.5/tradedangerous/mfd/saitek/x52pro.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/misc/checkpricebounds.py` & `tradedangerous-11.1.5/tradedangerous/misc/checkpricebounds.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/misc/clipboard.py` & `tradedangerous-11.1.5/tradedangerous/misc/clipboard.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/misc/coord64.py` & `tradedangerous-11.1.5/tradedangerous/misc/coord64.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/misc/derp-sentinel.py` & `tradedangerous-11.1.5/tradedangerous/misc/derp-sentinel.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/misc/diff-system-csvs.py` & `tradedangerous-11.1.5/tradedangerous/misc/diff-system-csvs.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/misc/eddb.py` & `tradedangerous-11.1.5/tradedangerous/misc/eddb.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/misc/eddn.py` & `tradedangerous-11.1.5/tradedangerous/misc/eddn.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/misc/edsc.py` & `tradedangerous-11.1.5/tradedangerous/misc/edsc.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/misc/edsm.py` & `tradedangerous-11.1.5/tradedangerous/misc/edsm.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/misc/importeddbstats.py` & `tradedangerous-11.1.5/tradedangerous/misc/importeddbstats.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/misc/prices-json-exp.py` & `tradedangerous-11.1.5/tradedangerous/misc/prices-json-exp.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/misc/progress.py` & `tradedangerous-11.1.5/tradedangerous/misc/progress.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/plugins/__init__.py` & `tradedangerous-11.1.5/tradedangerous/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/plugins/edapi_plug.py` & `tradedangerous-11.1.5/tradedangerous/plugins/edapi_plug.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/plugins/edcd_plug.py` & `tradedangerous-11.1.5/tradedangerous/plugins/edcd_plug.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/plugins/eddblink_plug.py` & `tradedangerous-11.1.5/tradedangerous/plugins/eddblink_plug.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,47 +8,26 @@
 from .. import plugins, cache, transfers
 from ..misc import progress as pbar
 from ..plugins import PluginException
 
 import certifi
 import csv
 import datetime
+from email.utils import parsedate_to_datetime
 import os
 import requests
 import sqlite3
 import ssl
 import typing
-import locale
-import platform
 
 
 if typing.TYPE_CHECKING:
     from typing import Optional
     from .. tradeenv import TradeEnv
 
-# Find the first English UTF-8 locale for use in parsing timestamps.
-LOCALE = None
-if platform.system() == 'Windows':
-    for lang in locale.windows_locale.values():
-        if "en" in lang:
-            LOCALE = lang
-            break
-else:
-    # for other operating systems
-    for lang in locale.locale_alias.values():
-        if "en" in lang and "UTF-8" in lang:
-            LOCALE = lang
-            break
-if not LOCALE:
-    raise PluginException(
-        "Unable to find compatible locale.\n" +
-        "This plugin needs an English, UTF-8 compatible " +
-        "locale installed in order to function correctly.\n" + 
-        "Please refer to your OS for instructions installing one."
-    )
 # Constants
 BASE_URL = os.environ.get('TD_SERVER') or "https://elite.tromador.com/files/"
 CONTEXT=ssl.create_default_context(cafile=certifi.where())
 
 
 class DecodingError(PluginException):
     pass
@@ -184,18 +163,16 @@
         headers = {"User-Agent": "Trade-Dangerous", "Accept-Encoding": "identity"}
         try:
             response = requests.head(url, headers=headers, timeout=70)
         except Exception as e:  # pylint: disable=broad-exception-caught
             self.tdenv.WARN("Problem with download:\n    URL: {}\n    Error: {}", url, str(e))
             return False
         
-        locale.setlocale(locale.LC_ALL, LOCALE)
         last_modified = response.headers.get("last-modified")
-        dump_mod_time = datetime.datetime.strptime(last_modified, "%a, %d %b %Y %H:%M:%S %Z").timestamp()
-        locale.setlocale(locale.LC_ALL, '')
+        dump_mod_time = parsedate_to_datetime(last_modified).timestamp()
         
         if Path.exists(localPath):
             local_mod_time = localPath.stat().st_mtime
             if local_mod_time >= dump_mod_time:
                 self.tdenv.DEBUG0("'{}': Dump is not more recent than Local.", path)
                 return False
         
@@ -348,16 +325,14 @@
         self.tdenv.NOTE("Optimizing database...")
         db.execute("VACUUM")
         self.tdb.close()
         
         self.tdenv.NOTE("Finished processing market data. End time = {}", self.now())
     
     def run(self):
-        self.tdenv.DEBUG2(f'Using "{LOCALE}" locale for parsing modified timestamps. Please include this information in any error reports.')
-        
         self.tdenv.ignoreUnknown = True
         
         # Create the /eddb folder for downloading the source files if it doesn't exist.
         try:
             Path(str(self.dataPath)).mkdir()
         except FileExistsError:
             pass
```

### Comparing `tradedangerous-11.1.4/tradedangerous/plugins/edmc_batch_plug.py` & `tradedangerous-11.1.5/tradedangerous/plugins/edmc_batch_plug.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/plugins/journal_plug.py` & `tradedangerous-11.1.5/tradedangerous/plugins/journal_plug.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/plugins/netlog_plug.py` & `tradedangerous-11.1.5/tradedangerous/plugins/netlog_plug.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/plugins/spansh_plug.py` & `tradedangerous-11.1.5/tradedangerous/plugins/spansh_plug.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/prices.py` & `tradedangerous-11.1.5/tradedangerous/prices.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/submit-distances.py` & `tradedangerous-11.1.5/tradedangerous/submit-distances.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/templates/Added.csv` & `tradedangerous-11.1.5/tradedangerous/templates/Added.csv`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/templates/RareItem.csv` & `tradedangerous-11.1.5/tradedangerous/templates/RareItem.csv`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/templates/TradeDangerous.sql` & `tradedangerous-11.1.5/tradedangerous/templates/TradeDangerous.sql`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/tools.py` & `tradedangerous-11.1.5/tradedangerous/tools.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/tradecalc.py` & `tradedangerous-11.1.5/tradedangerous/tradecalc.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/tradedb.py` & `tradedangerous-11.1.5/tradedangerous/tradedb.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/tradeenv.py` & `tradedangerous-11.1.5/tradedangerous/tradeenv.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/transfers.py` & `tradedangerous-11.1.5/tradedangerous/transfers.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/utils.py` & `tradedangerous-11.1.5/tradedangerous/utils.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradedangerous/version.py` & `tradedangerous-11.1.5/tradedangerous/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,9 +8,9 @@
 # this software so long as you include this copyright notice.
 # I guarantee there is at least one bug neither of us knew about.
 # --------------------------------------------------------------------
 
 """just keeper of current version"""
 
 # TODO: remember to update tests when version changes
-__version__ = '11.1.4'
+__version__ = '11.1.5'
```

### Comparing `tradedangerous-11.1.4/tradedangerous.egg-info/PKG-INFO` & `tradedangerous-11.1.5/tradedangerous.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tradedangerous
-Version: 11.1.4
+Version: 11.1.5
 Summary: Trade-Dangerous is a set of powerful trading tools for Elite Dangerous, organized around one of the most powerful trade run optimizers available.
 Home-page: https://github.com/eyeonus/Trade-Dangerous
 Author: eyeonus
 Author-email: eyeonus@gmail.com
 License: MPL
 Project-URL: Bug Tracker, https://github.com/eyeonus/Trade-Dangerous/issues
 Project-URL: Documentation, https://github.com/eyeonus/Trade-Dangerous/wiki
```

### Comparing `tradedangerous-11.1.4/tradedangerous.egg-info/SOURCES.txt` & `tradedangerous-11.1.5/tradedangerous.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.4/tradegui.py` & `tradedangerous-11.1.5/tradegui.py`

 * *Files identical despite different names*

