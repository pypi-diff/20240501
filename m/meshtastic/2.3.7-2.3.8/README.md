# Comparing `tmp/meshtastic-2.3.7.tar.gz` & `tmp/meshtastic-2.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meshtastic-2.3.7.tar", last modified: Thu Apr 25 18:34:00 2024, max compression
+gzip compressed data, was "meshtastic-2.3.8.tar", last modified: Wed May  1 16:42:42 2024, max compression
```

## Comparing `meshtastic-2.3.7.tar` & `meshtastic-2.3.8.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:34:00.231000 meshtastic-2.3.7/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-25 18:33:54.000000 meshtastic-2.3.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-25 18:33:54.000000 meshtastic-2.3.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-04-25 18:34:00.231000 meshtastic-2.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-04-25 18:33:54.000000 meshtastic-2.3.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:34:00.231000 meshtastic-2.3.7/meshtastic/
--rw-r--r--   0 runner    (1001) docker     (127)     9091 2024-04-25 18:33:54.000000 meshtastic-2.3.7/meshtastic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    56982 2024-04-25 18:33:54.000000 meshtastic-2.3.7/meshtastic/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-04-25 18:33:54.000000 meshtastic-2.3.7/meshtastic/admin_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    25228 2024-04-25 18:33:54.000000 meshtastic-2.3.7/meshtastic/admin_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-25 18:33:54.000000 meshtastic-2.3.7/meshtastic/apponly_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-04-25 18:33:54.000000 meshtastic-2.3.7/meshtastic/apponly_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-04-25 18:33:54.000000 meshtastic-2.3.7/meshtastic/atak_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-04-25 18:33:54.000000 meshtastic-2.3.7/meshtastic/atak_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8224 2024-04-25 18:33:54.000000 meshtastic-2.3.7/meshtastic/ble_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-25 18:33:54.000000 meshtastic-2.3.7/meshtastic/cannedmessages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-25 18:33:54.000000 meshtastic-2.3.7/meshtastic/cannedmessages_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-25 18:33:54.000000 meshtastic-2.3.7/meshtastic/channel_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     9476 2024-04-25 18:33:54.000000 meshtastic-2.3.7/meshtastic/channel_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-25 18:33:54.000000 meshtastic-2.3.7/meshtastic/clientonly_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-25 18:33:54.000000 meshtastic-2.3.7/meshtastic/clientonly_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10953 2024-04-25 18:33:54.000000 meshtastic-2.3.7/meshtastic/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    66376 2024-04-25 18:33:54.000000 meshtastic-2.3.7/meshtastic/config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-04-25 18:33:54.000000 meshtastic-2.3.7/meshtastic/connection_status_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7484 2024-04-25 18:33:54.000000 meshtastic-2.3.7/meshtastic/connection_status_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-04-25 18:33:54.000000 meshtastic-2.3.7/meshtastic/deviceonly_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    14192 2024-04-25 18:33:54.000000 meshtastic-2.3.7/meshtastic/deviceonly_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-04-25 18:33:54.000000 meshtastic-2.3.7/meshtastic/localonly_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     9543 2024-04-25 18:33:54.000000 meshtastic-2.3.7/meshtastic/localonly_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    45270 2024-04-25 18:33:54.000000 meshtastic-2.3.7/meshtastic/mesh_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    15110 2024-04-25 18:33:54.000000 meshtastic-2.3.7/meshtastic/mesh_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    87037 2024-04-25 18:33:54.000000 meshtastic-2.3.7/meshtastic/mesh_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11502 2024-04-25 18:33:54.000000 meshtastic-2.3.7/meshtastic/module_config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    48852 2024-04-25 18:33:54.000000 meshtastic-2.3.7/meshtastic/module_config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-25 18:33:54.000000 meshtastic-2.3.7/meshtastic/mqtt_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-04-25 18:33:54.000000 meshtastic-2.3.7/meshtastic/mqtt_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-25 18:33:54.000000 meshtastic-2.3.7/meshtastic/mt_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-04-25 18:33:54.000000 meshtastic-2.3.7/meshtastic/nanopb_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    16031 2024-04-25 18:33:54.000000 meshtastic-2.3.7/meshtastic/nanopb_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    31935 2024-04-25 18:33:54.000000 meshtastic-2.3.7/meshtastic/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-25 18:33:54.000000 meshtastic-2.3.7/meshtastic/paxcount_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-25 18:33:54.000000 meshtastic-2.3.7/meshtastic/paxcount_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-25 18:33:54.000000 meshtastic-2.3.7/meshtastic/portnums_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    13631 2024-04-25 18:33:54.000000 meshtastic-2.3.7/meshtastic/portnums_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-04-25 18:33:54.000000 meshtastic-2.3.7/meshtastic/remote_hardware.py
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-25 18:33:54.000000 meshtastic-2.3.7/meshtastic/remote_hardware_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-04-25 18:33:54.000000 meshtastic-2.3.7/meshtastic/remote_hardware_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-25 18:33:54.000000 meshtastic-2.3.7/meshtastic/rtttl_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-25 18:33:54.000000 meshtastic-2.3.7/meshtastic/rtttl_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-04-25 18:33:54.000000 meshtastic-2.3.7/meshtastic/serial_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-04-25 18:33:54.000000 meshtastic-2.3.7/meshtastic/storeforward_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    11982 2024-04-25 18:33:54.000000 meshtastic-2.3.7/meshtastic/storeforward_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7866 2024-04-25 18:33:54.000000 meshtastic-2.3.7/meshtastic/stream_interface.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6140 2024-04-25 18:33:54.000000 meshtastic-2.3.7/meshtastic/supported_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-04-25 18:33:54.000000 meshtastic-2.3.7/meshtastic/tcp_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-04-25 18:33:54.000000 meshtastic-2.3.7/meshtastic/telemetry_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    14907 2024-04-25 18:33:54.000000 meshtastic-2.3.7/meshtastic/telemetry_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6013 2024-04-25 18:33:54.000000 meshtastic-2.3.7/meshtastic/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8653 2024-04-25 18:33:54.000000 meshtastic-2.3.7/meshtastic/tunnel.py
--rw-r--r--   0 runner    (1001) docker     (127)    21506 2024-04-25 18:33:54.000000 meshtastic-2.3.7/meshtastic/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-25 18:33:54.000000 meshtastic-2.3.7/meshtastic/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-25 18:33:54.000000 meshtastic-2.3.7/meshtastic/xmodem_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-25 18:33:54.000000 meshtastic-2.3.7/meshtastic/xmodem_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:34:00.231000 meshtastic-2.3.7/meshtastic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-04-25 18:34:00.000000 meshtastic-2.3.7/meshtastic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-25 18:34:00.000000 meshtastic-2.3.7/meshtastic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 18:34:00.000000 meshtastic-2.3.7/meshtastic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-25 18:34:00.000000 meshtastic-2.3.7/meshtastic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-25 18:34:00.000000 meshtastic-2.3.7/meshtastic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-25 18:34:00.000000 meshtastic-2.3.7/meshtastic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 18:34:00.231000 meshtastic-2.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-25 18:33:54.000000 meshtastic-2.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:42:42.605169 meshtastic-2.3.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-01 16:42:37.000000 meshtastic-2.3.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-01 16:42:37.000000 meshtastic-2.3.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-05-01 16:42:42.605169 meshtastic-2.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-05-01 16:42:37.000000 meshtastic-2.3.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:42:42.601169 meshtastic-2.3.8/meshtastic/
+-rw-r--r--   0 runner    (1001) docker     (127)     9091 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56982 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/admin_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25228 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/admin_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/apponly_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/apponly_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/atak_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/atak_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8224 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/ble_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/cannedmessages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/cannedmessages_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/channel_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9814 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/channel_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/clientonly_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/clientonly_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10953 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66376 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/connection_status_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7484 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/connection_status_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/deviceonly_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14192 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/deviceonly_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/localonly_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9543 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/localonly_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    46114 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/mesh_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15110 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/mesh_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    87037 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/mesh_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11502 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/module_config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48852 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/module_config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/mqtt_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/mqtt_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/mt_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/nanopb_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16031 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/nanopb_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    31992 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/paxcount_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/paxcount_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/portnums_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13631 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/portnums_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/remote_hardware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/remote_hardware_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/remote_hardware_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/rtttl_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/rtttl_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/serial_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/storeforward_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11982 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/storeforward_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7866 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/stream_interface.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6140 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/supported_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/tcp_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/telemetry_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14907 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/telemetry_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6013 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8653 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/tunnel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21571 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/xmodem_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-05-01 16:42:37.000000 meshtastic-2.3.8/meshtastic/xmodem_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:42:42.605169 meshtastic-2.3.8/meshtastic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-05-01 16:42:42.000000 meshtastic-2.3.8/meshtastic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-01 16:42:42.000000 meshtastic-2.3.8/meshtastic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 16:42:42.000000 meshtastic-2.3.8/meshtastic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-01 16:42:42.000000 meshtastic-2.3.8/meshtastic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-01 16:42:42.000000 meshtastic-2.3.8/meshtastic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-01 16:42:42.000000 meshtastic-2.3.8/meshtastic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 16:42:42.605169 meshtastic-2.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-01 16:42:37.000000 meshtastic-2.3.8/setup.py
```

### Comparing `meshtastic-2.3.7/LICENSE.txt` & `meshtastic-2.3.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.7/PKG-INFO` & `meshtastic-2.3.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meshtastic
-Version: 2.3.7
+Version: 2.3.8
 Summary: Python API & client shell for talking to Meshtastic devices
 Home-page: https://github.com/meshtastic/python
 Author: Meshtastic Developers
 Author-email: contact@meshtastic.org
 License: GPL-3.0-only
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 4 - Beta
```

### Comparing `meshtastic-2.3.7/README.md` & `meshtastic-2.3.8/README.md`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.7/meshtastic/__init__.py` & `meshtastic-2.3.8/meshtastic/__init__.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.7/meshtastic/__main__.py` & `meshtastic-2.3.8/meshtastic/__main__.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.7/meshtastic/admin_pb2.py` & `meshtastic-2.3.8/meshtastic/admin_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.7/meshtastic/admin_pb2.pyi` & `meshtastic-2.3.8/meshtastic/admin_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.7/meshtastic/apponly_pb2.py` & `meshtastic-2.3.8/meshtastic/apponly_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.7/meshtastic/apponly_pb2.pyi` & `meshtastic-2.3.8/meshtastic/apponly_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.7/meshtastic/atak_pb2.py` & `meshtastic-2.3.8/meshtastic/atak_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.7/meshtastic/atak_pb2.pyi` & `meshtastic-2.3.8/meshtastic/atak_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.7/meshtastic/ble_interface.py` & `meshtastic-2.3.8/meshtastic/ble_interface.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.7/meshtastic/cannedmessages_pb2.py` & `meshtastic-2.3.8/meshtastic/cannedmessages_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.7/meshtastic/cannedmessages_pb2.pyi` & `meshtastic-2.3.8/meshtastic/cannedmessages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.7/meshtastic/channel_pb2.py` & `meshtastic-2.3.8/meshtastic/channel_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,26 +9,26 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18meshtastic/channel.proto\x12\nmeshtastic\"\xb8\x01\n\x0f\x43hannelSettings\x12\x17\n\x0b\x63hannel_num\x18\x01 \x01(\rB\x02\x18\x01\x12\x0b\n\x03psk\x18\x02 \x01(\x0c\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\n\n\x02id\x18\x04 \x01(\x07\x12\x16\n\x0euplink_enabled\x18\x05 \x01(\x08\x12\x18\n\x10\x64ownlink_enabled\x18\x06 \x01(\x08\x12\x33\n\x0fmodule_settings\x18\x07 \x01(\x0b\x32\x1a.meshtastic.ModuleSettings\",\n\x0eModuleSettings\x12\x1a\n\x12position_precision\x18\x01 \x01(\r\"\xa1\x01\n\x07\x43hannel\x12\r\n\x05index\x18\x01 \x01(\x05\x12-\n\x08settings\x18\x02 \x01(\x0b\x32\x1b.meshtastic.ChannelSettings\x12&\n\x04role\x18\x03 \x01(\x0e\x32\x18.meshtastic.Channel.Role\"0\n\x04Role\x12\x0c\n\x08\x44ISABLED\x10\x00\x12\x0b\n\x07PRIMARY\x10\x01\x12\r\n\tSECONDARY\x10\x02\x42\x62\n\x13\x63om.geeksville.meshB\rChannelProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18meshtastic/channel.proto\x12\nmeshtastic\"\xb8\x01\n\x0f\x43hannelSettings\x12\x17\n\x0b\x63hannel_num\x18\x01 \x01(\rB\x02\x18\x01\x12\x0b\n\x03psk\x18\x02 \x01(\x0c\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\n\n\x02id\x18\x04 \x01(\x07\x12\x16\n\x0euplink_enabled\x18\x05 \x01(\x08\x12\x18\n\x10\x64ownlink_enabled\x18\x06 \x01(\x08\x12\x33\n\x0fmodule_settings\x18\x07 \x01(\x0b\x32\x1a.meshtastic.ModuleSettings\"E\n\x0eModuleSettings\x12\x1a\n\x12position_precision\x18\x01 \x01(\r\x12\x17\n\x0fis_client_muted\x18\x02 \x01(\x08\"\xa1\x01\n\x07\x43hannel\x12\r\n\x05index\x18\x01 \x01(\x05\x12-\n\x08settings\x18\x02 \x01(\x0b\x32\x1b.meshtastic.ChannelSettings\x12&\n\x04role\x18\x03 \x01(\x0e\x32\x18.meshtastic.Channel.Role\"0\n\x04Role\x12\x0c\n\x08\x44ISABLED\x10\x00\x12\x0b\n\x07PRIMARY\x10\x01\x12\r\n\tSECONDARY\x10\x02\x42\x62\n\x13\x63om.geeksville.meshB\rChannelProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'meshtastic.channel_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\023com.geeksville.meshB\rChannelProtosZ\"github.com/meshtastic/go/generated\252\002\024Meshtastic.Protobufs\272\002\000'
   _CHANNELSETTINGS.fields_by_name['channel_num']._options = None
   _CHANNELSETTINGS.fields_by_name['channel_num']._serialized_options = b'\030\001'
   _CHANNELSETTINGS._serialized_start=41
   _CHANNELSETTINGS._serialized_end=225
   _MODULESETTINGS._serialized_start=227
-  _MODULESETTINGS._serialized_end=271
-  _CHANNEL._serialized_start=274
-  _CHANNEL._serialized_end=435
-  _CHANNEL_ROLE._serialized_start=387
-  _CHANNEL_ROLE._serialized_end=435
+  _MODULESETTINGS._serialized_end=296
+  _CHANNEL._serialized_start=299
+  _CHANNEL._serialized_end=460
+  _CHANNEL_ROLE._serialized_start=412
+  _CHANNEL_ROLE._serialized_end=460
 # @@protoc_insertion_point(module_scope)
```

