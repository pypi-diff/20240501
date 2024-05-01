# Comparing `tmp/yalexs-3.0.1.tar.gz` & `tmp/yalexs-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yalexs-3.0.1.tar", last modified: Tue Apr  2 20:53:38 2024, max compression
+gzip compressed data, was "yalexs-3.1.0.tar", last modified: Wed May  1 13:01:59 2024, max compression
```

## Comparing `yalexs-3.0.1.tar` & `yalexs-3.1.0.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2024-04-02 20:53:38.376696 yalexs-3.0.1/
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2024-04-02 20:53:38.357679 yalexs-3.0.1/.github/
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2024-04-02 20:53:38.360432 yalexs-3.0.1/.github/workflows/
--rw-r--r--   0 bdraco     (501) staff       (20)     2254 2023-05-17 14:08:38.000000 yalexs-3.0.1/.github/workflows/ci.yaml
--rw-r--r--   0 bdraco     (501) staff       (20)     1180 2023-02-17 14:03:03.000000 yalexs-3.0.1/.gitignore
--rw-r--r--   0 bdraco     (501) staff       (20)     1063 2023-02-17 14:03:03.000000 yalexs-3.0.1/LICENSE
--rw-r--r--   0 bdraco     (501) staff       (20)      398 2023-02-17 14:03:03.000000 yalexs-3.0.1/MANIFEST
--rw-r--r--   0 bdraco     (501) staff       (20)      908 2024-04-02 20:53:38.376638 yalexs-3.0.1/PKG-INFO
--rw-r--r--   0 bdraco     (501) staff       (20)     4569 2023-02-17 14:03:03.000000 yalexs-3.0.1/README.md
--rw-r--r--   0 bdraco     (501) staff       (20)       66 2023-02-17 14:03:03.000000 yalexs-3.0.1/build.sh
--rw-r--r--   0 bdraco     (501) staff       (20)     4283 2023-02-17 14:03:03.000000 yalexs-3.0.1/known_activities.md
--rw-r--r--   0 bdraco     (501) staff       (20)     1247 2024-02-28 07:31:33.000000 yalexs-3.0.1/pylintrc
--rw-r--r--   0 bdraco     (501) staff       (20)       91 2024-02-26 23:08:14.000000 yalexs-3.0.1/requirements.txt
--rw-r--r--   0 bdraco     (501) staff       (20)      141 2023-05-22 13:33:40.000000 yalexs-3.0.1/requirements_tests.txt
--rw-r--r--   0 bdraco     (501) staff       (20)      886 2024-04-02 20:53:38.376989 yalexs-3.0.1/setup.cfg
--rw-r--r--   0 bdraco     (501) staff       (20)     1054 2024-04-02 20:53:09.000000 yalexs-3.0.1/setup.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2024-04-02 20:53:38.362826 yalexs-3.0.1/tests/
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2024-04-02 20:53:38.371208 yalexs-3.0.1/tests/fixtures/
--rw-r--r--   0 bdraco     (501) staff       (20)      311 2023-02-17 14:03:03.000000 yalexs-3.0.1/tests/fixtures/auto_lock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      926 2023-02-17 14:03:03.000000 yalexs-3.0.1/tests/fixtures/auto_relock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      918 2023-02-17 14:03:03.000000 yalexs-3.0.1/tests/fixtures/auto_unlock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1331 2023-02-17 14:03:03.000000 yalexs-3.0.1/tests/fixtures/bluetooth_lock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      774 2023-02-17 14:03:03.000000 yalexs-3.0.1/tests/fixtures/door_closed_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      777 2023-02-17 14:03:03.000000 yalexs-3.0.1/tests/fixtures/door_closed_activity_wrong_deviceid.json
--rw-r--r--   0 bdraco     (501) staff       (20)      780 2023-02-17 14:03:03.000000 yalexs-3.0.1/tests/fixtures/door_closed_activity_wrong_houseid.json
--rw-r--r--   0 bdraco     (501) staff       (20)      772 2023-02-17 14:03:03.000000 yalexs-3.0.1/tests/fixtures/door_open_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1475 2023-02-17 14:03:03.000000 yalexs-3.0.1/tests/fixtures/doorbell_motion_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      907 2023-02-17 14:03:03.000000 yalexs-3.0.1/tests/fixtures/doorbell_motion_activity_no_image.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1501 2023-02-17 14:03:03.000000 yalexs-3.0.1/tests/fixtures/doorbell_motion_activity_old.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1495 2023-02-17 14:03:03.000000 yalexs-3.0.1/tests/fixtures/doorbell_motion_activity_wrong.json
--rw-r--r--   0 bdraco     (501) staff       (20)     3198 2023-02-17 14:03:03.000000 yalexs-3.0.1/tests/fixtures/get_doorbell.battery_full.json
--rw-r--r--   0 bdraco     (501) staff       (20)     3188 2023-02-17 14:03:03.000000 yalexs-3.0.1/tests/fixtures/get_doorbell.battery_low.json
--rw-r--r--   0 bdraco     (501) staff       (20)     3197 2023-02-17 14:03:03.000000 yalexs-3.0.1/tests/fixtures/get_doorbell.battery_medium.json
--rw-r--r--   0 bdraco     (501) staff       (20)     2488 2023-02-17 14:03:03.000000 yalexs-3.0.1/tests/fixtures/get_doorbell.json
--rw-r--r--   0 bdraco     (501) staff       (20)     3780 2023-02-17 14:03:03.000000 yalexs-3.0.1/tests/fixtures/get_doorbell.offline.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1898 2023-02-17 14:03:03.000000 yalexs-3.0.1/tests/fixtures/get_doorbell_missing_image.json
--rw-r--r--   0 bdraco     (501) staff       (20)     2255 2023-02-17 14:03:03.000000 yalexs-3.0.1/tests/fixtures/get_doorbells.json
--rw-r--r--   0 bdraco     (501) staff       (20)     9741 2023-02-17 14:03:03.000000 yalexs-3.0.1/tests/fixtures/get_house_activities.json
--rw-r--r--   0 bdraco     (501) staff       (20)     2744 2023-02-17 14:03:03.000000 yalexs-3.0.1/tests/fixtures/get_lock.doorsense_init.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1182 2023-02-17 14:03:03.000000 yalexs-3.0.1/tests/fixtures/get_lock.nostatus_with_doorsense.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1680 2023-02-17 14:03:03.000000 yalexs-3.0.1/tests/fixtures/get_lock.offline.json
--rw-r--r--   0 bdraco     (501) staff       (20)     2745 2023-02-17 14:03:03.000000 yalexs-3.0.1/tests/fixtures/get_lock.online.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1368 2023-02-17 14:03:03.000000 yalexs-3.0.1/tests/fixtures/get_lock.online_with_doorsense.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1373 2023-02-17 14:03:03.000000 yalexs-3.0.1/tests/fixtures/get_lock.online_with_doorsense_disabled.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1633 2023-02-17 14:03:03.000000 yalexs-3.0.1/tests/fixtures/get_lock_v2.online.json
--rw-r--r--   0 bdraco     (501) staff       (20)      408 2023-02-17 14:03:03.000000 yalexs-3.0.1/tests/fixtures/get_locks.json
--rw-r--r--   0 bdraco     (501) staff       (20)      664 2023-02-17 14:03:03.000000 yalexs-3.0.1/tests/fixtures/get_pins.json
--rw-r--r--   0 bdraco     (501) staff       (20)      444 2024-02-09 19:27:20.000000 yalexs-3.0.1/tests/fixtures/homekey_unlock_activity_v4.json
--rw-r--r--   0 bdraco     (501) staff       (20)      848 2023-02-17 14:03:03.000000 yalexs-3.0.1/tests/fixtures/keypad_lock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      682 2023-02-17 14:03:03.000000 yalexs-3.0.1/tests/fixtures/lock.json
--rw-r--r--   0 bdraco     (501) staff       (20)      366 2023-08-06 22:02:35.000000 yalexs-3.0.1/tests/fixtures/lock_accessory_motion_detect.json
--rw-r--r--   0 bdraco     (501) staff       (20)      800 2023-02-17 14:03:03.000000 yalexs-3.0.1/tests/fixtures/lock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)     2745 2023-08-06 22:09:05.000000 yalexs-3.0.1/tests/fixtures/lock_with_doorbell.online.json
--rw-r--r--   0 bdraco     (501) staff       (20)      641 2023-02-17 14:03:03.000000 yalexs-3.0.1/tests/fixtures/lock_without_doorstate.json
--rw-r--r--   0 bdraco     (501) staff       (20)      315 2023-02-17 14:03:03.000000 yalexs-3.0.1/tests/fixtures/manual_lock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      316 2024-03-18 22:03:45.000000 yalexs-3.0.1/tests/fixtures/manual_unlatch_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      321 2023-02-17 14:03:03.000000 yalexs-3.0.1/tests/fixtures/manual_unlock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      458 2023-02-17 14:03:03.000000 yalexs-3.0.1/tests/fixtures/pin_unlock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      409 2023-02-17 14:03:03.000000 yalexs-3.0.1/tests/fixtures/pin_unlock_activity_missing_image.json
--rw-r--r--   0 bdraco     (501) staff       (20)      479 2023-02-17 14:03:03.000000 yalexs-3.0.1/tests/fixtures/pin_unlock_activity_with_image.json
--rw-r--r--   0 bdraco     (501) staff       (20)      827 2023-02-17 14:03:03.000000 yalexs-3.0.1/tests/fixtures/remote_lock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      435 2023-02-17 14:03:03.000000 yalexs-3.0.1/tests/fixtures/remote_lock_activity_v4.json
--rw-r--r--   0 bdraco     (501) staff       (20)      449 2024-03-18 22:03:45.000000 yalexs-3.0.1/tests/fixtures/remote_unlatch_activity_v4.json
--rw-r--r--   0 bdraco     (501) staff       (20)      441 2023-02-17 14:03:03.000000 yalexs-3.0.1/tests/fixtures/remote_unlock_activity_v4.json
--rw-r--r--   0 bdraco     (501) staff       (20)      559 2023-02-17 14:03:03.000000 yalexs-3.0.1/tests/fixtures/remote_unlock_activity_v4_2.json
--rw-r--r--   0 bdraco     (501) staff       (20)      434 2023-09-21 06:28:29.000000 yalexs-3.0.1/tests/fixtures/rf_unlock_activity_v4.json
--rw-r--r--   0 bdraco     (501) staff       (20)      686 2023-02-17 14:03:03.000000 yalexs-3.0.1/tests/fixtures/unlock.json
--rw-r--r--   0 bdraco     (501) staff       (20)      732 2023-02-17 14:03:03.000000 yalexs-3.0.1/tests/fixtures/unlock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      648 2023-02-17 14:03:03.000000 yalexs-3.0.1/tests/fixtures/unlock_without_doorstate.json
--rw-r--r--   0 bdraco     (501) staff       (20)    20956 2024-03-18 22:03:45.000000 yalexs-3.0.1/tests/test_activity.py
--rw-r--r--   0 bdraco     (501) staff       (20)    34831 2024-03-18 22:03:45.000000 yalexs-3.0.1/tests/test_api.py
--rw-r--r--   0 bdraco     (501) staff       (20)    45572 2024-03-18 22:03:45.000000 yalexs-3.0.1/tests/test_api_async.py
--rw-r--r--   0 bdraco     (501) staff       (20)     7495 2023-02-17 14:03:03.000000 yalexs-3.0.1/tests/test_authenticator.py
--rw-r--r--   0 bdraco     (501) staff       (20)     8968 2023-05-17 14:08:38.000000 yalexs-3.0.1/tests/test_authenticator_async.py
--rw-r--r--   0 bdraco     (501) staff       (20)    20795 2024-03-18 22:03:45.000000 yalexs-3.0.1/tests/test_pubnub_activity.py
--rw-r--r--   0 bdraco     (501) staff       (20)    15746 2024-01-23 23:57:00.000000 yalexs-3.0.1/tests/test_util.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1316 2023-02-17 14:33:57.000000 yalexs-3.0.1/tox.ini
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2024-04-02 20:53:38.375244 yalexs-3.0.1/yalexs/
--rw-r--r--   0 bdraco     (501) staff       (20)      115 2024-04-02 20:53:09.000000 yalexs-3.0.1/yalexs/__init__.py
--rw-r--r--   0 bdraco     (501) staff       (20)    19678 2024-04-02 20:53:06.000000 yalexs-3.0.1/yalexs/activity.py
--rw-r--r--   0 bdraco     (501) staff       (20)    10788 2024-03-18 22:03:45.000000 yalexs-3.0.1/yalexs/api.py
--rw-r--r--   0 bdraco     (501) staff       (20)    16727 2024-03-18 22:03:45.000000 yalexs-3.0.1/yalexs/api_async.py
--rw-r--r--   0 bdraco     (501) staff       (20)    10653 2024-03-18 22:03:45.000000 yalexs-3.0.1/yalexs/api_common.py
--rw-r--r--   0 bdraco     (501) staff       (20)     4874 2023-08-21 13:01:43.000000 yalexs-3.0.1/yalexs/authenticator.py
--rw-r--r--   0 bdraco     (501) staff       (20)     5311 2023-08-21 13:01:43.000000 yalexs-3.0.1/yalexs/authenticator_async.py
--rw-r--r--   0 bdraco     (501) staff       (20)     5302 2023-08-21 13:01:43.000000 yalexs-3.0.1/yalexs/authenticator_common.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2024-04-02 20:53:38.376278 yalexs-3.0.1/yalexs/backports/
--rw-r--r--   0 bdraco     (501) staff       (20)        0 2023-05-17 14:08:38.000000 yalexs-3.0.1/yalexs/backports/__init__.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1021 2024-02-08 20:31:13.000000 yalexs-3.0.1/yalexs/backports/enum.py
--rw-r--r--   0 bdraco     (501) staff       (20)     2373 2024-02-09 19:25:59.000000 yalexs-3.0.1/yalexs/backports/functools.py
--rw-r--r--   0 bdraco     (501) staff       (20)     2222 2023-08-20 21:56:05.000000 yalexs-3.0.1/yalexs/bridge.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1283 2023-05-22 13:33:40.000000 yalexs-3.0.1/yalexs/const.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1717 2023-08-20 21:56:05.000000 yalexs-3.0.1/yalexs/device.py
--rw-r--r--   0 bdraco     (501) staff       (20)     5771 2024-02-28 07:31:33.000000 yalexs-3.0.1/yalexs/doorbell.py
--rw-r--r--   0 bdraco     (501) staff       (20)      919 2024-02-28 07:31:33.000000 yalexs-3.0.1/yalexs/exceptions.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1044 2023-05-18 17:02:22.000000 yalexs-3.0.1/yalexs/keypad.py
--rw-r--r--   0 bdraco     (501) staff       (20)     8562 2024-03-18 22:03:45.000000 yalexs-3.0.1/yalexs/lock.py
--rw-r--r--   0 bdraco     (501) staff       (20)     2439 2023-08-21 13:01:43.000000 yalexs-3.0.1/yalexs/pin.py
--rw-r--r--   0 bdraco     (501) staff       (20)     5418 2024-03-18 22:03:45.000000 yalexs-3.0.1/yalexs/pubnub_activity.py
--rw-r--r--   0 bdraco     (501) staff       (20)     4484 2023-05-22 13:11:27.000000 yalexs-3.0.1/yalexs/pubnub_async.py
--rw-r--r--   0 bdraco     (501) staff       (20)      565 2023-08-21 13:01:43.000000 yalexs-3.0.1/yalexs/time.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1175 2023-08-21 13:01:43.000000 yalexs-3.0.1/yalexs/users.py
--rw-r--r--   0 bdraco     (501) staff       (20)     4425 2024-02-28 07:31:33.000000 yalexs-3.0.1/yalexs/util.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2024-04-02 20:53:38.375863 yalexs-3.0.1/yalexs.egg-info/
--rw-r--r--   0 bdraco     (501) staff       (20)      908 2024-04-02 20:53:38.000000 yalexs-3.0.1/yalexs.egg-info/PKG-INFO
--rw-r--r--   0 bdraco     (501) staff       (20)     3189 2024-04-02 20:53:38.000000 yalexs-3.0.1/yalexs.egg-info/SOURCES.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        1 2024-04-02 20:53:38.000000 yalexs-3.0.1/yalexs.egg-info/dependency_links.txt
--rw-r--r--   0 bdraco     (501) staff       (20)      107 2024-04-02 20:53:38.000000 yalexs-3.0.1/yalexs.egg-info/requires.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        7 2024-04-02 20:53:38.000000 yalexs-3.0.1/yalexs.egg-info/top_level.txt
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2024-05-01 13:01:59.593856 yalexs-3.1.0/
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2024-05-01 13:01:59.578617 yalexs-3.1.0/.github/
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2024-05-01 13:01:59.581112 yalexs-3.1.0/.github/workflows/
+-rw-r--r--   0 bdraco     (501) staff       (20)     2319 2024-05-01 13:01:25.000000 yalexs-3.1.0/.github/workflows/ci.yaml
+-rw-r--r--   0 bdraco     (501) staff       (20)     1180 2023-02-17 14:03:03.000000 yalexs-3.1.0/.gitignore
+-rw-r--r--   0 bdraco     (501) staff       (20)     1063 2023-02-17 14:03:03.000000 yalexs-3.1.0/LICENSE
+-rw-r--r--   0 bdraco     (501) staff       (20)      398 2023-02-17 14:03:03.000000 yalexs-3.1.0/MANIFEST
+-rw-r--r--   0 bdraco     (501) staff       (20)      908 2024-05-01 13:01:59.593802 yalexs-3.1.0/PKG-INFO
+-rw-r--r--   0 bdraco     (501) staff       (20)     4569 2023-02-17 14:03:03.000000 yalexs-3.1.0/README.md
+-rw-r--r--   0 bdraco     (501) staff       (20)       66 2023-02-17 14:03:03.000000 yalexs-3.1.0/build.sh
+-rw-r--r--   0 bdraco     (501) staff       (20)     4283 2023-02-17 14:03:03.000000 yalexs-3.1.0/known_activities.md
+-rw-r--r--   0 bdraco     (501) staff       (20)     1247 2024-02-28 07:31:33.000000 yalexs-3.1.0/pylintrc
+-rw-r--r--   0 bdraco     (501) staff       (20)       91 2024-02-26 23:08:14.000000 yalexs-3.1.0/requirements.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)      141 2023-05-22 13:33:40.000000 yalexs-3.1.0/requirements_tests.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)      886 2024-05-01 13:01:59.594123 yalexs-3.1.0/setup.cfg
+-rw-r--r--   0 bdraco     (501) staff       (20)     1054 2024-05-01 13:01:27.000000 yalexs-3.1.0/setup.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2024-05-01 13:01:59.582171 yalexs-3.1.0/tests/
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2024-05-01 13:01:59.589990 yalexs-3.1.0/tests/fixtures/
+-rw-r--r--   0 bdraco     (501) staff       (20)      311 2023-02-17 14:03:03.000000 yalexs-3.1.0/tests/fixtures/auto_lock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      926 2023-02-17 14:03:03.000000 yalexs-3.1.0/tests/fixtures/auto_relock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      918 2023-02-17 14:03:03.000000 yalexs-3.1.0/tests/fixtures/auto_unlock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1331 2023-02-17 14:03:03.000000 yalexs-3.1.0/tests/fixtures/bluetooth_lock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      774 2023-02-17 14:03:03.000000 yalexs-3.1.0/tests/fixtures/door_closed_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      777 2023-02-17 14:03:03.000000 yalexs-3.1.0/tests/fixtures/door_closed_activity_wrong_deviceid.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      780 2023-02-17 14:03:03.000000 yalexs-3.1.0/tests/fixtures/door_closed_activity_wrong_houseid.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      772 2023-02-17 14:03:03.000000 yalexs-3.1.0/tests/fixtures/door_open_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1475 2023-02-17 14:03:03.000000 yalexs-3.1.0/tests/fixtures/doorbell_motion_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      907 2023-02-17 14:03:03.000000 yalexs-3.1.0/tests/fixtures/doorbell_motion_activity_no_image.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1501 2023-02-17 14:03:03.000000 yalexs-3.1.0/tests/fixtures/doorbell_motion_activity_old.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1495 2023-02-17 14:03:03.000000 yalexs-3.1.0/tests/fixtures/doorbell_motion_activity_wrong.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     3198 2023-02-17 14:03:03.000000 yalexs-3.1.0/tests/fixtures/get_doorbell.battery_full.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     3188 2023-02-17 14:03:03.000000 yalexs-3.1.0/tests/fixtures/get_doorbell.battery_low.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     3197 2023-02-17 14:03:03.000000 yalexs-3.1.0/tests/fixtures/get_doorbell.battery_medium.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     2488 2023-02-17 14:03:03.000000 yalexs-3.1.0/tests/fixtures/get_doorbell.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     3780 2023-02-17 14:03:03.000000 yalexs-3.1.0/tests/fixtures/get_doorbell.offline.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1898 2023-02-17 14:03:03.000000 yalexs-3.1.0/tests/fixtures/get_doorbell_missing_image.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     2255 2023-02-17 14:03:03.000000 yalexs-3.1.0/tests/fixtures/get_doorbells.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     9741 2023-02-17 14:03:03.000000 yalexs-3.1.0/tests/fixtures/get_house_activities.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     2744 2023-02-17 14:03:03.000000 yalexs-3.1.0/tests/fixtures/get_lock.doorsense_init.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1182 2023-02-17 14:03:03.000000 yalexs-3.1.0/tests/fixtures/get_lock.nostatus_with_doorsense.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1680 2023-02-17 14:03:03.000000 yalexs-3.1.0/tests/fixtures/get_lock.offline.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     2745 2023-02-17 14:03:03.000000 yalexs-3.1.0/tests/fixtures/get_lock.online.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1368 2023-02-17 14:03:03.000000 yalexs-3.1.0/tests/fixtures/get_lock.online_with_doorsense.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1373 2023-02-17 14:03:03.000000 yalexs-3.1.0/tests/fixtures/get_lock.online_with_doorsense_disabled.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1633 2023-02-17 14:03:03.000000 yalexs-3.1.0/tests/fixtures/get_lock_v2.online.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      408 2023-02-17 14:03:03.000000 yalexs-3.1.0/tests/fixtures/get_locks.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      664 2023-02-17 14:03:03.000000 yalexs-3.1.0/tests/fixtures/get_pins.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      444 2024-02-09 19:27:20.000000 yalexs-3.1.0/tests/fixtures/homekey_unlock_activity_v4.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      848 2023-02-17 14:03:03.000000 yalexs-3.1.0/tests/fixtures/keypad_lock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      682 2023-02-17 14:03:03.000000 yalexs-3.1.0/tests/fixtures/lock.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      366 2023-08-06 22:02:35.000000 yalexs-3.1.0/tests/fixtures/lock_accessory_motion_detect.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      800 2023-02-17 14:03:03.000000 yalexs-3.1.0/tests/fixtures/lock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     2745 2023-08-06 22:09:05.000000 yalexs-3.1.0/tests/fixtures/lock_with_doorbell.online.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      641 2023-02-17 14:03:03.000000 yalexs-3.1.0/tests/fixtures/lock_without_doorstate.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      315 2023-02-17 14:03:03.000000 yalexs-3.1.0/tests/fixtures/manual_lock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      316 2024-03-18 22:03:45.000000 yalexs-3.1.0/tests/fixtures/manual_unlatch_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      321 2023-02-17 14:03:03.000000 yalexs-3.1.0/tests/fixtures/manual_unlock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      458 2023-02-17 14:03:03.000000 yalexs-3.1.0/tests/fixtures/pin_unlock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      409 2023-02-17 14:03:03.000000 yalexs-3.1.0/tests/fixtures/pin_unlock_activity_missing_image.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      479 2023-02-17 14:03:03.000000 yalexs-3.1.0/tests/fixtures/pin_unlock_activity_with_image.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      827 2023-02-17 14:03:03.000000 yalexs-3.1.0/tests/fixtures/remote_lock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      435 2023-02-17 14:03:03.000000 yalexs-3.1.0/tests/fixtures/remote_lock_activity_v4.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      449 2024-03-18 22:03:45.000000 yalexs-3.1.0/tests/fixtures/remote_unlatch_activity_v4.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      441 2023-02-17 14:03:03.000000 yalexs-3.1.0/tests/fixtures/remote_unlock_activity_v4.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      559 2023-02-17 14:03:03.000000 yalexs-3.1.0/tests/fixtures/remote_unlock_activity_v4_2.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      434 2023-09-21 06:28:29.000000 yalexs-3.1.0/tests/fixtures/rf_unlock_activity_v4.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      686 2023-02-17 14:03:03.000000 yalexs-3.1.0/tests/fixtures/unlock.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      732 2023-02-17 14:03:03.000000 yalexs-3.1.0/tests/fixtures/unlock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      648 2023-02-17 14:03:03.000000 yalexs-3.1.0/tests/fixtures/unlock_without_doorstate.json
+-rw-r--r--   0 bdraco     (501) staff       (20)    20956 2024-03-18 22:03:45.000000 yalexs-3.1.0/tests/test_activity.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    34831 2024-03-18 22:03:45.000000 yalexs-3.1.0/tests/test_api.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    48791 2024-05-01 13:01:25.000000 yalexs-3.1.0/tests/test_api_async.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     7495 2023-02-17 14:03:03.000000 yalexs-3.1.0/tests/test_authenticator.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     8968 2023-05-17 14:08:38.000000 yalexs-3.1.0/tests/test_authenticator_async.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    20795 2024-03-18 22:03:45.000000 yalexs-3.1.0/tests/test_pubnub_activity.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    15746 2024-01-23 23:57:00.000000 yalexs-3.1.0/tests/test_util.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1316 2023-02-17 14:33:57.000000 yalexs-3.1.0/tox.ini
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2024-05-01 13:01:59.592767 yalexs-3.1.0/yalexs/
+-rw-r--r--   0 bdraco     (501) staff       (20)      115 2024-05-01 13:01:27.000000 yalexs-3.1.0/yalexs/__init__.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    19678 2024-04-02 20:53:06.000000 yalexs-3.1.0/yalexs/activity.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    10788 2024-03-18 22:03:45.000000 yalexs-3.1.0/yalexs/api.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    16727 2024-03-18 22:03:45.000000 yalexs-3.1.0/yalexs/api_async.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    10653 2024-03-18 22:03:45.000000 yalexs-3.1.0/yalexs/api_common.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     4874 2023-08-21 13:01:43.000000 yalexs-3.1.0/yalexs/authenticator.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     5311 2023-08-21 13:01:43.000000 yalexs-3.1.0/yalexs/authenticator_async.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     5302 2023-08-21 13:01:43.000000 yalexs-3.1.0/yalexs/authenticator_common.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2024-05-01 13:01:59.593611 yalexs-3.1.0/yalexs/backports/
+-rw-r--r--   0 bdraco     (501) staff       (20)        0 2023-05-17 14:08:38.000000 yalexs-3.1.0/yalexs/backports/__init__.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1021 2024-02-08 20:31:13.000000 yalexs-3.1.0/yalexs/backports/enum.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     2373 2024-02-09 19:25:59.000000 yalexs-3.1.0/yalexs/backports/functools.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     2222 2023-08-20 21:56:05.000000 yalexs-3.1.0/yalexs/bridge.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1283 2023-05-22 13:33:40.000000 yalexs-3.1.0/yalexs/const.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1717 2023-08-20 21:56:05.000000 yalexs-3.1.0/yalexs/device.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     5771 2024-02-28 07:31:33.000000 yalexs-3.1.0/yalexs/doorbell.py
+-rw-r--r--   0 bdraco     (501) staff       (20)      919 2024-02-28 07:31:33.000000 yalexs-3.1.0/yalexs/exceptions.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1044 2023-05-18 17:02:22.000000 yalexs-3.1.0/yalexs/keypad.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     8755 2024-05-01 13:01:25.000000 yalexs-3.1.0/yalexs/lock.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     2439 2023-08-21 13:01:43.000000 yalexs-3.1.0/yalexs/pin.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     5418 2024-03-18 22:03:45.000000 yalexs-3.1.0/yalexs/pubnub_activity.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     4484 2023-05-22 13:11:27.000000 yalexs-3.1.0/yalexs/pubnub_async.py
+-rw-r--r--   0 bdraco     (501) staff       (20)      565 2023-08-21 13:01:43.000000 yalexs-3.1.0/yalexs/time.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1175 2023-08-21 13:01:43.000000 yalexs-3.1.0/yalexs/users.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     4425 2024-02-28 07:31:33.000000 yalexs-3.1.0/yalexs/util.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2024-05-01 13:01:59.593308 yalexs-3.1.0/yalexs.egg-info/
+-rw-r--r--   0 bdraco     (501) staff       (20)      908 2024-05-01 13:01:59.000000 yalexs-3.1.0/yalexs.egg-info/PKG-INFO
+-rw-r--r--   0 bdraco     (501) staff       (20)     3189 2024-05-01 13:01:59.000000 yalexs-3.1.0/yalexs.egg-info/SOURCES.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        1 2024-05-01 13:01:59.000000 yalexs-3.1.0/yalexs.egg-info/dependency_links.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)      107 2024-05-01 13:01:59.000000 yalexs-3.1.0/yalexs.egg-info/requires.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        7 2024-05-01 13:01:59.000000 yalexs-3.1.0/yalexs.egg-info/top_level.txt
```

### Comparing `yalexs-3.0.1/.github/workflows/ci.yaml` & `yalexs-3.1.0/.github/workflows/ci.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -62,22 +62,24 @@
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install tox tox-gh-actions
     - name: Test with tox
       run: TOXENV=codecov tox
     - name: Upload coverage to Codecov
