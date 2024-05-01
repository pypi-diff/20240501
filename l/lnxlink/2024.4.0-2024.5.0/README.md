# Comparing `tmp/lnxlink-2024.4.0.tar.gz` & `tmp/lnxlink-2024.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lnxlink-2024.4.0.tar", last modified: Fri Mar 29 19:04:33 2024, max compression
+gzip compressed data, was "lnxlink-2024.5.0.tar", last modified: Wed May  1 15:39:44 2024, max compression
```

## Comparing `lnxlink-2024.4.0.tar` & `lnxlink-2024.5.0.tar`

### file list

```diff
@@ -1,62 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:04:33.621395 lnxlink-2024.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-03-29 19:04:29.000000 lnxlink-2024.4.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-03-29 19:04:33.621395 lnxlink-2024.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-03-29 19:04:29.000000 lnxlink-2024.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:04:33.613395 lnxlink-2024.4.0/lnxlink/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:04:29.000000 lnxlink-2024.4.0/lnxlink/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    20241 2024-03-29 19:04:29.000000 lnxlink-2024.4.0/lnxlink/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8081 2024-03-29 19:04:29.000000 lnxlink-2024.4.0/lnxlink/config_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-03-29 19:04:29.000000 lnxlink-2024.4.0/lnxlink/consts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:04:33.621395 lnxlink-2024.4.0/lnxlink/modules/
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-03-29 19:04:29.000000 lnxlink-2024.4.0/lnxlink/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-03-29 19:04:29.000000 lnxlink-2024.4.0/lnxlink/modules/audio_select.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-03-29 19:04:29.000000 lnxlink-2024.4.0/lnxlink/modules/bash.py
--rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-03-29 19:04:29.000000 lnxlink-2024.4.0/lnxlink/modules/battery.py
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-03-29 19:04:29.000000 lnxlink-2024.4.0/lnxlink/modules/boot_select.py
--rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-03-29 19:04:29.000000 lnxlink-2024.4.0/lnxlink/modules/brightness.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-03-29 19:04:29.000000 lnxlink-2024.4.0/lnxlink/modules/camera_used.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-03-29 19:04:29.000000 lnxlink-2024.4.0/lnxlink/modules/cpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-03-29 19:04:29.000000 lnxlink-2024.4.0/lnxlink/modules/disk_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-03-29 19:04:29.000000 lnxlink-2024.4.0/lnxlink/modules/display_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-03-29 19:04:29.000000 lnxlink-2024.4.0/lnxlink/modules/fullscreen.py
--rw-r--r--   0 runner    (1001) docker     (127)     5234 2024-03-29 19:04:29.000000 lnxlink-2024.4.0/lnxlink/modules/gpio.py
--rw-r--r--   0 runner    (1001) docker     (127)     4177 2024-03-29 19:04:29.000000 lnxlink-2024.4.0/lnxlink/modules/gpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-03-29 19:04:29.000000 lnxlink-2024.4.0/lnxlink/modules/idle.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-03-29 19:04:29.000000 lnxlink-2024.4.0/lnxlink/modules/inference_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-03-29 19:04:29.000000 lnxlink-2024.4.0/lnxlink/modules/keep_alive.py
--rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-03-29 19:04:29.000000 lnxlink-2024.4.0/lnxlink/modules/keyboard_hotkeys.py
--rw-r--r--   0 runner    (1001) docker     (127)     8904 2024-03-29 19:04:29.000000 lnxlink-2024.4.0/lnxlink/modules/media.py
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-03-29 19:04:29.000000 lnxlink-2024.4.0/lnxlink/modules/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-03-29 19:04:29.000000 lnxlink-2024.4.0/lnxlink/modules/microphone_used.py
--rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-03-29 19:04:29.000000 lnxlink-2024.4.0/lnxlink/modules/mouse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-03-29 19:04:29.000000 lnxlink-2024.4.0/lnxlink/modules/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-03-29 19:04:29.000000 lnxlink-2024.4.0/lnxlink/modules/notify.py
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-03-29 19:04:29.000000 lnxlink-2024.4.0/lnxlink/modules/power_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-03-29 19:04:29.000000 lnxlink-2024.4.0/lnxlink/modules/required_restart.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-03-29 19:04:29.000000 lnxlink-2024.4.0/lnxlink/modules/restart.py
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-03-29 19:04:29.000000 lnxlink-2024.4.0/lnxlink/modules/screen_onoff.py
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-03-29 19:04:29.000000 lnxlink-2024.4.0/lnxlink/modules/screenshot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:04:33.621395 lnxlink-2024.4.0/lnxlink/modules/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-03-29 19:04:29.000000 lnxlink-2024.4.0/lnxlink/modules/scripts/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-03-29 19:04:29.000000 lnxlink-2024.4.0/lnxlink/modules/send_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-03-29 19:04:29.000000 lnxlink-2024.4.0/lnxlink/modules/shutdown.py
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-03-29 19:04:29.000000 lnxlink-2024.4.0/lnxlink/modules/speech_recognition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-03-29 19:04:29.000000 lnxlink-2024.4.0/lnxlink/modules/statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-03-29 19:04:29.000000 lnxlink-2024.4.0/lnxlink/modules/suspend.py
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-03-29 19:04:29.000000 lnxlink-2024.4.0/lnxlink/modules/sys_updates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-03-29 19:04:29.000000 lnxlink-2024.4.0/lnxlink/modules/systemd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-03-29 19:04:29.000000 lnxlink-2024.4.0/lnxlink/modules/temperature.py
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-03-29 19:04:29.000000 lnxlink-2024.4.0/lnxlink/modules/update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-03-29 19:04:29.000000 lnxlink-2024.4.0/lnxlink/modules/webcam.py
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-03-29 19:04:29.000000 lnxlink-2024.4.0/lnxlink/modules/wifi.py
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-03-29 19:04:29.000000 lnxlink-2024.4.0/lnxlink/modules/xdg_open.py
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-03-29 19:04:29.000000 lnxlink-2024.4.0/lnxlink/system_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:04:33.613395 lnxlink-2024.4.0/lnxlink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-03-29 19:04:33.000000 lnxlink-2024.4.0/lnxlink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-03-29 19:04:33.000000 lnxlink-2024.4.0/lnxlink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 19:04:33.000000 lnxlink-2024.4.0/lnxlink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-29 19:04:33.000000 lnxlink-2024.4.0/lnxlink.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-29 19:04:33.000000 lnxlink-2024.4.0/lnxlink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-29 19:04:33.000000 lnxlink-2024.4.0/lnxlink.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      968 2024-03-29 19:04:29.000000 lnxlink-2024.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-29 19:04:33.625395 lnxlink-2024.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:39:44.268826 lnxlink-2024.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-05-01 15:39:44.268826 lnxlink-2024.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:39:44.260826 lnxlink-2024.5.0/lnxlink/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20496 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8081 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/config_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/consts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:39:44.268826 lnxlink-2024.5.0/lnxlink/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/active_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/audio_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/bash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/battery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/boot_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/brightness.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/camera_used.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/disk_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/display_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/fullscreen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5234 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/gpio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/idle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/inference_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/keep_alive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/keyboard_hotkeys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8904 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/microphone_used.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/mouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/notify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/power_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/required_restart.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/restart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/screen_onoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/screenshot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:39:44.268826 lnxlink-2024.5.0/lnxlink/modules/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/scripts/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/send_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/shutdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/speaker_used.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/speech_recognition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/suspend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/sys_updates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/systemd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/temperature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/webcam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/wifi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/modules/xdg_open.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/lnxlink/system_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:39:44.264826 lnxlink-2024.5.0/lnxlink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-05-01 15:39:44.000000 lnxlink-2024.5.0/lnxlink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-01 15:39:44.000000 lnxlink-2024.5.0/lnxlink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 15:39:44.000000 lnxlink-2024.5.0/lnxlink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-01 15:39:44.000000 lnxlink-2024.5.0/lnxlink.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-01 15:39:44.000000 lnxlink-2024.5.0/lnxlink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-01 15:39:44.000000 lnxlink-2024.5.0/lnxlink.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      943 2024-05-01 15:39:39.000000 lnxlink-2024.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-01 15:39:44.268826 lnxlink-2024.5.0/setup.cfg
```

### Comparing `lnxlink-2024.4.0/LICENSE.md` & `lnxlink-2024.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lnxlink-2024.4.0/PKG-INFO` & `lnxlink-2024.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lnxlink
-Version: 2024.4.0
+Version: 2024.5.0
 Summary: Internet Of Things (IOT) integration with Linux using MQTT
 Home-page: https://bkbilly.github.io/lnxlink
 Author-email: bkbilly <bkbilly@hotmail.com>
 Project-URL: Source Code, https://github.com/bkbilly/lnxlink
 Project-URL: Documentation, https://bkbilly.gitbook.io/lnxlink
 Keywords: lnxlink
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lnxlink-2024.4.0/README.md` & `lnxlink-2024.5.0/README.md`

 * *Files identical despite different names*

### Comparing `lnxlink-2024.4.0/lnxlink/__main__.py` & `lnxlink-2024.5.0/lnxlink/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,14 +191,21 @@
                 ca_certs=ca_certs,
                 certfile=certfile,
                 keyfile=keyfile,
                 cert_reqs=cert_reqs,
             )
             if ca_certs is None:
                 self.client.tls_insecure_set(True)