### Comparing `meshtastic-2.3.7/meshtastic/channel_pb2.pyi` & `meshtastic-2.3.8/meshtastic/channel_pb2.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -121,24 +121,31 @@
     """
     This message is specifically for modules to store per-channel configuration data.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     POSITION_PRECISION_FIELD_NUMBER: builtins.int
+    IS_CLIENT_MUTED_FIELD_NUMBER: builtins.int
     position_precision: builtins.int
     """
     Bits of precision for the location sent in position packets.
     """
+    is_client_muted: builtins.bool
+    """
+    Controls whether or not the phone / clients should mute the current channel
+    Useful for noisy public channels you don't necessarily want to disable
+    """
     def __init__(
         self,
         *,
         position_precision: builtins.int = ...,
+        is_client_muted: builtins.bool = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["position_precision", b"position_precision"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["is_client_muted", b"is_client_muted", "position_precision", b"position_precision"]) -> None: ...
 
 global___ModuleSettings = ModuleSettings
 
 @typing_extensions.final
 class Channel(google.protobuf.message.Message):
     """
     A pair of a channel number, mode and the (sharable) settings for that channel
```

### Comparing `meshtastic-2.3.7/meshtastic/clientonly_pb2.py` & `meshtastic-2.3.8/meshtastic/clientonly_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.7/meshtastic/clientonly_pb2.pyi` & `meshtastic-2.3.8/meshtastic/clientonly_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.7/meshtastic/config_pb2.py` & `meshtastic-2.3.8/meshtastic/config_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.7/meshtastic/config_pb2.pyi` & `meshtastic-2.3.8/meshtastic/config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.7/meshtastic/connection_status_pb2.py` & `meshtastic-2.3.8/meshtastic/connection_status_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.7/meshtastic/connection_status_pb2.pyi` & `meshtastic-2.3.8/meshtastic/connection_status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.7/meshtastic/deviceonly_pb2.py` & `meshtastic-2.3.8/meshtastic/deviceonly_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.7/meshtastic/deviceonly_pb2.pyi` & `meshtastic-2.3.8/meshtastic/deviceonly_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.7/meshtastic/localonly_pb2.py` & `meshtastic-2.3.8/meshtastic/localonly_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.7/meshtastic/localonly_pb2.pyi` & `meshtastic-2.3.8/meshtastic/localonly_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.7/meshtastic/mesh_interface.py` & `meshtastic-2.3.8/meshtastic/mesh_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,14 +81,15 @@
         self.currentPacketId: int = random.randint(0, 0xFFFFFFFF)
         self.nodesByNum: Optional[Dict[int, Dict]] = None
         self.configId: Optional[int] = None
         self.gotResponse: bool = False  # used in gpio read
         self.mask: Optional[int] = None  # used in gpio read and gpio watch
         self.queueStatus: Optional[mesh_pb2.QueueStatus] = None
         self.queue: collections.OrderedDict = collections.OrderedDict()