-      uses: codecov/codecov-action@v3
+      uses: codecov/codecov-action@v4
       with:
         flags: unittests
         env_vars: OS,PYTHON
         name: codecov-umbrella
         fail_ci_if_error: true
         verbose: true
-
+      env:
+        CODECOV_TOKEN: ${{ secrets.CODECOV_TOKEN }}
+  
   bandit:
     runs-on: ubuntu-latest
 
     strategy:
       matrix:
         python-version: [3.9]
```

### Comparing `yalexs-3.0.1/.gitignore` & `yalexs-3.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/LICENSE` & `yalexs-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/PKG-INFO` & `yalexs-3.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yalexs
-Version: 3.0.1
+Version: 3.1.0
 Summary: Python API for Yale Access (formerly August) Smart Lock and Doorbell
 Home-page: https://github.com/bdraco/yalexs
 Author: bdraco
 Author-email: nick@koston.org
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `yalexs-3.0.1/README.md` & `yalexs-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/known_activities.md` & `yalexs-3.1.0/known_activities.md`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/pylintrc` & `yalexs-3.1.0/pylintrc`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/setup.cfg` & `yalexs-3.1.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 3.0.1
+current_version = 3.1.0
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version="{current_version}"
 replace = version="{new_version}"
```

### Comparing `yalexs-3.0.1/setup.py` & `yalexs-3.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="yalexs",
-    version="3.0.1",
+    version="3.1.0",
     python_requires=">=3.9",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