+        if self.config["mqtt"]["lwt"]["enabled"]:
+            self.client.will_set(
+                f"{self.pref_topic}/lwt",
+                payload="OFF",
+                qos=self.config["mqtt"]["lwt"]["qos"],
+                retain=True,
+            )
         try:
             self.client.connect(
                 self.config["mqtt"]["server"], self.config["mqtt"]["port"], 60
             )
         except ssl.SSLCertVerificationError:
             logger.info("TLS not verified, using insecure connection instead")
             self.client.tls_insecure_set(True)
```

### Comparing `lnxlink-2024.4.0/lnxlink/config_setup.py` & `lnxlink-2024.5.0/lnxlink/config_setup.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2024.4.0/lnxlink/consts.py` & `lnxlink-2024.5.0/lnxlink/consts.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 SERVICEHEADLESS = """[Unit]
 Description=LNXlink
 After=network-online.target
 
 [Service]
 Type=simple
 Restart=always
+RestartSec=5
 User=root
 
 ExecStart={exec_cmd}
 
 [Install]
 WantedBy=default.target
 """
@@ -19,14 +20,15 @@
 Description=LNXlink
 After=network-online.target multi-user.target graphical.target
 PartOf=graphical-session.target
 
 [Service]
 Type=simple
 Restart=always
