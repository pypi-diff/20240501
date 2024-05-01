# Comparing `tmp/ikabot-7.0.2.tar.gz` & `tmp/ikabot-7.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ikabot-7.0.2.tar", last modified: Sat Apr 27 17:56:14 2024, max compression
+gzip compressed data, was "ikabot-7.0.3.tar", last modified: Wed May  1 14:38:34 2024, max compression
```

## Comparing `ikabot-7.0.2.tar` & `ikabot-7.0.3.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:56:14.692282 ikabot-7.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-27 17:56:10.000000 ikabot-7.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-27 17:56:10.000000 ikabot-7.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-27 17:56:14.692282 ikabot-7.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-27 17:56:10.000000 ikabot-7.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:56:14.676282 ikabot-7.0.2/ikabot/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10909 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/command_line.py
--rw-r--r--   0 runner    (1001) docker     (127)     5123 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:56:14.684282 ikabot-7.0.2/ikabot/function/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12042 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/activateMiracle.py
--rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/activateShrine.py
--rw-r--r--   0 runner    (1001) docker     (127)     5943 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/alertAttacks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/alertLowWine.py
--rw-r--r--   0 runner    (1001) docker     (127)    22648 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/attackBarbarians.py
--rw-r--r--   0 runner    (1001) docker     (127)    15191 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/autoPirate.py
--rw-r--r--   0 runner    (1001) docker     (127)    11721 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/buyResources.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/checkForUpdate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/constructBuilding.py
--rw-r--r--   0 runner    (1001) docker     (127)    22509 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/constructionList.py
--rw-r--r--   0 runner    (1001) docker     (127)    52825 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/decaptchaConf.py
--rw-r--r--   0 runner    (1001) docker     (127)    14348 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/distributeResources.py
--rw-r--r--   0 runner    (1001) docker     (127)     6899 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/donate.py
--rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/donationBot.py
--rw-r--r--   0 runner    (1001) docker     (127)    24043 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/dumpWorld.py
--rw-r--r--   0 runner    (1001) docker     (127)     7969 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/getStatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/importExportCookie.py
--rw-r--r--   0 runner    (1001) docker     (127)     8564 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/investigate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/killTasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/loadCustomModule.py
--rw-r--r--   0 runner    (1001) docker     (127)    20484 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/loginDaily.py
--rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/proxyConf.py
--rw-r--r--   0 runner    (1001) docker     (127)     8748 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/searchForIslandSpaces.py
--rw-r--r--   0 runner    (1001) docker     (127)    15397 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/sellResources.py
--rw-r--r--   0 runner    (1001) docker     (127)     5161 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/sendResources.py
--rw-r--r--   0 runner    (1001) docker     (127)     4866 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/shipMovements.py
--rw-r--r--   0 runner    (1001) docker     (127)     9303 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/stationArmy.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/testTelegramBot.py
--rw-r--r--   0 runner    (1001) docker     (127)    17449 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/trainArmy.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/vacationMode.py
--rw-r--r--   0 runner    (1001) docker     (127)    64399 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/function/webServer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:56:14.684282 ikabot-7.0.2/ikabot/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5777 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/helpers/aesCipher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/helpers/apiComm.py
--rw-r--r--   0 runner    (1001) docker     (127)    10619 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/helpers/botComm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/helpers/dns.py
--rw-r--r--   0 runner    (1001) docker     (127)     9125 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/helpers/getJson.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/helpers/gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/helpers/market.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/helpers/naval.py
--rw-r--r--   0 runner    (1001) docker     (127)     9342 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/helpers/pedirInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     7886 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/helpers/planRoutes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/helpers/process.py
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/helpers/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/helpers/signals.py
--rw-r--r--   0 runner    (1001) docker     (127)     4568 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/helpers/varios.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:56:14.676282 ikabot-7.0.2/ikabot/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:56:14.676282 ikabot-7.0.2/ikabot/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:56:14.688282 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/activateMiracle.po
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/aesCipher.po
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/alertAttacks.po
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/alertLowWine.po
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/botComm.po
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/buyResources.po
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/checkForUpdate.po
--rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/command_line.po
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/config.po
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/constructBuilding.po
--rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/constructionList.po
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/distributeResources.po
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/donate.po
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/donationBot.po
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/getStatus.po
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/gui.mo
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/gui.po
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/loginDaily.po
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/pedirInfo.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/pedirInfo.po
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/searchForIslandSpaces.po
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/sellResources.po
--rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/sendResources.po
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/session.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/session.po
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/shipMovements.po
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/signals.mo
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/signals.po
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/trainArmy.pot
--rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/trainFleets.po
--rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/trainTroops.po
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/update.po
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/vacationMode.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:56:14.688282 ikabot-7.0.2/ikabot/web/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    59889 2024-04-27 17:56:10.000000 ikabot-7.0.2/ikabot/web/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:56:14.692282 ikabot-7.0.2/ikabot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-27 17:56:14.000000 ikabot-7.0.2/ikabot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-04-27 17:56:14.000000 ikabot-7.0.2/ikabot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 17:56:14.000000 ikabot-7.0.2/ikabot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-27 17:56:14.000000 ikabot-7.0.2/ikabot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-27 17:56:14.000000 ikabot-7.0.2/ikabot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-27 17:56:14.000000 ikabot-7.0.2/ikabot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 17:56:14.692282 ikabot-7.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-27 17:56:10.000000 ikabot-7.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:38:34.399276 ikabot-7.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-01 14:38:29.000000 ikabot-7.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-01 14:38:29.000000 ikabot-7.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-05-01 14:38:34.399276 ikabot-7.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-01 14:38:29.000000 ikabot-7.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:38:34.383276 ikabot-7.0.3/ikabot/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11282 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/command_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5123 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:38:34.387276 ikabot-7.0.3/ikabot/function/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12042 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/function/activateMiracle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/function/activateShrine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5943 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/function/alertAttacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/function/alertLowWine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22648 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/function/attackBarbarians.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15191 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/function/autoPirate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11721 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/function/buyResources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/function/checkForUpdate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/function/constructBuilding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22509 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/function/constructionList.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52825 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/function/decaptchaConf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14348 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/function/distributeResources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6899 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/function/donate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/function/donationBot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24043 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/function/dumpWorld.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7969 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/function/getStatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/function/importExportCookie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8564 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/function/investigate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/function/killTasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/function/loadCustomModule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20484 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/function/loginDaily.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/function/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/function/proxyConf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8748 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/function/searchForIslandSpaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15397 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/function/sellResources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5161 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/function/sendResources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4866 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/function/shipMovements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9303 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/function/stationArmy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/function/testTelegramBot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17449 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/function/trainArmy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/function/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/function/vacationMode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64399 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/function/webServer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:38:34.391276 ikabot-7.0.3/ikabot/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5777 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/helpers/aesCipher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/helpers/apiComm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10619 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/helpers/botComm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/helpers/dns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9125 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/helpers/getJson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/helpers/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/helpers/market.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/helpers/naval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9342 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/helpers/pedirInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7886 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/helpers/planRoutes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/helpers/process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/helpers/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/helpers/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4568 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/helpers/varios.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:38:34.379276 ikabot-7.0.3/ikabot/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:38:34.379276 ikabot-7.0.3/ikabot/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:38:34.395276 ikabot-7.0.3/ikabot/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/locale/es/LC_MESSAGES/activateMiracle.po
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/locale/es/LC_MESSAGES/aesCipher.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/locale/es/LC_MESSAGES/alertAttacks.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/locale/es/LC_MESSAGES/alertLowWine.po
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/locale/es/LC_MESSAGES/botComm.po
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/locale/es/LC_MESSAGES/buyResources.po
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/locale/es/LC_MESSAGES/checkForUpdate.po
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/locale/es/LC_MESSAGES/command_line.po
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/locale/es/LC_MESSAGES/config.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/locale/es/LC_MESSAGES/constructBuilding.po
+-rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/locale/es/LC_MESSAGES/constructionList.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/locale/es/LC_MESSAGES/distributeResources.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/locale/es/LC_MESSAGES/donate.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/locale/es/LC_MESSAGES/donationBot.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/locale/es/LC_MESSAGES/getStatus.po
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/locale/es/LC_MESSAGES/gui.mo
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/locale/es/LC_MESSAGES/gui.po
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/locale/es/LC_MESSAGES/loginDaily.po
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/locale/es/LC_MESSAGES/pedirInfo.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/locale/es/LC_MESSAGES/pedirInfo.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/locale/es/LC_MESSAGES/searchForIslandSpaces.po
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/locale/es/LC_MESSAGES/sellResources.po
+-rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/locale/es/LC_MESSAGES/sendResources.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/locale/es/LC_MESSAGES/session.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/locale/es/LC_MESSAGES/session.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/locale/es/LC_MESSAGES/shipMovements.po
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/locale/es/LC_MESSAGES/signals.mo
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/locale/es/LC_MESSAGES/signals.po
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/locale/es/LC_MESSAGES/trainArmy.pot
+-rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/locale/es/LC_MESSAGES/trainFleets.po
+-rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/locale/es/LC_MESSAGES/trainTroops.po
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/locale/es/LC_MESSAGES/update.po
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/locale/es/LC_MESSAGES/vacationMode.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:38:34.395276 ikabot-7.0.3/ikabot/web/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59889 2024-05-01 14:38:29.000000 ikabot-7.0.3/ikabot/web/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:38:34.395276 ikabot-7.0.3/ikabot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-05-01 14:38:34.000000 ikabot-7.0.3/ikabot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-05-01 14:38:34.000000 ikabot-7.0.3/ikabot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 14:38:34.000000 ikabot-7.0.3/ikabot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-01 14:38:34.000000 ikabot-7.0.3/ikabot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-01 14:38:34.000000 ikabot-7.0.3/ikabot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-01 14:38:34.000000 ikabot-7.0.3/ikabot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 14:38:34.399276 ikabot-7.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-01 14:38:29.000000 ikabot-7.0.3/setup.py
```

### Comparing `ikabot-7.0.2/LICENSE` & `ikabot-7.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/PKG-INFO` & `ikabot-7.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: ikabot
-Version: 7.0.2
+Version: 7.0.3
 Home-page: https://github.com/Ikabot-Collective/ikabot
 Author: physics-sp
 Author-email: physics-sp@protonmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: requests[socks]
 Requires-Dist: cryptography
 Requires-Dist: psutil