```

### Comparing `yalexs-3.0.1/tests/fixtures/auto_relock_activity.json` & `yalexs-3.1.0/tests/fixtures/auto_relock_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/tests/fixtures/auto_unlock_activity.json` & `yalexs-3.1.0/tests/fixtures/auto_unlock_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/tests/fixtures/bluetooth_lock_activity.json` & `yalexs-3.1.0/tests/fixtures/bluetooth_lock_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/tests/fixtures/door_closed_activity.json` & `yalexs-3.1.0/tests/fixtures/door_closed_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/tests/fixtures/door_closed_activity_wrong_deviceid.json` & `yalexs-3.1.0/tests/fixtures/door_closed_activity_wrong_deviceid.json`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/tests/fixtures/door_closed_activity_wrong_houseid.json` & `yalexs-3.1.0/tests/fixtures/door_closed_activity_wrong_houseid.json`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/tests/fixtures/door_open_activity.json` & `yalexs-3.1.0/tests/fixtures/door_open_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/tests/fixtures/doorbell_motion_activity.json` & `yalexs-3.1.0/tests/fixtures/doorbell_motion_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/tests/fixtures/doorbell_motion_activity_no_image.json` & `yalexs-3.1.0/tests/fixtures/doorbell_motion_activity_no_image.json`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/tests/fixtures/doorbell_motion_activity_old.json` & `yalexs-3.1.0/tests/fixtures/doorbell_motion_activity_old.json`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/tests/fixtures/doorbell_motion_activity_wrong.json` & `yalexs-3.1.0/tests/fixtures/doorbell_motion_activity_wrong.json`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/tests/fixtures/get_doorbell.battery_full.json` & `yalexs-3.1.0/tests/fixtures/get_doorbell.battery_full.json`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/tests/fixtures/get_doorbell.battery_low.json` & `yalexs-3.1.0/tests/fixtures/get_doorbell.battery_low.json`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/tests/fixtures/get_doorbell.battery_medium.json` & `yalexs-3.1.0/tests/fixtures/get_doorbell.battery_medium.json`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/tests/fixtures/get_doorbell.json` & `yalexs-3.1.0/tests/fixtures/get_doorbell.json`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/tests/fixtures/get_doorbell.offline.json` & `yalexs-3.1.0/tests/fixtures/get_doorbell.offline.json`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/tests/fixtures/get_doorbell_missing_image.json` & `yalexs-3.1.0/tests/fixtures/get_doorbell_missing_image.json`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/tests/fixtures/get_doorbells.json` & `yalexs-3.1.0/tests/fixtures/get_doorbells.json`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/tests/fixtures/get_house_activities.json` & `yalexs-3.1.0/tests/fixtures/get_house_activities.json`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/tests/fixtures/get_lock.doorsense_init.json` & `yalexs-3.1.0/tests/fixtures/get_lock.doorsense_init.json`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/tests/fixtures/get_lock.nostatus_with_doorsense.json` & `yalexs-3.1.0/tests/fixtures/get_lock.nostatus_with_doorsense.json`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/tests/fixtures/get_lock.offline.json` & `yalexs-3.1.0/tests/fixtures/get_lock.offline.json`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/tests/fixtures/get_lock.online.json` & `yalexs-3.1.0/tests/fixtures/get_lock.online.json`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/tests/fixtures/get_lock.online_with_doorsense.json` & `yalexs-3.1.0/tests/fixtures/get_lock.online_with_doorsense.json`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/tests/fixtures/get_lock.online_with_doorsense_disabled.json` & `yalexs-3.1.0/tests/fixtures/get_lock.online_with_doorsense_disabled.json`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/tests/fixtures/get_lock_v2.online.json` & `yalexs-3.1.0/tests/fixtures/get_lock_v2.online.json`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/tests/fixtures/get_pins.json` & `yalexs-3.1.0/tests/fixtures/get_pins.json`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/tests/fixtures/keypad_lock_activity.json` & `yalexs-3.1.0/tests/fixtures/keypad_lock_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/tests/fixtures/lock.json` & `yalexs-3.1.0/tests/fixtures/lock.json`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/tests/fixtures/lock_activity.json` & `yalexs-3.1.0/tests/fixtures/lock_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/tests/fixtures/lock_with_doorbell.online.json` & `yalexs-3.1.0/tests/fixtures/lock_with_doorbell.online.json`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/tests/fixtures/lock_without_doorstate.json` & `yalexs-3.1.0/tests/fixtures/lock_without_doorstate.json`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/tests/fixtures/remote_lock_activity.json` & `yalexs-3.1.0/tests/fixtures/remote_lock_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/tests/fixtures/remote_unlock_activity_v4_2.json` & `yalexs-3.1.0/tests/fixtures/remote_unlock_activity_v4_2.json`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/tests/fixtures/unlock.json` & `yalexs-3.1.0/tests/fixtures/unlock.json`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/tests/fixtures/unlock_activity.json` & `yalexs-3.1.0/tests/fixtures/unlock_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/tests/fixtures/unlock_without_doorstate.json` & `yalexs-3.1.0/tests/fixtures/unlock_without_doorstate.json`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/tests/test_activity.py` & `yalexs-3.1.0/tests/test_activity.py`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/tests/test_api.py` & `yalexs-3.1.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/tests/test_api_async.py` & `yalexs-3.1.0/tests/test_api_async.py`

 * *Files 2% similar despite different names*

```diff
@@ -393,14 +393,15 @@
 
         api = ApiAsync(ClientSession())
         lock = await api.async_get_lock_detail(
             ACCESS_TOKEN, "A6697750D607098BAE8D6BAA11EF8063"
         )
 
         assert lock.doorbell is False