+RestartSec=5
 
 ExecStart={exec_cmd}
 
 [Install]
 WantedBy=default.target
 """
```

### Comparing `lnxlink-2024.4.0/lnxlink/modules/__init__.py` & `lnxlink-2024.5.0/lnxlink/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2024.4.0/lnxlink/modules/audio_select.py` & `lnxlink-2024.5.0/lnxlink/modules/audio_select.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2024.4.0/lnxlink/modules/bash.py` & `lnxlink-2024.5.0/lnxlink/modules/bash.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2024.4.0/lnxlink/modules/battery.py` & `lnxlink-2024.5.0/lnxlink/modules/battery.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2024.4.0/lnxlink/modules/boot_select.py` & `lnxlink-2024.5.0/lnxlink/modules/boot_select.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2024.4.0/lnxlink/modules/brightness.py` & `lnxlink-2024.5.0/lnxlink/modules/brightness.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2024.4.0/lnxlink/modules/camera_used.py` & `lnxlink-2024.5.0/lnxlink/modules/camera_used.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2024.4.0/lnxlink/modules/cpu.py` & `lnxlink-2024.5.0/lnxlink/modules/cpu.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2024.4.0/lnxlink/modules/disk_usage.py` & `lnxlink-2024.5.0/lnxlink/modules/disk_usage.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,16 +42,16 @@
             self.disks[disk_name]["attributes"]["connected"] = False
             self.disks[disk_name]["percent"] = None
         self.disks = disks
         if len(mounted) > 0:
             self.lnxlink.setup_discovery()
         return self.disks
 
-    def _bytetomb(self, byte):
-        return round(byte / 1024 / 1024, 0)
+    def _bytetogb(self, byte):
+        return round(byte / 1024 / 1024 / 1024, 0)
 
     def _get_disks(self):
         """Get a list of all disks"""
         disks = {}
         disk_includes = (
             self.lnxlink.config["settings"]
             .get("disk_usage", [])
@@ -81,17 +81,15 @@
 
             try:
                 disk_stats = psutil.disk_usage(disk.mountpoint)
                 device = disk.device.replace("/", "_").strip("_")
                 disks[device] = {}
                 disks[device]["percent"] = disk_stats.percent
                 disks[device]["attributes"] = {}
-                disks[device]["attributes"]["total"] = self._bytetomb(disk_stats.total)
-                disks[device]["attributes"]["used"] = self._bytetomb(disk_stats.used)
-                disks[device]["attributes"]["free"] = self._bytetomb(disk_stats.free)
+                disks[device]["attributes"]["total"] = self._bytetogb(disk_stats.total)
                 disks[device]["attributes"]["connected"] = True
                 disks[device]["attributes"]["mountpoint"] = disk.mountpoint
             except Exception as err:
                 logger.error(
                     "Error with disk usage [fstype: %s, device: %s, mountpoint: %s]: %s",
                     disk.fstype,
                     disk.device,
```

### Comparing `lnxlink-2024.4.0/lnxlink/modules/display_env.py` & `lnxlink-2024.5.0/lnxlink/modules/display_env.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2024.4.0/lnxlink/modules/fullscreen.py` & `lnxlink-2024.5.0/lnxlink/modules/fullscreen.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2024.4.0/lnxlink/modules/gpio.py` & `lnxlink-2024.5.0/lnxlink/modules/gpio.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2024.4.0/lnxlink/modules/gpu.py` & `lnxlink-2024.5.0/lnxlink/modules/gpu.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,18 +50,18 @@
             }
         for gpu_id in range(self.gpu_ids["nvidia"]):
             nvidia_gpu = list(self.lib["nvidia"].get_gpus())[gpu_id]
             gpu_util = nvidia_gpu.gpu_util
             gpu_util = self._older_gpu_load(gpu_id, gpu_util)
             gpus[f"nvidia_{gpu_id}"] = {
                 "load": gpu_util,
+                "memory": round(nvidia_gpu.mem_util, 0),
+                "temperature": nvidia_gpu.temperature,
                 "attributes": {
                     "Name": nvidia_gpu.name,
-                    "Memory usage": round(nvidia_gpu.mem_util, 0),
-                    "Temperature": nvidia_gpu.temperature,
                 },
             }
         return gpus
 
     def _older_gpu_load(self, gpu_id, gpu_util):
         """For older GPUs, use nvidia-settings to get gpu usage"""
         if math.isnan(gpu_util):
@@ -91,17 +91,18 @@
                 "unit": "%",
                 "state_class": "measurement",
                 "value_template": f"{{{{ value_json.amd_{gpu_id}.load }}}}",
                 "attributes_template": f"{{{{ value_json.amd_{gpu_id}.attributes | tojson }}}}",
                 "enabled": True,
             }
         for gpu_id in range(self.gpu_ids["nvidia"]):
-            discovery_info[f"GPU NVIDIA {gpu_id}"] = {
-                "type": "sensor",
-                "icon": "mdi:expansion-card-variant",
-                "unit": "%",
-                "state_class": "measurement",
-                "value_template": f"{{{{ value_json.nvidia_{gpu_id}.load }}}}",
-                "attributes_template": f"{{{{ value_json.nvidia_{gpu_id}.attributes | tojson }}}}",
-                "enabled": True,
-            }
+            for expose, unit in (("load", "%"), ("memory", "%"), ("temperature", "°C")):
+                discovery_info[f"GPU NVIDIA {gpu_id} {expose}"] = {
+                    "type": "sensor",
+                    "icon": "mdi:expansion-card-variant",
+                    "unit": unit,
+                    "state_class": "measurement",
+                    "value_template": f"{{{{ value_json.nvidia_{gpu_id}.{expose} }}}}",
+                    "attributes_template": f"{{{{ value_json.nvidia_{gpu_id}.attributes | tojson }}}}",
+                    "enabled": True,
+                }
         return discovery_info
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `lnxlink-2024.4.0/lnxlink/modules/idle.py` & `lnxlink-2024.5.0/lnxlink/modules/idle.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2024.4.0/lnxlink/modules/inference_time.py` & `lnxlink-2024.5.0/lnxlink/modules/inference_time.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2024.4.0/lnxlink/modules/keep_alive.py` & `lnxlink-2024.5.0/lnxlink/modules/keep_alive.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2024.4.0/lnxlink/modules/keyboard_hotkeys.py` & `lnxlink-2024.5.0/lnxlink/modules/keyboard_hotkeys.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2024.4.0/lnxlink/modules/media.py` & `lnxlink-2024.5.0/lnxlink/modules/media.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2024.4.0/lnxlink/modules/memory.py` & `lnxlink-2024.5.0/lnxlink/modules/memory.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2024.4.0/lnxlink/modules/microphone_used.py` & `lnxlink-2024.5.0/lnxlink/modules/microphone_used.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2024.4.0/lnxlink/modules/mouse.py` & `lnxlink-2024.5.0/lnxlink/modules/mouse.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,14 +19,18 @@
         self.movement = [0, 0]
         if which("xdotool") is None:
             raise SystemError("System command 'xdotool' not found")
 
     def exposed_controls(self):
         """Exposes to home assistant"""
         return {
+            "Mouse Coordinates": {
+                "type": "text",
+                "icon": "mdi:mouse-variant",
+            },
             "Mouse Left": {
                 "type": "button",
                 "icon": "mdi:gamepad-circle-left",
             },
             "Mouse Right": {
                 "type": "button",
                 "icon": "mdi:gamepad-circle-right",
@@ -37,30 +41,36 @@
             },
             "Mouse Down": {
                 "type": "button",
                 "icon": "mdi:gamepad-circle-down",
             },
             "Mouse Click": {
                 "type": "button",
-                "icon": "mdi:cursor-default-click",
+                "icon": "mdi:mouse-left-click",
             },
             "Mouse Click Right": {
                 "type": "button",
-                "icon": "mdi:cursor-default",
+                "icon": "mdi:mouse-right-click",
             },
         }
 
     def start_control(self, topic, data):
         """Control system"""
         if os.environ.get("DISPLAY") is None:
             if self.lnxlink.display is not None:
                 os.environ["DISPLAY"] = self.lnxlink.display
                 logger.info("Initializing empty DISPLAY environment variable")
 
-        if topic[1] == "mouse_left":
+        if topic[1] == "mouse_coordinates":
+            if "," in data:
+                coords = data.replace(" ", "").split(",")
+            elif " " in data:
+                coords = data.split(" ")
+            syscommand(f"xdotool mousemove {coords[0]} {coords[1]}")
+        elif topic[1] == "mouse_left":
             self._move([-1, 0])
         elif topic[1] == "mouse_right":
             self._move([1, 0])
         elif topic[1] == "mouse_up":
             self._move([0, -1])
         elif topic[1] == "mouse_down":
             self._move([0, 1])
```

### Comparing `lnxlink-2024.4.0/lnxlink/modules/network.py` & `lnxlink-2024.5.0/lnxlink/modules/network.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2024.4.0/lnxlink/modules/notify.py` & `lnxlink-2024.5.0/lnxlink/modules/notify.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2024.4.0/lnxlink/modules/power_profile.py` & `lnxlink-2024.5.0/lnxlink/modules/power_profile.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2024.4.0/lnxlink/modules/required_restart.py` & `lnxlink-2024.5.0/lnxlink/modules/required_restart.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2024.4.0/lnxlink/modules/restart.py` & `lnxlink-2024.5.0/lnxlink/modules/restart.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2024.4.0/lnxlink/modules/screen_onoff.py` & `lnxlink-2024.5.0/lnxlink/modules/screen_onoff.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2024.4.0/lnxlink/modules/screenshot.py` & `lnxlink-2024.5.0/lnxlink/modules/screenshot.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2024.4.0/lnxlink/modules/scripts/helpers.py` & `lnxlink-2024.5.0/lnxlink/modules/scripts/helpers.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2024.4.0/lnxlink/modules/send_keys.py` & `lnxlink-2024.5.0/lnxlink/modules/send_keys.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2024.4.0/lnxlink/modules/shutdown.py` & `lnxlink-2024.5.0/lnxlink/modules/shutdown.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2024.4.0/lnxlink/modules/speech_recognition.py` & `lnxlink-2024.5.0/lnxlink/modules/speech_recognition.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2024.4.0/lnxlink/modules/statistics.py` & `lnxlink-2024.5.0/lnxlink/modules/statistics.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2024.4.0/lnxlink/modules/suspend.py` & `lnxlink-2024.5.0/lnxlink/modules/suspend.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2024.4.0/lnxlink/modules/sys_updates.py` & `lnxlink-2024.5.0/lnxlink/modules/sys_updates.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2024.4.0/lnxlink/modules/systemd.py` & `lnxlink-2024.5.0/lnxlink/modules/systemd.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2024.4.0/lnxlink/modules/temperature.py` & `lnxlink-2024.5.0/lnxlink/modules/temperature.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2024.4.0/lnxlink/modules/update.py` & `lnxlink-2024.5.0/lnxlink/modules/update.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2024.4.0/lnxlink/modules/webcam.py` & `lnxlink-2024.5.0/lnxlink/modules/webcam.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2024.4.0/lnxlink/modules/wifi.py` & `lnxlink-2024.5.0/lnxlink/modules/wifi.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2024.4.0/lnxlink/modules/xdg_open.py` & `lnxlink-2024.5.0/lnxlink/modules/xdg_open.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2024.4.0/lnxlink/system_monitor.py` & `lnxlink-2024.5.0/lnxlink/system_monitor.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2024.4.0/lnxlink.egg-info/PKG-INFO` & `lnxlink-2024.5.0/lnxlink.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lnxlink
-Version: 2024.4.0
+Version: 2024.5.0
 Summary: Internet Of Things (IOT) integration with Linux using MQTT
 Home-page: https://bkbilly.github.io/lnxlink
 Author-email: bkbilly <bkbilly@hotmail.com>
 Project-URL: Source Code, https://github.com/bkbilly/lnxlink
 Project-URL: Documentation, https://bkbilly.gitbook.io/lnxlink
 Keywords: lnxlink
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lnxlink-2024.4.0/lnxlink.egg-info/SOURCES.txt` & `lnxlink-2024.5.0/lnxlink.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 lnxlink.egg-info/PKG-INFO
 lnxlink.egg-info/SOURCES.txt
 lnxlink.egg-info/dependency_links.txt
 lnxlink.egg-info/entry_points.txt
 lnxlink.egg-info/requires.txt
 lnxlink.egg-info/top_level.txt
 lnxlink/modules/__init__.py
+lnxlink/modules/active_window.py
 lnxlink/modules/audio_select.py
 lnxlink/modules/bash.py
 lnxlink/modules/battery.py
 lnxlink/modules/boot_select.py
 lnxlink/modules/brightness.py
 lnxlink/modules/camera_used.py
 lnxlink/modules/cpu.py
@@ -39,14 +40,15 @@
 lnxlink/modules/power_profile.py
 lnxlink/modules/required_restart.py
 lnxlink/modules/restart.py
 lnxlink/modules/screen_onoff.py
 lnxlink/modules/screenshot.py
 lnxlink/modules/send_keys.py
 lnxlink/modules/shutdown.py
+lnxlink/modules/speaker_used.py
 lnxlink/modules/speech_recognition.py
 lnxlink/modules/statistics.py
 lnxlink/modules/suspend.py
 lnxlink/modules/sys_updates.py
 lnxlink/modules/systemd.py
 lnxlink/modules/temperature.py
 lnxlink/modules/update.py
```

### Comparing `lnxlink-2024.4.0/pyproject.toml` & `lnxlink-2024.5.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=68.0.0", "wheel~=0.40.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name              = "lnxlink"
-version           = "2024.4.0"
+version           = "2024.5.0"
 description       = "Internet Of Things (IOT) integration with Linux using MQTT"
 readme            = "README.md"
 keywords          = ["lnxlink"]
 requires-python   = ">=3.7.0"
 authors     = [
     {name="bkbilly", email="bkbilly@hotmail.com"}
 ]
@@ -18,15 +18,14 @@
     "Operating System :: Unix",
 ]
 dependencies = [
     "distro>=1.7.0",
     "PyYAML>=5.3.1",
     "paho-mqtt>=1.5.1",
     "requests>=2.28.1",
-    "pyOpenSSL>=22.1.0",
     "jc>=1.23.0",
     "psutil>=5.8.0"
 ]
 
 
 [project.urls]
 "Source Code" = "https://github.com/bkbilly/lnxlink"
```