+        self._localChannels = None
 
     def close(self):
         """Shutdown this interface"""
         if self.heartbeatTimer:
             self.heartbeatTimer.cancel()
 
         self._sendDisconnect()
@@ -129,15 +130,15 @@
                     # decode the base64 value
                     addr = convert_mac_addr(val)
                     n2["user"]["macaddr"] = addr
 
                 # use id as dictionary key for correct json format in list of nodes
                 nodeid = n2["user"]["id"]
                 nodes[nodeid] = n2
-        infos = owner + myinfo + metadata + mesh + json.dumps(nodes)
+        infos = owner + myinfo + metadata + mesh + json.dumps(nodes, indent=2)
         print(infos)
         return infos
 
     def showNodes(self, includeSelf: bool=True, file=sys.stdout) -> str:  # pylint: disable=W0613
         """Show table summary of nodes in mesh"""
 
         def formatFloat(value, precision=2, unit="") -> Optional[str]:
@@ -678,14 +679,15 @@
             prefs = self.localNode.localConfig
             i = prefs.power.ls_secs / 2
             logging.debug(f"Sending heartbeat, interval {i}")
             if i != 0:
                 self.heartbeatTimer = threading.Timer(i, callback)
                 self.heartbeatTimer.start()
                 p = mesh_pb2.ToRadio()