+        assert lock.unlatch_supported is False
         self.assertEqual("A6697750D607098BAE8D6BAA11EF8063", lock.device_id)
         self.assertEqual("Front Door Lock", lock.device_name)
         self.assertEqual("000000000000", lock.house_id)
         self.assertEqual("X2FSW05DGA", lock.serial_number)
         self.assertEqual("109717e9-3.0.44-3.0.30", lock.firmware_version)
         self.assertEqual(88, lock.battery_level)
         self.assertEqual("AUG-SL02-M02-S02", lock.model)
@@ -435,14 +436,30 @@
         lock = await api.async_get_lock_detail(
             ACCESS_TOKEN, "A6697750D607098BAE8D6BAA11EF8063"
         )
 
         assert lock.doorbell is True
 
     @aioresponses()
+    async def test_async_get_lock_with_unlatch(self, mock):
+        mock.get(
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_GET_LOCK_URL)
+            .format(lock_id="68895DD075A1444FAD4C00B273EEEF28"),
+            body=load_fixture("lock_with_unlatch.online.json"),
+        )
+
+        api = ApiAsync(ClientSession())
+        lock = await api.async_get_lock_detail(
+            ACCESS_TOKEN, "68895DD075A1444FAD4C00B273EEEF28"
+        )
+
+        assert lock.unlatch_supported is True
+
+    @aioresponses()
     async def test_async_get_v2_lock_detail_bridge_online(self, mock):
         mock.get(
             ApiCommon(DEFAULT_BRAND)
             .get_brand_url(API_GET_LOCK_URL)
             .format(lock_id="snip"),
             body=load_fixture("get_lock_v2.online.json"),
         )