+Provides-Extra: webserver
+Requires-Dist: flask; extra == "webserver"
 
 <div align="center">
 
 ![Ikabot Banner](assets/banner.png)
 
 [![Downloads](https://static.pepy.tech/badge/ikabot)](https://pepy.tech/project/ikabot) ![GitHub Repo stars](https://img.shields.io/github/stars/Ikabot-Collective/ikabot?style=flat) ![licence](https://img.shields.io/github/license/Ikabot-Collective/ikabot?style=flat)
```

#### html2text {}

```diff
@@ -1,13 +1,14 @@
-Metadata-Version: 2.1 Name: ikabot Version: 7.0.2 Home-page: https://
+Metadata-Version: 2.1 Name: ikabot Version: 7.0.3 Home-page: https://
 github.com/Ikabot-Collective/ikabot Author: physics-sp Author-email: physics-
 sp@protonmail.com License: MIT Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Description-Content-Type:
 text/markdown License-File: LICENSE Requires-Dist: requests Requires-Dist:
-requests[socks] Requires-Dist: cryptography Requires-Dist: psutil
+requests[socks] Requires-Dist: cryptography Requires-Dist: psutil Provides-
+Extra: webserver Requires-Dist: flask; extra == "webserver"
   ![Ikabot Banner](assets/banner.png) [![Downloads](https://static.pepy.tech/
 badge/ikabot)](https://pepy.tech/project/ikabot) ![GitHub Repo stars](https://
   img.shields.io/github/stars/Ikabot-Collective/ikabot?style=flat) ![licence]
   (https://img.shields.io/github/license/Ikabot-Collective/ikabot?style=flat)
  Ikabot is a cross-platform Python program that enhances your Ikariam game by
    offering premium features for free, focusing on city management, warfare
      strategies, and streamlined alerts. -[Discover the features](https://
```

### Comparing `ikabot-7.0.2/README.md` & `ikabot-7.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/command_line.py` & `ikabot-7.0.3/ikabot/command_line.py`

 * *Files 4% similar despite different names*

```diff
@@ -230,20 +230,20 @@
             selected += 1200
 
     if selected == 20:
         print(_("(0) Back"))
         print(_("(1) Monitor islands"))
         print(_("(2) Dump & Search world"))
         
-        selected = read(min=0, max=8, digit=True)
+        selected = read(min=0, max=2, digit=True)
         if selected == 0:
             menu(session)
             return
         if selected > 0:
-            selected += 2100
+            selected += 2000
 
     if selected == 21:
         banner()
         print(_("(0) Back"))
         print(_("(1) Configure Proxy"))
         if telegramDataIsValid(session):
             print(_("(2) Change the Telegram data"))
@@ -335,7 +335,14 @@
 
 
 if __name__ == "__main__":
     # On Windows calling this function is necessary.
     if sys.platform.startswith("win"):
         multiprocessing.freeze_support()
     main()
+
+#############################################################
+# This is necessary to ensure that flask is frozen together #
+# with other requirements when creating ikabot.exe          #
+try: import flask                                           #
+except: pass                                                #
+#############################################################
```

### Comparing `ikabot-7.0.2/ikabot/config.py` & `ikabot-7.0.3/ikabot/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import gettext
 import locale
 import os
 import random
 
 # Version changed automatically by the release pipeline
-IKABOT_VERSION = "7.0.2"
+IKABOT_VERSION = "7.0.3"
 
 IKABOT_VERSION_TAG = "v" + IKABOT_VERSION
 
 local = locale.setlocale(locale.LC_ALL, "")
 if "es_" in local:
     languages = ["es"]
 else:
```

### Comparing `ikabot-7.0.2/ikabot/function/activateMiracle.py` & `ikabot-7.0.3/ikabot/function/activateMiracle.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/function/activateShrine.py` & `ikabot-7.0.3/ikabot/function/activateShrine.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/function/alertAttacks.py` & `ikabot-7.0.3/ikabot/function/alertAttacks.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/function/alertLowWine.py` & `ikabot-7.0.3/ikabot/function/alertLowWine.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/function/attackBarbarians.py` & `ikabot-7.0.3/ikabot/function/attackBarbarians.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/function/autoPirate.py` & `ikabot-7.0.3/ikabot/function/autoPirate.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/function/buyResources.py` & `ikabot-7.0.3/ikabot/function/buyResources.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/function/checkForUpdate.py` & `ikabot-7.0.3/ikabot/function/checkForUpdate.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/function/constructBuilding.py` & `ikabot-7.0.3/ikabot/function/constructBuilding.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/function/constructionList.py` & `ikabot-7.0.3/ikabot/function/constructionList.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/function/decaptchaConf.py` & `ikabot-7.0.3/ikabot/function/decaptchaConf.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/function/distributeResources.py` & `ikabot-7.0.3/ikabot/function/distributeResources.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/function/donate.py` & `ikabot-7.0.3/ikabot/function/donate.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/function/donationBot.py` & `ikabot-7.0.3/ikabot/function/donationBot.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/function/dumpWorld.py` & `ikabot-7.0.3/ikabot/function/dumpWorld.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/function/getStatus.py` & `ikabot-7.0.3/ikabot/function/getStatus.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/function/importExportCookie.py` & `ikabot-7.0.3/ikabot/function/importExportCookie.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/function/investigate.py` & `ikabot-7.0.3/ikabot/function/investigate.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/function/killTasks.py` & `ikabot-7.0.3/ikabot/function/killTasks.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/function/loadCustomModule.py` & `ikabot-7.0.3/ikabot/function/loadCustomModule.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/function/loginDaily.py` & `ikabot-7.0.3/ikabot/function/loginDaily.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/function/logs.py` & `ikabot-7.0.3/ikabot/function/logs.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/function/proxyConf.py` & `ikabot-7.0.3/ikabot/function/proxyConf.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/function/searchForIslandSpaces.py` & `ikabot-7.0.3/ikabot/function/searchForIslandSpaces.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/function/sellResources.py` & `ikabot-7.0.3/ikabot/function/sellResources.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/function/sendResources.py` & `ikabot-7.0.3/ikabot/function/sendResources.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/function/shipMovements.py` & `ikabot-7.0.3/ikabot/function/shipMovements.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/function/stationArmy.py` & `ikabot-7.0.3/ikabot/function/stationArmy.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/function/testTelegramBot.py` & `ikabot-7.0.3/ikabot/function/testTelegramBot.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/function/trainArmy.py` & `ikabot-7.0.3/ikabot/function/trainArmy.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/function/update.py` & `ikabot-7.0.3/ikabot/function/update.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/function/vacationMode.py` & `ikabot-7.0.3/ikabot/function/vacationMode.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/function/webServer.py` & `ikabot-7.0.3/ikabot/function/webServer.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/helpers/aesCipher.py` & `ikabot-7.0.3/ikabot/helpers/aesCipher.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/helpers/apiComm.py` & `ikabot-7.0.3/ikabot/helpers/apiComm.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/helpers/botComm.py` & `ikabot-7.0.3/ikabot/helpers/botComm.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/helpers/dns.py` & `ikabot-7.0.3/ikabot/helpers/dns.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/helpers/getJson.py` & `ikabot-7.0.3/ikabot/helpers/getJson.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/helpers/gui.py` & `ikabot-7.0.3/ikabot/helpers/gui.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/helpers/market.py` & `ikabot-7.0.3/ikabot/helpers/market.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/helpers/naval.py` & `ikabot-7.0.3/ikabot/helpers/naval.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/helpers/pedirInfo.py` & `ikabot-7.0.3/ikabot/helpers/pedirInfo.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/helpers/planRoutes.py` & `ikabot-7.0.3/ikabot/helpers/planRoutes.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/helpers/process.py` & `ikabot-7.0.3/ikabot/helpers/process.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/helpers/resources.py` & `ikabot-7.0.3/ikabot/helpers/resources.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/helpers/signals.py` & `ikabot-7.0.3/ikabot/helpers/signals.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/helpers/varios.py` & `ikabot-7.0.3/ikabot/helpers/varios.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/activateMiracle.po` & `ikabot-7.0.3/ikabot/locale/es/LC_MESSAGES/activateMiracle.po`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/aesCipher.po` & `ikabot-7.0.3/ikabot/locale/es/LC_MESSAGES/aesCipher.po`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/alertAttacks.po` & `ikabot-7.0.3/ikabot/locale/es/LC_MESSAGES/alertAttacks.po`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/alertLowWine.po` & `ikabot-7.0.3/ikabot/locale/es/LC_MESSAGES/alertLowWine.po`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/botComm.po` & `ikabot-7.0.3/ikabot/locale/es/LC_MESSAGES/botComm.po`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/buyResources.po` & `ikabot-7.0.3/ikabot/locale/es/LC_MESSAGES/buyResources.po`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/checkForUpdate.po` & `ikabot-7.0.3/ikabot/locale/es/LC_MESSAGES/checkForUpdate.po`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/command_line.po` & `ikabot-7.0.3/ikabot/locale/es/LC_MESSAGES/command_line.po`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/config.po` & `ikabot-7.0.3/ikabot/locale/es/LC_MESSAGES/config.po`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/constructBuilding.po` & `ikabot-7.0.3/ikabot/locale/es/LC_MESSAGES/constructBuilding.po`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/constructionList.po` & `ikabot-7.0.3/ikabot/locale/es/LC_MESSAGES/constructionList.po`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/distributeResources.po` & `ikabot-7.0.3/ikabot/locale/es/LC_MESSAGES/distributeResources.po`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/donate.po` & `ikabot-7.0.3/ikabot/locale/es/LC_MESSAGES/donate.po`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/donationBot.po` & `ikabot-7.0.3/ikabot/locale/es/LC_MESSAGES/donationBot.po`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/getStatus.po` & `ikabot-7.0.3/ikabot/locale/es/LC_MESSAGES/getStatus.po`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/gui.po` & `ikabot-7.0.3/ikabot/locale/es/LC_MESSAGES/gui.po`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/loginDaily.po` & `ikabot-7.0.3/ikabot/locale/es/LC_MESSAGES/loginDaily.po`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/pedirInfo.mo` & `ikabot-7.0.3/ikabot/locale/es/LC_MESSAGES/pedirInfo.mo`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/pedirInfo.po` & `ikabot-7.0.3/ikabot/locale/es/LC_MESSAGES/pedirInfo.po`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/searchForIslandSpaces.po` & `ikabot-7.0.3/ikabot/locale/es/LC_MESSAGES/searchForIslandSpaces.po`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/sellResources.po` & `ikabot-7.0.3/ikabot/locale/es/LC_MESSAGES/sellResources.po`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/sendResources.po` & `ikabot-7.0.3/ikabot/locale/es/LC_MESSAGES/sendResources.po`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/session.mo` & `ikabot-7.0.3/ikabot/locale/es/LC_MESSAGES/session.mo`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/session.po` & `ikabot-7.0.3/ikabot/locale/es/LC_MESSAGES/session.po`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/shipMovements.po` & `ikabot-7.0.3/ikabot/locale/es/LC_MESSAGES/shipMovements.po`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/signals.po` & `ikabot-7.0.3/ikabot/locale/es/LC_MESSAGES/signals.po`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/trainArmy.pot` & `ikabot-7.0.3/ikabot/locale/es/LC_MESSAGES/trainArmy.pot`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/trainFleets.po` & `ikabot-7.0.3/ikabot/locale/es/LC_MESSAGES/trainFleets.po`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/trainTroops.po` & `ikabot-7.0.3/ikabot/locale/es/LC_MESSAGES/trainTroops.po`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/update.po` & `ikabot-7.0.3/ikabot/locale/es/LC_MESSAGES/update.po`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/locale/es/LC_MESSAGES/vacationMode.po` & `ikabot-7.0.3/ikabot/locale/es/LC_MESSAGES/vacationMode.po`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot/web/session.py` & `ikabot-7.0.3/ikabot/web/session.py`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/ikabot.egg-info/PKG-INFO` & `ikabot-7.0.3/ikabot.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: ikabot
-Version: 7.0.2
+Version: 7.0.3
 Home-page: https://github.com/Ikabot-Collective/ikabot
 Author: physics-sp
 Author-email: physics-sp@protonmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: requests[socks]
 Requires-Dist: cryptography
 Requires-Dist: psutil
+Provides-Extra: webserver
+Requires-Dist: flask; extra == "webserver"
 
 <div align="center">
 
 ![Ikabot Banner](assets/banner.png)
 
 [![Downloads](https://static.pepy.tech/badge/ikabot)](https://pepy.tech/project/ikabot) ![GitHub Repo stars](https://img.shields.io/github/stars/Ikabot-Collective/ikabot?style=flat) ![licence](https://img.shields.io/github/license/Ikabot-Collective/ikabot?style=flat)
```

#### html2text {}

```diff
@@ -1,13 +1,14 @@
-Metadata-Version: 2.1 Name: ikabot Version: 7.0.2 Home-page: https://
+Metadata-Version: 2.1 Name: ikabot Version: 7.0.3 Home-page: https://
 github.com/Ikabot-Collective/ikabot Author: physics-sp Author-email: physics-
 sp@protonmail.com License: MIT Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Description-Content-Type:
 text/markdown License-File: LICENSE Requires-Dist: requests Requires-Dist:
-requests[socks] Requires-Dist: cryptography Requires-Dist: psutil
+requests[socks] Requires-Dist: cryptography Requires-Dist: psutil Provides-
+Extra: webserver Requires-Dist: flask; extra == "webserver"
   ![Ikabot Banner](assets/banner.png) [![Downloads](https://static.pepy.tech/
 badge/ikabot)](https://pepy.tech/project/ikabot) ![GitHub Repo stars](https://
   img.shields.io/github/stars/Ikabot-Collective/ikabot?style=flat) ![licence]
   (https://img.shields.io/github/license/Ikabot-Collective/ikabot?style=flat)
  Ikabot is a cross-platform Python program that enhances your Ikariam game by
    offering premium features for free, focusing on city management, warfare
      strategies, and streamlined alerts. -[Discover the features](https://
```

### Comparing `ikabot-7.0.2/ikabot.egg-info/SOURCES.txt` & `ikabot-7.0.3/ikabot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ikabot-7.0.2/setup.py` & `ikabot-7.0.3/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     license="MIT",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Ikabot-Collective/ikabot",
     include_package_data=True,
     packages=setuptools.find_packages(),
     install_requires=["requests", "requests[socks]", "cryptography", "psutil"],
+    extras_require={"webServer": ["flask"]},
     entry_points={
         "console_scripts": ["ikabot=ikabot.command_line:main"],
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
     ],
```