+                p.heartbeat.CopyFrom(mesh_pb2.Heartbeat())
                 self._sendToRadio(p)
 
         callback()  # run our periodic callback now, it will make another timer if necessary
 
     def _connected(self):
         """Called by this class to tell clients we are now fully connected to a node"""
         # (because I'm lazy) _connected might be called when remote Node
@@ -701,14 +703,15 @@
             )
 
     def _startConfig(self):
         """Start device packets flowing"""
         self.myInfo = None
         self.nodes = {}  # nodes keyed by ID
         self.nodesByNum = {}  # nodes keyed by nodenum
+        self._localChannels = [] # empty until we start getting channels pushed from the device (during config)
 
         startConfig = mesh_pb2.ToRadio()
         self.configId = random.randint(0, 0xFFFFFFFF)
         startConfig.want_config_id = self.configId
         self._sendToRadio(startConfig)
 
     def _sendDisconnect(self):
@@ -782,15 +785,20 @@
         logging.error(f"Subclass must provide toradio: {toRadio}")
 
     def _handleConfigComplete(self) -> None:
         """
         Done with initial config messages, now send regular MeshPackets
         to ask for settings and channels
         """
-        self.localNode.requestChannels()
+        # This is no longer necessary because the current protocol statemachine has already proactively sent us the locally visible channels
+        # self.localNode.requestChannels()
+        self.localNode.setChannels(self._localChannels)
+
+        # the following should only be called after we have settings and channels
+        self._connected()  # Tell everyone else we are ready to go
 
     def _handleQueueStatusFromRadio(self, queueStatus) -> None:
         self.queueStatus = queueStatus
         logging.debug(
             f"TX QUEUE free {queueStatus.free} of {queueStatus.maxlen}, res = {queueStatus.res}, id = {queueStatus.mesh_packet_id:08x} "
         )
 