@@ -771,14 +788,46 @@
         self.assertEqual(activities[1].device_id, "ABC123")
         self.assertEqual(activities[1].device_type, "lock")
         self.assertEqual(activities[1].action, "doorclosed")
         self.assertEqual(activities[0].activity_start_time, expected_lock_dt)
         self.assertEqual(activities[0].activity_end_time, expected_lock_dt)
 
     @aioresponses()
+    async def test_async_unlatch_return_activities_from_fixture(self, mock):
+        lock_id = 1234
+        mock.put(
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_UNLATCH_URL)
+            .format(lock_id=lock_id),
+            body=load_fixture("unlatch.json"),
+        )
+
+        api = ApiAsync(ClientSession())
+        activities = await api.async_unlatch_return_activities(ACCESS_TOKEN, lock_id)
+        expected_unlatch_dt = (
+            dateutil.parser.parse("2024-03-20T06:39:42.192Z")
+            .astimezone(tz=tzlocal())
+            .replace(tzinfo=None)
+        )
+
+        self.assertEqual(len(activities), 2)
+        self.assertIsInstance(activities[0], yalexs.activity.LockOperationActivity)
+        self.assertEqual(activities[0].device_id, "ABC123")
+        self.assertEqual(activities[0].device_type, "lock")
+        self.assertEqual(activities[0].action, "unlatch")
+        self.assertEqual(activities[0].activity_start_time, expected_unlatch_dt)
+        self.assertEqual(activities[0].activity_end_time, expected_unlatch_dt)
+        self.assertIsInstance(activities[1], yalexs.activity.DoorOperationActivity)
+        self.assertEqual(activities[1].device_id, "ABC123")
+        self.assertEqual(activities[1].device_type, "lock")
+        self.assertEqual(activities[1].action, "dooropen")
+        self.assertEqual(activities[1].activity_start_time, expected_unlatch_dt)
+        self.assertEqual(activities[1].activity_end_time, expected_unlatch_dt)
+
+    @aioresponses()
     async def test_async_unlock_return_activities_from_fixture(self, mock):
         lock_id = 1234
         mock.put(
             ApiCommon(DEFAULT_BRAND)
             .get_brand_url(API_UNLOCK_URL)
             .format(lock_id=lock_id),
             body=load_fixture("unlock.json"),
@@ -831,14 +880,42 @@
         self.assertEqual(activities[0].device_id, "ABC123")
         self.assertEqual(activities[0].device_type, "lock")
         self.assertEqual(activities[0].action, "lock")
         self.assertEqual(activities[0].activity_start_time, expected_lock_dt)
         self.assertEqual(activities[0].activity_end_time, expected_lock_dt)
 
     @aioresponses()
+    async def test_async_unlatch_return_activities_from_fixture_with_no_doorstate(
+        self, mock
+    ):
+        lock_id = 1234
+        mock.put(
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_UNLATCH_URL)
+            .format(lock_id=lock_id),
+            body=load_fixture("unlatch_without_doorstate.json"),
+        )
+
+        api = ApiAsync(ClientSession())
+        activities = await api.async_unlatch_return_activities(ACCESS_TOKEN, lock_id)
+        expected_unlatch_dt = (
+            dateutil.parser.parse("2024-03-20T06:39:42.192Z")
+            .astimezone(tz=tzlocal())
+            .replace(tzinfo=None)
+        )
+
+        self.assertEqual(len(activities), 1)
+        self.assertIsInstance(activities[0], yalexs.activity.LockOperationActivity)
+        self.assertEqual(activities[0].device_id, "ABC123")
+        self.assertEqual(activities[0].device_type, "lock")
+        self.assertEqual(activities[0].action, "unlatch")
+        self.assertEqual(activities[0].activity_start_time, expected_unlatch_dt)
+        self.assertEqual(activities[0].activity_end_time, expected_unlatch_dt)
+
+    @aioresponses()
     async def test_async_unlock_return_activities_from_fixture_with_no_doorstate(
         self, mock
     ):
         lock_id = 1234
         mock.put(
             ApiCommon(DEFAULT_BRAND)
             .get_brand_url(API_UNLOCK_URL)
```

### Comparing `yalexs-3.0.1/tests/test_authenticator.py` & `yalexs-3.1.0/tests/test_authenticator.py`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/tests/test_authenticator_async.py` & `yalexs-3.1.0/tests/test_authenticator_async.py`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/tests/test_pubnub_activity.py` & `yalexs-3.1.0/tests/test_pubnub_activity.py`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/tests/test_util.py` & `yalexs-3.1.0/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/tox.ini` & `yalexs-3.1.0/tox.ini`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/yalexs/activity.py` & `yalexs-3.1.0/yalexs/activity.py`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/yalexs/api.py` & `yalexs-3.1.0/yalexs/api.py`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/yalexs/api_async.py` & `yalexs-3.1.0/yalexs/api_async.py`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/yalexs/api_common.py` & `yalexs-3.1.0/yalexs/api_common.py`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/yalexs/authenticator.py` & `yalexs-3.1.0/yalexs/authenticator.py`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/yalexs/authenticator_async.py` & `yalexs-3.1.0/yalexs/authenticator_async.py`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/yalexs/authenticator_common.py` & `yalexs-3.1.0/yalexs/authenticator_common.py`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/yalexs/backports/enum.py` & `yalexs-3.1.0/yalexs/backports/enum.py`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/yalexs/backports/functools.py` & `yalexs-3.1.0/yalexs/backports/functools.py`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/yalexs/bridge.py` & `yalexs-3.1.0/yalexs/bridge.py`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/yalexs/const.py` & `yalexs-3.1.0/yalexs/const.py`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/yalexs/device.py` & `yalexs-3.1.0/yalexs/device.py`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/yalexs/doorbell.py` & `yalexs-3.1.0/yalexs/doorbell.py`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/yalexs/exceptions.py` & `yalexs-3.1.0/yalexs/exceptions.py`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/yalexs/keypad.py` & `yalexs-3.1.0/yalexs/keypad.py`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/yalexs/lock.py` & `yalexs-3.1.0/yalexs/lock.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,24 +19,26 @@
 JAMMED_STATUS = (
     "kAugLockState_UnknownStaticPosition",
     "FAILED_BRIDGE_ERROR_LOCK_JAMMED",
 )
 
 CLOSED_STATUS = ("closed", "kAugLockDoorState_Closed", "kAugDoorState_Closed")
 OPEN_STATUS = ("open", "kAugLockDoorState_Open", "kAugDoorState_Open")
-DISABLE_STATUS = ("init", "", None)
+DISABLE_STATUS = ("init", "kAugDoorState_Init", "", None)
 
 LOCK_STATUS_KEY = "status"
 DOOR_STATE_KEY = "doorState"
 
 DOORMAN_MODEL_TYPES = {7, 10}
+UNLATCH_MODEL_TYPES = {17}
 
 
 # Type 7 is a doorman
 # Type 10 is a doorman in the Swedish market
+# Type 17 is a Linus L2
 class Lock(Device):
     def __init__(self, device_id, data):
         super().__init__(
             device_id,
             data["LockName"],
             data["HouseID"],
         )
@@ -115,14 +117,18 @@
         return self._model
 
     @cached_property
     def doorbell(self) -> bool:
         return self._data["Type"] in DOORMAN_MODEL_TYPES
 
     @cached_property
+    def unlatch_supported(self) -> bool:
+        return self._data["Type"] in UNLATCH_MODEL_TYPES
+
+    @cached_property
     def battery_level(self):
         return self._battery_level
 
     @cached_property
     def keypad(self):
         return self._keypad_detail
```

### Comparing `yalexs-3.0.1/yalexs/pin.py` & `yalexs-3.1.0/yalexs/pin.py`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/yalexs/pubnub_activity.py` & `yalexs-3.1.0/yalexs/pubnub_activity.py`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/yalexs/pubnub_async.py` & `yalexs-3.1.0/yalexs/pubnub_async.py`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/yalexs/time.py` & `yalexs-3.1.0/yalexs/time.py`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/yalexs/users.py` & `yalexs-3.1.0/yalexs/users.py`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/yalexs/util.py` & `yalexs-3.1.0/yalexs/util.py`

 * *Files identical despite different names*

### Comparing `yalexs-3.0.1/yalexs.egg-info/PKG-INFO` & `yalexs-3.1.0/yalexs.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yalexs
-Version: 3.0.1
+Version: 3.1.0
 Summary: Python API for Yale Access (formerly August) Smart Lock and Doorbell
 Home-page: https://github.com/bdraco/yalexs
 Author: bdraco
 Author-email: nick@koston.org
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `yalexs-3.0.1/yalexs.egg-info/SOURCES.txt` & `yalexs-3.1.0/yalexs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