@@ -855,15 +863,16 @@
                 )
             )
         elif fromRadio.config_complete_id == self.configId:
             # we ignore the config_complete_id, it is unneeded for our
             # stream API fromRadio.config_complete_id
             logging.debug(f"Config complete ID {self.configId}")
             self._handleConfigComplete()
-
+        elif fromRadio.HasField("channel"):
+            self._handleChannel(fromRadio.channel)
         elif fromRadio.HasField("packet"):
             self._handlePacketFromRadio(fromRadio.packet)
 
         elif fromRadio.HasField("queueStatus"):
             self._handleQueueStatusFromRadio(fromRadio.queueStatus)
 
         elif fromRadio.rebooted:
@@ -982,14 +991,18 @@
         if nodeNum in self.nodesByNum:
             return self.nodesByNum[nodeNum]
         else:
             n = {"num": nodeNum}  # Create a minimal node db entry
             self.nodesByNum[nodeNum] = n
             return n
 
+    def _handleChannel(self, channel):
+        """During initial config the local node will proactively send all N (8) channels it knows"""
+        self._localChannels.append(channel)
+
     def _handlePacketFromRadio(self, meshPacket, hack=False):
         """Handle a MeshPacket that just arrived from the radio
 
         hack - well, since we used 'from', which is a python keyword,
                as an attribute to MeshPacket in protobufs,
                there really is no way to do something like this:
                     meshPacket = mesh_pb2.MeshPacket()
```

### Comparing `meshtastic-2.3.7/meshtastic/mesh_pb2.py` & `meshtastic-2.3.8/meshtastic/mesh_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.7/meshtastic/mesh_pb2.pyi` & `meshtastic-2.3.8/meshtastic/mesh_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.7/meshtastic/module_config_pb2.py` & `meshtastic-2.3.8/meshtastic/module_config_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.7/meshtastic/module_config_pb2.pyi` & `meshtastic-2.3.8/meshtastic/module_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.7/meshtastic/mqtt_pb2.py` & `meshtastic-2.3.8/meshtastic/mqtt_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.7/meshtastic/mqtt_pb2.pyi` & `meshtastic-2.3.8/meshtastic/mqtt_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.7/meshtastic/mt_config.py` & `meshtastic-2.3.8/meshtastic/mt_config.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.7/meshtastic/nanopb_pb2.py` & `meshtastic-2.3.8/meshtastic/nanopb_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.7/meshtastic/nanopb_pb2.pyi` & `meshtastic-2.3.8/meshtastic/nanopb_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.7/meshtastic/node.py` & `meshtastic-2.3.8/meshtastic/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,22 +60,27 @@
         if adminURL != publicURL:
             print(f"Complete URL (includes all channels): {adminURL}")
 
     def showInfo(self):
         """Show human readable description of our node"""
         prefs = ""
         if self.localConfig:
-            prefs = message_to_json(self.localConfig)
+            prefs = message_to_json(self.localConfig, multiline=True)
         print(f"Preferences: {prefs}\n")
         prefs = ""
         if self.moduleConfig:
-            prefs = message_to_json(self.moduleConfig)
+            prefs = message_to_json(self.moduleConfig, multiline=True)
         print(f"Module preferences: {prefs}\n")
         self.showChannels()
 
+    def setChannels(self, channels):
+        """Set the channels for this node"""
+        self.channels = channels
+        self._fixupChannels()
+
     def requestChannels(self):
         """Send regular MeshPackets to ask channels."""
         logging.debug(f"requestChannels for nodeNum:{self.nodeNum}")
         self.channels = None
         self.partialChannels = []  # We keep our channels in a temp array until finished
 
         self._requestChannel(0)
@@ -650,15 +655,15 @@
             onResponse = self.onAckNak
         return self._sendAdmin(p, onResponse=onResponse)
 
     def _fixupChannels(self):
         """Fixup indexes and add disabled channels as needed"""
 
         # Add extra disabled channels as needed
-        # TODO: These 2 lines seem to not do anything.
+        # This is needed because the protobufs will have index **missing** if the channel number is zero
         for index, ch in enumerate(self.channels):
             ch.index = index  # fixup indexes
 
         self._fillChannels()
 
     def _fillChannels(self):
         """Mark unused channels as disabled"""
@@ -722,17 +727,14 @@
         index = c.index
 
         if index >= 8 - 1:
             logging.debug("Finished downloading channels")
 
             self.channels = self.partialChannels
             self._fixupChannels()
-
-            # FIXME, the following should only be called after we have settings and channels
-            self.iface._connected()  # Tell everyone else we are ready to go
         else:
             self._requestChannel(index + 1)
 
     def onAckNak(self, p):
         """Informative handler for ACK/NAK responses"""
         if p["decoded"]["routing"]["errorReason"] != "NONE":
             print(
```

### Comparing `meshtastic-2.3.7/meshtastic/paxcount_pb2.py` & `meshtastic-2.3.8/meshtastic/paxcount_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.7/meshtastic/paxcount_pb2.pyi` & `meshtastic-2.3.8/meshtastic/paxcount_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.7/meshtastic/portnums_pb2.py` & `meshtastic-2.3.8/meshtastic/portnums_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.7/meshtastic/portnums_pb2.pyi` & `meshtastic-2.3.8/meshtastic/portnums_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.7/meshtastic/remote_hardware.py` & `meshtastic-2.3.8/meshtastic/remote_hardware.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.7/meshtastic/remote_hardware_pb2.py` & `meshtastic-2.3.8/meshtastic/remote_hardware_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.7/meshtastic/remote_hardware_pb2.pyi` & `meshtastic-2.3.8/meshtastic/remote_hardware_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.7/meshtastic/rtttl_pb2.py` & `meshtastic-2.3.8/meshtastic/rtttl_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.7/meshtastic/rtttl_pb2.pyi` & `meshtastic-2.3.8/meshtastic/rtttl_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.7/meshtastic/serial_interface.py` & `meshtastic-2.3.8/meshtastic/serial_interface.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.7/meshtastic/storeforward_pb2.py` & `meshtastic-2.3.8/meshtastic/storeforward_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.7/meshtastic/storeforward_pb2.pyi` & `meshtastic-2.3.8/meshtastic/storeforward_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.7/meshtastic/stream_interface.py` & `meshtastic-2.3.8/meshtastic/stream_interface.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.7/meshtastic/supported_device.py` & `meshtastic-2.3.8/meshtastic/supported_device.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.7/meshtastic/tcp_interface.py` & `meshtastic-2.3.8/meshtastic/tcp_interface.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.7/meshtastic/telemetry_pb2.py` & `meshtastic-2.3.8/meshtastic/telemetry_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.7/meshtastic/telemetry_pb2.pyi` & `meshtastic-2.3.8/meshtastic/telemetry_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.7/meshtastic/test.py` & `meshtastic-2.3.8/meshtastic/test.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.7/meshtastic/tunnel.py` & `meshtastic-2.3.8/meshtastic/tunnel.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.7/meshtastic/util.py` & `meshtastic-2.3.8/meshtastic/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -623,10 +623,12 @@
         return pypi_version
 
     if parsed_pypi_version <= parsed_act_version:
         return None
 
     return pypi_version
 
-def message_to_json(message):
-    "Return protobuf message as JSON. Always print all fields, even when not present in data."
-    return stripnl(MessageToJson(message, always_print_fields_with_no_presence=True))
+
+def message_to_json(message, multiline=False):
+    """Return protobuf message as JSON. Always print all fields, even when not present in data."""
+    json = MessageToJson(message, always_print_fields_with_no_presence=True)
+    return stripnl(json) if not multiline else json
```

### Comparing `meshtastic-2.3.7/meshtastic/xmodem_pb2.py` & `meshtastic-2.3.8/meshtastic/xmodem_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.7/meshtastic/xmodem_pb2.pyi` & `meshtastic-2.3.8/meshtastic/xmodem_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.7/meshtastic.egg-info/PKG-INFO` & `meshtastic-2.3.8/meshtastic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meshtastic
-Version: 2.3.7
+Version: 2.3.8
 Summary: Python API & client shell for talking to Meshtastic devices
 Home-page: https://github.com/meshtastic/python
 Author: Meshtastic Developers
 Author-email: contact@meshtastic.org
 License: GPL-3.0-only
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 4 - Beta
```

### Comparing `meshtastic-2.3.7/meshtastic.egg-info/SOURCES.txt` & `meshtastic-2.3.8/meshtastic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.7/setup.py` & `meshtastic-2.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 # This call to setup() does all the work
 setup(
     name="meshtastic",
-    version="2.3.7",
+    version="2.3.8",
     description="Python API & client shell for talking to Meshtastic devices",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/meshtastic/python",
     author="Meshtastic Developers",
     author_email="contact@meshtastic.org",
     license="GPL-3.0-only",
```

