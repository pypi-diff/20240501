# Comparing `tmp/parallax_app-0.37.1.tar.gz` & `tmp/parallax_app-0.37.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parallax_app-0.37.1.tar", last modified: Fri Apr 26 19:23:07 2024, max compression
+gzip compressed data, was "parallax_app-0.37.5.tar", last modified: Wed May  1 18:25:06 2024, max compression
```

## Comparing `parallax_app-0.37.1.tar` & `parallax_app-0.37.5.tar`

### file list

```diff
@@ -1,83 +1,87 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 19:23:07.389256 parallax_app-0.37.1/
--rw-rw-rw-   0        0        0      345 2024-04-26 18:57:43.000000 parallax_app-0.37.1/.gitignore
--rw-rw-rw-   0        0        0      284 2024-04-26 18:57:43.000000 parallax_app-0.37.1/.readthedocs.yaml
--rw-rw-rw-   0        0        0     1113 2024-04-26 18:57:43.000000 parallax_app-0.37.1/LICENSE
--rw-rw-rw-   0        0        0     3081 2024-04-26 19:23:07.388255 parallax_app-0.37.1/PKG-INFO
--rw-rw-rw-   0        0        0     1892 2024-04-26 18:57:43.000000 parallax_app-0.37.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-26 19:23:07.264814 parallax_app-0.37.1/docs/
--rw-rw-rw-   0        0        0      654 2024-04-26 18:57:43.000000 parallax_app-0.37.1/docs/Makefile
--rw-rw-rw-   0        0        0     1606 2024-04-26 18:57:43.000000 parallax_app-0.37.1/docs/ReadMe.rst
--rw-rw-rw-   0        0        0     1110 2024-04-26 18:57:43.000000 parallax_app-0.37.1/docs/conf.py
--rw-rw-rw-   0        0        0      481 2024-04-26 18:57:43.000000 parallax_app-0.37.1/docs/index.rst
--rwxrwxrwx   0        0        0      800 2024-04-26 18:57:43.000000 parallax_app-0.37.1/docs/make.bat
--rw-rw-rw-   0        0        0       92 2024-04-26 18:57:43.000000 parallax_app-0.37.1/docs/modules.rst
--rw-rw-rw-   0        0        0     3826 2024-04-26 18:57:43.000000 parallax_app-0.37.1/docs/parallax.rst
--rw-rw-rw-   0        0        0       26 2024-04-26 18:57:43.000000 parallax_app-0.37.1/docs/requirements.txt
-drwxrwxrwx   0        0        0        0 2024-04-26 19:23:07.296815 parallax_app-0.37.1/img/
--rw-rw-rw-   0        0        0     4622 2024-04-26 18:57:43.000000 parallax_app-0.37.1/img/arrow-right.png
--rw-rw-rw-   0        0        0     1257 2024-04-26 18:57:43.000000 parallax_app-0.37.1/img/gear.png
--rw-rw-rw-   0        0        0     1145 2024-04-26 18:57:43.000000 parallax_app-0.37.1/img/recordingButton.png
--rw-rw-rw-   0        0        0    28195 2024-04-26 18:57:43.000000 parallax_app-0.37.1/img/sextant.png
--rw-rw-rw-   0        0        0     7808 2024-04-26 18:57:43.000000 parallax_app-0.37.1/img/snapshotButton_white.png
--rw-rw-rw-   0        0        0    11773 2024-04-26 18:57:43.000000 parallax_app-0.37.1/img/stop-sign.png
--rw-rw-rw-   0        0        0    22337 2024-04-26 18:57:43.000000 parallax_app-0.37.1/img/target.png
-drwxrwxrwx   0        0        0        0 2024-04-26 19:23:07.317207 parallax_app-0.37.1/parallax/
--rw-rw-rw-   0        0        0      137 2024-04-26 18:57:43.000000 parallax_app-0.37.1/parallax/__init__.py
--rw-rw-rw-   0        0        0     2323 2024-04-26 18:57:43.000000 parallax_app-0.37.1/parallax/__main__.py
--rw-rw-rw-   0        0        0    20640 2024-04-26 18:57:43.000000 parallax_app-0.37.1/parallax/calibration_camera.py
--rw-rw-rw-   0        0        0    28521 2024-04-26 18:57:43.000000 parallax_app-0.37.1/parallax/camera.py
--rw-rw-rw-   0        0        0    11558 2024-04-26 18:57:43.000000 parallax_app-0.37.1/parallax/curr_bg_cmp_processor.py
--rw-rw-rw-   0        0        0     9100 2024-04-26 18:57:43.000000 parallax_app-0.37.1/parallax/curr_prev_cmp_processor.py
--rw-rw-rw-   0        0        0    33169 2024-04-26 18:57:43.000000 parallax_app-0.37.1/parallax/main_window_wip.py
--rw-rw-rw-   0        0        0     4852 2024-04-26 18:57:43.000000 parallax_app-0.37.1/parallax/mask_generator.py
--rw-rw-rw-   0        0        0     5288 2024-04-26 18:57:43.000000 parallax_app-0.37.1/parallax/model.py
--rw-rw-rw-   0        0        0     3747 2024-04-26 18:57:43.000000 parallax_app-0.37.1/parallax/no_filter.py
--rw-rw-rw-   0        0        0    13008 2024-04-26 18:57:43.000000 parallax_app-0.37.1/parallax/probe_calibration.py
--rw-rw-rw-   0        0        0    12242 2024-04-26 18:57:43.000000 parallax_app-0.37.1/parallax/probe_detect_manager.py
--rw-rw-rw-   0        0        0    18723 2024-04-26 18:57:43.000000 parallax_app-0.37.1/parallax/probe_detector.py
--rw-rw-rw-   0        0        0     6451 2024-04-26 18:57:43.000000 parallax_app-0.37.1/parallax/probe_fine_tip_detector.py
--rw-rw-rw-   0        0        0     4681 2024-04-26 18:57:43.000000 parallax_app-0.37.1/parallax/recording_manager.py
--rw-rw-rw-   0        0        0    11329 2024-04-26 18:57:43.000000 parallax_app-0.37.1/parallax/reticle_detect_manager.py
--rw-rw-rw-   0        0        0    22539 2024-04-26 18:57:43.000000 parallax_app-0.37.1/parallax/reticle_detection.py
--rw-rw-rw-   0        0        0     6712 2024-04-26 18:57:43.000000 parallax_app-0.37.1/parallax/reticle_detection_coords_interests.py
--rw-rw-rw-   0        0        0    12601 2024-04-26 18:57:43.000000 parallax_app-0.37.1/parallax/screen_widget.py
--rw-rw-rw-   0        0        0    18015 2024-04-26 18:57:43.000000 parallax_app-0.37.1/parallax/stage_listener.py
--rw-rw-rw-   0        0        0     4334 2024-04-26 18:57:43.000000 parallax_app-0.37.1/parallax/stage_ui.py
--rw-rw-rw-   0        0        0    25986 2024-04-26 18:57:43.000000 parallax_app-0.37.1/parallax/stage_widget.py
--rw-rw-rw-   0        0        0     6843 2024-04-26 18:57:43.000000 parallax_app-0.37.1/parallax/user_setting_manager.py
--rw-rw-rw-   0        0        0     3364 2024-04-26 18:57:43.000000 parallax_app-0.37.1/parallax/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-26 19:23:07.386256 parallax_app-0.37.1/parallax_app.egg-info/
--rw-rw-rw-   0        0        0     3081 2024-04-26 19:23:07.000000 parallax_app-0.37.1/parallax_app.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1774 2024-04-26 19:23:07.000000 parallax_app-0.37.1/parallax_app.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 19:23:07.000000 parallax_app-0.37.1/parallax_app.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      234 2024-04-26 19:23:07.000000 parallax_app-0.37.1/parallax_app.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-26 19:23:07.000000 parallax_app-0.37.1/parallax_app.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1753 2024-04-26 18:57:43.000000 parallax_app-0.37.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-26 19:23:07.389256 parallax_app-0.37.1/setup.cfg
--rw-rw-rw-   0        0        0      216 2024-04-26 18:57:43.000000 parallax_app-0.37.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-26 19:23:07.344233 parallax_app-0.37.1/tests/
--rw-rw-rw-   0        0        0      479 2024-04-26 18:57:43.000000 parallax_app-0.37.1/tests/test_camera.py
--rw-rw-rw-   0        0        0      405 2024-04-26 18:57:43.000000 parallax_app-0.37.1/tests/test_model.py
--rw-rw-rw-   0        0        0     1579 2024-04-26 18:57:43.000000 parallax_app-0.37.1/tests/test_screen_widget.py
-drwxrwxrwx   0        0        0        0 2024-04-26 19:23:07.355255 parallax_app-0.37.1/ui/
--rw-rw-rw-   0        0        0   192973 2024-04-26 18:57:43.000000 parallax_app-0.37.1/ui/ParallaxReadME.JPG
-drwxrwxrwx   0        0        0        0 2024-04-26 19:23:07.355255 parallax_app-0.37.1/ui/font/
--rw-rw-rw-   0        0        0   259308 2024-04-26 18:57:43.000000 parallax_app-0.37.1/ui/font/FiraCode-VariableFont_wght.ttf
--rw-rw-rw-   0        0        0     9977 2024-04-26 18:57:43.000000 parallax_app-0.37.1/ui/mainWindow.ui
--rw-rw-rw-   0        0        0     4500 2024-04-26 18:57:43.000000 parallax_app-0.37.1/ui/probe_calib.ui
-drwxrwxrwx   0        0        0        0 2024-04-26 19:23:07.385255 parallax_app-0.37.1/ui/resources/
--rw-rw-rw-   0        0        0     4622 2024-04-26 18:57:43.000000 parallax_app-0.37.1/ui/resources/arrow-right.png
--rw-rw-rw-   0        0        0      934 2024-04-26 18:57:43.000000 parallax_app-0.37.1/ui/resources/check.png
--rw-rw-rw-   0        0        0     1257 2024-04-26 18:57:43.000000 parallax_app-0.37.1/ui/resources/gear.png
--rw-rw-rw-   0        0        0     4794 2024-04-26 18:57:43.000000 parallax_app-0.37.1/ui/resources/recordingButton.png
--rw-rw-rw-   0        0        0     4781 2024-04-26 18:57:43.000000 parallax_app-0.37.1/ui/resources/recordingButton_disabled.png
--rw-rw-rw-   0        0        0    28195 2024-04-26 18:57:43.000000 parallax_app-0.37.1/ui/resources/sextant.png
--rw-rw-rw-   0        0        0    13098 2024-04-26 18:57:43.000000 parallax_app-0.37.1/ui/resources/snapshotButton_disabled.png
--rw-rw-rw-   0        0        0     8144 2024-04-26 18:57:43.000000 parallax_app-0.37.1/ui/resources/snapshotButton_green.png
--rw-rw-rw-   0        0        0    15545 2024-04-26 18:57:43.000000 parallax_app-0.37.1/ui/resources/snapshotButton_white.png
--rw-rw-rw-   0        0        0    11773 2024-04-26 18:57:43.000000 parallax_app-0.37.1/ui/resources/stop-sign.png
--rw-rw-rw-   0        0        0    22337 2024-04-26 18:57:43.000000 parallax_app-0.37.1/ui/resources/target.png
--rw-rw-rw-   0        0        0      436 2024-04-26 18:57:43.000000 parallax_app-0.37.1/ui/resources/x.png
--rw-rw-rw-   0        0        0     4019 2024-04-26 18:57:43.000000 parallax_app-0.37.1/ui/reticle_calib.ui
--rw-rw-rw-   0        0        0    10881 2024-04-26 18:57:43.000000 parallax_app-0.37.1/ui/settingPopUpMenu.ui
--rw-rw-rw-   0        0        0    10735 2024-04-26 18:57:43.000000 parallax_app-0.37.1/ui/stage_info.ui
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:25:06.688980 parallax_app-0.37.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:25:06.672980 parallax_app-0.37.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:25:06.676980 parallax_app-0.37.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-01 18:24:24.000000 parallax_app-0.37.5/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-01 18:24:24.000000 parallax_app-0.37.5/.github/workflows/tag_and_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-01 18:24:24.000000 parallax_app-0.37.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-01 18:24:24.000000 parallax_app-0.37.5/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-01 18:24:24.000000 parallax_app-0.37.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-05-01 18:25:06.688980 parallax_app-0.37.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-05-01 18:24:24.000000 parallax_app-0.37.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:25:06.676980 parallax_app-0.37.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-01 18:24:24.000000 parallax_app-0.37.5/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-01 18:24:24.000000 parallax_app-0.37.5/docs/ReadMe.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-01 18:24:24.000000 parallax_app-0.37.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-01 18:24:24.000000 parallax_app-0.37.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-01 18:24:24.000000 parallax_app-0.37.5/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-01 18:24:24.000000 parallax_app-0.37.5/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-05-01 18:24:24.000000 parallax_app-0.37.5/docs/parallax.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-01 18:24:24.000000 parallax_app-0.37.5/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:25:06.680980 parallax_app-0.37.5/img/
+-rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-05-01 18:24:24.000000 parallax_app-0.37.5/img/arrow-right.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-01 18:24:24.000000 parallax_app-0.37.5/img/gear.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-01 18:24:24.000000 parallax_app-0.37.5/img/recordingButton.png
+-rw-r--r--   0 runner    (1001) docker     (127)    28195 2024-05-01 18:24:24.000000 parallax_app-0.37.5/img/sextant.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7808 2024-05-01 18:24:24.000000 parallax_app-0.37.5/img/snapshotButton_white.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11773 2024-05-01 18:24:24.000000 parallax_app-0.37.5/img/stop-sign.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22337 2024-05-01 18:24:24.000000 parallax_app-0.37.5/img/target.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:25:06.684980 parallax_app-0.37.5/parallax/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-01 18:24:24.000000 parallax_app-0.37.5/parallax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-01 18:24:24.000000 parallax_app-0.37.5/parallax/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20086 2024-05-01 18:24:24.000000 parallax_app-0.37.5/parallax/calibration_camera.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27694 2024-05-01 18:24:24.000000 parallax_app-0.37.5/parallax/camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11239 2024-05-01 18:24:24.000000 parallax_app-0.37.5/parallax/curr_bg_cmp_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8851 2024-05-01 18:24:24.000000 parallax_app-0.37.5/parallax/curr_prev_cmp_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32394 2024-05-01 18:24:24.000000 parallax_app-0.37.5/parallax/main_window_wip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-05-01 18:24:24.000000 parallax_app-0.37.5/parallax/mask_generator.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5120 2024-05-01 18:24:24.000000 parallax_app-0.37.5/parallax/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3629 2024-05-01 18:24:24.000000 parallax_app-0.37.5/parallax/no_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12656 2024-05-01 18:24:24.000000 parallax_app-0.37.5/parallax/probe_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11920 2024-05-01 18:24:24.000000 parallax_app-0.37.5/parallax/probe_detect_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18237 2024-05-01 18:24:24.000000 parallax_app-0.37.5/parallax/probe_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6280 2024-05-01 18:24:24.000000 parallax_app-0.37.5/parallax/probe_fine_tip_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-05-01 18:24:24.000000 parallax_app-0.37.5/parallax/recording_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-01 18:24:24.000000 parallax_app-0.37.5/parallax/reticle_detect_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23325 2024-05-01 18:24:24.000000 parallax_app-0.37.5/parallax/reticle_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6982 2024-05-01 18:24:24.000000 parallax_app-0.37.5/parallax/reticle_detection_coords_interests.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12228 2024-05-01 18:24:24.000000 parallax_app-0.37.5/parallax/screen_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17562 2024-05-01 18:24:24.000000 parallax_app-0.37.5/parallax/stage_listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-05-01 18:24:24.000000 parallax_app-0.37.5/parallax/stage_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25325 2024-05-01 18:24:24.000000 parallax_app-0.37.5/parallax/stage_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6670 2024-05-01 18:24:24.000000 parallax_app-0.37.5/parallax/user_setting_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-05-01 18:24:24.000000 parallax_app-0.37.5/parallax/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:25:06.688980 parallax_app-0.37.5/parallax_app.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-05-01 18:25:06.000000 parallax_app-0.37.5/parallax_app.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-01 18:25:06.000000 parallax_app-0.37.5/parallax_app.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 18:25:06.000000 parallax_app-0.37.5/parallax_app.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-01 18:25:06.000000 parallax_app-0.37.5/parallax_app.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-01 18:25:06.000000 parallax_app-0.37.5/parallax_app.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-01 18:24:24.000000 parallax_app-0.37.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 18:25:06.688980 parallax_app-0.37.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-01 18:24:24.000000 parallax_app-0.37.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:25:06.684980 parallax_app-0.37.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-01 18:24:24.000000 parallax_app-0.37.5/tests/test_camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-01 18:24:24.000000 parallax_app-0.37.5/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-01 18:24:24.000000 parallax_app-0.37.5/tests/test_screen_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:25:06.684980 parallax_app-0.37.5/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)   192973 2024-05-01 18:24:24.000000 parallax_app-0.37.5/ui/ParallaxReadME.JPG
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:25:06.684980 parallax_app-0.37.5/ui/font/
+-rw-r--r--   0 runner    (1001) docker     (127)   259308 2024-05-01 18:24:24.000000 parallax_app-0.37.5/ui/font/FiraCode-VariableFont_wght.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     9643 2024-05-01 18:24:24.000000 parallax_app-0.37.5/ui/mainWindow.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-05-01 18:24:24.000000 parallax_app-0.37.5/ui/probe_calib.ui
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:25:06.688980 parallax_app-0.37.5/ui/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-05-01 18:24:24.000000 parallax_app-0.37.5/ui/resources/arrow-right.png
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-01 18:24:24.000000 parallax_app-0.37.5/ui/resources/check.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-01 18:24:24.000000 parallax_app-0.37.5/ui/resources/gear.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-05-01 18:24:24.000000 parallax_app-0.37.5/ui/resources/recordingButton.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4781 2024-05-01 18:24:24.000000 parallax_app-0.37.5/ui/resources/recordingButton_disabled.png
+-rw-r--r--   0 runner    (1001) docker     (127)    28195 2024-05-01 18:24:24.000000 parallax_app-0.37.5/ui/resources/sextant.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13098 2024-05-01 18:24:24.000000 parallax_app-0.37.5/ui/resources/snapshotButton_disabled.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8144 2024-05-01 18:24:24.000000 parallax_app-0.37.5/ui/resources/snapshotButton_green.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15545 2024-05-01 18:24:24.000000 parallax_app-0.37.5/ui/resources/snapshotButton_white.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11773 2024-05-01 18:24:24.000000 parallax_app-0.37.5/ui/resources/stop-sign.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22337 2024-05-01 18:24:24.000000 parallax_app-0.37.5/ui/resources/target.png
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-01 18:24:24.000000 parallax_app-0.37.5/ui/resources/x.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-05-01 18:24:24.000000 parallax_app-0.37.5/ui/reticle_calib.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    10440 2024-05-01 18:24:24.000000 parallax_app-0.37.5/ui/settingPopUpMenu.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-05-01 18:24:24.000000 parallax_app-0.37.5/ui/stage_info.ui
```

### Comparing `parallax_app-0.37.1/LICENSE` & `parallax_app-0.37.5/LICENSE`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 Allen Institute for Neural Dynamics
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2022 Allen Institute for Neural Dynamics
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `parallax_app-0.37.1/README.md` & `parallax_app-0.37.5/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,71 +1,77 @@
-# Parallax
-
-![Parallax](ui/ParallaxReadME.JPG)
-
-Parallax is a graphical user interface designed to streamline the process of setting up and performing acute *in vivo* electrophysiology experiments.
-
-
-### Prerequisites
-- Python~=3.8 (Recommended to install via [Anaconda](https://www.anaconda.com/products/individual) or [Miniconda](https://docs.conda.io/en/latest/miniconda.html))
-- PySpin (for Linux or Mac OS users)
-
-
-### Installation
-1. Create virtual environment and activate it:
-- On Windows:
-```bash
-python -m venv venv
-./venv/Scripts/activate
-```
-- On Linux/Mac:
-```bash
-python -m venv venv
-source venv/bin/activate
-```
-
-2. To install the latest version:
-```bash
-pip install parallax-app
-```
-To upgrate to the latest version:
-```bash
-pip install parallax-app --upgrade
-```
-
-### Running Parallax
-```bash
-python -m parallax
-```
-
-### Development mode
-1. Clone the repository:
-```bash
-git clone https://github.com/AllenNeuralDynamics/parallax.git
-```
-2. Install Dependencies:
-```bash
-pip install -e .[dev]
-```
-
-### Documentation
-1. To install the dependencies:
-```bash
-pip install -e .[docs]
-```
-2. Then to create the documentation html files, run:
-```bash
-sphinx-build -b html docs/ docs/_build
-```
-
-### Additional Setup for Linux and Mac OS
-For Linux or Mac OS, you'll need to install PySpin manually (not required for
-Windows):
-* download the Spinnaker SDK package for your system from [here](https://flir.app.boxcn.net/v/SpinnakerSDK)
-* follow the installation instructions in the README
-* Install the Python bindings found alongside the SDK package
-
-### Support and Contribution
-If you encounter any issues or would like to contribute to the project, please check out our issues page on GitHub.
-
-### License
-Parallax is licensed under the Allen Institute Software License. For more details, see the LICENSE file.
+# Parallax
+
+![Parallax](ui/ParallaxReadME.JPG)
+
+Parallax is a graphical user interface designed to streamline the process of setting up and performing acute *in vivo* electrophysiology experiments.
+
+User documentation available on [here](https://parallax.readthedocs.io/en/latest/).
+
+### Prerequisites
+- **Python~=3.8** (Recommended to install via [Anaconda](https://www.anaconda.com/products/individual) or [Miniconda](https://docs.conda.io/en/latest/miniconda.html))
+- PySpin (for Linux or Mac OS users)
+
+
+### Installation
+1. Create virtual environment using **Python version 3.8** and activate it:
+- On Windows:
+```bash
+python -m venv venv
+./venv/Scripts/activate
+```
+- On Linux/Mac:
+```bash
+python -m venv venv
+source venv/bin/activate
+```
+
+2. To install the latest version:
+```bash
+pip install parallax-app
+```
+To upgrate to the latest version:
+```bash
+pip install parallax-app --upgrade
+```
+
+3. To install camera interface:
+```bash
+pip install parallax-app[camera]
+```
+
+### Running Parallax
+```bash
+python -m parallax
+```
+
+### Development mode
+1. Clone the repository:
+```bash
+git clone https://github.com/AllenNeuralDynamics/parallax.git
+```
+2. Install Dependencies:
+```bash
+pip install -e .[dev]
+```
+
+### Documentation
+1. To install the dependencies:
+```bash
+pip install -e .[docs]
+```
+2. Then to create the documentation html files, run:
+```bash
+sphinx-build -b html docs/ docs/_build
+```
+
+### Additional Setup for Linux and Mac OS
+For Linux or Mac OS, you'll need to install PySpin manually (not required for
+Windows):
+* download the Spinnaker SDK package for your system from [here](https://flir.app.boxcn.net/v/SpinnakerSDK)
+* follow the installation instructions in the README
+* Install the Python bindings found alongside the SDK package
+
+### Support and Contribution
+If you encounter any issues or would like to contribute to the project, please check out our issues page on GitHub.
+
+### License
+Parallax is licensed under the MIT License. For more details, see the LICENSE file.
```

### Comparing `parallax_app-0.37.1/docs/Makefile` & `parallax_app-0.37.5/docs/Makefile`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# Minimal makefile for Sphinx documentation
-#
-
-# You can set these variables from the command line, and also
-# from the environment for the first two.
-SPHINXOPTS    ?=
-SPHINXBUILD   ?= sphinx-build
-SOURCEDIR     = .
-BUILDDIR      = _build
-
-# Put it first so that "make" without argument is like "make help".
-help:
-	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
-
-.PHONY: help Makefile
-
-# Catch-all target: route all unknown targets to Sphinx using the new
-# "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
-%: Makefile
-	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
+# Minimal makefile for Sphinx documentation
+#
+
+# You can set these variables from the command line, and also
+# from the environment for the first two.
+SPHINXOPTS    ?=
+SPHINXBUILD   ?= sphinx-build
+SOURCEDIR     = .
+BUILDDIR      = _build
+
+# Put it first so that "make" without argument is like "make help".
+help:
+	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
+
+.PHONY: help Makefile
+
+# Catch-all target: route all unknown targets to Sphinx using the new
+# "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
+%: Makefile
+	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
```

### Comparing `parallax_app-0.37.1/docs/ReadMe.rst` & `parallax_app-0.37.5/docs/ReadMe.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,84 +1,92 @@
-Welcome to Parallax
-=========================
-
-.. image:: ../ui/ParallaxReadME.jpg
-   :alt: Parallax
-
-Parallax is a graphical user interface designed to streamline the process of setting up and performing acute in vivo electrophysiology experiments.
-
-
-Prerequisites
-=========================
-- Python~=3.8 (Recommended to install via [Anaconda](https://www.anaconda.com/products/individual) or [Miniconda](https://docs.conda.io/en/latest/miniconda.html))
-- PySpin (for Linux or Mac OS users)
-
-
-Installing and Upgrading
-=========================
-
-1. Create virtual environment and activate it:
-- On Windows:
-
-.. code-block:: bash
-
-   python -m venv venv
-   ./venv/Scripts/activate
-
-- On Linux/Mac:
-
-.. code-block:: bash
-
-   python -m venv venv
-   source venv/bin/activate
-
-2. To install the latest version:
-
-.. code-block:: bash
-
-   pip install parallax-app
-
-To upgrate to the latest version:
-
-.. code-block:: bash
-
-   pip install parallax-app --upgrade
-
-Running Parallax
-=========================
-
-.. code-block:: bash
-
-   python -m parallax
-
-   
-Development mode
-=========================
-
-1. Clone the repository:
-
-.. code-block:: bash
-
-   git clone https://github.com/AllenNeuralDynamics/parallax.git
-
-2. Install Dependencies:
-
-.. code-block:: bash
-
-   pip install -e .[dev]
-
-
-Documentation
-=========================
-
-1. To install the dependencies:
-
-.. code-block:: bash
-
-   pip install -e .[docs]
-
-2. Then to create the documentation html files, run:
-
-.. code-block:: bash
-
-   sphinx-build -b html docs/ docs/_build
-
+Welcome to Parallax
+=========================
+
+.. image:: ../ui/ParallaxReadME.jpg
+   :alt: Parallax
+
+Parallax is a graphical user interface designed to streamline the process of setting up and performing acute in vivo electrophysiology experiments.
+
+
+Prerequisites
+=========================
+- **Python~=3.8** (Recommended to install via [Anaconda](https://www.anaconda.com/products/individual) or [Miniconda](https://docs.conda.io/en/latest/miniconda.html))
+- PySpin (for Linux or Mac OS users)
+
+
+Installing and Upgrading
+=========================
+
+1. Create virtual environment using **Python version 3.8** and activate it:
+- On Windows:
+
+.. code-block:: bash
+
+   python -m venv venv
+   ./venv/Scripts/activate
+
+- On Linux/Mac:
+
+.. code-block:: bash
+
+   python -m venv venv
+   source venv/bin/activate
+
+2. To install the latest version:
+
+.. code-block:: bash
+
+   pip install parallax-app
+
+To upgrate to the latest version:
+
+.. code-block:: bash
+
+   pip install parallax-app --upgrade
+
+
+3. To install camera interface:
+
+.. code-block:: bash
+   
+   pip install parallax-app[camera]
+
+
+Running Parallax
+=========================
+
+.. code-block:: bash
+
+   python -m parallax
+
+   
+Development mode
+=========================
+
+1. Clone the repository:
+
+.. code-block:: bash
+
+   git clone https://github.com/AllenNeuralDynamics/parallax.git
+
+2. Install Dependencies:
+
+.. code-block:: bash
+
+   pip install -e .[dev]
+
+
+Documentation
+=========================
+
+1. To install the dependencies:
+
+.. code-block:: bash
+
+   pip install -e .[docs]
+
+2. Then to create the documentation html files, run:
+
+.. code-block:: bash
+
+   sphinx-build -b html docs/ docs/_build
+
```

### Comparing `parallax_app-0.37.1/docs/conf.py` & `parallax_app-0.37.5/docs/conf.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-# Configuration file for the Sphinx documentation builder.
-#
-# For the full list of built-in configuration values, see the documentation:
-# https://www.sphinx-doc.org/en/master/usage/configuration.html
-
-# -- Project information -----------------------------------------------------
-# https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
-import os
-import sys
-
-sys.path.insert(0, os.path.abspath(".."))
-
-project = 'Parallax'
-copyright = '2024, Hanna Lee'
-author = 'Hanna Lee'
-release = '0.37.1'
-
-# -- General configuration ---------------------------------------------------
-# https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
-
-extensions = ["sphinx.ext.todo", "sphinx.ext.viewcode", "sphinx.ext.autodoc"]
-
-templates_path = ['_templates']
-exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
-
-
-
-# -- Options for HTML output -------------------------------------------------
-# https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
-
-html_theme = 'furo'
-html_static_path = ['_static']
+# Configuration file for the Sphinx documentation builder.
+#
+# For the full list of built-in configuration values, see the documentation:
+# https://www.sphinx-doc.org/en/master/usage/configuration.html
+
+# -- Project information -----------------------------------------------------
+# https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
+import os
+import sys
+
+sys.path.insert(0, os.path.abspath(".."))
+
+project = 'Parallax'
+copyright = '2024, Hanna Lee'
+author = 'Hanna Lee'
+release = '0.37.1'
+
+# -- General configuration ---------------------------------------------------
+# https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
+
+extensions = ["sphinx.ext.todo", "sphinx.ext.viewcode", "sphinx.ext.autodoc"]
+
+templates_path = ['_templates']
+exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
+
+
+
+# -- Options for HTML output -------------------------------------------------
+# https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
+
+html_theme = 'furo'
+html_static_path = ['_static']
```

### Comparing `parallax_app-0.37.1/docs/make.bat` & `parallax_app-0.37.5/docs/make.bat`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-@ECHO OFF
-
-pushd %~dp0
-
-REM Command file for Sphinx documentation
-
-if "%SPHINXBUILD%" == "" (
-	set SPHINXBUILD=sphinx-build
-)
-set SOURCEDIR=.
-set BUILDDIR=_build
-
-%SPHINXBUILD% >NUL 2>NUL
-if errorlevel 9009 (
-	echo.
-	echo.The 'sphinx-build' command was not found. Make sure you have Sphinx
-	echo.installed, then set the SPHINXBUILD environment variable to point
-	echo.to the full path of the 'sphinx-build' executable. Alternatively you
-	echo.may add the Sphinx directory to PATH.
-	echo.
-	echo.If you don't have Sphinx installed, grab it from
-	echo.https://www.sphinx-doc.org/
-	exit /b 1
-)
-
-if "%1" == "" goto help
-
-%SPHINXBUILD% -M %1 %SOURCEDIR% %BUILDDIR% %SPHINXOPTS% %O%
-goto end
-
-:help
-%SPHINXBUILD% -M help %SOURCEDIR% %BUILDDIR% %SPHINXOPTS% %O%
-
-:end
-popd
+@ECHO OFF
+
+pushd %~dp0
+
+REM Command file for Sphinx documentation
+
+if "%SPHINXBUILD%" == "" (
+	set SPHINXBUILD=sphinx-build
+)
+set SOURCEDIR=.
+set BUILDDIR=_build
+
+%SPHINXBUILD% >NUL 2>NUL
+if errorlevel 9009 (
+	echo.
+	echo.The 'sphinx-build' command was not found. Make sure you have Sphinx
+	echo.installed, then set the SPHINXBUILD environment variable to point
+	echo.to the full path of the 'sphinx-build' executable. Alternatively you
+	echo.may add the Sphinx directory to PATH.
+	echo.
+	echo.If you don't have Sphinx installed, grab it from
+	echo.https://www.sphinx-doc.org/
+	exit /b 1
+)
+
+if "%1" == "" goto help
+
+%SPHINXBUILD% -M %1 %SOURCEDIR% %BUILDDIR% %SPHINXOPTS% %O%
+goto end
+
+:help
+%SPHINXBUILD% -M help %SOURCEDIR% %BUILDDIR% %SPHINXOPTS% %O%
+
+:end
+popd
```

### Comparing `parallax_app-0.37.1/img/arrow-right.png` & `parallax_app-0.37.5/img/arrow-right.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.1/img/gear.png` & `parallax_app-0.37.5/img/gear.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.1/img/recordingButton.png` & `parallax_app-0.37.5/img/recordingButton.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.1/img/sextant.png` & `parallax_app-0.37.5/img/sextant.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.1/img/snapshotButton_white.png` & `parallax_app-0.37.5/img/snapshotButton_white.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.1/img/stop-sign.png` & `parallax_app-0.37.5/img/stop-sign.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.1/img/target.png` & `parallax_app-0.37.5/img/target.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.1/parallax/__main__.py` & `parallax_app-0.37.5/parallax/__main__.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,74 +1,74 @@
-"""
-Parallax: A GUI application for controlling hardware devices.
-"""
-
-import argparse
-import atexit
-import logging
-import os
-
-from PyQt5.QtWidgets import QApplication
-
-from parallax.main_window_wip import MainWindow as MainWindowV2
-from parallax.model import Model
-
-
-def setup_logging():
-    """Set up logging to file."""
-    logger = logging.getLogger()
-    logger.handlers.clear()
-    logger.setLevel(logging.WARNING)
-
-    # Create the directory if it doesn't exist
-    package_dir = os.path.dirname(os.path.abspath(__file__))
-    debug_dir = os.path.join(os.path.dirname(package_dir), "debug")
-    os.makedirs(debug_dir, exist_ok=True)
-    log_file_path = os.path.join(debug_dir, "parallax_debug.log")
-
-    with open(log_file_path, "w") as log_file:
-        # Clear the log file
-        pass
-
-    log_handler = logging.FileHandler(log_file_path)
-    log_handler.setLevel(logging.DEBUG)
-    log_handler.setFormatter(
-        logging.Formatter(
-            fmt="%(asctime)s:%(name)s:%(levelname)s: %(message)s"
-        )
-    )
-    logger.addHandler(log_handler)
-
-
-# Main function to run the Parallax application
-if __name__ == "__main__":
-    # Parse command line arguments to configure application behavior
-    parser = argparse.ArgumentParser()
-    parser.add_argument(
-        "-d",
-        "--dummy",
-        action="store_true",
-        help="Dummy mode for testing without hardware",
-    )
-    args = parser.parse_args()
-
-    # Print a message if running in dummy mode (no hardware interaction)
-    if args.dummy:
-        print("\nRunning in dummy mode; hardware devices not accessible.")
-
-    # Set up logging as configured in the setup_logging function
-    setup_logging()
-
-    # Initialize the Qt application
-    app = QApplication([])
-    model = Model(version="V2")  # Initialize the data model with version "V2"
-    main_window = MainWindowV2(model, dummy=args.dummy)  # main window
-
-    # Show the main window on screen
-    main_window.show()
-    # Start the Qt application's main loop
-    app.exec()
-
-    # Register cleanup functions to be called on program termination
-    atexit.register(model.clean)  # Clean up resources used by the model
-    # Save user configurations on exit
-    atexit.register(main_window.save_user_configs)
+"""
+Parallax: A GUI application for controlling hardware devices.
+"""
+
+import argparse
+import atexit
+import logging
+import os
+
+from PyQt5.QtWidgets import QApplication
+
+from parallax.main_window_wip import MainWindow as MainWindowV2
+from parallax.model import Model
+
+
+def setup_logging():
+    """Set up logging to file."""
+    logger = logging.getLogger()
+    logger.handlers.clear()
+    logger.setLevel(logging.WARNING)
+
+    # Create the directory if it doesn't exist
+    package_dir = os.path.dirname(os.path.abspath(__file__))
+    debug_dir = os.path.join(os.path.dirname(package_dir), "debug")
+    os.makedirs(debug_dir, exist_ok=True)
+    log_file_path = os.path.join(debug_dir, "parallax_debug.log")
+
+    with open(log_file_path, "w") as log_file:
+        # Clear the log file
+        pass
+
+    log_handler = logging.FileHandler(log_file_path)
+    log_handler.setLevel(logging.DEBUG)
+    log_handler.setFormatter(
+        logging.Formatter(
+            fmt="%(asctime)s:%(name)s:%(levelname)s: %(message)s"
+        )
+    )
+    logger.addHandler(log_handler)
+
+
+# Main function to run the Parallax application
+if __name__ == "__main__":
+    # Parse command line arguments to configure application behavior
+    parser = argparse.ArgumentParser()
+    parser.add_argument(
+        "-d",
+        "--dummy",
+        action="store_true",
+        help="Dummy mode for testing without hardware",
+    )
+    args = parser.parse_args()
+
+    # Print a message if running in dummy mode (no hardware interaction)
+    if args.dummy:
+        print("\nRunning in dummy mode; hardware devices not accessible.")
+
+    # Set up logging as configured in the setup_logging function
+    setup_logging()
+
+    # Initialize the Qt application
+    app = QApplication([])
+    model = Model(version="V2")  # Initialize the data model with version "V2"
+    main_window = MainWindowV2(model, dummy=args.dummy)  # main window
+
+    # Show the main window on screen
+    main_window.show()
+    # Start the Qt application's main loop
+    app.exec()
+
+    # Register cleanup functions to be called on program termination
+    atexit.register(model.clean)  # Clean up resources used by the model
+    # Save user configurations on exit
+    atexit.register(main_window.save_user_configs)
```

### Comparing `parallax_app-0.37.1/parallax/calibration_camera.py` & `parallax_app-0.37.5/parallax/calibration_camera.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,556 +1,556 @@
-"""
-Module for camera calibration and stereo calibration.
-This module provides classes for intrinsic camera calibration
-(`CalibrationCamera`) and stereo camera calibration (`CalibrationStereo`).
-Classes:
--CalibrationCamera: Class for intrinsic camera calibration.
--CalibrationStereo: Class for stereo camera calibration.
-"""
-
-import logging
-
-import cv2
-import numpy as np
-
-# Set logger name
-logger = logging.getLogger(__name__)
-logger.setLevel(logging.DEBUG)
-# Set the logging level for PyQt5.uic.uiparser/properties
-logging.getLogger("PyQt5.uic.uiparser").setLevel(logging.DEBUG)
-logging.getLogger("PyQt5.uic.properties").setLevel(logging.DEBUG)
-
-# Objectpoints
-WORLD_SCALE = 0.2  # 200 um per tick mark --> Translation matrix will be in mm
-X_COORDS_HALF = 15
-Y_COORDS_HALF = 15
-X_COORDS = X_COORDS_HALF * 2 + 1
-Y_COORDS = Y_COORDS_HALF * 2 + 1
-OBJPOINTS = np.zeros((X_COORDS + Y_COORDS, 3), np.float32)
-OBJPOINTS[:X_COORDS, 0] = np.arange(-X_COORDS_HALF, X_COORDS_HALF + 1)
-OBJPOINTS[X_COORDS:, 1] = np.arange(-Y_COORDS_HALF, Y_COORDS_HALF + 1)
-OBJPOINTS = OBJPOINTS * WORLD_SCALE
-OBJPOINTS = np.around(OBJPOINTS, decimals=2)
-CENTER_INDEX_X = X_COORDS_HALF
-CENTER_INDEX_Y = X_COORDS + Y_COORDS_HALF
-
-# Calibration
-CRIT = (cv2.TERM_CRITERIA_EPS, 0, 1e-11)
-"""
-imtx = np.array([[1.52e+04, 0.0e+00, 2e+03],
-                [0.0e+00, 1.52e+04, 1.5e+03],
-                [0.0e+00, 0.0e+00, 1.0e+00]],
-                dtype=np.float32)
-idist = np.array([[ 0e+00, 0e+00, 0e+00, 0e+00, 0e+00 ]],
-                    dtype=np.float32)
-
-imtx = np.array([[1.515e+04, 0.0e+00, 2e+03],
-                [0.0e+00, 1.515e+04, 1.5e+03],
-                [0.0e+00, 0.0e+00, 1.0e+00]],
-                dtype=np.float32)
-idist = np.array([[ -0.02e+00, 5e+00, 0e+00, 0e+00, 100e+00 ]],
-                    dtype=np.float32)
-"""
-imtx = np.array([[1.519e+04, 0.0e+00, 2e+03],
-                [0.0e+00, 1.519e+04, 1.5e+03],
-                [0.0e+00, 0.0e+00, 1.0e+00]],
-                dtype=np.float32)
-
-idist = np.array([[0e00, 0e00, 0e00, 0e00, 0e00]], dtype=np.float32)
-
-# Intrinsic flag
-myflags1 = (
-    cv2.CALIB_USE_INTRINSIC_GUESS
-    | cv2.CALIB_FIX_FOCAL_LENGTH
-    | cv2.CALIB_FIX_PRINCIPAL_POINT
-    | cv2.CALIB_FIX_ASPECT_RATIO
-    | cv2.CALIB_FIX_K1
-    | cv2.CALIB_FIX_K2
-    | cv2.CALIB_FIX_K3
-    | cv2.CALIB_FIX_TANGENT_DIST
-)
-
-myflags2 = (
-    cv2.CALIB_FIX_PRINCIPAL_POINT
-    | cv2.CALIB_USE_INTRINSIC_GUESS
-    | cv2.CALIB_FIX_ASPECT_RATIO
-    | cv2.CALIB_FIX_FOCAL_LENGTH
-)
-
-SIZE = (4000, 3000)
-
-
-class CalibrationCamera:
-    """Class for intrinsic calibration."""
-
-    def __init__(self, camera_name):
-        """Initialize the CalibrationCamera object"""
-        self.name = camera_name
-        self.n_interest_pixels = 15
-        self.imgpoints = None
-        self.objpoints = None
-
-    def _get_changed_data_format(self, x_axis, y_axis):
-        """
-        Change data format for calibration.
-
-        Args:
-            x_axis (list): X-axis coordinates.
-            y_axis (list): Y-axis coordinates.
-
-        Returns:
-            numpy.ndarray: Reshaped coordinates.
-        """
-        x_axis = np.array(x_axis)
-        y_axis = np.array(y_axis)
-        coords_lines = np.vstack([x_axis, y_axis])
-        nCoords_per_axis = self.n_interest_pixels * 2 + 1
-        coords_lines_reshaped = coords_lines.reshape(
-            (nCoords_per_axis * 2, 2)
-        ).astype(np.float32)
-        return coords_lines_reshaped
-
-    def _process_reticle_points(self, x_axis, y_axis):
-        """
-        Process reticle points for calibration.
-        Args:
-            x_axis (list): X-axis coordinates.
-            y_axis (list): Y-axis coordinates.
-        Returns:
-            tuple: Image points and object points.
-        """
-        self.objpoints = []
-        self.imgpoints = []
-
-        coords_lines_foramtted = self._get_changed_data_format(x_axis, y_axis)
-        self.imgpoints.append(coords_lines_foramtted)
-        self.objpoints.append(OBJPOINTS)
-
-        self.objpoints = np.array(self.objpoints)
-        self.imgpoints = np.array(self.imgpoints)
-        return self.imgpoints, self.objpoints
-
-    def calibrate_camera(self, x_axis, y_axis):
-        """
-        Calibrate camera Intrinsic.
-
-        Args:
-            x_axis (list): X-axis coordinates.
-            y_axis (list): Y-axis coordinates.
-
-        Returns:
-            tuple: Calibration results (ret, mtx, dist).
-        """
-        self._process_reticle_points(x_axis, y_axis)
-        ret, self.mtx, self.dist, self.rvecs, self.tvecs = cv2.calibrateCamera(
-            self.objpoints,
-            self.imgpoints,
-            SIZE,
-            imtx,
-            idist,
-            flags=myflags1,
-            criteria=CRIT,
-        )
-
-        format_mtxt = (
-            "\n".join(
-                [" ".join([f"{val:.2f}" for val in row]) for row in self.mtx]
-            )
-            + "\n"
-        )
-        format_dist = " ".join([f"{val:.2f}" for val in self.dist[0]]) + "\n"
-        logger.debug(f"A reproj error: {ret}")
-        logger.debug(f"Intrinsic: {format_mtxt}\n")
-        logger.debug(f"Distortion: {format_dist}\n")
-        logger.debug(f"Focal length: {self.mtx[0][0]*1.85/1000}")
-        distancesA = [np.linalg.norm(vec) for vec in self.tvecs]
-        logger.debug(
-            f"Distance from camera to world center: {np.mean(distancesA)}"
-        )
-        return ret, self.mtx, self.dist
-
-    def get_predefined_intrinsic(self, x_axis, y_axis):
-        """
-        Fetches predefined intrinsic camera parameters for specific models.
-        Parameters:
-        - x_axis (int or float): The x-axis value for reticle processing.
-        - y_axis (int or float): The y-axis value for reticle processing.
-
-        Returns:
-        - A tuple of (bool, numpy.ndarray or None, numpy.ndarray or None) 
-        representing success status, intrinsic matrix, 
-        and distortion coefficients respectively.
-        """
-        self._process_reticle_points(x_axis, y_axis)
-        if self.name == "22517664":
-            self.mtx = np.array([[1.520480e+04, 0.0e+00, 2e+03],
-                [0.0e+00, 1.520480e+04, 1.5e+03],
-                [0.0e+00, 0.0e+00, 1.0e+00]],
-                dtype=np.float32)
-            self.dist = np.array([[-0.02, 8.26, -0.01, -0.00, -63.01]],
-                                dtype=np.float32)
-            return True, self.mtx, self.dist
-        
-        elif self.name == "22433200":
-            self.mtx = np.array([[1.507121e+04, 0.0e+00, 2e+03],
-                [0.0e+00, 1.507121e+04, 1.5e+03],
-                [0.0e+00, 0.0e+00, 1.0e+00]],
-                dtype=np.float32)
-            self.dist = np.array([[-0.02, 1.90, -0.00, -0.01, 200.94]],
-                                dtype=np.float32)
-            return True, self.mtx, self.dist
-        
-        else:
-            return False, None, None
-
-    def get_origin_xyz(self):
-        """
-        Get origin (0,0) and axis points (x, y, z coords) in image coordinates.
-
-        Returns:
-            tuple: Origin, x-axis, y-axis, z-axis points.
-        """
-        axis = np.float32([[3, 0, 0], [0, 3, 0], [0, 0, 3]]).reshape(-1, 3)
-        # Find the rotation and translation vectors.
-        # Output rotation vector (see Rodrigues ) that, together with tvec,
-        # brings points from the model coordinate system 
-        # to the camera coordinate system.
-        if self.objpoints is not None:
-            solvePnP_method = cv2.SOLVEPNP_ITERATIVE
-            _, rvecs, tvecs = cv2.solvePnP(
-                self.objpoints,
-                self.imgpoints,
-                self.mtx,
-                self.dist,
-                flags=solvePnP_method,
-            )
-            imgpts, _ = cv2.projectPoints(
-                axis, rvecs, tvecs, self.mtx, self.dist
-            )
-            origin = tuple(
-                self.imgpoints[0][CENTER_INDEX_X].ravel().astype(int)
-            )
-            x = tuple(imgpts[0].ravel().astype(int))
-            y = tuple(imgpts[1].ravel().astype(int))
-            z = tuple(imgpts[2].ravel().astype(int))
-            return origin, x, y, z
-        else:
-            return None
-
-
-class CalibrationStereo(CalibrationCamera):
-    """
-    Class for stereo camera calibration.
-    """
-
-    def __init__(
-        self, camA, imgpointsA, intrinsicA, camB, imgpointsB, intrinsicB):
-        """Initialize the CalibrationStereo object"""
-        self.n_interest_pixels = 15
-        self.camA = camA
-        self.camB = camB
-        self.imgpointsA, self.objpoints = self._process_reticle_points(
-            imgpointsA[0], imgpointsA[1])
-        self.imgpointsB, self.objpoints = self._process_reticle_points(
-            imgpointsB[0], imgpointsB[1])
-        self.mtxA, self.distA = intrinsicA[0], intrinsicA[1]
-        self.mtxB, self.distB = intrinsicB[0], intrinsicB[1]
-        self.criteria = (cv2.TERM_CRITERIA_EPS + cv2.TERM_CRITERIA_MAX_ITER, 100, 0.001)
-        self.flags = cv2.CALIB_FIX_INTRINSIC
-        self.retval, self.R_AB, self.T_AB, self.E_AB, self.F_AB = None, None, None, None, None 
-        self.P_A, self.P_B = None, None
-
-    def calibrate_stereo(self):
-        """Calibrate stereo cameras.
-
-        Returns:
-            tuple: Stereo calibration results (retval, R_AB, T_AB, E_AB, F_AB).
-        """
-        self.retval, _, _, _, _, self.R_AB, self.T_AB, self.E_AB, self.F_AB = (
-            cv2.stereoCalibrate(
-                self.objpoints,
-                self.imgpointsA,
-                self.imgpointsB,
-                self.mtxA,
-                self.distA,
-                self.mtxB,
-                self.distB,
-                SIZE,
-                criteria=self.criteria,
-                flags=self.flags,
-            )
-        )
-
-        print("\n== Stereo Calibration ==")
-        print("AB")
-        print(self.retval)
-        print(f"R: \n{self.R_AB}")
-        print(f"T: \n{self.T_AB}")
-        print(np.linalg.norm(self.T_AB))
-
-        formatted_F = (
-            "F_AB:\n"
-            + "\n".join(
-                [" ".join([f"{val:.5f}" for val in row]) for row in self.F_AB]
-            ) + "\n")
-        formatted_E = (
-            "E_AB:\n"
-            + "\n".join(
-                [" ".join([f"{val:.5f}" for val in row]) for row in self.E_AB]
-            ) + "\n")
-        print(formatted_F)
-        print(formatted_E)
-
-        self.P_A = self.mtxA @ np.hstack((np.eye(3), np.zeros((3, 1))))
-        self.P_B = self.mtxB @ np.hstack((self.R_AB, self.T_AB.reshape(-1, 1)))
-
-        return self.retval, self.R_AB, self.T_AB, self.E_AB, self.F_AB
-
-    def _matching_camera_order(self, camA, coordA, camB, coordB):
-        """Match camera order based on initialization order.
-
-        Args:
-            camA (str): Camera A name.
-            coordA (tuple): Coordinates from camera A.
-            camB (str): Camera B name.
-            coordB (tuple): Coordinates from camera B.
-
-        Returns:
-            tuple: Matched camera order and coordinates.
-        """
-        if self.camA == camA:
-            return camA, coordA, camB, coordB
-
-        if self.camA == camB:
-            return camB, coordB, camA, coordA
-
-    def triangulation(self, P_1, P_2, imgpoints_1, imgpoints_2):
-        """Triangulate 3D points from stereo image points.
-
-        Args:
-            P_1 (numpy.ndarray): Projection matrix of camera 1.
-            P_2 (numpy.ndarray): Projection matrix of camera 2.
-            imgpoints_1 (numpy.ndarray): Image points from camera 1.
-            imgpoints_2 (numpy.ndarray): Image points from camera 2.
-
-        Returns:
-            numpy.ndarray: Triangulated 3D points.
-        """
-        points_4d_hom = cv2.triangulatePoints(
-            P_1, P_2, imgpoints_1.T, imgpoints_2.T
-        )
-        points_3d_hom = points_4d_hom / points_4d_hom[3]
-        points_3d_hom = points_3d_hom.T
-        return points_3d_hom[:, :3]
-
-    def change_coords_system_from_camA_to_global(self, points_3d_AB):
-        """
-        Change coordinate system from camera A to global using solvePnPRansac.
-
-        Args:
-            points_3d_AB (numpy.ndarray):
-            3D points in camera A coordinate system.
-
-        Returns:
-            numpy.ndarray: 3D points in global coordinate system.
-        """
-        _, rvecs, tvecs, _ = cv2.solvePnPRansac(
-            self.objpoints, self.imgpointsA, self.mtxA, self.distA
-        )
-        # Convert rotation vectors to rotation matrices
-        rmat, _ = cv2.Rodrigues(rvecs)
-        # Invert the rotation and translation
-        rmat_inv = rmat.T  # Transpose of rotation matrix is its inverse
-        tvecs_inv = -rmat_inv @ tvecs
-        # Transform the points
-        points_3d_G = np.dot(rmat_inv, points_3d_AB.T).T + tvecs_inv.T
-        return points_3d_G
-
-    def change_coords_system_from_camA_to_global_iterative(self, points_3d_AB):
-        """Change coordinate system from camera A to global 
-        using iterative method.
-
-        Args:
-            points_3d_AB (numpy.ndarray):
-            3D points in camera A coordinate system.
-
-        Returns:
-            numpy.ndarray: 3D points in global coordinate system.
-        """
-        solvePnP_method = cv2.SOLVEPNP_ITERATIVE
-        _, rvecs, tvecs = cv2.solvePnP(
-            self.objpoints,
-            self.imgpointsA,
-            self.mtxA,
-            self.distA,
-            flags=solvePnP_method,
-        )
-        logger.debug("solvePnP")
-        logger.debug(rvecs)
-        logger.debug(tvecs)
-        # Convert rotation vectors to rotation matrices
-        rmat, _ = cv2.Rodrigues(rvecs)
-        # Invert the rotation and translation
-        self.rmat_inv = rmat.T  # Transpose of rotation matrix is its inverse
-        self.tvecs_inv = -self.rmat_inv @ tvecs
-        # Transform the points
-        points_3d_G = np.dot(self.rmat_inv, points_3d_AB.T).T + self.tvecs_inv.T
-        return points_3d_G
-
-    def change_coords_system_from_camA_to_global_savedRT(self, points_3d_AB):
-        """Change coordinate system from camera A to global
-        using saved rotation and translation.
-
-        Args:
-            points_3d_AB (numpy.ndarray):
-            3D points in camera A coordinate system.
-
-        Returns:
-            numpy.ndarray: 3D points in global coordinate system.
-        """
-        points_3d_G = np.dot(self.rmat_inv, points_3d_AB.T).T + self.tvecs_inv.T
-        return points_3d_G
-
-    def get_global_coords(self, camA, coordA, camB, coordB):
-        """Get global coordinates from stereo image coordinates.
-
-        Args:
-            camA (str): Camera A name.
-            coordA (tuple): Coordinates from camera A.
-            camB (str): Camera B name.
-            coordB (tuple): Coordinates from camera B.
-
-        Returns:
-            numpy.ndarray: 3D points in global coordinate system.
-        """
-        camA, coordA, camB, coordB = self._matching_camera_order(
-            camA, coordA, camB, coordB
-        )
-        coordA = np.array(coordA).astype(np.float32)
-        coordB = np.array(coordB).astype(np.float32)
-        points_3d_AB = self.triangulation(self.P_B, self.P_A, coordB, coordA)
-        points_3d_G = self.change_coords_system_from_camA_to_global_savedRT(
-            points_3d_AB
-        )
-
-        logger.debug(
-            f"points_3d_G: {points_3d_G}, coordA: {coordA}, coordB: {coordB}"
-        )
-        return points_3d_G
-
-    def test_x_y_z_performance(self, points_3d_G):
-        # Calculate the differences for each dimension
-        differences_x = points_3d_G[:, 0] - self.objpoints[0, :, 0]
-        differences_y = points_3d_G[:, 1] - self.objpoints[0, :, 1]
-        differences_z = points_3d_G[:, 2] - self.objpoints[0, :, 2]
-
-        # Calculate the mean squared differences for each dimension
-        mean_squared_diff_x = np.mean(np.square(differences_x))
-        mean_squared_diff_y = np.mean(np.square(differences_y))
-        mean_squared_diff_z = np.mean(np.square(differences_z))
-
-        # Calculate the L2 norm (Euclidean distance) for each dimension
-        l2_x = np.sqrt(mean_squared_diff_x)
-        l2_y = np.sqrt(mean_squared_diff_y)
-        l2_z = np.sqrt(mean_squared_diff_z)
-
-        print(
-            f"x: {l2_x*1000}µm³, y: {l2_y*1000}µm³, z:{l2_z*1000}µm³"
-        )
-
-    def test_performance(self, camA, coordA, camB, coordB):
-        """Test stereo calibration.
-
-        Args:
-            camA (str): Camera A name.
-            coordA (tuple): Coordinates from camera A.
-            camB (str): Camera B name.
-            coordB (tuple): Coordinates from camera B.
-
-        Returns:
-            numpy.ndarray: Predicted 3D points in global coordinate system.
-        """
-        camA, coordA, camB, coordB = self._matching_camera_order(
-            camA, coordA, camB, coordB
-        )
-        logger.debug(f"coordA: {coordA}")
-        logger.debug(f"coordB: {coordB}")
-        points_3d_AB = self.triangulation(
-            self.P_B, self.P_A, self.imgpointsB, self.imgpointsA
-        )
-        np.set_printoptions(suppress=True, precision=8)
-
-        points_3d_G = self.change_coords_system_from_camA_to_global_iterative(
-            points_3d_AB
-        )
-        print("\n=solvePnP SOLVEPNP_ITERATIVE=")
-        differences = points_3d_G - self.objpoints[0]
-        squared_distances = np.sum(np.square(differences), axis=1)
-        euclidean_distances = np.sqrt(squared_distances)
-        average_L2_distance = np.mean(euclidean_distances)
-        print(
-            f"(Reprojection error) Object points L2 diff: \
-            {average_L2_distance*1000} µm³"
-        )
-        self.test_x_y_z_performance(points_3d_G)
-        print(f"Object points predict:\n{np.around(points_3d_G, decimals=5)}")
-
-        self.test_pixel_error()
-        return average_L2_distance
-
-    def test_pixel_error(self):
-        """Test pixel reprojection error."""
-        mean_error = 0
-        for i in range(len(self.objpoints)):
-            imgpointsA_converted = np.array(
-                self.imgpointsA[i], dtype=np.float32
-            ).reshape(-1, 2)
-            solvePnP_method = cv2.SOLVEPNP_ITERATIVE
-            retval, rvecs, tvecs = cv2.solvePnP(
-                self.objpoints[i],
-                imgpointsA_converted,
-                self.mtxA,
-                self.distA,
-                flags=solvePnP_method,
-            )
-            imgpoints2, _ = cv2.projectPoints(
-                self.objpoints[i], rvecs, tvecs, self.mtxA, self.distA
-            )
-
-            imgpoints2_reshaped = imgpoints2.reshape(-1, 2)
-            differences = imgpointsA_converted - imgpoints2_reshaped
-            squared_distances = np.sum(np.square(differences), axis=1)
-            distances = np.sqrt(squared_distances)
-            average_L2_distance = np.mean(distances)
-            mean_error += average_L2_distance
-            logger.debug("A pixel diff")
-            logger.debug(imgpointsA_converted-imgpoints2_reshaped)
-        total_err = mean_error / len(self.objpoints)
-        print(f"(Reprojection error) Pixel L2 diff A: {total_err} pixels")
-
-        mean_error = 0
-        for i in range(len(self.objpoints)):
-            imgpointsB_converted = np.array(
-                self.imgpointsB[i], dtype=np.float32
-            ).reshape(-1, 2)
-            solvePnP_method = cv2.SOLVEPNP_ITERATIVE
-            retval, rvecs, tvecs = cv2.solvePnP(
-                self.objpoints[i],
-                imgpointsB_converted,
-                self.mtxB,
-                self.distB,
-                flags=solvePnP_method,
-            )
-            imgpoints2, _ = cv2.projectPoints(
-                self.objpoints[i], rvecs, tvecs, self.mtxB, self.distB
-            )
-
-            imgpoints2_reshaped = imgpoints2.reshape(-1, 2)
-            differences = imgpointsB_converted - imgpoints2_reshaped
-            distances = np.sqrt(np.sum(np.square(differences), axis=1))
-            average_L2_distance = np.mean(distances)
-            mean_error += average_L2_distance
-            logger.debug("B pixel diff")
-            logger.debug(imgpointsB_converted - imgpoints2_reshaped)
-
-        total_err = mean_error / len(self.objpoints)
-        print(f"(Reprojection error) Pixel L2 diff B: {total_err} pixels")
+"""
+Module for camera calibration and stereo calibration.
+This module provides classes for intrinsic camera calibration
+(`CalibrationCamera`) and stereo camera calibration (`CalibrationStereo`).
+Classes:
+-CalibrationCamera: Class for intrinsic camera calibration.
+-CalibrationStereo: Class for stereo camera calibration.
+"""
+
+import logging
+
+import cv2
+import numpy as np
+
+# Set logger name
+logger = logging.getLogger(__name__)
+logger.setLevel(logging.WARNING)
+# Set the logging level for PyQt5.uic.uiparser/properties
+logging.getLogger("PyQt5.uic.uiparser").setLevel(logging.DEBUG)
+logging.getLogger("PyQt5.uic.properties").setLevel(logging.DEBUG)
+
+# Objectpoints
+WORLD_SCALE = 0.2  # 200 um per tick mark --> Translation matrix will be in mm
+X_COORDS_HALF = 15
+Y_COORDS_HALF = 15
+X_COORDS = X_COORDS_HALF * 2 + 1
+Y_COORDS = Y_COORDS_HALF * 2 + 1
+OBJPOINTS = np.zeros((X_COORDS + Y_COORDS, 3), np.float32)
+OBJPOINTS[:X_COORDS, 0] = np.arange(-X_COORDS_HALF, X_COORDS_HALF + 1)
+OBJPOINTS[X_COORDS:, 1] = np.arange(-Y_COORDS_HALF, Y_COORDS_HALF + 1)
+OBJPOINTS = OBJPOINTS * WORLD_SCALE
+OBJPOINTS = np.around(OBJPOINTS, decimals=2)
+CENTER_INDEX_X = X_COORDS_HALF
+CENTER_INDEX_Y = X_COORDS + Y_COORDS_HALF
+
+# Calibration
+CRIT = (cv2.TERM_CRITERIA_EPS, 0, 1e-11)
+"""
+imtx = np.array([[1.52e+04, 0.0e+00, 2e+03],
+                [0.0e+00, 1.52e+04, 1.5e+03],
+                [0.0e+00, 0.0e+00, 1.0e+00]],
+                dtype=np.float32)
+idist = np.array([[ 0e+00, 0e+00, 0e+00, 0e+00, 0e+00 ]],
+                    dtype=np.float32)
+
+imtx = np.array([[1.515e+04, 0.0e+00, 2e+03],
+                [0.0e+00, 1.515e+04, 1.5e+03],
+                [0.0e+00, 0.0e+00, 1.0e+00]],
+                dtype=np.float32)
+idist = np.array([[ -0.02e+00, 5e+00, 0e+00, 0e+00, 100e+00 ]],
+                    dtype=np.float32)
+"""
+imtx = np.array([[1.519e+04, 0.0e+00, 2e+03],
+                [0.0e+00, 1.519e+04, 1.5e+03],
+                [0.0e+00, 0.0e+00, 1.0e+00]],
+                dtype=np.float32)
+
+idist = np.array([[0e00, 0e00, 0e00, 0e00, 0e00]], dtype=np.float32)
+
+# Intrinsic flag
+myflags1 = (
+    cv2.CALIB_USE_INTRINSIC_GUESS
+    | cv2.CALIB_FIX_FOCAL_LENGTH
+    | cv2.CALIB_FIX_PRINCIPAL_POINT
+    | cv2.CALIB_FIX_ASPECT_RATIO
+    | cv2.CALIB_FIX_K1
+    | cv2.CALIB_FIX_K2
+    | cv2.CALIB_FIX_K3
+    | cv2.CALIB_FIX_TANGENT_DIST
+)
+
+myflags2 = (
+    cv2.CALIB_FIX_PRINCIPAL_POINT
+    | cv2.CALIB_USE_INTRINSIC_GUESS
+    | cv2.CALIB_FIX_ASPECT_RATIO
+    | cv2.CALIB_FIX_FOCAL_LENGTH
+)
+
+SIZE = (4000, 3000)
+
+
+class CalibrationCamera:
+    """Class for intrinsic calibration."""
+
+    def __init__(self, camera_name):
+        """Initialize the CalibrationCamera object"""
+        self.name = camera_name
+        self.n_interest_pixels = 15
+        self.imgpoints = None
+        self.objpoints = None
+
+    def _get_changed_data_format(self, x_axis, y_axis):
+        """
+        Change data format for calibration.
+
+        Args:
+            x_axis (list): X-axis coordinates.
+            y_axis (list): Y-axis coordinates.
+
+        Returns:
+            numpy.ndarray: Reshaped coordinates.
+        """
+        x_axis = np.array(x_axis)
+        y_axis = np.array(y_axis)
+        coords_lines = np.vstack([x_axis, y_axis])
+        nCoords_per_axis = self.n_interest_pixels * 2 + 1
+        coords_lines_reshaped = coords_lines.reshape(
+            (nCoords_per_axis * 2, 2)
+        ).astype(np.float32)
+        return coords_lines_reshaped
+
+    def _process_reticle_points(self, x_axis, y_axis):
+        """
+        Process reticle points for calibration.
+        Args:
+            x_axis (list): X-axis coordinates.
+            y_axis (list): Y-axis coordinates.
+        Returns:
+            tuple: Image points and object points.
+        """
+        self.objpoints = []
+        self.imgpoints = []
+
+        coords_lines_foramtted = self._get_changed_data_format(x_axis, y_axis)
+        self.imgpoints.append(coords_lines_foramtted)
+        self.objpoints.append(OBJPOINTS)
+
+        self.objpoints = np.array(self.objpoints)
+        self.imgpoints = np.array(self.imgpoints)
+        return self.imgpoints, self.objpoints
+
+    def calibrate_camera(self, x_axis, y_axis):
+        """
+        Calibrate camera Intrinsic.
+
+        Args:
+            x_axis (list): X-axis coordinates.
+            y_axis (list): Y-axis coordinates.
+
+        Returns:
+            tuple: Calibration results (ret, mtx, dist).
+        """
+        self._process_reticle_points(x_axis, y_axis)
+        ret, self.mtx, self.dist, self.rvecs, self.tvecs = cv2.calibrateCamera(
+            self.objpoints,
+            self.imgpoints,
+            SIZE,
+            imtx,
+            idist,
+            flags=myflags1,
+            criteria=CRIT,
+        )
+
+        format_mtxt = (
+            "\n".join(
+                [" ".join([f"{val:.2f}" for val in row]) for row in self.mtx]
+            )
+            + "\n"
+        )
+        format_dist = " ".join([f"{val:.2f}" for val in self.dist[0]]) + "\n"
+        logger.debug(f"A reproj error: {ret}")
+        logger.debug(f"Intrinsic: {format_mtxt}\n")
+        logger.debug(f"Distortion: {format_dist}\n")
+        logger.debug(f"Focal length: {self.mtx[0][0]*1.85/1000}")
+        distancesA = [np.linalg.norm(vec) for vec in self.tvecs]
+        logger.debug(
+            f"Distance from camera to world center: {np.mean(distancesA)}"
+        )
+        return ret, self.mtx, self.dist
+
+    def get_predefined_intrinsic(self, x_axis, y_axis):
+        """
+        Fetches predefined intrinsic camera parameters for specific models.
+        Parameters:
+        - x_axis (int or float): The x-axis value for reticle processing.
+        - y_axis (int or float): The y-axis value for reticle processing.
+
+        Returns:
+        - A tuple of (bool, numpy.ndarray or None, numpy.ndarray or None) 
+        representing success status, intrinsic matrix, 
+        and distortion coefficients respectively.
+        """
+        self._process_reticle_points(x_axis, y_axis)
+        if self.name == "22517664":
+            self.mtx = np.array([[1.520480e+04, 0.0e+00, 2e+03],
+                [0.0e+00, 1.520480e+04, 1.5e+03],
+                [0.0e+00, 0.0e+00, 1.0e+00]],
+                dtype=np.float32)
+            self.dist = np.array([[-0.02, 8.26, -0.01, -0.00, -63.01]],
+                                dtype=np.float32)
+            return True, self.mtx, self.dist
+        
+        elif self.name == "22433200":
+            self.mtx = np.array([[1.507121e+04, 0.0e+00, 2e+03],
+                [0.0e+00, 1.507121e+04, 1.5e+03],
+                [0.0e+00, 0.0e+00, 1.0e+00]],
+                dtype=np.float32)
+            self.dist = np.array([[-0.02, 1.90, -0.00, -0.01, 200.94]],
+                                dtype=np.float32)
+            return True, self.mtx, self.dist
+        
+        else:
+            return False, None, None
+
+    def get_origin_xyz(self):
+        """
+        Get origin (0,0) and axis points (x, y, z coords) in image coordinates.
+
+        Returns:
+            tuple: Origin, x-axis, y-axis, z-axis points.
+        """
+        axis = np.float32([[3, 0, 0], [0, 3, 0], [0, 0, 3]]).reshape(-1, 3)
+        # Find the rotation and translation vectors.
+        # Output rotation vector (see Rodrigues ) that, together with tvec,
+        # brings points from the model coordinate system 
+        # to the camera coordinate system.
+        if self.objpoints is not None:
+            solvePnP_method = cv2.SOLVEPNP_ITERATIVE
+            _, rvecs, tvecs = cv2.solvePnP(
+                self.objpoints,
+                self.imgpoints,
+                self.mtx,
+                self.dist,
+                flags=solvePnP_method,
+            )
+            imgpts, _ = cv2.projectPoints(
+                axis, rvecs, tvecs, self.mtx, self.dist
+            )
+            origin = tuple(
+                self.imgpoints[0][CENTER_INDEX_X].ravel().astype(int)
+            )
+            x = tuple(imgpts[0].ravel().astype(int))
+            y = tuple(imgpts[1].ravel().astype(int))
+            z = tuple(imgpts[2].ravel().astype(int))
+            return origin, x, y, z
+        else:
+            return None
+
+
+class CalibrationStereo(CalibrationCamera):
+    """
+    Class for stereo camera calibration.
+    """
+
+    def __init__(
+        self, camA, imgpointsA, intrinsicA, camB, imgpointsB, intrinsicB):
+        """Initialize the CalibrationStereo object"""
+        self.n_interest_pixels = 15
+        self.camA = camA
+        self.camB = camB
+        self.imgpointsA, self.objpoints = self._process_reticle_points(
+            imgpointsA[0], imgpointsA[1])
+        self.imgpointsB, self.objpoints = self._process_reticle_points(
+            imgpointsB[0], imgpointsB[1])
+        self.mtxA, self.distA = intrinsicA[0], intrinsicA[1]
+        self.mtxB, self.distB = intrinsicB[0], intrinsicB[1]
+        self.criteria = (cv2.TERM_CRITERIA_EPS + cv2.TERM_CRITERIA_MAX_ITER, 100, 0.001)
+        self.flags = cv2.CALIB_FIX_INTRINSIC
+        self.retval, self.R_AB, self.T_AB, self.E_AB, self.F_AB = None, None, None, None, None 
+        self.P_A, self.P_B = None, None
+
+    def calibrate_stereo(self):
+        """Calibrate stereo cameras.
+
+        Returns:
+            tuple: Stereo calibration results (retval, R_AB, T_AB, E_AB, F_AB).
+        """
+        self.retval, _, _, _, _, self.R_AB, self.T_AB, self.E_AB, self.F_AB = (
+            cv2.stereoCalibrate(
+                self.objpoints,
+                self.imgpointsA,
+                self.imgpointsB,
+                self.mtxA,
+                self.distA,
+                self.mtxB,
+                self.distB,
+                SIZE,
+                criteria=self.criteria,
+                flags=self.flags,
+            )
+        )
+
+        print("\n== Stereo Calibration ==")
+        print("AB")
+        print(self.retval)
+        print(f"R: \n{self.R_AB}")
+        print(f"T: \n{self.T_AB}")
+        print(np.linalg.norm(self.T_AB))
+
+        formatted_F = (
+            "F_AB:\n"
+            + "\n".join(
+                [" ".join([f"{val:.5f}" for val in row]) for row in self.F_AB]
+            ) + "\n")
+        formatted_E = (
+            "E_AB:\n"
+            + "\n".join(
+                [" ".join([f"{val:.5f}" for val in row]) for row in self.E_AB]
+            ) + "\n")
+        print(formatted_F)
+        print(formatted_E)
+
+        self.P_A = self.mtxA @ np.hstack((np.eye(3), np.zeros((3, 1))))
+        self.P_B = self.mtxB @ np.hstack((self.R_AB, self.T_AB.reshape(-1, 1)))
+
+        return self.retval, self.R_AB, self.T_AB, self.E_AB, self.F_AB
+
+    def _matching_camera_order(self, camA, coordA, camB, coordB):
+        """Match camera order based on initialization order.
+
+        Args:
+            camA (str): Camera A name.
+            coordA (tuple): Coordinates from camera A.
+            camB (str): Camera B name.
+            coordB (tuple): Coordinates from camera B.
+
+        Returns:
+            tuple: Matched camera order and coordinates.
+        """
+        if self.camA == camA:
+            return camA, coordA, camB, coordB
+
+        if self.camA == camB:
+            return camB, coordB, camA, coordA
+
+    def triangulation(self, P_1, P_2, imgpoints_1, imgpoints_2):
+        """Triangulate 3D points from stereo image points.
+
+        Args:
+            P_1 (numpy.ndarray): Projection matrix of camera 1.
+            P_2 (numpy.ndarray): Projection matrix of camera 2.
+            imgpoints_1 (numpy.ndarray): Image points from camera 1.
+            imgpoints_2 (numpy.ndarray): Image points from camera 2.
+
+        Returns:
+            numpy.ndarray: Triangulated 3D points.
+        """
+        points_4d_hom = cv2.triangulatePoints(
+            P_1, P_2, imgpoints_1.T, imgpoints_2.T
+        )
+        points_3d_hom = points_4d_hom / points_4d_hom[3]
+        points_3d_hom = points_3d_hom.T
+        return points_3d_hom[:, :3]
+
+    def change_coords_system_from_camA_to_global(self, points_3d_AB):
+        """
+        Change coordinate system from camera A to global using solvePnPRansac.
+
+        Args:
+            points_3d_AB (numpy.ndarray):
+            3D points in camera A coordinate system.
+
+        Returns:
+            numpy.ndarray: 3D points in global coordinate system.
+        """
+        _, rvecs, tvecs, _ = cv2.solvePnPRansac(
+            self.objpoints, self.imgpointsA, self.mtxA, self.distA
+        )
+        # Convert rotation vectors to rotation matrices
+        rmat, _ = cv2.Rodrigues(rvecs)
+        # Invert the rotation and translation
+        rmat_inv = rmat.T  # Transpose of rotation matrix is its inverse
+        tvecs_inv = -rmat_inv @ tvecs
+        # Transform the points
+        points_3d_G = np.dot(rmat_inv, points_3d_AB.T).T + tvecs_inv.T
+        return points_3d_G
+
+    def change_coords_system_from_camA_to_global_iterative(self, points_3d_AB):
+        """Change coordinate system from camera A to global 
+        using iterative method.
+
+        Args:
+            points_3d_AB (numpy.ndarray):
+            3D points in camera A coordinate system.
+
+        Returns:
+            numpy.ndarray: 3D points in global coordinate system.
+        """
+        solvePnP_method = cv2.SOLVEPNP_ITERATIVE
+        _, rvecs, tvecs = cv2.solvePnP(
+            self.objpoints,
+            self.imgpointsA,
+            self.mtxA,
+            self.distA,
+            flags=solvePnP_method,
+        )
+        logger.debug("solvePnP")
+        logger.debug(rvecs)
+        logger.debug(tvecs)
+        # Convert rotation vectors to rotation matrices
+        rmat, _ = cv2.Rodrigues(rvecs)
+        # Invert the rotation and translation
+        self.rmat_inv = rmat.T  # Transpose of rotation matrix is its inverse
+        self.tvecs_inv = -self.rmat_inv @ tvecs
+        # Transform the points
+        points_3d_G = np.dot(self.rmat_inv, points_3d_AB.T).T + self.tvecs_inv.T
+        return points_3d_G
+
+    def change_coords_system_from_camA_to_global_savedRT(self, points_3d_AB):
+        """Change coordinate system from camera A to global
+        using saved rotation and translation.
+
+        Args:
+            points_3d_AB (numpy.ndarray):
+            3D points in camera A coordinate system.
+
+        Returns:
+            numpy.ndarray: 3D points in global coordinate system.
+        """
+        points_3d_G = np.dot(self.rmat_inv, points_3d_AB.T).T + self.tvecs_inv.T
+        return points_3d_G
+
+    def get_global_coords(self, camA, coordA, camB, coordB):
+        """Get global coordinates from stereo image coordinates.
+
+        Args:
+            camA (str): Camera A name.
+            coordA (tuple): Coordinates from camera A.
+            camB (str): Camera B name.
+            coordB (tuple): Coordinates from camera B.
+
+        Returns:
+            numpy.ndarray: 3D points in global coordinate system.
+        """
+        camA, coordA, camB, coordB = self._matching_camera_order(
+            camA, coordA, camB, coordB
+        )
+        coordA = np.array(coordA).astype(np.float32)
+        coordB = np.array(coordB).astype(np.float32)
+        points_3d_AB = self.triangulation(self.P_B, self.P_A, coordB, coordA)
+        points_3d_G = self.change_coords_system_from_camA_to_global_savedRT(
+            points_3d_AB
+        )
+
+        logger.debug(
+            f"points_3d_G: {points_3d_G}, coordA: {coordA}, coordB: {coordB}"
+        )
+        return points_3d_G
+
+    def test_x_y_z_performance(self, points_3d_G):
+        # Calculate the differences for each dimension
+        differences_x = points_3d_G[:, 0] - self.objpoints[0, :, 0]
+        differences_y = points_3d_G[:, 1] - self.objpoints[0, :, 1]
+        differences_z = points_3d_G[:, 2] - self.objpoints[0, :, 2]
+
+        # Calculate the mean squared differences for each dimension
+        mean_squared_diff_x = np.mean(np.square(differences_x))
+        mean_squared_diff_y = np.mean(np.square(differences_y))
+        mean_squared_diff_z = np.mean(np.square(differences_z))
+
+        # Calculate the L2 norm (Euclidean distance) for each dimension
+        l2_x = np.sqrt(mean_squared_diff_x)
+        l2_y = np.sqrt(mean_squared_diff_y)
+        l2_z = np.sqrt(mean_squared_diff_z)
+
+        print(
+            f"x: {l2_x*1000}µm³, y: {l2_y*1000}µm³, z:{l2_z*1000}µm³"
+        )
+
+    def test_performance(self, camA, coordA, camB, coordB):
+        """Test stereo calibration.
+
+        Args:
+            camA (str): Camera A name.
+            coordA (tuple): Coordinates from camera A.
+            camB (str): Camera B name.
+            coordB (tuple): Coordinates from camera B.
+
+        Returns:
+            numpy.ndarray: Predicted 3D points in global coordinate system.
+        """
+        camA, coordA, camB, coordB = self._matching_camera_order(
+            camA, coordA, camB, coordB
+        )
+        logger.debug(f"coordA: {coordA}")
+        logger.debug(f"coordB: {coordB}")
+        points_3d_AB = self.triangulation(
+            self.P_B, self.P_A, self.imgpointsB, self.imgpointsA
+        )
+        np.set_printoptions(suppress=True, precision=8)
+
+        points_3d_G = self.change_coords_system_from_camA_to_global_iterative(
+            points_3d_AB
+        )
+        print("\n=solvePnP SOLVEPNP_ITERATIVE=")
+        differences = points_3d_G - self.objpoints[0]
+        squared_distances = np.sum(np.square(differences), axis=1)
+        euclidean_distances = np.sqrt(squared_distances)
+        average_L2_distance = np.mean(euclidean_distances)
+        print(
+            f"(Reprojection error) Object points L2 diff: \
+            {average_L2_distance*1000} µm³"
+        )
+        self.test_x_y_z_performance(points_3d_G)
+        print(f"Object points predict:\n{np.around(points_3d_G, decimals=5)}")
+
+        self.test_pixel_error()
+        return average_L2_distance
+
+    def test_pixel_error(self):
+        """Test pixel reprojection error."""
+        mean_error = 0
+        for i in range(len(self.objpoints)):
+            imgpointsA_converted = np.array(
+                self.imgpointsA[i], dtype=np.float32
+            ).reshape(-1, 2)
+            solvePnP_method = cv2.SOLVEPNP_ITERATIVE
+            retval, rvecs, tvecs = cv2.solvePnP(
+                self.objpoints[i],
+                imgpointsA_converted,
+                self.mtxA,
+                self.distA,
+                flags=solvePnP_method,
+            )
+            imgpoints2, _ = cv2.projectPoints(
+                self.objpoints[i], rvecs, tvecs, self.mtxA, self.distA
+            )
+
+            imgpoints2_reshaped = imgpoints2.reshape(-1, 2)
+            differences = imgpointsA_converted - imgpoints2_reshaped
+            squared_distances = np.sum(np.square(differences), axis=1)
+            distances = np.sqrt(squared_distances)
+            average_L2_distance = np.mean(distances)
+            mean_error += average_L2_distance
+            logger.debug("A pixel diff")
+            logger.debug(imgpointsA_converted-imgpoints2_reshaped)
+        total_err = mean_error / len(self.objpoints)
+        print(f"(Reprojection error) Pixel L2 diff A: {total_err} pixels")
+
+        mean_error = 0
+        for i in range(len(self.objpoints)):
+            imgpointsB_converted = np.array(
+                self.imgpointsB[i], dtype=np.float32
+            ).reshape(-1, 2)
+            solvePnP_method = cv2.SOLVEPNP_ITERATIVE
+            retval, rvecs, tvecs = cv2.solvePnP(
+                self.objpoints[i],
+                imgpointsB_converted,
+                self.mtxB,
+                self.distB,
+                flags=solvePnP_method,
+            )
+            imgpoints2, _ = cv2.projectPoints(
+                self.objpoints[i], rvecs, tvecs, self.mtxB, self.distB
+            )
+
+            imgpoints2_reshaped = imgpoints2.reshape(-1, 2)
+            differences = imgpointsB_converted - imgpoints2_reshaped
+            distances = np.sqrt(np.sum(np.square(differences), axis=1))
+            average_L2_distance = np.mean(distances)
+            mean_error += average_L2_distance
+            logger.debug("B pixel diff")
+            logger.debug(imgpointsB_converted - imgpoints2_reshaped)
+
+        total_err = mean_error / len(self.objpoints)
+        print(f"(Reprojection error) Pixel L2 diff B: {total_err} pixels")
```

### Comparing `parallax_app-0.37.1/parallax/camera.py` & `parallax_app-0.37.5/parallax/camera.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,827 +1,827 @@
-"""
-PySpinCamera: A class to interface with cameras using the PySpin library.
-"""
-
-import datetime
-import logging
-import os
-import threading
-import time
-
-import cv2
-import numpy as np
-
-# Initialize the logger
-logger = logging.getLogger(__name__)
-supported_camera_models = ["BFS-U3-120S4C", "BFS-U3-04S2M"]
-
-# Check for the availability of the PySpin library
-try:
-    import PySpin
-except ImportError:
-    PySpin = None
-    logger.warn("Could not import PySpin.")
-
-
-def list_cameras(dummy=False, version="V1"):
-    """
-    List available cameras.
-
-    Parameters:
-    - dummy (bool): If True, lists only mock cameras. Default is False.
-
-    Returns:
-    - list: List of available PySpin cameras.
-    """
-    # Init version, V1: original, V2: WIP with new GUI
-    global VERSION
-    VERSION = version
-
-    global pyspin_cameras, pyspin_instance
-    cameras = []
-    if not dummy:
-        if PySpin is not None:
-            cameras.extend(PySpinCamera.list_cameras())
-    return cameras
-
-
-def close_cameras():
-    """Close all available cameras."""
-    if PySpin is not None:
-        PySpinCamera.close_cameras()
-
-
-class PySpinCamera:
-    """
-    Represents a camera managed by the PySpin library.
-    """
-
-    pyspin_cameras = None
-    pyspin_instance = None
-    cameras = []
-
-    @classmethod
-    def list_cameras(cls):
-        """
-        List available PySpin cameras.
-
-        Returns:
-        - list: List of available PySpin cameras.
-        """
-        if cls.pyspin_instance is None:
-            cls.pyspin_instance = PySpin.System.GetInstance()
-        cls.pyspin_cameras = cls.pyspin_instance.GetCameras()
-        ncameras = cls.pyspin_cameras.GetSize()
-
-        cls.cameras = []
-        for i in range(ncameras):
-            camera_pyspin = cls.pyspin_cameras.GetByIndex(i)
-            camera = PySpinCamera(camera_pyspin)
-            if camera is not None:
-                cls.cameras.append(camera)
-            else:
-                camera.stop(clean=True)
-
-        return cls.cameras
-
-    # Class method to close all PySpin cameras
-    @classmethod
-    def close_cameras(cls):
-        """
-        Release resources and close all PySpin cameras.
-        """
-        logger.info("cleaning up SpinSDK")
-        for camera in cls.cameras:
-            camera.stop(clean=True)
-        if cls.pyspin_cameras is not None:
-            cls.pyspin_cameras.Clear()
-        if cls.pyspin_instance is not None:
-            cls.pyspin_instance.ReleaseInstance()
-
-    # Constructor for PySpinCamera
-    def __init__(self, camera_pyspin):
-        """
-        Initialize a PySpinCamera instance.
-
-        Parameters:
-        - camera_pyspin: The underlying PySpin camera object.
-        """
-        self.running = False
-        self.camera = camera_pyspin
-        self.tldnm = self.camera.GetTLDeviceNodeMap()
-        self.camera.Init()
-        self.node_map = self.camera.GetNodeMap()
-
-        self.last_image = None
-        self.last_image_filled = threading.Event()
-        self.last_image_cleared = threading.Event()
-
-        self.video_output = None
-        self.video_recording_on = threading.Event()
-        self.video_recording_idle = threading.Event()
-        self.height = None
-        self.width = None
-        self.channels = None
-        self.frame_rate = None
-
-        self.device_model = self.camera.DeviceModelName()
-        self.device_color_type = None
-        camera_color_type = self.device_model.split("-")[2][-1]
-        if camera_color_type == "M":
-            self.device_color_type = "Mono"
-        elif camera_color_type == "C":
-            self.device_color_type = "Color"
-        elif camera_color_type == "P":
-            self.device_color_type = "Polarized"
-            print("Polarized Camera model not supported.")
-            return None
-        else:
-            print("Not supported camera type.")
-            return None
-        print(
-            self.device_model, self.device_color_type, self.name(sn_only=True)
-        )
-
-        # set BufferHandlingMode to NewestOnly (necessary to update the image)
-        s_nodemap = self.camera.GetTLStreamNodeMap()
-        node_bufferhandling_mode = PySpin.CEnumerationPtr(
-            s_nodemap.GetNode("StreamBufferHandlingMode")
-        )
-        node_newestonly = node_bufferhandling_mode.GetEntryByName("NewestOnly")
-        node_newestonly_mode = node_newestonly.GetValue()
-        node_bufferhandling_mode.SetIntValue(node_newestonly_mode)
-
-        # Set White Balance
-        if self.device_color_type == "Color":
-            self.node_wbauto_mode = PySpin.CEnumerationPtr(
-                self.node_map.GetNode("BalanceWhiteAuto")
-            )
-            self.node_wbauto_mode_off = self.node_wbauto_mode.GetEntryByName(
-                "Off"
-            )
-            self.node_wbauto_mode_on = self.node_wbauto_mode.GetEntryByName(
-                "Continuous"
-            )
-            self.node_wbauto_mode.SetIntValue(
-                self.node_wbauto_mode_on.GetValue()
-            )  # Default: Auto mode on
-            self.node_balanceratio_mode = PySpin.CEnumerationPtr(
-                self.node_map.GetNode("BalanceRatioSelector")
-            )
-            self.node_wb = PySpin.CFloatPtr(
-                self.node_map.GetNode("BalanceRatio")
-            )
-            self.node_balanceratio_mode_red = (
-                self.node_balanceratio_mode.GetEntryByName("Red")
-            )  # Red Channel
-            self.node_balanceratio_mode_blue = (
-                self.node_balanceratio_mode.GetEntryByName("Blue")
-            )  # Blue Channel
-
-        # set exposure time
-        self.node_expauto_mode = PySpin.CEnumerationPtr(
-            self.node_map.GetNode("ExposureAuto")
-        )
-        self.node_expauto_mode_off = self.node_expauto_mode.GetEntryByName(
-            "Off"
-        )
-        self.node_expauto_mode_on = self.node_expauto_mode.GetEntryByName(
-            "Continuous"
-        )
-        self.node_expauto_mode.SetIntValue(
-            self.node_expauto_mode_on.GetValue()
-        )  # Default: Auto mode on
-        self.node_exptime = PySpin.CFloatPtr(
-            self.node_map.GetNode("ExposureTime")
-        )
-
-        # set gain
-        self.node_gainauto_mode = PySpin.CEnumerationPtr(
-            self.node_map.GetNode("GainAuto")
-        )
-        self.node_gainauto_mode_off = self.node_gainauto_mode.GetEntryByName(
-            "Off"
-        )
-        self.node_gainauto_mode_on = self.node_gainauto_mode.GetEntryByName(
-            "Continuous"
-        )
-        self.node_gain = PySpin.CFloatPtr(self.node_map.GetNode("Gain"))
-        self.node_gainauto_mode.SetIntValue(
-            self.node_gainauto_mode_on.GetValue()
-        )  # Default: Auto mode on
-
-        # set gamma
-        self.node_gammaenable_mode = PySpin.CBooleanPtr(
-            self.node_map.GetNode("GammaEnable")
-        )
-        self.node_gammaenable_mode.SetValue(True)  # Default: Gammal Enable on
-        self.node_gamma = PySpin.CFloatPtr(self.node_map.GetNode("Gamma"))
-        self.node_gamma.SetValue(0.8)
-
-        # set pixel format
-        node_pixelformat = PySpin.CEnumerationPtr(
-            self.node_map.GetNode("PixelFormat")
-        )
-        self.pixelformat = None
-        if self.device_color_type == "Mono":
-            self.pixelformat = "Mono"
-            entry_pixelformat_mono8 = node_pixelformat.GetEntryByName("Mono8")
-            node_pixelformat.SetIntValue(entry_pixelformat_mono8.GetValue())
-        elif self.device_color_type == "Color":
-            self.pixelformat = "BayerRG8"
-            entry_pixelformat_bayerRG8 = node_pixelformat.GetEntryByName(
-                "BayerRG8"
-            )
-            node_pixelformat.SetIntValue(entry_pixelformat_bayerRG8.GetValue())
-
-        # acquisition on initialization
-        if VERSION == "V1":
-            # begin acquisition
-            # V1: Start continuous acquisition on initialization.
-            self.begin_continuous_acquisition()
-        elif VERSION == "V2":
-            # V2: Start continuous acquisition when 'Start' button is toggled and end acquisition when untoggled.
-            # On initialization, start onetime acquisition to get one frame.
-            pass
-
-    def set_wb(self, channel, wb=1.2):
-        """
-        Sets the white balance of the camera.
-
-        Args:
-        - wb (float): The desired white balance value. min:1.8, max:2.5
-        """
-        if self.device_color_type == "Color":
-            self.node_wbauto_mode.SetIntValue(
-                self.node_wbauto_mode_off.GetValue()
-            )
-            if channel == "Red":
-                self.node_balanceratio_mode.SetIntValue(
-                    self.node_balanceratio_mode_red.GetValue()
-                )
-                self.node_wb.SetValue(wb)
-            elif channel == "Blue":
-                self.node_balanceratio_mode.SetIntValue(
-                    self.node_balanceratio_mode_blue.GetValue()
-                )
-                self.node_wb.SetValue(wb)
-        else:
-            pass
-
-    def get_wb(self, channel):
-        """
-        Get the gamma of the camera for the auto mode.
-        """
-        if self.device_color_type == "Color":
-            self.node_wbauto_mode.SetIntValue(
-                self.node_wbauto_mode_on.GetValue()
-            )  # Set continuous for mono camera
-            time.sleep(0.5)
-            if channel == "Red":
-                self.node_balanceratio_mode.SetIntValue(
-                    self.node_balanceratio_mode_red.GetValue()
-                )
-                time.sleep(0.5)
-                return self.node_wb.GetValue()
-            elif channel == "Blue":
-                self.node_balanceratio_mode.SetIntValue(
-                    self.node_balanceratio_mode_blue.GetValue()
-                )
-                time.sleep(0.5)
-                return self.node_wb.GetValue()
-        else:
-            return -1
-
-    def set_gamma(self, gamma=1.0):
-        """
-        Sets the gamma correction of the camera.
-
-        Args:
-        - gamma (float): The desired gamma value. min:0.25 max:1.25
-        """
-        self.node_gammaenable_mode.SetValue(True)
-        self.node_gamma.SetValue(gamma)
-
-    def disable_gamma(self):
-        """
-        Disable the gamma of the camera.
-        """
-        self.node_gammaenable_mode.SetValue(False)
-
-    def set_gain(self, gain=20.0):
-        """
-        Sets the gain of the camera.
-
-        Args:
-        - gain (float): The desired gain value. min:0, max:27.0
-        """
-        self.node_gainauto_mode.SetIntValue(
-            self.node_gainauto_mode_off.GetValue()
-        )
-        self.node_gain.SetValue(gain)
-
-    def get_gain(self):
-        """
-        Get the gain of the camera for the auto mode.
-        """
-        initial_val = self.node_gain.GetValue()
-        self.node_gainauto_mode.SetIntValue(
-            self.node_gainauto_mode_on.GetValue()
-        )  # Set continuous for mono camera
-
-        time.sleep(0.5)  # Wait for a short period
-        updated_val = self.node_gain.GetValue()
-        if updated_val != initial_val:
-            return updated_val  # Return the updated value if there's a change
-
-        return initial_val  # Return the initial value if no change is detected
-
-    def set_exposure(self, expTime=16000):
-        """
-        Sets the exposure time of the camera.
-
-        Args:
-        - expTime (int): The desired exposure time in microseconds.
-        """
-        self.node_expauto_mode.SetIntValue(
-            self.node_expauto_mode_off.GetValue()
-        )  # Return back to manual mode
-        self.node_exptime.SetValue(expTime)
-
-    def get_exposure(self):
-        """
-        Get the exposure time of the camera for the auto mode.
-        """
-        initial_val = self.node_exptime.GetValue()
-        self.node_expauto_mode.SetIntValue(
-            self.node_expauto_mode_on.GetValue()
-        )  # Enable the Auto mode
-
-        time.sleep(0.5)  # Wait for a short period
-        updated_val = self.node_exptime.GetValue()
-        if updated_val != initial_val:
-            return updated_val  # Return the updated value if there's a change
-
-        return initial_val  # Return the initial value if no change is detected
-
-    def name(self, sn_only=False):
-        """
-        Retrieves the name and serial number of the camera.
-
-        Args:
-        - sn_only (bool): Whether to return only the serial number.
-
-        Returns:
-        - str: The device model and serial number or just the serial number.
-        """
-        sn = self.camera.DeviceSerialNumber()
-        device_model = self.camera.DeviceModelName()
-        if sn_only:
-            return sn
-        else:
-            return "%s (Serial # %s)" % (device_model, sn)
-
-    def begin_singleframe_acquisition(self):
-        """
-        Begings a single Frame image acquisition.
-        """
-        # set acquisition mode to singleFrame
-        node_acquisition_mode = PySpin.CEnumerationPtr(
-            self.node_map.GetNode("AcquisitionMode")
-        )
-        node_acquisition_mode_singleframe = (
-            node_acquisition_mode.GetEntryByName("SingleFrame")
-        )
-        acquisition_mode_singleframe = (
-            node_acquisition_mode_singleframe.GetValue()
-        )
-        node_acquisition_mode.SetIntValue(acquisition_mode_singleframe)
-
-        # Begin Acquisition: Image acquisition must be ended when no more images are needed.
-        self.camera.BeginAcquisition()
-        print(f"Begin Single Frame Acquisition {self.name(sn_only=True)} ")
-        self.capture_thread = threading.Thread(
-            target=self.capture, daemon=False
-        )
-        self.capture_thread.start()
-
-    def end_singleframe_acquisition(self):
-        """End Acquisition"""
-        self.last_image_cleared.wait()
-        self.capture_thread.join()
-        self.camera.EndAcquisition()
-        self.last_image = None
-        self.last_image_cleared.clear()
-        self.last_image_filled.clear()
-
-    def begin_continuous_acquisition(self):
-        """
-        Begins the image acquisition process in continuous mode and starts the capture loop in a separate thread.
-        """
-        if self.running:
-            print("Error: camera is already running")
-            return -1
-
-        # set acquisition mode continuous (continuous stream of images)
-        node_acquisition_mode = PySpin.CEnumerationPtr(
-            self.node_map.GetNode("AcquisitionMode")
-        )
-        node_acquisition_mode_continuous = node_acquisition_mode.GetEntryByName(
-            "Continuous"
-        )
-        acquisition_mode_continuous = (
-            node_acquisition_mode_continuous.GetValue()
-        )
-        node_acquisition_mode.SetIntValue(acquisition_mode_continuous)
-
-        # Begin Acquisition: Image acquisition must be ended when no more images are needed.
-        self.camera.BeginAcquisition()
-        logger.debug(f"BeginAcquisition {self.name(sn_only=True)} ")
-        self.running = True
-        self.capture_thread = threading.Thread(
-            target=self.capture_loop, daemon=True
-        )
-        self.capture_thread.start()
-
-    def capture_loop(self):
-        """
-        Continuous loop to capture images while the camera is running.
-        """
-        while self.running:
-            self.capture()
-            # print(".", end="",flush=True)
-
-    def capture(self):
-        """
-        Captures an image and checks for its completeness.
-        If video recording is enabled, writes the image to the video file.
-
-        *** NOTES ***
-        Capturing an image houses images on the camera buffer.
-        Trying to capture an image that does not exist will hang the camera.
-        Using-statements help ensure that images are released.
-        If too many images remain unreleased, the buffer will fill,
-        causing the camera to hang.
-        Images can also be released manually by calling Release().
-        """
-        # Timestamp for the current capture
-        ts = time.time()
-        self.last_capture_time = ts
-
-        # Retrieve the next image from the camera
-        image = self.camera.GetNextImage(1000)
-
-        while image.IsIncomplete():
-            time.sleep(0.001)
-
-        # Release the previous image from the buffer if it exists
-        if self.last_image is not None:
-            try:
-                self.last_image.Release()
-            except PySpin.SpinnakerException:
-                print("Spinnaker Exception: Couldn't release last image")
-
-        # Update the last captured image reference
-        self.last_image = image
-        self.last_image_filled.set()
-
-        # Record the image if video recording is active
-        if self.video_recording_on.is_set():
-            self.video_recording_idle.clear()
-
-            frame = self.get_last_image_data()
-            frame = cv2.cvtColor(frame, cv2.COLOR_RGB2BGR)
-
-            self.video_output.write(frame)
-            self.video_recording_idle.set()
-
-    def get_last_capture_time(self, millisecond=False):
-        """
-        Returns the timestamp of the last captured image in a formatted string.
-
-        Returns:
-        - str: Timestamp in the format 'YYYYMMDD-HHMMSS'.
-        """
-        ts = self.last_capture_time
-        dt = datetime.datetime.fromtimestamp(ts)
-        if millisecond:
-            return "%04d%02d%02d-%02d%02d%02d.%03d" % (
-                dt.year,
-                dt.month,
-                dt.day,
-                dt.hour,
-                dt.minute,
-                dt.second,
-                dt.microsecond // 1000,
-            )
-        else:
-            return "%04d%02d%02d-%02d%02d%02d" % (
-                dt.year,
-                dt.month,
-                dt.day,
-                dt.hour,
-                dt.minute,
-                dt.second,
-            )
-
-    def save_last_image(
-        self, filepath, isTimestamp=False, custom_name="Microscope_"
-    ):
-        """
-        Saves the last captured image to the specified file path.
-
-        Args:
-        - filepath (str): Directory to save the image.
-        - isTimestamp (bool): Whether to append a timestamp to the filename.
-        - custom_name (str): Custom prefix for the filename. 
-        S/N is set as custom name.
-        """
-        image_name = (
-            "{}_{}.png".format(custom_name, self.get_last_capture_time())
-            if isTimestamp
-            else "{}.png".format(custom_name)
-        )
-        full_path = os.path.join(filepath, image_name)
-        logger.debug(f"Saving image to {full_path}")
-        print(f"Saving image to {full_path}")
-
-        # Save the image
-        try:
-            image_converted = self.get_last_image_data()
-            if image_converted is not None:
-                # Convert the image from RGB to BGR
-                image_converted = cv2.cvtColor(
-                    image_converted, cv2.COLOR_RGB2BGR
-                )
-                cv2.imwrite(full_path, image_converted)
-            else:
-                logger.error("Image not found or couldn't be retrieved.")
-        except Exception as e:
-            logger.error(f"An error occurred while saving the image: {e}")
-
-    def get_last_image(self):
-        """
-        Returns the last captured image.
-
-        Returns:
-        - PySpin.Image: The last captured image.
-        """
-        return self.last_image
-
-    # Get the last captured image data as a numpy array
-    def get_last_image_data(self):
-        """
-        Returns the last captured image data as a numpy array.
-        Shape: (height, width, 3) for RGB,  (height, width) for mono
-
-        Returns:
-        - numpy.ndarray: Image data in array format.
-        """
-        # Wait until last_image is not None
-        self.last_image_filled.wait()
-        frame_image = self.last_image.GetNDArray()
-        if self.pixelformat == "BayerRG8":
-            frame_image = cv2.cvtColor(frame_image, cv2.COLOR_BayerRG2BGR)
-        return frame_image
-
-    # Get the last captured image data as a numpy array
-    def get_last_image_data_singleFrame(self):
-        """
-        Returns the last captured image data as a numpy array.
-        Shape: (height, width, 3) for RGB,  (height, width) for mono
-
-        Returns:
-        - numpy.ndarray: Image data in array format.
-        """
-        # Wait until last_image is not None
-        self.last_image_filled.wait()
-        frame_image = self.last_image.GetNDArray()
-        if self.pixelformat == "BayerRG8":
-            frame_image = cv2.cvtColor(frame_image, cv2.COLOR_BayerRG2BGR)
-        self.last_image_cleared.set()
-        return frame_image
-
-    def camera_info(self):
-        """
-        Retrieves and logs the camera's essential information 
-        such as frame dimensions and channels.
-        """
-        # Gather camera details
-        self.height = self.camera.Height()
-        self.width = self.camera.Width()
-        try:
-            if self.last_image is not None:
-                self.channels = self.last_image.GetNumChannels()
-        except Exception as e:
-            logger.error(f"An error occurred while getting channel info: {e}")
-        logger.info(
-            f"camera frame width: {self.width}, height: {self.width}, channels: {self.channels}"
-        )
-
-        # Set frame rate equal to the current acquisition frame rate (Hz)
-        nodeFramerate = PySpin.CFloatPtr(
-            self.node_map.GetNode("AcquisitionFrameRate")
-        )
-        if (not PySpin.IsAvailable(nodeFramerate)) or (
-            not PySpin.IsReadable(nodeFramerate)
-        ):
-            logger.error("Unable to retrieve frame rate. Aborting...")
-            return -1
-        self.frame_rate = nodeFramerate.GetValue()
-        logger.info(f"Frame rate to be set to {self.frame_rate}")
-
-    def save_recording(
-        self, filepath, isTimestamp=False, custom_name="Microscope_"
-    ):
-        """
-        Begins video recording and saves the video to the specified file path.
-
-        Args:
-        - filepath (str): Directory to save the video.
-        - isTimestamp (bool): Whether to append a timestamp to the filename.
-        - custom_name (str): Custom prefix for the filename.
-        """
-        # Formulate the video name based on the input parameters
-        video_name = (
-            "{}_{}.avi".format(custom_name, self.get_last_capture_time())
-            if isTimestamp
-            else "{}.avi".format(custom_name)
-        )
-        full_path = os.path.join(filepath, video_name)
-        print(f"Saving video to {full_path}")
-        logger.debug(f"Try saving video to {full_path}")
-
-        # Update camera details
-        self.camera_info()
-
-        # Begin the video recording with appropriate configurations
-        fourcc = cv2.VideoWriter_fourcc(*"XVID")
-        self.video_output = cv2.VideoWriter(
-            full_path, fourcc, self.frame_rate, (self.width, self.height), True
-        )
-        self.video_recording_on.set()
-
-    def stop_recording(self):
-        """
-        Stops the ongoing video capture process and releases video resources.
-        """
-        self.video_recording_on.clear()
-        self.video_recording_idle.wait()
-        self.video_recording_idle.clear()
-        self.video_output.release()
-
-    # Clean up the camera
-    def stop(self, clean=False):
-        """
-        Cleans up resources associated with the camera and video recording.
-
-        Note:
-            Do not change the order of codes without referring PySpin manual.
-            They are ordered by PySpin Camera Init / Turn off sequence.
-        """
-        if self.running:
-            self.running = False
-            self.capture_thread.join()
-            self.camera.EndAcquisition()
-            self.last_image = None
-            self.last_image_filled.clear()
-
-        if self.video_recording_on.is_set():
-            self.stop_recording()
-
-        if clean:
-            del self.camera
-
-
-# Class for simulating a mock camera
-class MockCamera:
-    """Mock Camera showing salts and pepper noise images"""
-
-    n_cameras = 0
-
-    def __init__(self):
-        """Initialize a mock camera with a unique name"""
-        self._name = f"MockCamera{MockCamera.n_cameras}"
-        MockCamera.n_cameras += 1
-        # Create mock image data with random values
-        self.data = np.random.randint(
-            0, 255, size=(5, 3000, 4000), dtype="ubyte"
-        )
-        self._next_frame = 0
-        self.device_color_type = None
-
-    def name(self, sn_only=False):
-        """Get the name of the mock camera"""
-        return self._name
-
-    def get_last_image_data(self):
-        """
-        Return last image as numpy array with shape (height, width, 3) for RGB
-		or (height, width) for mono.
-        """
-        frame = self.data[self._next_frame]
-        self._next_frame = (self._next_frame + 1) % self.data.shape[0]
-        return frame
-
-    def save_last_image(
-        self, filepath, isTimestamp=False, custom_name="MockCamera_"
-    ):
-        """Dummy function"""
-        print("This is MockCamera. Cannot capture the image")
-        return
-
-    def set_wb(self, wb=2.0):
-        """Dummy function"""
-        logger.info("This is MockCamera. Setting is not applicable")
-        return
-
-    def set_gamma(self, gamma=1.0):
-        """Dummy function"""
-        logger.info("This is MockCamera. Setting is not applicable")
-        return
-
-    def set_gain(self, gain=25.0):
-        """Dummy function"""
-        logger.info("This is MockCamera. Setting is not applicable")
-        return
-
-    def set_exposure(self, expTime=16000):
-        """Dummy function"""
-        logger.info("This is MockCamera. Setting is not applicable")
-        return
-
-    def stop(self, clean=False):
-        """Dummy function"""
-        logger.info("This is MockCamera. Stop")
-        return
-
-    def begin_continuous_acquisition(self):
-        """Dummy function"""
-        return
-
-    def get_last_capture_time(self, millisecond=False):
-        """Dummy function"""
-        return
-
-    def stop(self, clean=False):
-        """Dummy function"""
-        return
-
-
-class VideoSource:
-    """Video Source"""
-
-    def __init__(self, filename):
-        """Initialize a video source with a given filename"""
-        self.filename = filename
-        self._name = os.path.basename(self.filename)
-        self.cap = cv2.VideoCapture(self.filename)
-
-    def name(self, sn_only=False):
-        """Get the name of the video source"""
-        return self._name
-
-    def get_last_image_data(self):
-        """Read the last captured frame from the video source"""
-        ret, frame = self.cap.read()
-        if ret:
-            return frame
-        else:
-            # If the video has ended, reset the video source to the beginning
-            self.cap.set(cv2.CAP_PROP_POS_FRAMES, 0)
-            return np.random.randint(0, 255, size=(3000, 4000), dtype="ubyte")
-
-    def save_last_image(
-        self, filepath, isTimestamp=False, custom_name="VideoSource_"
-    ):
-        """Dummy function"""
-        print("This is from Video Source. Cannot capture the image")
-        return
-
-    def set_wb(self, wb=2.0):
-        """Dummy function"""
-        logger.info("This is VideoSource. Setting is not applicable")
-        return
-
-    def set_gamma(self, gamma=1.0):
-        """Dummy function"""
-        logger.info("This is VideoSource. Setting is not applicable")
-        return
-
-    def set_gain(self, gain=25.0):
-        """Dummy function"""
-        logger.info("This is VideoSource. Setting is not applicable")
-        return
-
-    def set_exposure(self, expTime=125000):
-        """Dummy function"""
-        logger.info("This is VideoSource. Setting is not applicable")
-        return
-
-    def begin_continuous_acquisition(self):
-        """Dummy function"""
-        return
-
-    def stop(self, clean=False):
-        """Dummy function"""
-        return
+"""
+PySpinCamera: A class to interface with cameras using the PySpin library.
+"""
+
+import datetime
+import logging
+import os
+import threading
+import time
+
+import cv2
+import numpy as np
+
+# Initialize the logger
+logger = logging.getLogger(__name__)
+supported_camera_models = ["BFS-U3-120S4C", "BFS-U3-04S2M"]
+
+# Check for the availability of the PySpin library
+try:
+    import PySpin
+except ImportError:
+    PySpin = None
+    logger.warn("Could not import PySpin.")
+
+
+def list_cameras(dummy=False, version="V1"):
+    """
+    List available cameras.
+
+    Parameters:
+    - dummy (bool): If True, lists only mock cameras. Default is False.
+
+    Returns:
+    - list: List of available PySpin cameras.
+    """
+    # Init version, V1: original, V2: WIP with new GUI
+    global VERSION
+    VERSION = version
+
+    global pyspin_cameras, pyspin_instance
+    cameras = []
+    if not dummy:
+        if PySpin is not None:
+            cameras.extend(PySpinCamera.list_cameras())
+    return cameras
+
+
+def close_cameras():
+    """Close all available cameras."""
+    if PySpin is not None:
+        PySpinCamera.close_cameras()
+
+
+class PySpinCamera:
+    """
+    Represents a camera managed by the PySpin library.
+    """
+
+    pyspin_cameras = None
+    pyspin_instance = None
+    cameras = []
+
+    @classmethod
+    def list_cameras(cls):
+        """
+        List available PySpin cameras.
+
+        Returns:
+        - list: List of available PySpin cameras.
+        """
+        if cls.pyspin_instance is None:
+            cls.pyspin_instance = PySpin.System.GetInstance()
+        cls.pyspin_cameras = cls.pyspin_instance.GetCameras()
+        ncameras = cls.pyspin_cameras.GetSize()
+
+        cls.cameras = []
+        for i in range(ncameras):
+            camera_pyspin = cls.pyspin_cameras.GetByIndex(i)
+            camera = PySpinCamera(camera_pyspin)
+            if camera is not None:
+                cls.cameras.append(camera)
+            else:
+                camera.stop(clean=True)
+
+        return cls.cameras
+
+    # Class method to close all PySpin cameras
+    @classmethod
+    def close_cameras(cls):
+        """
+        Release resources and close all PySpin cameras.
+        """
+        logger.info("cleaning up SpinSDK")
+        for camera in cls.cameras:
+            camera.stop(clean=True)
+        if cls.pyspin_cameras is not None:
+            cls.pyspin_cameras.Clear()
+        if cls.pyspin_instance is not None:
+            cls.pyspin_instance.ReleaseInstance()
+
+    # Constructor for PySpinCamera
+    def __init__(self, camera_pyspin):
+        """
+        Initialize a PySpinCamera instance.
+
+        Parameters:
+        - camera_pyspin: The underlying PySpin camera object.
+        """
+        self.running = False
+        self.camera = camera_pyspin
+        self.tldnm = self.camera.GetTLDeviceNodeMap()
+        self.camera.Init()
+        self.node_map = self.camera.GetNodeMap()
+
+        self.last_image = None
+        self.last_image_filled = threading.Event()
+        self.last_image_cleared = threading.Event()
+
+        self.video_output = None
+        self.video_recording_on = threading.Event()
+        self.video_recording_idle = threading.Event()
+        self.height = None
+        self.width = None
+        self.channels = None
+        self.frame_rate = None
+
+        self.device_model = self.camera.DeviceModelName()
+        self.device_color_type = None
+        camera_color_type = self.device_model.split("-")[2][-1]
+        if camera_color_type == "M":
+            self.device_color_type = "Mono"
+        elif camera_color_type == "C":
+            self.device_color_type = "Color"
+        elif camera_color_type == "P":
+            self.device_color_type = "Polarized"
+            print("Polarized Camera model not supported.")
+            return None
+        else:
+            print("Not supported camera type.")
+            return None
+        print(
+            self.device_model, self.device_color_type, self.name(sn_only=True)
+        )
+
+        # set BufferHandlingMode to NewestOnly (necessary to update the image)
+        s_nodemap = self.camera.GetTLStreamNodeMap()
+        node_bufferhandling_mode = PySpin.CEnumerationPtr(
+            s_nodemap.GetNode("StreamBufferHandlingMode")
+        )
+        node_newestonly = node_bufferhandling_mode.GetEntryByName("NewestOnly")
+        node_newestonly_mode = node_newestonly.GetValue()
+        node_bufferhandling_mode.SetIntValue(node_newestonly_mode)
+
+        # Set White Balance
+        if self.device_color_type == "Color":
+            self.node_wbauto_mode = PySpin.CEnumerationPtr(
+                self.node_map.GetNode("BalanceWhiteAuto")
+            )
+            self.node_wbauto_mode_off = self.node_wbauto_mode.GetEntryByName(
+                "Off"
+            )
+            self.node_wbauto_mode_on = self.node_wbauto_mode.GetEntryByName(
+                "Continuous"
+            )
+            self.node_wbauto_mode.SetIntValue(
+                self.node_wbauto_mode_on.GetValue()
+            )  # Default: Auto mode on
+            self.node_balanceratio_mode = PySpin.CEnumerationPtr(
+                self.node_map.GetNode("BalanceRatioSelector")
+            )
+            self.node_wb = PySpin.CFloatPtr(
+                self.node_map.GetNode("BalanceRatio")
+            )
+            self.node_balanceratio_mode_red = (
+                self.node_balanceratio_mode.GetEntryByName("Red")
+            )  # Red Channel
+            self.node_balanceratio_mode_blue = (
+                self.node_balanceratio_mode.GetEntryByName("Blue")
+            )  # Blue Channel
+
+        # set exposure time
+        self.node_expauto_mode = PySpin.CEnumerationPtr(
+            self.node_map.GetNode("ExposureAuto")
+        )
+        self.node_expauto_mode_off = self.node_expauto_mode.GetEntryByName(
+            "Off"
+        )
+        self.node_expauto_mode_on = self.node_expauto_mode.GetEntryByName(
+            "Continuous"
+        )
+        self.node_expauto_mode.SetIntValue(
+            self.node_expauto_mode_on.GetValue()
+        )  # Default: Auto mode on
+        self.node_exptime = PySpin.CFloatPtr(
+            self.node_map.GetNode("ExposureTime")
+        )
+
+        # set gain
+        self.node_gainauto_mode = PySpin.CEnumerationPtr(
+            self.node_map.GetNode("GainAuto")
+        )
+        self.node_gainauto_mode_off = self.node_gainauto_mode.GetEntryByName(
+            "Off"
+        )
+        self.node_gainauto_mode_on = self.node_gainauto_mode.GetEntryByName(
+            "Continuous"
+        )
+        self.node_gain = PySpin.CFloatPtr(self.node_map.GetNode("Gain"))
+        self.node_gainauto_mode.SetIntValue(
+            self.node_gainauto_mode_on.GetValue()
+        )  # Default: Auto mode on
+
+        # set gamma
+        self.node_gammaenable_mode = PySpin.CBooleanPtr(
+            self.node_map.GetNode("GammaEnable")
+        )
+        self.node_gammaenable_mode.SetValue(True)  # Default: Gammal Enable on
+        self.node_gamma = PySpin.CFloatPtr(self.node_map.GetNode("Gamma"))
+        self.node_gamma.SetValue(0.8)
+
+        # set pixel format
+        node_pixelformat = PySpin.CEnumerationPtr(
+            self.node_map.GetNode("PixelFormat")
+        )
+        self.pixelformat = None
+        if self.device_color_type == "Mono":
+            self.pixelformat = "Mono"
+            entry_pixelformat_mono8 = node_pixelformat.GetEntryByName("Mono8")
+            node_pixelformat.SetIntValue(entry_pixelformat_mono8.GetValue())
+        elif self.device_color_type == "Color":
+            self.pixelformat = "BayerRG8"
+            entry_pixelformat_bayerRG8 = node_pixelformat.GetEntryByName(
+                "BayerRG8"
+            )
+            node_pixelformat.SetIntValue(entry_pixelformat_bayerRG8.GetValue())
+
+        # acquisition on initialization
+        if VERSION == "V1":
+            # begin acquisition
+            # V1: Start continuous acquisition on initialization.
+            self.begin_continuous_acquisition()
+        elif VERSION == "V2":
+            # V2: Start continuous acquisition when 'Start' button is toggled and end acquisition when untoggled.
+            # On initialization, start onetime acquisition to get one frame.
+            pass
+
+    def set_wb(self, channel, wb=1.2):
+        """
+        Sets the white balance of the camera.
+
+        Args:
+        - wb (float): The desired white balance value. min:1.8, max:2.5
+        """
+        if self.device_color_type == "Color":
+            self.node_wbauto_mode.SetIntValue(
+                self.node_wbauto_mode_off.GetValue()
+            )
+            if channel == "Red":
+                self.node_balanceratio_mode.SetIntValue(
+                    self.node_balanceratio_mode_red.GetValue()
+                )
+                self.node_wb.SetValue(wb)
+            elif channel == "Blue":
+                self.node_balanceratio_mode.SetIntValue(
+                    self.node_balanceratio_mode_blue.GetValue()
+                )
+                self.node_wb.SetValue(wb)
+        else:
+            pass
+
+    def get_wb(self, channel):
+        """
+        Get the gamma of the camera for the auto mode.
+        """
+        if self.device_color_type == "Color":
+            self.node_wbauto_mode.SetIntValue(
+                self.node_wbauto_mode_on.GetValue()
+            )  # Set continuous for mono camera
+            time.sleep(0.5)
+            if channel == "Red":
+                self.node_balanceratio_mode.SetIntValue(
+                    self.node_balanceratio_mode_red.GetValue()
+                )
+                time.sleep(0.5)
+                return self.node_wb.GetValue()
+            elif channel == "Blue":
+                self.node_balanceratio_mode.SetIntValue(
+                    self.node_balanceratio_mode_blue.GetValue()
+                )
+                time.sleep(0.5)
+                return self.node_wb.GetValue()
+        else:
+            return -1
+
+    def set_gamma(self, gamma=1.0):
+        """
+        Sets the gamma correction of the camera.
+
+        Args:
+        - gamma (float): The desired gamma value. min:0.25 max:1.25
+        """
+        self.node_gammaenable_mode.SetValue(True)
+        self.node_gamma.SetValue(gamma)
+
+    def disable_gamma(self):
+        """
+        Disable the gamma of the camera.
+        """
+        self.node_gammaenable_mode.SetValue(False)
+
+    def set_gain(self, gain=20.0):
+        """
+        Sets the gain of the camera.
+
+        Args:
+        - gain (float): The desired gain value. min:0, max:27.0
+        """
+        self.node_gainauto_mode.SetIntValue(
+            self.node_gainauto_mode_off.GetValue()
+        )
+        self.node_gain.SetValue(gain)
+
+    def get_gain(self):
+        """
+        Get the gain of the camera for the auto mode.
+        """
+        initial_val = self.node_gain.GetValue()
+        self.node_gainauto_mode.SetIntValue(
+            self.node_gainauto_mode_on.GetValue()
+        )  # Set continuous for mono camera
+
+        time.sleep(0.5)  # Wait for a short period
+        updated_val = self.node_gain.GetValue()
+        if updated_val != initial_val:
+            return updated_val  # Return the updated value if there's a change
+
+        return initial_val  # Return the initial value if no change is detected
+
+    def set_exposure(self, expTime=16000):
+        """
+        Sets the exposure time of the camera.
+
+        Args:
+        - expTime (int): The desired exposure time in microseconds.
+        """
+        self.node_expauto_mode.SetIntValue(
+            self.node_expauto_mode_off.GetValue()
+        )  # Return back to manual mode
+        self.node_exptime.SetValue(expTime)
+
+    def get_exposure(self):
+        """
+        Get the exposure time of the camera for the auto mode.
+        """
+        initial_val = self.node_exptime.GetValue()
+        self.node_expauto_mode.SetIntValue(
+            self.node_expauto_mode_on.GetValue()
+        )  # Enable the Auto mode
+
+        time.sleep(0.5)  # Wait for a short period
+        updated_val = self.node_exptime.GetValue()
+        if updated_val != initial_val:
+            return updated_val  # Return the updated value if there's a change
+
+        return initial_val  # Return the initial value if no change is detected
+
+    def name(self, sn_only=False):
+        """
+        Retrieves the name and serial number of the camera.
+
+        Args:
+        - sn_only (bool): Whether to return only the serial number.
+
+        Returns:
+        - str: The device model and serial number or just the serial number.
+        """
+        sn = self.camera.DeviceSerialNumber()
+        device_model = self.camera.DeviceModelName()
+        if sn_only:
+            return sn
+        else:
+            return "%s (Serial # %s)" % (device_model, sn)
+
+    def begin_singleframe_acquisition(self):
+        """
+        Begings a single Frame image acquisition.
+        """
+        # set acquisition mode to singleFrame
+        node_acquisition_mode = PySpin.CEnumerationPtr(
+            self.node_map.GetNode("AcquisitionMode")
+        )
+        node_acquisition_mode_singleframe = (
+            node_acquisition_mode.GetEntryByName("SingleFrame")
+        )
+        acquisition_mode_singleframe = (
+            node_acquisition_mode_singleframe.GetValue()
+        )
+        node_acquisition_mode.SetIntValue(acquisition_mode_singleframe)
+
+        # Begin Acquisition: Image acquisition must be ended when no more images are needed.
+        self.camera.BeginAcquisition()
+        print(f"Begin Single Frame Acquisition {self.name(sn_only=True)} ")
+        self.capture_thread = threading.Thread(
+            target=self.capture, daemon=False
+        )
+        self.capture_thread.start()
+
+    def end_singleframe_acquisition(self):
+        """End Acquisition"""
+        self.last_image_cleared.wait()
+        self.capture_thread.join()
+        self.camera.EndAcquisition()
+        self.last_image = None
+        self.last_image_cleared.clear()
+        self.last_image_filled.clear()
+
+    def begin_continuous_acquisition(self):
+        """
+        Begins the image acquisition process in continuous mode and starts the capture loop in a separate thread.
+        """
+        if self.running:
+            print("Error: camera is already running")
+            return -1
+
+        # set acquisition mode continuous (continuous stream of images)
+        node_acquisition_mode = PySpin.CEnumerationPtr(
+            self.node_map.GetNode("AcquisitionMode")
+        )
+        node_acquisition_mode_continuous = node_acquisition_mode.GetEntryByName(
+            "Continuous"
+        )
+        acquisition_mode_continuous = (
+            node_acquisition_mode_continuous.GetValue()
+        )
+        node_acquisition_mode.SetIntValue(acquisition_mode_continuous)
+
+        # Begin Acquisition: Image acquisition must be ended when no more images are needed.
+        self.camera.BeginAcquisition()
+        logger.debug(f"BeginAcquisition {self.name(sn_only=True)} ")
+        self.running = True
+        self.capture_thread = threading.Thread(
+            target=self.capture_loop, daemon=True
+        )
+        self.capture_thread.start()
+
+    def capture_loop(self):
+        """
+        Continuous loop to capture images while the camera is running.
+        """
+        while self.running:
+            self.capture()
+            # print(".", end="",flush=True)
+
+    def capture(self):
+        """
+        Captures an image and checks for its completeness.
+        If video recording is enabled, writes the image to the video file.
+
+        *** NOTES ***
+        Capturing an image houses images on the camera buffer.
+        Trying to capture an image that does not exist will hang the camera.
+        Using-statements help ensure that images are released.
+        If too many images remain unreleased, the buffer will fill,
+        causing the camera to hang.
+        Images can also be released manually by calling Release().
+        """
+        # Timestamp for the current capture
+        ts = time.time()
+        self.last_capture_time = ts
+
+        # Retrieve the next image from the camera
+        image = self.camera.GetNextImage(1000)
+
+        while image.IsIncomplete():
+            time.sleep(0.001)
+
+        # Release the previous image from the buffer if it exists
+        if self.last_image is not None:
+            try:
+                self.last_image.Release()
+            except PySpin.SpinnakerException:
+                print("Spinnaker Exception: Couldn't release last image")
+
+        # Update the last captured image reference
+        self.last_image = image
+        self.last_image_filled.set()
+
+        # Record the image if video recording is active
+        if self.video_recording_on.is_set():
+            self.video_recording_idle.clear()
+
+            frame = self.get_last_image_data()
+            frame = cv2.cvtColor(frame, cv2.COLOR_RGB2BGR)
+
+            self.video_output.write(frame)
+            self.video_recording_idle.set()
+
+    def get_last_capture_time(self, millisecond=False):
+        """
+        Returns the timestamp of the last captured image in a formatted string.
+
+        Returns:
+        - str: Timestamp in the format 'YYYYMMDD-HHMMSS'.
+        """
+        ts = self.last_capture_time
+        dt = datetime.datetime.fromtimestamp(ts)
+        if millisecond:
+            return "%04d%02d%02d-%02d%02d%02d.%03d" % (
+                dt.year,
+                dt.month,
+                dt.day,
+                dt.hour,
+                dt.minute,
+                dt.second,
+                dt.microsecond // 1000,
+            )
+        else:
+            return "%04d%02d%02d-%02d%02d%02d" % (
+                dt.year,
+                dt.month,
+                dt.day,
+                dt.hour,
+                dt.minute,
+                dt.second,
+            )
+
+    def save_last_image(
+        self, filepath, isTimestamp=False, custom_name="Microscope_"
+    ):
+        """
+        Saves the last captured image to the specified file path.
+
+        Args:
+        - filepath (str): Directory to save the image.
+        - isTimestamp (bool): Whether to append a timestamp to the filename.
+        - custom_name (str): Custom prefix for the filename. 
+        S/N is set as custom name.
+        """
+        image_name = (
+            "{}_{}.png".format(custom_name, self.get_last_capture_time())
+            if isTimestamp
+            else "{}.png".format(custom_name)
+        )
+        full_path = os.path.join(filepath, image_name)
+        logger.debug(f"Saving image to {full_path}")
+        print(f"Saving image to {full_path}")
+
+        # Save the image
+        try:
+            image_converted = self.get_last_image_data()
+            if image_converted is not None:
+                # Convert the image from RGB to BGR
+                image_converted = cv2.cvtColor(
+                    image_converted, cv2.COLOR_RGB2BGR
+                )
+                cv2.imwrite(full_path, image_converted)
+            else:
+                logger.error("Image not found or couldn't be retrieved.")
+        except Exception as e:
+            logger.error(f"An error occurred while saving the image: {e}")
+
+    def get_last_image(self):
+        """
+        Returns the last captured image.
+
+        Returns:
+        - PySpin.Image: The last captured image.
+        """
+        return self.last_image
+
+    # Get the last captured image data as a numpy array
+    def get_last_image_data(self):
+        """
+        Returns the last captured image data as a numpy array.
+        Shape: (height, width, 3) for RGB,  (height, width) for mono
+
+        Returns:
+        - numpy.ndarray: Image data in array format.
+        """
+        # Wait until last_image is not None
+        self.last_image_filled.wait()
+        frame_image = self.last_image.GetNDArray()
+        if self.pixelformat == "BayerRG8":
+            frame_image = cv2.cvtColor(frame_image, cv2.COLOR_BayerRG2BGR)
+        return frame_image
+
+    # Get the last captured image data as a numpy array
+    def get_last_image_data_singleFrame(self):
+        """
+        Returns the last captured image data as a numpy array.
+        Shape: (height, width, 3) for RGB,  (height, width) for mono
+
+        Returns:
+        - numpy.ndarray: Image data in array format.
+        """
+        # Wait until last_image is not None
+        self.last_image_filled.wait()
+        frame_image = self.last_image.GetNDArray()
+        if self.pixelformat == "BayerRG8":
+            frame_image = cv2.cvtColor(frame_image, cv2.COLOR_BayerRG2BGR)
+        self.last_image_cleared.set()
+        return frame_image
+
+    def camera_info(self):
+        """
+        Retrieves and logs the camera's essential information 
+        such as frame dimensions and channels.
+        """
+        # Gather camera details
+        self.height = self.camera.Height()
+        self.width = self.camera.Width()
+        try:
+            if self.last_image is not None:
+                self.channels = self.last_image.GetNumChannels()
+        except Exception as e:
+            logger.error(f"An error occurred while getting channel info: {e}")
+        logger.info(
+            f"camera frame width: {self.width}, height: {self.width}, channels: {self.channels}"
+        )
+
+        # Set frame rate equal to the current acquisition frame rate (Hz)
+        nodeFramerate = PySpin.CFloatPtr(
+            self.node_map.GetNode("AcquisitionFrameRate")
+        )
+        if (not PySpin.IsAvailable(nodeFramerate)) or (
+            not PySpin.IsReadable(nodeFramerate)
+        ):
+            logger.error("Unable to retrieve frame rate. Aborting...")
+            return -1
+        self.frame_rate = nodeFramerate.GetValue()
+        logger.info(f"Frame rate to be set to {self.frame_rate}")
+
+    def save_recording(
+        self, filepath, isTimestamp=False, custom_name="Microscope_"
+    ):
+        """
+        Begins video recording and saves the video to the specified file path.
+
+        Args:
+        - filepath (str): Directory to save the video.
+        - isTimestamp (bool): Whether to append a timestamp to the filename.
+        - custom_name (str): Custom prefix for the filename.
+        """
+        # Formulate the video name based on the input parameters
+        video_name = (
+            "{}_{}.avi".format(custom_name, self.get_last_capture_time())
+            if isTimestamp
+            else "{}.avi".format(custom_name)
+        )
+        full_path = os.path.join(filepath, video_name)
+        print(f"Saving video to {full_path}")
+        logger.debug(f"Try saving video to {full_path}")
+
+        # Update camera details
+        self.camera_info()
+
+        # Begin the video recording with appropriate configurations
+        fourcc = cv2.VideoWriter_fourcc(*"XVID")
+        self.video_output = cv2.VideoWriter(
+            full_path, fourcc, self.frame_rate, (self.width, self.height), True
+        )
+        self.video_recording_on.set()
+
+    def stop_recording(self):
+        """
+        Stops the ongoing video capture process and releases video resources.
+        """
+        self.video_recording_on.clear()
+        self.video_recording_idle.wait()
+        self.video_recording_idle.clear()
+        self.video_output.release()
+
+    # Clean up the camera
+    def stop(self, clean=False):
+        """
+        Cleans up resources associated with the camera and video recording.
+
+        Note:
+            Do not change the order of codes without referring PySpin manual.
+            They are ordered by PySpin Camera Init / Turn off sequence.
+        """
+        if self.running:
+            self.running = False
+            self.capture_thread.join()
+            self.camera.EndAcquisition()
+            self.last_image = None
+            self.last_image_filled.clear()
+
+        if self.video_recording_on.is_set():
+            self.stop_recording()
+
+        if clean:
+            del self.camera
+
+
+# Class for simulating a mock camera
+class MockCamera:
+    """Mock Camera showing salts and pepper noise images"""
+
+    n_cameras = 0
+
+    def __init__(self):
+        """Initialize a mock camera with a unique name"""
+        self._name = f"MockCamera{MockCamera.n_cameras}"
+        MockCamera.n_cameras += 1
+        # Create mock image data with random values
+        self.data = np.random.randint(
+            0, 255, size=(5, 3000, 4000), dtype="ubyte"
+        )
+        self._next_frame = 0
+        self.device_color_type = None
+
+    def name(self, sn_only=False):
+        """Get the name of the mock camera"""
+        return self._name
+
+    def get_last_image_data(self):
+        """
+        Return last image as numpy array with shape (height, width, 3) for RGB
+		or (height, width) for mono.
+        """
+        frame = self.data[self._next_frame]
+        self._next_frame = (self._next_frame + 1) % self.data.shape[0]
+        return frame
+
+    def save_last_image(
+        self, filepath, isTimestamp=False, custom_name="MockCamera_"
+    ):
+        """Dummy function"""
+        print("This is MockCamera. Cannot capture the image")
+        return
+
+    def set_wb(self, wb=2.0):
+        """Dummy function"""
+        logger.info("This is MockCamera. Setting is not applicable")
+        return
+
+    def set_gamma(self, gamma=1.0):
+        """Dummy function"""
+        logger.info("This is MockCamera. Setting is not applicable")
+        return
+
+    def set_gain(self, gain=25.0):
+        """Dummy function"""
+        logger.info("This is MockCamera. Setting is not applicable")
+        return
+
+    def set_exposure(self, expTime=16000):
+        """Dummy function"""
+        logger.info("This is MockCamera. Setting is not applicable")
+        return
+
+    def stop(self, clean=False):
+        """Dummy function"""
+        logger.info("This is MockCamera. Stop")
+        return
+
+    def begin_continuous_acquisition(self):
+        """Dummy function"""
+        return
+
+    def get_last_capture_time(self, millisecond=False):
+        """Dummy function"""
+        return
+
+    def stop(self, clean=False):
+        """Dummy function"""
+        return
+
+
+class VideoSource:
+    """Video Source"""
+
+    def __init__(self, filename):
+        """Initialize a video source with a given filename"""
+        self.filename = filename
+        self._name = os.path.basename(self.filename)
+        self.cap = cv2.VideoCapture(self.filename)
+
+    def name(self, sn_only=False):
+        """Get the name of the video source"""
+        return self._name
+
+    def get_last_image_data(self):
+        """Read the last captured frame from the video source"""
+        ret, frame = self.cap.read()
+        if ret:
+            return frame
+        else:
+            # If the video has ended, reset the video source to the beginning
+            self.cap.set(cv2.CAP_PROP_POS_FRAMES, 0)
+            return np.random.randint(0, 255, size=(3000, 4000), dtype="ubyte")
+
+    def save_last_image(
+        self, filepath, isTimestamp=False, custom_name="VideoSource_"
+    ):
+        """Dummy function"""
+        print("This is from Video Source. Cannot capture the image")
+        return
+
+    def set_wb(self, wb=2.0):
+        """Dummy function"""
+        logger.info("This is VideoSource. Setting is not applicable")
+        return
+
+    def set_gamma(self, gamma=1.0):
+        """Dummy function"""
+        logger.info("This is VideoSource. Setting is not applicable")
+        return
+
+    def set_gain(self, gain=25.0):
+        """Dummy function"""
+        logger.info("This is VideoSource. Setting is not applicable")
+        return
+
+    def set_exposure(self, expTime=125000):
+        """Dummy function"""
+        logger.info("This is VideoSource. Setting is not applicable")
+        return
+
+    def begin_continuous_acquisition(self):
+        """Dummy function"""
+        return
+
+    def stop(self, clean=False):
+        """Dummy function"""
+        return
```

### Comparing `parallax_app-0.37.1/parallax/curr_bg_cmp_processor.py` & `parallax_app-0.37.5/parallax/curr_bg_cmp_processor.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,320 +1,320 @@
-"""
-CurrBgCmpProcessor: Module for finding the difference image 
-using Current and Background Comparison.
-
-This module provides classes and methods for processing images 
-to detect differences between a current image and a background image, 
-with the aim of detecting a probe and its tip.
-
-Classes:
-    - CurrBgCmpProcessor: Main class for performing the comparison
-      and detecting the probe.
-
-Usage:
-    - Initialize an instance of CurrBgCmpProcessor with necessary parameters.
-    - Use the first_cmp() method to perform the initial comparison.
-    - Use the update_cmp() method to update the comparison and detect changes 
-    over time.
-"""
-
-import logging
-
-import cv2
-import numpy as np
-
-from .probe_fine_tip_detector import ProbeFineTipDetector
-from .utils import UtilsCoords, UtilsCrops
-
-# Set logger name
-logger = logging.getLogger(__name__)
-# Set the logging level for PyQt5.uic.uiparser/properties to WARNING, 
-# to ignore DEBUG messages
-logging.getLogger("PyQt5.uic.uiparser").setLevel(logging.WARNING)
-logging.getLogger("PyQt5.uic.properties").setLevel(logging.WARNING)
-
-
-class CurrBgCmpProcessor(UtilsCoords, UtilsCrops, ProbeFineTipDetector):
-    """Finding diff image using Current and Background Comparison"""
-
-    def __init__(
-        self, ProbeDetector, original_size, resized_size, reticle_zone=None
-    ):
-        """
-        Initialize the CurrBgCmpProcessor.
-
-        Args:
-            ProbeDetector (object): An instance of the ProbeDetector class.
-            original_size (tuple): The original size of the image (height, width).
-            resized_size (tuple): The resized size of the image (height, width).
-            reticle_zone (numpy.ndarray, optional): The reticle zone image. Defaults to None.
-        """
-        UtilsCoords.__init__(self, original_size, resized_size)
-        UtilsCrops.__init__(self)
-        ProbeFineTipDetector.__init__(self)
-        self.img_fname = None
-        self.diff_img = None
-        self.diff_img_crop = None
-        self.curr = None
-        self.mask = None
-        self.bg = None
-        self.org_img = None
-        self.IMG_SIZE = resized_size
-        self.IMG_SIZE_ORIGINAL = original_size
-        self.ProbeDetector = ProbeDetector
-        self.reticle_zone = reticle_zone
-        self.crop_init = 50
-
-    def update_reticle_zone(self, reticle_zone):
-        """Update the reticle zone.
-
-        Args:
-            reticle_zone (numpy.ndarray): Reticle zone image.
-        """
-        self.reticle_zone = reticle_zone
-
-    def first_cmp(self, curr_img, mask, org_img, img_fname=None):
-        """Perform first comparison
-
-        Args:
-            curr_img (numpy.ndarray): Current image.
-            mask (numpy.ndarray): Mask image.
-            org_img (numpy.ndarray): Original image.
-            img_fname (str, optional): Image filename. Defaults to None.
-
-        Returns:
-            bool: True if probe is detected, False otherwise.
-        """
-        logger.debug("CurrBgCmpProcessor::first_cmp")
-        ret = False
-        self.img_fname = img_fname
-        self.mask = mask
-        self.curr_img = curr_img
-        self.curr_img = self._get_binary(self.curr_img)
-        if self.bg is None:
-            self._create_bg(self.curr_img)
-        self._preprocess_diff_image(self.curr_img)
-        ret = self._detect_probe()
-        if ret:
-            logger.debug("FirstCurrBgCmpProcessor:: detect")
-            _ = self._get_precise_tip(org_img)
-            self.bg = cv2.bitwise_not(
-                cv2.bitwise_xor(self.diff_img, self.curr_img), mask=self.mask
-            )
-
-        return ret
-
-    def update_cmp(self, curr_img, mask, org_img, img_fname=None):
-        """Update the comparison.
-
-        Args:
-            curr_img (numpy.ndarray): Current image.
-            mask (numpy.ndarray): Mask image.
-            org_img (numpy.ndarray): Original image.
-            img_fname (str, optional): Image filename. Defaults to None.
-
-        Returns:
-            bool: True if probe is detected and precise tip is found, False otherwise.
-        """
-        ret = False
-        self.img_fname = img_fname
-        self.mask = mask
-        self.curr_img = curr_img
-        self.curr_img = self._get_binary(self.curr_img)
-        if self.bg is None:
-            self._create_bg(self.curr_img)
-
-        self._preprocess_diff_image(self.curr_img)
-        ret = self._update_crop()
-        if ret:
-            ret_precise_tip = self._get_precise_tip(org_img)
-            self._update_bg()
-            pass
-
-        return ret and ret_precise_tip
-
-    def _update_bg(self):
-        """Update the background image."""
-        kernel = np.ones((3, 3), np.uint8)
-        self.diff_img_crop = cv2.dilate(
-            self.diff_img_crop, kernel, iterations=1
-        )
-
-        # Find and process contours
-        contours, _ = cv2.findContours(
-            self.diff_img_crop, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE
-        )
-        if len(contours) >= 2:
-            largest_contour = max(contours, key=cv2.contourArea)
-            for contour in contours:
-                if contour is not largest_contour:
-                    self.diff_img_crop = cv2.drawContours(
-                        self.diff_img_crop, [contour], -1, (0, 0, 0), -1
-                    )
-
-        # Initialize an empty image for drawing
-        diff_img = np.zeros_like(self.diff_img)
-
-        # Calculate the direction and extend the line between probe tip and base
-        offset = 10
-        tip_direction = np.array(self.ProbeDetector.probe_tip) - np.array(
-            self.ProbeDetector.probe_base
-        )
-        tip_direction_normalized = tip_direction / np.linalg.norm(tip_direction)
-        extended_probe_tip = tuple(
-            np.array(self.ProbeDetector.probe_tip)
-            + (offset * tip_direction_normalized).astype(int)
-        )
-        extended_probe_base = tuple(
-            np.array(self.ProbeDetector.probe_base)
-            - (offset * tip_direction_normalized).astype(int)
-        )
-
-        # Draw the extended line
-        cv2.line(
-            diff_img, extended_probe_tip, extended_probe_base, 255, thickness=5
-        )
-
-        # Combine the processed image with the current image to extract the background
-        self.bg = cv2.bitwise_and(self.curr_img, cv2.bitwise_not(diff_img))
-        self.bg = cv2.bitwise_not(self.bg, mask=self.mask)
-
-    def _update_crop(self):
-        """Update the crop region.
-
-        Returns:
-            bool: True if probe is detected, False otherwise.
-        """
-        # Draw
-        # diff_img_ = self.diff_img.copy()
-        # diff_img_ = cv2.cvtColor(diff_img_, cv2.COLOR_GRAY2BGR)
-
-        ret = False
-        crop_size = self.crop_init
-        crop_utils = UtilsCrops()
-        while (ret is False) and (
-            crop_size <= max(self.IMG_SIZE[0], self.IMG_SIZE[1])
-        ):
-            top, bottom, left, right = crop_utils.calculate_crop_region(
-                self.ProbeDetector.probe_tip,
-                self.ProbeDetector.probe_base,
-                crop_size,
-                self.IMG_SIZE,
-            )
-            self.diff_img_crop = self.diff_img[top:bottom, left:right]
-            hough_minLineLength_adpative = (
-                60 + int(crop_size / self.crop_init) * 5
-            )
-            ret = self.ProbeDetector.update_probe(
-                self.diff_img_crop,
-                self.mask,
-                hough_minLineLength=hough_minLineLength_adpative,
-                maxLineGap=0,
-                offset_x=left,
-                offset_y=top,
-                img_fname=self.img_fname,
-            )
-
-            # cv2.rectangle(diff_img_, (left, top), (right, bottom), (155, 155, 0), 5)  # Green rectangle
-
-            if ret and crop_utils.is_point_on_crop_region(
-                self.ProbeDetector.probe_tip, top, bottom, left, right, buffer=5
-            ):
-                ret = False
-            """
-            if ret:
-                cv2.circle(diff_img_, self.ProbeDetector.probe_tip, 3, (0, 0, 255), -1)  # RED circle
-                cv2.circle(diff_img_, self.ProbeDetector.probe_base, 3, (0, 255, 0), -1)  # Green circle
-                cv2.imwrite('debug/crop.jpg', diff_img_)
-                cv2.imwrite('debug/reticle_zone.jpg', self.reticle_zone)
-            """
-            if ret and self.reticle_zone is not None:
-                tip_in_reticle = self._is_point_in_reticle_region(
-                    self.reticle_zone, self.ProbeDetector.probe_tip
-                )
-                base_in_reticle = self._is_point_in_reticle_region(
-                    self.reticle_zone, self.ProbeDetector.probe_base
-                )
-                if tip_in_reticle and base_in_reticle:
-                    return False
-
-            if ret:
-                break
-
-            crop_size += 100
-
-        del crop_utils  # Garbage Collect
-        return ret
-
-    def _is_point_in_reticle_region(self, image, point):
-        """Check if a point is in the reticle region."""
-        return image[point[1], point[0]] == 255
-
-    def _get_precise_tip(self, org_img):
-        """Get precise probe tip on original size image
-        Args:
-            org_img (numpy.ndarray): Original image.
-
-        Returns:
-            bool: True if precise tip is found, False otherwise.
-        """
-        coords_utils = UtilsCoords(self.IMG_SIZE_ORIGINAL, self.IMG_SIZE)
-        probe_fine_tip = ProbeFineTipDetector()
-        crop_utils = UtilsCrops()
-        ret = False
-
-        probe_tip_original_coords = coords_utils.scale_coords_to_original(
-            self.ProbeDetector.probe_tip
-        )
-        top, bottom, left, right = crop_utils.calculate_crop_region(
-            probe_tip_original_coords,
-            probe_tip_original_coords,
-            crop_size=20,
-            IMG_SIZE=self.IMG_SIZE_ORIGINAL,
-        )
-        self.tip_image = org_img[top:bottom, left:right]
-        ret = probe_fine_tip.get_precise_tip(
-            self.tip_image,
-            probe_tip_original_coords,
-            offset_x=left,
-            offset_y=top,
-            direction=self.ProbeDetector.probe_tip_direction,
-            img_fname=self.img_fname,
-        )
-        if ret:
-            self.ProbeDetector.probe_tip_org = probe_fine_tip.tip
-
-        del probe_fine_tip  # Garbage Collect
-        del coords_utils
-        del crop_utils
-
-        return ret
-
-    def _get_binary(self, curr_img):
-        """Get binary image.
-        Args:
-            curr_img (numpy.ndarray): Current image.
-        Returns:
-            numpy.ndarray: Binary image.
-        """
-        curr_img = cv2.adaptiveThreshold(
-            curr_img,
-            255,
-            cv2.ADAPTIVE_THRESH_GAUSSIAN_C,
-            cv2.THRESH_BINARY,
-            17,
-            2,
-        )
-        curr_img = cv2.bitwise_not(curr_img)
-        return curr_img
-
-    def _create_bg(self, curr_img):
-        """Create background image."""
-        self.bg = cv2.bitwise_not(curr_img)
-
-    def _preprocess_diff_image(self, curr_img):
-        """Preprocess difference image."""
-        self.diff_img = cv2.bitwise_and(curr_img, self.bg, mask=self.mask)
-
-    def _detect_probe(self):
-        """Detect probe in difference image."""
+"""
+CurrBgCmpProcessor: Module for finding the difference image 
+using Current and Background Comparison.
+
+This module provides classes and methods for processing images 
+to detect differences between a current image and a background image, 
+with the aim of detecting a probe and its tip.
+
+Classes:
+    - CurrBgCmpProcessor: Main class for performing the comparison
+      and detecting the probe.
+
+Usage:
+    - Initialize an instance of CurrBgCmpProcessor with necessary parameters.
+    - Use the first_cmp() method to perform the initial comparison.
+    - Use the update_cmp() method to update the comparison and detect changes 
+    over time.
+"""
+
+import logging
+
+import cv2
+import numpy as np
+
+from .probe_fine_tip_detector import ProbeFineTipDetector
+from .utils import UtilsCoords, UtilsCrops
+
+# Set logger name
+logger = logging.getLogger(__name__)
+# Set the logging level for PyQt5.uic.uiparser/properties to WARNING, 
+# to ignore DEBUG messages
+logging.getLogger("PyQt5.uic.uiparser").setLevel(logging.WARNING)
+logging.getLogger("PyQt5.uic.properties").setLevel(logging.WARNING)
+
+
+class CurrBgCmpProcessor(UtilsCoords, UtilsCrops, ProbeFineTipDetector):
+    """Finding diff image using Current and Background Comparison"""
+
+    def __init__(
+        self, ProbeDetector, original_size, resized_size, reticle_zone=None
+    ):
+        """
+        Initialize the CurrBgCmpProcessor.
+
+        Args:
+            ProbeDetector (object): An instance of the ProbeDetector class.
+            original_size (tuple): The original size of the image (height, width).
+            resized_size (tuple): The resized size of the image (height, width).
+            reticle_zone (numpy.ndarray, optional): The reticle zone image. Defaults to None.
+        """
+        UtilsCoords.__init__(self, original_size, resized_size)
+        UtilsCrops.__init__(self)
+        ProbeFineTipDetector.__init__(self)
+        self.img_fname = None
+        self.diff_img = None
+        self.diff_img_crop = None
+        self.curr = None
+        self.mask = None
+        self.bg = None
+        self.org_img = None
+        self.IMG_SIZE = resized_size
+        self.IMG_SIZE_ORIGINAL = original_size
+        self.ProbeDetector = ProbeDetector
+        self.reticle_zone = reticle_zone
+        self.crop_init = 50
+
+    def update_reticle_zone(self, reticle_zone):
+        """Update the reticle zone.
+
+        Args:
+            reticle_zone (numpy.ndarray): Reticle zone image.
+        """
+        self.reticle_zone = reticle_zone
+
+    def first_cmp(self, curr_img, mask, org_img, img_fname=None):
+        """Perform first comparison
+
+        Args:
+            curr_img (numpy.ndarray): Current image.
+            mask (numpy.ndarray): Mask image.
+            org_img (numpy.ndarray): Original image.
+            img_fname (str, optional): Image filename. Defaults to None.
+
+        Returns:
+            bool: True if probe is detected, False otherwise.
+        """
+        logger.debug("CurrBgCmpProcessor::first_cmp")
+        ret = False
+        self.img_fname = img_fname
+        self.mask = mask
+        self.curr_img = curr_img
+        self.curr_img = self._get_binary(self.curr_img)
+        if self.bg is None:
+            self._create_bg(self.curr_img)
+        self._preprocess_diff_image(self.curr_img)
+        ret = self._detect_probe()
+        if ret:
+            logger.debug("FirstCurrBgCmpProcessor:: detect")
+            _ = self._get_precise_tip(org_img)
+            self.bg = cv2.bitwise_not(
+                cv2.bitwise_xor(self.diff_img, self.curr_img), mask=self.mask
+            )
+
+        return ret
+
+    def update_cmp(self, curr_img, mask, org_img, img_fname=None):
+        """Update the comparison.
+
+        Args:
+            curr_img (numpy.ndarray): Current image.
+            mask (numpy.ndarray): Mask image.
+            org_img (numpy.ndarray): Original image.
+            img_fname (str, optional): Image filename. Defaults to None.
+
+        Returns:
+            bool: True if probe is detected and precise tip is found, False otherwise.
+        """
+        ret = False
+        self.img_fname = img_fname
+        self.mask = mask
+        self.curr_img = curr_img
+        self.curr_img = self._get_binary(self.curr_img)
+        if self.bg is None:
+            self._create_bg(self.curr_img)
+
+        self._preprocess_diff_image(self.curr_img)
+        ret = self._update_crop()
+        if ret:
+            ret_precise_tip = self._get_precise_tip(org_img)
+            self._update_bg()
+            pass
+
+        return ret and ret_precise_tip
+
+    def _update_bg(self):
+        """Update the background image."""
+        kernel = np.ones((3, 3), np.uint8)
+        self.diff_img_crop = cv2.dilate(
+            self.diff_img_crop, kernel, iterations=1
+        )
+
+        # Find and process contours
+        contours, _ = cv2.findContours(
+            self.diff_img_crop, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE
+        )
+        if len(contours) >= 2:
+            largest_contour = max(contours, key=cv2.contourArea)
+            for contour in contours:
+                if contour is not largest_contour:
+                    self.diff_img_crop = cv2.drawContours(
+                        self.diff_img_crop, [contour], -1, (0, 0, 0), -1
+                    )
+
+        # Initialize an empty image for drawing
+        diff_img = np.zeros_like(self.diff_img)
+
+        # Calculate the direction and extend the line between probe tip and base
+        offset = 10
+        tip_direction = np.array(self.ProbeDetector.probe_tip) - np.array(
+            self.ProbeDetector.probe_base
+        )
+        tip_direction_normalized = tip_direction / np.linalg.norm(tip_direction)
+        extended_probe_tip = tuple(
+            np.array(self.ProbeDetector.probe_tip)
+            + (offset * tip_direction_normalized).astype(int)
+        )
+        extended_probe_base = tuple(
+            np.array(self.ProbeDetector.probe_base)
+            - (offset * tip_direction_normalized).astype(int)
+        )
+
+        # Draw the extended line
+        cv2.line(
+            diff_img, extended_probe_tip, extended_probe_base, 255, thickness=5
+        )
+
+        # Combine the processed image with the current image to extract the background
+        self.bg = cv2.bitwise_and(self.curr_img, cv2.bitwise_not(diff_img))
+        self.bg = cv2.bitwise_not(self.bg, mask=self.mask)
+
+    def _update_crop(self):
+        """Update the crop region.
+
+        Returns:
+            bool: True if probe is detected, False otherwise.
+        """
+        # Draw
+        # diff_img_ = self.diff_img.copy()
+        # diff_img_ = cv2.cvtColor(diff_img_, cv2.COLOR_GRAY2BGR)
+
+        ret = False
+        crop_size = self.crop_init
+        crop_utils = UtilsCrops()
+        while (ret is False) and (
+            crop_size <= max(self.IMG_SIZE[0], self.IMG_SIZE[1])
+        ):
+            top, bottom, left, right = crop_utils.calculate_crop_region(
+                self.ProbeDetector.probe_tip,
+                self.ProbeDetector.probe_base,
+                crop_size,
+                self.IMG_SIZE,
+            )
+            self.diff_img_crop = self.diff_img[top:bottom, left:right]
+            hough_minLineLength_adpative = (
+                60 + int(crop_size / self.crop_init) * 5
+            )
+            ret = self.ProbeDetector.update_probe(
+                self.diff_img_crop,
+                self.mask,
+                hough_minLineLength=hough_minLineLength_adpative,
+                maxLineGap=0,
+                offset_x=left,
+                offset_y=top,
+                img_fname=self.img_fname,
+            )
+
+            # cv2.rectangle(diff_img_, (left, top), (right, bottom), (155, 155, 0), 5)  # Green rectangle
+
+            if ret and crop_utils.is_point_on_crop_region(
+                self.ProbeDetector.probe_tip, top, bottom, left, right, buffer=5
+            ):
+                ret = False
+            """
+            if ret:
+                cv2.circle(diff_img_, self.ProbeDetector.probe_tip, 3, (0, 0, 255), -1)  # RED circle
+                cv2.circle(diff_img_, self.ProbeDetector.probe_base, 3, (0, 255, 0), -1)  # Green circle
+                cv2.imwrite('debug/crop.jpg', diff_img_)
+                cv2.imwrite('debug/reticle_zone.jpg', self.reticle_zone)
+            """
+            if ret and self.reticle_zone is not None:
+                tip_in_reticle = self._is_point_in_reticle_region(
+                    self.reticle_zone, self.ProbeDetector.probe_tip
+                )
+                base_in_reticle = self._is_point_in_reticle_region(
+                    self.reticle_zone, self.ProbeDetector.probe_base
+                )
+                if tip_in_reticle and base_in_reticle:
+                    return False
+
+            if ret:
+                break
+
+            crop_size += 100
+
+        del crop_utils  # Garbage Collect
+        return ret
+
+    def _is_point_in_reticle_region(self, image, point):
+        """Check if a point is in the reticle region."""
+        return image[point[1], point[0]] == 255
+
+    def _get_precise_tip(self, org_img):
+        """Get precise probe tip on original size image
+        Args:
+            org_img (numpy.ndarray): Original image.
+
+        Returns:
+            bool: True if precise tip is found, False otherwise.
+        """
+        coords_utils = UtilsCoords(self.IMG_SIZE_ORIGINAL, self.IMG_SIZE)
+        probe_fine_tip = ProbeFineTipDetector()
+        crop_utils = UtilsCrops()
+        ret = False
+
+        probe_tip_original_coords = coords_utils.scale_coords_to_original(
+            self.ProbeDetector.probe_tip
+        )
+        top, bottom, left, right = crop_utils.calculate_crop_region(
+            probe_tip_original_coords,
+            probe_tip_original_coords,
+            crop_size=20,
+            IMG_SIZE=self.IMG_SIZE_ORIGINAL,
+        )
+        self.tip_image = org_img[top:bottom, left:right]
+        ret = probe_fine_tip.get_precise_tip(
+            self.tip_image,
+            probe_tip_original_coords,
+            offset_x=left,
+            offset_y=top,
+            direction=self.ProbeDetector.probe_tip_direction,
+            img_fname=self.img_fname,
+        )
+        if ret:
+            self.ProbeDetector.probe_tip_org = probe_fine_tip.tip
+
+        del probe_fine_tip  # Garbage Collect
+        del coords_utils
+        del crop_utils
+
+        return ret
+
+    def _get_binary(self, curr_img):
+        """Get binary image.
+        Args:
+            curr_img (numpy.ndarray): Current image.
+        Returns:
+            numpy.ndarray: Binary image.
+        """
+        curr_img = cv2.adaptiveThreshold(
+            curr_img,
+            255,
+            cv2.ADAPTIVE_THRESH_GAUSSIAN_C,
+            cv2.THRESH_BINARY,
+            17,
+            2,
+        )
+        curr_img = cv2.bitwise_not(curr_img)
+        return curr_img
+
+    def _create_bg(self, curr_img):
+        """Create background image."""
+        self.bg = cv2.bitwise_not(curr_img)
+
+    def _preprocess_diff_image(self, curr_img):
+        """Preprocess difference image."""
+        self.diff_img = cv2.bitwise_and(curr_img, self.bg, mask=self.mask)
+
+    def _detect_probe(self):
+        """Detect probe in difference image."""
         return self.ProbeDetector.first_detect_probe(self.diff_img, self.mask)
```

### Comparing `parallax_app-0.37.1/parallax/curr_prev_cmp_processor.py` & `parallax_app-0.37.5/parallax/curr_prev_cmp_processor.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,250 +1,250 @@
-"""
-CurrPrevCmpProcessor: Module for finding the difference image 
-using Current Previous Comparison.
-
-This module provides classes and methods for processing images
-to detect differences between a current image and a previous image, with the aim of detecting a probe and its tip.
-
-Classes:
-    - CurrPrevCmpProcessor: Main class for performing
-      the comparison and detecting the probe.
-
-Usage:
-    - Initialize an instance of CurrPrevCmpProcessor with necessary parameters.
-    - Use the first_cmp() method to perform the initial comparison.
-    - Use the update_cmp() method to update the comparison
-      and detect changes over time.
-"""
-
-import logging
-import os
-
-import cv2
-import numpy as np
-
-from .probe_fine_tip_detector import ProbeFineTipDetector
-from .utils import UtilsCoords, UtilsCrops
-
-# Set logger name
-logger = logging.getLogger(__name__)
-# Set the logging level for PyQt5.uic.uiparser/properties
-logging.getLogger("PyQt5.uic.uiparser").setLevel(logging.WARNING)
-logging.getLogger("PyQt5.uic.properties").setLevel(logging.WARNING)
-
-
-class CurrPrevCmpProcessor(UtilsCoords, UtilsCrops, ProbeFineTipDetector):
-    """Finding diff image using Current Previous Comparison"""
-
-    def __init__(self, ProbeDetector, original_size, resized_size):
-        """
-        Initialize the CurrPrevCmpProcessor.
-
-        Args:
-            ProbeDetector (object): An instance of the ProbeDetector class.
-            original_size (tuple): The original size of the image (height, width).
-            resized_size (tuple): The resized size of the image (height, width).
-        """
-        UtilsCoords.__init__(self, original_size, resized_size)
-        UtilsCrops.__init__(self)
-        ProbeFineTipDetector.__init__(self)
-        self.img_fname = None
-        self.diff_img = None
-        self.mask = None
-        self.org_img = None
-        self.IMG_SIZE = resized_size
-        self.IMG_SIZE_ORIGINAL = original_size
-        self.pixel_detect_thresh = 20
-        self.shadow_threshold = 0.5
-        self.ProbeDetector = ProbeDetector
-        self.crop_init = 50
-
-    def first_cmp(self, curr_img, prev_img, mask, org_img, img_fname=None):
-        """Perform first comparison.
-
-        Args:
-            curr_img (numpy.ndarray): Current image.
-            prev_img (numpy.ndarray): Previous image.
-            mask (numpy.ndarray): Mask image.
-            org_img (numpy.ndarray): Original image.
-            img_fname (str, optional): Image filename. Defaults to None.
-
-        Returns:
-            bool: True if probe is detected, False otherwise.
-        """
-        ret = False
-        self.img_fname = img_fname
-        self.mask = mask
-        self._preprocess_diff_images(curr_img, prev_img)  # Subtraction
-        if not self._apply_threshold():
-            return ret
-        ret = self.ProbeDetector.first_detect_probe(self.diff_img, self.mask)
-        if ret:
-            logger.debug("CurrPrevCmpProcessor First::detect")
-            ret_precise_tip = self._get_precise_tip(org_img)
-
-        return ret
-
-    def update_cmp(self, curr_img, prev_img, mask, org_img, img_fname=None):
-        """Update the comparison.
-
-        Args:
-            curr_img (numpy.ndarray): Current image.
-            prev_img (numpy.ndarray): Previous image.
-            mask (numpy.ndarray): Mask image.
-            org_img (numpy.ndarray): Original image.
-            img_fname (str, optional): Image filename. Defaults to None.
-
-        Returns:
-            bool: True if probe is detected and precise tip is found, False otherwise.
-        """
-        ret = False
-        self.img_fname = img_fname
-        self.mask = mask
-        self._preprocess_diff_images(curr_img, prev_img)  # Subtraction
-        if not self._apply_threshold():
-            return False
-        ret = self._update_crop()
-        if ret:
-            logger.debug("CurrPrevCmpProcessor Update::detect")
-            ret_precise_tip = self._get_precise_tip(org_img)
-
-        return ret and ret_precise_tip
-
-    def _update_crop(self):
-        """Update the crop region.
-
-        Returns:
-            bool: True if probe is detected, False otherwise.
-        """
-        # Draw
-        # diff_img_ = self.diff_img.copy()
-        # diff_img_ = cv2.cvtColor(diff_img_, cv2.COLOR_GRAY2BGR)
-
-        ret = False
-        crop_size = self.crop_init
-        crop_utils = UtilsCrops()
-        while (ret is False) and (
-            crop_size <= max(self.IMG_SIZE[0], self.IMG_SIZE[1])
-        ):
-            top, bottom, left, right = crop_utils.calculate_crop_region(
-                self.ProbeDetector.probe_tip,
-                self.ProbeDetector.probe_base,
-                crop_size,
-                self.IMG_SIZE,
-            )
-            diff_img_crop = self.diff_img[top:bottom, left:right]
-            hough_minLineLength_adpative = (
-                40 + int(crop_size / self.crop_init) * 5
-            )
-            ret = self.ProbeDetector.update_probe(
-                diff_img_crop,
-                self.mask,
-                hough_minLineLength=hough_minLineLength_adpative,
-                offset_x=left,
-                offset_y=top,
-                img_fname=self.img_fname,
-            )
-            # cv2.rectangle(diff_img_, (left, top), (right, bottom), (0, 155, 155), 5)  # Green rectangle
-
-            if ret and crop_utils.is_point_on_crop_region(
-                self.ProbeDetector.probe_tip, top, bottom, left, right
-            ):
-                ret = False
-
-            """
-            if ret:
-                cv2.circle(diff_img_, self.ProbeDetector.probe_tip, 3, (0, 0, 255), -1)  # RED circle
-                cv2.circle(diff_img_, self.ProbeDetector.probe_base, 3, (0, 255, 0), -1)  # RED circle
-                #output_fname = os.path.basename(self.img_fname).replace('.', '_2_diff_thres.')
-                #cv2.imwrite('output/' + output_fname, diff_img_)
-                break
-            """
-
-            crop_size += 100
-
-        del crop_utils  # Garbage Collect
-        return ret
-
-    def _get_precise_tip(self, org_img):
-        """Get precise probe tip using original image
-
-        Args:
-            org_img (numpy.ndarray): Original image.
-
-        Returns:
-            bool: True if precise tip is found, False otherwise.
-        """
-        coords_utils = UtilsCoords(self.IMG_SIZE_ORIGINAL, self.IMG_SIZE)
-        probe_fine_tip = ProbeFineTipDetector()
-        crop_utils = UtilsCrops()
-        ret = False
-
-        probe_tip_original_coords = coords_utils.scale_coords_to_original(
-            self.ProbeDetector.probe_tip
-        )
-        top, bottom, left, right = crop_utils.calculate_crop_region(
-            probe_tip_original_coords,
-            probe_tip_original_coords,
-            crop_size=25,
-            IMG_SIZE=self.IMG_SIZE_ORIGINAL,
-        )
-        self.tip_image = org_img[top:bottom, left:right]
-        ret = probe_fine_tip.get_precise_tip(
-            self.tip_image,
-            probe_tip_original_coords,
-            offset_x=left,
-            offset_y=top,
-            direction=self.ProbeDetector.probe_tip_direction,
-            img_fname=self.img_fname,
-        )
-        if ret:
-            self.ProbeDetector.probe_tip_org = probe_fine_tip.tip
-
-        del probe_fine_tip  # Garbage Collect
-        del coords_utils
-        del crop_utils
-
-        return ret
-
-    def _detect_probe(self):
-        """Detect probe in difference image.
-
-        Returns:
-            bool: True if probe is detected, False otherwise.
-        """
-        return self.ProbeDetector.first_detect_probe(self.diff_img, self.mask)
-
-    def _preprocess_diff_images(self, curr_img, prev_img):
-        """Subtract current image from previous image to find differences.
-
-        Args:
-            curr_img (numpy.ndarray): Current image.
-            prev_img (numpy.ndarray): Previous image.
-        """
-        self.diff_img = cv2.subtract(prev_img, curr_img, mask=self.mask)
-        # output_fname = os.path.basename(self.img_fname).replace('.', '_2_diff.')
-        # cv2.imwrite('output/' + output_fname, self.diff_img)
-
-    def _apply_threshold(self):
-        """Apply threshold to suppress shadows and check significant differences.
-
-        Returns:
-            bool: True if significant differences are found, False otherwise.
-        """
-        max_value = np.max(self.diff_img)
-        if max_value < 20:
-            logger.debug(
-                f"Not strong pattern detected on diff image. max_value: {max_value}"
-            )
-            return False
-
-        threshold_value = self.shadow_threshold * max_value
-        self.diff_img[self.diff_img < threshold_value] = 0
-        _, self.diff_img = cv2.threshold(
-            self.diff_img, 0, 255, cv2.THRESH_BINARY + cv2.THRESH_OTSU
-        )
-        self.diff_img = cv2.bitwise_and(
-            self.diff_img, self.diff_img, mask=self.mask
-        )
-
+"""
+CurrPrevCmpProcessor: Module for finding the difference image 
+using Current Previous Comparison.
+
+This module provides classes and methods for processing images
+to detect differences between a current image and a previous image, with the aim of detecting a probe and its tip.
+
+Classes:
+    - CurrPrevCmpProcessor: Main class for performing
+      the comparison and detecting the probe.
+
+Usage:
+    - Initialize an instance of CurrPrevCmpProcessor with necessary parameters.
+    - Use the first_cmp() method to perform the initial comparison.
+    - Use the update_cmp() method to update the comparison
+      and detect changes over time.
+"""
+
+import logging
+import os
+
+import cv2
+import numpy as np
+
+from .probe_fine_tip_detector import ProbeFineTipDetector
+from .utils import UtilsCoords, UtilsCrops
+
+# Set logger name
+logger = logging.getLogger(__name__)
+# Set the logging level for PyQt5.uic.uiparser/properties
+logging.getLogger("PyQt5.uic.uiparser").setLevel(logging.WARNING)
+logging.getLogger("PyQt5.uic.properties").setLevel(logging.WARNING)
+
+
+class CurrPrevCmpProcessor(UtilsCoords, UtilsCrops, ProbeFineTipDetector):
+    """Finding diff image using Current Previous Comparison"""
+
+    def __init__(self, ProbeDetector, original_size, resized_size):
+        """
+        Initialize the CurrPrevCmpProcessor.
+
+        Args:
+            ProbeDetector (object): An instance of the ProbeDetector class.
+            original_size (tuple): The original size of the image (height, width).
+            resized_size (tuple): The resized size of the image (height, width).
+        """
+        UtilsCoords.__init__(self, original_size, resized_size)
+        UtilsCrops.__init__(self)
+        ProbeFineTipDetector.__init__(self)
+        self.img_fname = None
+        self.diff_img = None
+        self.mask = None
+        self.org_img = None
+        self.IMG_SIZE = resized_size
+        self.IMG_SIZE_ORIGINAL = original_size
+        self.pixel_detect_thresh = 20
+        self.shadow_threshold = 0.5
+        self.ProbeDetector = ProbeDetector
+        self.crop_init = 50
+
+    def first_cmp(self, curr_img, prev_img, mask, org_img, img_fname=None):
+        """Perform first comparison.
+
+        Args:
+            curr_img (numpy.ndarray): Current image.
+            prev_img (numpy.ndarray): Previous image.
+            mask (numpy.ndarray): Mask image.
+            org_img (numpy.ndarray): Original image.
+            img_fname (str, optional): Image filename. Defaults to None.
+
+        Returns:
+            bool: True if probe is detected, False otherwise.
+        """
+        ret = False
+        self.img_fname = img_fname
+        self.mask = mask
+        self._preprocess_diff_images(curr_img, prev_img)  # Subtraction
+        if not self._apply_threshold():
+            return ret
+        ret = self.ProbeDetector.first_detect_probe(self.diff_img, self.mask)
+        if ret:
+            logger.debug("CurrPrevCmpProcessor First::detect")
+            ret_precise_tip = self._get_precise_tip(org_img)
+
+        return ret
+
+    def update_cmp(self, curr_img, prev_img, mask, org_img, img_fname=None):
+        """Update the comparison.
+
+        Args:
+            curr_img (numpy.ndarray): Current image.
+            prev_img (numpy.ndarray): Previous image.
+            mask (numpy.ndarray): Mask image.
+            org_img (numpy.ndarray): Original image.
+            img_fname (str, optional): Image filename. Defaults to None.
+
+        Returns:
+            bool: True if probe is detected and precise tip is found, False otherwise.
+        """
+        ret = False
+        self.img_fname = img_fname
+        self.mask = mask
+        self._preprocess_diff_images(curr_img, prev_img)  # Subtraction
+        if not self._apply_threshold():
+            return False
+        ret = self._update_crop()
+        if ret:
+            logger.debug("CurrPrevCmpProcessor Update::detect")
+            ret_precise_tip = self._get_precise_tip(org_img)
+
+        return ret and ret_precise_tip
+
+    def _update_crop(self):
+        """Update the crop region.
+
+        Returns:
+            bool: True if probe is detected, False otherwise.
+        """
+        # Draw
+        # diff_img_ = self.diff_img.copy()
+        # diff_img_ = cv2.cvtColor(diff_img_, cv2.COLOR_GRAY2BGR)
+
+        ret = False
+        crop_size = self.crop_init
+        crop_utils = UtilsCrops()
+        while (ret is False) and (
+            crop_size <= max(self.IMG_SIZE[0], self.IMG_SIZE[1])
+        ):
+            top, bottom, left, right = crop_utils.calculate_crop_region(
+                self.ProbeDetector.probe_tip,
+                self.ProbeDetector.probe_base,
+                crop_size,
+                self.IMG_SIZE,
+            )
+            diff_img_crop = self.diff_img[top:bottom, left:right]
+            hough_minLineLength_adpative = (
+                40 + int(crop_size / self.crop_init) * 5
+            )
+            ret = self.ProbeDetector.update_probe(
+                diff_img_crop,
+                self.mask,
+                hough_minLineLength=hough_minLineLength_adpative,
+                offset_x=left,
+                offset_y=top,
+                img_fname=self.img_fname,
+            )
+            # cv2.rectangle(diff_img_, (left, top), (right, bottom), (0, 155, 155), 5)  # Green rectangle
+
+            if ret and crop_utils.is_point_on_crop_region(
+                self.ProbeDetector.probe_tip, top, bottom, left, right
+            ):
+                ret = False
+
+            """
+            if ret:
+                cv2.circle(diff_img_, self.ProbeDetector.probe_tip, 3, (0, 0, 255), -1)  # RED circle
+                cv2.circle(diff_img_, self.ProbeDetector.probe_base, 3, (0, 255, 0), -1)  # RED circle
+                #output_fname = os.path.basename(self.img_fname).replace('.', '_2_diff_thres.')
+                #cv2.imwrite('output/' + output_fname, diff_img_)
+                break
+            """
+
+            crop_size += 100
+
+        del crop_utils  # Garbage Collect
+        return ret
+
+    def _get_precise_tip(self, org_img):
+        """Get precise probe tip using original image
+
+        Args:
+            org_img (numpy.ndarray): Original image.
+
+        Returns:
+            bool: True if precise tip is found, False otherwise.
+        """
+        coords_utils = UtilsCoords(self.IMG_SIZE_ORIGINAL, self.IMG_SIZE)
+        probe_fine_tip = ProbeFineTipDetector()
+        crop_utils = UtilsCrops()
+        ret = False
+
+        probe_tip_original_coords = coords_utils.scale_coords_to_original(
+            self.ProbeDetector.probe_tip
+        )
+        top, bottom, left, right = crop_utils.calculate_crop_region(
+            probe_tip_original_coords,
+            probe_tip_original_coords,
+            crop_size=25,
+            IMG_SIZE=self.IMG_SIZE_ORIGINAL,
+        )
+        self.tip_image = org_img[top:bottom, left:right]
+        ret = probe_fine_tip.get_precise_tip(
+            self.tip_image,
+            probe_tip_original_coords,
+            offset_x=left,
+            offset_y=top,
+            direction=self.ProbeDetector.probe_tip_direction,
+            img_fname=self.img_fname,
+        )
+        if ret:
+            self.ProbeDetector.probe_tip_org = probe_fine_tip.tip
+
+        del probe_fine_tip  # Garbage Collect
+        del coords_utils
+        del crop_utils
+
+        return ret
+
+    def _detect_probe(self):
+        """Detect probe in difference image.
+
+        Returns:
+            bool: True if probe is detected, False otherwise.
+        """
+        return self.ProbeDetector.first_detect_probe(self.diff_img, self.mask)
+
+    def _preprocess_diff_images(self, curr_img, prev_img):
+        """Subtract current image from previous image to find differences.
+
+        Args:
+            curr_img (numpy.ndarray): Current image.
+            prev_img (numpy.ndarray): Previous image.
+        """
+        self.diff_img = cv2.subtract(prev_img, curr_img, mask=self.mask)
+        # output_fname = os.path.basename(self.img_fname).replace('.', '_2_diff.')
+        # cv2.imwrite('output/' + output_fname, self.diff_img)
+
+    def _apply_threshold(self):
+        """Apply threshold to suppress shadows and check significant differences.
+
+        Returns:
+            bool: True if significant differences are found, False otherwise.
+        """
+        max_value = np.max(self.diff_img)
+        if max_value < 20:
+            logger.debug(
+                f"Not strong pattern detected on diff image. max_value: {max_value}"
+            )
+            return False
+
+        threshold_value = self.shadow_threshold * max_value
+        self.diff_img[self.diff_img < threshold_value] = 0
+        _, self.diff_img = cv2.threshold(
+            self.diff_img, 0, 255, cv2.THRESH_BINARY + cv2.THRESH_OTSU
+        )
+        self.diff_img = cv2.bitwise_and(
+            self.diff_img, self.diff_img, mask=self.mask
+        )
+
         return True
```

### Comparing `parallax_app-0.37.1/parallax/main_window_wip.py` & `parallax_app-0.37.5/parallax/main_window_wip.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,775 +1,775 @@
-"""
-This script defines the main components of the application
-including the main window, UI elements,
-camera and stage management, and recording functionality.
-
-Modules imported:
-- PyQt5 modules for building the graphical user interface.
-- Other libraries and modules necessary for the application's functionality.
-
-Classes:
-- MainWindow: Represents the main window of the application.
-"""
-
-import logging
-import os
-from functools import partial
-
-from PyQt5.QtCore import QCoreApplication, QPoint, QStandardPaths, QTimer
-from PyQt5.QtGui import QFont, QFontDatabase
-# Import required PyQt5 modules and other libraries
-from PyQt5.QtWidgets import (QApplication, QFileDialog, QGridLayout, QGroupBox,
-                             QMainWindow, QScrollArea, QSplitter, QToolButton,
-                             QVBoxLayout, QWidget)
-from PyQt5.uic import loadUi
-
-from .recording_manager import RecordingManager
-from .screen_widget import ScreenWidget
-from .stage_widget import StageWidget
-from .user_setting_manager import UserSettingsManager
-
-# Set logger name
-logger = logging.getLogger(__name__)
-# Set the logging level for PyQt5.uic.uiparser/properties
-logging.getLogger("PyQt5.uic.uiparser").setLevel(logging.WARNING)
-logging.getLogger("PyQt5.uic.properties").setLevel(logging.WARNING)
-
-# User Preferences (Data directory, UI config..) setting file
-package_dir = os.path.dirname(os.path.abspath(__file__))
-ui_dir = os.path.join(os.path.dirname(package_dir), "ui")
-SETTINGS_FILE = "settings.json"
-
-
-# Main application window
-class MainWindow(QMainWindow):
-    """
-    The main window of the application.
-
-    This class represents the main window of the application
-    and handles the user interface
-    components, camera and stage management, and recording functionality.
-    """
-
-    def __init__(self, model, dummy=False):
-        """
-        Initialize the MainWindow.
-
-        Args:
-            model (object): The data model for the application.
-            dummy (bool, optional): Flag indicating whether
-            to run in dummy mode. Defaults to False.
-        """
-        QMainWindow.__init__(self)  # Initialize the QMainWindow
-        self.model = model
-        self.dummy = dummy
-        
-        # Initialize an empty list to keep track of microscopeGrp widgets instances
-        self.screen_widgets = []
-        self.recording_camera_list = []
-
-        # Update camera information
-        self.refresh_cameras()
-        logger.debug(
-            f"nPySpinCameras: {self.model.nPySpinCameras}, nMockCameras: {self.model.nMockCameras}"
-        )
-
-        # Update stage information
-        self.refresh_stages()
-        logger.debug(f"stages: {self.model.stages}")
-
-        self.user_setting = UserSettingsManager()
-        # Load column configuration from user preferences
-        self.nColumn = self.user_setting.load_settings_item("main", "nColumn")
-        if self.nColumn is None or 0:
-            self.nColumn = 1
-        if self.model.nPySpinCameras:
-            self.nColumn = min(self.model.nPySpinCameras, self.nColumn)
-
-        # Load the main widget with UI components
-        ui = os.path.join(ui_dir, "mainWindow.ui")
-        loadUi(ui, self)
-
-        # Load Fira Code font
-        fira_code_font_path = os.path.join(
-            ui_dir, "font/FiraCode-VariableFont_wght.ttf"
-        )
-        QFontDatabase.addApplicationFont(fira_code_font_path)
-        fira_code_font = QFont("Fira Code Light", 10)  # Setting font size to 10
-        QApplication.setFont(fira_code_font)
-
-        # Load existing user preferences
-        nColumn, directory, width, height = (
-            self.user_setting.load_mainWindow_settings()
-        )
-        self.nColumnsSpinBox.setValue(nColumn)
-        self.dirLabel.setText(directory)
-        if width is not None and height is not None:
-            self.resize(width, height)
-
-        # Attach directory selection event handler for saving files
-        self.browseDirButton.clicked.connect(self.dir_setting_handler)
-
-        # Configure the column spin box
-        self.nColumnsSpinBox.setMaximum(max(self.model.nPySpinCameras, 1))
-        self.nColumnsSpinBox.setValue(self.nColumn)
-        if self.model.nPySpinCameras:
-            self.nColumnsSpinBox.valueChanged.connect(
-                self.column_changed_handler
-            )
-
-        # Refreshing the settingMenu while it is toggled
-        self.settings_refresh_timer = QTimer()
-
-        # Create the widget for screen
-        self.scrollArea = QScrollArea(self.centralwidget)
-        self.scrollArea.setWidgetResizable(True)
-        self.scrollArea.setObjectName("scrollArea")
-        self.scrollAreaWidgetContents = QWidget()
-        self.scrollAreaWidgetContents.setObjectName("scrollAreaWidgetContents")
-        self.gridLayout = QGridLayout(self.scrollAreaWidgetContents)
-
-        # Dynamically generate Microscope display
-        if self.model.nPySpinCameras:
-            self.display_microscope()  # Attach screen widget
-        else:  # Display only mock camera
-            self.display_mock_camera()
-
-        # Stage_widget
-        self.stage_widget = StageWidget(self.model, ui_dir, self.screen_widgets)
-        splitter = QSplitter()
-        splitter.addWidget(self.scrollAreaWidgetContents)
-        splitter.addWidget(self.stage_widget)
-        self.verticalLayout_4.addWidget(splitter)
-
-        # Start button. If toggled, start camera acquisition
-        self.startButton.clicked.connect(self.start_button_handler)
-
-        # Recording functions
-        self.recordingManager = RecordingManager(self.model)
-        self.snapshotButton.clicked.connect(
-            lambda: self.recordingManager.save_last_image(
-                self.dirLabel.text(), self.screen_widgets
-            )
-        )
-        self.recordButton.clicked.connect(
-            self.record_button_handler
-        )  # Recording video button
-
-        # Refreshing the screen timer
-        self.refresh_timer = QTimer()
-        self.refresh_timer.timeout.connect(self.refresh)
-
-        # Toggle start button on init
-        self.start_button_handler()
-
-    def refresh_cameras(self):
-        """
-        This method is responsible for scanning for available cameras and updating the camera list.
-        It adds mock cameras for testing purposes and scans for actual cameras if the application
-        is not in dummy mode. This ensures that the list of available cameras is always up-to-date.
-        """
-        # Add mock cameras for testing purposes
-        self.model.add_mock_cameras()
-        # If not in dummy mode, scan for actual available cameras
-        if not self.dummy:
-            try:
-                self.model.scan_for_cameras()
-            except Exception as e:
-                print(
-                    f" Something still holds a reference to the camera.\n {e}"
-                )
-
-    def refresh_stages(self):
-        """Search for connected stages"""
-        if not self.dummy:
-            self.model.scan_for_usb_stages()
-
-    def record_button_handler(self):
-        """
-        Handles the record button press event.
-        If the record button is checked, start recording. Otherwise, stop recording.
-        """
-        if self.recordButton.isChecked():
-            save_path = self.dirLabel.text()
-            self.recordingManager.save_recording(save_path, self.screen_widgets)
-        else:
-            self.recordingManager.stop_recording(self.screen_widgets)
-
-    def start_button_handler(self):
-        """
-        Handles the start button press event.
-
-        If the start button is checked, initiate acquisition from all cameras and start refreshing images.
-        If unchecked, stop acquisition from all cameras and stop refreshing images.
-        """
-        # Initialize the list to keep track of cameras that have been started or stopped
-        refresh_camera_list = []
-
-        # Check if the start button is toggled on
-        if self.startButton.isChecked():
-            print("\nRefreshing Screen")
-            # Camera begin acquisition
-            for screen in self.screen_widgets:
-                camera_name = screen.get_camera_name()
-                if camera_name not in refresh_camera_list:
-                    screen.start_acquisition_camera()
-                    refresh_camera_list.append(camera_name)
-
-            # Refreshing images to display screen
-            self.refresh_timer.start(125)
-
-            # Start button is checked, enable record and snapshot button.
-            self.recordButton.setEnabled(True)
-            self.snapshotButton.setEnabled(True)
-
-        else:
-            print("Stop Refreshing Screen")
-            # Start button is unchecked, disable record and snapshot button.
-            self.recordButton.setEnabled(False)
-            self.recordButton.setChecked(False)
-            self.snapshotButton.setEnabled(False)
-
-            # Stop Refresh: stop refreshing images to display screen
-            if self.refresh_timer.isActive():
-                self.refresh_timer.stop()
-
-            # End acquisition from camera: stop acquiring images from camera to framebuffer
-            for screen in self.screen_widgets:
-                camera_name = screen.get_camera_name()
-                if camera_name not in refresh_camera_list:
-                    screen.stop_acquisition_camera()
-                    refresh_camera_list.append(camera_name)
-
-    def refresh(self):
-        """Refreshing from framebuffer to screen"""
-        for screen in self.screen_widgets:
-            screen.refresh()  # Refresh the screens
-
-    def display_mock_camera(self):
-        """Display mock camera when there is no detected camera."""
-        self.createNewGroupBox(0, 0, mock=True)
-
-    def display_microscope(self):
-        """Dynamically arrange Microscopes based on camera count and column configuration."""
-        # Calculate rows and columns
-        rows, cols, cnt = (
-            self.model.nPySpinCameras // self.nColumn,
-            self.nColumn,
-            0,
-        )
-        rows += 1 if self.model.nPySpinCameras % cols else 0
-        # Create grid of Microscope displays
-        for row_idx in range(0, rows):
-            for col_idx in range(0, cols):
-                if cnt < self.model.nPySpinCameras:
-                    self.createNewGroupBox(row_idx, col_idx, screen_index=cnt)
-                    cnt += 1
-                else:
-                    break  # Stop when all Microscopes are displayed
-
-    def column_changed_handler(self, val):
-        """Rearrange the layout of Microscopes when the column number changes."""
-        # Identify current Microscope widgets
-        camera_screen_list = []
-        # Detach the identified widgets
-        for i in range(self.gridLayout.count()):
-            widget = self.gridLayout.itemAt(i).widget()
-            if isinstance(
-                widget, QGroupBox
-            ):  # Ensure we're handling the correct type of widget
-                camera_screen_list.append(widget)
-
-        # Detach the identified widgets
-        for widget in camera_screen_list:
-            self.gridLayout.removeWidget(widget)
-            widget.hide()  # Temporarily hide the widget
-
-        # Calculate new rows and columns layout
-        rows, cols, cnt = self.model.nPySpinCameras // val, val, 0
-        rows += 1 if self.model.nPySpinCameras % cols else 0
-
-        # Reattach widgets in the new layout
-        for row_idx in range(0, rows):
-            for col_idx in range(0, cols):
-                if cnt < len(camera_screen_list):
-                    widget = camera_screen_list[cnt]
-                    self.gridLayout.addWidget(widget, row_idx, col_idx, 1, 1)
-                    widget.show()  # Make the widget visible again
-                    cnt += 1
-                else:
-                    break
-
-    def createNewGroupBox(self, rows, cols, mock=False, screen_index=None):
-        """
-        Create a new group box widget representing a microscope, and add it to the grid layout.
-        This function is responsible for generating a unique name for the microscope, creating a group box to
-        represent it, adding a screen widget for camera display, a settings button, and configuring their
-        properties and layouts. It also adds the group box to the grid layout at the specified row and column
-        indices, and updates the settings menu for the microscope.
-
-        Parameters:
-        - rows (int): The row index in the grid layout where the group box should be added.
-        - cols (int): The column index in the grid layout where the group box should be added.
-        - mock (bool, optional): If True, a mock camera will be associated with this microscope. Default is False.
-        - screen_index (int, optional): The index of the camera in the model's camera list to be associated
-        with this microscope. Required if mock is False.
-        """
-        # Generate unique names based on row and column indices
-        newNameMicroscope = ""
-        # Generate unique names based on camera number
-        if mock:
-            newNameMicroscope = "Mock Camera"
-        else:
-            newNameMicroscope = f"Microscope_{screen_index+1}"
-        microscopeGrp = QGroupBox(self.scrollAreaWidgetContents)
-
-        # Construct and configure the Microscope widget
-        microscopeGrp.setObjectName(newNameMicroscope)
-        microscopeGrp.setStyleSheet("background-color: rgb(58, 58, 58);")
-        font_grpbox = QFont()
-        font_grpbox.setPointSize(9)  # Setting font size to 9
-        microscopeGrp.setFont(font_grpbox)
-        verticalLayout = QVBoxLayout(microscopeGrp)
-        verticalLayout.setObjectName("verticalLayout")
-
-        # Add screens
-        if mock:
-            screen = ScreenWidget(
-                self.model.cameras[0], model=self.model, parent=microscopeGrp
-            )
-        else:
-            screen = ScreenWidget(
-                self.model.cameras[screen_index],
-                model=self.model,
-                parent=microscopeGrp,
-            )
-        screen.setObjectName(f"Screen")
-        verticalLayout.addWidget(screen)
-
-        if mock is False:
-            # Add setting button
-            settingButton = QToolButton(microscopeGrp)
-            settingButton.setObjectName(f"Setting")
-            settingButton.setFont(font_grpbox)
-            settingButton.setCheckable(True)
-            self.create_settings_menu(
-                microscopeGrp, newNameMicroscope, screen, screen_index
-            )
-            settingButton.toggled.connect(
-                lambda checked: self.show_settings_menu(settingButton, checked)
-            )
-            verticalLayout.addWidget(settingButton)
-            settingButton.setText(
-                QCoreApplication.translate(
-                    "MainWindow", "SETTINGS \u25ba", None
-                )
-            )
-
-            # Load setting file from JSON
-            self.update_setting_menu(microscopeGrp)
-
-        # Add widget to the gridlayout
-        self.gridLayout.addWidget(microscopeGrp, rows, cols, 1, 1)
-
-        # Add the new microscopeGrpBox instance to the list
-        self.screen_widgets.append(screen)
-
-    def create_settings_menu(
-        self, microscopeGrp, newNameMicroscope, screen, screen_index
-    ):
-        """
-        Create the settings menu for each Microscope widget.
-
-        This function initializes the settings menu UI, loads it with necessary data,
-        and associates the relevant signals with their slots.
-        The settings menu is hidden by default and will be shown
-        when the user toggles the settings button.
-
-        Parameters:
-        - microscopeGrp (QGroupBox): The group box representing a Microscope widget.
-        - newNameMicroscope (str): The unique name assigned to the Microscope widget.
-        - screen (ScreenWidget): The screen widget associated with the Microscope.
-        - screen_index (int): The index of the camera in the model's camera list to be associated with this screen.
-        """
-        # Initialize the settings menu UI from the .ui file
-        settingMenu = QWidget(microscopeGrp)
-        setting_ui = os.path.join(ui_dir, "settingPopUpMenu.ui")
-        loadUi(setting_ui, settingMenu)
-        settingMenu.setObjectName("SettingsMenu")
-        settingMenu.hide()  # Hide the menu by default
-
-        # S/N
-        # Add the list of cameras (serial number) in ComboBox
-        for sn in self.model.cameras_sn:        
-            settingMenu.snComboBox.addItem(sn) 
-        # Select the sn for the current screen
-        sn = screen.get_camera_name()           
-        index = settingMenu.snComboBox.findText(sn)
-        if index >= 0:
-            settingMenu.snComboBox.setCurrentIndex(index)
-        else:
-            logger.error("SN not found in the list")
-
-        # If serial number is changed, connect to update_screen function and update setting menu
-        settingMenu.snComboBox.currentIndexChanged.connect(
-            lambda: self.update_screen(
-                screen, screen_index, settingMenu.snComboBox.currentText()
-            )
-        )
-
-        # Custom name
-        customName = self.user_setting.load_settings_item(
-            sn, "customName"
-        )  # Default name on init
-        customName = customName if customName else newNameMicroscope
-        settingMenu.customName.setText(customName)
-        self.update_groupbox_name(
-            microscopeGrp, customName
-        )  # Update GroupBox name
-        # Name) If custom name is changed, change the groupBox name.
-        settingMenu.customName.textChanged.connect(
-            lambda: self.update_groupbox_name(
-                microscopeGrp, settingMenu.customName.text()
-            )
-        )
-        settingMenu.customName.textChanged.connect(
-            lambda: self.user_setting.update_user_configs_settingMenu(
-                microscopeGrp, "customName", settingMenu.customName.text()
-            )
-        )
-
-        # Exposure
-        settingMenu.expSlider.valueChanged.connect(
-            lambda: screen.set_camera_setting(
-                setting="exposure", val=settingMenu.expSlider.value() * 1000
-            )
-        )
-        settingMenu.expSlider.valueChanged.connect(
-            lambda: settingMenu.expNum.setNum(settingMenu.expSlider.value())
-        )
-        settingMenu.expSlider.valueChanged.connect(
-            lambda: self.user_setting.update_user_configs_settingMenu(
-                microscopeGrp, "exp", settingMenu.expSlider.value()
-            )
-        )
-        settingMenu.expAuto.clicked.connect(
-            lambda: settingMenu.expSlider.setValue(
-                int(screen.get_camera_setting(setting="exposure") / 1000)
-            )
-        )
-
-        # Gain
-        settingMenu.gainSlider.valueChanged.connect(
-            lambda: screen.set_camera_setting(
-                setting="gain", val=settingMenu.gainSlider.value()
-            )
-        )
-        settingMenu.gainSlider.valueChanged.connect(
-            lambda: settingMenu.gainNum.setNum(settingMenu.gainSlider.value())
-        )
-        settingMenu.gainSlider.valueChanged.connect(
-            lambda: self.user_setting.update_user_configs_settingMenu(
-                microscopeGrp, "gain", settingMenu.gainSlider.value()
-            )
-        )
-        settingMenu.gainAuto.clicked.connect(
-            lambda: settingMenu.gainSlider.setValue(
-                screen.get_camera_setting(setting="gain")
-            )
-        )
-
-        # Gamma
-        settingMenu.gammaSlider.valueChanged.connect(
-            lambda: screen.set_camera_setting(
-                setting="gamma", val=settingMenu.gammaSlider.value() / 100
-            )
-        )
-        settingMenu.gammaSlider.valueChanged.connect(
-            lambda: settingMenu.gammaNum.setText(
-                "{:.2f}".format(settingMenu.gammaSlider.value() / 100)
-            )
-        )
-        settingMenu.gammaSlider.valueChanged.connect(
-            lambda: self.user_setting.update_user_configs_settingMenu(
-                microscopeGrp, "gamma", settingMenu.gammaSlider.value()
-            )
-        )
-        settingMenu.gammaAuto.clicked.connect(
-            lambda: settingMenu.gammaSlider.setEnabled(
-                not settingMenu.gammaSlider.isEnabled()
-            )
-        )
-        settingMenu.gammaAuto.clicked.connect(
-            lambda: self.user_setting.update_user_configs_settingMenu(
-                microscopeGrp, "gammaAuto", settingMenu.gammaSlider.isEnabled()
-            )
-        )
-
-        # W/B
-        settingLayout = settingMenu.layout()
-        settingLayout.addWidget(settingMenu.wbAuto, 5, 1, 2, 1)
-        # Blue Channel
-        settingMenu.wbSliderBlue.valueChanged.connect(
-            lambda: screen.set_camera_setting(
-                setting="wbBlue", val=settingMenu.wbSliderBlue.value() / 100
-            )
-        )
-        settingMenu.wbSliderBlue.valueChanged.connect(
-            lambda: settingMenu.wbNumBlue.setText(
-                "{:.2f}".format(settingMenu.wbSliderBlue.value() / 100)
-            )
-        )
-        settingMenu.wbSliderBlue.valueChanged.connect(
-            lambda: self.user_setting.update_user_configs_settingMenu(
-                microscopeGrp, "wbBlue", settingMenu.wbSliderBlue.value()
-            )
-        )
-        settingMenu.wbAuto.clicked.connect(
-            lambda: settingMenu.wbSliderBlue.setValue(
-                screen.get_camera_setting(setting="wbBlue") * 100
-            )
-        )
-
-        # Red Channel
-        settingMenu.wbSliderRed.valueChanged.connect(
-            lambda: screen.set_camera_setting(
-                setting="wbRed", val=settingMenu.wbSliderRed.value() / 100
-            )
-        )
-        settingMenu.wbSliderRed.valueChanged.connect(
-            lambda: settingMenu.wbNumRed.setText(
-                "{:.2f}".format(settingMenu.wbSliderRed.value() / 100)
-            )
-        )
-        settingMenu.wbSliderRed.valueChanged.connect(
-            lambda: self.user_setting.update_user_configs_settingMenu(
-                microscopeGrp, "wbRed", settingMenu.wbSliderRed.value()
-            )
-        )
-        settingMenu.wbAuto.clicked.connect(
-            lambda: settingMenu.wbSliderRed.setValue(
-                screen.get_camera_setting(setting="wbRed") * 100
-            )
-        )
-
-    def update_screen(self, screen, screen_index, selected_sn):
-        """
-        Update the screen with a new camera based on the selected serial number.
-
-        This method manages the update of the camera associated with a specific microscope screen. It takes into
-        account the current state of the application, i.e., whether acquisition is ongoing or not, and performs
-        the necessary actions to update the camera and manage acquisition accordingly.
-
-        Parameters:
-        - screen (ScreenWidget): The screen widget associated with the microscope.
-        - screen_index (int): The index of the screen in the list of all microscope screens.
-        - selected_sn (str): The serial number of the camera selected to be associated with the microscope.
-        """
-        # Camera lists that currently attached on the model.
-        camera_list = {
-            camera.name(sn_only=True): camera for camera in self.model.cameras
-        }
-
-        # Get the prev camera lists displaying on the screen
-        prev_camera, curr_camera = screen.get_camera_name(), selected_sn
-        prev_lists = [
-            screen.get_camera_name()
-            for screen in self.screen_widgets
-            if screen.get_camera_name()
-        ]
-        if (
-            0 <= screen_index < len(prev_lists)
-        ):  # Ensure screen_index is within valid range
-            curr_list = prev_lists[:]
-            curr_list.pop(screen_index)
-            curr_list.insert(screen_index, curr_camera)
-        else:
-            logger.error(f"Invalid screen index: {screen_index}")
-        logger.debug(f"prev_list: {prev_lists}")
-        logger.debug(f"curr_list: {curr_list}")
-
-        # Handle updates based on the current state of the application
-        if (
-            self.startButton.isChecked()
-        ):  # If the 'Start' button is enabled (continuous acquisition mode)
-            if set(prev_lists) == set(curr_list):
-                # If the list of cameras hasn't changed, just update the current screen's camera
-                screen.set_camera(camera_list.get(curr_camera))
-            else:
-                if prev_camera not in curr_list:
-                    # If the previous camera has been removed from the list, stop its acquisition
-                    screen.stop_acquisition_camera()
-                    screen.set_camera(camera_list.get(curr_camera))
-                if curr_camera not in prev_lists:
-                    # If the selected camera is new (wasn't in the previous list), start its acquisition
-                    screen.set_camera(camera_list.get(curr_camera))
-                    screen.start_acquisition_camera()
-        else:
-            # If the 'Start' button is disabled, start single frame acquisition to show the image
-            screen.set_camera(camera_list.get(curr_camera))
-            screen.single_acquisition_camera()
-            screen.refresh_single_frame()
-            screen.stop_single_acquisition_camera()
-
-    def update_groupbox_name(self, microscopeGrp, customName):
-        """
-        Update the title and object name of the group box representing a microscope.
-
-        This method is used to update the visual representation of a microscope based on a custom name provided
-        by the user.
-
-        Parameters:
-        - microscopeGrp (QGroupBox): The group box representing the microscope.
-        - customName (str): The custom name to set as the title and object name of the group box.
-        """
-        if customName:
-            microscopeGrp.setTitle(customName)
-            microscopeGrp.setObjectName(customName)
-
-    def show_settings_menu(self, settingButton, is_checked):
-        """
-        Show or hide the settings menu associated with a microscope group box.
-
-        This method is connected to the toggled signal of a QToolButton, which represents
-        the settings button for a microscope group box. When the button is toggled, it
-        shows or hides the settings menu and starts or stops a timer to refresh the settings
-        values displayed in the menu.
-
-        Parameters:
-        - settingButton (QToolButton): The settings button associated with the microscope group box.
-        - is_checked (bool): Indicates whether the settings button is checked (True) or unchecked (False).
-        """
-        microscopeGrp = settingButton.parent()
-        # Find the settingMenu within this microscopeGrp
-        settingMenu = microscopeGrp.findChild(QWidget, "SettingsMenu")
-        self.settings_refresh_timer.timeout.connect(
-            partial(self.update_setting_menu, microscopeGrp)
-        )
-
-        if is_checked:
-            # If the settings button is checked, start the settings refresh 
-            # timer and show the settings menu
-            # update setting menu every 0.1 sec
-            self.settings_refresh_timer.start(100)      
-            
-
-            # Show the setting menu next to setting button
-            button_position = settingButton.mapToGlobal(settingButton.pos())
-            menu_x = button_position.x() + settingButton.width()
-            menu_x = menu_x - microscopeGrp.mapToGlobal(QPoint(0, 0)).x()
-            menu_y = (
-                settingButton.y()
-                + settingButton.height()
-                - settingMenu.height()
-            )
-            logger.debug(
-                f"(SettingMenu) coordinates of setting menu: x: {menu_x}, y: {menu_y}"
-            )
-            settingMenu.move(menu_x, menu_y)
-            settingMenu.show()
-        else:
-            # If the settings button is unchecked, stop the settings 
-            # refresh timer and hide the settings menu
-            self.settings_refresh_timer.stop()
-            settingMenu.hide()
-
-    def update_setting_menu(self, microscopeGrp):
-        """
-        Update the values displayed in the settings menu based on the current camera settings.
-
-        This method is called periodically by a QTimer to refresh the values displayed in the
-        settings menu, ensuring they are up-to-date with the current settings of the camera.
-
-        Parameters:
-        - microscopeGrp (QGroupBox): The microscope group box associated with the settings menu to be updated.
-        """
-
-        # Find the settingMenu within this microscopeGrp
-        settingMenu = microscopeGrp.findChild(QWidget, "SettingsMenu")
-        screen = microscopeGrp.findChild(ScreenWidget, "Screen")
-
-        # Display the S/N of camera
-        sn = screen.get_camera_name()
-        # Load the saved settings
-        saved_settings = self.user_setting.load_settings_item(sn)
-        if saved_settings:
-            # If saved settings are found, update the sliders in the settings menu with the saved values
-            settingMenu.expSlider.setValue(saved_settings.get("exp", 15))
-            settingMenu.gainSlider.setValue(saved_settings.get("gain", 20))
-
-            # Gamma
-            gammaAuto = saved_settings.get("gammaAuto", None)
-            if gammaAuto == True:
-                settingMenu.gammaSlider.setEnabled(True)
-                settingMenu.gammaSlider.setValue(
-                    saved_settings.get("gamma", 100)
-                )
-            elif gammaAuto == False:
-                settingMenu.gammaSlider.setEnabled(False)
-            else:
-                pass
-
-            # W/B
-            if screen.get_camera_color_type() == "Color":
-                settingMenu.wbAuto.setDisabled(False)
-                settingMenu.wbSliderRed.setDisabled(False)
-                settingMenu.wbSliderBlue.setDisabled(False)
-                settingMenu.wbSliderRed.setValue(
-                    saved_settings.get("wbRed", 1.2)
-                )
-                settingMenu.wbSliderBlue.setValue(
-                    saved_settings.get("wbBlue", 2.8)
-                )
-            elif screen.get_camera_color_type() == "Mono":
-                settingMenu.wbAuto.setDisabled(True)
-                settingMenu.wbSliderRed.setDisabled(True)
-                settingMenu.wbSliderBlue.setDisabled(True)
-                settingMenu.wbNumRed.setText("--")
-                settingMenu.wbNumBlue.setText("--")
-
-        else:
-            settingMenu.gainAuto.click()
-            settingMenu.wbAuto.click()
-            settingMenu.expAuto.click()
-            self.user_setting.update_user_configs_settingMenu(
-                microscopeGrp, "gammaAuto", True
-            )
-            self.user_setting.update_user_configs_settingMenu(
-                microscopeGrp, "gamma", settingMenu.gammaSlider.value()
-            )
-
-    def dir_setting_handler(self):
-        """
-        This method handles the selection of a directory for saving files. It opens a dialog that allows
-        the user to browse their filesystem and select a directory. The selected directory's path is then
-        displayed on the user interface.
-
-        This is a crucial function for users who need to save data or configurations, as it provides a
-        simple and intuitive way to specify the location where files should be saved.
-        """
-        # Fetch the default documents directory path
-        documents_dir = QStandardPaths.writableLocation(
-            QStandardPaths.DocumentsLocation
-        )
-        # Open a dialog to allow the user to select a directory
-        directory = QFileDialog.getExistingDirectory(
-            self, "Select Directory", documents_dir
-        )
-        # If a directory is chosen, update the label to display the chosen path
-        if directory:
-            self.dirLabel.setText(directory)
-
-    def save_user_configs(self):
-        """
-        Saves user configuration settings to a persistent storage.
-
-        This method retrieves current configuration values from the UI, including
-        the number of columns (nColumn), directory path (directory), and the window's
-        width and height. It then passes these values to the `save_user_configs` method
-        of the `user_setting` object to be saved.
-        """
-        nColumn = self.nColumnsSpinBox.value()
-        directory = self.dirLabel.text()
-        width = self.width()
-        height = self.height()
-        self.user_setting.save_user_configs(nColumn, directory, width, height)
+"""
+This script defines the main components of the application
+including the main window, UI elements,
+camera and stage management, and recording functionality.
+
+Modules imported:
+- PyQt5 modules for building the graphical user interface.
+- Other libraries and modules necessary for the application's functionality.
+
+Classes:
+- MainWindow: Represents the main window of the application.
+"""
+
+import logging
+import os
+from functools import partial
+
+from PyQt5.QtCore import QCoreApplication, QPoint, QStandardPaths, QTimer
+from PyQt5.QtGui import QFont, QFontDatabase
+# Import required PyQt5 modules and other libraries
+from PyQt5.QtWidgets import (QApplication, QFileDialog, QGridLayout, QGroupBox,
+                             QMainWindow, QScrollArea, QSplitter, QToolButton,
+                             QVBoxLayout, QWidget)
+from PyQt5.uic import loadUi
+
+from .recording_manager import RecordingManager
+from .screen_widget import ScreenWidget
+from .stage_widget import StageWidget
+from .user_setting_manager import UserSettingsManager
+
+# Set logger name
+logger = logging.getLogger(__name__)
+# Set the logging level for PyQt5.uic.uiparser/properties
+logging.getLogger("PyQt5.uic.uiparser").setLevel(logging.WARNING)
+logging.getLogger("PyQt5.uic.properties").setLevel(logging.WARNING)
+
+# User Preferences (Data directory, UI config..) setting file
+package_dir = os.path.dirname(os.path.abspath(__file__))
+ui_dir = os.path.join(os.path.dirname(package_dir), "ui")
+SETTINGS_FILE = "settings.json"
+
+
+# Main application window
+class MainWindow(QMainWindow):
+    """
+    The main window of the application.
+
+    This class represents the main window of the application
+    and handles the user interface
+    components, camera and stage management, and recording functionality.
+    """
+
+    def __init__(self, model, dummy=False):
+        """
+        Initialize the MainWindow.
+
+        Args:
+            model (object): The data model for the application.
+            dummy (bool, optional): Flag indicating whether
+            to run in dummy mode. Defaults to False.
+        """
+        QMainWindow.__init__(self)  # Initialize the QMainWindow
+        self.model = model
+        self.dummy = dummy
+        
+        # Initialize an empty list to keep track of microscopeGrp widgets instances
+        self.screen_widgets = []
+        self.recording_camera_list = []
+
+        # Update camera information
+        self.refresh_cameras()
+        logger.debug(
+            f"nPySpinCameras: {self.model.nPySpinCameras}, nMockCameras: {self.model.nMockCameras}"
+        )
+
+        # Update stage information
+        self.refresh_stages()
+        logger.debug(f"stages: {self.model.stages}")
+
+        self.user_setting = UserSettingsManager()
+        # Load column configuration from user preferences
+        self.nColumn = self.user_setting.load_settings_item("main", "nColumn")
+        if self.nColumn is None or 0:
+            self.nColumn = 1
+        if self.model.nPySpinCameras:
+            self.nColumn = min(self.model.nPySpinCameras, self.nColumn)
+
+        # Load the main widget with UI components
+        ui = os.path.join(ui_dir, "mainWindow.ui")
+        loadUi(ui, self)
+
+        # Load Fira Code font
+        fira_code_font_path = os.path.join(
+            ui_dir, "font/FiraCode-VariableFont_wght.ttf"
+        )
+        QFontDatabase.addApplicationFont(fira_code_font_path)
+        fira_code_font = QFont("Fira Code Light", 10)  # Setting font size to 10
+        QApplication.setFont(fira_code_font)
+
+        # Load existing user preferences
+        nColumn, directory, width, height = (
+            self.user_setting.load_mainWindow_settings()
+        )
+        self.nColumnsSpinBox.setValue(nColumn)
+        self.dirLabel.setText(directory)
+        if width is not None and height is not None:
+            self.resize(width, height)
+
+        # Attach directory selection event handler for saving files
+        self.browseDirButton.clicked.connect(self.dir_setting_handler)
+
+        # Configure the column spin box
+        self.nColumnsSpinBox.setMaximum(max(self.model.nPySpinCameras, 1))
+        self.nColumnsSpinBox.setValue(self.nColumn)
+        if self.model.nPySpinCameras:
+            self.nColumnsSpinBox.valueChanged.connect(
+                self.column_changed_handler
+            )
+
+        # Refreshing the settingMenu while it is toggled
+        self.settings_refresh_timer = QTimer()
+
+        # Create the widget for screen
+        self.scrollArea = QScrollArea(self.centralwidget)
+        self.scrollArea.setWidgetResizable(True)
+        self.scrollArea.setObjectName("scrollArea")
+        self.scrollAreaWidgetContents = QWidget()
+        self.scrollAreaWidgetContents.setObjectName("scrollAreaWidgetContents")
+        self.gridLayout = QGridLayout(self.scrollAreaWidgetContents)
+
+        # Dynamically generate Microscope display
+        if self.model.nPySpinCameras:
+            self.display_microscope()  # Attach screen widget
+        else:  # Display only mock camera
+            self.display_mock_camera()
+
+        # Stage_widget
+        self.stage_widget = StageWidget(self.model, ui_dir, self.screen_widgets)
+        splitter = QSplitter()
+        splitter.addWidget(self.scrollAreaWidgetContents)
+        splitter.addWidget(self.stage_widget)
+        self.verticalLayout_4.addWidget(splitter)
+
+        # Start button. If toggled, start camera acquisition
+        self.startButton.clicked.connect(self.start_button_handler)
+
+        # Recording functions
+        self.recordingManager = RecordingManager(self.model)
+        self.snapshotButton.clicked.connect(
+            lambda: self.recordingManager.save_last_image(
+                self.dirLabel.text(), self.screen_widgets
+            )
+        )
+        self.recordButton.clicked.connect(
+            self.record_button_handler
+        )  # Recording video button
+
+        # Refreshing the screen timer
+        self.refresh_timer = QTimer()
+        self.refresh_timer.timeout.connect(self.refresh)
+
+        # Toggle start button on init
+        self.start_button_handler()
+
+    def refresh_cameras(self):
+        """
+        This method is responsible for scanning for available cameras and updating the camera list.
+        It adds mock cameras for testing purposes and scans for actual cameras if the application
+        is not in dummy mode. This ensures that the list of available cameras is always up-to-date.
+        """
+        # Add mock cameras for testing purposes
+        self.model.add_mock_cameras()
+        # If not in dummy mode, scan for actual available cameras
+        if not self.dummy:
+            try:
+                self.model.scan_for_cameras()
+            except Exception as e:
+                print(
+                    f" Something still holds a reference to the camera.\n {e}"
+                )
+
+    def refresh_stages(self):
+        """Search for connected stages"""
+        if not self.dummy:
+            self.model.scan_for_usb_stages()
+
+    def record_button_handler(self):
+        """
+        Handles the record button press event.
+        If the record button is checked, start recording. Otherwise, stop recording.
+        """
+        if self.recordButton.isChecked():
+            save_path = self.dirLabel.text()
+            self.recordingManager.save_recording(save_path, self.screen_widgets)
+        else:
+            self.recordingManager.stop_recording(self.screen_widgets)
+
+    def start_button_handler(self):
+        """
+        Handles the start button press event.
+
+        If the start button is checked, initiate acquisition from all cameras and start refreshing images.
+        If unchecked, stop acquisition from all cameras and stop refreshing images.
+        """
+        # Initialize the list to keep track of cameras that have been started or stopped
+        refresh_camera_list = []
+
+        # Check if the start button is toggled on
+        if self.startButton.isChecked():
+            print("\nRefreshing Screen")
+            # Camera begin acquisition
+            for screen in self.screen_widgets:
+                camera_name = screen.get_camera_name()
+                if camera_name not in refresh_camera_list:
+                    screen.start_acquisition_camera()
+                    refresh_camera_list.append(camera_name)
+
+            # Refreshing images to display screen
+            self.refresh_timer.start(125)
+
+            # Start button is checked, enable record and snapshot button.
+            self.recordButton.setEnabled(True)
+            self.snapshotButton.setEnabled(True)
+
+        else:
+            print("Stop Refreshing Screen")
+            # Start button is unchecked, disable record and snapshot button.
+            self.recordButton.setEnabled(False)
+            self.recordButton.setChecked(False)
+            self.snapshotButton.setEnabled(False)
+
+            # Stop Refresh: stop refreshing images to display screen
+            if self.refresh_timer.isActive():
+                self.refresh_timer.stop()
+
+            # End acquisition from camera: stop acquiring images from camera to framebuffer
+            for screen in self.screen_widgets:
+                camera_name = screen.get_camera_name()
+                if camera_name not in refresh_camera_list:
+                    screen.stop_acquisition_camera()
+                    refresh_camera_list.append(camera_name)
+
+    def refresh(self):
+        """Refreshing from framebuffer to screen"""
+        for screen in self.screen_widgets:
+            screen.refresh()  # Refresh the screens
+
+    def display_mock_camera(self):
+        """Display mock camera when there is no detected camera."""
+        self.createNewGroupBox(0, 0, mock=True)
+
+    def display_microscope(self):
+        """Dynamically arrange Microscopes based on camera count and column configuration."""
+        # Calculate rows and columns
+        rows, cols, cnt = (
+            self.model.nPySpinCameras // self.nColumn,
+            self.nColumn,
+            0,
+        )
+        rows += 1 if self.model.nPySpinCameras % cols else 0
+        # Create grid of Microscope displays
+        for row_idx in range(0, rows):
+            for col_idx in range(0, cols):
+                if cnt < self.model.nPySpinCameras:
+                    self.createNewGroupBox(row_idx, col_idx, screen_index=cnt)
+                    cnt += 1
+                else:
+                    break  # Stop when all Microscopes are displayed
+
+    def column_changed_handler(self, val):
+        """Rearrange the layout of Microscopes when the column number changes."""
+        # Identify current Microscope widgets
+        camera_screen_list = []
+        # Detach the identified widgets
+        for i in range(self.gridLayout.count()):
+            widget = self.gridLayout.itemAt(i).widget()
+            if isinstance(
+                widget, QGroupBox
+            ):  # Ensure we're handling the correct type of widget
+                camera_screen_list.append(widget)
+
+        # Detach the identified widgets
+        for widget in camera_screen_list:
+            self.gridLayout.removeWidget(widget)
+            widget.hide()  # Temporarily hide the widget
+
+        # Calculate new rows and columns layout
+        rows, cols, cnt = self.model.nPySpinCameras // val, val, 0
+        rows += 1 if self.model.nPySpinCameras % cols else 0
+
+        # Reattach widgets in the new layout
+        for row_idx in range(0, rows):
+            for col_idx in range(0, cols):
+                if cnt < len(camera_screen_list):
+                    widget = camera_screen_list[cnt]
+                    self.gridLayout.addWidget(widget, row_idx, col_idx, 1, 1)
+                    widget.show()  # Make the widget visible again
+                    cnt += 1
+                else:
+                    break
+
+    def createNewGroupBox(self, rows, cols, mock=False, screen_index=None):
+        """
+        Create a new group box widget representing a microscope, and add it to the grid layout.
+        This function is responsible for generating a unique name for the microscope, creating a group box to
+        represent it, adding a screen widget for camera display, a settings button, and configuring their
+        properties and layouts. It also adds the group box to the grid layout at the specified row and column
+        indices, and updates the settings menu for the microscope.
+
+        Parameters:
+        - rows (int): The row index in the grid layout where the group box should be added.
+        - cols (int): The column index in the grid layout where the group box should be added.
+        - mock (bool, optional): If True, a mock camera will be associated with this microscope. Default is False.
+        - screen_index (int, optional): The index of the camera in the model's camera list to be associated
+        with this microscope. Required if mock is False.
+        """
+        # Generate unique names based on row and column indices
+        newNameMicroscope = ""
+        # Generate unique names based on camera number
+        if mock:
+            newNameMicroscope = "Mock Camera"
+        else:
+            newNameMicroscope = f"Microscope_{screen_index+1}"
+        microscopeGrp = QGroupBox(self.scrollAreaWidgetContents)
+
+        # Construct and configure the Microscope widget
+        microscopeGrp.setObjectName(newNameMicroscope)
+        microscopeGrp.setStyleSheet("background-color: rgb(58, 58, 58);")
+        font_grpbox = QFont()
+        font_grpbox.setPointSize(9)  # Setting font size to 9
+        microscopeGrp.setFont(font_grpbox)
+        verticalLayout = QVBoxLayout(microscopeGrp)
+        verticalLayout.setObjectName("verticalLayout")
+
+        # Add screens
+        if mock:
+            screen = ScreenWidget(
+                self.model.cameras[0], model=self.model, parent=microscopeGrp
+            )
+        else:
+            screen = ScreenWidget(
+                self.model.cameras[screen_index],
+                model=self.model,
+                parent=microscopeGrp,
+            )
+        screen.setObjectName(f"Screen")
+        verticalLayout.addWidget(screen)
+
+        if mock is False:
+            # Add setting button
+            settingButton = QToolButton(microscopeGrp)
+            settingButton.setObjectName(f"Setting")
+            settingButton.setFont(font_grpbox)
+            settingButton.setCheckable(True)
+            self.create_settings_menu(
+                microscopeGrp, newNameMicroscope, screen, screen_index
+            )
+            settingButton.toggled.connect(
+                lambda checked: self.show_settings_menu(settingButton, checked)
+            )
+            verticalLayout.addWidget(settingButton)
+            settingButton.setText(
+                QCoreApplication.translate(
+                    "MainWindow", "SETTINGS \u25ba", None
+                )
+            )
+
+            # Load setting file from JSON
+            self.update_setting_menu(microscopeGrp)
+
+        # Add widget to the gridlayout
+        self.gridLayout.addWidget(microscopeGrp, rows, cols, 1, 1)
+
+        # Add the new microscopeGrpBox instance to the list
+        self.screen_widgets.append(screen)
+
+    def create_settings_menu(
+        self, microscopeGrp, newNameMicroscope, screen, screen_index
+    ):
+        """
+        Create the settings menu for each Microscope widget.
+
+        This function initializes the settings menu UI, loads it with necessary data,
+        and associates the relevant signals with their slots.
+        The settings menu is hidden by default and will be shown
+        when the user toggles the settings button.
+
+        Parameters:
+        - microscopeGrp (QGroupBox): The group box representing a Microscope widget.
+        - newNameMicroscope (str): The unique name assigned to the Microscope widget.
+        - screen (ScreenWidget): The screen widget associated with the Microscope.
+        - screen_index (int): The index of the camera in the model's camera list to be associated with this screen.
+        """
+        # Initialize the settings menu UI from the .ui file
+        settingMenu = QWidget(microscopeGrp)
+        setting_ui = os.path.join(ui_dir, "settingPopUpMenu.ui")
+        loadUi(setting_ui, settingMenu)
+        settingMenu.setObjectName("SettingsMenu")
+        settingMenu.hide()  # Hide the menu by default
+
+        # S/N
+        # Add the list of cameras (serial number) in ComboBox
+        for sn in self.model.cameras_sn:        
+            settingMenu.snComboBox.addItem(sn) 
+        # Select the sn for the current screen
+        sn = screen.get_camera_name()           
+        index = settingMenu.snComboBox.findText(sn)
+        if index >= 0:
+            settingMenu.snComboBox.setCurrentIndex(index)
+        else:
+            logger.error("SN not found in the list")
+
+        # If serial number is changed, connect to update_screen function and update setting menu
+        settingMenu.snComboBox.currentIndexChanged.connect(
+            lambda: self.update_screen(
+                screen, screen_index, settingMenu.snComboBox.currentText()
+            )
+        )
+
+        # Custom name
+        customName = self.user_setting.load_settings_item(
+            sn, "customName"
+        )  # Default name on init
+        customName = customName if customName else newNameMicroscope
+        settingMenu.customName.setText(customName)
+        self.update_groupbox_name(
+            microscopeGrp, customName
+        )  # Update GroupBox name
+        # Name) If custom name is changed, change the groupBox name.
+        settingMenu.customName.textChanged.connect(
+            lambda: self.update_groupbox_name(
+                microscopeGrp, settingMenu.customName.text()
+            )
+        )
+        settingMenu.customName.textChanged.connect(
+            lambda: self.user_setting.update_user_configs_settingMenu(
+                microscopeGrp, "customName", settingMenu.customName.text()
+            )
+        )
+
+        # Exposure
+        settingMenu.expSlider.valueChanged.connect(
+            lambda: screen.set_camera_setting(
+                setting="exposure", val=settingMenu.expSlider.value() * 1000
+            )
+        )
+        settingMenu.expSlider.valueChanged.connect(
+            lambda: settingMenu.expNum.setNum(settingMenu.expSlider.value())
+        )
+        settingMenu.expSlider.valueChanged.connect(
+            lambda: self.user_setting.update_user_configs_settingMenu(
+                microscopeGrp, "exp", settingMenu.expSlider.value()
+            )
+        )
+        settingMenu.expAuto.clicked.connect(
+            lambda: settingMenu.expSlider.setValue(
+                int(screen.get_camera_setting(setting="exposure") / 1000)
+            )
+        )
+
+        # Gain
+        settingMenu.gainSlider.valueChanged.connect(
+            lambda: screen.set_camera_setting(
+                setting="gain", val=settingMenu.gainSlider.value()
+            )
+        )
+        settingMenu.gainSlider.valueChanged.connect(
+            lambda: settingMenu.gainNum.setNum(settingMenu.gainSlider.value())
+        )
+        settingMenu.gainSlider.valueChanged.connect(
+            lambda: self.user_setting.update_user_configs_settingMenu(
+                microscopeGrp, "gain", settingMenu.gainSlider.value()
+            )
+        )
+        settingMenu.gainAuto.clicked.connect(
+            lambda: settingMenu.gainSlider.setValue(
+                screen.get_camera_setting(setting="gain")
+            )
+        )
+
+        # Gamma
+        settingMenu.gammaSlider.valueChanged.connect(
+            lambda: screen.set_camera_setting(
+                setting="gamma", val=settingMenu.gammaSlider.value() / 100
+            )
+        )
+        settingMenu.gammaSlider.valueChanged.connect(
+            lambda: settingMenu.gammaNum.setText(
+                "{:.2f}".format(settingMenu.gammaSlider.value() / 100)
+            )
+        )
+        settingMenu.gammaSlider.valueChanged.connect(
+            lambda: self.user_setting.update_user_configs_settingMenu(
+                microscopeGrp, "gamma", settingMenu.gammaSlider.value()
+            )
+        )
+        settingMenu.gammaAuto.clicked.connect(
+            lambda: settingMenu.gammaSlider.setEnabled(
+                not settingMenu.gammaSlider.isEnabled()
+            )
+        )
+        settingMenu.gammaAuto.clicked.connect(
+            lambda: self.user_setting.update_user_configs_settingMenu(
+                microscopeGrp, "gammaAuto", settingMenu.gammaSlider.isEnabled()
+            )
+        )
+
+        # W/B
+        settingLayout = settingMenu.layout()
+        settingLayout.addWidget(settingMenu.wbAuto, 5, 1, 2, 1)
+        # Blue Channel
+        settingMenu.wbSliderBlue.valueChanged.connect(
+            lambda: screen.set_camera_setting(
+                setting="wbBlue", val=settingMenu.wbSliderBlue.value() / 100
+            )
+        )
+        settingMenu.wbSliderBlue.valueChanged.connect(
+            lambda: settingMenu.wbNumBlue.setText(
+                "{:.2f}".format(settingMenu.wbSliderBlue.value() / 100)
+            )
+        )
+        settingMenu.wbSliderBlue.valueChanged.connect(
+            lambda: self.user_setting.update_user_configs_settingMenu(
+                microscopeGrp, "wbBlue", settingMenu.wbSliderBlue.value()
+            )
+        )
+        settingMenu.wbAuto.clicked.connect(
+            lambda: settingMenu.wbSliderBlue.setValue(
+                screen.get_camera_setting(setting="wbBlue") * 100
+            )
+        )
+
+        # Red Channel
+        settingMenu.wbSliderRed.valueChanged.connect(
+            lambda: screen.set_camera_setting(
+                setting="wbRed", val=settingMenu.wbSliderRed.value() / 100
+            )
+        )
+        settingMenu.wbSliderRed.valueChanged.connect(
+            lambda: settingMenu.wbNumRed.setText(
+                "{:.2f}".format(settingMenu.wbSliderRed.value() / 100)
+            )
+        )
+        settingMenu.wbSliderRed.valueChanged.connect(
+            lambda: self.user_setting.update_user_configs_settingMenu(
+                microscopeGrp, "wbRed", settingMenu.wbSliderRed.value()
+            )
+        )
+        settingMenu.wbAuto.clicked.connect(
+            lambda: settingMenu.wbSliderRed.setValue(
+                screen.get_camera_setting(setting="wbRed") * 100
+            )
+        )
+
+    def update_screen(self, screen, screen_index, selected_sn):
+        """
+        Update the screen with a new camera based on the selected serial number.
+
+        This method manages the update of the camera associated with a specific microscope screen. It takes into
+        account the current state of the application, i.e., whether acquisition is ongoing or not, and performs
+        the necessary actions to update the camera and manage acquisition accordingly.
+
+        Parameters:
+        - screen (ScreenWidget): The screen widget associated with the microscope.
+        - screen_index (int): The index of the screen in the list of all microscope screens.
+        - selected_sn (str): The serial number of the camera selected to be associated with the microscope.
+        """
+        # Camera lists that currently attached on the model.
+        camera_list = {
+            camera.name(sn_only=True): camera for camera in self.model.cameras
+        }
+
+        # Get the prev camera lists displaying on the screen
+        prev_camera, curr_camera = screen.get_camera_name(), selected_sn
+        prev_lists = [
+            screen.get_camera_name()
+            for screen in self.screen_widgets
+            if screen.get_camera_name()
+        ]
+        if (
+            0 <= screen_index < len(prev_lists)
+        ):  # Ensure screen_index is within valid range
+            curr_list = prev_lists[:]
+            curr_list.pop(screen_index)
+            curr_list.insert(screen_index, curr_camera)
+        else:
+            logger.error(f"Invalid screen index: {screen_index}")
+        logger.debug(f"prev_list: {prev_lists}")
+        logger.debug(f"curr_list: {curr_list}")
+
+        # Handle updates based on the current state of the application
+        if (
+            self.startButton.isChecked()
+        ):  # If the 'Start' button is enabled (continuous acquisition mode)
+            if set(prev_lists) == set(curr_list):
+                # If the list of cameras hasn't changed, just update the current screen's camera
+                screen.set_camera(camera_list.get(curr_camera))
+            else:
+                if prev_camera not in curr_list:
+                    # If the previous camera has been removed from the list, stop its acquisition
+                    screen.stop_acquisition_camera()
+                    screen.set_camera(camera_list.get(curr_camera))
+                if curr_camera not in prev_lists:
+                    # If the selected camera is new (wasn't in the previous list), start its acquisition
+                    screen.set_camera(camera_list.get(curr_camera))
+                    screen.start_acquisition_camera()
+        else:
+            # If the 'Start' button is disabled, start single frame acquisition to show the image
+            screen.set_camera(camera_list.get(curr_camera))
+            screen.single_acquisition_camera()
+            screen.refresh_single_frame()
+            screen.stop_single_acquisition_camera()
+
+    def update_groupbox_name(self, microscopeGrp, customName):
+        """
+        Update the title and object name of the group box representing a microscope.
+
+        This method is used to update the visual representation of a microscope based on a custom name provided
+        by the user.
+
+        Parameters:
+        - microscopeGrp (QGroupBox): The group box representing the microscope.
+        - customName (str): The custom name to set as the title and object name of the group box.
+        """
+        if customName:
+            microscopeGrp.setTitle(customName)
+            microscopeGrp.setObjectName(customName)
+
+    def show_settings_menu(self, settingButton, is_checked):
+        """
+        Show or hide the settings menu associated with a microscope group box.
+
+        This method is connected to the toggled signal of a QToolButton, which represents
+        the settings button for a microscope group box. When the button is toggled, it
+        shows or hides the settings menu and starts or stops a timer to refresh the settings
+        values displayed in the menu.
+
+        Parameters:
+        - settingButton (QToolButton): The settings button associated with the microscope group box.
+        - is_checked (bool): Indicates whether the settings button is checked (True) or unchecked (False).
+        """
+        microscopeGrp = settingButton.parent()
+        # Find the settingMenu within this microscopeGrp
+        settingMenu = microscopeGrp.findChild(QWidget, "SettingsMenu")
+        self.settings_refresh_timer.timeout.connect(
+            partial(self.update_setting_menu, microscopeGrp)
+        )
+
+        if is_checked:
+            # If the settings button is checked, start the settings refresh 
+            # timer and show the settings menu
+            # update setting menu every 0.1 sec
+            self.settings_refresh_timer.start(100)      
+            
+
+            # Show the setting menu next to setting button
+            button_position = settingButton.mapToGlobal(settingButton.pos())
+            menu_x = button_position.x() + settingButton.width()
+            menu_x = menu_x - microscopeGrp.mapToGlobal(QPoint(0, 0)).x()
+            menu_y = (
+                settingButton.y()
+                + settingButton.height()
+                - settingMenu.height()
+            )
+            logger.debug(
+                f"(SettingMenu) coordinates of setting menu: x: {menu_x}, y: {menu_y}"
+            )
+            settingMenu.move(menu_x, menu_y)
+            settingMenu.show()
+        else:
+            # If the settings button is unchecked, stop the settings 
+            # refresh timer and hide the settings menu
+            self.settings_refresh_timer.stop()
+            settingMenu.hide()
+
+    def update_setting_menu(self, microscopeGrp):
+        """
+        Update the values displayed in the settings menu based on the current camera settings.
+
+        This method is called periodically by a QTimer to refresh the values displayed in the
+        settings menu, ensuring they are up-to-date with the current settings of the camera.
+
+        Parameters:
+        - microscopeGrp (QGroupBox): The microscope group box associated with the settings menu to be updated.
+        """
+
+        # Find the settingMenu within this microscopeGrp
+        settingMenu = microscopeGrp.findChild(QWidget, "SettingsMenu")
+        screen = microscopeGrp.findChild(ScreenWidget, "Screen")
+
+        # Display the S/N of camera
+        sn = screen.get_camera_name()
+        # Load the saved settings
+        saved_settings = self.user_setting.load_settings_item(sn)
+        if saved_settings:
+            # If saved settings are found, update the sliders in the settings menu with the saved values
+            settingMenu.expSlider.setValue(saved_settings.get("exp", 15))
+            settingMenu.gainSlider.setValue(saved_settings.get("gain", 20))
+
+            # Gamma
+            gammaAuto = saved_settings.get("gammaAuto", None)
+            if gammaAuto == True:
+                settingMenu.gammaSlider.setEnabled(True)
+                settingMenu.gammaSlider.setValue(
+                    saved_settings.get("gamma", 100)
+                )
+            elif gammaAuto == False:
+                settingMenu.gammaSlider.setEnabled(False)
+            else:
+                pass
+
+            # W/B
+            if screen.get_camera_color_type() == "Color":
+                settingMenu.wbAuto.setDisabled(False)
+                settingMenu.wbSliderRed.setDisabled(False)
+                settingMenu.wbSliderBlue.setDisabled(False)
+                settingMenu.wbSliderRed.setValue(
+                    saved_settings.get("wbRed", 1.2)
+                )
+                settingMenu.wbSliderBlue.setValue(
+                    saved_settings.get("wbBlue", 2.8)
+                )
+            elif screen.get_camera_color_type() == "Mono":
+                settingMenu.wbAuto.setDisabled(True)
+                settingMenu.wbSliderRed.setDisabled(True)
+                settingMenu.wbSliderBlue.setDisabled(True)
+                settingMenu.wbNumRed.setText("--")
+                settingMenu.wbNumBlue.setText("--")
+
+        else:
+            settingMenu.gainAuto.click()
+            settingMenu.wbAuto.click()
+            settingMenu.expAuto.click()
+            self.user_setting.update_user_configs_settingMenu(
+                microscopeGrp, "gammaAuto", True
+            )
+            self.user_setting.update_user_configs_settingMenu(
+                microscopeGrp, "gamma", settingMenu.gammaSlider.value()
+            )
+
+    def dir_setting_handler(self):
+        """
+        This method handles the selection of a directory for saving files. It opens a dialog that allows
+        the user to browse their filesystem and select a directory. The selected directory's path is then
+        displayed on the user interface.
+
+        This is a crucial function for users who need to save data or configurations, as it provides a
+        simple and intuitive way to specify the location where files should be saved.
+        """
+        # Fetch the default documents directory path
+        documents_dir = QStandardPaths.writableLocation(
+            QStandardPaths.DocumentsLocation
+        )
+        # Open a dialog to allow the user to select a directory
+        directory = QFileDialog.getExistingDirectory(
+            self, "Select Directory", documents_dir
+        )
+        # If a directory is chosen, update the label to display the chosen path
+        if directory:
+            self.dirLabel.setText(directory)
+
+    def save_user_configs(self):
+        """
+        Saves user configuration settings to a persistent storage.
+
+        This method retrieves current configuration values from the UI, including
+        the number of columns (nColumn), directory path (directory), and the window's
+        width and height. It then passes these values to the `save_user_configs` method
+        of the `user_setting` object to be saved.
+        """
+        nColumn = self.nColumnsSpinBox.value()
+        directory = self.dirLabel.text()
+        width = self.width()
+        height = self.height()
+        self.user_setting.save_user_configs(nColumn, directory, width, height)
```

### Comparing `parallax_app-0.37.1/parallax/model.py` & `parallax_app-0.37.5/parallax/model.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,168 +1,168 @@
-"""
-The Model class is the core component for managing cameras, stages, and calibration data.
-"""
-
-from PyQt5.QtCore import QObject, pyqtSignal
-
-from .camera import MockCamera, PySpinCamera, close_cameras, list_cameras
-from .stage_listener import Stage, StageInfo
-
-
-class Model(QObject):
-    """Model class to handle cameras, stages, and calibration data."""
-
-    msg_posted = pyqtSignal(str)
-    accutest_point_reached = pyqtSignal()
-
-    def __init__(self, version="V1"):
-        """Initialize model object"""
-        QObject.__init__(self)
-        self.version = version
-        # camera
-        self.cameras = []
-        self.cameras_sn = []
-        self.nPySpinCameras = 0
-        self.nMockCameras = 0
-        self.focos = []
-
-        # stage
-        self.nStages = 0
-        self.init_stages()
-        self.elevators = {}
-        self.stage_listener_url = "http://localhost:8080/"
-
-        # probe detector
-        self.probeDetectors = []
-
-        # coords axis
-        self.coords_axis = {}
-        self.camera_intrinsic = {}
-        self.camera_extrinsic = {}
-        self.calibration = None
-        self.calibrations = {}
-
-        self.cal_in_progress = False
-        self.accutest_in_progress = False
-        self.lcorr, self.rcorr = False, False
-
-        self.img_point_last = None
-        self.obj_point_last = None
-        self.transforms = {}
-
-    def set_last_object_point(self, obj_point):
-        """Set the last object point."""
-        self.obj_point_last = obj_point
-
-    def add_calibration(self, cal):
-        """Add a calibration."""
-        self.calibrations[cal.name] = cal
-
-    def set_calibration(self, calibration):
-        """Set the calibration."""
-        self.calibration = calibration
-
-    def set_lcorr(self, xc, yc):
-        """Set left coordinates."""
-        self.lcorr = [xc, yc]
-
-    def clear_lcorr(self):
-        """Clear left coordinates."""
-        self.lcorr = False
-
-    def set_rcorr(self, xc, yc):
-        """Set right coordinates."""
-        self.rcorr = [xc, yc]
-
-    def clear_rcorr(self):
-        """Clear right coordinates."""
-        self.rcorr = False
-
-    def init_stages(self):
-        """Initialize stages."""
-        self.stages = {}
-
-    def add_video_source(self, video_source):
-        """Add a video source."""
-        self.cameras.append(video_source)
-
-    def add_mock_cameras(self, n=1):
-        """Add mock cameras."""
-        for i in range(n):
-            self.cameras.append(MockCamera())
-
-    def scan_for_cameras(self):
-        """Scan for cameras."""
-        self.cameras = list_cameras(version=self.version) + self.cameras
-        self.cameras_sn = [camera.name(sn_only=True) for camera in self.cameras]
-        self.nMockCameras = len(
-            [
-                camera
-                for camera in self.cameras
-                if isinstance(camera, MockCamera)
-            ]
-        )
-        self.nPySpinCameras = len(
-            [
-                camera
-                for camera in self.cameras
-                if isinstance(camera, PySpinCamera)
-            ]
-        )
-
-    def scan_for_usb_stages(self):
-        """Scan for USB stages."""
-        stage_info = StageInfo(self.stage_listener_url)
-        instances = stage_info.get_instances()
-        self.init_stages()
-        for instance in instances:
-            stage = Stage(stage_info=instance)
-            self.add_stage(stage)
-        self.nStages = len(self.stages)
-
-    def add_stage(self, stage):
-        """Add a stage."""
-        self.stages[stage.sn] = stage
-
-    def get_stage(self, stage_sn):
-        """Get a stage."""
-        return self.stages.get(stage_sn)
-
-    def add_probe_detector(self, probeDetector):
-        """Add a probe detector."""
-        self.probeDetectors.append(probeDetector)
-
-    def add_coords_axis(self, camera_name, coords):
-        """Add coordinates axis."""
-        self.coords_axis[camera_name] = coords
-
-    def get_coords_axis(self, camera_name):
-        """Get coordinates axis."""
-        return self.coords_axis.get(camera_name)
-
-    def add_camera_intrinsic(self, camera_name, mtx, dist):
-        """Add camera intrinsic parameters."""
-        self.camera_intrinsic[camera_name] = [mtx, dist]
-
-    def get_camera_intrinsic(self, camera_name):
-        """Get camera intrinsic parameters."""
-        return self.camera_intrinsic.get(camera_name)
-
-    def add_camera_extrinsic(self, name1, name2, retVal, R, T, E, F):
-        """Add camera extrinsic parameters."""
-        self.camera_extrinsic[name1 + "-" + name2] = [retVal, R, T, E, F]
-
-    def get_camera_extrinsic(self, name1, name2):
-        """Get camera extrinsic parameters."""
-        return self.camera_extrinsic.get(name1 + "-" + name2)
-
-    def clean(self):
-        """Clean up."""
-        close_cameras()
-
-    def save_all_camera_frames(self):
-        """Save all camera frames."""
-        for i, camera in enumerate(self.cameras):
-            if camera.last_image:
-                filename = 'camera%d_%s.png' % (i, camera.get_last_capture_time())
-                camera.save_last_image(filename)
-                self.msg_log.post("Saved camera frame: %s" % filename)
+"""
+The Model class is the core component for managing cameras, stages, and calibration data.
+"""
+
+from PyQt5.QtCore import QObject, pyqtSignal
+
+from .camera import MockCamera, PySpinCamera, close_cameras, list_cameras
+from .stage_listener import Stage, StageInfo
+
+
+class Model(QObject):
+    """Model class to handle cameras, stages, and calibration data."""
+
+    msg_posted = pyqtSignal(str)
+    accutest_point_reached = pyqtSignal()
+
+    def __init__(self, version="V1"):
+        """Initialize model object"""
+        QObject.__init__(self)
+        self.version = version
+        # camera
+        self.cameras = []
+        self.cameras_sn = []
+        self.nPySpinCameras = 0
+        self.nMockCameras = 0
+        self.focos = []
+
+        # stage
+        self.nStages = 0
+        self.init_stages()
+        self.elevators = {}
+        self.stage_listener_url = "http://localhost:8080/"
+
+        # probe detector
+        self.probeDetectors = []
+
+        # coords axis
+        self.coords_axis = {}
+        self.camera_intrinsic = {}
+        self.camera_extrinsic = {}
+        self.calibration = None
+        self.calibrations = {}
+
+        self.cal_in_progress = False
+        self.accutest_in_progress = False
+        self.lcorr, self.rcorr = False, False
+
+        self.img_point_last = None
+        self.obj_point_last = None
+        self.transforms = {}
+
+    def set_last_object_point(self, obj_point):
+        """Set the last object point."""
+        self.obj_point_last = obj_point
+
+    def add_calibration(self, cal):
+        """Add a calibration."""
+        self.calibrations[cal.name] = cal
+
+    def set_calibration(self, calibration):
+        """Set the calibration."""
+        self.calibration = calibration
+
+    def set_lcorr(self, xc, yc):
+        """Set left coordinates."""
+        self.lcorr = [xc, yc]
+
+    def clear_lcorr(self):
+        """Clear left coordinates."""
+        self.lcorr = False
+
+    def set_rcorr(self, xc, yc):
+        """Set right coordinates."""
+        self.rcorr = [xc, yc]
+
+    def clear_rcorr(self):
+        """Clear right coordinates."""
+        self.rcorr = False
+
+    def init_stages(self):
+        """Initialize stages."""
+        self.stages = {}
+
+    def add_video_source(self, video_source):
+        """Add a video source."""
+        self.cameras.append(video_source)
+
+    def add_mock_cameras(self, n=1):
+        """Add mock cameras."""
+        for i in range(n):
+            self.cameras.append(MockCamera())
+
+    def scan_for_cameras(self):
+        """Scan for cameras."""
+        self.cameras = list_cameras(version=self.version) + self.cameras
+        self.cameras_sn = [camera.name(sn_only=True) for camera in self.cameras]
+        self.nMockCameras = len(
+            [
+                camera
+                for camera in self.cameras
+                if isinstance(camera, MockCamera)
+            ]
+        )
+        self.nPySpinCameras = len(
+            [
+                camera
+                for camera in self.cameras
+                if isinstance(camera, PySpinCamera)
+            ]
+        )
+
+    def scan_for_usb_stages(self):
+        """Scan for USB stages."""
+        stage_info = StageInfo(self.stage_listener_url)
+        instances = stage_info.get_instances()
+        self.init_stages()
+        for instance in instances:
+            stage = Stage(stage_info=instance)
+            self.add_stage(stage)
+        self.nStages = len(self.stages)
+
+    def add_stage(self, stage):
+        """Add a stage."""
+        self.stages[stage.sn] = stage
+
+    def get_stage(self, stage_sn):
+        """Get a stage."""
+        return self.stages.get(stage_sn)
+
+    def add_probe_detector(self, probeDetector):
+        """Add a probe detector."""
+        self.probeDetectors.append(probeDetector)
+
+    def add_coords_axis(self, camera_name, coords):
+        """Add coordinates axis."""
+        self.coords_axis[camera_name] = coords
+
+    def get_coords_axis(self, camera_name):
+        """Get coordinates axis."""
+        return self.coords_axis.get(camera_name)
+
+    def add_camera_intrinsic(self, camera_name, mtx, dist):
+        """Add camera intrinsic parameters."""
+        self.camera_intrinsic[camera_name] = [mtx, dist]
+
+    def get_camera_intrinsic(self, camera_name):
+        """Get camera intrinsic parameters."""
+        return self.camera_intrinsic.get(camera_name)
+
+    def add_camera_extrinsic(self, name1, name2, retVal, R, T, E, F):
+        """Add camera extrinsic parameters."""
+        self.camera_extrinsic[name1 + "-" + name2] = [retVal, R, T, E, F]
+
+    def get_camera_extrinsic(self, name1, name2):
+        """Get camera extrinsic parameters."""
+        return self.camera_extrinsic.get(name1 + "-" + name2)
+
+    def clean(self):
+        """Clean up."""
+        close_cameras()
+
+    def save_all_camera_frames(self):
+        """Save all camera frames."""
+        for i, camera in enumerate(self.cameras):
+            if camera.last_image:
+                filename = 'camera%d_%s.png' % (i, camera.get_last_capture_time())
+                camera.save_last_image(filename)
+                self.msg_log.post("Saved camera frame: %s" % filename)
```

### Comparing `parallax_app-0.37.1/parallax/probe_calibration.py` & `parallax_app-0.37.5/parallax/probe_calibration.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,352 +1,352 @@
-"""
-ProbeCalibration transforms probe coordinates from local to global space"
-- local space: Stage coordinates
-- global space: Reticle coordinates
-"""
-
-import csv
-import logging
-import os
-
-import numpy as np
-import pandas as pd
-from PyQt5.QtCore import QObject, pyqtSignal
-from sklearn.linear_model import LinearRegression
-
-# Set logger name
-logger = logging.getLogger(__name__)
-logger.setLevel(logging.DEBUG)
-# Set the logging level for PyQt5.uic.uiparser/properties to WARNING, to ignore DEBUG messages
-logging.getLogger("PyQt5.uic.uiparser").setLevel(logging.WARNING)
-logging.getLogger("PyQt5.uic.properties").setLevel(logging.WARNING)
-
-
-class ProbeCalibration(QObject):
-    """
-    Handles the transformation of probe coordinates from local (stage) to global (reticle) space.
-
-    Attributes:
-        calib_complete_x (pyqtSignal): Signal emitted when calibration in the X direction is complete.
-        calib_complete_y (pyqtSignal): Signal emitted when calibration in the Y direction is complete.
-        calib_complete_z (pyqtSignal): Signal emitted when calibration in the Z direction is complete.
-        calib_complete (pyqtSignal): General signal emitted when calibration is fully complete.
-
-    Args:
-        stage_listener (QObject): The stage listener object that emits signals related to stage movements.
-    """
-
-    calib_complete_x = pyqtSignal()
-    calib_complete_y = pyqtSignal()
-    calib_complete_z = pyqtSignal()
-    calib_complete = pyqtSignal(str, object)
-    transM_info = pyqtSignal(object, float, object)
-
-    """Class for probe calibration."""
-
-    def __init__(self, stage_listener):
-        """
-        Initializes the ProbeCalibration object with a given stage listener.
-        """
-        super().__init__()
-        self.stage_listener = stage_listener
-        self.stage_listener.probeCalibRequest.connect(self.update)
-        self.stages = {}
-        self.df = None
-        self.inliers = []
-        self.stage = None
-        self.threshold_min_max = 2000  # TODO
-        self.model_LR, self.transM_LR, self.transM_LR_prev = None, None, None
-        self.threshold_matrix = np.array(
-            [
-                [0.00002, 0.00002, 0.00002, 50.0],  # TODO
-                [0.00002, 0.00002, 0.00002, 50.0],
-                [0.00002, 0.00002, 0.00002, 50.0],
-                [0.0, 0.0, 0.0, 0.0],
-            ]
-        )
-        self.LR_err_L2_threshold = 20  # TODO
-        self._create_file()
-
-        # Test signal
-        self.reset_calib()
-
-    def reset_calib(self):
-        """
-        Resets calibration to its initial state, clearing any stored min and max values.
-        """
-        self.min_x, self.max_x = float("inf"), float("-inf")
-        self.min_y, self.max_y = float("inf"), float("-inf")
-        self.min_z, self.max_z = float("inf"), float("-inf")
-        self.transM_LR_prev = np.zeros((4, 4), dtype=np.float64)
-        self.signal_emitted_x = False
-        self.signal_emitted_y = False
-        self.signal_emitted_z = False
-
-    def _create_file(self):
-        """
-        Creates or clears the CSV file used to store local and global points during calibration.
-        """
-        package_dir = os.path.dirname(os.path.abspath(__file__))
-        debug_dir = os.path.join(os.path.dirname(package_dir), "debug")
-        os.makedirs(debug_dir, exist_ok=True)
-        self.csv_file = os.path.join(debug_dir, "points.csv")
-
-        # Check if the file exists and remove it if it does
-        if os.path.exists(self.csv_file):
-            os.remove(self.csv_file)
-
-        # Create a new file and write column names
-        with open(self.csv_file, "w", newline="") as file:
-            writer = csv.writer(file)
-            # Define column names
-            column_names = [
-                "local_x",
-                "local_y",
-                "local_z",
-                "global_x",
-                "global_y",
-                "global_z",
-            ]
-            writer.writerow(column_names)
-
-    def clear(self):
-        """
-        Clears all stored data and resets the transformation matrix to its default state.
-        """
-        self._create_file()
-        self.model_LR, self.transM_LR, self.transM_LR_prev = None, None, None
-
-    def _get_local_global_points(self):
-        """
-        Retrieves local and global points from the CSV file as numpy arrays.
-
-        Returns:
-            tuple: A tuple containing arrays of local points and global points.
-        """
-        self.df = pd.read_csv(self.csv_file)
-        # Extract local and global points
-        local_points = self.df[["local_x", "local_y", "local_z"]].values
-        global_points = self.df[["global_x", "global_y", "global_z"]].values
-        return local_points, global_points
-
-    def _get_transM_LR(self, local_points, global_points):
-        """
-        Computes the transformation matrix from local to global coordinates.
-
-        Args:
-            local_points (np.array): Array of local points.
-            global_points (np.array): Array of global points.
-
-        Returns:
-            tuple: Linear regression model and transformation matrix.
-        """
-        local_points_with_bias = np.hstack(
-            [local_points, np.ones((local_points.shape[0], 1))]
-        )
-
-        # Train the linear regression model
-        model = LinearRegression(fit_intercept=False)
-        model.fit(local_points_with_bias, global_points)
-
-        # Weights and Bias
-        # All but last column, which are the weights
-        weights = model.coef_[:, :-1]
-        bias = model.coef_[:, -1] # Last column, which is the bias
-
-        # Combine weights and bias to form the transformation matrix
-        transformation_matrix = np.hstack([weights, bias.reshape(-1, 1)])
-        # Adding the extra row to complete the affine transformation matrix
-        transformation_matrix = np.vstack([transformation_matrix, [0, 0, 0, 1]])
-
-        return model, transformation_matrix
-
-    def _update_local_global_point(self):
-        """
-        Updates the CSV file with a new set of local and global points from the current stage position.
-        """
-        with open(self.csv_file, "a", newline="") as file:
-            writer = csv.writer(file)
-            writer.writerow(
-                [
-                    self.stage.stage_x,
-                    self.stage.stage_y,
-                    self.stage.stage_z,
-                    self.stage.stage_x_global,
-                    self.stage.stage_y_global,
-                    self.stage.stage_z_global,
-                ]
-            )
-
-    def _is_criteria_met_transM(self):
-        """
-        Checks if the transformation matrix has stabilized within certain thresholds.
-
-        Returns:
-            bool: True if the criteria are met, otherwise False.
-        """
-        diff_matrix = np.abs(self.transM_LR - self.transM_LR_prev)
-        if np.all(diff_matrix <= self.threshold_matrix):
-            return True
-        else:
-            return False
-
-    def _update_min_max_x_y_z(self):
-        self.min_x, self.max_x = min(self.min_x, self.stage.stage_x), max(
-            self.max_x, self.stage.stage_x
-        )
-        self.min_y, self.max_y = min(self.min_y, self.stage.stage_y), max(
-            self.max_y, self.stage.stage_y
-        )
-        self.min_z, self.max_z = min(self.min_z, self.stage.stage_z), max(
-            self.max_z, self.stage.stage_z
-        )
-
-    def _is_criteria_met_points_min_max(self):
-        """
-        Checks if the range of collected points in each direction exceeds minimum thresholds.
-
-        Returns:
-            bool: True if sufficient range is achieved, otherwise False.
-        """
-        
-        if self.max_x - self.min_x > self.threshold_min_max \
-            or self.max_y - self.min_y > self.threshold_min_max \
-            or self.max_z - self.min_z > self.threshold_min_max:
-            self._enough_points_emit_signal()
-
-        if self.max_x - self.min_x > self.threshold_min_max \
-            and self.max_y - self.min_y > self.threshold_min_max \
-            and self.max_z - self.min_z > self.threshold_min_max:
-            return True
-        else:
-            return False
-
-    def _apply_transformation(self):
-        """
-        Applies the calculated transformation matrix to convert a local point to global coordinates.
-
-        Returns:
-            np.array: The transformed global point.
-        """
-        local_point = np.array(
-            [self.stage.stage_x, self.stage.stage_y, self.stage.stage_z, 1]
-        )
-        global_point = np.dot(self.transM_LR, local_point)
-        return global_point[:3]
-
-    def _l2_error_current_point(self):
-        transformed_point = self._apply_transformation()
-        global_point = np.array(
-            [
-                self.stage.stage_x_global,
-                self.stage.stage_y_global,
-                self.stage.stage_z_global,
-            ]
-        )
-        LR_err_L2 = np.linalg.norm(transformed_point - global_point)
-
-        return LR_err_L2
-
-    def _is_criteria_met_l2_error(self):
-        """
-        Evaluates if the L2 error between the transformed point and the actual global point is within threshold.
-
-        Returns:
-            bool: True if the error is within threshold, otherwise False.
-        """
-        if self.LR_err_L2_current <= self.LR_err_L2_threshold:
-            return True
-        else:
-            return False
-
-    def _enough_points_emit_signal(self):
-        """
-        Emits calibration complete signals based on the sufficiency of point ranges in each direction.
-        """
-        if (
-            not self.signal_emitted_x
-            and self.max_x - self.min_x > self.threshold_min_max
-        ):
-            self.calib_complete_x.emit()
-            self.signal_emitted_x = True
-        if (
-            not self.signal_emitted_y
-            and self.max_y - self.min_y > self.threshold_min_max
-        ):
-            self.calib_complete_y.emit()
-            self.signal_emitted_y = True
-        if (
-            not self.signal_emitted_z
-            and self.max_z - self.min_z > self.threshold_min_max
-        ):
-            self.calib_complete_z.emit()
-            self.signal_emitted_z = True
-
-    def _is_enough_points(self):
-        """Check if there are enough points for calibration.
-
-        Returns:
-            bool: True if there are enough points, False otherwise.
-        """
-        # End Criteria:
-        # 1. distance maxX-minX, maxY-minY, maxZ-minZ
-        # 2. transM_LR difference in some epsilon value
-        # 3. L2 error (Global and Exp) is less than some values (e.g. 20 mincrons)
-        if self._is_criteria_met_points_min_max():
-            if self._is_criteria_met_transM():
-                if self._is_criteria_met_l2_error():
-                    logger.debug("Enough points gathered.")
-                    return True
-
-        self.transM_LR_prev = self.transM_LR
-        return False
-
-    def _update_info_ui(self):
-        x_diff = self.max_x - self.min_x
-        y_diff = self.max_y - self.min_y
-        z_diff = self.max_z - self.min_z
-        self.transM_info.emit(
-            self.transM_LR,
-            self.LR_err_L2_current,
-            np.array([x_diff, y_diff, z_diff]),
-        )
-
-    def update(self, stage):
-        """
-        Main method to update calibration with a new stage position and check if calibration is complete.
-
-        Args:
-            stage (Stage): The current stage object with new position data.
-        """
-        # update points in the file
-        self.stage = stage
-        self._update_local_global_point()
-        # get whole list of local and global points in pd format
-        local_points, global_points = self._get_local_global_points()
-        self.model_LR, self.transM_LR = self._get_transM_LR(
-            local_points, global_points
-        )
-        self.LR_err_L2_current = self._l2_error_current_point()
-        self._update_min_max_x_y_z()  # update min max x,y,z
-
-        # update transformation matrix and overall LR in UI
-        self._update_info_ui()
-
-        # if ret, send the signal
-        ret = self._is_enough_points()
-        if ret:
-            self.calib_complete.emit(self.stage.sn, self.transM_LR)
-            logger.debug(
-                f"complete probe calibration {self.stage.sn}, {self.transM_LR}"
-            )
-
-    def reshape_array(self):
-        """
-        Reshapes arrays of local and global points for processing.
-
-        Returns:
-            tuple: Reshaped local and global points arrays.
-        """
-        local_points = np.array(self.local_points)
-        global_points = np.array(self.global_points)
-        return local_points.reshape(-1, 1, 3), global_points.reshape(-1, 1, 3)
+"""
+ProbeCalibration transforms probe coordinates from local to global space"
+- local space: Stage coordinates
+- global space: Reticle coordinates
+"""
+
+import csv
+import logging
+import os
+
+import numpy as np
+import pandas as pd
+from PyQt5.QtCore import QObject, pyqtSignal
+from sklearn.linear_model import LinearRegression
+
+# Set logger name
+logger = logging.getLogger(__name__)
+logger.setLevel(logging.DEBUG)
+# Set the logging level for PyQt5.uic.uiparser/properties to WARNING, to ignore DEBUG messages
+logging.getLogger("PyQt5.uic.uiparser").setLevel(logging.WARNING)
+logging.getLogger("PyQt5.uic.properties").setLevel(logging.WARNING)
+
+
+class ProbeCalibration(QObject):
+    """
+    Handles the transformation of probe coordinates from local (stage) to global (reticle) space.
+
+    Attributes:
+        calib_complete_x (pyqtSignal): Signal emitted when calibration in the X direction is complete.
+        calib_complete_y (pyqtSignal): Signal emitted when calibration in the Y direction is complete.
+        calib_complete_z (pyqtSignal): Signal emitted when calibration in the Z direction is complete.
+        calib_complete (pyqtSignal): General signal emitted when calibration is fully complete.
+
+    Args:
+        stage_listener (QObject): The stage listener object that emits signals related to stage movements.
+    """
+
+    calib_complete_x = pyqtSignal()
+    calib_complete_y = pyqtSignal()
+    calib_complete_z = pyqtSignal()
+    calib_complete = pyqtSignal(str, object)
+    transM_info = pyqtSignal(object, float, object)
+
+    """Class for probe calibration."""
+
+    def __init__(self, stage_listener):
+        """
+        Initializes the ProbeCalibration object with a given stage listener.
+        """
+        super().__init__()
+        self.stage_listener = stage_listener
+        self.stage_listener.probeCalibRequest.connect(self.update)
+        self.stages = {}
+        self.df = None
+        self.inliers = []
+        self.stage = None
+        self.threshold_min_max = 2000  # TODO
+        self.model_LR, self.transM_LR, self.transM_LR_prev = None, None, None
+        self.threshold_matrix = np.array(
+            [
+                [0.00002, 0.00002, 0.00002, 50.0],  # TODO
+                [0.00002, 0.00002, 0.00002, 50.0],
+                [0.00002, 0.00002, 0.00002, 50.0],
+                [0.0, 0.0, 0.0, 0.0],
+            ]
+        )
+        self.LR_err_L2_threshold = 20  # TODO
+        self._create_file()
+
+        # Test signal
+        self.reset_calib()
+
+    def reset_calib(self):
+        """
+        Resets calibration to its initial state, clearing any stored min and max values.
+        """
+        self.min_x, self.max_x = float("inf"), float("-inf")
+        self.min_y, self.max_y = float("inf"), float("-inf")
+        self.min_z, self.max_z = float("inf"), float("-inf")
+        self.transM_LR_prev = np.zeros((4, 4), dtype=np.float64)
+        self.signal_emitted_x = False
+        self.signal_emitted_y = False
+        self.signal_emitted_z = False
+
+    def _create_file(self):
+        """
+        Creates or clears the CSV file used to store local and global points during calibration.
+        """
+        package_dir = os.path.dirname(os.path.abspath(__file__))
+        debug_dir = os.path.join(os.path.dirname(package_dir), "debug")
+        os.makedirs(debug_dir, exist_ok=True)
+        self.csv_file = os.path.join(debug_dir, "points.csv")
+
+        # Check if the file exists and remove it if it does
+        if os.path.exists(self.csv_file):
+            os.remove(self.csv_file)
+
+        # Create a new file and write column names
+        with open(self.csv_file, "w", newline="") as file:
+            writer = csv.writer(file)
+            # Define column names
+            column_names = [
+                "local_x",
+                "local_y",
+                "local_z",
+                "global_x",
+                "global_y",
+                "global_z",
+            ]
+            writer.writerow(column_names)
+
+    def clear(self):
+        """
+        Clears all stored data and resets the transformation matrix to its default state.
+        """
+        self._create_file()
+        self.model_LR, self.transM_LR, self.transM_LR_prev = None, None, None
+
+    def _get_local_global_points(self):
+        """
+        Retrieves local and global points from the CSV file as numpy arrays.
+
+        Returns:
+            tuple: A tuple containing arrays of local points and global points.
+        """
+        self.df = pd.read_csv(self.csv_file)
+        # Extract local and global points
+        local_points = self.df[["local_x", "local_y", "local_z"]].values
+        global_points = self.df[["global_x", "global_y", "global_z"]].values
+        return local_points, global_points
+
+    def _get_transM_LR(self, local_points, global_points):
+        """
+        Computes the transformation matrix from local to global coordinates.
+
+        Args:
+            local_points (np.array): Array of local points.
+            global_points (np.array): Array of global points.
+
+        Returns:
+            tuple: Linear regression model and transformation matrix.
+        """
+        local_points_with_bias = np.hstack(
+            [local_points, np.ones((local_points.shape[0], 1))]
+        )
+
+        # Train the linear regression model
+        model = LinearRegression(fit_intercept=False)
+        model.fit(local_points_with_bias, global_points)
+
+        # Weights and Bias
+        # All but last column, which are the weights
+        weights = model.coef_[:, :-1]
+        bias = model.coef_[:, -1] # Last column, which is the bias
+
+        # Combine weights and bias to form the transformation matrix
+        transformation_matrix = np.hstack([weights, bias.reshape(-1, 1)])
+        # Adding the extra row to complete the affine transformation matrix
+        transformation_matrix = np.vstack([transformation_matrix, [0, 0, 0, 1]])
+
+        return model, transformation_matrix
+
+    def _update_local_global_point(self):
+        """
+        Updates the CSV file with a new set of local and global points from the current stage position.
+        """
+        with open(self.csv_file, "a", newline="") as file:
+            writer = csv.writer(file)
+            writer.writerow(
+                [
+                    self.stage.stage_x,
+                    self.stage.stage_y,
+                    self.stage.stage_z,
+                    self.stage.stage_x_global,
+                    self.stage.stage_y_global,
+                    self.stage.stage_z_global,
+                ]
+            )
+
+    def _is_criteria_met_transM(self):
+        """
+        Checks if the transformation matrix has stabilized within certain thresholds.
+
+        Returns:
+            bool: True if the criteria are met, otherwise False.
+        """
+        diff_matrix = np.abs(self.transM_LR - self.transM_LR_prev)
+        if np.all(diff_matrix <= self.threshold_matrix):
+            return True
+        else:
+            return False
+
+    def _update_min_max_x_y_z(self):
+        self.min_x, self.max_x = min(self.min_x, self.stage.stage_x), max(
+            self.max_x, self.stage.stage_x
+        )
+        self.min_y, self.max_y = min(self.min_y, self.stage.stage_y), max(
+            self.max_y, self.stage.stage_y
+        )
+        self.min_z, self.max_z = min(self.min_z, self.stage.stage_z), max(
+            self.max_z, self.stage.stage_z
+        )
+
+    def _is_criteria_met_points_min_max(self):
+        """
+        Checks if the range of collected points in each direction exceeds minimum thresholds.
+
+        Returns:
+            bool: True if sufficient range is achieved, otherwise False.
+        """
+        
+        if self.max_x - self.min_x > self.threshold_min_max \
+            or self.max_y - self.min_y > self.threshold_min_max \
+            or self.max_z - self.min_z > self.threshold_min_max:
+            self._enough_points_emit_signal()
+
+        if self.max_x - self.min_x > self.threshold_min_max \
+            and self.max_y - self.min_y > self.threshold_min_max \
+            and self.max_z - self.min_z > self.threshold_min_max:
+            return True
+        else:
+            return False
+
+    def _apply_transformation(self):
+        """
+        Applies the calculated transformation matrix to convert a local point to global coordinates.
+
+        Returns:
+            np.array: The transformed global point.
+        """
+        local_point = np.array(
+            [self.stage.stage_x, self.stage.stage_y, self.stage.stage_z, 1]
+        )
+        global_point = np.dot(self.transM_LR, local_point)
+        return global_point[:3]
+
+    def _l2_error_current_point(self):
+        transformed_point = self._apply_transformation()
+        global_point = np.array(
+            [
+                self.stage.stage_x_global,
+                self.stage.stage_y_global,
+                self.stage.stage_z_global,
+            ]
+        )
+        LR_err_L2 = np.linalg.norm(transformed_point - global_point)
+
+        return LR_err_L2
+
+    def _is_criteria_met_l2_error(self):
+        """
+        Evaluates if the L2 error between the transformed point and the actual global point is within threshold.
+
+        Returns:
+            bool: True if the error is within threshold, otherwise False.
+        """
+        if self.LR_err_L2_current <= self.LR_err_L2_threshold:
+            return True
+        else:
+            return False
+
+    def _enough_points_emit_signal(self):
+        """
+        Emits calibration complete signals based on the sufficiency of point ranges in each direction.
+        """
+        if (
+            not self.signal_emitted_x
+            and self.max_x - self.min_x > self.threshold_min_max
+        ):
+            self.calib_complete_x.emit()
+            self.signal_emitted_x = True
+        if (
+            not self.signal_emitted_y
+            and self.max_y - self.min_y > self.threshold_min_max
+        ):
+            self.calib_complete_y.emit()
+            self.signal_emitted_y = True
+        if (
+            not self.signal_emitted_z
+            and self.max_z - self.min_z > self.threshold_min_max
+        ):
+            self.calib_complete_z.emit()
+            self.signal_emitted_z = True
+
+    def _is_enough_points(self):
+        """Check if there are enough points for calibration.
+
+        Returns:
+            bool: True if there are enough points, False otherwise.
+        """
+        # End Criteria:
+        # 1. distance maxX-minX, maxY-minY, maxZ-minZ
+        # 2. transM_LR difference in some epsilon value
+        # 3. L2 error (Global and Exp) is less than some values (e.g. 20 mincrons)
+        if self._is_criteria_met_points_min_max():
+            if self._is_criteria_met_transM():
+                if self._is_criteria_met_l2_error():
+                    logger.debug("Enough points gathered.")
+                    return True
+
+        self.transM_LR_prev = self.transM_LR
+        return False
+
+    def _update_info_ui(self):
+        x_diff = self.max_x - self.min_x
+        y_diff = self.max_y - self.min_y
+        z_diff = self.max_z - self.min_z
+        self.transM_info.emit(
+            self.transM_LR,
+            self.LR_err_L2_current,
+            np.array([x_diff, y_diff, z_diff]),
+        )
+
+    def update(self, stage):
+        """
+        Main method to update calibration with a new stage position and check if calibration is complete.
+
+        Args:
+            stage (Stage): The current stage object with new position data.
+        """
+        # update points in the file
+        self.stage = stage
+        self._update_local_global_point()
+        # get whole list of local and global points in pd format
+        local_points, global_points = self._get_local_global_points()
+        self.model_LR, self.transM_LR = self._get_transM_LR(
+            local_points, global_points
+        )
+        self.LR_err_L2_current = self._l2_error_current_point()
+        self._update_min_max_x_y_z()  # update min max x,y,z
+
+        # update transformation matrix and overall LR in UI
+        self._update_info_ui()
+
+        # if ret, send the signal
+        ret = self._is_enough_points()
+        if ret:
+            self.calib_complete.emit(self.stage.sn, self.transM_LR)
+            logger.debug(
+                f"complete probe calibration {self.stage.sn}, {self.transM_LR}"
+            )
+
+    def reshape_array(self):
+        """
+        Reshapes arrays of local and global points for processing.
+
+        Returns:
+            tuple: Reshaped local and global points arrays.
+        """
+        local_points = np.array(self.local_points)
+        global_points = np.array(self.global_points)
+        return local_points.reshape(-1, 1, 3), global_points.reshape(-1, 1, 3)
```

### Comparing `parallax_app-0.37.1/parallax/probe_detect_manager.py` & `parallax_app-0.37.5/parallax/probe_detect_manager.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,323 +1,323 @@
-"""
-ProbeDetectManager coordinates probe detection in images, leveraging PyQt threading 
-and signals for real-time processing. It handles frame updates, detection, 
-and result communication, utilizing components like MaskGenerator and ProbeDetector.
-"""
-
-import logging
-import time
-
-import cv2
-import numpy as np
-from PyQt5.QtCore import QObject, QThread, pyqtSignal
-
-from .curr_bg_cmp_processor import CurrBgCmpProcessor
-from .curr_prev_cmp_processor import CurrPrevCmpProcessor
-from .mask_generator import MaskGenerator
-from .probe_detector import ProbeDetector
-from .reticle_detection import ReticleDetection
-
-# Set logger name
-logger = logging.getLogger(__name__)
-# Set the logging level for PyQt5.uic.uiparser/properties to WARNING, to ignore DEBUG messages
-logging.getLogger("PyQt5.uic.uiparser").setLevel(logging.WARNING)
-logging.getLogger("PyQt5.uic.properties").setLevel(logging.WARNING)
-
-
-class ProbeDetectManager(QObject):
-    """Manager class for probe detection."""
-
-    name = "None"
-    frame_processed = pyqtSignal(object)
-    found_coords = pyqtSignal(str, str, tuple, tuple)
-
-    class Worker(QObject):
-        """Worker class for probe detection."""
-
-        finished = pyqtSignal()
-        frame_processed = pyqtSignal(object)
-        found_coords = pyqtSignal(str, str, tuple)
-
-        def __init__(self, name, model):
-            """Initialize Worker object"""
-            QObject.__init__(self)
-            self.model = model
-            self.name = name
-            self.running = False
-            self.is_detection_on = False
-            self.new = False
-            self.frame = None
-            self.reticle_coords = self.model.get_coords_axis(self.name)
-
-            # TODO move to model structure
-            self.prev_img = None
-            self.reticle_zone = None
-            self.is_probe_updated = True
-            self.probes = {}
-            self.sn = None
-
-            self.IMG_SIZE = (1000, 750)
-            self.IMG_SIZE_ORIGINAL = (4000, 3000)  # TODO
-            self.CROP_INIT = 50
-            self.mask_detect = MaskGenerator()
-
-        def update_sn(self, sn):
-            """Update the serial number and initialize probe detectors.
-
-            Args:
-                sn (str): Serial number.
-            """
-            if sn not in self.probes.keys():
-                self.sn = sn
-                self.probeDetect = ProbeDetector(self.sn, self.IMG_SIZE)
-                self.currPrevCmpProcess = CurrPrevCmpProcessor(
-                    self.probeDetect, self.IMG_SIZE_ORIGINAL, self.IMG_SIZE
-                )
-                self.currBgCmpProcess = CurrBgCmpProcessor(
-                    self.probeDetect, self.IMG_SIZE_ORIGINAL, self.IMG_SIZE
-                )
-                self.probes[self.sn] = {
-                    "probeDetector": self.probeDetect,
-                    "currPrevCmpProcess": self.currPrevCmpProcess,
-                    "currBgCmpProcess": self.currBgCmpProcess,
-                }
-            else:
-                if sn != self.sn:
-                    self.sn = sn
-                    self.probeDetect = self.probes[self.sn]["probeDetector"]
-                    self.currPrevCmpProcess = self.probes[self.sn][
-                        "currPrevCmpProcess"
-                    ]
-                    self.currBgCmpProcess = self.probes[self.sn][
-                        "currBgCmpProcess"
-                    ]
-                else:
-                    pass
-
-        def update_frame(self, frame, timestamp):
-            """Update the frame and timestamp.
-
-            Args:
-                frame (numpy.ndarray): Input frame.
-                timestamp (str): Timestamp of the frame.
-            """
-            self.frame = frame
-            self.new = True
-            self.timestamp = timestamp
-
-        def process(self, frame, timestamp):
-            """Process the frame for probe detection.
-            1. First run currPrevCmpProcess
-            2. If it fails on 1, run currBgCmpProcess
-
-            Args:
-                frame (numpy.ndarray): Input frame.
-                timestamp (str): Timestamp of the frame.
-
-            Returns:
-                tuple: Processed frame and timestamp.
-            """
-            if frame.ndim > 2:
-                gray_img = cv2.cvtColor(frame, cv2.COLOR_BGR2GRAY)
-            else:
-                gray_img = frame
-
-            resized_img = cv2.resize(gray_img, self.IMG_SIZE)
-            self.curr_img = cv2.GaussianBlur(resized_img, (9, 9), 0)
-            mask = self.mask_detect.process(resized_img)  # Generate Mask
-
-            if self.mask_detect.is_reticle_exist and self.reticle_zone is None:
-                reticle = ReticleDetection(
-                    self.IMG_SIZE, self.mask_detect, self.name
-                )
-                self.reticle_zone = reticle.get_reticle_zone(
-                    frame
-                )  # Generate X and Y Coordinates zone
-                self.currBgCmpProcess.update_reticle_zone(self.reticle_zone)
-
-            if self.prev_img is not None:
-                if (
-                    self.probeDetect.angle is None
-                ):  # Detecting probe for the first time
-                    ret = self.currPrevCmpProcess.first_cmp(
-                        self.curr_img, self.prev_img, mask, gray_img
-                    )
-                    if ret is False:
-                        ret = self.currBgCmpProcess.first_cmp(
-                            self.curr_img, mask, gray_img
-                        )
-                    if ret:
-                        logger.debug("First detect")
-                        logger.debug(
-                            f"angle: {self.probeDetect.angle}, \
-                            tip: {self.probeDetect.probe_tip}, \
-                            base: {self.probeDetect.probe_base}"
-                        )
-                else:  # Tracking for the known probe
-                    ret = self.currPrevCmpProcess.update_cmp(
-                        self.curr_img, self.prev_img, mask, gray_img
-                    )
-                    if ret is False:
-                        ret = self.currBgCmpProcess.update_cmp(
-                            self.curr_img, mask, gray_img
-                        )
-
-                    if ret:  # Found
-                        self.found_coords.emit(
-                            timestamp, self.sn, self.probeDetect.probe_tip_org
-                        )
-                        cv2.circle(
-                            frame,
-                            self.probeDetect.probe_tip_org,
-                            5,
-                            (255, 255, 0),
-                            -1,
-                        )
-
-                if ret:
-                    self.prev_img = self.curr_img
-            else:
-                self.prev_img = self.curr_img
-
-            return frame, timestamp
-
-        def stop_running(self):
-            """Stop the worker from running."""
-            self.running = False
-
-        def start_running(self):
-            """Start the worker running."""
-            self.running = True
-
-        def start_detection(self):
-            """Start the probe detection."""
-            self.is_detection_on = True
-
-        def stop_detection(self):
-            """Stop the probe detection."""
-            self.is_detection_on = False
-
-        def process_draw_reticle(self, frame):
-            if self.reticle_coords is not None:
-                for idx, coords in enumerate(self.reticle_coords):
-                    # Normalize indices to 0-255 for colormap application.
-                    indices = np.linspace(
-                        0, 255, len(coords), endpoint=True, dtype=np.uint8
-                    )
-                    # Apply 'jet' colormap to x-coords, 'winter' to the y-coords.
-                    colormap = cv2.applyColorMap(
-                        indices,
-                        cv2.COLORMAP_JET if idx == 0 else cv2.COLORMAP_WINTER,
-                    )
-
-                    for point_idx, (x, y) in enumerate(coords):
-                        color = colormap[point_idx][0].tolist()
-                        cv2.circle(frame, (x, y), 2, color, -1)
-            return frame
-
-        def run(self):
-            """Run the worker thread."""
-            print("probe_detect_manager running ")
-            while self.running:
-                if self.new:
-                    if self.is_detection_on:
-                        self.frame, self.timestamp = self.process(
-                            self.frame, self.timestamp
-                        )
-                    self.frame = self.process_draw_reticle(self.frame)
-                    self.frame_processed.emit(self.frame)
-                    self.new = False
-                time.sleep(0.001)
-            print("probe_detect_manager running done")
-            self.finished.emit()
-
-    def __init__(self, model, camera_name):
-        """Initialize ProbeDetectManager object"""
-        super().__init__()
-        self.model = model
-        self.worker = None
-        self.name = camera_name
-        self.thread = None
-        self.init_thread()
-
-    def init_thread(self):
-        """Initialize the worker thread."""
-        self.thread = QThread()
-        self.worker = self.Worker(self.name, self.model)
-        self.worker.moveToThread(self.thread)
-        self.thread.started.connect(self.worker.run)
-        self.worker.frame_processed.connect(self.frame_processed)
-        self.worker.found_coords.connect(self.found_coords_print)
-        self.worker.finished.connect(self.thread.quit)
-        self.worker.finished.connect(self.worker.deleteLater)
-        self.thread.finished.connect(self.thread.deleteLater)
-
-    def process(self, frame, timestamp):
-        """Process the frame using the worker.
-
-        Args:
-            frame (numpy.ndarray): Input frame.
-            timestamp (str): Timestamp of the frame.
-        """
-        if self.worker is not None:
-            self.worker.update_frame(frame, timestamp)
-
-    def found_coords_print(self, timestamp, sn, pixel_coords):
-        """Emit the found coordinates signal.
-
-        Args:
-            timestamp (str): Timestamp of the frame.
-            sn (str): Serial number.
-            pixel_coords (tuple): Pixel coordinates of the probe tip.
-        """
-        moving_stage = self.model.get_stage(sn)
-        if moving_stage is not None:
-            stage_info = (
-                moving_stage.stage_x,
-                moving_stage.stage_y,
-                moving_stage.stage_z,
-            )
-        # print(timestamp, sn, stage_info, pixel_coords)
-        self.found_coords.emit(timestamp, sn, stage_info, pixel_coords)
-
-    def start(self):
-        """Start the probe detection manager."""
-        self.init_thread()  # Reinitialize and start the worker and thread
-        self.worker.start_running()
-        self.thread.start()
-
-    def stop(self):
-        """Stop the probe detection manager."""
-        if self.worker is not None:
-            self.worker.stop_running()
-
-    def start_detection(self, sn):  # Call from stage listener.
-        """Start the probe detection for a specific serial number.
-
-        Args:
-            sn (str): Serial number.
-        """
-        if self.worker is not None:
-            self.worker.update_sn(sn)
-            self.worker.start_detection()
-
-    def stop_detection(self, sn):  # Call from stage listener.
-        """Stop the probe detection for a specific serial number.
-
-        Args:
-            sn (str): Serial number.
-        """
-        if self.worker is not None:
-            self.worker.stop_detection()
-
-    def clean(self):
-        """Clean up the probe detection manager."""
-        if self.worker is not None:
-            self.worker.stop_running()
-        if self.thread is not None:
-            self.thread.quit()
-            self.thread.wait()
-
-    def __del__(self):
-        """Destructor for the probe detection manager."""
+"""
+ProbeDetectManager coordinates probe detection in images, leveraging PyQt threading 
+and signals for real-time processing. It handles frame updates, detection, 
+and result communication, utilizing components like MaskGenerator and ProbeDetector.
+"""
+
+import logging
+import time
+
+import cv2
+import numpy as np
+from PyQt5.QtCore import QObject, QThread, pyqtSignal
+
+from .curr_bg_cmp_processor import CurrBgCmpProcessor
+from .curr_prev_cmp_processor import CurrPrevCmpProcessor
+from .mask_generator import MaskGenerator
+from .probe_detector import ProbeDetector
+from .reticle_detection import ReticleDetection
+
+# Set logger name
+logger = logging.getLogger(__name__)
+# Set the logging level for PyQt5.uic.uiparser/properties to WARNING, to ignore DEBUG messages
+logging.getLogger("PyQt5.uic.uiparser").setLevel(logging.WARNING)
+logging.getLogger("PyQt5.uic.properties").setLevel(logging.WARNING)
+
+
+class ProbeDetectManager(QObject):
+    """Manager class for probe detection."""
+
+    name = "None"
+    frame_processed = pyqtSignal(object)
+    found_coords = pyqtSignal(str, str, tuple, tuple)
+
+    class Worker(QObject):
+        """Worker class for probe detection."""
+
+        finished = pyqtSignal()
+        frame_processed = pyqtSignal(object)
+        found_coords = pyqtSignal(str, str, tuple)
+
+        def __init__(self, name, model):
+            """Initialize Worker object"""
+            QObject.__init__(self)
+            self.model = model
+            self.name = name
+            self.running = False
+            self.is_detection_on = False
+            self.new = False
+            self.frame = None
+            self.reticle_coords = self.model.get_coords_axis(self.name)
+
+            # TODO move to model structure
+            self.prev_img = None
+            self.reticle_zone = None
+            self.is_probe_updated = True
+            self.probes = {}
+            self.sn = None
+
+            self.IMG_SIZE = (1000, 750)
+            self.IMG_SIZE_ORIGINAL = (4000, 3000)  # TODO
+            self.CROP_INIT = 50
+            self.mask_detect = MaskGenerator()
+
+        def update_sn(self, sn):
+            """Update the serial number and initialize probe detectors.
+
+            Args:
+                sn (str): Serial number.
+            """
+            if sn not in self.probes.keys():
+                self.sn = sn
+                self.probeDetect = ProbeDetector(self.sn, self.IMG_SIZE)
+                self.currPrevCmpProcess = CurrPrevCmpProcessor(
+                    self.probeDetect, self.IMG_SIZE_ORIGINAL, self.IMG_SIZE
+                )
+                self.currBgCmpProcess = CurrBgCmpProcessor(
+                    self.probeDetect, self.IMG_SIZE_ORIGINAL, self.IMG_SIZE
+                )
+                self.probes[self.sn] = {
+                    "probeDetector": self.probeDetect,
+                    "currPrevCmpProcess": self.currPrevCmpProcess,
+                    "currBgCmpProcess": self.currBgCmpProcess,
+                }
+            else:
+                if sn != self.sn:
+                    self.sn = sn
+                    self.probeDetect = self.probes[self.sn]["probeDetector"]
+                    self.currPrevCmpProcess = self.probes[self.sn][
+                        "currPrevCmpProcess"
+                    ]
+                    self.currBgCmpProcess = self.probes[self.sn][
+                        "currBgCmpProcess"
+                    ]
+                else:
+                    pass
+
+        def update_frame(self, frame, timestamp):
+            """Update the frame and timestamp.
+
+            Args:
+                frame (numpy.ndarray): Input frame.
+                timestamp (str): Timestamp of the frame.
+            """
+            self.frame = frame
+            self.new = True
+            self.timestamp = timestamp
+
+        def process(self, frame, timestamp):
+            """Process the frame for probe detection.
+            1. First run currPrevCmpProcess
+            2. If it fails on 1, run currBgCmpProcess
+
+            Args:
+                frame (numpy.ndarray): Input frame.
+                timestamp (str): Timestamp of the frame.
+
+            Returns:
+                tuple: Processed frame and timestamp.
+            """
+            if frame.ndim > 2:
+                gray_img = cv2.cvtColor(frame, cv2.COLOR_BGR2GRAY)
+            else:
+                gray_img = frame
+
+            resized_img = cv2.resize(gray_img, self.IMG_SIZE)
+            self.curr_img = cv2.GaussianBlur(resized_img, (9, 9), 0)
+            mask = self.mask_detect.process(resized_img)  # Generate Mask
+
+            if self.mask_detect.is_reticle_exist and self.reticle_zone is None:
+                reticle = ReticleDetection(
+                    self.IMG_SIZE, self.mask_detect, self.name
+                )
+                self.reticle_zone = reticle.get_reticle_zone(
+                    frame
+                )  # Generate X and Y Coordinates zone
+                self.currBgCmpProcess.update_reticle_zone(self.reticle_zone)
+
+            if self.prev_img is not None:
+                if (
+                    self.probeDetect.angle is None
+                ):  # Detecting probe for the first time
+                    ret = self.currPrevCmpProcess.first_cmp(
+                        self.curr_img, self.prev_img, mask, gray_img
+                    )
+                    if ret is False:
+                        ret = self.currBgCmpProcess.first_cmp(
+                            self.curr_img, mask, gray_img
+                        )
+                    if ret:
+                        logger.debug("First detect")
+                        logger.debug(
+                            f"angle: {self.probeDetect.angle}, \
+                            tip: {self.probeDetect.probe_tip}, \
+                            base: {self.probeDetect.probe_base}"
+                        )
+                else:  # Tracking for the known probe
+                    ret = self.currPrevCmpProcess.update_cmp(
+                        self.curr_img, self.prev_img, mask, gray_img
+                    )
+                    if ret is False:
+                        ret = self.currBgCmpProcess.update_cmp(
+                            self.curr_img, mask, gray_img
+                        )
+
+                    if ret:  # Found
+                        self.found_coords.emit(
+                            timestamp, self.sn, self.probeDetect.probe_tip_org
+                        )
+                        cv2.circle(
+                            frame,
+                            self.probeDetect.probe_tip_org,
+                            5,
+                            (255, 255, 0),
+                            -1,
+                        )
+
+                if ret:
+                    self.prev_img = self.curr_img
+            else:
+                self.prev_img = self.curr_img
+
+            return frame, timestamp
+
+        def stop_running(self):
+            """Stop the worker from running."""
+            self.running = False
+
+        def start_running(self):
+            """Start the worker running."""
+            self.running = True
+
+        def start_detection(self):
+            """Start the probe detection."""
+            self.is_detection_on = True
+
+        def stop_detection(self):
+            """Stop the probe detection."""
+            self.is_detection_on = False
+
+        def process_draw_reticle(self, frame):
+            if self.reticle_coords is not None:
+                for idx, coords in enumerate(self.reticle_coords):
+                    # Normalize indices to 0-255 for colormap application.
+                    indices = np.linspace(
+                        0, 255, len(coords), endpoint=True, dtype=np.uint8
+                    )
+                    # Apply 'jet' colormap to x-coords, 'winter' to the y-coords.
+                    colormap = cv2.applyColorMap(
+                        indices,
+                        cv2.COLORMAP_JET if idx == 0 else cv2.COLORMAP_WINTER,
+                    )
+
+                    for point_idx, (x, y) in enumerate(coords):
+                        color = colormap[point_idx][0].tolist()
+                        cv2.circle(frame, (x, y), 2, color, -1)
+            return frame
+
+        def run(self):
+            """Run the worker thread."""
+            print("probe_detect_manager running ")
+            while self.running:
+                if self.new:
+                    if self.is_detection_on:
+                        self.frame, self.timestamp = self.process(
+                            self.frame, self.timestamp
+                        )
+                    self.frame = self.process_draw_reticle(self.frame)
+                    self.frame_processed.emit(self.frame)
+                    self.new = False
+                time.sleep(0.001)
+            print("probe_detect_manager running done")
+            self.finished.emit()
+
+    def __init__(self, model, camera_name):
+        """Initialize ProbeDetectManager object"""
+        super().__init__()
+        self.model = model
+        self.worker = None
+        self.name = camera_name
+        self.thread = None
+        self.init_thread()
+
+    def init_thread(self):
+        """Initialize the worker thread."""
+        self.thread = QThread()
+        self.worker = self.Worker(self.name, self.model)
+        self.worker.moveToThread(self.thread)
+        self.thread.started.connect(self.worker.run)
+        self.worker.frame_processed.connect(self.frame_processed)
+        self.worker.found_coords.connect(self.found_coords_print)
+        self.worker.finished.connect(self.thread.quit)
+        self.worker.finished.connect(self.worker.deleteLater)
+        self.thread.finished.connect(self.thread.deleteLater)
+
+    def process(self, frame, timestamp):
+        """Process the frame using the worker.
+
+        Args:
+            frame (numpy.ndarray): Input frame.
+            timestamp (str): Timestamp of the frame.
+        """
+        if self.worker is not None:
+            self.worker.update_frame(frame, timestamp)
+
+    def found_coords_print(self, timestamp, sn, pixel_coords):
+        """Emit the found coordinates signal.
+
+        Args:
+            timestamp (str): Timestamp of the frame.
+            sn (str): Serial number.
+            pixel_coords (tuple): Pixel coordinates of the probe tip.
+        """
+        moving_stage = self.model.get_stage(sn)
+        if moving_stage is not None:
+            stage_info = (
+                moving_stage.stage_x,
+                moving_stage.stage_y,
+                moving_stage.stage_z,
+            )
+        # print(timestamp, sn, stage_info, pixel_coords)
+        self.found_coords.emit(timestamp, sn, stage_info, pixel_coords)
+
+    def start(self):
+        """Start the probe detection manager."""
+        self.init_thread()  # Reinitialize and start the worker and thread
+        self.worker.start_running()
+        self.thread.start()
+
+    def stop(self):
+        """Stop the probe detection manager."""
+        if self.worker is not None:
+            self.worker.stop_running()
+
+    def start_detection(self, sn):  # Call from stage listener.
+        """Start the probe detection for a specific serial number.
+
+        Args:
+            sn (str): Serial number.
+        """
+        if self.worker is not None:
+            self.worker.update_sn(sn)
+            self.worker.start_detection()
+
+    def stop_detection(self, sn):  # Call from stage listener.
+        """Stop the probe detection for a specific serial number.
+
+        Args:
+            sn (str): Serial number.
+        """
+        if self.worker is not None:
+            self.worker.stop_detection()
+
+    def clean(self):
+        """Clean up the probe detection manager."""
+        if self.worker is not None:
+            self.worker.stop_running()
+        if self.thread is not None:
+            self.thread.quit()
+            self.thread.wait()
+
+    def __del__(self):
+        """Destructor for the probe detection manager."""
         self.clean()
```

### Comparing `parallax_app-0.37.1/parallax/probe_detector.py` & `parallax_app-0.37.5/parallax/probe_detector.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,487 +1,487 @@
-"""
-ProbeDetector identifies probe tip and base in images using contour processing 
-and Hough Line Transform, with gradient analysis for refinement and directional 
-checks to ensure accuracy.
-"""
-
-import logging
-from collections import Counter
-
-import cv2
-import numpy as np
-
-# Set logger name
-logger = logging.getLogger(__name__)
-# Set the logging level for PyQt5.uic.uiparser/properties to WARNING, to ignore DEBUG messages
-logging.getLogger("PyQt5.uic.uiparser").setLevel(logging.WARNING)
-logging.getLogger("PyQt5.uic.properties").setLevel(logging.WARNING)
-
-
-class ProbeDetector:
-    """Class for detecting the probe in an image."""
-
-    def __init__(self, sn, IMG_SIZE, angle_step=9):
-        """Initialize Probe Detector object"""
-        self.sn = sn
-        self.IMG_SIZE = IMG_SIZE
-        self.angle_step = angle_step
-        self.angle = None
-        self.probe_tip, self.probe_base = (0, 0), (0, 0)
-        self.probe_tip_org = (0, 0)
-        self.probe_tip_direction = "S"
-        self.gradients = []
-        self.angle_step_bins, self.angle_step_bins_with_neighbor = [], []
-        self._init_gradient_bins()
-
-    def _init_gradient_bins(self):
-        """Initialize gradient bins."""
-        self.angle_step_bins = np.arange(
-            0, 180 + self.angle_step, self.angle_step
-        )
-        self.angle_step_bins_with_neighbor = np.append(
-            np.insert(self.angle_step_bins, 0, 180), 0
-        )
-
-    def _find_represent_gradient(self, gradient=0):
-        """Find the representative gradient.
-        Returns:
-            float: Representative gradient value.
-        """
-        index = np.argmin(np.abs(self.angle_step_bins - gradient))
-        return self.angle_step_bins[index]
-
-    def _find_neighboring_gradients(self, target_angle):
-        """Find the neighboring gradients.
-        Args:
-            target_angle (float): Target angle.
-        Returns:
-            numpy.ndarray: Neighboring gradients.
-        """
-        gradient_index = np.where(self.angle_step_bins == target_angle)[0][0]
-        neighboring_gradients = self.angle_step_bins_with_neighbor[
-            gradient_index : gradient_index + 3
-        ]
-        return neighboring_gradients
-
-    def _contour_preprocessing(
-        self, img, thresh=20, remove_noise=True, noise_threshold=1
-    ):
-        """Preprocess the image using contour detection.
-        Args:
-            img (numpy.ndarray): Input image.
-            thresh (int): Threshold for contour area. Defaults to 20.
-            remove_noise (bool): Flag to remove noise contours. Defaults to True.
-            noise_threshold (int): Threshold for noise contour area. Defaults to 1.
-        Returns:
-            numpy.ndarray: Preprocessed image.
-        """
-        # Contour
-        contours, _ = cv2.findContours(
-            img, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE
-        )
-        if not contours:
-            logger.debug(f"get_probe:: Not found contours. threshold: {thresh}")
-            return None
-        largest_contour = max(contours, key=cv2.contourArea)
-        if cv2.contourArea(largest_contour) < thresh:
-            logger.debug(
-                f"get_probe:: largest_contour is less than threshold {cv2.contourArea(largest_contour)}"
-            )
-            return None
-        if remove_noise:
-            for contour in contours:
-                # Remove Noise
-                if cv2.contourArea(contour) < noise_threshold*noise_threshold:
-                    img = cv2.drawContours(img, [contour], -1, (0, 0, 0), -1)
-        return img
-
-    def _get_probe_direction(self, probe_tip, probe_base):
-        """Get the direction of the probe.
-        Args:
-            probe_tip (tuple): Coordinates of the probe tip.
-            probe_base (tuple): Coordinates of the probe base.
-        Returns:
-            str: Direction of the probe (N, NE, E, SE, S, SW, W, NW, Unknown).
-        """
-        dx = probe_tip[0] - probe_base[0]
-        dy = probe_tip[1] - probe_base[1]
-        if dy > 0:
-            if dx > 0:
-                return "SE"
-            elif dx < 0:
-                return "SW"
-            else:
-                return "S"
-        elif dy < 0:
-            if dx > 0:
-                return "NE"
-            elif dx < 0:
-                return "NW"
-            else:
-                return "N"
-        else:
-            if dx > 0:
-                return "E"
-            elif dx < 0:
-                return "W"
-            else:
-                return "Unknown"
-
-    def _hough_line_first_detection(
-        self, img, minLineLength=150, maxLineGap=40
-    ):
-        """Perform Hough line detection for the first time.
-
-        Args:
-            img (numpy.ndarray): Input image.
-            minLineLength (int): Minimum length of the line. Defaults to 150.
-            maxLineGap (int): Maximum gap between line segments. Defaults to 40.
-
-        Returns:
-            tuple: (found_ret, highest_point, lowest_point)
-                - found_ret (bool): Flag indicating if the probe is found.
-                - highest_point (tuple): Coordinates of the highest point of the probe.
-                - lowest_point (tuple): Coordinates of the lowest point of the probe.
-        """
-        found_ret = False
-        self.gradients = []
-        max_y, min_y = 0, img.shape[0]
-        lowest_point = (0, 0)
-        highest_point = (0, 0)
-        line_segments = cv2.HoughLinesP(
-            img,
-            1,
-            np.pi / 180,
-            100,
-            minLineLength=minLineLength,
-            maxLineGap=maxLineGap,
-        )
-
-        # Draw the line segments
-        if line_segments is not None:
-            # logger.debug(len(line_segments))
-            if (len(line_segments)) >= 30:
-                logger.debug(
-                    "hough_line_detection:: Too many line detected. Possibly Plane image "
-                )
-                return None, highest_point, lowest_point
-
-            for line in line_segments:
-                x2, y2, x1, y1 = line[0]
-                # Calculate the gradient
-                gradient = np.arctan2(y2 - y1, x2 - x1)
-                gradient = np.degrees(gradient)
-                gradient += 180
-                gradient %= 180
-                representing_gradient = self._find_represent_gradient(gradient)
-                self.gradients.append(representing_gradient)
-                if y1 > max_y:
-                    max_y = y1
-                    lowest_point = (x1, y1)
-                if y2 > max_y:
-                    max_y = y2
-                    lowest_point = (x2, y2)
-                if y1 < min_y:
-                    min_y = y1
-                    highest_point = (x1, y1)
-                if y2 <= min_y:
-                    min_y = y2
-                    highest_point = (x2, y2)
-
-        if len(self.gradients) > 0:
-            if self._is_distance_in_thres(highest_point, lowest_point):
-                logger.debug(
-                    f"Distance between tip and base is too close {highest_point} {lowest_point}"
-                )
-                return False, highest_point, lowest_point
-            found_ret = True
-            logger.debug(f"First line detection {self.gradients}")
-            self.angle = np.median(self.gradients)
-            return found_ret, highest_point, lowest_point
-        else:
-            return found_ret, highest_point, lowest_point
-
-    def _hough_line_update(self, img, minLineLength=50, maxLineGap=9):
-        """Update the Hough line detection.
-        Args:
-            img (numpy.ndarray): Input image.
-            minLineLength (int): Minimum length of the line. Defaults to 50.
-            maxLineGap (int): Maximum gap between line segments. Defaults to 9.
-
-        Returns:
-            tuple: (found_ret, highest_point, lowest_point)
-                - found_ret (bool): Flag indicating if the probe is found.
-                - highest_point (tuple): Coordinates of the highest point of the probe.
-                - lowest_point (tuple): Coordinates of the lowest point of the probe.
-        """
-        self.gradients = []
-        updated_gradient = self.angle
-        max_y, min_y = 0, img.shape[0]
-        line_segments = cv2.HoughLinesP(
-            img,
-            1,
-            np.pi / 180,
-            50,
-            minLineLength=minLineLength,
-            maxLineGap=maxLineGap,
-        )
-        found_ret, lowest_point, highest_point = False, (0, 0), (0, 0)
-
-        # Find the neighboring gradients
-        gradient_index = np.where(self.angle_step_bins == self.angle)
-
-        if gradient_index is None:
-            return found_ret, highest_point, lowest_point
-
-        # Check if gradient_index is not empty
-        if gradient_index[0].size == 0:
-            return found_ret, highest_point, lowest_point
-
-        gradient_index = gradient_index[0][0]
-        neighboring_gradients = self.angle_step_bins_with_neighbor[
-            gradient_index : gradient_index + 3
-        ]
-
-        # Draw the line segments
-        if line_segments is not None:
-            if (len(line_segments)) >= 30:
-                logger.debug(
-                    "get_tip_hough_line_detection:: Too many line detected. Possibly Plane image"
-                )
-                return found_ret, highest_point, lowest_point
-
-            for line in line_segments:
-                x2, y2, x1, y1 = line[0]
-                # Calculate the gradient
-                gradient = np.arctan2(y2 - y1, x2 - x1)
-                gradient = np.degrees(gradient)
-                gradient += 180
-                gradient %= 180
-                representing_gradient = self._find_represent_gradient(gradient)
-
-                if representing_gradient in neighboring_gradients:
-                    self.gradients.append(representing_gradient)
-                    found_ret = True
-                    if y1 > max_y:
-                        max_y = y1
-                        lowest_point = (x1, y1)
-                    if y2 > max_y:
-                        max_y = y2
-                        lowest_point = (x2, y2)
-                    if y1 < min_y:
-                        min_y = y1
-                        highest_point = (x1, y1)
-                    if y2 <= min_y:
-                        min_y = y2
-                        highest_point = (x2, y2)
-
-            if found_ret is False:
-                return found_ret, highest_point, lowest_point
-        else:
-            logger.debug("get_tip_hough_line_detection:: Not found the line")
-            return found_ret, highest_point, lowest_point
-
-        if found_ret:
-            if self._is_distance_in_thres(highest_point, lowest_point):
-                logger.debug(
-                    f"Distance between tip and base is too close, {highest_point} {lowest_point}"
-                )
-                return False, highest_point, lowest_point
-
-            gradient_counts = Counter(self.gradients)
-            updated_gradient, _ = gradient_counts.most_common(1)[0]
-            logger.debug(
-                f"target angle: {self.angle}, updated_detected: {updated_gradient}, neighbor: {neighboring_gradients}"
-            )
-            # logger.debug(gradient_counts)
-            self.angle = updated_gradient
-            return found_ret, highest_point, lowest_point
-        else:
-            return found_ret, highest_point, lowest_point
-
-    def _get_probe_point(self, mask, p1, p2, img_fname=None):
-        """Get the probe tip and base points.
-
-        Args:
-            mask (numpy.ndarray): Mask image.
-            p1 (tuple): First point coordinates.
-            p2 (tuple): Second point coordinates.
-            img_fname (str, optional): Image filename. Defaults to None.
-
-        Returns:
-            tuple: (probe_tip, probe_base)
-                - probe_tip (tuple): Coordinates of the probe tip.
-                - probe_base (tuple): Coordinates of the probe base.
-        """
-
-        mask = cv2.copyMakeBorder(
-            mask, 1, 1, 1, 1, cv2.BORDER_CONSTANT, value=[0, 0, 0]
-        )
-        dist_transform = cv2.distanceTransform(mask, cv2.DIST_L2, 3)
-        """
-        if img_fname:
-            mask_ = cv2.cvtColor(mask, cv2.COLOR_GRAY2BGR)
-            cv2.circle(mask_, p1, 5, (0, 255, 0), -1)  # Green circle
-            cv2.circle(mask_, p2, 5, (0, 0, 255), -1)  # Green circle
-            
-            output_fname = os.path.basename(img_fname).replace('.', '_mask.')
-            cv2.imwrite('output/' + output_fname, mask_)
-        """
-        dist_p1 = dist_transform[p1[1], p1[0]]  # [y, x]
-        dist_p2 = dist_transform[p2[1], p2[0]]
-        logger.debug(f"dist_p1: {dist_p1}, dist_p2: {dist_p2}")
-        if dist_p1 > dist_p2:
-            return p1, p2  # Return order: probe_tip, probe_base
-        else:
-            return p2, p1
-
-    def _get_probe_point_known_direction(
-        self, highest_point, lowest_point, direction="S"
-    ):
-        """Get the probe tip and base points based on known direction.
-
-        Args:
-            highest_point (tuple): Coordinates of the highest point.
-            lowest_point (tuple): Coordinates of the lowest point.
-            direction (str): Direction of the probe. Defaults to "S".
-
-        Returns:
-            tuple: (probe_tip, probe_base)
-                - probe_tip (tuple): Coordinates of the probe tip.
-                - probe_base (tuple): Coordinates of the probe base.
-        """
-        if direction in ["S", "W", "SW", "SE"]:
-            return lowest_point, highest_point
-        else:
-            return highest_point, lowest_point
-
-    def _is_distance_in_thres(self, point1, point2, thres=50):
-        """Check if the distance between two points is within a threshold.
-
-        Args:
-            point1 (tuple): Coordinates of the first point.
-            point2 (tuple): Coordinates of the second point.
-            thres (int): Distance threshold. Defaults to 50.
-
-        Returns:
-            bool: True if the distance is within the threshold, False otherwise.
-        """
-        dist = ((point1[0] - point2[0]) ** 2 +
-                (point1[1] - point2[1]) ** 2 )** 0.5
-        return dist < thres
-
-    # Get the gradient / pixel points of probe at first time
-    def first_detect_probe(
-        self,
-        img,
-        mask,
-        contour_thresh=50,
-        hough_minLineLength=130,
-        offset_x=0,
-        offset_y=0,
-    ):
-        """Detect the probe in the image for the first time.
-
-        Args:
-            img (numpy.ndarray): Input image.
-            mask (numpy.ndarray): Mask image.
-            contour_thresh (int): Threshold for contour area. Defaults to 50.
-            hough_minLineLength (int): Minimum length of the line for Hough transform. Defaults to 130.
-            offset_x (int): X-offset for probe coordinates.
-            offset_y (int): Y-offset for probe coordinates.
-
-        Returns:
-            bool: True if the probe is detected, False otherwise.
-        """
-        ret = False
-        img = self._contour_preprocessing(img, thresh=contour_thresh)
-        if img is None:
-            return ret
-
-        ret, highest_point, lowest_point = self._hough_line_first_detection(
-            img, minLineLength=hough_minLineLength, maxLineGap=50
-        )  # update self.angle
-        if ret:
-            self.probe_tip, self.probe_base = self._get_probe_point(
-                mask, highest_point, lowest_point
-            )
-            self.probe_tip_direction = self._get_probe_direction(
-                self.probe_tip, self.probe_base
-            )
-            self.probe_tip = (
-                self.probe_tip[0] + offset_x,
-                self.probe_tip[1] + offset_y,
-            )
-            self.probe_base = (
-                self.probe_base[0] + offset_x,
-                self.probe_base[1] + offset_y,
-            )
-            logger.debug(f"tip : {self.probe_tip}, base: {self.probe_base}")
-        return ret
-
-    def update_probe(
-        self,
-        img,
-        mask,
-        contour_thresh=20,
-        hough_minLineLength=200,
-        maxLineGap=10,
-        offset_x=0,
-        offset_y=0,
-        img_fname=None,
-    ):
-        """Update the probe detection in the image."""
-        ret = False
-        img = self._contour_preprocessing(
-            img, thresh=contour_thresh, remove_noise=False
-        )
-        if img is None:
-            logger.debug("update_probe:: contour_preprocessing fail")
-            return False
-
-        backup_angle = self.angle
-        ret, highest_point, lowest_point = self._hough_line_update(
-            img, minLineLength=hough_minLineLength, maxLineGap=maxLineGap
-        )  # self.angle updated
-        if ret:
-            highest_point = (
-                highest_point[0] + offset_x,
-                highest_point[1] + offset_y,
-            )
-            lowest_point = (
-                lowest_point[0] + offset_x,
-                lowest_point[1] + offset_y,
-            )
-
-            logger.debug(
-                f"backup_angle: {backup_angle}, self.angle: {self.angle}"
-            )
-            if self.angle == backup_angle:
-                self.probe_tip, self.probe_base = (
-                    self._get_probe_point_known_direction(
-                        highest_point,
-                        lowest_point,
-                        direction=self.probe_tip_direction,
-                    )
-                )
-            else:
-                self.probe_tip, self.probe_base = self._get_probe_point(
-                    mask, highest_point, lowest_point
-                )
-                self.probe_tip_direction = self._get_probe_direction(
-                    self.probe_tip, self.probe_base
-                )
-
-                """
-                print(self.probe_tip, self.probe_base, self.probe_tip_direction)
-                mask = cv2.cvtColor(mask, cv2.COLOR_GRAY2BGR)
-                cv2.circle(mask, self.probe_tip, 3, (0, 0, 255), 5)  # RED circle
-                cv2.circle(mask, self.probe_base, 3, (0, 255, 0), 5)  # RED circle
-                output_fname = os.path.basename(img_fname).replace('.', '_4_mask.')
-                cv2.imwrite('output/' + output_fname, mask)
-                """
-        else:
-            logger.debug("update_probe:: get_tip_hough_line_detection fail")
-            return False
-
+"""
+ProbeDetector identifies probe tip and base in images using contour processing 
+and Hough Line Transform, with gradient analysis for refinement and directional 
+checks to ensure accuracy.
+"""
+
+import logging
+from collections import Counter
+
+import cv2
+import numpy as np
+
+# Set logger name
+logger = logging.getLogger(__name__)
+# Set the logging level for PyQt5.uic.uiparser/properties to WARNING, to ignore DEBUG messages
+logging.getLogger("PyQt5.uic.uiparser").setLevel(logging.WARNING)
+logging.getLogger("PyQt5.uic.properties").setLevel(logging.WARNING)
+
+
+class ProbeDetector:
+    """Class for detecting the probe in an image."""
+
+    def __init__(self, sn, IMG_SIZE, angle_step=9):
+        """Initialize Probe Detector object"""
+        self.sn = sn
+        self.IMG_SIZE = IMG_SIZE
+        self.angle_step = angle_step
+        self.angle = None
+        self.probe_tip, self.probe_base = (0, 0), (0, 0)
+        self.probe_tip_org = (0, 0)
+        self.probe_tip_direction = "S"
+        self.gradients = []
+        self.angle_step_bins, self.angle_step_bins_with_neighbor = [], []
+        self._init_gradient_bins()
+
+    def _init_gradient_bins(self):
+        """Initialize gradient bins."""
+        self.angle_step_bins = np.arange(
+            0, 180 + self.angle_step, self.angle_step
+        )
+        self.angle_step_bins_with_neighbor = np.append(
+            np.insert(self.angle_step_bins, 0, 180), 0
+        )
+
+    def _find_represent_gradient(self, gradient=0):
+        """Find the representative gradient.
+        Returns:
+            float: Representative gradient value.
+        """
+        index = np.argmin(np.abs(self.angle_step_bins - gradient))
+        return self.angle_step_bins[index]
+
+    def _find_neighboring_gradients(self, target_angle):
+        """Find the neighboring gradients.
+        Args:
+            target_angle (float): Target angle.
+        Returns:
+            numpy.ndarray: Neighboring gradients.
+        """
+        gradient_index = np.where(self.angle_step_bins == target_angle)[0][0]
+        neighboring_gradients = self.angle_step_bins_with_neighbor[
+            gradient_index : gradient_index + 3
+        ]
+        return neighboring_gradients
+
+    def _contour_preprocessing(
+        self, img, thresh=20, remove_noise=True, noise_threshold=1
+    ):
+        """Preprocess the image using contour detection.
+        Args:
+            img (numpy.ndarray): Input image.
+            thresh (int): Threshold for contour area. Defaults to 20.
+            remove_noise (bool): Flag to remove noise contours. Defaults to True.
+            noise_threshold (int): Threshold for noise contour area. Defaults to 1.
+        Returns:
+            numpy.ndarray: Preprocessed image.
+        """
+        # Contour
+        contours, _ = cv2.findContours(
+            img, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE
+        )
+        if not contours:
+            logger.debug(f"get_probe:: Not found contours. threshold: {thresh}")
+            return None
+        largest_contour = max(contours, key=cv2.contourArea)
+        if cv2.contourArea(largest_contour) < thresh:
+            logger.debug(
+                f"get_probe:: largest_contour is less than threshold {cv2.contourArea(largest_contour)}"
+            )
+            return None
+        if remove_noise:
+            for contour in contours:
+                # Remove Noise
+                if cv2.contourArea(contour) < noise_threshold*noise_threshold:
+                    img = cv2.drawContours(img, [contour], -1, (0, 0, 0), -1)
+        return img
+
+    def _get_probe_direction(self, probe_tip, probe_base):
+        """Get the direction of the probe.
+        Args:
+            probe_tip (tuple): Coordinates of the probe tip.
+            probe_base (tuple): Coordinates of the probe base.
+        Returns:
+            str: Direction of the probe (N, NE, E, SE, S, SW, W, NW, Unknown).
+        """
+        dx = probe_tip[0] - probe_base[0]
+        dy = probe_tip[1] - probe_base[1]
+        if dy > 0:
+            if dx > 0:
+                return "SE"
+            elif dx < 0:
+                return "SW"
+            else:
+                return "S"
+        elif dy < 0:
+            if dx > 0:
+                return "NE"
+            elif dx < 0:
+                return "NW"
+            else:
+                return "N"
+        else:
+            if dx > 0:
+                return "E"
+            elif dx < 0:
+                return "W"
+            else:
+                return "Unknown"
+
+    def _hough_line_first_detection(
+        self, img, minLineLength=150, maxLineGap=40
+    ):
+        """Perform Hough line detection for the first time.
+
+        Args:
+            img (numpy.ndarray): Input image.
+            minLineLength (int): Minimum length of the line. Defaults to 150.
+            maxLineGap (int): Maximum gap between line segments. Defaults to 40.
+
+        Returns:
+            tuple: (found_ret, highest_point, lowest_point)
+                - found_ret (bool): Flag indicating if the probe is found.
+                - highest_point (tuple): Coordinates of the highest point of the probe.
+                - lowest_point (tuple): Coordinates of the lowest point of the probe.
+        """
+        found_ret = False
+        self.gradients = []
+        max_y, min_y = 0, img.shape[0]
+        lowest_point = (0, 0)
+        highest_point = (0, 0)
+        line_segments = cv2.HoughLinesP(
+            img,
+            1,
+            np.pi / 180,
+            100,
+            minLineLength=minLineLength,
+            maxLineGap=maxLineGap,
+        )
+
+        # Draw the line segments
+        if line_segments is not None:
+            # logger.debug(len(line_segments))
+            if (len(line_segments)) >= 30:
+                logger.debug(
+                    "hough_line_detection:: Too many line detected. Possibly Plane image "
+                )
+                return None, highest_point, lowest_point
+
+            for line in line_segments:
+                x2, y2, x1, y1 = line[0]
+                # Calculate the gradient
+                gradient = np.arctan2(y2 - y1, x2 - x1)
+                gradient = np.degrees(gradient)
+                gradient += 180
+                gradient %= 180
+                representing_gradient = self._find_represent_gradient(gradient)
+                self.gradients.append(representing_gradient)
+                if y1 > max_y:
+                    max_y = y1
+                    lowest_point = (x1, y1)
+                if y2 > max_y:
+                    max_y = y2
+                    lowest_point = (x2, y2)
+                if y1 < min_y:
+                    min_y = y1
+                    highest_point = (x1, y1)
+                if y2 <= min_y:
+                    min_y = y2
+                    highest_point = (x2, y2)
+
+        if len(self.gradients) > 0:
+            if self._is_distance_in_thres(highest_point, lowest_point):
+                logger.debug(
+                    f"Distance between tip and base is too close {highest_point} {lowest_point}"
+                )
+                return False, highest_point, lowest_point
+            found_ret = True
+            logger.debug(f"First line detection {self.gradients}")
+            self.angle = np.median(self.gradients)
+            return found_ret, highest_point, lowest_point
+        else:
+            return found_ret, highest_point, lowest_point
+
+    def _hough_line_update(self, img, minLineLength=50, maxLineGap=9):
+        """Update the Hough line detection.
+        Args:
+            img (numpy.ndarray): Input image.
+            minLineLength (int): Minimum length of the line. Defaults to 50.
+            maxLineGap (int): Maximum gap between line segments. Defaults to 9.
+
+        Returns:
+            tuple: (found_ret, highest_point, lowest_point)
+                - found_ret (bool): Flag indicating if the probe is found.
+                - highest_point (tuple): Coordinates of the highest point of the probe.
+                - lowest_point (tuple): Coordinates of the lowest point of the probe.
+        """
+        self.gradients = []
+        updated_gradient = self.angle
+        max_y, min_y = 0, img.shape[0]
+        line_segments = cv2.HoughLinesP(
+            img,
+            1,
+            np.pi / 180,
+            50,
+            minLineLength=minLineLength,
+            maxLineGap=maxLineGap,
+        )
+        found_ret, lowest_point, highest_point = False, (0, 0), (0, 0)
+
+        # Find the neighboring gradients
+        gradient_index = np.where(self.angle_step_bins == self.angle)
+
+        if gradient_index is None:
+            return found_ret, highest_point, lowest_point
+
+        # Check if gradient_index is not empty
+        if gradient_index[0].size == 0:
+            return found_ret, highest_point, lowest_point
+
+        gradient_index = gradient_index[0][0]
+        neighboring_gradients = self.angle_step_bins_with_neighbor[
+            gradient_index : gradient_index + 3
+        ]
+
+        # Draw the line segments
+        if line_segments is not None:
+            if (len(line_segments)) >= 30:
+                logger.debug(
+                    "get_tip_hough_line_detection:: Too many line detected. Possibly Plane image"
+                )
+                return found_ret, highest_point, lowest_point
+
+            for line in line_segments:
+                x2, y2, x1, y1 = line[0]
+                # Calculate the gradient
+                gradient = np.arctan2(y2 - y1, x2 - x1)
+                gradient = np.degrees(gradient)
+                gradient += 180
+                gradient %= 180
+                representing_gradient = self._find_represent_gradient(gradient)
+
+                if representing_gradient in neighboring_gradients:
+                    self.gradients.append(representing_gradient)
+                    found_ret = True
+                    if y1 > max_y:
+                        max_y = y1
+                        lowest_point = (x1, y1)
+                    if y2 > max_y:
+                        max_y = y2
+                        lowest_point = (x2, y2)
+                    if y1 < min_y:
+                        min_y = y1
+                        highest_point = (x1, y1)
+                    if y2 <= min_y:
+                        min_y = y2
+                        highest_point = (x2, y2)
+
+            if found_ret is False:
+                return found_ret, highest_point, lowest_point
+        else:
+            logger.debug("get_tip_hough_line_detection:: Not found the line")
+            return found_ret, highest_point, lowest_point
+
+        if found_ret:
+            if self._is_distance_in_thres(highest_point, lowest_point):
+                logger.debug(
+                    f"Distance between tip and base is too close, {highest_point} {lowest_point}"
+                )
+                return False, highest_point, lowest_point
+
+            gradient_counts = Counter(self.gradients)
+            updated_gradient, _ = gradient_counts.most_common(1)[0]
+            logger.debug(
+                f"target angle: {self.angle}, updated_detected: {updated_gradient}, neighbor: {neighboring_gradients}"
+            )
+            # logger.debug(gradient_counts)
+            self.angle = updated_gradient
+            return found_ret, highest_point, lowest_point
+        else:
+            return found_ret, highest_point, lowest_point
+
+    def _get_probe_point(self, mask, p1, p2, img_fname=None):
+        """Get the probe tip and base points.
+
+        Args:
+            mask (numpy.ndarray): Mask image.
+            p1 (tuple): First point coordinates.
+            p2 (tuple): Second point coordinates.
+            img_fname (str, optional): Image filename. Defaults to None.
+
+        Returns:
+            tuple: (probe_tip, probe_base)
+                - probe_tip (tuple): Coordinates of the probe tip.
+                - probe_base (tuple): Coordinates of the probe base.
+        """
+
+        mask = cv2.copyMakeBorder(
+            mask, 1, 1, 1, 1, cv2.BORDER_CONSTANT, value=[0, 0, 0]
+        )
+        dist_transform = cv2.distanceTransform(mask, cv2.DIST_L2, 3)
+        """
+        if img_fname:
+            mask_ = cv2.cvtColor(mask, cv2.COLOR_GRAY2BGR)
+            cv2.circle(mask_, p1, 5, (0, 255, 0), -1)  # Green circle
+            cv2.circle(mask_, p2, 5, (0, 0, 255), -1)  # Green circle
+            
+            output_fname = os.path.basename(img_fname).replace('.', '_mask.')
+            cv2.imwrite('output/' + output_fname, mask_)
+        """
+        dist_p1 = dist_transform[p1[1], p1[0]]  # [y, x]
+        dist_p2 = dist_transform[p2[1], p2[0]]
+        logger.debug(f"dist_p1: {dist_p1}, dist_p2: {dist_p2}")
+        if dist_p1 > dist_p2:
+            return p1, p2  # Return order: probe_tip, probe_base
+        else:
+            return p2, p1
+
+    def _get_probe_point_known_direction(
+        self, highest_point, lowest_point, direction="S"
+    ):
+        """Get the probe tip and base points based on known direction.
+
+        Args:
+            highest_point (tuple): Coordinates of the highest point.
+            lowest_point (tuple): Coordinates of the lowest point.
+            direction (str): Direction of the probe. Defaults to "S".
+
+        Returns:
+            tuple: (probe_tip, probe_base)
+                - probe_tip (tuple): Coordinates of the probe tip.
+                - probe_base (tuple): Coordinates of the probe base.
+        """
+        if direction in ["S", "W", "SW", "SE"]:
+            return lowest_point, highest_point
+        else:
+            return highest_point, lowest_point
+
+    def _is_distance_in_thres(self, point1, point2, thres=50):
+        """Check if the distance between two points is within a threshold.
+
+        Args:
+            point1 (tuple): Coordinates of the first point.
+            point2 (tuple): Coordinates of the second point.
+            thres (int): Distance threshold. Defaults to 50.
+
+        Returns:
+            bool: True if the distance is within the threshold, False otherwise.
+        """
+        dist = ((point1[0] - point2[0]) ** 2 +
+                (point1[1] - point2[1]) ** 2 )** 0.5
+        return dist < thres
+
+    # Get the gradient / pixel points of probe at first time
+    def first_detect_probe(
+        self,
+        img,
+        mask,
+        contour_thresh=50,
+        hough_minLineLength=130,
+        offset_x=0,
+        offset_y=0,
+    ):
+        """Detect the probe in the image for the first time.
+
+        Args:
+            img (numpy.ndarray): Input image.
+            mask (numpy.ndarray): Mask image.
+            contour_thresh (int): Threshold for contour area. Defaults to 50.
+            hough_minLineLength (int): Minimum length of the line for Hough transform. Defaults to 130.
+            offset_x (int): X-offset for probe coordinates.
+            offset_y (int): Y-offset for probe coordinates.
+
+        Returns:
+            bool: True if the probe is detected, False otherwise.
+        """
+        ret = False
+        img = self._contour_preprocessing(img, thresh=contour_thresh)
+        if img is None:
+            return ret
+
+        ret, highest_point, lowest_point = self._hough_line_first_detection(
+            img, minLineLength=hough_minLineLength, maxLineGap=50
+        )  # update self.angle
+        if ret:
+            self.probe_tip, self.probe_base = self._get_probe_point(
+                mask, highest_point, lowest_point
+            )
+            self.probe_tip_direction = self._get_probe_direction(
+                self.probe_tip, self.probe_base
+            )
+            self.probe_tip = (
+                self.probe_tip[0] + offset_x,
+                self.probe_tip[1] + offset_y,
+            )
+            self.probe_base = (
+                self.probe_base[0] + offset_x,
+                self.probe_base[1] + offset_y,
+            )
+            logger.debug(f"tip : {self.probe_tip}, base: {self.probe_base}")
+        return ret
+
+    def update_probe(
+        self,
+        img,
+        mask,
+        contour_thresh=20,
+        hough_minLineLength=200,
+        maxLineGap=10,
+        offset_x=0,
+        offset_y=0,
+        img_fname=None,
+    ):
+        """Update the probe detection in the image."""
+        ret = False
+        img = self._contour_preprocessing(
+            img, thresh=contour_thresh, remove_noise=False
+        )
+        if img is None:
+            logger.debug("update_probe:: contour_preprocessing fail")
+            return False
+
+        backup_angle = self.angle
+        ret, highest_point, lowest_point = self._hough_line_update(
+            img, minLineLength=hough_minLineLength, maxLineGap=maxLineGap
+        )  # self.angle updated
+        if ret:
+            highest_point = (
+                highest_point[0] + offset_x,
+                highest_point[1] + offset_y,
+            )
+            lowest_point = (
+                lowest_point[0] + offset_x,
+                lowest_point[1] + offset_y,
+            )
+
+            logger.debug(
+                f"backup_angle: {backup_angle}, self.angle: {self.angle}"
+            )
+            if self.angle == backup_angle:
+                self.probe_tip, self.probe_base = (
+                    self._get_probe_point_known_direction(
+                        highest_point,
+                        lowest_point,
+                        direction=self.probe_tip_direction,
+                    )
+                )
+            else:
+                self.probe_tip, self.probe_base = self._get_probe_point(
+                    mask, highest_point, lowest_point
+                )
+                self.probe_tip_direction = self._get_probe_direction(
+                    self.probe_tip, self.probe_base
+                )
+
+                """
+                print(self.probe_tip, self.probe_base, self.probe_tip_direction)
+                mask = cv2.cvtColor(mask, cv2.COLOR_GRAY2BGR)
+                cv2.circle(mask, self.probe_tip, 3, (0, 0, 255), 5)  # RED circle
+                cv2.circle(mask, self.probe_base, 3, (0, 255, 0), 5)  # RED circle
+                output_fname = os.path.basename(img_fname).replace('.', '_4_mask.')
+                cv2.imwrite('output/' + output_fname, mask)
+                """
+        else:
+            logger.debug("update_probe:: get_tip_hough_line_detection fail")
+            return False
+
         return ret
```

### Comparing `parallax_app-0.37.1/parallax/probe_fine_tip_detector.py` & `parallax_app-0.37.5/parallax/probe_fine_tip_detector.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,171 +1,171 @@
-"""
-ProbeFineTipDetector identifies a probe's fine tip in original images through preprocessing, 
-Harris corner detection, and geometric analysis, accommodating various probe orientations 
-for precise positioning tasks.
-"""
-
-import logging
-
-import cv2
-import numpy as np
-
-# Set logger name
-logger = logging.getLogger(__name__)
-# Set the logging level for PyQt5.uic.uiparser/properties to WARNING, to ignore DEBUG messages
-logging.getLogger("PyQt5.uic.uiparser").setLevel(logging.WARNING)
-logging.getLogger("PyQt5.uic.properties").setLevel(logging.WARNING)
-
-
-class ProbeFineTipDetector:
-    """Class for detecting the fine tip of the probe in an image."""
-
-    def __init__(self):
-        """Initialize ProbeFineTipDetector object"""
-        self.img = None
-        self.tip = (0, 0)
-        self.offset_x = 0
-        self.offset_y = 0
-        self.direction = "S"
-        self.img_fname = None
-
-    def _preprocess_image(self):
-        """Preprocess the image for tip detection."""
-        self.img = cv2.GaussianBlur(self.img, (7, 7), 0)
-        sharpened_image = cv2.Laplacian(self.img, cv2.CV_64F)
-        sharpened_image = np.uint8(np.absolute(sharpened_image))
-        _, self.img = cv2.threshold(
-            self.img, 0, 255, cv2.THRESH_BINARY + cv2.THRESH_OTSU
-        )
-        # kernel_ellipse_3 = cv2.getStructuringElement(cv2.MORPH_ELLIPSE, (3, 3)) #TODO
-        # self.img = cv2.erode(self.img, kernel_ellipse_3, iterations=1)
-
-    def _is_valid(self):
-        """Check if the image is valid for tip detection.
-        Returns:
-            bool: True if the image is valid, False otherwise.
-        """
-        height, width = self.img.shape[:2]
-        boundary_img = np.zeros_like(self.img)
-        cv2.rectangle(boundary_img, (0, 0), (width - 1, height - 1), 255, 1)
-        and_result = cv2.bitwise_and(cv2.bitwise_not(self.img), boundary_img)
-        contours_boundary, _ = cv2.findContours(
-            and_result, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE
-        )
-        if len(contours_boundary) >= 2:
-            logger.debug(
-                f"get_probe_precise_tip fail. N of contours_boundary :{len(contours_boundary)}"
-            )
-            return False
-
-        boundary_img = np.zeros_like(self.img)
-        boundary_img[0, 0] = 255
-        boundary_img[width - 1, 0] = 255
-        boundary_img[0, height - 1] = 255
-        boundary_img[width - 1, height - 1] = 255
-        and_result = cv2.bitwise_and(and_result, boundary_img)
-        contours_boundary, _ = cv2.findContours(
-            and_result, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE
-        )
-        if len(contours_boundary) >= 2:
-            logger.debug(
-                f"get_probe_precise_tip fail. No detection of tip :{len(contours_boundary)}"
-            )
-            return False
-
-        return True
-
-    def _detect_closest_centroid(self):
-        """Detect the closest centroid to the tip.
-
-        Returns:
-            tuple: Coordinates of the closest centroid.
-        """
-        cx, cy = self.tip[0], self.tip[1]
-        closest_centroid = (cx, cy)
-        min_distance = float("inf")
-
-        harris_corners = cv2.cornerHarris(self.img, blockSize=7, ksize=5, k=0.1)
-        threshold = 0.3 * harris_corners.max()
-
-        corner_marks = np.zeros_like(self.img)
-        corner_marks[harris_corners > threshold] = 255
-        contours, _ = cv2.findContours(
-            corner_marks, cv2.RETR_TREE, cv2.CHAIN_APPROX_SIMPLE
-        )
-
-        for contour in contours:
-            tip = self._get_direction_tip(contour)
-            tip_x, tip_y = tip[0] + self.offset_x, tip[1] + self.offset_y
-            distance = np.sqrt((tip_x - cx) ** 2 + (tip_y - cy) ** 2)
-            if distance < min_distance:
-                min_distance = distance
-                closest_centroid = (tip_x, tip_y)
-
-        return closest_centroid
-
-    def _get_direction_tip(self, contour):
-        """Get the tip coordinates based on the direction.
-
-        Args:
-            contour (numpy.ndarray): Contour of the tip.
-
-        Returns:
-            tuple: Coordinates of the tip based on the direction.
-        """
-        tip = (0, 0)
-        if self.direction == "S":
-            tip = max(contour, key=lambda point: point[0][1])[0]
-        elif self.direction == "N":
-            tip = min(contour, key=lambda point: point[0][1])[0]
-        elif self.direction == "E":
-            tip = max(contour, key=lambda point: point[0][0])[0]
-        elif self.direction == "W":
-            tip = min(contour, key=lambda point: point[0][0])[0]
-        elif self.direction == "NE":
-            tip = min(contour, key=lambda point: point[0][1] - point[0][0])[0]
-        elif self.direction == "NW":
-            tip = min(contour, key=lambda point: point[0][1] + point[0][0])[0]
-        elif self.direction == "SE":
-            tip = max(contour, key=lambda point: point[0][1] + point[0][0])[0]
-        elif self.direction == "SW":
-            tip = max(contour, key=lambda point: point[0][1] - point[0][0])[0]
-
-        return tip
-
-    def _register(
-        self, img, tip, offset_x=0, offset_y=0, direction=None, img_fname=None
-    ):
-        """Register the image, tip coordinates, offsets, direction, and filename."""
-        self.img = img
-        self.tip = tip
-        self.offset_x = offset_x
-        self.offset_y = offset_y
-        self.direction = direction
-        self.img_fname = img_fname
-
-    def get_precise_tip(
-        self, img, tip, offset_x=0, offset_y=0, direction=None, img_fname=None
-    ):
-        """Get the precise tip coordinates from the image."""
-        self._register(
-            img,
-            tip,
-            offset_x=offset_x,
-            offset_y=offset_y,
-            direction=direction,
-            img_fname=img_fname,
-        )
-
-        self._preprocess_image()
-        if not self._is_valid():
-            logger.debug("Boundary check failed.")
-            return False
-
-        self.tip = self._detect_closest_centroid()
-        # cv2.circle(self.img, (self.tip[0]-offset_x, self.tip[1]-offset_y), 1, (255, 255, 0), -1)
-
-        # Save the final image with the detected tip
-        # output_fname = os.path.basename(self.img_fname).replace('.', '_3_tip.')
-        # cv2.imwrite('output/' + output_fname, self.img_original)
-
-        return True
+"""
+ProbeFineTipDetector identifies a probe's fine tip in original images through preprocessing, 
+Harris corner detection, and geometric analysis, accommodating various probe orientations 
+for precise positioning tasks.
+"""
+
+import logging
+
+import cv2
+import numpy as np
+
+# Set logger name
+logger = logging.getLogger(__name__)
+# Set the logging level for PyQt5.uic.uiparser/properties to WARNING, to ignore DEBUG messages
+logging.getLogger("PyQt5.uic.uiparser").setLevel(logging.WARNING)
+logging.getLogger("PyQt5.uic.properties").setLevel(logging.WARNING)
+
+
+class ProbeFineTipDetector:
+    """Class for detecting the fine tip of the probe in an image."""
+
+    def __init__(self):
+        """Initialize ProbeFineTipDetector object"""
+        self.img = None
+        self.tip = (0, 0)
+        self.offset_x = 0
+        self.offset_y = 0
+        self.direction = "S"
+        self.img_fname = None
+
+    def _preprocess_image(self):
+        """Preprocess the image for tip detection."""
+        self.img = cv2.GaussianBlur(self.img, (7, 7), 0)
+        sharpened_image = cv2.Laplacian(self.img, cv2.CV_64F)
+        sharpened_image = np.uint8(np.absolute(sharpened_image))
+        _, self.img = cv2.threshold(
+            self.img, 0, 255, cv2.THRESH_BINARY + cv2.THRESH_OTSU
+        )
+        # kernel_ellipse_3 = cv2.getStructuringElement(cv2.MORPH_ELLIPSE, (3, 3)) #TODO
+        # self.img = cv2.erode(self.img, kernel_ellipse_3, iterations=1)
+
+    def _is_valid(self):
+        """Check if the image is valid for tip detection.
+        Returns:
+            bool: True if the image is valid, False otherwise.
+        """
+        height, width = self.img.shape[:2]
+        boundary_img = np.zeros_like(self.img)
+        cv2.rectangle(boundary_img, (0, 0), (width - 1, height - 1), 255, 1)
+        and_result = cv2.bitwise_and(cv2.bitwise_not(self.img), boundary_img)
+        contours_boundary, _ = cv2.findContours(
+            and_result, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE
+        )
+        if len(contours_boundary) >= 2:
+            logger.debug(
+                f"get_probe_precise_tip fail. N of contours_boundary :{len(contours_boundary)}"
+            )
+            return False
+
+        boundary_img = np.zeros_like(self.img)
+        boundary_img[0, 0] = 255
+        boundary_img[width - 1, 0] = 255
+        boundary_img[0, height - 1] = 255
+        boundary_img[width - 1, height - 1] = 255
+        and_result = cv2.bitwise_and(and_result, boundary_img)
+        contours_boundary, _ = cv2.findContours(
+            and_result, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE
+        )
+        if len(contours_boundary) >= 2:
+            logger.debug(
+                f"get_probe_precise_tip fail. No detection of tip :{len(contours_boundary)}"
+            )
+            return False
+
+        return True
+
+    def _detect_closest_centroid(self):
+        """Detect the closest centroid to the tip.
+
+        Returns:
+            tuple: Coordinates of the closest centroid.
+        """
+        cx, cy = self.tip[0], self.tip[1]
+        closest_centroid = (cx, cy)
+        min_distance = float("inf")
+
+        harris_corners = cv2.cornerHarris(self.img, blockSize=7, ksize=5, k=0.1)
+        threshold = 0.3 * harris_corners.max()
+
+        corner_marks = np.zeros_like(self.img)
+        corner_marks[harris_corners > threshold] = 255
+        contours, _ = cv2.findContours(
+            corner_marks, cv2.RETR_TREE, cv2.CHAIN_APPROX_SIMPLE
+        )
+
+        for contour in contours:
+            tip = self._get_direction_tip(contour)
+            tip_x, tip_y = tip[0] + self.offset_x, tip[1] + self.offset_y
+            distance = np.sqrt((tip_x - cx) ** 2 + (tip_y - cy) ** 2)
+            if distance < min_distance:
+                min_distance = distance
+                closest_centroid = (tip_x, tip_y)
+
+        return closest_centroid
+
+    def _get_direction_tip(self, contour):
+        """Get the tip coordinates based on the direction.
+
+        Args:
+            contour (numpy.ndarray): Contour of the tip.
+
+        Returns:
+            tuple: Coordinates of the tip based on the direction.
+        """
+        tip = (0, 0)
+        if self.direction == "S":
+            tip = max(contour, key=lambda point: point[0][1])[0]
+        elif self.direction == "N":
+            tip = min(contour, key=lambda point: point[0][1])[0]
+        elif self.direction == "E":
+            tip = max(contour, key=lambda point: point[0][0])[0]
+        elif self.direction == "W":
+            tip = min(contour, key=lambda point: point[0][0])[0]
+        elif self.direction == "NE":
+            tip = min(contour, key=lambda point: point[0][1] - point[0][0])[0]
+        elif self.direction == "NW":
+            tip = min(contour, key=lambda point: point[0][1] + point[0][0])[0]
+        elif self.direction == "SE":
+            tip = max(contour, key=lambda point: point[0][1] + point[0][0])[0]
+        elif self.direction == "SW":
+            tip = max(contour, key=lambda point: point[0][1] - point[0][0])[0]
+
+        return tip
+
+    def _register(
+        self, img, tip, offset_x=0, offset_y=0, direction=None, img_fname=None
+    ):
+        """Register the image, tip coordinates, offsets, direction, and filename."""
+        self.img = img
+        self.tip = tip
+        self.offset_x = offset_x
+        self.offset_y = offset_y
+        self.direction = direction
+        self.img_fname = img_fname
+
+    def get_precise_tip(
+        self, img, tip, offset_x=0, offset_y=0, direction=None, img_fname=None
+    ):
+        """Get the precise tip coordinates from the image."""
+        self._register(
+            img,
+            tip,
+            offset_x=offset_x,
+            offset_y=offset_y,
+            direction=direction,
+            img_fname=img_fname,
+        )
+
+        self._preprocess_image()
+        if not self._is_valid():
+            logger.debug("Boundary check failed.")
+            return False
+
+        self.tip = self._detect_closest_centroid()
+        # cv2.circle(self.img, (self.tip[0]-offset_x, self.tip[1]-offset_y), 1, (255, 255, 0), -1)
+
+        # Save the final image with the detected tip
+        # output_fname = os.path.basename(self.img_fname).replace('.', '_3_tip.')
+        # cv2.imwrite('output/' + output_fname, self.img_original)
+
+        return True
```

### Comparing `parallax_app-0.37.1/parallax/recording_manager.py` & `parallax_app-0.37.5/parallax/recording_manager.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,96 +1,96 @@
-"""
-RecordingManager manages snapshot saving and video recording from multiple camera feeds, 
-supporting custom file naming and ensuring recordings are properly initiated and 
-stopped across active cameras.
-"""
-
-import logging
-import os
-
-# Set logger name
-logger = logging.getLogger(__name__)
-# Set the logging level for PyQt5.uic.uiparser/properties to WARNING, to ignore DEBUG messages
-logging.getLogger("PyQt5.uic.uiparser").setLevel(logging.WARNING)
-logging.getLogger("PyQt5.uic.properties").setLevel(logging.WARNING)
-
-
-class RecordingManager:
-    """RecordingManager manages snapshot saving and video recording"""
-
-    def __init__(self, model):
-        """Initialize recording manager"""
-        self.model = model
-        self.recording_camera_list = []
-
-    def save_last_image(self, save_path, screen_widgets):
-        """Saves the last captured image from all active camera feeds."""
-        # Initialize the list to keep track of cameras from which an image has been saved
-        snapshot_camera_list = []
-        # Get the directory path where the images will be saved
-        if os.path.exists(save_path):
-            print("\nSnapshot...")
-            for screen in screen_widgets:
-                # Save image only for 'Blackfly' camera
-                if screen.is_camera():
-                    # Use custom name of the camera if it has one, otherwise use the camera's serial number
-                    camera_name = screen.get_camera_name()
-                    if camera_name not in snapshot_camera_list:
-                        customName = screen.parent().title()
-                        customName = customName if customName else camera_name
-
-                        # Save the image with a timestamp and custom name
-                        screen.save_image(
-                            save_path, isTimestamp=True, name=customName
-                        )
-
-                        # Add the camera to the list of cameras from which an image has been saved
-                        snapshot_camera_list.append(camera_name)
-                else:
-                    logger.debug("save_last_image) camera not found")
-        else:
-            print(f"Directory {save_path} does not exist!")
-
-    def save_recording(self, save_path, screen_widgets):
-        """
-        Initiates recording for all active camera feeds.
-        Records video from all active camera feeds and saves them to a specified directory.
-        The directory path is taken from the label showing the current save directory.
-        """
-        # Initialize the list to keep track of cameras that are currently recording
-        self.recording_camera_list = []
-
-        if os.path.exists(save_path):
-            # Iterate through each screen widget
-            print("\nRecording... ")
-            for screen in screen_widgets:
-                # Check if the current screen is a camera
-                if screen.is_camera():  # If name is 'Blackfly"
-                    camera_name = (
-                        screen.get_camera_name()
-                    )  # Get the name of the camer
-                    # If this camera is not already in the list of recording cameras, then record
-                    if camera_name not in self.recording_camera_list:
-                        # Use custom name of the camera if it has one, otherwise use the camera's serial number
-                        customName = screen.parent().title()
-                        customName = customName if customName else camera_name
-                        # Start recording and save the video with a timestamp and custom name
-                        screen.save_recording(
-                            save_path, isTimestamp=True, name=customName
-                        )
-                        self.recording_camera_list.append(camera_name)
-        else:
-            # If the save directory does not exist
-            print(f"Directory {save_path} does not exist!")
-
-    def stop_recording(self, screen_widgets):
-        """
-        Stops recording for all cameras that are currently recording.
-        """
-        # Iterate through each screen widget
-        for screen in screen_widgets:
-            camera_name = screen.get_camera_name()
-            # Check if it is 'Balckfly' camera and in the list of recording cameras
-            if screen.is_camera() and camera_name in self.recording_camera_list:
-                screen.stop_recording()  # Stop recording
-                # Remove the camera from the list of cameras that are currently recording
-                self.recording_camera_list.remove(camera_name)
+"""
+RecordingManager manages snapshot saving and video recording from multiple camera feeds, 
+supporting custom file naming and ensuring recordings are properly initiated and 
+stopped across active cameras.
+"""
+
+import logging
+import os
+
+# Set logger name
+logger = logging.getLogger(__name__)
+# Set the logging level for PyQt5.uic.uiparser/properties to WARNING, to ignore DEBUG messages
+logging.getLogger("PyQt5.uic.uiparser").setLevel(logging.WARNING)
+logging.getLogger("PyQt5.uic.properties").setLevel(logging.WARNING)
+
+
+class RecordingManager:
+    """RecordingManager manages snapshot saving and video recording"""
+
+    def __init__(self, model):
+        """Initialize recording manager"""
+        self.model = model
+        self.recording_camera_list = []
+
+    def save_last_image(self, save_path, screen_widgets):
+        """Saves the last captured image from all active camera feeds."""
+        # Initialize the list to keep track of cameras from which an image has been saved
+        snapshot_camera_list = []
+        # Get the directory path where the images will be saved
+        if os.path.exists(save_path):
+            print("\nSnapshot...")
+            for screen in screen_widgets:
+                # Save image only for 'Blackfly' camera
+                if screen.is_camera():
+                    # Use custom name of the camera if it has one, otherwise use the camera's serial number
+                    camera_name = screen.get_camera_name()
+                    if camera_name not in snapshot_camera_list:
+                        customName = screen.parent().title()
+                        customName = customName if customName else camera_name
+
+                        # Save the image with a timestamp and custom name
+                        screen.save_image(
+                            save_path, isTimestamp=True, name=customName
+                        )
+
+                        # Add the camera to the list of cameras from which an image has been saved
+                        snapshot_camera_list.append(camera_name)
+                else:
+                    logger.debug("save_last_image) camera not found")
+        else:
+            print(f"Directory {save_path} does not exist!")
+
+    def save_recording(self, save_path, screen_widgets):
+        """
+        Initiates recording for all active camera feeds.
+        Records video from all active camera feeds and saves them to a specified directory.
+        The directory path is taken from the label showing the current save directory.
+        """
+        # Initialize the list to keep track of cameras that are currently recording
+        self.recording_camera_list = []
+
+        if os.path.exists(save_path):
+            # Iterate through each screen widget
+            print("\nRecording... ")
+            for screen in screen_widgets:
+                # Check if the current screen is a camera
+                if screen.is_camera():  # If name is 'Blackfly"
+                    camera_name = (
+                        screen.get_camera_name()
+                    )  # Get the name of the camer
+                    # If this camera is not already in the list of recording cameras, then record
+                    if camera_name not in self.recording_camera_list:
+                        # Use custom name of the camera if it has one, otherwise use the camera's serial number
+                        customName = screen.parent().title()
+                        customName = customName if customName else camera_name
+                        # Start recording and save the video with a timestamp and custom name
+                        screen.save_recording(
+                            save_path, isTimestamp=True, name=customName
+                        )
+                        self.recording_camera_list.append(camera_name)
+        else:
+            # If the save directory does not exist
+            print(f"Directory {save_path} does not exist!")
+
+    def stop_recording(self, screen_widgets):
+        """
+        Stops recording for all cameras that are currently recording.
+        """
+        # Iterate through each screen widget
+        for screen in screen_widgets:
+            camera_name = screen.get_camera_name()
+            # Check if it is 'Balckfly' camera and in the list of recording cameras
+            if screen.is_camera() and camera_name in self.recording_camera_list:
+                screen.stop_recording()  # Stop recording
+                # Remove the camera from the list of cameras that are currently recording
+                self.recording_camera_list.remove(camera_name)
```

### Comparing `parallax_app-0.37.1/parallax/reticle_detect_manager.py` & `parallax_app-0.37.5/parallax/reticle_detect_manager.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,302 +1,310 @@
-"""
-Manages reticle detection in images through a worker thread, integrating line detection, 
-masking, coordinate analysis, and camera calibration. Uses PyQt's signals 
-for thread-safe operations and real-time processing feedback.
-"""
-
-import logging
-import time
-
-import cv2
-import numpy as np
-from PyQt5.QtCore import QObject, QThread, pyqtSignal
-
-from .calibration_camera import CalibrationCamera
-from .mask_generator import MaskGenerator
-from .reticle_detection import ReticleDetection
-from .reticle_detection_coords_interests import ReticleDetectCoordsInterest
-
-# Set logger name
-logger = logging.getLogger(__name__)
-logger.setLevel(logging.WARNING)
-# Set the logging level for PyQt5.uic.uiparser/properties to WARNING, to ignore DEBUG messages
-logging.getLogger("PyQt5.uic.uiparser").setLevel(logging.DEBUG)
-logging.getLogger("PyQt5.uic.properties").setLevel(logging.DEBUG)
-
-
-class ReticleDetectManager(QObject):
-    """Reticle detection class"""
-
-    name = "None"
-    frame_processed = pyqtSignal(object)
-    found_coords = pyqtSignal(np.ndarray, np.ndarray, np.ndarray, np.ndarray)
-
-    class Worker(QObject):
-        """Reticle detection Worker Thread"""
-
-        finished = pyqtSignal()
-        frame_processed = pyqtSignal(object)
-        found_coords = pyqtSignal(
-            np.ndarray, np.ndarray, np.ndarray, np.ndarray
-        )
-
-        def __init__(self, name):
-            """Initialize the worker"""
-            QObject.__init__(self)
-            self.name = name
-            self.running = False
-            self.is_detection_on = False
-            self.new = False
-            self.frame = None
-            self.IMG_SIZE_ORIGINAL = (4000, 3000)  # TODO
-            self.frame_success = None
-
-            self.mask_detect = MaskGenerator()
-            self.reticleDetector = ReticleDetection(
-                self.IMG_SIZE_ORIGINAL, self.mask_detect, self.name
-            )
-            self.coordsInterests = ReticleDetectCoordsInterest()
-            self.calibrationCamera = CalibrationCamera(self.name)
-
-        def update_frame(self, frame):
-            """Update the frame to be processed."""
-            self.frame = frame
-            # Deal with one frame at a time. This may cause the frame drop
-            if self.new is False:
-                self.new = True
-
-        def draw(self, frame, x_axis_coords, y_axis_coords):
-            """Draw the coordinates on the frame.
-
-            Args:
-                frame (numpy.ndarray): Input frame.
-                x_axis_coords (numpy.ndarray): X-axis coordinates.
-                y_axis_coords (numpy.ndarray): Y-axis coordinates.
-
-            Returns:
-                numpy.ndarray: Frame with coordinates drawn.
-            """
-            if x_axis_coords is None or y_axis_coords is None:
-                return frame
-            for pixel in x_axis_coords:
-                pt = tuple(pixel)
-                cv2.circle(frame, pt, 7, (255, 255, 0), -1)
-            for pixel in y_axis_coords:
-                pt = tuple(pixel)
-                cv2.circle(frame, pt, 7, (0, 255, 255), -1)
-            return frame
-
-        def draw_xyz(self, frame, origin, x, y, z):
-            """Draw the XYZ axes on the frame."""
-            frame = cv2.line(frame, origin, x, (0, 0, 255), 3)  # Blue line
-            frame = cv2.line(frame, origin, y, (0, 255, 0), 3)  # Green line
-            frame = cv2.line(frame, origin, z, (255, 0, 0), 3)  # Red line
-            return frame
-
-        def draw_calibration_info(self, frame, ret, mtx, dist):
-            """
-            Draw calibration information on the frame.
-
-            Parameters:
-            - frame: The image frame on which to draw.
-            - ret: Boolean indicating if calibration was successful.
-            - mtx: The camera matrix obtained from calibration.
-            - dist: The distortion coefficients obtained from calibration.
-            """
-
-            # Starting position for the text
-            offset_start = 50
-            line_height = 60
-
-            # Basic settings for the text
-            font = cv2.FONT_HERSHEY_SIMPLEX
-            font_scale = 1.5
-            font_color = (255, 255, 255)  # White color
-            line_type = 2
-
-            # Status text
-            status_text = f"Overall RMS re-projection error: {ret}"
-            cv2.putText(
-                frame,
-                status_text,
-                (10, offset_start),
-                font,
-                font_scale,
-                font_color,
-                line_type,
-            )
-
-            # Camera matrix text
-            mtx_lines = [
-                f"Camera Matrix:",
-                f"[{mtx[0][0]:.2f}, {mtx[0][1]:.2f}, {mtx[0][2]:.2f}]",
-                f"[{mtx[1][0]:.2f}, {mtx[1][1]:.2f}, {mtx[1][2]:.2f}]",
-                f"[{mtx[2][0]:.2f}, {mtx[2][1]:.2f}, {mtx[2][2]:.2f}]"
-            ]
-            # Draw each line of the camera matrix
-            for i, line in enumerate(mtx_lines):
-                cv2.putText(
-                    frame,
-                    line,
-                    (10, offset_start + line_height + i * line_height),
-                    font,
-                    font_scale,
-                    font_color,
-                    line_type,
-                )
-
-            # Distortion coefficients text
-            dist_text = f"Dist Coeffs: [{dist[0][0]:.4f}, {dist[0][1]:.4f}, \
-                {dist[0][2]:.4f}, {dist[0][3]:.4f} {dist[0][4]:.4f}]"
-            cv2.putText(
-                frame,
-                dist_text,
-                (10, offset_start + line_height * 5),
-                font,
-                font_scale,
-                font_color,
-                line_type,
-            )
-
-            return frame
-
-        def process(self, frame):
-            """Process the frame for reticle detection."""
-            # cv2.circle(frame, (2000,1500), 10, (255, 0, 0), -1)
-            ret, frame_, _, inliner_lines_pixels = (
-                self.reticleDetector.get_coords(frame)
-            )
-            if ret:
-                ret, x_axis_coords, y_axis_coords = (
-                    self.coordsInterests.get_coords_interest(
-                        inliner_lines_pixels
-                    )
-                )
-            if ret:
-                # TODO
-                # ret, mtx, dist = self.calibrationCamera.get_predefined_intrinsic(x_axis_coords, y_axis_coords)
-                # if not ret:
-                ret, mtx, dist = self.calibrationCamera.calibrate_camera(
-                    x_axis_coords, y_axis_coords
-                )
-                if ret:
-                    # Draw
-                    self.found_coords.emit(
-                        x_axis_coords, y_axis_coords, mtx, dist
-                    )
-                    origin, x, y, z = self.calibrationCamera.get_origin_xyz()
-                    frame = self.draw_xyz(frame, origin, x, y, z)
-                    frame = self.draw(frame, x_axis_coords, y_axis_coords)
-                    frame = self.draw_calibration_info(frame, ret, mtx, dist)
-                self.frame_success = frame
-            if self.frame_success is None:
-                logger.debug(f"{ self.name} reticle detection fail ")
-                return frame
-            else:
-                logger.debug(f"{ self.name} reticle detection success ")
-                return self.frame_success
-
-        def stop_running(self):
-            """Stop the worker from running."""
-            self.running = False
-
-        def start_running(self):
-            """Start the worker running."""
-            self.running = True
-
-        def start_detection(self):
-            """Start the reticle detection."""
-            self.is_detection_on = True
-
-        def stop_detection(self):
-            """Stop the reticle detection."""
-            self.is_detection_on = False
-
-        def run(self):
-            """Run the worker thread."""
-            while self.running:
-                if self.new:
-                    self.frame = self.process(self.frame)
-                    self.frame_processed.emit(self.frame)
-                self.new = False
-                time.sleep(0.001)
-            self.finished.emit()
-            logger.debug(f"thread finished {self.name}")
-
-        def set_name(self, name):
-            """Set name as camera serial number."""
-            self.name = name
-
-    def __init__(self, camera_name):
-        """Initialize the reticle detection manager."""
-        logger.debug("Init reticle detect manager")
-        super().__init__()
-        self.worker = None
-        self.name = camera_name
-        self.thread = None
-
-    def init_thread(self):
-        """Initialize the worker thread."""
-        if self.thread is not None:
-            self.clean()  # Clean up existing thread and worker before reinitializing
-        self.thread = QThread()
-        self.worker = self.Worker(self.name)
-        self.worker.moveToThread(self.thread)
-
-        self.thread.started.connect(self.worker.run)
-        self.thread.finished.connect(self.thread.deleteLater)
-        self.thread.destroyed.connect(self.onThreadDestroyed)
-        self.threadDeleted = False
-
-        self.worker.frame_processed.connect(self.frame_processed)
-        self.worker.found_coords.connect(self.found_coords)
-        self.worker.finished.connect(self.thread.quit)
-        self.worker.finished.connect(self.worker.deleteLater)
-        logger.debug(f"init camera name: {self.name}")
-
-    def process(self, frame):
-        """Process the frame using the worker.
-
-        Args:
-            frame (numpy.ndarray): Input frame.
-        """
-        if self.worker is not None:
-            self.worker.update_frame(frame)
-
-    def start(self):
-        """Start the reticle detection manager."""
-        self.init_thread()  # Reinitialize and start the worker and thread
-        self.worker.start_running()
-        self.thread.start()
-        logger.debug(f"thread started {self.name}")
-
-    def stop(self):
-        """Stop the reticle detection manager."""
-        if self.worker is not None:
-            self.worker.stop_running()
-
-    def set_name(self, camera_name):
-        """Set camera name."""
-        self.name = camera_name
-        if self.worker is not None:
-            self.worker.set_name(self.name)
-        logger.debug(f"camera name: {self.name}")
-
-    def clean(self):
-        """Safely clean up the reticle detection manager."""
-        logger.debug("Cleaning the thread")
-        if self.worker is not None:
-            self.worker.stop_running()  # Signal the worker to stop
-        if not self.threadDeleted and self.thread.isRunning():
-            self.thread.quit()  # Ask the thread to quit
-            self.thread.wait()  # Wait for the thread to finish
-        self.thread = None  # Clear the reference to the thread
-        self.worker = None  # Clear the reference to the worker
-
-    def onThreadDestroyed(self):
-        """Flag if thread is deleted"""
-        self.threadDeleted = True
-
-    def __del__(self):
-        """Destructor for the reticle detection manager."""
+"""
+Manages reticle detection in images through a worker thread, integrating line detection, 
+masking, coordinate analysis, and camera calibration. Uses PyQt's signals 
+for thread-safe operations and real-time processing feedback.
+"""
+
+import logging
+import time
+
+import cv2
+import numpy as np
+from PyQt5.QtCore import QObject, QThread, pyqtSignal
+
+from .calibration_camera import CalibrationCamera
+from .mask_generator import MaskGenerator
+from .reticle_detection import ReticleDetection
+from .reticle_detection_coords_interests import ReticleDetectCoordsInterest
+
+# Set logger name
+logger = logging.getLogger(__name__)
+logger.setLevel(logging.DEBUG)
+# Set the logging level for PyQt5.uic.uiparser/properties to WARNING, to ignore DEBUG messages
+logging.getLogger("PyQt5.uic.uiparser").setLevel(logging.DEBUG)
+logging.getLogger("PyQt5.uic.properties").setLevel(logging.DEBUG)
+
+
+class ReticleDetectManager(QObject):
+    """Reticle detection class"""
+
+    name = "None"
+    frame_processed = pyqtSignal(object)
+    found_coords = pyqtSignal(np.ndarray, np.ndarray, np.ndarray, np.ndarray)
+
+    class Worker(QObject):
+        """Reticle detection Worker Thread"""
+
+        finished = pyqtSignal()
+        frame_processed = pyqtSignal(object)
+        found_coords = pyqtSignal(
+            np.ndarray, np.ndarray, np.ndarray, np.ndarray
+        )
+
+        def __init__(self, name):
+            """Initialize the worker"""
+            QObject.__init__(self)
+            self.name = name
+            self.running = False
+            self.is_detection_on = False
+            self.new = False
+            self.frame = None
+            self.IMG_SIZE_ORIGINAL = (4000, 3000)  # TODO
+            self.frame_success = None
+
+            self.mask_detect = MaskGenerator(initial_detect = True)
+            self.reticleDetector = ReticleDetection(
+                self.IMG_SIZE_ORIGINAL, self.mask_detect, self.name
+            )
+            self.coordsInterests = ReticleDetectCoordsInterest()
+            self.calibrationCamera = CalibrationCamera(self.name)
+
+        def update_frame(self, frame):
+            """Update the frame to be processed."""
+            self.frame = frame
+            # Deal with one frame at a time. This may cause the frame drop
+            if self.new is False:
+                self.new = True
+
+        def draw(self, frame, x_axis_coords, y_axis_coords):
+            """Draw the coordinates on the frame.
+
+            Args:
+                frame (numpy.ndarray): Input frame.
+                x_axis_coords (numpy.ndarray): X-axis coordinates.
+                y_axis_coords (numpy.ndarray): Y-axis coordinates.
+
+            Returns:
+                numpy.ndarray: Frame with coordinates drawn.
+            """
+            if x_axis_coords is None or y_axis_coords is None:
+                return frame
+            for pixel in x_axis_coords:
+                pt = tuple(pixel)
+                cv2.circle(frame, pt, 7, (255, 255, 0), -1)
+            for pixel in y_axis_coords:
+                pt = tuple(pixel)
+                cv2.circle(frame, pt, 7, (0, 255, 255), -1)
+            return frame
+
+        def draw_xyz(self, frame, origin, x, y, z):
+            """Draw the XYZ axes on the frame."""
+            frame = cv2.line(frame, origin, x, (0, 0, 255), 3)  # Blue line
+            frame = cv2.line(frame, origin, y, (0, 255, 0), 3)  # Green line
+            frame = cv2.line(frame, origin, z, (255, 0, 0), 3)  # Red line
+            return frame
+
+        def draw_calibration_info(self, frame, ret, mtx, dist):
+            """
+            Draw calibration information on the frame.
+
+            Parameters:
+            - frame: The image frame on which to draw.
+            - ret: Boolean indicating if calibration was successful.
+            - mtx: The camera matrix obtained from calibration.
+            - dist: The distortion coefficients obtained from calibration.
+            """
+
+            # Starting position for the text
+            offset_start = 50
+            line_height = 60
+
+            # Basic settings for the text
+            font = cv2.FONT_HERSHEY_SIMPLEX
+            font_scale = 1.5
+            font_color = (255, 255, 255)  # White color
+            line_type = 2
+
+            # Status text
+            status_text = f"Overall RMS re-projection error: {ret}"
+            cv2.putText(
+                frame,
+                status_text,
+                (10, offset_start),
+                font,
+                font_scale,
+                font_color,
+                line_type,
+            )
+
+            # Camera matrix text
+            mtx_lines = [
+                f"Camera Matrix:",
+                f"[{mtx[0][0]:.2f}, {mtx[0][1]:.2f}, {mtx[0][2]:.2f}]",
+                f"[{mtx[1][0]:.2f}, {mtx[1][1]:.2f}, {mtx[1][2]:.2f}]",
+                f"[{mtx[2][0]:.2f}, {mtx[2][1]:.2f}, {mtx[2][2]:.2f}]"
+            ]
+            # Draw each line of the camera matrix
+            for i, line in enumerate(mtx_lines):
+                cv2.putText(
+                    frame,
+                    line,
+                    (10, offset_start + line_height + i * line_height),
+                    font,
+                    font_scale,
+                    font_color,
+                    line_type,
+                )
+
+            # Distortion coefficients text
+            dist_text = f"Dist Coeffs: [{dist[0][0]:.4f}, {dist[0][1]:.4f}, \
+                {dist[0][2]:.4f}, {dist[0][3]:.4f} {dist[0][4]:.4f}]"
+            cv2.putText(
+                frame,
+                dist_text,
+                (10, offset_start + line_height * 5),
+                font,
+                font_scale,
+                font_color,
+                line_type,
+            )
+
+            return frame
+
+        def process(self, frame):
+            """Process the frame for reticle detection."""
+            # cv2.circle(frame, (2000,1500), 10, (255, 0, 0), -1)
+            ret, frame_, _, inliner_lines_pixels = (
+                self.reticleDetector.get_coords(frame)
+            )
+            if not ret:
+                logger.debug(f"{ self.name} get_coords fails ")
+            else:
+                ret, x_axis_coords, y_axis_coords = (
+                    self.coordsInterests.get_coords_interest(
+                        inliner_lines_pixels
+                    )
+                )
+
+            if not ret:
+                logger.debug(f"{ self.name} get_coords_interest fails ")
+            else:
+                # TODO
+                # ret, mtx, dist = self.calibrationCamera.get_predefined_intrinsic(x_axis_coords, y_axis_coords)
+                # if not ret:
+                ret, mtx, dist = self.calibrationCamera.calibrate_camera(
+                    x_axis_coords, y_axis_coords
+                )
+                if not ret:
+                    logger.debug(f"{ self.name} calibrate_camera fails ")
+                else:
+                    # Draw
+                    self.found_coords.emit(
+                        x_axis_coords, y_axis_coords, mtx, dist
+                    )
+                    origin, x, y, z = self.calibrationCamera.get_origin_xyz()
+                    frame = self.draw_xyz(frame, origin, x, y, z)
+                    frame = self.draw(frame, x_axis_coords, y_axis_coords)
+                    frame = self.draw_calibration_info(frame, ret, mtx, dist)
+                self.frame_success = frame
+            
+            if self.frame_success is None:
+                logger.debug(f"{ self.name} reticle detection fail ")
+                return frame
+            else:
+                logger.debug(f"{ self.name} reticle detection success \n")
+                return self.frame_success
+
+        def stop_running(self):
+            """Stop the worker from running."""
+            self.running = False
+
+        def start_running(self):
+            """Start the worker running."""
+            self.running = True
+
+        def start_detection(self):
+            """Start the reticle detection."""
+            self.is_detection_on = True
+
+        def stop_detection(self):
+            """Stop the reticle detection."""
+            self.is_detection_on = False
+
+        def run(self):
+            """Run the worker thread."""
+            while self.running:
+                if self.new:
+                    self.frame = self.process(self.frame)
+                    self.frame_processed.emit(self.frame)
+                self.new = False
+                time.sleep(0.001)
+            self.finished.emit()
+            logger.debug(f"thread finished {self.name}")
+
+        def set_name(self, name):
+            """Set name as camera serial number."""
+            self.name = name
+
+    def __init__(self, camera_name):
+        """Initialize the reticle detection manager."""
+        logger.debug("Init reticle detect manager")
+        super().__init__()
+        self.worker = None
+        self.name = camera_name
+        self.thread = None
+
+    def init_thread(self):
+        """Initialize the worker thread."""
+        if self.thread is not None:
+            self.clean()  # Clean up existing thread and worker before reinitializing
+        self.thread = QThread()
+        self.worker = self.Worker(self.name)
+        self.worker.moveToThread(self.thread)
+
+        self.thread.started.connect(self.worker.run)
+        self.thread.finished.connect(self.thread.deleteLater)
+        self.thread.destroyed.connect(self.onThreadDestroyed)
+        self.threadDeleted = False
+
+        self.worker.frame_processed.connect(self.frame_processed)
+        self.worker.found_coords.connect(self.found_coords)
+        self.worker.finished.connect(self.thread.quit)
+        self.worker.finished.connect(self.worker.deleteLater)
+        logger.debug(f"init camera name: {self.name}")
+
+    def process(self, frame):
+        """Process the frame using the worker.
+
+        Args:
+            frame (numpy.ndarray): Input frame.
+        """
+        if self.worker is not None:
+            self.worker.update_frame(frame)
+
+    def start(self):
+        """Start the reticle detection manager."""
+        self.init_thread()  # Reinitialize and start the worker and thread
+        self.worker.start_running()
+        self.thread.start()
+        logger.debug(f"thread started {self.name}")
+
+    def stop(self):
+        """Stop the reticle detection manager."""
+        if self.worker is not None:
+            self.worker.stop_running()
+
+    def set_name(self, camera_name):
+        """Set camera name."""
+        self.name = camera_name
+        if self.worker is not None:
+            self.worker.set_name(self.name)
+        logger.debug(f"camera name: {self.name}")
+
+    def clean(self):
+        """Safely clean up the reticle detection manager."""
+        logger.debug("Cleaning the thread")
+        if self.worker is not None:
+            self.worker.stop_running()  # Signal the worker to stop
+        if not self.threadDeleted and self.thread.isRunning():
+            self.thread.quit()  # Ask the thread to quit
+            self.thread.wait()  # Wait for the thread to finish
+        self.thread = None  # Clear the reference to the thread
+        self.worker = None  # Clear the reference to the worker
+
+    def onThreadDestroyed(self):
+        """Flag if thread is deleted"""
+        self.threadDeleted = True
+
+    def __del__(self):
+        """Destructor for the reticle detection manager."""
         self.clean()
```

### Comparing `parallax_app-0.37.1/parallax/reticle_detection.py` & `parallax_app-0.37.5/parallax/reticle_detection.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,585 +1,619 @@
-""" ReticleDetection for identifying reticle coordinates in microscopy images
-
-Process: 
-- preprocessing, masking, and morphological operations
-- Utilizes adaptive thresholding, Gaussian blurring, and RANSAC for line detection, line drawing, and pixel refinement
-- Supports line intersection and missing point estimation
-"""
-
-import logging
-import warnings
-
-import cv2
-import numpy as np
-from scipy.stats import linregress
-from skimage.measure import LineModelND, ransac
-
-# Set logger name
-logger = logging.getLogger(__name__)
-# Set the logging level for PyQt5.uic.uiparser/properties to WARNING, to ignore DEBUG messages
-logger.setLevel(logging.WARNING)
-logging.getLogger("PyQt5.uic.uiparser").setLevel(logging.WARNING)
-logging.getLogger("PyQt5.uic.properties").setLevel(logging.WARNING)
-
-
-class ReticleDetection:
-    """Class for detecting reticle lines and coordinates."""
-
-    def __init__(self, IMG_SIZE, reticle_frame_detector, camera_name):
-        """Initialize Reticle Detection object"""
-        self.image_size = IMG_SIZE
-        self.reticle_frame_detector = reticle_frame_detector
-        self.mask = None
-        self.name = camera_name
-
-    def _preprocess_image(self, img):
-        """Convert image to grayscale, blur, and resize."""
-        # Check if image is already grayscale
-        if img.ndim == 3 and img.shape[2] == 3:  # Check if image has 3 channels
-            bg = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)
-        else:
-            bg = img
-
-        bg = cv2.GaussianBlur(bg, (11, 11), 0)
-        return bg
-
-    def _apply_mask(self, img):
-        """Apply the mask to the image."""
-        self.mask = self.reticle_frame_detector.process(img)
-        return cv2.bitwise_and(img, img, mask=self.mask)
-
-    def _draw_reticle_lines(self, img, pixels_in_lines):
-        """Draw lines on the reticle points based on detected pixels."""
-        reticle_points = np.zeros_like(img)
-        width, height = self.image_size
-
-        for pixels_in_line in pixels_in_lines:
-            self._draw_line(reticle_points, pixels_in_line, width, height)
-
-        # cv2.imwrite("debug/reticle_zone.jpg", reticle_points)
-        return reticle_points
-
-    def _draw_line(self, reticle_points, pixels_in_line, width, height):
-        """Draw a single line across the reticle points."""
-        x1, y1 = pixels_in_line[0]
-        x2, y2 = pixels_in_line[-1]
-
-        if x2 - x1 == 0:  # Prevent division by zero
-            m = np.inf
-            x_vert = x1  # Vertical line x-coordinate
-        else:
-            m = (y2 - y1) / (x2 - x1)
-            b = y1 - m * x1
-
-        if m == np.inf:
-            cv2.line(
-                reticle_points,
-                (x_vert, 0),
-                (x_vert, height),
-                (255, 255, 255),
-                35,
-            )
-        else:
-            y_start = int(m * 0 + b)
-            y_end = int(m * width + b)
-            cv2.line(
-                reticle_points,
-                (0, y_start),
-                (width, y_end),
-                (255, 255, 255),
-                35,
-            )
-
-    def _ransac_detect_lines(self, img):
-        """Detect lines using RANSAC algorithm.
-
-        Args:
-            img (numpy.ndarray): Input image.
-
-        Returns:
-            tuple: (ret, inlier_lines, inlier_pixels)
-                - ret (bool): True if two lines are detected, False otherwise.
-                - inlier_lines (list): List of detected line models.
-                - inlier_pixels (list): List of inlier pixel coordinates for each line.
-        """
-        inlier_lines = []
-        inlier_pixels = []
-
-        if img is None:
-            return False, inlier_lines, inlier_pixels
-
-        # Draw
-        if len(img.shape) == 2:  # Grayscale image
-            img_color = cv2.cvtColor(img, cv2.COLOR_GRAY2BGR)
-        else:  # Color image
-            img_color = img.copy()
-
-        contours, _ = cv2.findContours(
-            img, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE
-        )
-        centroids = np.array(self._get_centroid(contours))
-        if len(centroids) < 10:
-            logger.debug("points for rasac line detection are less than 10")
-            return False, inlier_lines, inlier_pixels
-
-        max_trials = 7000
-        residual_threshold = 2
-        counter = 50
-        while len(inlier_lines) < 2 and counter > 0:
-            with warnings.catch_warnings():
-                warnings.simplefilter("ignore", RuntimeWarning)
-                model_robust, inliers = ransac(
-                    centroids,
-                    LineModelND,
-                    min_samples=9,
-                    residual_threshold=residual_threshold,
-                    max_trials=max_trials,
-                )
-            inlier_points = centroids[inliers]
-            if len(inlier_points) >= 20:
-                logger.debug(f"residual_threshold: {residual_threshold}")
-                inlier_pixels.append(inlier_points)
-                inlier_lines.append(model_robust)
-                centroids = centroids[~inliers]
-                max_trials = 7000
-                residual_threshold = 2
-                counter = 50  # Reset counter
-            else:
-                max_trials += 2000  # if not found, run RASAC again
-                counter -= 1
-                if residual_threshold <= 15:
-                    residual_threshold += 1
-                continue
-
-        # Draw the centroids
-        """
-        for points in inlier_pixels:
-            for point in points:
-                cv2.circle(img_color, (int(point[0]), int(point[1])), 1, (0, 0, 255), -1)  # Draw green circles
-        cv2.imwrite("debug/centroid.jpg", img_color)
-        """
-
-        return len(inlier_lines) == 2, inlier_lines, inlier_pixels
-
-    def _fit_line(self, pixels):
-        """Fit a line to the given pixels.
-
-        Args:
-            pixels (numpy.ndarray): Pixel coordinates.
-
-        Returns:
-            tuple: (slope, intercept) of the fitted line.
-        """
-        x_coords, y_coords = zip(*pixels)
-        slope, intercept, _, _, _ = linregress(x_coords, y_coords)
-        return slope, intercept
-
-    def _find_intersection(self, line1, line2):
-        """Find the intersection point of two lines.
-
-        Args:
-            line1 (tuple): (slope, intercept) of the first line.
-            line2 (tuple): (slope, intercept) of the second line.
-
-        Returns:
-            tuple or None: (x, y) coordinates of the intersection point if it exists, None otherwise.
-        """
-        slope1, intercept1 = line1
-        slope2, intercept2 = line2
-
-        if slope1 == slope2:
-            return None  # No intersection (parallel lines)
-
-        x_intersect = (intercept2 - intercept1) / (slope1 - slope2)
-        y_intersect = slope1 * x_intersect + intercept1
-        return int(round(x_intersect)), int(round(y_intersect))
-
-    def _get_center_coords_index(self, center, coords):
-        """Get the index of the center coordinates in the given coordinates.
-
-        Args:
-            center (tuple): Center coordinates (x, y).
-            coords (numpy.ndarray): Array of coordinates.
-
-        Returns:
-            int or None: Index of the center coordinates in the coords array, None if not found.
-        """
-        x_center, y_center = center
-        for i in range(-4, 5):
-            for j in range(-4, 5):
-                test_center = np.array([x_center + i, y_center + j])
-                result = np.where((coords == test_center).all(axis=1))
-                if len(result[0]) > 0:
-                    return result[0][0]
-        return None
-
-    def _get_pixels_interest(self, center, coords, dist=10):
-        """Get the pixels of interest around the center coordinates.
-
-        Args:
-            center (tuple): Center coordinates (x, y).
-            coords (numpy.ndarray): Array of coordinates.
-            dist (int): Distance from the center to select pixels of interest. Defaults to 10.
-
-        Returns:
-            numpy.ndarray or None: Selected pixels of interest, None if center is not found.
-        """
-        center_index = self._get_center_coords_index(center, coords)
-        if center_index is None:
-            return
-
-        start_index = max(center_index - dist, 0)
-        end_index = min(center_index + dist + 1, len(coords))
-        return coords[start_index:end_index]
-
-    def _find_reticle_coords(self, pixels_in_lines):
-        """Find the reticle coordinates from the pixels in lines.
-        Args:
-            pixels_in_lines (list): List of pixel coordinates for each line.
-        Returns:
-            list: List of pixel coordinates of interest for each line.
-        """
-        if len(pixels_in_lines) != 2:
-            raise ValueError("Function requires exactly two lines")
-
-        line1 = self._fit_line(pixels_in_lines[0])
-        line2 = self._fit_line(pixels_in_lines[1])
-        center_point = self._find_intersection(line1, line2)
-
-        coords_interest = []
-        for pixels_in_line in pixels_in_lines:
-            coords = self._get_pixels_interest(center_point, pixels_in_line)
-            coords_interest.append(coords)
-
-        return coords_interest
-
-    def _eroding(self, img):
-        """Erode the image until the desired contour conditions are met.
-
-        Args:
-            img (numpy.ndarray): Input image.
-
-        Returns:
-            numpy.ndarray: Eroded image.
-        """
-        kernel_ellipse_3 = cv2.getStructuringElement(cv2.MORPH_ELLIPSE, (3, 3))
-        counter = 100
-        while counter > 0:
-            contours, _ = cv2.findContours(
-                img, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE
-            )
-            if not contours:
-                break
-
-            largest_contour = max(contours, key=cv2.contourArea)
-            largest_contour_area = cv2.contourArea(largest_contour)
-            if 50 < len(contours) < 300 and largest_contour_area < 30 * 30:
-                break
-            img = cv2.erode(img, kernel_ellipse_3, iterations=1)
-            img = cv2.morphologyEx(img, cv2.MORPH_OPEN, kernel_ellipse_3)
-            counter -= 1
-        return img
-
-    def _get_centroid(self, contours):
-        """Get the centroid of each contour.
-
-        Args:
-            contours (list): List of contours.
-
-        Returns:
-            list: List of centroid coordinates for each contour.
-        """
-        centroids = []
-        for contour in contours:
-            M = cv2.moments(contour)
-            if M["m00"] != 0:
-                cX = int(M["m10"] / M["m00"])
-                cY = int(M["m01"] / M["m00"])
-                centroids.append([cX, cY])
-        return centroids
-
-    def __del__(self):
-        """Delete the instance"""
-        # print("ReticleDetection Object destroyed")
-        pass
-
-    def _sort_points(self, points):
-        """Sort the points based on the dimension with greater median distance.
-
-        Args:
-            points (numpy.ndarray): Array of points.
-
-        Returns:
-            numpy.ndarray: Sorted points.
-        """
-        # Calculate differences between consecutive points
-        diffs = np.diff(points, axis=0)
-        x_diffs = diffs[:, 0]
-        y_diffs = diffs[:, 1]
-
-        # Compute median distances for x and y
-        median_x_diff = np.median(np.abs(x_diffs))
-        median_y_diff = np.median(np.abs(y_diffs))
-
-        # Determine which dimension has greater median distance
-        if median_x_diff > median_y_diff:
-            # Sort points based on x component if x has greater median distance
-            sorted_points = points[np.argsort(points[:, 0])]
-        else:
-            # Sort points based on y component if y has greater median distance
-            sorted_points = points[np.argsort(-points[:, 1])]
-
-        return sorted_points
-
-    def _estimate_missing_points(self, points, threshold_factor=1.5):
-        """Estimate missing points in the given points based on the average distance.
-
-        Args:
-            points (numpy.ndarray): Array of points.
-            threshold_factor (float): Factor to determine the threshold for large gaps. Defaults to 1.5.
-
-        Returns:
-            numpy.ndarray: Array of estimated missing points.
-        """
-        points = self._sort_points(points)
-
-        # Calculate the Euclidean distances between consecutive points
-        distances = np.linalg.norm(np.diff(points, axis=0), axis=1)
-
-        # Estimate the average distance
-        average_distance = np.median(distances)
-
-        # Identify large gaps
-        threshold = threshold_factor * average_distance
-        large_gaps = np.where(distances > threshold)[0]
-
-        # Estimate missing points in the large gaps
-        missing_points = []
-        for gap_index in large_gaps:
-            start_point = points[gap_index]
-            end_point = points[gap_index + 1]
-            num_missing = (
-                int(round(distances[gap_index] / average_distance)) - 1
-            )
-            for i in range(1, num_missing + 1):
-                missing_point = start_point + (end_point - start_point) * (
-                    i / (num_missing + 1)
-                )
-                missing_points.append(np.round(missing_point))
-
-        return np.array(missing_points)
-
-    def _add_missing_pixels(self, bg, lines, line_pixels):
-        """Add missing pixels to the line pixels based on the estimated missing points.
-
-        Args:
-            bg (numpy.ndarray): Background image.
-            lines (list): List of line models.
-            line_pixels (list): List of pixel coordinates for each line.
-
-        Returns:
-            tuple: (bg, refined_pixels)
-                - bg (numpy.ndarray): Background image with missing points drawn.
-                - refined_pixels (list): List of refined pixel coordinates for each line.
-        """
-        refined_pixels = []
-
-        for line_model, pixels in zip(lines, line_pixels):
-            pixels_array = np.array(pixels)
-            missing_points = self._estimate_missing_points(pixels_array)
-
-            if missing_points.ndim == 1 and missing_points.size > 0:
-                missing_points = missing_points.reshape(-1, 2)  # Reshape to 2D if it's flat but not empty
-            elif missing_points.size == 0:
-                missing_points_adjusted = np.array([])  # Handle empty case
-            else:
-                missing_points_adjusted = np.array(
-                    [
-                        (x, line_model.predict_y(np.array([x]))[0])
-                        for x in missing_points[:, 0]
-                    ]
-                )
-
-            # Combine original and adjusted missing points
-            if missing_points_adjusted.size > 0:
-                full_line_pixels = np.vstack(
-                    (pixels_array, missing_points_adjusted)
-                )
-            else:
-                full_line_pixels = pixels_array
-
-            # Sort pixels
-            # Calculate the ranges for x and y coordinates
-            minX, maxX = (
-                full_line_pixels[:, 0].min(),
-                full_line_pixels[:, 0].max(),
-            )
-            minY, maxY = (
-                full_line_pixels[:, 1].min(),
-                full_line_pixels[:, 1].max(),
-            )
-            # Determine the sorting order based on the comparison of ranges
-            if maxX - minX > maxY - minY:
-                # If range of x is greater, sort by x-coordinate
-                full_line_pixels = full_line_pixels[
-                    full_line_pixels[:, 0].argsort()
-                ]
-            else:
-                # Otherwise, sort by y-coordinate
-                full_line_pixels = full_line_pixels[
-                    full_line_pixels[:, 1].argsort()
-                ]
-
-            full_line_pixels = np.around(full_line_pixels).astype(int)
-            refined_pixels.append(full_line_pixels)
-
-            if len(missing_points_adjusted) > 0:
-                for pixel in missing_points_adjusted:
-                    pt = tuple(int(coordinate) for coordinate in pixel)
-                    cv2.circle(bg, pt, 2, (0, 255, 255), -1)
-
-        return bg, refined_pixels
-
-    def _refine_pixels(self, bg, lines, line_pixels):
-        """Refine the pixel coordinates fitting into lines based on the line models.
-
-        Args:
-            bg (numpy.ndarray): Background image.
-            lines (list): List of line models.
-            line_pixels (list): List of pixel coordinates for each line.
-
-        Returns:
-            tuple: (bg, lines, refined_pixels)
-                - bg (numpy.ndarray): Background image with refined pixels drawn.
-                - lines (list): List of line models.
-                - refined_pixels (list): List of refined pixel coordinates for each line.
-        """
-        refined_pixels = []
-
-        for line_model, pixels in zip(lines, line_pixels):
-            origin, direction = line_model.params[0], line_model.params[1]
-            # Extend the line
-            point1 = tuple((origin + -2000 * direction).astype(int))  
-            point2 = tuple((origin + 2000 * direction).astype(int))
-            cv2.line(bg, point1, point2, (0, 0, 255), 1)
-            pixels = np.array(pixels)
-            to_pixels = pixels - origin
-            proj_lengths = (
-                np.dot(to_pixels, direction) / np.linalg.norm(direction) ** 2
-            )
-            proj_points = np.outer(proj_lengths, direction) + origin
-
-            proj_points = np.round(proj_points).astype(int)
-            refined_pixels.append(proj_points)
-
-        # Draw
-        for refined_pixels_per_line in refined_pixels:
-            for pixel in refined_pixels_per_line:
-                pt = tuple(pixel)
-                cv2.circle(bg, pt, 3, (255, 0, 0), -1)
-        # cv2.imwrite("debug/refined_pixels.jpg", bg)
-        return bg, lines, refined_pixels
-
-    def get_reticle_zone(self, img):
-        """Get the reticle zone from the image.
-
-        Args:
-            img (numpy.ndarray): Input image.
-
-        Returns:
-            numpy.ndarray or None: Reticle zone image if reticle exists, None otherwise.
-        """
-        bg = self._preprocess_image(img)
-        bg = cv2.resize(bg, self.image_size)
-        masked = self._apply_mask(bg)
-        if self.reticle_frame_detector.is_reticle_exist:
-            ret, bg, _, pixels_in_lines = self.coords_detect_morph(bg)
-            return self._draw_reticle_lines(bg, pixels_in_lines)
-        else:
-            return None
-
-    def coords_detect_morph(self, img):
-        """
-        Applies morphological operations and adaptive thresholding
-        to detect coordinates in an image.
-        """
-        img_color = cv2.cvtColor(img, cv2.COLOR_GRAY2BGR)
-        if img.shape == (3000, 4000):
-            img = cv2.adaptiveThreshold(
-                img,
-                255,
-                cv2.ADAPTIVE_THRESH_GAUSSIAN_C,
-                cv2.THRESH_BINARY,
-                13,
-                2,
-            )
-        else:
-            img = cv2.adaptiveThreshold(
-                img,
-                255,
-                cv2.ADAPTIVE_THRESH_GAUSSIAN_C,
-                cv2.THRESH_BINARY,
-                11,
-                3,
-            )
-        img = cv2.medianBlur(img, 5)
-        img = cv2.bitwise_not(img, mask=self.mask)
-        kernel_ellipse_5 = cv2.getStructuringElement(cv2.MORPH_ELLIPSE, (5, 5))
-        kernel_ellipse_3 = cv2.getStructuringElement(cv2.MORPH_ELLIPSE, (3, 3))
-        img = cv2.morphologyEx(img, cv2.MORPH_CLOSE, kernel_ellipse_5)
-
-        img = self._eroding(img)
-        # cv2.imwrite("debug/after_eroding.jpg", img)
-        ret, inliner_lines, inliner_lines_pixels = self._ransac_detect_lines(img)
-        logger.debug(f"n of inliner lines: {len(inliner_lines_pixels)}")
-
-        # Draw
-        for inliner_lines_pixel in inliner_lines_pixels:
-            for pixel in inliner_lines_pixel:
-                pt = tuple(pixel)
-                cv2.circle(img_color, pt, 1, (0, 255, 0), -1)
-        # cv2.imwrite("debug/inliner_pixels.jpg", img_color)
-
-        return ret, img, inliner_lines, inliner_lines_pixels
-
-    def get_coords(self, img):
-        """Detect coordinates using morphological operations.
-
-        Args:
-            img (numpy.ndarray): Input image.
-
-        Returns:
-            tuple: (ret, img, inliner_lines, inliner_lines_pixels)
-                - ret (bool): True if coordinates are detected, False otherwise.
-                - img (numpy.ndarray): Processed image.
-                - inliner_lines (list): List of inlier line models.
-                - inliner_lines_pixels (list): List of inlier pixel coordinates for each line.
-        """
-        bg = self._preprocess_image(img)
-        masked = self._apply_mask(bg)
-
-        # if self.mask is not None:
-        #    cv2.imwrite("debug/mask.jpg", self.mask)
-
-        if self.reticle_frame_detector.is_reticle_exist:
-            ret, bg, inliner_lines, pixels_in_lines = self.coords_detect_morph(bg)
-            logger.debug(f"{self.name} nLines: {len(pixels_in_lines)}")
-            if ret:
-                bg, inliner_lines, pixels_in_lines = self._refine_pixels(bg, inliner_lines, pixels_in_lines)
-                logger.debug(f"{self.name} detect: {len(pixels_in_lines[0])}, {len(pixels_in_lines[1])}" )
-                bg, pixels_in_lines = self._add_missing_pixels(bg, inliner_lines, pixels_in_lines)
-                logger.debug(f"{self.name} interpolate: {len(pixels_in_lines[0])} {len(pixels_in_lines[1])}")
-                # cv2.imwrite("debug/added_missing_points.jpg", bg)
-            return ret, bg, inliner_lines, pixels_in_lines
-
-        return False, bg, None, None
-
-    """
-    def is_distance_tip_reticle_threshold(self, probe, reticle, thresh=10):
-        tip_x, tip_y = probe["tip_coords"]
-        dist_transform = cv2.distanceTransform(reticle, cv2.DIST_L2, cv2.DIST_MASK_PRECISE)
-        # Get the distance at the tip location
-        distance_at_tip = dist_transform[int(tip_y), int(tip_x)]
-        print("distance_at_tip: ", distance_at_tip)
-        return distance_at_tip > thresh
-    """
+""" ReticleDetection for identifying reticle coordinates in microscopy images
+
+Process: 
+- preprocessing, masking, and morphological operations
+- Utilizes adaptive thresholding, Gaussian blurring, and RANSAC for line detection, line drawing, and pixel refinement
+- Supports line intersection and missing point estimation
+"""
+
+import logging
+import warnings
+
+import cv2
+import numpy as np
+from scipy.stats import linregress
+from skimage.measure import LineModelND, ransac
+
+# Set logger name
+logger = logging.getLogger(__name__)
+# Set the logging level for PyQt5.uic.uiparser/properties to WARNING, to ignore DEBUG messages
+logger.setLevel(logging.WARNING)
+logging.getLogger("PyQt5.uic.uiparser").setLevel(logging.WARNING)
+logging.getLogger("PyQt5.uic.properties").setLevel(logging.WARNING)
+
+
+class ReticleDetection:
+    """Class for detecting reticle lines and coordinates."""
+
+    def __init__(self, IMG_SIZE, reticle_frame_detector, camera_name):
+        """Initialize Reticle Detection object"""
+        self.image_size = IMG_SIZE
+        self.reticle_frame_detector = reticle_frame_detector
+        self.mask = None
+        self.name = camera_name
+
+    def _preprocess_image(self, img):
+        """Convert image to grayscale, blur, and resize."""
+        # Check if image is already grayscale
+        if img.ndim == 3 and img.shape[2] == 3:  # Check if image has 3 channels
+            bg = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)
+        else:
+            bg = img
+
+        bg = cv2.GaussianBlur(bg, (11, 11), 0)
+        return bg
+
+    def _apply_mask(self, img):
+        """Apply the mask to the image."""
+        self.mask = self.reticle_frame_detector.process(img)
+        return cv2.bitwise_and(img, img, mask=self.mask)
+
+    def _draw_reticle_lines(self, img, pixels_in_lines):
+        """Draw lines on the reticle points based on detected pixels."""
+        reticle_points = np.zeros_like(img)
+        width, height = self.image_size
+
+        for pixels_in_line in pixels_in_lines:
+            self._draw_line(reticle_points, pixels_in_line, width, height)
+
+        # cv2.imwrite("debug/reticle_zone.jpg", reticle_points)
+        return reticle_points
+
+    def _draw_line(self, reticle_points, pixels_in_line, width, height):
+        """Draw a single line across the reticle points."""
+        x1, y1 = pixels_in_line[0]
+        x2, y2 = pixels_in_line[-1]
+
+        if x2 - x1 == 0:  # Prevent division by zero
+            m = np.inf
+            x_vert = x1  # Vertical line x-coordinate
+        else:
+            m = (y2 - y1) / (x2 - x1)
+            b = y1 - m * x1
+
+        if m == np.inf:
+            cv2.line(
+                reticle_points,
+                (x_vert, 0),
+                (x_vert, height),
+                (255, 255, 255),
+                35,
+            )
+        else:
+            y_start = int(m * 0 + b)
+            y_end = int(m * width + b)
+            cv2.line(
+                reticle_points,
+                (0, y_start),
+                (width, y_end),
+                (255, 255, 255),
+                35,
+            )
+
+    def _ransac_detect_lines(self, img):
+        """Detect lines using RANSAC algorithm.
+
+        Args:
+            img (numpy.ndarray): Input image.
+
+        Returns:
+            tuple: (ret, inlier_lines, inlier_pixels)
+                - ret (bool): True if two lines are detected, False otherwise.
+                - inlier_lines (list): List of detected line models.
+                - inlier_pixels (list): List of inlier pixel coordinates for each line.
+        """
+        inlier_lines = []
+        inlier_pixels = []
+
+        if img is None:
+            return False, inlier_lines, inlier_pixels
+
+        # Draw
+        if len(img.shape) == 2:  # Grayscale image
+            img_color = cv2.cvtColor(img, cv2.COLOR_GRAY2BGR)
+        else:  # Color image
+            img_color = img.copy()
+
+        contours, _ = cv2.findContours(
+            img, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE
+        )
+        centroids = np.array(self._get_centroid(contours))
+        if len(centroids) < 10:
+            logger.debug("points for rasac line detection are less than 10")
+            return False, inlier_lines, inlier_pixels
+
+        max_trials = 7000
+        residual_threshold = 2
+        counter = 50
+        while len(inlier_lines) < 2 and counter > 0:
+            with warnings.catch_warnings():
+                warnings.simplefilter("ignore", RuntimeWarning)
+                model_robust, inliers = ransac(
+                    centroids,
+                    LineModelND,
+                    min_samples=9,
+                    residual_threshold=residual_threshold,
+                    max_trials=max_trials,
+                )
+            inlier_points = centroids[inliers]
+            if len(inlier_points) >= 20:
+                logger.debug(f"residual_threshold: {residual_threshold}")
+                inlier_pixels.append(inlier_points)
+                inlier_lines.append(model_robust)
+                centroids = centroids[~inliers]
+                max_trials = 7000
+                residual_threshold = 2
+                counter = 50  # Reset counter
+            else:
+                max_trials += 2000  # if not found, run RASAC again
+                counter -= 1
+                if residual_threshold <= 15:
+                    residual_threshold += 1
+                continue
+
+        # Draw the centroids
+        """
+        for points in inlier_pixels:
+            for point in points:
+                cv2.circle(img_color, (int(point[0]), int(point[1])), 1, (0, 0, 255), -1)  # Draw green circles
+        cv2.imwrite("debug/centroid.jpg", img_color)
+        """
+
+        return len(inlier_lines) == 2, inlier_lines, inlier_pixels
+
+    def _fit_line(self, pixels):
+        """Fit a line to the given pixels.
+
+        Args:
+            pixels (numpy.ndarray): Pixel coordinates.
+
+        Returns:
+            tuple: (slope, intercept) of the fitted line.
+        """
+        x_coords, y_coords = zip(*pixels)
+        slope, intercept, _, _, _ = linregress(x_coords, y_coords)
+        return slope, intercept
+
+    def _find_intersection(self, line1, line2):
+        """Find the intersection point of two lines.
+
+        Args:
+            line1 (tuple): (slope, intercept) of the first line.
+            line2 (tuple): (slope, intercept) of the second line.
+
+        Returns:
+            tuple or None: (x, y) coordinates of the intersection point if it exists, None otherwise.
+        """
+        slope1, intercept1 = line1
+        slope2, intercept2 = line2
+
+        if slope1 == slope2:
+            return None  # No intersection (parallel lines)
+
+        x_intersect = (intercept2 - intercept1) / (slope1 - slope2)
+        y_intersect = slope1 * x_intersect + intercept1
+        return int(round(x_intersect)), int(round(y_intersect))
+
+    def _get_center_coords_index(self, center, coords):
+        """Get the index of the center coordinates in the given coordinates.
+
+        Args:
+            center (tuple): Center coordinates (x, y).
+            coords (numpy.ndarray): Array of coordinates.
+
+        Returns:
+            int or None: Index of the center coordinates in the coords array, None if not found.
+        """
+        x_center, y_center = center
+        for i in range(-4, 5):
+            for j in range(-4, 5):
+                test_center = np.array([x_center + i, y_center + j])
+                result = np.where((coords == test_center).all(axis=1))
+                if len(result[0]) > 0:
+                    return result[0][0]
+        return None
+
+    def _get_pixels_interest(self, center, coords, dist=10):
+        """Get the pixels of interest around the center coordinates.
+
+        Args:
+            center (tuple): Center coordinates (x, y).
+            coords (numpy.ndarray): Array of coordinates.
+            dist (int): Distance from the center to select pixels of interest. Defaults to 10.
+
+        Returns:
+            numpy.ndarray or None: Selected pixels of interest, None if center is not found.
+        """
+        center_index = self._get_center_coords_index(center, coords)
+        if center_index is None:
+            return
+
+        start_index = max(center_index - dist, 0)
+        end_index = min(center_index + dist + 1, len(coords))
+        return coords[start_index:end_index]
+
+    def _find_reticle_coords(self, pixels_in_lines):
+        """Find the reticle coordinates from the pixels in lines.
+        Args:
+            pixels_in_lines (list): List of pixel coordinates for each line.
+        Returns:
+            list: List of pixel coordinates of interest for each line.
+        """
+        if len(pixels_in_lines) != 2:
+            raise ValueError("Function requires exactly two lines")
+
+        line1 = self._fit_line(pixels_in_lines[0])
+        line2 = self._fit_line(pixels_in_lines[1])
+        center_point = self._find_intersection(line1, line2)
+
+        coords_interest = []
+        for pixels_in_line in pixels_in_lines:
+            coords = self._get_pixels_interest(center_point, pixels_in_line)
+            coords_interest.append(coords)
+
+        return coords_interest
+
+    def _eroding(self, img):
+        """Erode the image until the desired contour conditions are met.
+
+        Args:
+            img (numpy.ndarray): Input image.
+
+        Returns:
+            numpy.ndarray: Eroded image.
+        """
+        kernel_ellipse_3 = cv2.getStructuringElement(cv2.MORPH_ELLIPSE, (3, 3))
+        counter = 100
+        while counter > 0:
+            contours, _ = cv2.findContours(
+                img, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE
+            )
+            if not contours:
+                break
+
+            largest_contour = max(contours, key=cv2.contourArea)
+            largest_contour_area = cv2.contourArea(largest_contour)
+            if 50 < len(contours) < 300 and largest_contour_area < 30 * 30:
+                break
+            img = cv2.erode(img, kernel_ellipse_3, iterations=1)
+            img = cv2.morphologyEx(img, cv2.MORPH_OPEN, kernel_ellipse_3)
+            counter -= 1
+        return img
+
+    def _get_centroid(self, contours):
+        """Get the centroid of each contour.
+
+        Args:
+            contours (list): List of contours.
+
+        Returns:
+            list: List of centroid coordinates for each contour.
+        """
+        centroids = []
+        for contour in contours:
+            M = cv2.moments(contour)
+            if M["m00"] != 0:
+                cX = int(M["m10"] / M["m00"])
+                cY = int(M["m01"] / M["m00"])
+                centroids.append([cX, cY])
+        return centroids
+
+    def __del__(self):
+        """Delete the instance"""
+        # print("ReticleDetection Object destroyed")
+        pass
+
+    def _get_median_distance_x_y(self, points):
+        """Get the median distance for x and y components of the points.
+
+        Args:
+            points (numpy.ndarray): Array of points.
+
+        Returns:
+            tuple: (median_x, median_y)
+        """
+        # Calculate differences between consecutive points
+        diffs = np.diff(points, axis=0)
+        x_diffs = diffs[:, 0]
+        y_diffs = diffs[:, 1]
+        # Compute median distances for x and y
+        median_x_diff = np.median(np.abs(x_diffs))
+        median_y_diff = np.median(np.abs(y_diffs))
+        return median_x_diff, median_y_diff
+
+    def _sort_points(self, points):
+        """Sort the points based on the dimension with greater median distance.
+
+        Args:
+            points (numpy.ndarray): Array of points.
+
+        Returns:
+            numpy.ndarray: Sorted points.
+        """
+        
+        median_x_diff, median_y_diff = self._get_median_distance_x_y(points)
+
+        # Determine which dimension has greater median distance
+        if median_x_diff > median_y_diff:
+            # Sort points based on x component if x has greater median distance
+            sorted_points = points[np.argsort(points[:, 0])]
+        else:
+            # Sort points based on y component if y has greater median distance
+            sorted_points = points[np.argsort(-points[:, 1])]
+
+        return sorted_points
+
+    def _estimate_missing_points(self, points, threshold_factor=1.5):
+        """Estimate missing points in the given points based on the average distance.
+
+        Args:
+            points (numpy.ndarray): Array of points.
+            threshold_factor (float): Factor to determine the threshold for large gaps. Defaults to 1.5.
+
+        Returns:
+            numpy.ndarray: Array of estimated missing points.
+        """
+        points = self._sort_points(points)
+
+        # Calculate the Euclidean distances between consecutive points
+        distances = np.linalg.norm(np.diff(points, axis=0), axis=1)
+
+        # Estimate the average distance
+        average_distance = np.median(distances)
+
+        # Identify large gaps
+        threshold = threshold_factor * average_distance
+        large_gaps = np.where(distances > threshold)[0]
+
+        # Estimate missing points in the large gaps
+        missing_points = []
+        for gap_index in large_gaps:
+            start_point = points[gap_index]
+            end_point = points[gap_index + 1]
+            num_missing = (
+                int(round(distances[gap_index] / average_distance)) - 1
+            )
+            for i in range(1, num_missing + 1):
+                missing_point = start_point + (end_point - start_point) * (
+                    i / (num_missing + 1)
+                )
+                missing_points.append(np.round(missing_point))
+            
+            """
+            logger.debug(f"start_point: {start_point},\
+                         end_point: {end_point},\
+                         num_missing: {num_missing},\
+                         Missing points Interpolated: {missing_points}")
+            """
+            
+        return np.array(missing_points)
+
+    def _add_missing_pixels(self, bg, lines, line_pixels):
+        """Add missing pixels to the line pixels based on the estimated missing points.
+
+        Args:
+            bg (numpy.ndarray): Background image.
+            lines (list): List of line models.
+            line_pixels (list): List of pixel coordinates for each line.
+
+        Returns:
+            tuple: (bg, refined_pixels)
+                - bg (numpy.ndarray): Background image with missing points drawn.
+                - refined_pixels (list): List of refined pixel coordinates for each line.
+        """
+        refined_pixels = []
+
+        for line_model, pixels in zip(lines, line_pixels):
+            pixels_array = np.array(pixels)
+            missing_points = self._estimate_missing_points(pixels_array)
+            x_diff, y_diff = self._get_median_distance_x_y(pixels_array)
+
+            if missing_points.ndim == 1 and missing_points.size > 0:
+                missing_points = missing_points.reshape(-1, 2)  # Reshape to 2D if it's flat but not empty
+            elif missing_points.size == 0:
+                missing_points_adjusted = np.array([])  # Handle empty case
+            else:
+                if x_diff > y_diff:
+                    missing_points_adjusted = np.array([
+                            (x, line_model.predict_y(np.array([x]))[0])
+                            for x in missing_points[:, 0]   
+                    ])
+                else:
+                    missing_points_adjusted = np.array([
+                            (line_model.predict_x(np.array([y]))[0], y)
+                            for y in missing_points[:, 1]
+                    ])
+            logger.debug(f"missing_points: {missing_points}, adjusted: {missing_points_adjusted}")
+
+            # Combine original and adjusted missing points
+            if missing_points_adjusted.size > 0:
+                full_line_pixels = np.vstack(
+                    (pixels_array, missing_points_adjusted)
+                )
+            else:
+                full_line_pixels = pixels_array
+
+            # Sort pixels
+            if x_diff > y_diff:
+                # If range of x is greater, sort by x-coordinate
+                full_line_pixels = full_line_pixels[
+                    full_line_pixels[:, 0].argsort()
+                ]
+            else:
+                # Otherwise, sort by y-coordinate
+                full_line_pixels = full_line_pixels[
+                    full_line_pixels[:, 1].argsort()
+                ]
+
+            full_line_pixels = np.around(full_line_pixels).astype(int)
+            refined_pixels.append(full_line_pixels)
+
+            # Draw missing points
+            if len(missing_points_adjusted) > 0:
+                for pixel in missing_points_adjusted:
+                    pt = tuple(int(coordinate) for coordinate in pixel)
+                    cv2.circle(bg, pt, 2, (0, 255, 255), -1)
+
+        return bg, refined_pixels
+
+    def _refine_pixels(self, bg, lines, line_pixels):
+        """Refine the pixel coordinates fitting into lines based on the line models.
+
+        Args:
+            bg (numpy.ndarray): Background image.
+            lines (list): List of line models.
+            line_pixels (list): List of pixel coordinates for each line.
+
+        Returns:
+            tuple: (bg, lines, refined_pixels)
+                - bg (numpy.ndarray): Background image with refined pixels drawn.
+                - lines (list): List of line models.
+                - refined_pixels (list): List of refined pixel coordinates for each line.
+        """
+        refined_pixels = []
+
+        for line_model, pixels in zip(lines, line_pixels):
+            origin, direction = line_model.params[0], line_model.params[1]
+            # Extend the line
+            point1 = tuple((origin + -2000 * direction).astype(int))  
+            point2 = tuple((origin + 2000 * direction).astype(int))
+            cv2.line(bg, point1, point2, (0, 0, 255), 1)
+            pixels = np.array(pixels)
+            to_pixels = pixels - origin
+            proj_lengths = (
+                np.dot(to_pixels, direction) / np.linalg.norm(direction) ** 2
+            )
+            proj_points = np.outer(proj_lengths, direction) + origin
+
+            proj_points = np.round(proj_points).astype(int)
+            refined_pixels.append(proj_points)
+
+        # Draw
+        for refined_pixels_per_line in refined_pixels:
+            for pixel in refined_pixels_per_line:
+                pt = tuple(pixel)
+                cv2.circle(bg, pt, 3, (255, 0, 0), -1)
+        # cv2.imwrite("debug/refined_pixels.jpg", bg)
+        return bg, lines, refined_pixels
+
+    def get_reticle_zone(self, img):
+        """Get the reticle zone from the image.
+
+        Args:
+            img (numpy.ndarray): Input image.
+
+        Returns:
+            numpy.ndarray or None: Reticle zone image if reticle exists, None otherwise.
+        """
+        bg = self._preprocess_image(img)
+        bg = cv2.resize(bg, self.image_size)
+        masked = self._apply_mask(bg)
+        if self.reticle_frame_detector.is_reticle_exist:
+            ret, bg, _, pixels_in_lines = self.coords_detect_morph(bg)
+            return self._draw_reticle_lines(bg, pixels_in_lines)
+        else:
+            return None
+
+    def coords_detect_morph(self, img):
+        """
+        Applies morphological operations and adaptive thresholding
+        to detect coordinates in an image.
+        """
+        img_color = cv2.cvtColor(img, cv2.COLOR_GRAY2BGR)
+        if img.shape == (3000, 4000):
+            img = cv2.adaptiveThreshold(
+                img,
+                255,
+                cv2.ADAPTIVE_THRESH_GAUSSIAN_C,
+                cv2.THRESH_BINARY,
+                13,
+                2,
+            )
+        else:
+            img = cv2.adaptiveThreshold(
+                img,
+                255,
+                cv2.ADAPTIVE_THRESH_GAUSSIAN_C,
+                cv2.THRESH_BINARY,
+                11,
+                3,
+            )
+        img = cv2.medianBlur(img, 5)
+        img = cv2.bitwise_not(img, mask=self.mask)
+        kernel_ellipse_5 = cv2.getStructuringElement(cv2.MORPH_ELLIPSE, (5, 5))
+        kernel_ellipse_3 = cv2.getStructuringElement(cv2.MORPH_ELLIPSE, (3, 3))
+        img = cv2.morphologyEx(img, cv2.MORPH_CLOSE, kernel_ellipse_5)
+
+        img = self._eroding(img)
+        #cv2.imwrite("debug/after_eroding.jpg", img)
+        ret, inliner_lines, inliner_lines_pixels = self._ransac_detect_lines(img)
+        logger.debug(f"n of inliner lines: {len(inliner_lines_pixels)}")
+
+        # Draw
+        for inliner_lines_pixel in inliner_lines_pixels:
+            for pixel in inliner_lines_pixel:
+                pt = tuple(pixel)
+                cv2.circle(img_color, pt, 1, (0, 255, 0), -1)
+        # cv2.imwrite("debug/inliner_pixels.jpg", img_color)
+
+        return ret, img, inliner_lines, inliner_lines_pixels
+
+    def _draw_debug(self, img, pixels_in_lines, filename):
+        if logger.getEffectiveLevel() == logging.DEBUG:        
+            if img.ndim == 2:
+                img_ = cv2.cvtColor(img, cv2.COLOR_GRAY2BGR)
+            else:
+                img_ = img.copy()
+
+            if len(pixels_in_lines) == 2:
+                for pt in pixels_in_lines[0]:
+                    cv2.circle(img_, tuple(pt), 2, (0, 255, 0), -1)
+                for pt in pixels_in_lines[1]:
+                    cv2.circle(img_, tuple(pt), 1, (255, 0, 0), -1)
+
+            cv2.imwrite(f"debug/{filename}.jpg", img_)
+        else:
+            return
+
+    def get_coords(self, img):
+        """Detect coordinates using morphological operations.
+
+        Args:
+            img (numpy.ndarray): Input image.
+
+        Returns:
+            tuple: (ret, img, inliner_lines, inliner_lines_pixels)
+                - ret (bool): True if coordinates are detected, False otherwise.
+                - img (numpy.ndarray): Processed image.
+                - inliner_lines (list): List of inlier line models.
+                - inliner_lines_pixels (list): List of inlier pixel coordinates for each line.
+        """
+        bg = self._preprocess_image(img)
+        self._draw_debug(bg, [], "0_bg")
+        masked = self._apply_mask(bg)
+        self._draw_debug(masked, [], "1_bg")
+
+        ret, bg, inliner_lines, pixels_in_lines = self.coords_detect_morph(masked)
+        self._draw_debug(bg, pixels_in_lines, "2_detect_morph")
+        logger.debug(f"{self.name} nLines: {len(pixels_in_lines)}")
+
+        if ret:
+            bg, inliner_lines, pixels_in_lines = self._refine_pixels(bg, inliner_lines, pixels_in_lines)
+            logger.debug(f"{self.name} detect: {len(pixels_in_lines[0])}, {len(pixels_in_lines[1])}" )
+            self._draw_debug(bg, pixels_in_lines, "3_refine_pixels")
+    
+            bg, pixels_in_lines = self._add_missing_pixels(bg, inliner_lines, pixels_in_lines)
+            logger.debug(f"{self.name} interpolate: {len(pixels_in_lines[0])} {len(pixels_in_lines[1])}")
+            self._draw_debug(bg, pixels_in_lines, "4_add_missing_pixels")
+        
+        return ret, bg, inliner_lines, pixels_in_lines
+
+    """
+    def is_distance_tip_reticle_threshold(self, probe, reticle, thresh=10):
+        tip_x, tip_y = probe["tip_coords"]
+        dist_transform = cv2.distanceTransform(reticle, cv2.DIST_L2, cv2.DIST_MASK_PRECISE)
+        # Get the distance at the tip location
+        distance_at_tip = dist_transform[int(tip_y), int(tip_x)]
+        print("distance_at_tip: ", distance_at_tip)
+        return distance_at_tip > thresh
+    """
```

### Comparing `parallax_app-0.37.1/parallax/reticle_detection_coords_interests.py` & `parallax_app-0.37.5/parallax/reticle_detection_coords_interests.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,171 +1,180 @@
-
-"""
-Provides functionality to detect and analyze points of interest on reticle lines in images, 
-employing line fitting and orientation determination techniques suitable 
-for microscopy image analysis tasks.
-"""
-
-import logging
-
-import numpy as np
-from PyQt5.QtCore import QObject
-from scipy.stats import linregress
-
-# Set logger name
-logger = logging.getLogger(__name__)
-logger.setLevel(logging.WARNING)
-# Set the logging level for PyQt5.uic.uiparser/properties to WARNING, to ignore DEBUG messages
-logging.getLogger("PyQt5.uic.uiparser").setLevel(logging.WARNING)
-logging.getLogger("PyQt5.uic.properties").setLevel(logging.WARNING)
-
-
-class ReticleDetectCoordsInterest(QObject):
-    """Class for detecting coordinates of interest in reticle lines."""
-
-    def __init__(self):
-        """Initialize object"""
-        self.n_interest_pixels = 15
-        pass
-
-    def _fit_line(self, pixels):
-        """Fit a line to the given pixels.
-
-        Args:
-            pixels (list): List of pixel coordinates.
-
-        Returns:
-            tuple: Slope and intercept of the fitted line.
-        """
-        x_coords, y_coords = zip(*pixels)
-        slope, intercept, _, _, _ = linregress(x_coords, y_coords)
-        return slope, intercept
-
-    def _find_intersection(self, line1, line2):
-        """Find the intersection point of two lines.
-
-        Args:
-            line1 (tuple): Slope and intercept of the first line.
-            line2 (tuple): Slope and intercept of the second line.
-
-        Returns:
-            tuple or None: Coordinates of the intersection point if it exists, None otherwise.
-        """
-        slope1, intercept1 = line1
-        slope2, intercept2 = line2
-
-        # Check if lines are parallel
-        if slope1 == slope2:
-            return None  # No intersection (parallel lines)
-
-        # Calculate intersection point
-        x_intersect = (intercept2 - intercept1) / (slope1 - slope2)
-        y_intersect = slope1 * x_intersect + intercept1
-        return int(round(x_intersect)), int(round(y_intersect))
-
-    def _get_center_coords_index(self, center, coords):
-        """Get the index of the center coordinates in the given coordinates.
-
-        Args:
-            center (tuple): Center coordinates.
-            coords (numpy.ndarray): Array of coordinates.
-
-        Returns:
-            int or None: Index of the center coordinates if found, None otherwise.
-        """
-        x_center, y_center = center
-        for i in range(-5, 6):  # Range from -5 to 5
-            for j in range(-5, 6):  # Range from -5 to 5
-                test_center = np.array([x_center + i, y_center + j])
-                result = np.where((coords == test_center).all(axis=1))
-                if len(result[0]) > 0:  # Check if the element was found
-                    return result[0][0]  # Return the first occurrence index
-        return None
-
-    def _get_pixels_interest(self, center, coords):
-        """Get the pixels of interest around the center coordinates.
-
-        Args:
-            center (tuple): Center coordinates.
-            coords (numpy.ndarray): Array of coordinates.
-
-        Returns:
-            numpy.ndarray or None: Pixels of interest if found, None otherwise.
-        """
-        center_index = self._get_center_coords_index(center, coords)
-        if center_index is None:
-            return
-
-        coords[center_index] = center  # Replace center to center point we gets
-        start_index = max(center_index - self.n_interest_pixels, 0)
-        end_index = min(center_index + self.n_interest_pixels + 1, len(coords))
-        return coords[start_index:end_index]
-
-    def _get_orientation(self, pixels_in_lines):
-        """Get the orientation of the reticle lines.
-
-        Args:
-            pixels_in_lines (list): List of pixel lines.
-
-        Returns:
-            tuple: (ret, x_axis, y_axis)
-                - ret (bool): True if orientation is determined, False otherwise.
-                - x_axis (numpy.ndarray): X-axis coordinates.
-                - y_axis (numpy.ndarray): Y-axis coordinates.
-        """
-        if pixels_in_lines[0] is None or pixels_in_lines[1] is None:
-            logger.error("One of the pixel lines is None. Cannot proceed with orientation calculation.")
-            return False, None, None
-
-        # Temp solution: first coords of X axis is left side to first coords of Y axis.
-        min_x_value_line0 = min(pixels_in_lines[0], key=lambda x: x[0])
-        min_x_value_line1 = min(pixels_in_lines[1], key=lambda x: x[0])
-        # print(min_x_value_line0, min_x_value_line1)
-        if min_x_value_line0[0] < min_x_value_line1[0]:
-            x_axis, y_axis = pixels_in_lines[0], pixels_in_lines[1]
-        else:
-            x_axis, y_axis = pixels_in_lines[1], pixels_in_lines[0]
-
-        # Sort by ascending order
-        x_axis = x_axis[np.argsort(x_axis[:, 0])]
-        y_axis = y_axis[np.argsort(-y_axis[:, 1])]
-        return True, x_axis, y_axis
-
-    def get_coords_interest(self, pixels_in_lines):
-        """Get the coordinates of interest from the pixel lines.
-
-        Args:
-            pixels_in_lines (list): List of pixel lines.
-
-        Returns:
-            tuple: (ret, x_axis, y_axis)
-                - ret (bool): True if coordinates of interest are found, False otherwise.
-                - x_axis (numpy.ndarray): X-axis coordinates.
-                - y_axis (numpy.ndarray): Y-axis coordinates.
-        """
-        if len(pixels_in_lines) != 2:
-            return False, None, None
-
-        if pixels_in_lines[0] is None or pixels_in_lines[1] is None:
-            return False, None, None
-
-        if len(pixels_in_lines[0]) < self.n_interest_pixels*2 + 1 \
-            or len(pixels_in_lines[1]) < self.n_interest_pixels*2 + 1:
-            return False, None, None
-
-        coords_interest = []
-        # Find the center pixels (crossing point between two lines)
-        line1 = self._fit_line(pixels_in_lines[0])
-        line2 = self._fit_line(pixels_in_lines[1])
-        center_point = self._find_intersection(line1, line2)
-        logger.debug(f"center_point: {center_point}")
-
-        for pixels_in_line in pixels_in_lines:
-            coords = self._get_pixels_interest(center_point, pixels_in_line)
-            if coords is None or len(coords) < self.n_interest_pixels * 2 + 1:
-                return False, None, None
-            coords_interest.append(coords)
-
-        ret, x_axis, y_axis = self._get_orientation(coords_interest)
-        if ret is False:
-            return False, None, None
-        return True, x_axis, y_axis
+
+"""
+Provides functionality to detect and analyze points of interest on reticle lines in images, 
+employing line fitting and orientation determination techniques suitable 
+for microscopy image analysis tasks.
+"""
+
+import logging
+
+import numpy as np
+from PyQt5.QtCore import QObject
+from scipy.stats import linregress
+
+# Set logger name
+logger = logging.getLogger(__name__)
+logger.setLevel(logging.WARNING)
+# Set the logging level for PyQt5.uic.uiparser/properties to WARNING, to ignore DEBUG messages
+logging.getLogger("PyQt5.uic.uiparser").setLevel(logging.WARNING)
+logging.getLogger("PyQt5.uic.properties").setLevel(logging.WARNING)
+
+
+class ReticleDetectCoordsInterest(QObject):
+    """Class for detecting coordinates of interest in reticle lines."""
+
+    def __init__(self):
+        """Initialize object"""
+        self.n_interest_pixels = 15
+        pass
+
+    def _fit_line(self, pixels):
+        """Fit a line to the given pixels.
+
+        Args:
+            pixels (list): List of pixel coordinates.
+
+        Returns:
+            tuple: Slope and intercept of the fitted line.
+        """
+        x_coords, y_coords = zip(*pixels)
+        slope, intercept, _, _, _ = linregress(x_coords, y_coords)
+        return slope, intercept
+
+    def _find_intersection(self, line1, line2):
+        """Find the intersection point of two lines.
+
+        Args:
+            line1 (tuple): Slope and intercept of the first line.
+            line2 (tuple): Slope and intercept of the second line.
+
+        Returns:
+            tuple or None: Coordinates of the intersection point if it exists, None otherwise.
+        """
+        slope1, intercept1 = line1
+        slope2, intercept2 = line2
+
+        # Check if lines are parallel
+        if slope1 == slope2:
+            return None  # No intersection (parallel lines)
+
+        # Calculate intersection point
+        x_intersect = (intercept2 - intercept1) / (slope1 - slope2)
+        y_intersect = slope1 * x_intersect + intercept1
+        return int(round(x_intersect)), int(round(y_intersect))
+
+    def _get_center_coords_index(self, center, coords):
+        """Get the index of the center coordinates in the given coordinates.
+
+        Args:
+            center (tuple): Center coordinates.
+            coords (numpy.ndarray): Array of coordinates.
+
+        Returns:
+            int or None: Index of the center coordinates if found, None otherwise.
+        """
+        x_center, y_center = center
+        for i in range(-5, 6):  # Range from -5 to 5
+            for j in range(-5, 6):  # Range from -5 to 5
+                test_center = np.array(
+                    [x_center + i, y_center + j], dtype=coords.dtype
+                )
+                result = np.where((coords == test_center).all(axis=1))
+                if len(result[0]) > 0:  # Check if the element was found
+                    return result[0][0]  # Return the first occurrence index
+        return None
+
+    def _get_pixels_interest(self, center, coords):
+        """Get the pixels of interest around the center coordinates.
+
+        Args:
+            center (tuple): Center coordinates.
+            coords (numpy.ndarray): Array of coordinates.
+
+        Returns:
+            numpy.ndarray or None: Pixels of interest if found, None otherwise.
+        """
+        center_index = self._get_center_coords_index(center, coords)
+        if center_index is None:
+            logger.debug("Center coordinates not found.")
+            return
+
+        coords[center_index] = center  # Replace center to center point we gets
+        start_index = max(center_index - self.n_interest_pixels, 0)
+        end_index = min(center_index + self.n_interest_pixels + 1, len(coords))
+        return coords[start_index:end_index]
+
+    def _get_orientation(self, pixels_in_lines):
+        """Get the orientation of the reticle lines.
+
+        Args:
+            pixels_in_lines (list): List of pixel lines.
+
+        Returns:
+            tuple: (ret, x_axis, y_axis)
+                - ret (bool): True if orientation is determined, False otherwise.
+                - x_axis (numpy.ndarray): X-axis coordinates.
+                - y_axis (numpy.ndarray): Y-axis coordinates.
+        """
+        if pixels_in_lines[0] is None or pixels_in_lines[1] is None:
+            logger.error("One of the pixel lines is None. Cannot proceed with orientation calculation.")
+            return False, None, None
+
+        # Temp solution: first coords of X axis is left side to first coords of Y axis.
+        min_x_value_line0 = min(pixels_in_lines[0], key=lambda x: x[0])
+        min_x_value_line1 = min(pixels_in_lines[1], key=lambda x: x[0])
+        # print(min_x_value_line0, min_x_value_line1)
+        if min_x_value_line0[0] < min_x_value_line1[0]:
+            x_axis, y_axis = pixels_in_lines[0], pixels_in_lines[1]
+        else:
+            x_axis, y_axis = pixels_in_lines[1], pixels_in_lines[0]
+
+        # Sort by ascending order
+        x_axis = x_axis[np.argsort(x_axis[:, 0])]
+        y_axis = y_axis[np.argsort(-y_axis[:, 1])]
+        return True, x_axis, y_axis
+
+    def get_coords_interest(self, pixels_in_lines):
+        """Get the coordinates of interest from the pixel lines.
+
+        Args:
+            pixels_in_lines (list): List of pixel lines.
+
+        Returns:
+            tuple: (ret, x_axis, y_axis)
+                - ret (bool): True if coordinates of interest are found, False otherwise.
+                - x_axis (numpy.ndarray): X-axis coordinates.
+                - y_axis (numpy.ndarray): Y-axis coordinates.
+        """
+        if len(pixels_in_lines) != 2:
+            return False, None, None
+
+        if pixels_in_lines[0] is None or pixels_in_lines[1] is None:
+            return False, None, None
+
+        if len(pixels_in_lines[0]) < self.n_interest_pixels*2 + 1 \
+            or len(pixels_in_lines[1]) < self.n_interest_pixels*2 + 1:
+            return False, None, None
+
+        coords_interest = []
+        # Find the center pixels (crossing point between two lines)
+        line1 = self._fit_line(pixels_in_lines[0])
+        line2 = self._fit_line(pixels_in_lines[1])
+        center_point = self._find_intersection(line1, line2)
+        logger.debug(f"center_point: {center_point}")
+
+        for pixels_in_line in pixels_in_lines:
+            coords = self._get_pixels_interest(center_point, pixels_in_line)
+            if coords is None or len(coords) < self.n_interest_pixels * 2 + 1:
+                logger.debug(f"_get_pixels_interest fails.")
+                if coords is None:
+                    logger.debug(f"coords: None")
+                if coords is not None:
+                    logger.debug(f"length of coords: {len(coords)}")
+                return False, None, None
+            coords_interest.append(coords)
+
+        ret, x_axis, y_axis = self._get_orientation(coords_interest)
+        if ret is False:
+            logger.debug(f"getting orientation of x and y axis fails")
+            return False, None, None
+        return True, x_axis, y_axis
```

### Comparing `parallax_app-0.37.1/parallax/screen_widget.py` & `parallax_app-0.37.5/parallax/screen_widget.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,373 +1,373 @@
-
-"""
-Provides ScreenWidget for image interaction in microscopy apps, supporting image display, 
-point selection, and zooming. It integrates with probe and reticle detection managers 
-for real-time processing and offers camera control functions.
-"""
-
-import logging
-
-import cv2
-import pyqtgraph as pg
-from PyQt5 import QtCore
-from PyQt5.QtCore import Qt, pyqtSignal
-
-from .no_filter import NoFilter
-from .probe_detect_manager import ProbeDetectManager
-from .reticle_detect_manager import ReticleDetectManager
-
-# Set logger name
-logger = logging.getLogger(__name__)
-logger.setLevel(logging.DEBUG)
-# Set the logging level for PyQt5.uic.uiparser/properties to WARNING, to ignore DEBUG messages
-logging.getLogger("PyQt5.uic.uiparser").setLevel(logging.WARNING)
-logging.getLogger("PyQt5.uic.properties").setLevel(logging.WARNING)
-
-
-class ScreenWidget(pg.GraphicsView):
-    """Screens Class"""
-
-    selected = pyqtSignal(int, int)
-    cleared = pyqtSignal()
-    reticle_coords_detected = pyqtSignal()
-    probe_coords_detected = pyqtSignal()
-
-    def __init__(self, camera, filename=None, model=None, parent=None):
-        """Init screen widget object"""
-        super().__init__(parent=parent)
-        self.filename = filename
-        self.model = model
-
-        self.view_box = pg.ViewBox(defaultPadding=0)
-        self.setCentralItem(self.view_box)
-        self.view_box.setAspectLocked()
-        self.view_box.invertY()
-
-        self.image_item = ClickableImage()
-        self.image_item.axisOrder = "row-major"
-        self.view_box.addItem(self.image_item)
-        self.image_item.mouse_clicked.connect(self.image_clicked)
-
-        self.click_target = pg.TargetItem()
-        self.view_box.addItem(self.click_target)
-        self.click_target.setVisible(False)
-
-        self.click_target2 = pg.TargetItem()
-        self.view_box.addItem(self.click_target2)
-        self.click_target2.setVisible(False)
-
-        self.camera_actions = []
-        self.focochan_actions = []
-        self.filter_actions = []
-        self.detector_actions = []
-        self.reticle_coords = None
-        self.mtx, self.dist = None, None
-
-        # probe
-        self.probe_detect_last_timestamp = None
-        self.probe_detect_last_sn = None
-        self.probe_detect_last_coords = None
-
-        # camera
-        self.camera = camera
-        camera_name = self.get_camera_name()
-        self.focochan = None
-
-        # No filter
-        self.filter = NoFilter()
-        self.filter.frame_processed.connect(self.set_image_item_from_data)
-
-        # Reticle Detection
-        self.reticleDetector = ReticleDetectManager(camera_name)
-        self.reticleDetector.frame_processed.connect(
-            self.set_image_item_from_data
-        )
-        self.reticleDetector.found_coords.connect(self.found_reticle_coords)
-        self.reticleDetector.found_coords.connect(self.reticle_coords_detected)
-
-        # Probe Detection
-        self.probeDetector = ProbeDetectManager(self.model, camera_name)
-        self.model.add_probe_detector(self.probeDetector)
-        self.probeDetector.frame_processed.connect(
-            self.set_image_item_from_data
-        )
-        self.probeDetector.found_coords.connect(self.found_probe_coords)
-        self.probeDetector.found_coords.connect(self.probe_coords_detected)
-
-        if self.filename:
-            self.set_data(cv2.imread(filename, cv2.IMREAD_GRAYSCALE))
-
-    def refresh(self):
-        """
-        Refresh the image displayed in the screen widget. (Continuously)
-        """
-        if self.camera:
-            data = self.camera.get_last_image_data()
-            self.set_data(data)
-
-    def start_acquisition_camera(self):
-        """
-        Start the camera acquisition. (Continuously)
-        """
-        if self.camera:
-            self.camera.begin_continuous_acquisition()
-
-    def stop_acquisition_camera(self):
-        """
-        Stop the camera acquisition. (Continuously)
-        """
-        if self.camera:
-            self.camera.stop(clean=False)
-
-    def refresh_single_frame(self):
-        """
-        Refresh the image displayed in the screen widget. (Single Frame)
-        """
-        if self.camera:
-            data = self.camera.get_last_image_data_singleFrame()
-            self.set_data(data)
-
-    def single_acquisition_camera(self):
-        """
-        Start the camera acquisition. (Single Frame)
-        """
-        if self.camera:
-            self.camera.begin_singleframe_acquisition()
-
-    def stop_single_acquisition_camera(self):
-        """
-        Stop the camera acquisition. (Single Frame)
-        """
-        if self.camera:
-            self.camera.end_singleframe_acquisition()
-
-    def set_data(self, data):
-        """
-        Set the data displayed in the screen widget.
-        """
-        self.filter.process(data)
-        self.reticleDetector.process(data)
-        captured_time = self.camera.get_last_capture_time(millisecond=True)
-        self.probeDetector.process(data, captured_time)
-
-    def is_camera(self):
-        """
-        Return True if the camera is 'Blackfly' camera.
-        """
-        camera_name = self.camera.name(sn_only=False)
-        return True if "Blackfly" in camera_name else False
-
-    def get_camera_name(self):
-        """
-        Return the name of the camera.
-        """
-        return self.camera.name(sn_only=True) if self.camera else None
-
-    def clear_selected(self):
-        """
-        Clear the selected target.
-        """
-        self.click_target.setVisible(False)
-        self.cleared.emit()
-
-    def save_image(self, filepath, isTimestamp=False, name="Microscope_"):
-        """
-        Save the image displayed in the screen widget.
-        """
-        if self.camera:
-            self.camera.save_last_image(filepath, isTimestamp, name)
-
-    def save_recording(self, filepath, isTimestamp=False, name="Microscope_"):
-        """
-        Save the recording frames that are displayed from camera.
-        """
-        if self.camera:
-            self.camera.save_recording(filepath, isTimestamp, name)
-
-    def stop_recording(self):
-        """
-        Stop the recording.
-        """
-        if self.camera:
-            self.camera.stop_recording()
-
-    def set_image_item_from_data(self, data):
-        """display image from data"""
-        self.image_item.setImage(data, autoLevels=False)
-
-    def set_camera_setting(self, setting, val):
-        """
-        Set the camera settings. (exposure, gain, gamma, wb)
-
-        exposure (int): min: 90,000(10fps) max: 250,000(4fps)
-        gain (float): The desired gain value. min:0, max:27.0
-        wb (float): The desired white balance value. min:1.8, max:2.5
-        gamma (float): The desired gamma value. min:0.25 max:1.25
-        """
-        if self.camera:
-            if setting == "exposure":
-                self.camera.set_exposure(val)
-            elif setting == "gain":
-                self.camera.set_gain(val)
-            elif setting == "gamma":
-                self.camera.set_gamma(val)
-            elif setting == "wbRed":
-                self.camera.set_wb("Red", val)
-            elif setting == "wbBlue":
-                self.camera.set_wb("Blue", val)
-
-    def get_camera_setting(self, setting):
-        """Get the specified camera setting value.
-
-        Args:
-            setting (str): The camera setting to retrieve.
-                Possible values: "exposure", "gain", "gamma", "wbRed", "wbBlue".
-
-        Returns:
-            float: The value of the specified camera setting.
-        """
-        val = 0
-        if self.camera:
-            if setting == "exposure":
-                val = self.camera.get_exposure()
-            elif setting == "gain":
-                val = self.camera.get_gain()
-            elif setting == "gamma":
-                self.camera.disable_gamma()
-            elif setting == "wbRed":
-                val = self.camera.get_wb("Red")
-            elif setting == "wbBlue":
-                val = self.camera.get_wb("Blue")
-        return val
-
-    def get_camera_color_type(self):
-        """Get the color type of the camera.
-
-        Returns:
-            str: The color type of the camera.
-        """
-        if self.camera:
-            return self.camera.device_color_type
-
-    def image_clicked(self, event):
-        """
-        Handle the image click event.
-        """
-        if event.button() == QtCore.Qt.MouseButton.LeftButton:
-            self.select(event.pos())
-        elif event.button() == QtCore.Qt.MouseButton.MiddleButton:
-            self.zoom_out()
-
-    def select(self, pos):
-        """Select a position and emit the selected coordinates."""
-        self.click_target.setPos(pos)
-        self.click_target.setVisible(True)
-        self.selected.emit(*self.get_selected())
-
-    def select2(self, pos):
-        """Select a second position and make the click target visible."""
-        self.click_target2.setPos(pos)
-        self.click_target2.setVisible(True)
-
-    def zoom_out(self):
-        """
-        Zoom out the image. Fill the screen widget with the image.
-        """
-        self.view_box.autoRange()
-
-    def set_camera(self, camera):
-        """
-        Set the camera.
-        """
-        self.camera = camera
-        self.reticleDetector.set_name(self.get_camera_name())
-
-    def run_reticle_detection(self):
-        """Run reticle detection by stopping the filter and starting the reticle detector."""
-        logger.debug("run_reticle_detection")
-        self.filter.stop()
-        self.reticleDetector.start()
-
-    def run_probe_detection(self):
-        """Run probe detection by stopping the filter and starting the probe detector."""
-        logger.debug("run_probe_detection")
-        self.filter.stop()
-        self.probeDetector.start()
-
-    def run_no_filter(self):
-        """Run without any filter by stopping the reticle detector and probe detector."""
-        logger.debug("run_no_filter")
-        self.reticleDetector.stop()
-        self.probeDetector.stop()
-        self.filter.start()
-
-    def found_reticle_coords(self, x_coords, y_coords, mtx, dist):
-        """Store the found reticle coordinates, camera matrix, and distortion coefficients."""
-        self.reticle_coords = [x_coords, y_coords]
-        self.mtx = mtx
-        self.dist = dist
-
-    def reset_reticle_coords(self):
-        """Reset reticle coordinates."""
-        self.reticle_coords = None
-
-    def found_probe_coords(self, timestamp, probe_sn, stage_info, tip_coords):
-        """Store the found probe coordinates and related information."""
-        self.probe_detect_last_timestamp = timestamp
-        self.probe_detect_last_sn = probe_sn
-        self.stage_info = stage_info
-        self.probe_detect_last_coords = tip_coords
-
-    def get_last_detect_probe_info(self):
-        """Get the last detected probe information."""
-        return (
-            self.probe_detect_last_timestamp,
-            self.probe_detect_last_sn,
-            self.probe_detect_last_coords,
-        )
-
-    def get_camera_intrinsic(self):
-        """Get the camera intrinsic parameters."""
-        return self.mtx, self.dist
-
-    def get_reticle_coords(self):
-        """Get the reticle coordinates."""
-        return self.reticle_coords
-
-    def get_selected(self):
-        """
-        Return the selected target position.
-        """
-        if self.click_target.isVisible():
-            pos = self.click_target.pos()
-            return pos.x(), pos.y()
-        else:
-            return None, None
-
-    def wheelEvent(self, e):
-        """
-        Handle the mouse wheel event.
-        """
-        forward = bool(e.angleDelta().y() > 0)
-        control = bool(e.modifiers() & Qt.ControlModifier)
-        shift = bool(e.modifiers() & Qt.ShiftModifier)
-        if control:
-            if self.focochan:
-                foco, chan = self.focochan
-                dist = 20 if shift else 100
-                foco.time_move(chan, forward, dist, wait=True)
-        else:
-            super().wheelEvent(e)
-
-
-class ClickableImage(pg.ImageItem):
-    """This class captures mouse click events on images."""
-
-    mouse_clicked = pyqtSignal(object)
-
-    def mouseClickEvent(self, ev):
-        """
-        Handle the mouse click event.
-        """
-        super().mouseClickEvent(ev)
-        self.mouse_clicked.emit(ev)
+
+"""
+Provides ScreenWidget for image interaction in microscopy apps, supporting image display, 
+point selection, and zooming. It integrates with probe and reticle detection managers 
+for real-time processing and offers camera control functions.
+"""
+
+import logging
+
+import cv2
+import pyqtgraph as pg
+from PyQt5 import QtCore
+from PyQt5.QtCore import Qt, pyqtSignal
+
+from .no_filter import NoFilter
+from .probe_detect_manager import ProbeDetectManager
+from .reticle_detect_manager import ReticleDetectManager
+
+# Set logger name
+logger = logging.getLogger(__name__)
+logger.setLevel(logging.DEBUG)
+# Set the logging level for PyQt5.uic.uiparser/properties to WARNING, to ignore DEBUG messages
+logging.getLogger("PyQt5.uic.uiparser").setLevel(logging.WARNING)
+logging.getLogger("PyQt5.uic.properties").setLevel(logging.WARNING)
+
+
+class ScreenWidget(pg.GraphicsView):
+    """Screens Class"""
+
+    selected = pyqtSignal(int, int)
+    cleared = pyqtSignal()
+    reticle_coords_detected = pyqtSignal()
+    probe_coords_detected = pyqtSignal()
+
+    def __init__(self, camera, filename=None, model=None, parent=None):
+        """Init screen widget object"""
+        super().__init__(parent=parent)
+        self.filename = filename
+        self.model = model
+
+        self.view_box = pg.ViewBox(defaultPadding=0)
+        self.setCentralItem(self.view_box)
+        self.view_box.setAspectLocked()
+        self.view_box.invertY()
+
+        self.image_item = ClickableImage()
+        self.image_item.axisOrder = "row-major"
+        self.view_box.addItem(self.image_item)
+        self.image_item.mouse_clicked.connect(self.image_clicked)
+
+        self.click_target = pg.TargetItem()
+        self.view_box.addItem(self.click_target)
+        self.click_target.setVisible(False)
+
+        self.click_target2 = pg.TargetItem()
+        self.view_box.addItem(self.click_target2)
+        self.click_target2.setVisible(False)
+
+        self.camera_actions = []
+        self.focochan_actions = []
+        self.filter_actions = []
+        self.detector_actions = []
+        self.reticle_coords = None
+        self.mtx, self.dist = None, None
+
+        # probe
+        self.probe_detect_last_timestamp = None
+        self.probe_detect_last_sn = None
+        self.probe_detect_last_coords = None
+
+        # camera
+        self.camera = camera
+        camera_name = self.get_camera_name()
+        self.focochan = None
+
+        # No filter
+        self.filter = NoFilter()
+        self.filter.frame_processed.connect(self.set_image_item_from_data)
+
+        # Reticle Detection
+        self.reticleDetector = ReticleDetectManager(camera_name)
+        self.reticleDetector.frame_processed.connect(
+            self.set_image_item_from_data
+        )
+        self.reticleDetector.found_coords.connect(self.found_reticle_coords)
+        self.reticleDetector.found_coords.connect(self.reticle_coords_detected)
+
+        # Probe Detection
+        self.probeDetector = ProbeDetectManager(self.model, camera_name)
+        self.model.add_probe_detector(self.probeDetector)
+        self.probeDetector.frame_processed.connect(
+            self.set_image_item_from_data
+        )
+        self.probeDetector.found_coords.connect(self.found_probe_coords)
+        self.probeDetector.found_coords.connect(self.probe_coords_detected)
+
+        if self.filename:
+            self.set_data(cv2.imread(filename, cv2.IMREAD_GRAYSCALE))
+
+    def refresh(self):
+        """
+        Refresh the image displayed in the screen widget. (Continuously)
+        """
+        if self.camera:
+            data = self.camera.get_last_image_data()
+            self.set_data(data)
+
+    def start_acquisition_camera(self):
+        """
+        Start the camera acquisition. (Continuously)
+        """
+        if self.camera:
+            self.camera.begin_continuous_acquisition()
+
+    def stop_acquisition_camera(self):
+        """
+        Stop the camera acquisition. (Continuously)
+        """
+        if self.camera:
+            self.camera.stop(clean=False)
+
+    def refresh_single_frame(self):
+        """
+        Refresh the image displayed in the screen widget. (Single Frame)
+        """
+        if self.camera:
+            data = self.camera.get_last_image_data_singleFrame()
+            self.set_data(data)
+
+    def single_acquisition_camera(self):
+        """
+        Start the camera acquisition. (Single Frame)
+        """
+        if self.camera:
+            self.camera.begin_singleframe_acquisition()
+
+    def stop_single_acquisition_camera(self):
+        """
+        Stop the camera acquisition. (Single Frame)
+        """
+        if self.camera:
+            self.camera.end_singleframe_acquisition()
+
+    def set_data(self, data):
+        """
+        Set the data displayed in the screen widget.
+        """
+        self.filter.process(data)
+        self.reticleDetector.process(data)
+        captured_time = self.camera.get_last_capture_time(millisecond=True)
+        self.probeDetector.process(data, captured_time)
+
+    def is_camera(self):
+        """
+        Return True if the camera is 'Blackfly' camera.
+        """
+        camera_name = self.camera.name(sn_only=False)
+        return True if "Blackfly" in camera_name else False
+
+    def get_camera_name(self):
+        """
+        Return the name of the camera.
+        """
+        return self.camera.name(sn_only=True) if self.camera else None
+
+    def clear_selected(self):
+        """
+        Clear the selected target.
+        """
+        self.click_target.setVisible(False)
+        self.cleared.emit()
+
+    def save_image(self, filepath, isTimestamp=False, name="Microscope_"):
+        """
+        Save the image displayed in the screen widget.
+        """
+        if self.camera:
+            self.camera.save_last_image(filepath, isTimestamp, name)
+
+    def save_recording(self, filepath, isTimestamp=False, name="Microscope_"):
+        """
+        Save the recording frames that are displayed from camera.
+        """
+        if self.camera:
+            self.camera.save_recording(filepath, isTimestamp, name)
+
+    def stop_recording(self):
+        """
+        Stop the recording.
+        """
+        if self.camera:
+            self.camera.stop_recording()
+
+    def set_image_item_from_data(self, data):
+        """display image from data"""
+        self.image_item.setImage(data, autoLevels=False)
+
+    def set_camera_setting(self, setting, val):
+        """
+        Set the camera settings. (exposure, gain, gamma, wb)
+
+        exposure (int): min: 90,000(10fps) max: 250,000(4fps)
+        gain (float): The desired gain value. min:0, max:27.0
+        wb (float): The desired white balance value. min:1.8, max:2.5
+        gamma (float): The desired gamma value. min:0.25 max:1.25
+        """
+        if self.camera:
+            if setting == "exposure":
+                self.camera.set_exposure(val)
+            elif setting == "gain":
+                self.camera.set_gain(val)
+            elif setting == "gamma":
+                self.camera.set_gamma(val)
+            elif setting == "wbRed":
+                self.camera.set_wb("Red", val)
+            elif setting == "wbBlue":
+                self.camera.set_wb("Blue", val)
+
+    def get_camera_setting(self, setting):
+        """Get the specified camera setting value.
+
+        Args:
+            setting (str): The camera setting to retrieve.
+                Possible values: "exposure", "gain", "gamma", "wbRed", "wbBlue".
+
+        Returns:
+            float: The value of the specified camera setting.
+        """
+        val = 0
+        if self.camera:
+            if setting == "exposure":
+                val = self.camera.get_exposure()
+            elif setting == "gain":
+                val = self.camera.get_gain()
+            elif setting == "gamma":
+                self.camera.disable_gamma()
+            elif setting == "wbRed":
+                val = self.camera.get_wb("Red")
+            elif setting == "wbBlue":
+                val = self.camera.get_wb("Blue")
+        return val
+
+    def get_camera_color_type(self):
+        """Get the color type of the camera.
+
+        Returns:
+            str: The color type of the camera.
+        """
+        if self.camera:
+            return self.camera.device_color_type
+
+    def image_clicked(self, event):
+        """
+        Handle the image click event.
+        """
+        if event.button() == QtCore.Qt.MouseButton.LeftButton:
+            self.select(event.pos())
+        elif event.button() == QtCore.Qt.MouseButton.MiddleButton:
+            self.zoom_out()
+
+    def select(self, pos):
+        """Select a position and emit the selected coordinates."""
+        self.click_target.setPos(pos)
+        self.click_target.setVisible(True)
+        self.selected.emit(*self.get_selected())
+
+    def select2(self, pos):
+        """Select a second position and make the click target visible."""
+        self.click_target2.setPos(pos)
+        self.click_target2.setVisible(True)
+
+    def zoom_out(self):
+        """
+        Zoom out the image. Fill the screen widget with the image.
+        """
+        self.view_box.autoRange()
+
+    def set_camera(self, camera):
+        """
+        Set the camera.
+        """
+        self.camera = camera
+        self.reticleDetector.set_name(self.get_camera_name())
+
+    def run_reticle_detection(self):
+        """Run reticle detection by stopping the filter and starting the reticle detector."""
+        logger.debug("run_reticle_detection")
+        self.filter.stop()
+        self.reticleDetector.start()
+
+    def run_probe_detection(self):
+        """Run probe detection by stopping the filter and starting the probe detector."""
+        logger.debug("run_probe_detection")
+        self.filter.stop()
+        self.probeDetector.start()
+
+    def run_no_filter(self):
+        """Run without any filter by stopping the reticle detector and probe detector."""
+        logger.debug("run_no_filter")
+        self.reticleDetector.stop()
+        self.probeDetector.stop()
+        self.filter.start()
+
+    def found_reticle_coords(self, x_coords, y_coords, mtx, dist):
+        """Store the found reticle coordinates, camera matrix, and distortion coefficients."""
+        self.reticle_coords = [x_coords, y_coords]
+        self.mtx = mtx
+        self.dist = dist
+
+    def reset_reticle_coords(self):
+        """Reset reticle coordinates."""
+        self.reticle_coords = None
+
+    def found_probe_coords(self, timestamp, probe_sn, stage_info, tip_coords):
+        """Store the found probe coordinates and related information."""
+        self.probe_detect_last_timestamp = timestamp
+        self.probe_detect_last_sn = probe_sn
+        self.stage_info = stage_info
+        self.probe_detect_last_coords = tip_coords
+
+    def get_last_detect_probe_info(self):
+        """Get the last detected probe information."""
+        return (
+            self.probe_detect_last_timestamp,
+            self.probe_detect_last_sn,
+            self.probe_detect_last_coords,
+        )
+
+    def get_camera_intrinsic(self):
+        """Get the camera intrinsic parameters."""
+        return self.mtx, self.dist
+
+    def get_reticle_coords(self):
+        """Get the reticle coordinates."""
+        return self.reticle_coords
+
+    def get_selected(self):
+        """
+        Return the selected target position.
+        """
+        if self.click_target.isVisible():
+            pos = self.click_target.pos()
+            return pos.x(), pos.y()
+        else:
+            return None, None
+
+    def wheelEvent(self, e):
+        """
+        Handle the mouse wheel event.
+        """
+        forward = bool(e.angleDelta().y() > 0)
+        control = bool(e.modifiers() & Qt.ControlModifier)
+        shift = bool(e.modifiers() & Qt.ShiftModifier)
+        if control:
+            if self.focochan:
+                foco, chan = self.focochan
+                dist = 20 if shift else 100
+                foco.time_move(chan, forward, dist, wait=True)
+        else:
+            super().wheelEvent(e)
+
+
+class ClickableImage(pg.ImageItem):
+    """This class captures mouse click events on images."""
+
+    mouse_clicked = pyqtSignal(object)
+
+    def mouseClickEvent(self, ev):
+        """
+        Handle the mouse click event.
+        """
+        super().mouseClickEvent(ev)
+        self.mouse_clicked.emit(ev)
```

### Comparing `parallax_app-0.37.1/parallax/stage_listener.py` & `parallax_app-0.37.5/parallax/stage_listener.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,454 +1,454 @@
-"""
-Provides classes to manage stage data fetching, representation, and updates in microscopy 
-applications, using PyQt5 for threading and signals, and requests for HTTP requests.
-"""
-
-import logging
-import time
-from collections import deque
-from datetime import datetime
-
-import numpy as np
-import requests
-from PyQt5.QtCore import QObject, QThread, QTimer, pyqtSignal
-
-# Set logger name
-logger = logging.getLogger(__name__)
-logger.setLevel(logging.DEBUG)
-# Set the logging level for PyQt5.uic.uiparser/properties to WARNING, to ignore DEBUG messages
-logging.getLogger("PyQt5.uic.uiparser").setLevel(logging.WARNING)
-logging.getLogger("PyQt5.uic.properties").setLevel(logging.WARNING)
-
-
-class StageInfo(QObject):
-    """Class for retrieving stage information."""
-
-    def __init__(self, url):
-        """Initialize StageInfo thread"""
-        super().__init__()
-        self.url = url
-        self.nStages = 0
-        self.stages_sn = []
-
-    def get_instances(self):
-        """Get the instances of the stages.
-
-        Returns:
-            list: List of stage instances.
-        """
-        stages = []
-        try:
-            response = requests.get(self.url, timeout=5)
-            if response.status_code == 200:
-                data = response.json()
-                self.nStages = data["Probes"]
-                for i in range(self.nStages):
-                    stage = data["ProbeArray"][i]
-                    self.stages_sn.append(stage["SerialNumber"])
-                    stages.append(stage)
-        except Exception as e:
-            print(f"\nHttpServer for stages not enabled: {e}")
-            print("* Trouble Shooting: ")
-            print("1. Check New Scale Stage connection.")
-            print("2. Enable Http Server: 'http://localhost:8080/'")
-            print("3. Click 'Connect' on New Scale SW")
-
-        return stages
-
-
-class Stage(QObject):
-    """Class representing a stage."""
-
-    def __init__(self, stage_info=None):
-        """Initialize Stage thread"""
-        QObject.__init__(self)
-        if stage_info is not None:
-            self.sn = stage_info["SerialNumber"]
-            self.name = stage_info["Id"]
-            self.stage_x = stage_info["Stage_X"] * 1000
-            self.stage_y = stage_info["Stage_Y"] * 1000
-            self.stage_z = stage_info["Stage_Z"] * 1000
-            self.stage_x_global = None
-            self.stage_y_global = None
-            self.stage_z_global = None
-
-
-class Worker(QObject):
-    """Worker class for fetching stage data."""
-
-    dataChanged = pyqtSignal(dict)
-    stage_moving = pyqtSignal(dict)
-    stage_not_moving = pyqtSignal(dict)
-
-    def __init__(self, url):
-        """Initialize worker thread"""
-        super().__init__()
-        self.url = url
-        self.timer = QTimer()
-        self.timer.timeout.connect(self.fetchData)
-        self.last_stage_info = None
-        self.last_bigmove_stage_info = None
-        self.last_bigmove_detected_time = None
-        self._low_freq_interval = 1000
-        self._high_freq_interval = 10  # TODO
-        self.curr_interval = self._low_freq_interval
-        self._idle_time = 2
-        self.is_error_log_printed = False
-
-    def start(self, interval=1000):
-        """Start the worker thread.
-
-        Args:
-            interval (int): Interval in milliseconds. Defaults to 1000.
-        """
-        self.timer.start(interval)
-
-    def stop(self):
-        """Stop the timer."""
-        self.timer.stop()
-
-    def print_trouble_shooting_msg(self):
-        """Print the troubleshooting message."""
-        print("Trouble Shooting: ")
-        print("1. Check New Scale Stage connection.")
-        print("2. Enable Http Server: 'http://localhost:8080/'")
-        print("3. Click 'Connect' on New Scale SW")
-
-    def fetchData(self):
-        """Fetches content from the URL and checks for significant changes."""
-        try:
-            response = requests.get(self.url, timeout=1)
-            if response.status_code == 200:
-                data = response.json()
-                if data["Probes"] == 0:
-                    if self.is_error_log_printed == False:
-                        self.is_error_log_printed = True
-                        print("\nStage is not connected to New Scale SW")
-                        self.print_trouble_shooting_msg()
-                else:
-                    selected_probe = data["SelectedProbe"]
-                    probe = data["ProbeArray"][selected_probe]
-
-                    if self.last_stage_info is None:  # Initial
-                        self.last_stage_info = probe
-                        self.last_bigmove_stage_info = probe
-                        self.dataChanged.emit(probe)
-
-                    if self.curr_interval == self._high_freq_interval:
-                        # Update
-                        self.isSmallChange(probe)
-                        # If last updated move (in 30um) is more than 1 sec ago, switch to w/ low freq
-                        current_time = time.time()
-                        if current_time - self.last_bigmove_detected_time >= self._idle_time:
-                            logger.debug("low freq mode")
-                            self.curr_interval = self._low_freq_interval
-                            self.stop()
-                            self.start(interval=self.curr_interval)
-                            self.stage_not_moving.emit(probe)
-
-                    # If moves more than 30um, check w/ high freq
-                    if self.isSignificantChange(probe):
-                        if self.curr_interval == self._low_freq_interval:
-                            # 10 msec mode
-                            logger.debug("high freq mode")
-                            self.curr_interval = self._high_freq_interval
-                            self.stop()
-                            self.start(interval=self.curr_interval)
-                            self.stage_moving.emit(probe)
-
-                    self.is_error_log_printed = False
-            else:
-                print(f"Failed to access {self.url}. Status code: {response.status_code}")
-        except Exception as e:
-            if self.is_error_log_printed == False:
-                self.is_error_log_printed = True
-                print(f"\nHttpServer for stages not enabled: {e}")
-                self.print_trouble_shooting_msg()
-
-    def isSignificantChange(self, current_stage_info, stage_threshold=0.005):
-        """Check if the change in any axis exceeds the threshold."""
-        for axis in ['Stage_X', 'Stage_Y', 'Stage_Z']:
-            if abs(current_stage_info[axis] - self.last_bigmove_stage_info[axis]) >= stage_threshold:
-                self.last_bigmove_detected_time = time.time()
-                self.last_bigmove_stage_info = current_stage_info
-                return True
-        return False
-
-    def isSmallChange(self, current_stage_info, stage_threshold=0.0005):
-        """Check if the change in any axis exceeds the threshold."""
-        for axis in ['Stage_X', 'Stage_Y', 'Stage_Z']:
-            if abs(current_stage_info[axis] - self.last_stage_info[axis]) >= stage_threshold:
-                self.dataChanged.emit(current_stage_info)
-                self.last_stage_info = current_stage_info
-                return True
-        return False
-
-
-class StageListener(QObject):
-    """Class for listening to stage updates."""
-
-    probeCalibRequest = pyqtSignal(QObject)
-
-    def __init__(self, model, stage_ui):
-        """Initialize Stage Listener object"""
-        super().__init__()
-        self.model = model
-        self.timestamp_local, self.timestamp_img_captured = None, None
-        self.worker = Worker(self.model.stage_listener_url)
-        self.thread = QThread()
-        self.stage_ui = stage_ui
-        self.thread.started.connect(self.worker.start)
-        self.worker.dataChanged.connect(self.handleDataChange)
-        self.worker.stage_moving.connect(self.stageMovingStatus)
-        self.worker.stage_not_moving.connect(self.stageNotMovingStatus)
-        self.buffer_size = 20
-        self.buffer_ts_local_coords = deque(maxlen=self.buffer_size)
-        self.stage_global_data = None
-        self.transM_dict = {}
-
-    def start(self):
-        """Start the stage listener."""
-        if self.model.nStages != 0:
-            self.worker.moveToThread(self.thread)
-            self.thread.start()
-
-    def get_last_moved_time(self, millisecond=False):
-        """Get the last moved time of the stage.
-
-        Args:
-            millisecond (bool): Include milliseconds in the timestamp. Defaults to False.
-
-        Returns:
-            str: Last moved time as a string.
-        """
-        ts = time.time()
-        dt = datetime.fromtimestamp(ts)
-        if millisecond:
-            return "%04d%02d%02d-%02d%02d%02d.%03d" % (
-                dt.year,
-                dt.month,
-                dt.day,
-                dt.hour,
-                dt.minute,
-                dt.second,
-                dt.microsecond // 1000,
-            )
-        else:
-            return "%04d%02d%02d-%02d%02d%02d" % (
-                dt.year,
-                dt.month,
-                dt.day,
-                dt.hour,
-                dt.minute,
-                dt.second,
-            )
-
-    def append_to_buffer(self, ts, stage):
-        """Append stage data to the buffer.
-
-        Args:
-            ts (str): Timestamp.
-            stage (Stage): Stage object.
-        """
-        self.buffer_ts_local_coords.append(
-            (ts, [stage.stage_x, stage.stage_y, stage.stage_z])
-        )
-
-    def handleDataChange(self, probe):
-        """Handle changes in stage data.
-
-        Args:
-            probe (dict): Probe data.
-        """
-        # Format the current timestamp
-        self.timestamp_local = self.get_last_moved_time(millisecond=True)
-
-        id = probe["Id"]
-        sn = probe["SerialNumber"]
-        local_coords_x = round(probe["Stage_X"] * 1000, 1)
-        local_coords_y = round(probe["Stage_Y"] * 1000, 1)
-        local_coords_z = round(probe["Stage_Z"] * 1000, 1)
-
-        # update into model
-        moving_stage = self.model.stages.get(sn)
-
-        if moving_stage is not None:
-            moving_stage.stage_x = local_coords_x
-            moving_stage.stage_y = local_coords_y
-            moving_stage.stage_z = local_coords_z
-
-        # Update to buffer
-        self.append_to_buffer(self.timestamp_local, moving_stage)
-
-        # Update into UI
-        if self.stage_ui.get_selected_stage_sn() == sn:
-            self.stage_ui.updateStageLocalCoords()
-        # logger.debug(sn, moving_stage.stage_x, self.stage_ui.get_selected_stage_sn())
-
-        if sn in self.transM_dict:
-            transM = self.transM_dict[sn]
-            if transM is not None:
-                self._updateGlobalDataTransformM(sn, moving_stage, transM)
-
-    def _updateGlobalDataTransformM(self, sn, moving_stage, transM):
-        """
-        Applies a transformation matrix to the local coordinates of a moving stage and updates its global coordinates.
-
-        Args:
-            sn (str): The serial number of the moving stage.
-            moving_stage (Stage): An object representing the moving stage, with attributes for its local and global coordinates.
-            transM (np.ndarray): A 4x4 numpy array representing the transformation matrix used to convert local coordinates
-                                to global coordinates.
-
-        Effects:
-            - Updates the moving_stage object's `stage_x_global`, `stage_y_global`, and `stage_z_global` attributes with the
-            transformed global coordinates.
-            - If the moving stage is the currently selected stage in the UI, triggers an update of the global coordinates display.
-        """
-        # Transform
-        local_point = np.array(
-            [
-                moving_stage.stage_x,
-                moving_stage.stage_y,
-                moving_stage.stage_z,
-                1,
-            ]
-        )
-        global_point = np.dot(transM, local_point)
-        global_point = np.around(global_point[:3], decimals=1)
-        logger.debug(f"_updateGlobalDataTransformM: {sn}, {global_point}")
-
-        # Update into UI
-        moving_stage.stage_x_global = global_point[0]
-        moving_stage.stage_y_global = global_point[1]
-        moving_stage.stage_z_global = global_point[2]
-        if self.stage_ui.get_selected_stage_sn() == sn:
-            self.stage_ui.updateStageGlobalCoords()
-
-    def requestUpdateGlobalDataTransformM(self, sn, transM):
-        """
-        Stores or updates a transformation matrix for a specific stage identified by its serial number.
-        This method updates an internal dictionary, `transM_dict`, mapping stage serial numbers to their
-        corresponding transformation matrices.
-
-        Args:
-            sn (str): The serial number of the stage.
-            transM (np.ndarray): A 4x4 numpy array representing the transformation matrix for the specified stage.
-        """
-        self.transM_dict[sn] = transM
-        logger.debug(f"requestUpdateGlobalDataTransformM {sn} {transM}")
-
-    def requestClearGlobalDataTransformM(self):
-        """
-        Clears all stored transformation matrices and resets the UI to default global coordinates.
-
-        Effects:
-            - Clears `transM_dict`, removing all stored transformation matrices.
-            - Triggers a UI update to reset the display of global coordinates to default values.
-        """
-        self.transM_dict = {}
-        self.stage_ui.updateStageGlobalCoords_default()
-        logger.debug(f"requestClearGlobalDataTransformM {self.transM_dict}")
-
-    def _change_time_format(self, str_time):
-        """Change the time format from string to datetime."""
-        fmt = "%Y%m%d-%H%M%S.%f"
-        date_time = datetime.strptime(str_time, fmt)
-        return date_time
-
-    def _find_closest_local_coords(self):
-        """Find the closest local coordinates based on the image capture timestamp.
-
-        Returns:
-            tuple: (closest_ts, closest_coords)
-                - closest_ts (str): Closest timestamp.
-                - closest_coords (list): Closest local coordinates.
-        """
-        closest_ts = None
-        closest_coords = None
-        # Initialize a variable to track the smallest time difference
-        # Use a large initial value
-        smallest_time_diff = float("inf")
-
-        for ts, local_coords in self.buffer_ts_local_coords:
-            ts_datetime = self._change_time_format(ts)
-            time_diff = (self.ts_img_captured - ts_datetime).total_seconds()
-
-            if time_diff < 0:
-                break
-
-            # Ensure we're not exceeding the global timestamp and the time difference is the smallest so far
-            if 0 <= time_diff < smallest_time_diff:
-                smallest_time_diff = time_diff
-                closest_ts = ts
-                closest_coords = local_coords
-
-        return closest_ts, closest_coords
-
-    def handleGlobalDataChange(self, sn, global_coords, ts_img_captured):
-        """Handle changes in global stage data.
-
-        Args:
-            sn (str): Serial number of the stage.
-            coords (list): Global coordinates.
-            ts_img_captured (str): Timestamp of the captured image.
-        """
-        self.ts_img_captured = self._change_time_format(ts_img_captured)
-        ts_local_coords, local_coords = self._find_closest_local_coords()
-
-        logger.debug(
-            f"\ntimestamp local:{ts_local_coords} img_captured:{ts_img_captured}"
-        )
-        global_coords_x = round(global_coords[0][0] * 1000, 1)
-        global_coords_y = round(global_coords[0][1] * 1000, 1)
-        global_coords_z = round(global_coords[0][2] * 1000, 1)
-
-        if self.stage_global_data is None:
-            stage_info = {}
-            stage_info["SerialNumber"] = sn
-            stage_info["Id"] = None
-            stage_info["Stage_X"] = local_coords[0]
-            stage_info["Stage_Y"] = local_coords[1]
-            stage_info["Stage_Z"] = local_coords[2]
-            self.stage_global_data = Stage(stage_info)
-
-        if local_coords is not None:
-            self.sn = sn
-            self.stage_global_data.sn = sn
-            self.stage_global_data.stage_x = local_coords[0]
-            self.stage_global_data.stage_y = local_coords[1]
-            self.stage_global_data.stage_z = local_coords[2]
-            self.stage_global_data.stage_x_global = global_coords_x
-            self.stage_global_data.stage_y_global = global_coords_y
-            self.stage_global_data.stage_z_global = global_coords_z
-
-            self.probeCalibRequest.emit(self.stage_global_data)
-
-            # Update into UI
-            moving_stage = self.model.stages.get(sn)
-            if moving_stage is not None:
-                moving_stage.stage_x_global = global_coords_x
-                moving_stage.stage_y_global = global_coords_y
-                moving_stage.stage_z_global = global_coords_z
-            if self.stage_ui.get_selected_stage_sn() == sn:
-                self.stage_ui.updateStageGlobalCoords()
-
-    def stageMovingStatus(self, probe):
-        """Handle stage moving status.
-
-        Args:
-            probe (dict): Probe data.
-        """
-        sn = probe["SerialNumber"]
-        for probeDetector in self.model.probeDetectors:
-            probeDetector.start_detection(sn)
-
-    def stageNotMovingStatus(self, probe):
-        """Handle not moving probe status.
-
-        Args:
-            probe (dict): Probe data.
-        """
-        sn = probe["SerialNumber"]
-        for probeDetector in self.model.probeDetectors:
+"""
+Provides classes to manage stage data fetching, representation, and updates in microscopy 
+applications, using PyQt5 for threading and signals, and requests for HTTP requests.
+"""
+
+import logging
+import time
+from collections import deque
+from datetime import datetime
+
+import numpy as np
+import requests
+from PyQt5.QtCore import QObject, QThread, QTimer, pyqtSignal
+
+# Set logger name
+logger = logging.getLogger(__name__)
+logger.setLevel(logging.DEBUG)
+# Set the logging level for PyQt5.uic.uiparser/properties to WARNING, to ignore DEBUG messages
+logging.getLogger("PyQt5.uic.uiparser").setLevel(logging.WARNING)
+logging.getLogger("PyQt5.uic.properties").setLevel(logging.WARNING)
+
+
+class StageInfo(QObject):
+    """Class for retrieving stage information."""
+
+    def __init__(self, url):
+        """Initialize StageInfo thread"""
+        super().__init__()
+        self.url = url
+        self.nStages = 0
+        self.stages_sn = []
+
+    def get_instances(self):
+        """Get the instances of the stages.
+
+        Returns:
+            list: List of stage instances.
+        """
+        stages = []
+        try:
+            response = requests.get(self.url, timeout=5)
+            if response.status_code == 200:
+                data = response.json()
+                self.nStages = data["Probes"]
+                for i in range(self.nStages):
+                    stage = data["ProbeArray"][i]
+                    self.stages_sn.append(stage["SerialNumber"])
+                    stages.append(stage)
+        except Exception as e:
+            print(f"\nHttpServer for stages not enabled: {e}")
+            print("* Trouble Shooting: ")
+            print("1. Check New Scale Stage connection.")
+            print("2. Enable Http Server: 'http://localhost:8080/'")
+            print("3. Click 'Connect' on New Scale SW")
+
+        return stages
+
+
+class Stage(QObject):
+    """Class representing a stage."""
+
+    def __init__(self, stage_info=None):
+        """Initialize Stage thread"""
+        QObject.__init__(self)
+        if stage_info is not None:
+            self.sn = stage_info["SerialNumber"]
+            self.name = stage_info["Id"]
+            self.stage_x = stage_info["Stage_X"] * 1000
+            self.stage_y = stage_info["Stage_Y"] * 1000
+            self.stage_z = stage_info["Stage_Z"] * 1000
+            self.stage_x_global = None
+            self.stage_y_global = None
+            self.stage_z_global = None
+
+
+class Worker(QObject):
+    """Worker class for fetching stage data."""
+
+    dataChanged = pyqtSignal(dict)
+    stage_moving = pyqtSignal(dict)
+    stage_not_moving = pyqtSignal(dict)
+
+    def __init__(self, url):
+        """Initialize worker thread"""
+        super().__init__()
+        self.url = url
+        self.timer = QTimer()
+        self.timer.timeout.connect(self.fetchData)
+        self.last_stage_info = None
+        self.last_bigmove_stage_info = None
+        self.last_bigmove_detected_time = None
+        self._low_freq_interval = 1000
+        self._high_freq_interval = 10  # TODO
+        self.curr_interval = self._low_freq_interval
+        self._idle_time = 2
+        self.is_error_log_printed = False
+
+    def start(self, interval=1000):
+        """Start the worker thread.
+
+        Args:
+            interval (int): Interval in milliseconds. Defaults to 1000.
+        """
+        self.timer.start(interval)
+
+    def stop(self):
+        """Stop the timer."""
+        self.timer.stop()
+
+    def print_trouble_shooting_msg(self):
+        """Print the troubleshooting message."""
+        print("Trouble Shooting: ")
+        print("1. Check New Scale Stage connection.")
+        print("2. Enable Http Server: 'http://localhost:8080/'")
+        print("3. Click 'Connect' on New Scale SW")
+
+    def fetchData(self):
+        """Fetches content from the URL and checks for significant changes."""
+        try:
+            response = requests.get(self.url, timeout=1)
+            if response.status_code == 200:
+                data = response.json()
+                if data["Probes"] == 0:
+                    if self.is_error_log_printed == False:
+                        self.is_error_log_printed = True
+                        print("\nStage is not connected to New Scale SW")
+                        self.print_trouble_shooting_msg()
+                else:
+                    selected_probe = data["SelectedProbe"]
+                    probe = data["ProbeArray"][selected_probe]
+
+                    if self.last_stage_info is None:  # Initial
+                        self.last_stage_info = probe
+                        self.last_bigmove_stage_info = probe
+                        self.dataChanged.emit(probe)
+
+                    if self.curr_interval == self._high_freq_interval:
+                        # Update
+                        self.isSmallChange(probe)
+                        # If last updated move (in 30um) is more than 1 sec ago, switch to w/ low freq
+                        current_time = time.time()
+                        if current_time - self.last_bigmove_detected_time >= self._idle_time:
+                            logger.debug("low freq mode")
+                            self.curr_interval = self._low_freq_interval
+                            self.stop()
+                            self.start(interval=self.curr_interval)
+                            self.stage_not_moving.emit(probe)
+
+                    # If moves more than 30um, check w/ high freq
+                    if self.isSignificantChange(probe):
+                        if self.curr_interval == self._low_freq_interval:
+                            # 10 msec mode
+                            logger.debug("high freq mode")
+                            self.curr_interval = self._high_freq_interval
+                            self.stop()
+                            self.start(interval=self.curr_interval)
+                            self.stage_moving.emit(probe)
+
+                    self.is_error_log_printed = False
+            else:
+                print(f"Failed to access {self.url}. Status code: {response.status_code}")
+        except Exception as e:
+            if self.is_error_log_printed == False:
+                self.is_error_log_printed = True
+                print(f"\nHttpServer for stages not enabled: {e}")
+                self.print_trouble_shooting_msg()
+
+    def isSignificantChange(self, current_stage_info, stage_threshold=0.005):
+        """Check if the change in any axis exceeds the threshold."""
+        for axis in ['Stage_X', 'Stage_Y', 'Stage_Z']:
+            if abs(current_stage_info[axis] - self.last_bigmove_stage_info[axis]) >= stage_threshold:
+                self.last_bigmove_detected_time = time.time()
+                self.last_bigmove_stage_info = current_stage_info
+                return True
+        return False
+
+    def isSmallChange(self, current_stage_info, stage_threshold=0.0005):
+        """Check if the change in any axis exceeds the threshold."""
+        for axis in ['Stage_X', 'Stage_Y', 'Stage_Z']:
+            if abs(current_stage_info[axis] - self.last_stage_info[axis]) >= stage_threshold:
+                self.dataChanged.emit(current_stage_info)
+                self.last_stage_info = current_stage_info
+                return True
+        return False
+
+
+class StageListener(QObject):
+    """Class for listening to stage updates."""
+
+    probeCalibRequest = pyqtSignal(QObject)
+
+    def __init__(self, model, stage_ui):
+        """Initialize Stage Listener object"""
+        super().__init__()
+        self.model = model
+        self.timestamp_local, self.timestamp_img_captured = None, None
+        self.worker = Worker(self.model.stage_listener_url)
+        self.thread = QThread()
+        self.stage_ui = stage_ui
+        self.thread.started.connect(self.worker.start)
+        self.worker.dataChanged.connect(self.handleDataChange)
+        self.worker.stage_moving.connect(self.stageMovingStatus)
+        self.worker.stage_not_moving.connect(self.stageNotMovingStatus)
+        self.buffer_size = 20
+        self.buffer_ts_local_coords = deque(maxlen=self.buffer_size)
+        self.stage_global_data = None
+        self.transM_dict = {}
+
+    def start(self):
+        """Start the stage listener."""
+        if self.model.nStages != 0:
+            self.worker.moveToThread(self.thread)
+            self.thread.start()
+
+    def get_last_moved_time(self, millisecond=False):
+        """Get the last moved time of the stage.
+
+        Args:
+            millisecond (bool): Include milliseconds in the timestamp. Defaults to False.
+
+        Returns:
+            str: Last moved time as a string.
+        """
+        ts = time.time()
+        dt = datetime.fromtimestamp(ts)
+        if millisecond:
+            return "%04d%02d%02d-%02d%02d%02d.%03d" % (
+                dt.year,
+                dt.month,
+                dt.day,
+                dt.hour,
+                dt.minute,
+                dt.second,
+                dt.microsecond // 1000,
+            )
+        else:
+            return "%04d%02d%02d-%02d%02d%02d" % (
+                dt.year,
+                dt.month,
+                dt.day,
+                dt.hour,
+                dt.minute,
+                dt.second,
+            )
+
+    def append_to_buffer(self, ts, stage):
+        """Append stage data to the buffer.
+
+        Args:
+            ts (str): Timestamp.
+            stage (Stage): Stage object.
+        """
+        self.buffer_ts_local_coords.append(
+            (ts, [stage.stage_x, stage.stage_y, stage.stage_z])
+        )
+
+    def handleDataChange(self, probe):
+        """Handle changes in stage data.
+
+        Args:
+            probe (dict): Probe data.
+        """
+        # Format the current timestamp
+        self.timestamp_local = self.get_last_moved_time(millisecond=True)
+
+        id = probe["Id"]
+        sn = probe["SerialNumber"]
+        local_coords_x = round(probe["Stage_X"] * 1000, 1)
+        local_coords_y = round(probe["Stage_Y"] * 1000, 1)
+        local_coords_z = round(probe["Stage_Z"] * 1000, 1)
+
+        # update into model
+        moving_stage = self.model.stages.get(sn)
+
+        if moving_stage is not None:
+            moving_stage.stage_x = local_coords_x
+            moving_stage.stage_y = local_coords_y
+            moving_stage.stage_z = local_coords_z
+
+        # Update to buffer
+        self.append_to_buffer(self.timestamp_local, moving_stage)
+
+        # Update into UI
+        if self.stage_ui.get_selected_stage_sn() == sn:
+            self.stage_ui.updateStageLocalCoords()
+        # logger.debug(sn, moving_stage.stage_x, self.stage_ui.get_selected_stage_sn())
+
+        if sn in self.transM_dict:
+            transM = self.transM_dict[sn]
+            if transM is not None:
+                self._updateGlobalDataTransformM(sn, moving_stage, transM)
+
+    def _updateGlobalDataTransformM(self, sn, moving_stage, transM):
+        """
+        Applies a transformation matrix to the local coordinates of a moving stage and updates its global coordinates.
+
+        Args:
+            sn (str): The serial number of the moving stage.
+            moving_stage (Stage): An object representing the moving stage, with attributes for its local and global coordinates.
+            transM (np.ndarray): A 4x4 numpy array representing the transformation matrix used to convert local coordinates
+                                to global coordinates.
+
+        Effects:
+            - Updates the moving_stage object's `stage_x_global`, `stage_y_global`, and `stage_z_global` attributes with the
+            transformed global coordinates.
+            - If the moving stage is the currently selected stage in the UI, triggers an update of the global coordinates display.
+        """
+        # Transform
+        local_point = np.array(
+            [
+                moving_stage.stage_x,
+                moving_stage.stage_y,
+                moving_stage.stage_z,
+                1,
+            ]
+        )
+        global_point = np.dot(transM, local_point)
+        global_point = np.around(global_point[:3], decimals=1)
+        logger.debug(f"_updateGlobalDataTransformM: {sn}, {global_point}")
+
+        # Update into UI
+        moving_stage.stage_x_global = global_point[0]
+        moving_stage.stage_y_global = global_point[1]
+        moving_stage.stage_z_global = global_point[2]
+        if self.stage_ui.get_selected_stage_sn() == sn:
+            self.stage_ui.updateStageGlobalCoords()
+
+    def requestUpdateGlobalDataTransformM(self, sn, transM):
+        """
+        Stores or updates a transformation matrix for a specific stage identified by its serial number.
+        This method updates an internal dictionary, `transM_dict`, mapping stage serial numbers to their
+        corresponding transformation matrices.
+
+        Args:
+            sn (str): The serial number of the stage.
+            transM (np.ndarray): A 4x4 numpy array representing the transformation matrix for the specified stage.
+        """
+        self.transM_dict[sn] = transM
+        logger.debug(f"requestUpdateGlobalDataTransformM {sn} {transM}")
+
+    def requestClearGlobalDataTransformM(self):
+        """
+        Clears all stored transformation matrices and resets the UI to default global coordinates.
+
+        Effects:
+            - Clears `transM_dict`, removing all stored transformation matrices.
+            - Triggers a UI update to reset the display of global coordinates to default values.
+        """
+        self.transM_dict = {}
+        self.stage_ui.updateStageGlobalCoords_default()
+        logger.debug(f"requestClearGlobalDataTransformM {self.transM_dict}")
+
+    def _change_time_format(self, str_time):
+        """Change the time format from string to datetime."""
+        fmt = "%Y%m%d-%H%M%S.%f"
+        date_time = datetime.strptime(str_time, fmt)
+        return date_time
+
+    def _find_closest_local_coords(self):
+        """Find the closest local coordinates based on the image capture timestamp.
+
+        Returns:
+            tuple: (closest_ts, closest_coords)
+                - closest_ts (str): Closest timestamp.
+                - closest_coords (list): Closest local coordinates.
+        """
+        closest_ts = None
+        closest_coords = None
+        # Initialize a variable to track the smallest time difference
+        # Use a large initial value
+        smallest_time_diff = float("inf")
+
+        for ts, local_coords in self.buffer_ts_local_coords:
+            ts_datetime = self._change_time_format(ts)
+            time_diff = (self.ts_img_captured - ts_datetime).total_seconds()
+
+            if time_diff < 0:
+                break
+
+            # Ensure we're not exceeding the global timestamp and the time difference is the smallest so far
+            if 0 <= time_diff < smallest_time_diff:
+                smallest_time_diff = time_diff
+                closest_ts = ts
+                closest_coords = local_coords
+
+        return closest_ts, closest_coords
+
+    def handleGlobalDataChange(self, sn, global_coords, ts_img_captured):
+        """Handle changes in global stage data.
+
+        Args:
+            sn (str): Serial number of the stage.
+            coords (list): Global coordinates.
+            ts_img_captured (str): Timestamp of the captured image.
+        """
+        self.ts_img_captured = self._change_time_format(ts_img_captured)
+        ts_local_coords, local_coords = self._find_closest_local_coords()
+
+        logger.debug(
+            f"\ntimestamp local:{ts_local_coords} img_captured:{ts_img_captured}"
+        )
+        global_coords_x = round(global_coords[0][0] * 1000, 1)
+        global_coords_y = round(global_coords[0][1] * 1000, 1)
+        global_coords_z = round(global_coords[0][2] * 1000, 1)
+
+        if self.stage_global_data is None:
+            stage_info = {}
+            stage_info["SerialNumber"] = sn
+            stage_info["Id"] = None
+            stage_info["Stage_X"] = local_coords[0]
+            stage_info["Stage_Y"] = local_coords[1]
+            stage_info["Stage_Z"] = local_coords[2]
+            self.stage_global_data = Stage(stage_info)
+
+        if local_coords is not None:
+            self.sn = sn
+            self.stage_global_data.sn = sn
+            self.stage_global_data.stage_x = local_coords[0]
+            self.stage_global_data.stage_y = local_coords[1]
+            self.stage_global_data.stage_z = local_coords[2]
+            self.stage_global_data.stage_x_global = global_coords_x
+            self.stage_global_data.stage_y_global = global_coords_y
+            self.stage_global_data.stage_z_global = global_coords_z
+
+            self.probeCalibRequest.emit(self.stage_global_data)
+
+            # Update into UI
+            moving_stage = self.model.stages.get(sn)
+            if moving_stage is not None:
+                moving_stage.stage_x_global = global_coords_x
+                moving_stage.stage_y_global = global_coords_y
+                moving_stage.stage_z_global = global_coords_z
+            if self.stage_ui.get_selected_stage_sn() == sn:
+                self.stage_ui.updateStageGlobalCoords()
+
+    def stageMovingStatus(self, probe):
+        """Handle stage moving status.
+
+        Args:
+            probe (dict): Probe data.
+        """
+        sn = probe["SerialNumber"]
+        for probeDetector in self.model.probeDetectors:
+            probeDetector.start_detection(sn)
+
+    def stageNotMovingStatus(self, probe):
+        """Handle not moving probe status.
+
+        Args:
+            probe (dict): Probe data.
+        """
+        sn = probe["SerialNumber"]
+        for probeDetector in self.model.probeDetectors:
             probeDetector.stop_detection(sn)
```

### Comparing `parallax_app-0.37.1/parallax/stage_ui.py` & `parallax_app-0.37.5/parallax/stage_ui.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,106 +1,106 @@
-"""
-Defines StageUI, a PyQt5 QWidget for showing and updating stage information in the UI, 
-including serial numbers and coordinates. It interacts with the model to reflect 
-real-time data changes.
-"""
-
-from PyQt5.QtWidgets import QWidget
-
-
-class StageUI(QWidget):
-    """User interface for stage control and display."""
-
-    def __init__(self, model, parent=None):
-        """Initialize StageUI object"""
-        QWidget.__init__(self, parent)
-        self.selected_stage = None
-        self.model = model
-        self.ui = parent
-        self.update_stage_selector()
-        self.updateStageSN()
-        self.updateStageLocalCoords()
-        self.updateStageGlobalCoords()
-
-        self.ui.stage_selector.currentIndexChanged.connect(self.updateStageSN)
-        self.ui.stage_selector.currentIndexChanged.connect(
-            self.updateStageLocalCoords
-        )
-        self.ui.stage_selector.currentIndexChanged.connect(
-            self.updateStageGlobalCoords
-        )
-
-    def get_selected_stage_sn(self):
-        """Get the serial number of the selected stage.
-
-        Returns:
-            str or None: The serial number of the selected stage, or None if no stage is selected.
-        """
-        if self.selected_stage is not None:
-            return self.selected_stage.sn
-        return None
-
-    def update_stage_selector(self):
-        """Update the stage selector with available stages."""
-        self.ui.stage_selector.clear()
-        for stage in self.model.stages.keys():
-            self.ui.stage_selector.addItem("Probe " + stage, stage)
-
-    def _get_current_stage_id(self):
-        """Get the ID of the currently selected stage.
-
-        Returns:
-            str or None: The ID of the currently selected stage, or None if no stage is selected.
-        """
-        currentIndex = self.ui.stage_selector.currentIndex()
-        stage_id = self.ui.stage_selector.itemData(currentIndex)
-        return stage_id
-
-    def updateStageSN(self):
-        """Update the displayed stage serial number."""
-        stage_id = self._get_current_stage_id()
-        if stage_id:
-            self.selected_stage = self.model.stages.get(stage_id)
-            if self.selected_stage:
-                self.ui.stage_sn.setText(" " + self.selected_stage.sn)
-
-    def updateStageLocalCoords(self):
-        """Update the displayed local coordinates of the selected stage."""
-        stage_id = self._get_current_stage_id()
-        if stage_id:
-            self.selected_stage = self.model.stages.get(stage_id)
-            if self.selected_stage:
-                self.ui.local_coords_x.setText(str(self.selected_stage.stage_x))
-                self.ui.local_coords_y.setText(str(self.selected_stage.stage_y))
-                self.ui.local_coords_z.setText(str(self.selected_stage.stage_z))
-
-    def updateStageGlobalCoords(self):
-        """Update the displayed global coordinates of the selected stage."""
-        stage_id = self._get_current_stage_id()
-        if stage_id:
-            self.selected_stage = self.model.stages.get(stage_id)
-            if self.selected_stage:
-                if self.selected_stage.stage_x_global is not None \
-                and self.selected_stage.stage_y_global is not None \
-                and self.selected_stage.stage_z_global is not None:
-                    self.ui.global_coords_x.setText(
-                        str(self.selected_stage.stage_x_global)
-                    )
-                    self.ui.global_coords_y.setText(
-                        str(self.selected_stage.stage_y_global)
-                    )
-                    self.ui.global_coords_z.setText(
-                        str(self.selected_stage.stage_z_global)
-                    )
-                else:
-                    self.updateStageGlobalCoords_default()
-
-    def updateStageGlobalCoords_default(self):
-        """
-        Resets the global coordinates displayed in the UI to default placeholders.
-
-        This method is used to clear the display of global coordinates in the user interface,
-        setting them back to a default placeholder value ('-').
-        """
-        self.ui.global_coords_x.setText("-")
-        self.ui.global_coords_y.setText("-")
-        self.ui.global_coords_z.setText("-")
+"""
+Defines StageUI, a PyQt5 QWidget for showing and updating stage information in the UI, 
+including serial numbers and coordinates. It interacts with the model to reflect 
+real-time data changes.
+"""
+
+from PyQt5.QtWidgets import QWidget
+
+
+class StageUI(QWidget):
+    """User interface for stage control and display."""
+
+    def __init__(self, model, parent=None):
+        """Initialize StageUI object"""
+        QWidget.__init__(self, parent)
+        self.selected_stage = None
+        self.model = model
+        self.ui = parent
+        self.update_stage_selector()
+        self.updateStageSN()
+        self.updateStageLocalCoords()
+        self.updateStageGlobalCoords()
+
+        self.ui.stage_selector.currentIndexChanged.connect(self.updateStageSN)
+        self.ui.stage_selector.currentIndexChanged.connect(
+            self.updateStageLocalCoords
+        )
+        self.ui.stage_selector.currentIndexChanged.connect(
+            self.updateStageGlobalCoords
+        )
+
+    def get_selected_stage_sn(self):
+        """Get the serial number of the selected stage.
+
+        Returns:
+            str or None: The serial number of the selected stage, or None if no stage is selected.
+        """
+        if self.selected_stage is not None:
+            return self.selected_stage.sn
+        return None
+
+    def update_stage_selector(self):
+        """Update the stage selector with available stages."""
+        self.ui.stage_selector.clear()
+        for stage in self.model.stages.keys():
+            self.ui.stage_selector.addItem("Probe " + stage, stage)
+
+    def _get_current_stage_id(self):
+        """Get the ID of the currently selected stage.
+
+        Returns:
+            str or None: The ID of the currently selected stage, or None if no stage is selected.
+        """
+        currentIndex = self.ui.stage_selector.currentIndex()
+        stage_id = self.ui.stage_selector.itemData(currentIndex)
+        return stage_id
+
+    def updateStageSN(self):
+        """Update the displayed stage serial number."""
+        stage_id = self._get_current_stage_id()
+        if stage_id:
+            self.selected_stage = self.model.stages.get(stage_id)
+            if self.selected_stage:
+                self.ui.stage_sn.setText(" " + self.selected_stage.sn)
+
+    def updateStageLocalCoords(self):
+        """Update the displayed local coordinates of the selected stage."""
+        stage_id = self._get_current_stage_id()
+        if stage_id:
+            self.selected_stage = self.model.stages.get(stage_id)
+            if self.selected_stage:
+                self.ui.local_coords_x.setText(str(self.selected_stage.stage_x))
+                self.ui.local_coords_y.setText(str(self.selected_stage.stage_y))
+                self.ui.local_coords_z.setText(str(self.selected_stage.stage_z))
+
+    def updateStageGlobalCoords(self):
+        """Update the displayed global coordinates of the selected stage."""
+        stage_id = self._get_current_stage_id()
+        if stage_id:
+            self.selected_stage = self.model.stages.get(stage_id)
+            if self.selected_stage:
+                if self.selected_stage.stage_x_global is not None \
+                and self.selected_stage.stage_y_global is not None \
+                and self.selected_stage.stage_z_global is not None:
+                    self.ui.global_coords_x.setText(
+                        str(self.selected_stage.stage_x_global)
+                    )
+                    self.ui.global_coords_y.setText(
+                        str(self.selected_stage.stage_y_global)
+                    )
+                    self.ui.global_coords_z.setText(
+                        str(self.selected_stage.stage_z_global)
+                    )
+                else:
+                    self.updateStageGlobalCoords_default()
+
+    def updateStageGlobalCoords_default(self):
+        """
+        Resets the global coordinates displayed in the UI to default placeholders.
+
+        This method is used to clear the display of global coordinates in the user interface,
+        setting them back to a default placeholder value ('-').
+        """
+        self.ui.global_coords_x.setText("-")
+        self.ui.global_coords_y.setText("-")
+        self.ui.global_coords_z.setText("-")
```

### Comparing `parallax_app-0.37.1/parallax/stage_widget.py` & `parallax_app-0.37.5/parallax/stage_widget.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,661 +1,661 @@
-"""
-This module contains the StageWidget class, which is a PyQt5 QWidget subclass for controlling 
-and calibrating stages in microscopy instruments. It interacts with the application's model 
-to manage calibration data and provides UI functionalities for reticle and probe detection, 
-and camera calibration. The class integrates with PyQt5 for the UI, handling UI loading, 
-initializing components, and linking user actions to calibration processes.
-"""
-
-import logging
-import os
-
-import numpy as np
-from PyQt5.QtCore import QTimer
-from PyQt5.QtWidgets import (QLabel, QMessageBox, QPushButton, QSizePolicy,
-                             QSpacerItem, QWidget)
-from PyQt5.uic import loadUi
-
-from .calibration_camera import CalibrationStereo
-from .probe_calibration import ProbeCalibration
-from .stage_listener import StageListener
-from .stage_ui import StageUI
-
-logger = logging.getLogger(__name__)
-logger.setLevel(logging.WARNING)
-
-
-class StageWidget(QWidget):
-    """Widget for stage control and calibration."""
-
-    def __init__(self, model, ui_dir, screen_widgets):
-        """Initializes the StageWidget instance.
-
-        Parameters:
-            model: The data model used for storing calibration and stage information.
-            ui_dir (str): The directory path where UI files are located.
-            screen_widgets (list): A list of ScreenWidget instances for reticle and probe detection.
-        """
-        super().__init__()
-        self.model = model
-        self.screen_widgets = screen_widgets
-        loadUi(os.path.join(ui_dir, "stage_info.ui"), self)
-        self.setMaximumWidth(380)
-
-        # Load reticle_calib.ui into its placeholder
-        self.reticle_calib_widget = QWidget()  # Create a new widget
-        loadUi(os.path.join(ui_dir, "reticle_calib.ui"), self.reticle_calib_widget)
-        # Assuming reticleCalibPlaceholder is the name of an empty widget designated as a placeholder in your stage_info.ui
-        self.stage_status_ui.layout().addWidget(self.reticle_calib_widget)  # Add it to the placeholder's layout
-        self.reticle_calib_widget.setMinimumSize(0, 160)
-
-        # Load probe_calib.ui into its placeholder
-        self.probe_calib_widget = QWidget()  # Create a new widget
-        loadUi(os.path.join(ui_dir, "probe_calib.ui"), self.probe_calib_widget)
-        # Assuming probeCalibPlaceholder is the name of an empty widget designated as a placeholder in your stage_info.ui
-        self.stage_status_ui.layout().addWidget(self.probe_calib_widget)  # Add it to the placeholder's layout
-        self.probe_calib_widget.setMinimumSize(0, 450) 
-        
-        # Create a vertical spacer with expanding policy
-        spacer = QSpacerItem(20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
-        # Add the spacer to the layout
-        self.stage_status_ui.addItem(spacer)
-
-        # Access probe_calibration_btn
-        self.probe_calibration_btn = self.probe_calib_widget.findChild(
-            QPushButton, "probe_calibration_btn"
-        )
-        self.reticle_calibration_btn = self.reticle_calib_widget.findChild(
-            QPushButton, "reticle_calibration_btn"
-        )
-        self.acceptButton = self.reticle_calib_widget.findChild(
-            QPushButton, "acceptButton"
-        )
-        self.rejectButton = self.reticle_calib_widget.findChild(
-            QPushButton, "rejectButton"
-        )
-        self.reticleCalibrationLabel = self.reticle_calib_widget.findChild(
-            QLabel, "reticleCalibResultLabel"
-        )
-        self.calib_x = self.probe_calib_widget.findChild(QPushButton, "calib_x")
-        self.calib_y = self.probe_calib_widget.findChild(QPushButton, "calib_y")
-        self.calib_z = self.probe_calib_widget.findChild(QPushButton, "calib_z")
-        self.probeCalibrationLabel = self.probe_calib_widget.findChild(
-            QLabel, "probeCalibrationLabel"
-        )
-
-        # Reticle Widget
-        self.reticle_detection_status = (
-            None  # options: default, process, detected, accepted
-        )
-        self.reticle_calibration_btn.clicked.connect(
-            self.reticle_detection_button_handler
-        )
-        self.calibrationStereo = None
-        # Hide Accept and Reject Button in Reticle Detection
-        self.acceptButton.hide()
-        self.rejectButton.hide()
-        self.acceptButton.clicked.connect(
-            self.reticle_detect_accept_detected_status
-        )
-        self.rejectButton.clicked.connect(self.reticle_detect_default_status)
-        # Add a QTimer for delayed check
-        self.reticle_calibration_timer = QTimer(self)
-        self.reticle_calibration_timer.timeout.connect(
-            self.reticle_detect_default_status
-        )
-
-        # Stage widget
-        self.stageUI = StageUI(self.model, self)
-        self.probe_calibration_btn.setEnabled(False)
-        self.probe_calibration_btn.clicked.connect(
-            self.probe_detection_button_handler
-        )
-        # Start refreshing stage info
-        self.stageListener = StageListener(self.model, self.stageUI)
-        self.stageListener.start()
-        self.probeCalibration = ProbeCalibration(self.stageListener)
-        # Hide X, Y, and Z Buttons in Probe Detection
-        self.calib_x.hide()
-        self.calib_y.hide()
-        self.calib_z.hide()
-        self.probeCalibration.calib_complete_x.connect(self.calib_x_complete)
-        self.probeCalibration.calib_complete_y.connect(self.calib_y_complete)
-        self.probeCalibration.calib_complete_z.connect(self.calib_z_complete)
-        self.probeCalibration.calib_complete.connect(
-            self.probe_detect_accepted_status
-        )
-        self.probeCalibration.transM_info.connect(
-            self.update_probe_calib_status
-        )
-        self.calib_status_x, self.calib_status_y, self.calib_status_z = False, False, False
-        self.probe_detection_status = None    # options: default, process, x_y_z_detected, accepted
-
-        self.filter = "no_filter"
-
-    def reticle_detection_button_handler(self):
-        """
-        Handles clicks on the reticle detection button, initiating or canceling reticle detection.
-        """
-        logger.debug(f"\n reticle_detection_button_handler {self.reticle_detection_status}")
-        if self.reticle_calibration_btn.isChecked():
-            # Run reticle detectoin
-            self.reticle_detect_process_status()
-        else:
-            if self.reticle_detection_status == "accepted":
-                response = self.overwrite_popup_window()
-                if response:
-                    # Overwrite the result
-                    self.reticle_detect_default_status()
-                else:
-                    # Keep the last calibration result
-                    self.reticle_calibration_btn.setChecked(True)
-
-    def reticle_detect_default_status(self):
-        """
-        Resets the reticle detection process to its default state and updates the UI accordingly.
-        """
-        # Enable reticle_calibration_btn button
-        if not self.reticle_calibration_btn.isEnabled():
-            self.reticle_calibration_btn.setEnabled(True)
-
-        if self.reticle_detection_status == "process":
-            self.reticle_detect_fail_popup_window()
-
-        # Stop reticle detectoin, and run no filter
-        self.reticle_calibration_timer.stop()
-
-        if self.reticle_detection_status != "accepted":
-            for screen in self.screen_widgets:
-                screen.reticle_coords_detected.disconnect(
-                    self.reticle_detect_all_screen
-                )
-                screen.run_no_filter()
-            self.filter = "no_filter"
-
-        # Hide Accept and Reject Button
-        self.acceptButton.hide()
-        self.rejectButton.hide()
-
-        self.reticle_calibration_btn.setStyleSheet(
-            """
-            QPushButton {
-                color: white;
-                background-color: black;
-            }
-            QPushButton:hover {
-                background-color: #641e1e;
-            }
-        """)
-        self.reticle_detection_status = "default"
-        self.reticleCalibrationLabel.setText("")
-        if self.probe_calibration_btn.isEnabled():
-            # Disable probe calibration
-            self.probe_detect_default_status()
-
-    def overwrite_popup_window(self):
-        """
-        Displays a confirmation dialog to decide whether to overwrite the current reticle position.
-
-        Returns:
-            bool: True if the user chooses to overwrite, False otherwise.
-        """
-        message = (
-            f"Are you sure you want to overwrite the current reticle position?"
-        )
-        response = QMessageBox.warning(
-            self,
-            "Reticle Detection Failed",
-            message,
-            QMessageBox.Yes | QMessageBox.No,
-            QMessageBox.No,
-        )
-
-        # Check which button was clicked
-        if response == QMessageBox.Yes:
-            logger.debug("User clicked Yes.")
-            return True
-        else:
-            logger.debug("User clicked No.")
-            return False
-
-    def reticle_detect_fail_popup_window(self):
-        """
-        Displays a warning dialog indicating the failure of reticle detection on one or more cameras.
-        """
-        coords_detect_fail_cameras = []
-        for screen in self.screen_widgets:
-            coords = screen.get_reticle_coords()
-            if coords is None:
-                camera_name = screen.get_camera_name()
-                coords_detect_fail_cameras.append(camera_name)
-
-        message = (
-            f"No reticle detected on cameras: {coords_detect_fail_cameras}"
-        )
-        QMessageBox.warning(self, "Reticle Detection Failed", message)
-
-    def reticle_detect_process_status(self):
-        """
-        Updates the UI and internal state to reflect that the reticle detection process is underway.
-        """
-        # Disable reticle_calibration_btn button
-        if self.reticle_calibration_btn.isEnabled():
-            self.reticle_calibration_btn.setEnabled(False)
-
-        # Run reticle detectoin
-        self.reticle_calibration_btn.setStyleSheet(
-            "color: gray;"
-            "background-color: #ffaaaa;"
-        )
-        for screen in self.screen_widgets:
-            screen.reset_reticle_coords()
-            screen.reticle_coords_detected.connect(
-                self.reticle_detect_all_screen
-            )
-            screen.run_reticle_detection()
-        self.filter = "reticle_detection"
-
-        # Hide Accept and Reject Button
-        self.acceptButton.hide()
-        self.rejectButton.hide()
-
-        # Start the timer for 10 seconds to check the status later
-        self.reticle_detection_status = "process"
-        self.reticle_calibration_timer.start(10000)
-        logger.debug(self.reticle_detection_status)
-
-    def reticle_detect_detected_status(self):
-        """
-        Updates the UI and internal state to reflect that the reticle has been detected.
-        """
-        # Found the coords
-        self.reticle_detection_status = "detected"
-        self.reticle_calibration_timer.stop()
-
-        # Show Accept and Reject Button
-        self.acceptButton.show()
-        self.rejectButton.show()
-
-        # Change the button to brown.
-        self.reticle_calibration_btn.setStyleSheet(
-            "color: white;"
-            "background-color: #bc9e44;"
-        )
-
-    def reticle_detect_accept_detected_status(self):
-        """
-        Finalizes the reticle detection process, accepting the detected reticle position and updating the UI accordingly.
-        """
-        self.reticle_detection_status = "accepted"
-
-        # Change the button to green.
-        self.reticle_calibration_btn.setStyleSheet(
-            "color: white;"
-            "background-color: #84c083;"
-        )
-        # Show Accept and Reject Button
-        self.acceptButton.hide()
-        self.rejectButton.hide()
-
-        result = self.calibrate_stereo()
-        if result:
-            self.reticleCalibrationLabel.setText(
-                f"<span style='color:green;'><small>Coords Reproj RMSE:<br></small>"
-                f"<span style='color:green;'>{result*1000:.1f} µm³</span>"
-            )
-
-        for screen in self.screen_widgets:
-            screen.reticle_coords_detected.disconnect(
-                self.reticle_detect_all_screen
-            )
-            screen.run_no_filter()
-        self.filter = "no_filter"
-
-        # Enable reticle_calibration_btn button
-        if not self.reticle_calibration_btn.isEnabled():
-            self.reticle_calibration_btn.setEnabled(True)
-        logger.debug(self.reticle_detection_status)
-
-        # Enable probe calibration
-        if not self.probe_calibration_btn.isEnabled():
-            self.probe_calibration_btn.setEnabled(True)
-
-    def calibrate_stereo(self):
-        """
-        Performs stereo calibration using the detected reticle positions and updates the model with the calibration data.
-        """
-        # Streo Camera Calibration
-        if len(self.model.coords_axis) >=2 and len(self.model.camera_intrinsic) >=2:
-            img_coords = []
-            intrinsics = []
-            cam_names = []
-
-            for screen in self.screen_widgets:
-                camera_name = screen.get_camera_name()
-                cam_names.append(camera_name)
-                img_coords.append(self.model.get_coords_axis(camera_name))
-                intrinsics.append(self.model.get_camera_intrinsic(camera_name))
-
-            if len(intrinsics) >= 2:
-                print("\n== intrinsics ==")
-                print(f" cam {cam_names[0]}:\n  {intrinsics[0]}")
-                print(f" cam {cam_names[1]}:\n  {intrinsics[1]}")
-
-            # TODO
-            self.calibrationStereo = CalibrationStereo(
-                cam_names[0],
-                img_coords[0],
-                intrinsics[0],
-                cam_names[1],
-                img_coords[1],
-                intrinsics[1],
-            )
-            retval, R_AB, T_AB, E_AB, F_AB = (
-                self.calibrationStereo.calibrate_stereo()
-            )
-            self.model.add_camera_extrinsic(
-                cam_names[0], cam_names[1], retval, R_AB, T_AB, E_AB, F_AB
-            )
-
-            # Test
-            err = self.calibrationStereo.test_performance(
-                cam_names[0], img_coords[0], cam_names[1], img_coords[1]
-            )
-            return err
-        else:
-            return None
-
-    def reticle_detect_all_screen(self):
-        """
-        Checks all screens for reticle detection results and updates the status based on whether the reticle
-        has been detected on all screens.
-        """
-        """Detect reticle coordinates on all screens."""
-        for screen in self.screen_widgets:
-            coords = screen.get_reticle_coords()
-            if coords is None:
-                return
-
-        # Found the coords
-        self.reticle_detect_detected_status()
-
-        # self.reticle_calibration_btn.setText("Confirm ?")
-        for screen in self.screen_widgets:
-            coords = screen.get_reticle_coords()
-            mtx, dist = screen.get_camera_intrinsic()
-            camera_name = screen.get_camera_name()
-            # Retister the reticle coords in the model
-            self.model.add_coords_axis(camera_name, coords)
-            self.model.add_camera_intrinsic(camera_name, mtx, dist)
-
-    def probe_detect_all_screen(self):
-        """Detect probe coordinates on all screens."""
-        timestamp_cmp, sn_cmp = None, None
-        cam_names = []
-        tip_coords = []
-
-        if self.calibrationStereo is None:
-            print("Camera calibration has not done")
-            return
-
-        for screen in self.screen_widgets:
-            timestamp, sn, tip_coord = screen.get_last_detect_probe_info()
-
-            if (sn is None) or (tip_coords is None) or (timestamp is None):
-                return
-
-            if timestamp_cmp is None:
-                timestamp_cmp = timestamp
-            else:  # if timestamp is different between screens, return
-                if timestamp_cmp[:-2] != timestamp[:-2]:
-                    return
-
-            if sn_cmp is None:
-                sn_cmp = sn
-            else:  # if sn is different between screens, return
-                if sn_cmp != sn:
-                    return
-
-            camera_name = screen.get_camera_name()
-            cam_names.append(camera_name)
-            tip_coords.append(tip_coord)
-
-        # All screen has the same timestamp. Proceed the triangulation
-        global_coords = self.calibrationStereo.get_global_coords(
-            cam_names[0], tip_coords[0], cam_names[1], tip_coords[1]
-        )
-        self.stageListener.handleGlobalDataChange(sn, global_coords, timestamp)
-
-    def probe_overwrite_popup_window(self):
-        """
-        Displays a confirmation dialog asking the user if they want to overwrite the current probe position.
-
-        Returns:
-            bool: True if the user confirms the overwrite, False otherwise.
-        """
-        message = (
-            f"Are you sure you want to overwrite the current probe position?"
-        )
-        response = QMessageBox.warning(
-            self,
-            "Reticle Detection Failed",
-            message,
-            QMessageBox.Yes | QMessageBox.No,
-            QMessageBox.No,
-        )
-
-        # Check which button was clicked
-        if response == QMessageBox.Yes:
-            logger.debug("User clicked Yes.")
-            return True
-        else:
-            logger.debug("User clicked No.")
-            return False
-
-    def probe_detection_button_handler(self):
-        """Handle the probe detection button click."""
-        if self.probe_calibration_btn.isChecked():
-            self.probe_detect_process_status()
-        else:
-            response = self.probe_overwrite_popup_window()
-            if response:
-                self.probe_detect_default_status()
-            else:
-                # Keep the last calibration result
-                self.probe_calibration_btn.setChecked(True)
-
-    def probe_detect_default_status(self):
-        """
-        Resets the probe detection status to its default state and updates the UI to reflect this change.
-        This method is called after completing or aborting the probe detection process.
-        """
-        self.probe_detection_status = "default"
-        self.probe_calibration_btn.setStyleSheet("""
-            QPushButton {
-                color: white;
-                background-color: black;
-            }
-            QPushButton:hover {
-                background-color: #641e1e;
-            }
-        """)
-        self.hide_x_y_z()
-        self.probeCalibrationLabel.setText("")
-        self.probeCalibration.reset_calib()
-        # self.reset_calib_status()
-
-        self.probe_calibration_btn.setChecked(False)
-        if self.reticle_detection_status == "default":
-            self.probe_calibration_btn.setEnabled(False)
-
-        if self.filter == "probe_detection":
-            for screen in self.screen_widgets:
-                screen.probe_coords_detected.disconnect(
-                    self.probe_detect_all_screen
-                )
-                screen.run_no_filter()
-
-            self.filter = "no_filter"
-            self.probeCalibration.clear()
-
-        # update global coords
-        self.stageListener.requestClearGlobalDataTransformM()
-
-    def probe_detect_process_status(self):
-        """
-        Updates the UI and internal state to reflect that the probe detection process is underway.
-        """
-        self.probe_detection_status = "process"
-        self.probe_calibration_btn.setStyleSheet(
-            "color: white;"
-            "background-color: #bc9e44;"
-        )
-        self.calib_x.show()
-        self.calib_y.show()
-        self.calib_z.show()
-
-        for screen in self.screen_widgets:
-            screen.probe_coords_detected.connect(self.probe_detect_all_screen)
-            screen.run_probe_detection()
-        self.filter = "probe_detection"
-
-        # message
-        message = f"Move probe at least 2mm along X, Y, and Z axes"
-        QMessageBox.information(self, "Probe calibration info", message)
-
-    def probe_detect_accepted_status(self, stage_sn, transformation_matrix):
-        """
-        Finalizes the probe detection process, accepting the detected probe position and updating the UI accordingly.
-        Additionally, it updates the model with the transformation matrix obtained from the calibration.
-
-        Parameters:
-            stage_sn (str): The serial number of the stage for which the probe position is accepted.
-            transformation_matrix (np.ndarray): The transformation matrix obtained from the probe calibration process.
-        """
-        self.probe_detection_status = "accepted"
-        self.probe_calibration_btn.setStyleSheet(
-            "color: white;"
-            "background-color: #84c083;"
-        )
-        self.hide_x_y_z()
-        if self.filter == "probe_detection":
-            for screen in self.screen_widgets:
-                screen.probe_coords_detected.disconnect(
-                    self.probe_detect_all_screen
-                )
-                screen.run_no_filter()
-
-            self.filter = "no_filter"
-
-        # update global coords
-        self.stageListener.requestUpdateGlobalDataTransformM(
-            stage_sn, transformation_matrix
-        )
-
-    def hide_x_y_z(self):
-        """
-        Hides the X, Y, and Z calibration buttons and updates their styles to indicate that the calibration for
-        each axis has been completed.
-        """
-        if self.calib_x.isVisible():
-            self.calib_x.hide()
-            # Change the button to green.
-            self.calib_x.setStyleSheet(
-            "color: white;"
-            "background-color: black;"
-        )
-        if self.calib_y.isVisible():
-            self.calib_y.hide()
-            # Change the button to green.
-            self.calib_y.setStyleSheet(
-            "color: white;"
-            "background-color: black;"
-        )
-        if self.calib_z.isVisible():
-            self.calib_z.hide()
-            # Change the button to green.
-            self.calib_z.setStyleSheet(
-            "color: white;"
-            "background-color: black;"
-        )
-            
-    def calib_x_complete(self):
-        """
-        Updates the UI to indicate that the calibration for the X-axis is complete.
-        """
-        if self.calib_x.isVisible():
-            # Change the button to green.
-            self.calib_x.setStyleSheet(
-            "color: white;"
-            "background-color: #84c083;"
-        )
-    
-    def calib_y_complete(self):
-        """
-        Updates the UI to indicate that the calibration for the Y-axis is complete.
-        """
-        if self.calib_y.isVisible():
-            # Change the button to green.
-            self.calib_y.setStyleSheet(
-            "color: white;"
-            "background-color: #84c083;"
-        )
-
-
-    def calib_z_complete(self):
-        """
-        Updates the UI to indicate that the calibration for the Z-axis is complete.
-        """
-        if self.calib_z.isVisible():
-            # Change the button to green.
-            self.calib_z.setStyleSheet(
-            "color: white;"
-            "background-color: #84c083;"
-        )
-
-    def update_probe_calib_status_transM(self, transformation_matrix):
-        # Extract the rotation matrix (top-left 3x3)
-        R = transformation_matrix[:3, :3]
-        # Extract the translation vector (top 3 elements of the last column)
-        T = transformation_matrix[:3, 3]
-
-        # Set the formatted string as the label's text
-        content = (
-            f"<span style='color:yellow;'><small>"
-            f"[Transformation Matrix]<br></small></span>"
-            f"<span style='color:green;'><small><b>R:</b><br>"
-            f" {R[0][0]:.5f}, {R[0][1]:.5f}, {R[0][2]:.5f},<br>"
-            f" {R[1][0]:.5f}, {R[1][1]:.5f}, {R[1][2]:.5f},<br>"
-            f" {R[2][0]:.5f}, {R[2][1]:.5f}, {R[2][2]:.5f},<br>"
-            f"<b>T:</b><br>"
-            f" {T[0]:.0f}, {T[1]:.0f}, {T[2]:.0f}<br>"
-            f"</small></span>"
-        )
-        return content
-
-    def update_probe_calib_status_L2(self, L2_err):
-        content = (
-            f"<span style='color:yellow;'><small>[L2 distance]<br></small></span>"
-            f"<span style='color:green;'><small> {L2_err:.3f}<br>"
-            f"</small></span>"
-        )
-        return content
-
-    def update_probe_calib_status_distance_traveled(self, dist_traveled):
-        x, y, z = dist_traveled[0], dist_traveled[1], dist_traveled[2]
-        content = (
-            f"<span style='color:yellow;'><small>[Distance traveled (µm)]<br></small></span>"
-            f"<span style='color:green;'><small>"
-            f"x: {x} y: {y} z: {z}<br>"
-            f"</small></span>"
-        )
-        return content
-
-    def update_probe_calib_status(self, transformation_matrix, L2_err, dist_traveled):
-        content_transM = self.update_probe_calib_status_transM(transformation_matrix)
-        content_L2 = self.update_probe_calib_status_L2(L2_err)
-        content_L2_travel = self.update_probe_calib_status_distance_traveled(dist_traveled)
-        # Ensure HTML content is properly combined
-        full_content = content_transM + content_L2 + content_L2_travel
-
-        self.probeCalibrationLabel.setText(full_content)
+"""
+This module contains the StageWidget class, which is a PyQt5 QWidget subclass for controlling 
+and calibrating stages in microscopy instruments. It interacts with the application's model 
+to manage calibration data and provides UI functionalities for reticle and probe detection, 
+and camera calibration. The class integrates with PyQt5 for the UI, handling UI loading, 
+initializing components, and linking user actions to calibration processes.
+"""
+
+import logging
+import os
+
+import numpy as np
+from PyQt5.QtCore import QTimer
+from PyQt5.QtWidgets import (QLabel, QMessageBox, QPushButton, QSizePolicy,
+                             QSpacerItem, QWidget)
+from PyQt5.uic import loadUi
+
+from .calibration_camera import CalibrationStereo
+from .probe_calibration import ProbeCalibration
+from .stage_listener import StageListener
+from .stage_ui import StageUI
+
+logger = logging.getLogger(__name__)
+logger.setLevel(logging.WARNING)
+
+
+class StageWidget(QWidget):
+    """Widget for stage control and calibration."""
+
+    def __init__(self, model, ui_dir, screen_widgets):
+        """Initializes the StageWidget instance.
+
+        Parameters:
+            model: The data model used for storing calibration and stage information.
+            ui_dir (str): The directory path where UI files are located.
+            screen_widgets (list): A list of ScreenWidget instances for reticle and probe detection.
+        """
+        super().__init__()
+        self.model = model
+        self.screen_widgets = screen_widgets
+        loadUi(os.path.join(ui_dir, "stage_info.ui"), self)
+        self.setMaximumWidth(380)
+
+        # Load reticle_calib.ui into its placeholder
+        self.reticle_calib_widget = QWidget()  # Create a new widget
+        loadUi(os.path.join(ui_dir, "reticle_calib.ui"), self.reticle_calib_widget)
+        # Assuming reticleCalibPlaceholder is the name of an empty widget designated as a placeholder in your stage_info.ui
+        self.stage_status_ui.layout().addWidget(self.reticle_calib_widget)  # Add it to the placeholder's layout
+        self.reticle_calib_widget.setMinimumSize(0, 160)
+
+        # Load probe_calib.ui into its placeholder
+        self.probe_calib_widget = QWidget()  # Create a new widget
+        loadUi(os.path.join(ui_dir, "probe_calib.ui"), self.probe_calib_widget)
+        # Assuming probeCalibPlaceholder is the name of an empty widget designated as a placeholder in your stage_info.ui
+        self.stage_status_ui.layout().addWidget(self.probe_calib_widget)  # Add it to the placeholder's layout
+        self.probe_calib_widget.setMinimumSize(0, 450) 
+        
+        # Create a vertical spacer with expanding policy
+        spacer = QSpacerItem(20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
+        # Add the spacer to the layout
+        self.stage_status_ui.addItem(spacer)
+
+        # Access probe_calibration_btn
+        self.probe_calibration_btn = self.probe_calib_widget.findChild(
+            QPushButton, "probe_calibration_btn"
+        )
+        self.reticle_calibration_btn = self.reticle_calib_widget.findChild(
+            QPushButton, "reticle_calibration_btn"
+        )
+        self.acceptButton = self.reticle_calib_widget.findChild(
+            QPushButton, "acceptButton"
+        )
+        self.rejectButton = self.reticle_calib_widget.findChild(
+            QPushButton, "rejectButton"
+        )
+        self.reticleCalibrationLabel = self.reticle_calib_widget.findChild(
+            QLabel, "reticleCalibResultLabel"
+        )
+        self.calib_x = self.probe_calib_widget.findChild(QPushButton, "calib_x")
+        self.calib_y = self.probe_calib_widget.findChild(QPushButton, "calib_y")
+        self.calib_z = self.probe_calib_widget.findChild(QPushButton, "calib_z")
+        self.probeCalibrationLabel = self.probe_calib_widget.findChild(
+            QLabel, "probeCalibrationLabel"
+        )
+
+        # Reticle Widget
+        self.reticle_detection_status = (
+            None  # options: default, process, detected, accepted
+        )
+        self.reticle_calibration_btn.clicked.connect(
+            self.reticle_detection_button_handler
+        )
+        self.calibrationStereo = None
+        # Hide Accept and Reject Button in Reticle Detection
+        self.acceptButton.hide()
+        self.rejectButton.hide()
+        self.acceptButton.clicked.connect(
+            self.reticle_detect_accept_detected_status
+        )
+        self.rejectButton.clicked.connect(self.reticle_detect_default_status)
+        # Add a QTimer for delayed check
+        self.reticle_calibration_timer = QTimer(self)
+        self.reticle_calibration_timer.timeout.connect(
+            self.reticle_detect_default_status
+        )
+
+        # Stage widget
+        self.stageUI = StageUI(self.model, self)
+        self.probe_calibration_btn.setEnabled(False)
+        self.probe_calibration_btn.clicked.connect(
+            self.probe_detection_button_handler
+        )
+        # Start refreshing stage info
+        self.stageListener = StageListener(self.model, self.stageUI)
+        self.stageListener.start()
+        self.probeCalibration = ProbeCalibration(self.stageListener)
+        # Hide X, Y, and Z Buttons in Probe Detection
+        self.calib_x.hide()
+        self.calib_y.hide()
+        self.calib_z.hide()
+        self.probeCalibration.calib_complete_x.connect(self.calib_x_complete)
+        self.probeCalibration.calib_complete_y.connect(self.calib_y_complete)
+        self.probeCalibration.calib_complete_z.connect(self.calib_z_complete)
+        self.probeCalibration.calib_complete.connect(
+            self.probe_detect_accepted_status
+        )
+        self.probeCalibration.transM_info.connect(
+            self.update_probe_calib_status
+        )
+        self.calib_status_x, self.calib_status_y, self.calib_status_z = False, False, False
+        self.probe_detection_status = None    # options: default, process, x_y_z_detected, accepted
+
+        self.filter = "no_filter"
+
+    def reticle_detection_button_handler(self):
+        """
+        Handles clicks on the reticle detection button, initiating or canceling reticle detection.
+        """
+        logger.debug(f"\n reticle_detection_button_handler {self.reticle_detection_status}")
+        if self.reticle_calibration_btn.isChecked():
+            # Run reticle detectoin
+            self.reticle_detect_process_status()
+        else:
+            if self.reticle_detection_status == "accepted":
+                response = self.overwrite_popup_window()
+                if response:
+                    # Overwrite the result
+                    self.reticle_detect_default_status()
+                else:
+                    # Keep the last calibration result
+                    self.reticle_calibration_btn.setChecked(True)
+
+    def reticle_detect_default_status(self):
+        """
+        Resets the reticle detection process to its default state and updates the UI accordingly.
+        """
+        # Enable reticle_calibration_btn button
+        if not self.reticle_calibration_btn.isEnabled():
+            self.reticle_calibration_btn.setEnabled(True)
+
+        if self.reticle_detection_status == "process":
+            self.reticle_detect_fail_popup_window()
+
+        # Stop reticle detectoin, and run no filter
+        self.reticle_calibration_timer.stop()
+
+        if self.reticle_detection_status != "accepted":
+            for screen in self.screen_widgets:
+                screen.reticle_coords_detected.disconnect(
+                    self.reticle_detect_all_screen
+                )
+                screen.run_no_filter()
+            self.filter = "no_filter"
+
+        # Hide Accept and Reject Button
+        self.acceptButton.hide()
+        self.rejectButton.hide()
+
+        self.reticle_calibration_btn.setStyleSheet(
+            """
+            QPushButton {
+                color: white;
+                background-color: black;
+            }
+            QPushButton:hover {
+                background-color: #641e1e;
+            }
+        """)
+        self.reticle_detection_status = "default"
+        self.reticleCalibrationLabel.setText("")
+        if self.probe_calibration_btn.isEnabled():
+            # Disable probe calibration
+            self.probe_detect_default_status()
+
+    def overwrite_popup_window(self):
+        """
+        Displays a confirmation dialog to decide whether to overwrite the current reticle position.
+
+        Returns:
+            bool: True if the user chooses to overwrite, False otherwise.
+        """
+        message = (
+            f"Are you sure you want to overwrite the current reticle position?"
+        )
+        response = QMessageBox.warning(
+            self,
+            "Reticle Detection Failed",
+            message,
+            QMessageBox.Yes | QMessageBox.No,
+            QMessageBox.No,
+        )
+
+        # Check which button was clicked
+        if response == QMessageBox.Yes:
+            logger.debug("User clicked Yes.")
+            return True
+        else:
+            logger.debug("User clicked No.")
+            return False
+
+    def reticle_detect_fail_popup_window(self):
+        """
+        Displays a warning dialog indicating the failure of reticle detection on one or more cameras.
+        """
+        coords_detect_fail_cameras = []
+        for screen in self.screen_widgets:
+            coords = screen.get_reticle_coords()
+            if coords is None:
+                camera_name = screen.get_camera_name()
+                coords_detect_fail_cameras.append(camera_name)
+
+        message = (
+            f"No reticle detected on cameras: {coords_detect_fail_cameras}"
+        )
+        QMessageBox.warning(self, "Reticle Detection Failed", message)
+
+    def reticle_detect_process_status(self):
+        """
+        Updates the UI and internal state to reflect that the reticle detection process is underway.
+        """
+        # Disable reticle_calibration_btn button
+        if self.reticle_calibration_btn.isEnabled():
+            self.reticle_calibration_btn.setEnabled(False)
+
+        # Run reticle detectoin
+        self.reticle_calibration_btn.setStyleSheet(
+            "color: gray;"
+            "background-color: #ffaaaa;"
+        )
+        for screen in self.screen_widgets:
+            screen.reset_reticle_coords()
+            screen.reticle_coords_detected.connect(
+                self.reticle_detect_all_screen
+            )
+            screen.run_reticle_detection()
+        self.filter = "reticle_detection"
+
+        # Hide Accept and Reject Button
+        self.acceptButton.hide()
+        self.rejectButton.hide()
+
+        # Start the timer for 10 seconds to check the status later
+        self.reticle_detection_status = "process"
+        self.reticle_calibration_timer.start(10000)
+        logger.debug(self.reticle_detection_status)
+
+    def reticle_detect_detected_status(self):
+        """
+        Updates the UI and internal state to reflect that the reticle has been detected.
+        """
+        # Found the coords
+        self.reticle_detection_status = "detected"
+        self.reticle_calibration_timer.stop()
+
+        # Show Accept and Reject Button
+        self.acceptButton.show()
+        self.rejectButton.show()
+
+        # Change the button to brown.
+        self.reticle_calibration_btn.setStyleSheet(
+            "color: white;"
+            "background-color: #bc9e44;"
+        )
+
+    def reticle_detect_accept_detected_status(self):
+        """
+        Finalizes the reticle detection process, accepting the detected reticle position and updating the UI accordingly.
+        """
+        self.reticle_detection_status = "accepted"
+
+        # Change the button to green.
+        self.reticle_calibration_btn.setStyleSheet(
+            "color: white;"
+            "background-color: #84c083;"
+        )
+        # Show Accept and Reject Button
+        self.acceptButton.hide()
+        self.rejectButton.hide()
+
+        result = self.calibrate_stereo()
+        if result:
+            self.reticleCalibrationLabel.setText(
+                f"<span style='color:green;'><small>Coords Reproj RMSE:<br></small>"
+                f"<span style='color:green;'>{result*1000:.1f} µm³</span>"
+            )
+
+        for screen in self.screen_widgets:
+            screen.reticle_coords_detected.disconnect(
+                self.reticle_detect_all_screen
+            )
+            screen.run_no_filter()
+        self.filter = "no_filter"
+
+        # Enable reticle_calibration_btn button
+        if not self.reticle_calibration_btn.isEnabled():
+            self.reticle_calibration_btn.setEnabled(True)
+        logger.debug(self.reticle_detection_status)
+
+        # Enable probe calibration
+        if not self.probe_calibration_btn.isEnabled():
+            self.probe_calibration_btn.setEnabled(True)
+
+    def calibrate_stereo(self):
+        """
+        Performs stereo calibration using the detected reticle positions and updates the model with the calibration data.
+        """
+        # Streo Camera Calibration
+        if len(self.model.coords_axis) >=2 and len(self.model.camera_intrinsic) >=2:
+            img_coords = []
+            intrinsics = []
+            cam_names = []
+
+            for screen in self.screen_widgets:
+                camera_name = screen.get_camera_name()
+                cam_names.append(camera_name)
+                img_coords.append(self.model.get_coords_axis(camera_name))
+                intrinsics.append(self.model.get_camera_intrinsic(camera_name))
+
+            if len(intrinsics) >= 2:
+                print("\n== intrinsics ==")
+                print(f" cam {cam_names[0]}:\n  {intrinsics[0]}")
+                print(f" cam {cam_names[1]}:\n  {intrinsics[1]}")
+
+            # TODO
+            self.calibrationStereo = CalibrationStereo(
+                cam_names[0],
+                img_coords[0],
+                intrinsics[0],
+                cam_names[1],
+                img_coords[1],
+                intrinsics[1],
+            )
+            retval, R_AB, T_AB, E_AB, F_AB = (
+                self.calibrationStereo.calibrate_stereo()
+            )
+            self.model.add_camera_extrinsic(
+                cam_names[0], cam_names[1], retval, R_AB, T_AB, E_AB, F_AB
+            )
+
+            # Test
+            err = self.calibrationStereo.test_performance(
+                cam_names[0], img_coords[0], cam_names[1], img_coords[1]
+            )
+            return err
+        else:
+            return None
+
+    def reticle_detect_all_screen(self):
+        """
+        Checks all screens for reticle detection results and updates the status based on whether the reticle
+        has been detected on all screens.
+        """
+        """Detect reticle coordinates on all screens."""
+        for screen in self.screen_widgets:
+            coords = screen.get_reticle_coords()
+            if coords is None:
+                return
+
+        # Found the coords
+        self.reticle_detect_detected_status()
+
+        # self.reticle_calibration_btn.setText("Confirm ?")
+        for screen in self.screen_widgets:
+            coords = screen.get_reticle_coords()
+            mtx, dist = screen.get_camera_intrinsic()
+            camera_name = screen.get_camera_name()
+            # Retister the reticle coords in the model
+            self.model.add_coords_axis(camera_name, coords)
+            self.model.add_camera_intrinsic(camera_name, mtx, dist)
+
+    def probe_detect_all_screen(self):
+        """Detect probe coordinates on all screens."""
+        timestamp_cmp, sn_cmp = None, None
+        cam_names = []
+        tip_coords = []
+
+        if self.calibrationStereo is None:
+            print("Camera calibration has not done")
+            return
+
+        for screen in self.screen_widgets:
+            timestamp, sn, tip_coord = screen.get_last_detect_probe_info()
+
+            if (sn is None) or (tip_coords is None) or (timestamp is None):
+                return
+
+            if timestamp_cmp is None:
+                timestamp_cmp = timestamp
+            else:  # if timestamp is different between screens, return
+                if timestamp_cmp[:-2] != timestamp[:-2]:
+                    return
+
+            if sn_cmp is None:
+                sn_cmp = sn
+            else:  # if sn is different between screens, return
+                if sn_cmp != sn:
+                    return
+
+            camera_name = screen.get_camera_name()
+            cam_names.append(camera_name)
+            tip_coords.append(tip_coord)
+
+        # All screen has the same timestamp. Proceed the triangulation
+        global_coords = self.calibrationStereo.get_global_coords(
+            cam_names[0], tip_coords[0], cam_names[1], tip_coords[1]
+        )
+        self.stageListener.handleGlobalDataChange(sn, global_coords, timestamp)
+
+    def probe_overwrite_popup_window(self):
+        """
+        Displays a confirmation dialog asking the user if they want to overwrite the current probe position.
+
+        Returns:
+            bool: True if the user confirms the overwrite, False otherwise.
+        """
+        message = (
+            f"Are you sure you want to overwrite the current probe position?"
+        )
+        response = QMessageBox.warning(
+            self,
+            "Reticle Detection Failed",
+            message,
+            QMessageBox.Yes | QMessageBox.No,
+            QMessageBox.No,
+        )
+
+        # Check which button was clicked
+        if response == QMessageBox.Yes:
+            logger.debug("User clicked Yes.")
+            return True
+        else:
+            logger.debug("User clicked No.")
+            return False
+
+    def probe_detection_button_handler(self):
+        """Handle the probe detection button click."""
+        if self.probe_calibration_btn.isChecked():
+            self.probe_detect_process_status()
+        else:
+            response = self.probe_overwrite_popup_window()
+            if response:
+                self.probe_detect_default_status()
+            else:
+                # Keep the last calibration result
+                self.probe_calibration_btn.setChecked(True)
+
+    def probe_detect_default_status(self):
+        """
+        Resets the probe detection status to its default state and updates the UI to reflect this change.
+        This method is called after completing or aborting the probe detection process.
+        """
+        self.probe_detection_status = "default"
+        self.probe_calibration_btn.setStyleSheet("""
+            QPushButton {
+                color: white;
+                background-color: black;
+            }
+            QPushButton:hover {
+                background-color: #641e1e;
+            }
+        """)
+        self.hide_x_y_z()
+        self.probeCalibrationLabel.setText("")
+        self.probeCalibration.reset_calib()
+        # self.reset_calib_status()
+
+        self.probe_calibration_btn.setChecked(False)
+        if self.reticle_detection_status == "default":
+            self.probe_calibration_btn.setEnabled(False)
+
+        if self.filter == "probe_detection":
+            for screen in self.screen_widgets:
+                screen.probe_coords_detected.disconnect(
+                    self.probe_detect_all_screen
+                )
+                screen.run_no_filter()
+
+            self.filter = "no_filter"
+            self.probeCalibration.clear()
+
+        # update global coords
+        self.stageListener.requestClearGlobalDataTransformM()
+
+    def probe_detect_process_status(self):
+        """
+        Updates the UI and internal state to reflect that the probe detection process is underway.
+        """
+        self.probe_detection_status = "process"
+        self.probe_calibration_btn.setStyleSheet(
+            "color: white;"
+            "background-color: #bc9e44;"
+        )
+        self.calib_x.show()
+        self.calib_y.show()
+        self.calib_z.show()
+
+        for screen in self.screen_widgets:
+            screen.probe_coords_detected.connect(self.probe_detect_all_screen)
+            screen.run_probe_detection()
+        self.filter = "probe_detection"
+
+        # message
+        message = f"Move probe at least 2mm along X, Y, and Z axes"
+        QMessageBox.information(self, "Probe calibration info", message)
+
+    def probe_detect_accepted_status(self, stage_sn, transformation_matrix):
+        """
+        Finalizes the probe detection process, accepting the detected probe position and updating the UI accordingly.
+        Additionally, it updates the model with the transformation matrix obtained from the calibration.
+
+        Parameters:
+            stage_sn (str): The serial number of the stage for which the probe position is accepted.
+            transformation_matrix (np.ndarray): The transformation matrix obtained from the probe calibration process.
+        """
+        self.probe_detection_status = "accepted"
+        self.probe_calibration_btn.setStyleSheet(
+            "color: white;"
+            "background-color: #84c083;"
+        )
+        self.hide_x_y_z()
+        if self.filter == "probe_detection":
+            for screen in self.screen_widgets:
+                screen.probe_coords_detected.disconnect(
+                    self.probe_detect_all_screen
+                )
+                screen.run_no_filter()
+
+            self.filter = "no_filter"
+
+        # update global coords
+        self.stageListener.requestUpdateGlobalDataTransformM(
+            stage_sn, transformation_matrix
+        )
+
+    def hide_x_y_z(self):
+        """
+        Hides the X, Y, and Z calibration buttons and updates their styles to indicate that the calibration for
+        each axis has been completed.
+        """
+        if self.calib_x.isVisible():
+            self.calib_x.hide()
+            # Change the button to green.
+            self.calib_x.setStyleSheet(
+            "color: white;"
+            "background-color: black;"
+        )
+        if self.calib_y.isVisible():
+            self.calib_y.hide()
+            # Change the button to green.
+            self.calib_y.setStyleSheet(
+            "color: white;"
+            "background-color: black;"
+        )
+        if self.calib_z.isVisible():
+            self.calib_z.hide()
+            # Change the button to green.
+            self.calib_z.setStyleSheet(
+            "color: white;"
+            "background-color: black;"
+        )
+            
+    def calib_x_complete(self):
+        """
+        Updates the UI to indicate that the calibration for the X-axis is complete.
+        """
+        if self.calib_x.isVisible():
+            # Change the button to green.
+            self.calib_x.setStyleSheet(
+            "color: white;"
+            "background-color: #84c083;"
+        )
+    
+    def calib_y_complete(self):
+        """
+        Updates the UI to indicate that the calibration for the Y-axis is complete.
+        """
+        if self.calib_y.isVisible():
+            # Change the button to green.
+            self.calib_y.setStyleSheet(
+            "color: white;"
+            "background-color: #84c083;"
+        )
+
+
+    def calib_z_complete(self):
+        """
+        Updates the UI to indicate that the calibration for the Z-axis is complete.
+        """
+        if self.calib_z.isVisible():
+            # Change the button to green.
+            self.calib_z.setStyleSheet(
+            "color: white;"
+            "background-color: #84c083;"
+        )
+
+    def update_probe_calib_status_transM(self, transformation_matrix):
+        # Extract the rotation matrix (top-left 3x3)
+        R = transformation_matrix[:3, :3]
+        # Extract the translation vector (top 3 elements of the last column)
+        T = transformation_matrix[:3, 3]
+
+        # Set the formatted string as the label's text
+        content = (
+            f"<span style='color:yellow;'><small>"
+            f"[Transformation Matrix]<br></small></span>"
+            f"<span style='color:green;'><small><b>R:</b><br>"
+            f" {R[0][0]:.5f}, {R[0][1]:.5f}, {R[0][2]:.5f},<br>"
+            f" {R[1][0]:.5f}, {R[1][1]:.5f}, {R[1][2]:.5f},<br>"
+            f" {R[2][0]:.5f}, {R[2][1]:.5f}, {R[2][2]:.5f},<br>"
+            f"<b>T:</b><br>"
+            f" {T[0]:.0f}, {T[1]:.0f}, {T[2]:.0f}<br>"
+            f"</small></span>"
+        )
+        return content
+
+    def update_probe_calib_status_L2(self, L2_err):
+        content = (
+            f"<span style='color:yellow;'><small>[L2 distance]<br></small></span>"
+            f"<span style='color:green;'><small> {L2_err:.3f}<br>"
+            f"</small></span>"
+        )
+        return content
+
+    def update_probe_calib_status_distance_traveled(self, dist_traveled):
+        x, y, z = dist_traveled[0], dist_traveled[1], dist_traveled[2]
+        content = (
+            f"<span style='color:yellow;'><small>[Distance traveled (µm)]<br></small></span>"
+            f"<span style='color:green;'><small>"
+            f"x: {x} y: {y} z: {z}<br>"
+            f"</small></span>"
+        )
+        return content
+
+    def update_probe_calib_status(self, transformation_matrix, L2_err, dist_traveled):
+        content_transM = self.update_probe_calib_status_transM(transformation_matrix)
+        content_L2 = self.update_probe_calib_status_L2(L2_err)
+        content_L2_travel = self.update_probe_calib_status_distance_traveled(dist_traveled)
+        # Ensure HTML content is properly combined
+        full_content = content_transM + content_L2 + content_L2_travel
+
+        self.probeCalibrationLabel.setText(full_content)
```

### Comparing `parallax_app-0.37.1/parallax/utils.py` & `parallax_app-0.37.5/parallax/utils.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,91 +1,91 @@
-"""
-This module provides utility classes for manipulating coordinates and calculating
-crop regions within images. 
-- UtilsCoords: scaling coordinates between original and resized images
-- UtilsCrops: calculating crop regions based on specified criteria.
-"""
-
-
-class UtilsCoords:
-    """Utility class for coordinate scaling."""
-
-    def __init__(self, original_size, resized_size):
-        """Initialize the UtilsCoords object.
-
-        Args:
-            original_size (tuple): Original size of the image (width, height).
-            resized_size (tuple): Resized size of the image (width, height).
-        """
-        self.original_size = original_size
-        self.resized_size = resized_size
-
-    def scale_coords_to_original(self, tip):
-        """Scale coordinates from resized image to original image.
-
-        Args:
-            tip (tuple): Coordinates of the tip (x, y) in the resized image.
-
-        Returns:
-            tuple: Scaled coordinates of the tip (x, y) in the original image.
-        """
-        x, y = tip
-        original_width, original_height = self.original_size
-        resized_width, resized_height = self.resized_size
-
-        scale_x = original_width / resized_width
-        scale_y = original_height / resized_height
-
-        original_x = int(x * scale_x)
-        original_y = int(y * scale_y)
-
-        return original_x, original_y
-
-
-class UtilsCrops:
-    """Utility class for calculating crop regions."""
-
-    def __init__(self):
-        """Initialize the UtilsCrops object."""
-        pass
-
-    def calculate_crop_region(self, tip, base, crop_size, IMG_SIZE):
-        """Calculate the crop region based on tip and base coordinates.
-
-        Args:
-            tip (tuple): Coordinates of the tip (x, y).
-            base (tuple): Coordinates of the base (x, y).
-            crop_size (int): Size of the crop region.
-            IMG_SIZE (tuple): Size of the image (width, height).
-
-        Returns:
-            tuple: Crop region coordinates (top, bottom, left, right).
-        """
-        tip_x, tip_y = tip
-        base_x, base_y = base
-        top = max(min(tip_y, base_y) - crop_size, 0)
-        bottom = min(max(tip_y, base_y) + crop_size, IMG_SIZE[1])
-        left = max(min(tip_x, base_x) - crop_size, 0)
-        right = min(max(tip_x, base_x) + crop_size, IMG_SIZE[0])
-        return top, bottom, left, right
-
-    def is_point_on_crop_region(self, point, top, bottom, left, right, buffer=5):
-        """Check if a point is on the crop region boundary.
-
-        Args:
-            point (tuple): Coordinates of the point (x, y).
-            top (int): Top coordinate of the crop region.
-            bottom (int): Bottom coordinate of the crop region.
-            left (int): Left coordinate of the crop region.
-            right (int): Right coordinate of the crop region.
-            buffer (int): Buffer size around the crop region boundary. Defaults to 5.
-
-        Returns:
-            bool: True if the point is on the crop region boundary, False otherwise.
-        """
-        x, y = point
-        return (
-            (top - buffer <= y <= top + buffer)
-            or (bottom - buffer <= y <= bottom + buffer)
-            or (left - buffer <= x <= left + buffer)
-            or (right - buffer <= x <= right + buffer)
-        )
+"""
+This module provides utility classes for manipulating coordinates and calculating
+crop regions within images. 
+- UtilsCoords: scaling coordinates between original and resized images
+- UtilsCrops: calculating crop regions based on specified criteria.
+"""
+
+
+class UtilsCoords:
+    """Utility class for coordinate scaling."""
+
+    def __init__(self, original_size, resized_size):
+        """Initialize the UtilsCoords object.
+
+        Args:
+            original_size (tuple): Original size of the image (width, height).
+            resized_size (tuple): Resized size of the image (width, height).
+        """
+        self.original_size = original_size
+        self.resized_size = resized_size
+
+    def scale_coords_to_original(self, tip):
+        """Scale coordinates from resized image to original image.
+
+        Args:
+            tip (tuple): Coordinates of the tip (x, y) in the resized image.
+
+        Returns:
+            tuple: Scaled coordinates of the tip (x, y) in the original image.
+        """
+        x, y = tip
+        original_width, original_height = self.original_size
+        resized_width, resized_height = self.resized_size
+
+        scale_x = original_width / resized_width
+        scale_y = original_height / resized_height
+
+        original_x = int(x * scale_x)
+        original_y = int(y * scale_y)
+
+        return original_x, original_y
+
+
+class UtilsCrops:
+    """Utility class for calculating crop regions."""
+
+    def __init__(self):
+        """Initialize the UtilsCrops object."""
+        pass
+
+    def calculate_crop_region(self, tip, base, crop_size, IMG_SIZE):
+        """Calculate the crop region based on tip and base coordinates.
+
+        Args:
+            tip (tuple): Coordinates of the tip (x, y).
+            base (tuple): Coordinates of the base (x, y).
+            crop_size (int): Size of the crop region.
+            IMG_SIZE (tuple): Size of the image (width, height).
+
+        Returns:
+            tuple: Crop region coordinates (top, bottom, left, right).
+        """
+        tip_x, tip_y = tip
+        base_x, base_y = base
+        top = max(min(tip_y, base_y) - crop_size, 0)
+        bottom = min(max(tip_y, base_y) + crop_size, IMG_SIZE[1])
+        left = max(min(tip_x, base_x) - crop_size, 0)
+        right = min(max(tip_x, base_x) + crop_size, IMG_SIZE[0])
+        return top, bottom, left, right
+
+    def is_point_on_crop_region(self, point, top, bottom, left, right, buffer=5):
+        """Check if a point is on the crop region boundary.
+
+        Args:
+            point (tuple): Coordinates of the point (x, y).
+            top (int): Top coordinate of the crop region.
+            bottom (int): Bottom coordinate of the crop region.
+            left (int): Left coordinate of the crop region.
+            right (int): Right coordinate of the crop region.
+            buffer (int): Buffer size around the crop region boundary. Defaults to 5.
+
+        Returns:
+            bool: True if the point is on the crop region boundary, False otherwise.
+        """
+        x, y = point
+        return (
+            (top - buffer <= y <= top + buffer)
+            or (bottom - buffer <= y <= bottom + buffer)
+            or (left - buffer <= x <= left + buffer)
+            or (right - buffer <= x <= right + buffer)
+        )
```

### Comparing `parallax_app-0.37.1/parallax_app.egg-info/SOURCES.txt` & `parallax_app-0.37.5/parallax_app.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 .gitignore
 .readthedocs.yaml
 LICENSE
 README.md
 pyproject.toml
 setup.py
+.github/workflows/ci.yml
+.github/workflows/tag_and_publish.yml
 docs/Makefile
 docs/ReadMe.rst
 docs/conf.py
 docs/index.rst
 docs/make.bat
 docs/modules.rst
 docs/parallax.rst
```

### Comparing `parallax_app-0.37.1/tests/test_screen_widget.py` & `parallax_app-0.37.5/tests/test_screen_widget.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-import sys
-import pytest
-from PyQt5.QtWidgets import QApplication, QWidget, QVBoxLayout, QGroupBox
-from PyQt5.QtGui import QFont
-from unittest.mock import MagicMock
-from parallax.screen_widget import ScreenWidget
-
-@pytest.fixture(scope='session')
-def app():
-    """Create QApplication before running tests."""
-    return QApplication(sys.argv)
-
-@pytest.fixture
-def mock_model():
-    """Create a mock model with a list of mock cameras."""
-    model = MagicMock()
-    mock_camera = MagicMock()
-    model.cameras = [mock_camera]  # Assuming at least one mock camera is needed
-    return model
-
-def test_screen_widget_with_mock_camera(app, mock_model):
-    """Test the ScreenWidget with a mock camera."""
-    # Create the main window to host the widget
-    window = QWidget()
-    layout = QVBoxLayout(window)
-
-    # Create a group box to represent a microscope
-    microscope_grp = QGroupBox("Mock Microscope", window)
-    microscope_grp.setFont(QFont("Arial", 9))
-    microscope_grp.setStyleSheet("background-color: rgb(58, 58, 58);")
-    microscope_layout = QVBoxLayout(microscope_grp)
-
-    # Create and add the ScreenWidget to the group box
-    screen = ScreenWidget(mock_model.cameras[0], model=mock_model, parent=microscope_grp)
-    microscope_layout.addWidget(screen)
-
-    layout.addWidget(microscope_grp)
-    window.setLayout(layout)
-    window.show()
-
-    # This ensures the GUI event loop is running during the test
-    with pytest.raises(SystemExit):
-        sys.exit(app.exec_())
-
-if __name__ == "__main__":
-    pytest.main()
+import sys
+import pytest
+from PyQt5.QtWidgets import QApplication, QWidget, QVBoxLayout, QGroupBox
+from PyQt5.QtGui import QFont
+from unittest.mock import MagicMock
+from parallax.screen_widget import ScreenWidget
+
+@pytest.fixture(scope='session')
+def app():
+    """Create QApplication before running tests."""
+    return QApplication(sys.argv)
+
+@pytest.fixture
+def mock_model():
+    """Create a mock model with a list of mock cameras."""
+    model = MagicMock()
+    mock_camera = MagicMock()
+    model.cameras = [mock_camera]  # Assuming at least one mock camera is needed
+    return model
+
+def test_screen_widget_with_mock_camera(app, mock_model):
+    """Test the ScreenWidget with a mock camera."""
+    # Create the main window to host the widget
+    window = QWidget()
+    layout = QVBoxLayout(window)
+
+    # Create a group box to represent a microscope
+    microscope_grp = QGroupBox("Mock Microscope", window)
+    microscope_grp.setFont(QFont("Arial", 9))
+    microscope_grp.setStyleSheet("background-color: rgb(58, 58, 58);")
+    microscope_layout = QVBoxLayout(microscope_grp)
+
+    # Create and add the ScreenWidget to the group box
+    screen = ScreenWidget(mock_model.cameras[0], model=mock_model, parent=microscope_grp)
+    microscope_layout.addWidget(screen)
+
+    layout.addWidget(microscope_grp)
+    window.setLayout(layout)
+    window.show()
+
+    # This ensures the GUI event loop is running during the test
+    with pytest.raises(SystemExit):
+        sys.exit(app.exec_())
+
+if __name__ == "__main__":
+    pytest.main()
```

### Comparing `parallax_app-0.37.1/ui/ParallaxReadME.JPG` & `parallax_app-0.37.5/ui/ParallaxReadME.JPG`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.1/ui/font/FiraCode-VariableFont_wght.ttf` & `parallax_app-0.37.5/ui/font/FiraCode-VariableFont_wght.ttf`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.1/ui/mainWindow.ui` & `parallax_app-0.37.5/ui/settingPopUpMenu.ui`

 * *Files 24% similar despite different names*

#### Comparing `parallax_app-0.37.1/ui/mainWindow.ui` & `parallax_app-0.37.5/ui/settingPopUpMenu.ui`

```diff
@@ -1,334 +1,441 @@
 <?xml version="1.0" encoding="utf-8"?>
 <ui version="4.0">
-  <class>MainWindow</class>
-  <widget class="QMainWindow" name="MainWindow">
+  <class>Form</class>
+  <widget class="QWidget" name="Form">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
-        <width>1041</width>
-        <height>122</height>
+        <width>407</width>
+        <height>300</height>
       </rect>
     </property>
     <property name="minimumSize">
       <size>
-        <width>800</width>
-        <height>0</height>
+        <width>407</width>
+        <height>200</height>
       </size>
     </property>
-    <property name="windowTitle">
-      <string>Parallax</string>
+    <property name="maximumSize">
+      <size>
+        <width>400</width>
+        <height>300</height>
+      </size>
     </property>
-    <property name="windowIcon">
-      <iconset>
-        <normaloff>../img/sextant.png</normaloff>
-        ../img/sextant.png
-      </iconset>
+    <property name="windowTitle">
+      <string>Form</string>
     </property>
     <property name="styleSheet">
       <string notr="true">QWidget{
-background-color: rgb(00,00,00);
+background-color: rgb(58, 58, 58);
 color: #FFFFFF;
-}
-QPushButton{
-	background-color: black;
-}
- QPushButton:pressed {
-     background-color: rgb(224, 0, 0);     
-}
-QPushButton:hover {
-     background-color: rgb(100, 30, 30);
-}
-QPushButton#startButton:disabled:checked {
-	color: gray;
-}
-QPushButton#startButton:disabled:checked {
-	background-color: #ffaaaa;
-}
-QPushButton#startButton:disabled:!checked {
-	background-color: lightGreen;
+font: 9pt;
 }</string>
     </property>
-    <widget class="QWidget" name="centralwidget">
-      <layout class="QGridLayout" name="gridLayout_2">
-        <item row="1" column="0">
-          <layout class="QVBoxLayout" name="verticalLayout_4">
-            <property name="leftMargin">
-              <number>10</number>
-            </property>
-            <property name="topMargin">
-              <number>35</number>
-            </property>
-            <property name="rightMargin">
-              <number>20</number>
-            </property>
-            <property name="bottomMargin">
-              <number>10</number>
-            </property>
-            <item>
-              <widget class="QSplitter" name="splitter">
-                <property name="sizePolicy">
-                  <sizepolicy hsizetype="Expanding" vsizetype="Maximum">
-                    <horstretch>0</horstretch>
-                    <verstretch>0</verstretch>
-                  </sizepolicy>
-                </property>
-                <property name="maximumSize">
-                  <size>
-                    <width>16777215</width>
-                    <height>16777215</height>
-                  </size>
-                </property>
-                <property name="orientation">
-                  <enum>Qt::Horizontal</enum>
-                </property>
-                <widget class="QWidget" name="layoutWidget">
-                  <layout class="QHBoxLayout" name="horizontalLayout_2">
-                    <item>
-                      <widget class="QPushButton" name="startButton">
-                        <property name="minimumSize">
-                          <size>
-                            <width>80</width>
-                            <height>40</height>
-                          </size>
-                        </property>
-                        <property name="maximumSize">
-                          <size>
-                            <width>80</width>
-                            <height>40</height>
-                          </size>
-                        </property>
-                        <property name="font">
-                          <font>
-                            <family>Terminal</family>
-                            <pointsize>12</pointsize>
-                          </font>
-                        </property>
-                        <property name="styleSheet">
-                          <string notr="true">/* Disabled &amp; Checked */
-QPushButton#startButton:checked {
-	color: gray;
-	background-color: #ffaaaa;
-}</string>
-                        </property>
-                        <property name="text">
-                          <string>START</string>
-                        </property>
-                        <property name="iconSize">
-                          <size>
-                            <width>20</width>
-                            <height>20</height>
-                          </size>
-                        </property>
-                        <property name="checkable">
-                          <bool>true</bool>
-                        </property>
-                        <property name="checked">
-                          <bool>true</bool>
-                        </property>
-                      </widget>
-                    </item>
-                    <item>
-                      <widget class="QPushButton" name="recordButton">
-                        <property name="enabled">
-                          <bool>true</bool>
-                        </property>
-                        <property name="minimumSize">
-                          <size>
-                            <width>40</width>
-                            <height>40</height>
-                          </size>
-                        </property>
-                        <property name="maximumSize">
-                          <size>
-                            <width>40</width>
-                            <height>40</height>
-                          </size>
-                        </property>
-                        <property name="styleSheet">
-                          <string notr="true">/* Disabled &amp; Checked */
-QPushButton#recordButton:checked {
-	color: gray;
-	background-color: #ffaaaa;
-}</string>
-                        </property>
-                        <property name="text">
-                          <string/>
-                        </property>
-                        <property name="icon">
-                          <iconset>
-                            <normaloff>resources/recordingButton.png</normaloff>
-                            <disabledoff>resources/recordingButton_disabled.png</disabledoff>
-                            <disabledon>resources/recordingButton_disabled.png</disabledon>
-                            resources/recordingButton.png
-                          </iconset>
-                        </property>
-                        <property name="checkable">
-                          <bool>true</bool>
-                        </property>
-                      </widget>
-                    </item>
-                    <item>
-                      <widget class="QPushButton" name="snapshotButton">
-                        <property name="minimumSize">
-                          <size>
-                            <width>40</width>
-                            <height>40</height>
-                          </size>
-                        </property>
-                        <property name="maximumSize">
-                          <size>
-                            <width>40</width>
-                            <height>40</height>
-                          </size>
-                        </property>
-                        <property name="styleSheet">
-                          <string notr="true">/* Disabled &amp; Checked */
-QPushButton#snapshotButton:pressed {
-	color: gray;
-	background-color: #ffaaaa;
-}</string>
-                        </property>
-                        <property name="text">
-                          <string/>
-                        </property>
-                        <property name="icon">
-                          <iconset>
-                            <normaloff>resources/snapshotButton_green.png</normaloff>
-                            <disabledon>resources/snapshotButton_disabled.png</disabledon>
-                            resources/snapshotButton_green.png
-                          </iconset>
-                        </property>
-                        <property name="iconSize">
-                          <size>
-                            <width>22</width>
-                            <height>22</height>
-                          </size>
-                        </property>
-                      </widget>
-                    </item>
-                    <item>
-                      <widget class="QLabel" name="dirLabel">
-                        <property name="maximumSize">
-                          <size>
-                            <width>16777215</width>
-                            <height>40</height>
-                          </size>
-                        </property>
-                        <property name="font">
-                          <font>
-                            <pointsize>8</pointsize>
-                          </font>
-                        </property>
-                        <property name="styleSheet">
-                          <string notr="true"/>
-                        </property>
-                        <property name="text">
-                          <string>C:\</string>
-                        </property>
-                      </widget>
-                    </item>
-                    <item>
-                      <widget class="QToolButton" name="browseDirButton">
-                        <property name="minimumSize">
-                          <size>
-                            <width>40</width>
-                            <height>40</height>
-                          </size>
-                        </property>
-                        <property name="maximumSize">
-                          <size>
-                            <width>40</width>
-                            <height>40</height>
-                          </size>
-                        </property>
-                        <property name="styleSheet">
-                          <string notr="true">QToolButton#browseDirButton:pressed {
-	color: gray;
-	background-color: #ffaaaa;
-}</string>
-                        </property>
-                        <property name="text">
-                          <string>...</string>
-                        </property>
-                      </widget>
-                    </item>
-                  </layout>
-                </widget>
-                <widget class="QWidget" name="layoutWidget_2">
-                  <layout class="QHBoxLayout" name="horizontalLayout_4">
-                    <item>
-                      <spacer name="horizontalSpacer">
-                        <property name="orientation">
-                          <enum>Qt::Horizontal</enum>
-                        </property>
-                        <property name="sizeHint" stdset="0">
-                          <size>
-                            <width>68</width>
-                            <height>22</height>
-                          </size>
-                        </property>
-                      </spacer>
-                    </item>
-                    <item>
-                      <widget class="QLabel" name="columnsLabel">
-                        <property name="minimumSize">
-                          <size>
-                            <width>90</width>
-                            <height>30</height>
-                          </size>
-                        </property>
-                        <property name="maximumSize">
-                          <size>
-                            <width>90</width>
-                            <height>30</height>
-                          </size>
-                        </property>
-                        <property name="font">
-                          <font>
-                            <family>Terminal</family>
-                            <pointsize>12</pointsize>
-                          </font>
-                        </property>
-                        <property name="text">
-                          <string>Columns:</string>
-                        </property>
-                      </widget>
-                    </item>
-                    <item>
-                      <widget class="QSpinBox" name="nColumnsSpinBox">
-                        <property name="minimumSize">
-                          <size>
-                            <width>60</width>
-                            <height>40</height>
-                          </size>
-                        </property>
-                        <property name="maximumSize">
-                          <size>
-                            <width>60</width>
-                            <height>40</height>
-                          </size>
-                        </property>
-                        <property name="minimum">
-                          <number>1</number>
-                        </property>
-                        <property name="maximum">
-                          <number>6</number>
-                        </property>
-                        <property name="value">
-                          <number>1</number>
-                        </property>
-                      </widget>
-                    </item>
-                  </layout>
-                </widget>
-              </widget>
-            </item>
-          </layout>
-        </item>
-      </layout>
-    </widget>
+    <layout class="QGridLayout" name="gridLayout">
+      <property name="verticalSpacing">
+        <number>1</number>
+      </property>
+      <item row="0" column="0">
+        <widget class="QLabel" name="nameLabel">
+          <property name="minimumSize">
+            <size>
+              <width>100</width>
+              <height>0</height>
+            </size>
+          </property>
+          <property name="maximumSize">
+            <size>
+              <width>16777215</width>
+              <height>20</height>
+            </size>
+          </property>
+          <property name="text">
+            <string>Name:</string>
+          </property>
+        </widget>
+      </item>
+      <item row="7" column="3">
+        <widget class="QLabel" name="gammaNum">
+          <property name="text">
+            <string>1.0</string>
+          </property>
+        </widget>
+      </item>
+      <item row="5" column="2">
+        <widget class="QSlider" name="wbSliderRed">
+          <property name="minimum">
+            <number>25</number>
+          </property>
+          <property name="maximum">
+            <number>400</number>
+          </property>
+          <property name="value">
+            <number>130</number>
+          </property>
+          <property name="sliderPosition">
+            <number>130</number>
+          </property>
+          <property name="orientation">
+            <enum>Qt::Horizontal</enum>
+          </property>
+        </widget>
+      </item>
+      <item row="1" column="1" colspan="3">
+        <widget class="QComboBox" name="snComboBox"/>
+      </item>
+      <item row="4" column="3">
+        <widget class="QLabel" name="gainNum">
+          <property name="text">
+            <string>25</string>
+          </property>
+          <property name="textFormat">
+            <enum>Qt::PlainText</enum>
+          </property>
+        </widget>
+      </item>
+      <item row="6" column="3">
+        <widget class="QLabel" name="wbNumBlue">
+          <property name="text">
+            <string>2.8</string>
+          </property>
+        </widget>
+      </item>
+      <item row="7" column="0">
+        <widget class="QLabel" name="gammaLabel">
+          <property name="maximumSize">
+            <size>
+              <width>16777215</width>
+              <height>20</height>
+            </size>
+          </property>
+          <property name="text">
+            <string>Gamma:</string>
+          </property>
+        </widget>
+      </item>
+      <item row="1" column="0">
+        <widget class="QLabel" name="snLabel">
+          <property name="maximumSize">
+            <size>
+              <width>16777215</width>
+              <height>20</height>
+            </size>
+          </property>
+          <property name="text">
+            <string>S/N:</string>
+          </property>
+        </widget>
+      </item>
+      <item row="0" column="1" colspan="3">
+        <widget class="QLineEdit" name="customName">
+          <property name="minimumSize">
+            <size>
+              <width>100</width>
+              <height>0</height>
+            </size>
+          </property>
+          <property name="text">
+            <string>Microscope</string>
+          </property>
+        </widget>
+      </item>
+      <item row="3" column="0">
+        <widget class="QLabel" name="expLabel">
+          <property name="maximumSize">
+            <size>
+              <width>16777215</width>
+              <height>20</height>
+            </size>
+          </property>
+          <property name="text">
+            <string>Exposure:</string>
+          </property>
+        </widget>
+      </item>
+      <item row="7" column="2">
+        <widget class="QSlider" name="gammaSlider">
+          <property name="minimum">
+            <number>30</number>
+          </property>
+          <property name="maximum">
+            <number>125</number>
+          </property>
+          <property name="singleStep">
+            <number>1</number>
+          </property>
+          <property name="value">
+            <number>100</number>
+          </property>
+          <property name="orientation">
+            <enum>Qt::Horizontal</enum>
+          </property>
+          <property name="tickPosition">
+            <enum>QSlider::NoTicks</enum>
+          </property>
+        </widget>
+      </item>
+      <item row="3" column="3">
+        <widget class="QLabel" name="expNum">
+          <property name="text">
+            <string>16</string>
+          </property>
+          <property name="textFormat">
+            <enum>Qt::PlainText</enum>
+          </property>
+        </widget>
+      </item>
+      <item row="4" column="0">
+        <widget class="QLabel" name="gainLabel">
+          <property name="maximumSize">
+            <size>
+              <width>16777215</width>
+              <height>20</height>
+            </size>
+          </property>
+          <property name="text">
+            <string>Gain:</string>
+          </property>
+        </widget>
+      </item>
+      <item row="5" column="3">
+        <widget class="QLabel" name="wbNumRed">
+          <property name="text">
+            <string>1.2</string>
+          </property>
+        </widget>
+      </item>
+      <item row="6" column="2">
+        <widget class="QSlider" name="wbSliderBlue">
+          <property name="minimum">
+            <number>25</number>
+          </property>
+          <property name="maximum">
+            <number>400</number>
+          </property>
+          <property name="value">
+            <number>280</number>
+          </property>
+          <property name="orientation">
+            <enum>Qt::Horizontal</enum>
+          </property>
+        </widget>
+      </item>
+      <item row="2" column="1" alignment="Qt::AlignHCenter">
+        <widget class="QLabel" name="autoLabel">
+          <property name="maximumSize">
+            <size>
+              <width>16777215</width>
+              <height>20</height>
+            </size>
+          </property>
+          <property name="font">
+            <font>
+              <pointsize>9</pointsize>
+              <weight>50</weight>
+              <italic>false</italic>
+              <bold>false</bold>
+            </font>
+          </property>
+          <property name="text">
+            <string>Auto</string>
+          </property>
+          <property name="alignment">
+            <set>Qt::AlignCenter</set>
+          </property>
+        </widget>
+      </item>
+      <item row="4" column="2">
+        <widget class="QSlider" name="gainSlider">
+          <property name="maximum">
+            <number>27</number>
+          </property>
+          <property name="value">
+            <number>25</number>
+          </property>
+          <property name="orientation">
+            <enum>Qt::Horizontal</enum>
+          </property>
+        </widget>
+      </item>
+      <item row="5" column="0">
+        <widget class="QLabel" name="wbLabelRed">
+          <property name="maximumSize">
+            <size>
+              <width>16777215</width>
+              <height>20</height>
+            </size>
+          </property>
+          <property name="font">
+            <font>
+              <pointsize>9</pointsize>
+              <weight>50</weight>
+              <italic>false</italic>
+              <bold>false</bold>
+            </font>
+          </property>
+          <property name="text">
+            <string>W/B Red:</string>
+          </property>
+          <property name="wordWrap">
+            <bool>true</bool>
+          </property>
+        </widget>
+      </item>
+      <item row="6" column="0">
+        <widget class="QLabel" name="wbLabelBlue">
+          <property name="maximumSize">
+            <size>
+              <width>16777215</width>
+              <height>20</height>
+            </size>
+          </property>
+          <property name="text">
+            <string>W/B Blue:</string>
+          </property>
+        </widget>
+      </item>
+      <item row="3" column="2">
+        <widget class="QSlider" name="expSlider">
+          <property name="minimumSize">
+            <size>
+              <width>0</width>
+              <height>0</height>
+            </size>
+          </property>
+          <property name="minimum">
+            <number>1</number>
+          </property>
+          <property name="maximum">
+            <number>250</number>
+          </property>
+          <property name="value">
+            <number>16</number>
+          </property>
+          <property name="orientation">
+            <enum>Qt::Horizontal</enum>
+          </property>
+        </widget>
+      </item>
+      <item row="3" column="1">
+        <widget class="QPushButton" name="expAuto">
+          <property name="maximumSize">
+            <size>
+              <width>30</width>
+              <height>30</height>
+            </size>
+          </property>
+          <property name="text">
+            <string>♦</string>
+          </property>
+        </widget>
+      </item>
+      <item row="4" column="1">
+        <widget class="QPushButton" name="gainAuto">
+          <property name="maximumSize">
+            <size>
+              <width>30</width>
+              <height>30</height>
+            </size>
+          </property>
+          <property name="text">
+            <string>♦</string>
+          </property>
+        </widget>
+      </item>
+      <item row="5" column="1">
+        <widget class="QPushButton" name="wbAuto">
+          <property name="maximumSize">
+            <size>
+              <width>30</width>
+              <height>30</height>
+            </size>
+          </property>
+          <property name="text">
+            <string>♦</string>
+          </property>
+        </widget>
+      </item>
+      <item row="7" column="1">
+        <widget class="QPushButton" name="gammaAuto">
+          <property name="maximumSize">
+            <size>
+              <width>30</width>
+              <height>30</height>
+            </size>
+          </property>
+          <property name="text">
+            <string>♦</string>
+          </property>
+        </widget>
+      </item>
+    </layout>
   </widget>
   <resources/>
-  <connections/>
+  <connections>
+    <connection>
+      <sender>expSlider</sender>
+      <signal>valueChanged(int)</signal>
+      <receiver>expNum</receiver>
+      <slot>setNum(int)</slot>
+      <hints>
+        <hint type="sourcelabel">
+          <x>177</x>
+          <y>136</y>
+        </hint>
+        <hint type="destinationlabel">
+          <x>290</x>
+          <y>137</y>
+        </hint>
+      </hints>
+    </connection>
+    <connection>
+      <sender>gainSlider</sender>
+      <signal>valueChanged(int)</signal>
+      <receiver>gainNum</receiver>
+      <slot>setNum(int)</slot>
+      <hints>
+        <hint type="sourcelabel">
+          <x>235</x>
+          <y>173</y>
+        </hint>
+        <hint type="destinationlabel">
+          <x>290</x>
+          <y>176</y>
+        </hint>
+      </hints>
+    </connection>
+    <connection>
+      <sender>wbSliderRed</sender>
+      <signal>valueChanged(int)</signal>
+      <receiver>wbNumRed</receiver>
+      <slot>setNum(int)</slot>
+      <hints>
+        <hint type="sourcelabel">
+          <x>216</x>
+          <y>219</y>
+        </hint>
+        <hint type="destinationlabel">
+          <x>290</x>
+          <y>223</y>
+        </hint>
+      </hints>
+    </connection>
+    <connection>
+      <sender>gammaSlider</sender>
+      <signal>valueChanged(int)</signal>
+      <receiver>gammaNum</receiver>
+      <slot>setNum(int)</slot>
+      <hints>
+        <hint type="sourcelabel">
+          <x>230</x>
+          <y>262</y>
+        </hint>
+        <hint type="destinationlabel">
+          <x>290</x>
+          <y>262</y>
+        </hint>
+      </hints>
+    </connection>
+  </connections>
 </ui>
```

### Comparing `parallax_app-0.37.1/ui/resources/arrow-right.png` & `parallax_app-0.37.5/ui/resources/arrow-right.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.1/ui/resources/check.png` & `parallax_app-0.37.5/ui/resources/check.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.1/ui/resources/gear.png` & `parallax_app-0.37.5/ui/resources/gear.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.1/ui/resources/recordingButton.png` & `parallax_app-0.37.5/ui/resources/recordingButton.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.1/ui/resources/recordingButton_disabled.png` & `parallax_app-0.37.5/ui/resources/recordingButton_disabled.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.1/ui/resources/sextant.png` & `parallax_app-0.37.5/ui/resources/sextant.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.1/ui/resources/snapshotButton_disabled.png` & `parallax_app-0.37.5/ui/resources/snapshotButton_disabled.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.1/ui/resources/snapshotButton_green.png` & `parallax_app-0.37.5/ui/resources/snapshotButton_green.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.1/ui/resources/snapshotButton_white.png` & `parallax_app-0.37.5/ui/resources/snapshotButton_white.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.1/ui/resources/stop-sign.png` & `parallax_app-0.37.5/ui/resources/stop-sign.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.1/ui/resources/target.png` & `parallax_app-0.37.5/ui/resources/target.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.1/ui/settingPopUpMenu.ui` & `parallax_app-0.37.5/ui/mainWindow.ui`

 * *Files 22% similar despite different names*

#### Comparing `parallax_app-0.37.1/ui/settingPopUpMenu.ui` & `parallax_app-0.37.5/ui/mainWindow.ui`

```diff
@@ -1,441 +1,334 @@
 <?xml version="1.0" encoding="utf-8"?>
 <ui version="4.0">
-  <class>Form</class>
-  <widget class="QWidget" name="Form">
+  <class>MainWindow</class>
+  <widget class="QMainWindow" name="MainWindow">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
-        <width>407</width>
-        <height>300</height>
+        <width>1041</width>
+        <height>122</height>
       </rect>
     </property>
     <property name="minimumSize">
       <size>
-        <width>407</width>
-        <height>200</height>
-      </size>
-    </property>
-    <property name="maximumSize">
-      <size>
-        <width>400</width>
-        <height>300</height>
+        <width>800</width>
+        <height>0</height>
       </size>
     </property>
     <property name="windowTitle">
-      <string>Form</string>
+      <string>Parallax</string>
+    </property>
+    <property name="windowIcon">
+      <iconset>
+        <normaloff>../img/sextant.png</normaloff>
+        ../img/sextant.png
+      </iconset>
     </property>
     <property name="styleSheet">
       <string notr="true">QWidget{
-background-color: rgb(58, 58, 58);
+background-color: rgb(00,00,00);
 color: #FFFFFF;
-font: 9pt;
+}
+QPushButton{
+	background-color: black;
+}
+ QPushButton:pressed {
+     background-color: rgb(224, 0, 0);     
+}
+QPushButton:hover {
+     background-color: rgb(100, 30, 30);
+}
+QPushButton#startButton:disabled:checked {
+	color: gray;
+}
+QPushButton#startButton:disabled:checked {
+	background-color: #ffaaaa;
+}
+QPushButton#startButton:disabled:!checked {
+	background-color: lightGreen;
 }</string>
     </property>
-    <layout class="QGridLayout" name="gridLayout">
-      <property name="verticalSpacing">
-        <number>1</number>
-      </property>
-      <item row="0" column="0">
-        <widget class="QLabel" name="nameLabel">
-          <property name="minimumSize">
-            <size>
-              <width>100</width>
-              <height>0</height>
-            </size>
-          </property>
-          <property name="maximumSize">
-            <size>
-              <width>16777215</width>
-              <height>20</height>
-            </size>
-          </property>
-          <property name="text">
-            <string>Name:</string>
-          </property>
-        </widget>
-      </item>
-      <item row="7" column="3">
-        <widget class="QLabel" name="gammaNum">
-          <property name="text">
-            <string>1.0</string>
-          </property>
-        </widget>
-      </item>
-      <item row="5" column="2">
-        <widget class="QSlider" name="wbSliderRed">
-          <property name="minimum">
-            <number>25</number>
-          </property>
-          <property name="maximum">
-            <number>400</number>
-          </property>
-          <property name="value">
-            <number>130</number>
-          </property>
-          <property name="sliderPosition">
-            <number>130</number>
-          </property>
-          <property name="orientation">
-            <enum>Qt::Horizontal</enum>
-          </property>
-        </widget>
-      </item>
-      <item row="1" column="1" colspan="3">
-        <widget class="QComboBox" name="snComboBox"/>
-      </item>
-      <item row="4" column="3">
-        <widget class="QLabel" name="gainNum">
-          <property name="text">
-            <string>25</string>
-          </property>
-          <property name="textFormat">
-            <enum>Qt::PlainText</enum>
-          </property>
-        </widget>
-      </item>
-      <item row="6" column="3">
-        <widget class="QLabel" name="wbNumBlue">
-          <property name="text">
-            <string>2.8</string>
-          </property>
-        </widget>
-      </item>
-      <item row="7" column="0">
-        <widget class="QLabel" name="gammaLabel">
-          <property name="maximumSize">
-            <size>
-              <width>16777215</width>
-              <height>20</height>
-            </size>
-          </property>
-          <property name="text">
-            <string>Gamma:</string>
-          </property>
-        </widget>
-      </item>
-      <item row="1" column="0">
-        <widget class="QLabel" name="snLabel">
-          <property name="maximumSize">
-            <size>
-              <width>16777215</width>
-              <height>20</height>
-            </size>
-          </property>
-          <property name="text">
-            <string>S/N:</string>
-          </property>
-        </widget>
-      </item>
-      <item row="0" column="1" colspan="3">
-        <widget class="QLineEdit" name="customName">
-          <property name="minimumSize">
-            <size>
-              <width>100</width>
-              <height>0</height>
-            </size>
-          </property>
-          <property name="text">
-            <string>Microscope</string>
-          </property>
-        </widget>
-      </item>
-      <item row="3" column="0">
-        <widget class="QLabel" name="expLabel">
-          <property name="maximumSize">
-            <size>
-              <width>16777215</width>
-              <height>20</height>
-            </size>
-          </property>
-          <property name="text">
-            <string>Exposure:</string>
-          </property>
-        </widget>
-      </item>
-      <item row="7" column="2">
-        <widget class="QSlider" name="gammaSlider">
-          <property name="minimum">
-            <number>30</number>
-          </property>
-          <property name="maximum">
-            <number>125</number>
-          </property>
-          <property name="singleStep">
-            <number>1</number>
-          </property>
-          <property name="value">
-            <number>100</number>
-          </property>
-          <property name="orientation">
-            <enum>Qt::Horizontal</enum>
-          </property>
-          <property name="tickPosition">
-            <enum>QSlider::NoTicks</enum>
-          </property>
-        </widget>
-      </item>
-      <item row="3" column="3">
-        <widget class="QLabel" name="expNum">
-          <property name="text">
-            <string>16</string>
-          </property>
-          <property name="textFormat">
-            <enum>Qt::PlainText</enum>
-          </property>
-        </widget>
-      </item>
-      <item row="4" column="0">
-        <widget class="QLabel" name="gainLabel">
-          <property name="maximumSize">
-            <size>
-              <width>16777215</width>
-              <height>20</height>
-            </size>
-          </property>
-          <property name="text">
-            <string>Gain:</string>
-          </property>
-        </widget>
-      </item>
-      <item row="5" column="3">
-        <widget class="QLabel" name="wbNumRed">
-          <property name="text">
-            <string>1.2</string>
-          </property>
-        </widget>
-      </item>
-      <item row="6" column="2">
-        <widget class="QSlider" name="wbSliderBlue">
-          <property name="minimum">
-            <number>25</number>
-          </property>
-          <property name="maximum">
-            <number>400</number>
-          </property>
-          <property name="value">
-            <number>280</number>
-          </property>
-          <property name="orientation">
-            <enum>Qt::Horizontal</enum>
-          </property>
-        </widget>
-      </item>
-      <item row="2" column="1" alignment="Qt::AlignHCenter">
-        <widget class="QLabel" name="autoLabel">
-          <property name="maximumSize">
-            <size>
-              <width>16777215</width>
-              <height>20</height>
-            </size>
-          </property>
-          <property name="font">
-            <font>
-              <pointsize>9</pointsize>
-              <weight>50</weight>
-              <italic>false</italic>
-              <bold>false</bold>
-            </font>
-          </property>
-          <property name="text">
-            <string>Auto</string>
-          </property>
-          <property name="alignment">
-            <set>Qt::AlignCenter</set>
-          </property>
-        </widget>
-      </item>
-      <item row="4" column="2">
-        <widget class="QSlider" name="gainSlider">
-          <property name="maximum">
-            <number>27</number>
-          </property>
-          <property name="value">
-            <number>25</number>
-          </property>
-          <property name="orientation">
-            <enum>Qt::Horizontal</enum>
-          </property>
-        </widget>
-      </item>
-      <item row="5" column="0">
-        <widget class="QLabel" name="wbLabelRed">
-          <property name="maximumSize">
-            <size>
-              <width>16777215</width>
-              <height>20</height>
-            </size>
-          </property>
-          <property name="font">
-            <font>
-              <pointsize>9</pointsize>
-              <weight>50</weight>
-              <italic>false</italic>
-              <bold>false</bold>
-            </font>
-          </property>
-          <property name="text">
-            <string>W/B Red:</string>
-          </property>
-          <property name="wordWrap">
-            <bool>true</bool>
-          </property>
-        </widget>
-      </item>
-      <item row="6" column="0">
-        <widget class="QLabel" name="wbLabelBlue">
-          <property name="maximumSize">
-            <size>
-              <width>16777215</width>
-              <height>20</height>
-            </size>
-          </property>
-          <property name="text">
-            <string>W/B Blue:</string>
-          </property>
-        </widget>
-      </item>
-      <item row="3" column="2">
-        <widget class="QSlider" name="expSlider">
-          <property name="minimumSize">
-            <size>
-              <width>0</width>
-              <height>0</height>
-            </size>
-          </property>
-          <property name="minimum">
-            <number>1</number>
-          </property>
-          <property name="maximum">
-            <number>250</number>
-          </property>
-          <property name="value">
-            <number>16</number>
-          </property>
-          <property name="orientation">
-            <enum>Qt::Horizontal</enum>
-          </property>
-        </widget>
-      </item>
-      <item row="3" column="1">
-        <widget class="QPushButton" name="expAuto">
-          <property name="maximumSize">
-            <size>
-              <width>30</width>
-              <height>30</height>
-            </size>
-          </property>
-          <property name="text">
-            <string>♦</string>
-          </property>
-        </widget>
-      </item>
-      <item row="4" column="1">
-        <widget class="QPushButton" name="gainAuto">
-          <property name="maximumSize">
-            <size>
-              <width>30</width>
-              <height>30</height>
-            </size>
-          </property>
-          <property name="text">
-            <string>♦</string>
-          </property>
-        </widget>
-      </item>
-      <item row="5" column="1">
-        <widget class="QPushButton" name="wbAuto">
-          <property name="maximumSize">
-            <size>
-              <width>30</width>
-              <height>30</height>
-            </size>
-          </property>
-          <property name="text">
-            <string>♦</string>
-          </property>
-        </widget>
-      </item>
-      <item row="7" column="1">
-        <widget class="QPushButton" name="gammaAuto">
-          <property name="maximumSize">
-            <size>
-              <width>30</width>
-              <height>30</height>
-            </size>
-          </property>
-          <property name="text">
-            <string>♦</string>
-          </property>
-        </widget>
-      </item>
-    </layout>
+    <widget class="QWidget" name="centralwidget">
+      <layout class="QGridLayout" name="gridLayout_2">
+        <item row="1" column="0">
+          <layout class="QVBoxLayout" name="verticalLayout_4">
+            <property name="leftMargin">
+              <number>10</number>
+            </property>
+            <property name="topMargin">
+              <number>35</number>
+            </property>
+            <property name="rightMargin">
+              <number>20</number>
+            </property>
+            <property name="bottomMargin">
+              <number>10</number>
+            </property>
+            <item>
+              <widget class="QSplitter" name="splitter">
+                <property name="sizePolicy">
+                  <sizepolicy hsizetype="Expanding" vsizetype="Maximum">
+                    <horstretch>0</horstretch>
+                    <verstretch>0</verstretch>
+                  </sizepolicy>
+                </property>
+                <property name="maximumSize">
+                  <size>
+                    <width>16777215</width>
+                    <height>16777215</height>
+                  </size>
+                </property>
+                <property name="orientation">
+                  <enum>Qt::Horizontal</enum>
+                </property>
+                <widget class="QWidget" name="layoutWidget">
+                  <layout class="QHBoxLayout" name="horizontalLayout_2">
+                    <item>
+                      <widget class="QPushButton" name="startButton">
+                        <property name="minimumSize">
+                          <size>
+                            <width>80</width>
+                            <height>40</height>
+                          </size>
+                        </property>
+                        <property name="maximumSize">
+                          <size>
+                            <width>80</width>
+                            <height>40</height>
+                          </size>
+                        </property>
+                        <property name="font">
+                          <font>
+                            <family>Terminal</family>
+                            <pointsize>12</pointsize>
+                          </font>
+                        </property>
+                        <property name="styleSheet">
+                          <string notr="true">/* Disabled &amp; Checked */
+QPushButton#startButton:checked {
+	color: gray;
+	background-color: #ffaaaa;
+}</string>
+                        </property>
+                        <property name="text">
+                          <string>START</string>
+                        </property>
+                        <property name="iconSize">
+                          <size>
+                            <width>20</width>
+                            <height>20</height>
+                          </size>
+                        </property>
+                        <property name="checkable">
+                          <bool>true</bool>
+                        </property>
+                        <property name="checked">
+                          <bool>true</bool>
+                        </property>
+                      </widget>
+                    </item>
+                    <item>
+                      <widget class="QPushButton" name="recordButton">
+                        <property name="enabled">
+                          <bool>true</bool>
+                        </property>
+                        <property name="minimumSize">
+                          <size>
+                            <width>40</width>
+                            <height>40</height>
+                          </size>
+                        </property>
+                        <property name="maximumSize">
+                          <size>
+                            <width>40</width>
+                            <height>40</height>
+                          </size>
+                        </property>
+                        <property name="styleSheet">
+                          <string notr="true">/* Disabled &amp; Checked */
+QPushButton#recordButton:checked {
+	color: gray;
+	background-color: #ffaaaa;
+}</string>
+                        </property>
+                        <property name="text">
+                          <string/>
+                        </property>
+                        <property name="icon">
+                          <iconset>
+                            <normaloff>resources/recordingButton.png</normaloff>
+                            <disabledoff>resources/recordingButton_disabled.png</disabledoff>
+                            <disabledon>resources/recordingButton_disabled.png</disabledon>
+                            resources/recordingButton.png
+                          </iconset>
+                        </property>
+                        <property name="checkable">
+                          <bool>true</bool>
+                        </property>
+                      </widget>
+                    </item>
+                    <item>
+                      <widget class="QPushButton" name="snapshotButton">
+                        <property name="minimumSize">
+                          <size>
+                            <width>40</width>
+                            <height>40</height>
+                          </size>
+                        </property>
+                        <property name="maximumSize">
+                          <size>
+                            <width>40</width>
+                            <height>40</height>
+                          </size>
+                        </property>
+                        <property name="styleSheet">
+                          <string notr="true">/* Disabled &amp; Checked */
+QPushButton#snapshotButton:pressed {
+	color: gray;
+	background-color: #ffaaaa;
+}</string>
+                        </property>
+                        <property name="text">
+                          <string/>
+                        </property>
+                        <property name="icon">
+                          <iconset>
+                            <normaloff>resources/snapshotButton_green.png</normaloff>
+                            <disabledon>resources/snapshotButton_disabled.png</disabledon>
+                            resources/snapshotButton_green.png
+                          </iconset>
+                        </property>
+                        <property name="iconSize">
+                          <size>
+                            <width>22</width>
+                            <height>22</height>
+                          </size>
+                        </property>
+                      </widget>
+                    </item>
+                    <item>
+                      <widget class="QLabel" name="dirLabel">
+                        <property name="maximumSize">
+                          <size>
+                            <width>16777215</width>
+                            <height>40</height>
+                          </size>
+                        </property>
+                        <property name="font">
+                          <font>
+                            <pointsize>8</pointsize>
+                          </font>
+                        </property>
+                        <property name="styleSheet">
+                          <string notr="true"/>
+                        </property>
+                        <property name="text">
+                          <string>C:\</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item>
+                      <widget class="QToolButton" name="browseDirButton">
+                        <property name="minimumSize">
+                          <size>
+                            <width>40</width>
+                            <height>40</height>
+                          </size>
+                        </property>
+                        <property name="maximumSize">
+                          <size>
+                            <width>40</width>
+                            <height>40</height>
+                          </size>
+                        </property>
+                        <property name="styleSheet">
+                          <string notr="true">QToolButton#browseDirButton:pressed {
+	color: gray;
+	background-color: #ffaaaa;
+}</string>
+                        </property>
+                        <property name="text">
+                          <string>...</string>
+                        </property>
+                      </widget>
+                    </item>
+                  </layout>
+                </widget>
+                <widget class="QWidget" name="layoutWidget_2">
+                  <layout class="QHBoxLayout" name="horizontalLayout_4">
+                    <item>
+                      <spacer name="horizontalSpacer">
+                        <property name="orientation">
+                          <enum>Qt::Horizontal</enum>
+                        </property>
+                        <property name="sizeHint" stdset="0">
+                          <size>
+                            <width>68</width>
+                            <height>22</height>
+                          </size>
+                        </property>
+                      </spacer>
+                    </item>
+                    <item>
+                      <widget class="QLabel" name="columnsLabel">
+                        <property name="minimumSize">
+                          <size>
+                            <width>90</width>
+                            <height>30</height>
+                          </size>
+                        </property>
+                        <property name="maximumSize">
+                          <size>
+                            <width>90</width>
+                            <height>30</height>
+                          </size>
+                        </property>
+                        <property name="font">
+                          <font>
+                            <family>Terminal</family>
+                            <pointsize>12</pointsize>
+                          </font>
+                        </property>
+                        <property name="text">
+                          <string>Columns:</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item>
+                      <widget class="QSpinBox" name="nColumnsSpinBox">
+                        <property name="minimumSize">
+                          <size>
+                            <width>60</width>
+                            <height>40</height>
+                          </size>
+                        </property>
+                        <property name="maximumSize">
+                          <size>
+                            <width>60</width>
+                            <height>40</height>
+                          </size>
+                        </property>
+                        <property name="minimum">
+                          <number>1</number>
+                        </property>
+                        <property name="maximum">
+                          <number>6</number>
+                        </property>
+                        <property name="value">
+                          <number>1</number>
+                        </property>
+                      </widget>
+                    </item>
+                  </layout>
+                </widget>
+              </widget>
+            </item>
+          </layout>
+        </item>
+      </layout>
+    </widget>
   </widget>
   <resources/>
-  <connections>
-    <connection>
-      <sender>expSlider</sender>
-      <signal>valueChanged(int)</signal>
-      <receiver>expNum</receiver>
-      <slot>setNum(int)</slot>
-      <hints>
-        <hint type="sourcelabel">
-          <x>177</x>
-          <y>136</y>
-        </hint>
-        <hint type="destinationlabel">
-          <x>290</x>
-          <y>137</y>
-        </hint>
-      </hints>
-    </connection>
-    <connection>
-      <sender>gainSlider</sender>
-      <signal>valueChanged(int)</signal>
-      <receiver>gainNum</receiver>
-      <slot>setNum(int)</slot>
-      <hints>
-        <hint type="sourcelabel">
-          <x>235</x>
-          <y>173</y>
-        </hint>
-        <hint type="destinationlabel">
-          <x>290</x>
-          <y>176</y>
-        </hint>
-      </hints>
-    </connection>
-    <connection>
-      <sender>wbSliderRed</sender>
-      <signal>valueChanged(int)</signal>
-      <receiver>wbNumRed</receiver>
-      <slot>setNum(int)</slot>
-      <hints>
-        <hint type="sourcelabel">
-          <x>216</x>
-          <y>219</y>
-        </hint>
-        <hint type="destinationlabel">
-          <x>290</x>
-          <y>223</y>
-        </hint>
-      </hints>
-    </connection>
-    <connection>
-      <sender>gammaSlider</sender>
-      <signal>valueChanged(int)</signal>
-      <receiver>gammaNum</receiver>
-      <slot>setNum(int)</slot>
-      <hints>
-        <hint type="sourcelabel">
-          <x>230</x>
-          <y>262</y>
-        </hint>
-        <hint type="destinationlabel">
-          <x>290</x>
-          <y>262</y>
-        </hint>
-      </hints>
-    </connection>
-  </connections>
+  <connections/>
 </ui>
```

### Comparing `parallax_app-0.37.1/ui/stage_info.ui` & `parallax_app-0.37.5/ui/stage_info.ui`

 * *Format-specific differences are supported for XML files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: XML 1.0 document, Unicode text, UTF-8 text, with CRLF line terminators*

 * *Files 25% similar despite different names*

```diff
@@ -1,671 +1,648 @@
 00000000: 3c3f 786d 6c20 7665 7273 696f 6e3d 2231  <?xml version="1
 00000010: 2e30 2220 656e 636f 6469 6e67 3d22 5554  .0" encoding="UT
-00000020: 462d 3822 3f3e 0d0a 3c75 6920 7665 7273  F-8"?>..<ui vers
-00000030: 696f 6e3d 2234 2e30 223e 0d0a 203c 636c  ion="4.0">.. <cl
-00000040: 6173 733e 466f 726d 3c2f 636c 6173 733e  ass>Form</class>
-00000050: 0d0a 203c 7769 6467 6574 2063 6c61 7373  .. <widget class
-00000060: 3d22 5157 6964 6765 7422 206e 616d 653d  ="QWidget" name=
-00000070: 2246 6f72 6d22 3e0d 0a20 203c 7072 6f70  "Form">..  <prop
-00000080: 6572 7479 206e 616d 653d 2267 656f 6d65  erty name="geome
-00000090: 7472 7922 3e0d 0a20 2020 3c72 6563 743e  try">..   <rect>
-000000a0: 0d0a 2020 2020 3c78 3e30 3c2f 783e 0d0a  ..    <x>0</x>..
-000000b0: 2020 2020 3c79 3e30 3c2f 793e 0d0a 2020      <y>0</y>..  
-000000c0: 2020 3c77 6964 7468 3e35 3235 3c2f 7769    <width>525</wi
-000000d0: 6474 683e 0d0a 2020 2020 3c68 6569 6768  dth>..    <heigh
-000000e0: 743e 3735 343c 2f68 6569 6768 743e 0d0a  t>754</height>..
-000000f0: 2020 203c 2f72 6563 743e 0d0a 2020 3c2f     </rect>..  </
-00000100: 7072 6f70 6572 7479 3e0d 0a20 203c 7072  property>..  <pr
-00000110: 6f70 6572 7479 206e 616d 653d 2277 696e  operty name="win
-00000120: 646f 7754 6974 6c65 223e 0d0a 2020 203c  dowTitle">..   <
-00000130: 7374 7269 6e67 3e46 6f72 6d3c 2f73 7472  string>Form</str
-00000140: 696e 673e 0d0a 2020 3c2f 7072 6f70 6572  ing>..  </proper
-00000150: 7479 3e0d 0a20 203c 6c61 796f 7574 2063  ty>..  <layout c
-00000160: 6c61 7373 3d22 5147 7269 644c 6179 6f75  lass="QGridLayou
-00000170: 7422 206e 616d 653d 2267 7269 644c 6179  t" name="gridLay
-00000180: 6f75 7422 3e0d 0a20 2020 3c69 7465 6d20  out">..   <item 
-00000190: 726f 773d 2230 2220 636f 6c75 6d6e 3d22  row="0" column="
-000001a0: 3022 3e0d 0a20 2020 203c 6c61 796f 7574  0">..    <layout
-000001b0: 2063 6c61 7373 3d22 5156 426f 784c 6179   class="QVBoxLay
-000001c0: 6f75 7422 206e 616d 653d 2273 7461 6765  out" name="stage
-000001d0: 5f73 7461 7475 735f 7569 223e 0d0a 2020  _status_ui">..  
-000001e0: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
-000001f0: 653d 2273 7061 6369 6e67 223e 0d0a 2020  e="spacing">..  
-00000200: 2020 2020 3c6e 756d 6265 723e 313c 2f6e      <number>1</n
-00000210: 756d 6265 723e 0d0a 2020 2020 203c 2f70  umber>..     </p
-00000220: 726f 7065 7274 793e 0d0a 2020 2020 203c  roperty>..     <
-00000230: 7072 6f70 6572 7479 206e 616d 653d 2273  property name="s
-00000240: 697a 6543 6f6e 7374 7261 696e 7422 3e0d  izeConstraint">.
-00000250: 0a20 2020 2020 203c 656e 756d 3e51 4c61  .      <enum>QLa
-00000260: 796f 7574 3a3a 5365 7444 6566 6175 6c74  yout::SetDefault
-00000270: 436f 6e73 7472 6169 6e74 3c2f 656e 756d  Constraint</enum
-00000280: 3e0d 0a20 2020 2020 3c2f 7072 6f70 6572  >..     </proper
-00000290: 7479 3e0d 0a20 2020 2020 3c70 726f 7065  ty>..     <prope
-000002a0: 7274 7920 6e61 6d65 3d22 6c65 6674 4d61  rty name="leftMa
-000002b0: 7267 696e 223e 0d0a 2020 2020 2020 3c6e  rgin">..      <n
-000002c0: 756d 6265 723e 303c 2f6e 756d 6265 723e  umber>0</number>
-000002d0: 0d0a 2020 2020 203c 2f70 726f 7065 7274  ..     </propert
-000002e0: 793e 0d0a 2020 2020 203c 7072 6f70 6572  y>..     <proper
-000002f0: 7479 206e 616d 653d 2274 6f70 4d61 7267  ty name="topMarg
-00000300: 696e 223e 0d0a 2020 2020 2020 3c6e 756d  in">..      <num
-00000310: 6265 723e 313c 2f6e 756d 6265 723e 0d0a  ber>1</number>..
-00000320: 2020 2020 203c 2f70 726f 7065 7274 793e       </property>
-00000330: 0d0a 2020 2020 203c 7072 6f70 6572 7479  ..     <property
-00000340: 206e 616d 653d 2272 6967 6874 4d61 7267   name="rightMarg
-00000350: 696e 223e 0d0a 2020 2020 2020 3c6e 756d  in">..      <num
-00000360: 6265 723e 313c 2f6e 756d 6265 723e 0d0a  ber>1</number>..
-00000370: 2020 2020 203c 2f70 726f 7065 7274 793e       </property>
-00000380: 0d0a 2020 2020 203c 7072 6f70 6572 7479  ..     <property
-00000390: 206e 616d 653d 2262 6f74 746f 6d4d 6172   name="bottomMar
-000003a0: 6769 6e22 3e0d 0a20 2020 2020 203c 6e75  gin">..      <nu
-000003b0: 6d62 6572 3e30 3c2f 6e75 6d62 6572 3e0d  mber>0</number>.
-000003c0: 0a20 2020 2020 3c2f 7072 6f70 6572 7479  .     </property
-000003d0: 3e0d 0a20 2020 2020 3c69 7465 6d3e 0d0a  >..     <item>..
-000003e0: 2020 2020 2020 3c6c 6179 6f75 7420 636c        <layout cl
-000003f0: 6173 733d 2251 4772 6964 4c61 796f 7574  ass="QGridLayout
-00000400: 2220 6e61 6d65 3d22 7374 6167 655f 7374  " name="stage_st
-00000410: 6174 7573 5f75 695f 6772 6964 223e 0d0a  atus_ui_grid">..
-00000420: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
-00000430: 206e 616d 653d 2272 6967 6874 4d61 7267   name="rightMarg
-00000440: 696e 223e 0d0a 2020 2020 2020 2020 3c6e  in">..        <n
-00000450: 756d 6265 723e 323c 2f6e 756d 6265 723e  umber>2</number>
-00000460: 0d0a 2020 2020 2020 203c 2f70 726f 7065  ..       </prope
-00000470: 7274 793e 0d0a 2020 2020 2020 203c 7072  rty>..       <pr
-00000480: 6f70 6572 7479 206e 616d 653d 2268 6f72  operty name="hor
-00000490: 697a 6f6e 7461 6c53 7061 6369 6e67 223e  izontalSpacing">
-000004a0: 0d0a 2020 2020 2020 2020 3c6e 756d 6265  ..        <numbe
-000004b0: 723e 313c 2f6e 756d 6265 723e 0d0a 2020  r>1</number>..  
-000004c0: 2020 2020 203c 2f70 726f 7065 7274 793e       </property>
-000004d0: 0d0a 2020 2020 2020 203c 7072 6f70 6572  ..       <proper
-000004e0: 7479 206e 616d 653d 2276 6572 7469 6361  ty name="vertica
-000004f0: 6c53 7061 6369 6e67 223e 0d0a 2020 2020  lSpacing">..    
-00000500: 2020 2020 3c6e 756d 6265 723e 323c 2f6e      <number>2</n
-00000510: 756d 6265 723e 0d0a 2020 2020 2020 203c  umber>..       <
-00000520: 2f70 726f 7065 7274 793e 0d0a 2020 2020  /property>..    
-00000530: 2020 203c 6974 656d 2072 6f77 3d22 3222     <item row="2"
-00000540: 2063 6f6c 756d 6e3d 2232 223e 0d0a 2020   column="2">..  
-00000550: 2020 2020 2020 3c77 6964 6765 7420 636c        <widget cl
-00000560: 6173 733d 2251 5075 7368 4275 7474 6f6e  ass="QPushButton
-00000570: 2220 6e61 6d65 3d22 7075 7368 4275 7474  " name="pushButt
-00000580: 6f6e 223e 0d0a 2020 2020 2020 2020 203c  on">..         <
-00000590: 7072 6f70 6572 7479 206e 616d 653d 226d  property name="m
-000005a0: 6178 696d 756d 5369 7a65 223e 0d0a 2020  aximumSize">..  
-000005b0: 2020 2020 2020 2020 3c73 697a 653e 0d0a          <size>..
-000005c0: 2020 2020 2020 2020 2020 203c 7769 6474             <widt
-000005d0: 683e 3430 3c2f 7769 6474 683e 0d0a 2020  h>40</width>..  
-000005e0: 2020 2020 2020 2020 203c 6865 6967 6874           <height
-000005f0: 3e33 393c 2f68 6569 6768 743e 0d0a 2020  >39</height>..  
-00000600: 2020 2020 2020 2020 3c2f 7369 7a65 3e0d          </size>.
-00000610: 0a20 2020 2020 2020 2020 3c2f 7072 6f70  .         </prop
-00000620: 6572 7479 3e0d 0a20 2020 2020 2020 2020  erty>..         
-00000630: 3c70 726f 7065 7274 7920 6e61 6d65 3d22  <property name="
-00000640: 7374 796c 6553 6865 6574 223e 0d0a 2020  styleSheet">..  
-00000650: 2020 2020 2020 2020 3c73 7472 696e 6720          <string 
-00000660: 6e6f 7472 3d22 7472 7565 223e 6261 636b  notr="true">back
-00000670: 6772 6f75 6e64 2d63 6f6c 6f72 203a 2079  ground-color : y
-00000680: 656c 6c6f 773c 2f73 7472 696e 673e 0d0a  ellow</string>..
-00000690: 2020 2020 2020 2020 203c 2f70 726f 7065           </prope
-000006a0: 7274 793e 0d0a 2020 2020 2020 2020 203c  rty>..         <
-000006b0: 7072 6f70 6572 7479 206e 616d 653d 2274  property name="t
-000006c0: 6578 7422 3e0d 0a20 2020 2020 2020 2020  ext">..         
-000006d0: 203c 7374 7269 6e67 2f3e 0d0a 2020 2020   <string/>..    
-000006e0: 2020 2020 203c 2f70 726f 7065 7274 793e       </property>
-000006f0: 0d0a 2020 2020 2020 2020 3c2f 7769 6467  ..        </widg
-00000700: 6574 3e0d 0a20 2020 2020 2020 3c2f 6974  et>..       </it
-00000710: 656d 3e0d 0a20 2020 2020 2020 3c69 7465  em>..       <ite
-00000720: 6d20 726f 773d 2232 2220 636f 6c75 6d6e  m row="2" column
-00000730: 3d22 3022 2063 6f6c 7370 616e 3d22 3222  ="0" colspan="2"
-00000740: 3e0d 0a20 2020 2020 2020 203c 7769 6467  >..        <widg
-00000750: 6574 2063 6c61 7373 3d22 514c 6162 656c  et class="QLabel
-00000760: 2220 6e61 6d65 3d22 7374 6167 655f 736e  " name="stage_sn
-00000770: 223e 0d0a 2020 2020 2020 2020 203c 7072  ">..         <pr
-00000780: 6f70 6572 7479 206e 616d 653d 226d 696e  operty name="min
-00000790: 696d 756d 5369 7a65 223e 0d0a 2020 2020  imumSize">..    
-000007a0: 2020 2020 2020 3c73 697a 653e 0d0a 2020        <size>..  
-000007b0: 2020 2020 2020 2020 203c 7769 6474 683e           <width>
-000007c0: 303c 2f77 6964 7468 3e0d 0a20 2020 2020  0</width>..     
-000007d0: 2020 2020 2020 3c68 6569 6768 743e 3530        <height>50
-000007e0: 3c2f 6865 6967 6874 3e0d 0a20 2020 2020  </height>..     
-000007f0: 2020 2020 203c 2f73 697a 653e 0d0a 2020       </size>..  
-00000800: 2020 2020 2020 203c 2f70 726f 7065 7274         </propert
-00000810: 793e 0d0a 2020 2020 2020 2020 203c 7072  y>..         <pr
-00000820: 6f70 6572 7479 206e 616d 653d 226d 6178  operty name="max
-00000830: 696d 756d 5369 7a65 223e 0d0a 2020 2020  imumSize">..    
-00000840: 2020 2020 2020 3c73 697a 653e 0d0a 2020        <size>..  
-00000850: 2020 2020 2020 2020 203c 7769 6474 683e           <width>
-00000860: 3136 3737 3732 3135 3c2f 7769 6474 683e  16777215</width>
-00000870: 0d0a 2020 2020 2020 2020 2020 203c 6865  ..           <he
-00000880: 6967 6874 3e37 303c 2f68 6569 6768 743e  ight>70</height>
-00000890: 0d0a 2020 2020 2020 2020 2020 3c2f 7369  ..          </si
-000008a0: 7a65 3e0d 0a20 2020 2020 2020 2020 3c2f  ze>..         </
-000008b0: 7072 6f70 6572 7479 3e0d 0a20 2020 2020  property>..     
-000008c0: 2020 2020 3c70 726f 7065 7274 7920 6e61      <property na
-000008d0: 6d65 3d22 7465 7874 223e 0d0a 2020 2020  me="text">..    
-000008e0: 2020 2020 2020 3c73 7472 696e 673e 2053        <string> S
-000008f0: 4e3c 2f73 7472 696e 673e 0d0a 2020 2020  N</string>..    
-00000900: 2020 2020 203c 2f70 726f 7065 7274 793e       </property>
-00000910: 0d0a 2020 2020 2020 2020 3c2f 7769 6467  ..        </widg
-00000920: 6574 3e0d 0a20 2020 2020 2020 3c2f 6974  et>..       </it
-00000930: 656d 3e0d 0a20 2020 2020 2020 3c69 7465  em>..       <ite
-00000940: 6d20 726f 773d 2230 2220 636f 6c75 6d6e  m row="0" column
-00000950: 3d22 3022 2063 6f6c 7370 616e 3d22 3322  ="0" colspan="3"
-00000960: 3e0d 0a20 2020 2020 2020 203c 7769 6467  >..        <widg
-00000970: 6574 2063 6c61 7373 3d22 514c 6162 656c  et class="QLabel
-00000980: 2220 6e61 6d65 3d22 6c61 6265 6c22 3e0d  " name="label">.
-00000990: 0a20 2020 2020 2020 2020 3c70 726f 7065  .         <prope
-000009a0: 7274 7920 6e61 6d65 3d22 6d69 6e69 6d75  rty name="minimu
-000009b0: 6d53 697a 6522 3e0d 0a20 2020 2020 2020  mSize">..       
-000009c0: 2020 203c 7369 7a65 3e0d 0a20 2020 2020     <size>..     
-000009d0: 2020 2020 2020 3c77 6964 7468 3e30 3c2f        <width>0</
-000009e0: 7769 6474 683e 0d0a 2020 2020 2020 2020  width>..        
-000009f0: 2020 203c 6865 6967 6874 3e33 303c 2f68     <height>30</h
-00000a00: 6569 6768 743e 0d0a 2020 2020 2020 2020  eight>..        
-00000a10: 2020 3c2f 7369 7a65 3e0d 0a20 2020 2020    </size>..     
-00000a20: 2020 2020 3c2f 7072 6f70 6572 7479 3e0d      </property>.
-00000a30: 0a20 2020 2020 2020 2020 3c70 726f 7065  .         <prope
-00000a40: 7274 7920 6e61 6d65 3d22 6d61 7869 6d75  rty name="maximu
-00000a50: 6d53 697a 6522 3e0d 0a20 2020 2020 2020  mSize">..       
-00000a60: 2020 203c 7369 7a65 3e0d 0a20 2020 2020     <size>..     
-00000a70: 2020 2020 2020 3c77 6964 7468 3e31 3637        <width>167
-00000a80: 3737 3231 353c 2f77 6964 7468 3e0d 0a20  77215</width>.. 
-00000a90: 2020 2020 2020 2020 2020 3c68 6569 6768            <heigh
-00000aa0: 743e 3330 3c2f 6865 6967 6874 3e0d 0a20  t>30</height>.. 
-00000ab0: 2020 2020 2020 2020 203c 2f73 697a 653e           </size>
-00000ac0: 0d0a 2020 2020 2020 2020 203c 2f70 726f  ..         </pro
-00000ad0: 7065 7274 793e 0d0a 2020 2020 2020 2020  perty>..        
-00000ae0: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
-00000af0: 2274 6578 7422 3e0d 0a20 2020 2020 2020  "text">..       
-00000b00: 2020 203c 7374 7269 6e67 2f3e 0d0a 2020     <string/>..  
-00000b10: 2020 2020 2020 203c 2f70 726f 7065 7274         </propert
-00000b20: 793e 0d0a 2020 2020 2020 2020 3c2f 7769  y>..        </wi
-00000b30: 6467 6574 3e0d 0a20 2020 2020 2020 3c2f  dget>..       </
-00000b40: 6974 656d 3e0d 0a20 2020 2020 2020 3c69  item>..       <i
-00000b50: 7465 6d20 726f 773d 2237 2220 636f 6c75  tem row="7" colu
-00000b60: 6d6e 3d22 3022 2063 6f6c 7370 616e 3d22  mn="0" colspan="
-00000b70: 3322 3e0d 0a20 2020 2020 2020 203c 7769  3">..        <wi
-00000b80: 6467 6574 2063 6c61 7373 3d22 514c 6162  dget class="QLab
-00000b90: 656c 2220 6e61 6d65 3d22 6c61 6265 6c5f  el" name="label_
-00000ba0: 3322 3e0d 0a20 2020 2020 2020 2020 3c70  3">..         <p
-00000bb0: 726f 7065 7274 7920 6e61 6d65 3d22 6d61  roperty name="ma
-00000bc0: 7869 6d75 6d53 697a 6522 3e0d 0a20 2020  ximumSize">..   
-00000bd0: 2020 2020 2020 203c 7369 7a65 3e0d 0a20         <size>.. 
-00000be0: 2020 2020 2020 2020 2020 3c77 6964 7468            <width
-00000bf0: 3e31 3530 3c2f 7769 6474 683e 0d0a 2020  >150</width>..  
-00000c00: 2020 2020 2020 2020 203c 6865 6967 6874           <height
-00000c10: 3e33 303c 2f68 6569 6768 743e 0d0a 2020  >30</height>..  
-00000c20: 2020 2020 2020 2020 3c2f 7369 7a65 3e0d          </size>.
-00000c30: 0a20 2020 2020 2020 2020 3c2f 7072 6f70  .         </prop
-00000c40: 6572 7479 3e0d 0a20 2020 2020 2020 2020  erty>..         
-00000c50: 3c70 726f 7065 7274 7920 6e61 6d65 3d22  <property name="
-00000c60: 7465 7874 223e 0d0a 2020 2020 2020 2020  text">..        
-00000c70: 2020 3c73 7472 696e 672f 3e0d 0a20 2020    <string/>..   
-00000c80: 2020 2020 2020 3c2f 7072 6f70 6572 7479        </property
-00000c90: 3e0d 0a20 2020 2020 2020 203c 2f77 6964  >..        </wid
-00000ca0: 6765 743e 0d0a 2020 2020 2020 203c 2f69  get>..       </i
-00000cb0: 7465 6d3e 0d0a 2020 2020 2020 203c 6974  tem>..       <it
-00000cc0: 656d 2072 6f77 3d22 3422 2063 6f6c 756d  em row="4" colum
-00000cd0: 6e3d 2231 2220 616c 6967 6e6d 656e 743d  n="1" alignment=
-00000ce0: 2251 743a 3a41 6c69 676e 5269 6768 7422  "Qt::AlignRight"
-00000cf0: 3e0d 0a20 2020 2020 2020 203c 7769 6467  >..        <widg
-00000d00: 6574 2063 6c61 7373 3d22 514c 6162 656c  et class="QLabel
-00000d10: 2220 6e61 6d65 3d22 6c6f 6361 6c5f 636f  " name="local_co
-00000d20: 6f72 6473 5f78 223e 0d0a 2020 2020 2020  ords_x">..      
-00000d30: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
-00000d40: 653d 226d 6178 696d 756d 5369 7a65 223e  e="maximumSize">
-00000d50: 0d0a 2020 2020 2020 2020 2020 3c73 697a  ..          <siz
-00000d60: 653e 0d0a 2020 2020 2020 2020 2020 203c  e>..           <
-00000d70: 7769 6474 683e 3136 3737 3732 3135 3c2f  width>16777215</
-00000d80: 7769 6474 683e 0d0a 2020 2020 2020 2020  width>..        
-00000d90: 2020 203c 6865 6967 6874 3e31 3637 3737     <height>16777
-00000da0: 3231 353c 2f68 6569 6768 743e 0d0a 2020  215</height>..  
-00000db0: 2020 2020 2020 2020 3c2f 7369 7a65 3e0d          </size>.
-00000dc0: 0a20 2020 2020 2020 2020 3c2f 7072 6f70  .         </prop
-00000dd0: 6572 7479 3e0d 0a20 2020 2020 2020 2020  erty>..         
-00000de0: 3c70 726f 7065 7274 7920 6e61 6d65 3d22  <property name="
-00000df0: 7465 7874 223e 0d0a 2020 2020 2020 2020  text">..        
-00000e00: 2020 3c73 7472 696e 673e 2d3c 2f73 7472    <string>-</str
-00000e10: 696e 673e 0d0a 2020 2020 2020 2020 203c  ing>..         <
-00000e20: 2f70 726f 7065 7274 793e 0d0a 2020 2020  /property>..    
-00000e30: 2020 2020 3c2f 7769 6467 6574 3e0d 0a20      </widget>.. 
-00000e40: 2020 2020 2020 3c2f 6974 656d 3e0d 0a20        </item>.. 
-00000e50: 2020 2020 2020 3c69 7465 6d20 726f 773d        <item row=
-00000e60: 2231 3122 2063 6f6c 756d 6e3d 2232 223e  "11" column="2">
-00000e70: 0d0a 2020 2020 2020 2020 3c77 6964 6765  ..        <widge
-00000e80: 7420 636c 6173 733d 2251 4c61 6265 6c22  t class="QLabel"
-00000e90: 206e 616d 653d 226c 6162 656c 5f31 3822   name="label_18"
-00000ea0: 3e0d 0a20 2020 2020 2020 2020 3c70 726f  >..         <pro
-00000eb0: 7065 7274 7920 6e61 6d65 3d22 7465 7874  perty name="text
-00000ec0: 223e 0d0a 2020 2020 2020 2020 2020 3c73  ">..          <s
-00000ed0: 7472 696e 673e 20ce bc6d 3c2f 7374 7269  tring> ..m</stri
-00000ee0: 6e67 3e0d 0a20 2020 2020 2020 2020 3c2f  ng>..         </
-00000ef0: 7072 6f70 6572 7479 3e0d 0a20 2020 2020  property>..     
-00000f00: 2020 203c 2f77 6964 6765 743e 0d0a 2020     </widget>..  
-00000f10: 2020 2020 203c 2f69 7465 6d3e 0d0a 2020       </item>..  
-00000f20: 2020 2020 203c 6974 656d 2072 6f77 3d22       <item row="
-00000f30: 3322 2063 6f6c 756d 6e3d 2230 2220 636f  3" column="0" co
-00000f40: 6c73 7061 6e3d 2233 223e 0d0a 2020 2020  lspan="3">..    
-00000f50: 2020 2020 3c77 6964 6765 7420 636c 6173      <widget clas
-00000f60: 733d 2251 4c61 6265 6c22 206e 616d 653d  s="QLabel" name=
-00000f70: 226c 6f63 616c 5f63 6f6f 7264 7322 3e0d  "local_coords">.
-00000f80: 0a20 2020 2020 2020 2020 3c70 726f 7065  .         <prope
-00000f90: 7274 7920 6e61 6d65 3d22 6d69 6e69 6d75  rty name="minimu
-00000fa0: 6d53 697a 6522 3e0d 0a20 2020 2020 2020  mSize">..       
-00000fb0: 2020 203c 7369 7a65 3e0d 0a20 2020 2020     <size>..     
-00000fc0: 2020 2020 2020 3c77 6964 7468 3e30 3c2f        <width>0</
-00000fd0: 7769 6474 683e 0d0a 2020 2020 2020 2020  width>..        
-00000fe0: 2020 203c 6865 6967 6874 3e37 303c 2f68     <height>70</h
-00000ff0: 6569 6768 743e 0d0a 2020 2020 2020 2020  eight>..        
-00001000: 2020 3c2f 7369 7a65 3e0d 0a20 2020 2020    </size>..     
-00001010: 2020 2020 3c2f 7072 6f70 6572 7479 3e0d      </property>.
-00001020: 0a20 2020 2020 2020 2020 3c70 726f 7065  .         <prope
-00001030: 7274 7920 6e61 6d65 3d22 6d61 7869 6d75  rty name="maximu
-00001040: 6d53 697a 6522 3e0d 0a20 2020 2020 2020  mSize">..       
-00001050: 2020 203c 7369 7a65 3e0d 0a20 2020 2020     <size>..     
-00001060: 2020 2020 2020 3c77 6964 7468 3e31 3637        <width>167
-00001070: 3737 3231 353c 2f77 6964 7468 3e0d 0a20  77215</width>.. 
-00001080: 2020 2020 2020 2020 2020 3c68 6569 6768            <heigh
-00001090: 743e 3730 3c2f 6865 6967 6874 3e0d 0a20  t>70</height>.. 
-000010a0: 2020 2020 2020 2020 203c 2f73 697a 653e           </size>
-000010b0: 0d0a 2020 2020 2020 2020 203c 2f70 726f  ..         </pro
-000010c0: 7065 7274 793e 0d0a 2020 2020 2020 2020  perty>..        
-000010d0: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
-000010e0: 2274 6578 7422 3e0d 0a20 2020 2020 2020  "text">..       
-000010f0: 2020 203c 7374 7269 6e67 3e20 4c6f 6361     <string> Loca
-00001100: 6c20 636f 6f72 6473 3c2f 7374 7269 6e67  l coords</string
-00001110: 3e0d 0a20 2020 2020 2020 2020 3c2f 7072  >..         </pr
-00001120: 6f70 6572 7479 3e0d 0a20 2020 2020 2020  operty>..       
-00001130: 203c 2f77 6964 6765 743e 0d0a 2020 2020   </widget>..    
-00001140: 2020 203c 2f69 7465 6d3e 0d0a 2020 2020     </item>..    
-00001150: 2020 203c 6974 656d 2072 6f77 3d22 3422     <item row="4"
-00001160: 2063 6f6c 756d 6e3d 2230 223e 0d0a 2020   column="0">..  
-00001170: 2020 2020 2020 3c77 6964 6765 7420 636c        <widget cl
-00001180: 6173 733d 2251 4c61 6265 6c22 206e 616d  ass="QLabel" nam
-00001190: 653d 226c 6162 656c 5f32 223e 0d0a 2020  e="label_2">..  
-000011a0: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
-000011b0: 206e 616d 653d 226d 6178 696d 756d 5369   name="maximumSi
-000011c0: 7a65 223e 0d0a 2020 2020 2020 2020 2020  ze">..          
-000011d0: 3c73 697a 653e 0d0a 2020 2020 2020 2020  <size>..        
-000011e0: 2020 203c 7769 6474 683e 3136 3737 3732     <width>167772
-000011f0: 3135 3c2f 7769 6474 683e 0d0a 2020 2020  15</width>..    
-00001200: 2020 2020 2020 203c 6865 6967 6874 3e35         <height>5
-00001210: 303c 2f68 6569 6768 743e 0d0a 2020 2020  0</height>..    
-00001220: 2020 2020 2020 3c2f 7369 7a65 3e0d 0a20        </size>.. 
-00001230: 2020 2020 2020 2020 3c2f 7072 6f70 6572          </proper
-00001240: 7479 3e0d 0a20 2020 2020 2020 2020 3c70  ty>..         <p
-00001250: 726f 7065 7274 7920 6e61 6d65 3d22 7465  roperty name="te
-00001260: 7874 223e 0d0a 2020 2020 2020 2020 2020  xt">..          
-00001270: 3c73 7472 696e 673e 2020 583a 3c2f 7374  <string>  X:</st
-00001280: 7269 6e67 3e0d 0a20 2020 2020 2020 2020  ring>..         
-00001290: 3c2f 7072 6f70 6572 7479 3e0d 0a20 2020  </property>..   
-000012a0: 2020 2020 203c 2f77 6964 6765 743e 0d0a       </widget>..
-000012b0: 2020 2020 2020 203c 2f69 7465 6d3e 0d0a         </item>..
-000012c0: 2020 2020 2020 203c 6974 656d 2072 6f77         <item row
-000012d0: 3d22 3922 2063 6f6c 756d 6e3d 2232 223e  ="9" column="2">
-000012e0: 0d0a 2020 2020 2020 2020 3c77 6964 6765  ..        <widge
-000012f0: 7420 636c 6173 733d 2251 4c61 6265 6c22  t class="QLabel"
-00001300: 206e 616d 653d 226c 6162 656c 5f31 3622   name="label_16"
-00001310: 3e0d 0a20 2020 2020 2020 2020 3c70 726f  >..         <pro
-00001320: 7065 7274 7920 6e61 6d65 3d22 7465 7874  perty name="text
-00001330: 223e 0d0a 2020 2020 2020 2020 2020 3c73  ">..          <s
-00001340: 7472 696e 673e 20ce bc6d 3c2f 7374 7269  tring> ..m</stri
-00001350: 6e67 3e0d 0a20 2020 2020 2020 2020 3c2f  ng>..         </
-00001360: 7072 6f70 6572 7479 3e0d 0a20 2020 2020  property>..     
-00001370: 2020 203c 2f77 6964 6765 743e 0d0a 2020     </widget>..  
-00001380: 2020 2020 203c 2f69 7465 6d3e 0d0a 2020       </item>..  
-00001390: 2020 2020 203c 6974 656d 2072 6f77 3d22       <item row="
-000013a0: 3622 2063 6f6c 756d 6e3d 2230 223e 0d0a  6" column="0">..
-000013b0: 2020 2020 2020 2020 3c77 6964 6765 7420          <widget 
-000013c0: 636c 6173 733d 2251 4c61 6265 6c22 206e  class="QLabel" n
-000013d0: 616d 653d 226c 6162 656c 5f31 3122 3e0d  ame="label_11">.
-000013e0: 0a20 2020 2020 2020 2020 3c70 726f 7065  .         <prope
-000013f0: 7274 7920 6e61 6d65 3d22 6d61 7869 6d75  rty name="maximu
-00001400: 6d53 697a 6522 3e0d 0a20 2020 2020 2020  mSize">..       
-00001410: 2020 203c 7369 7a65 3e0d 0a20 2020 2020     <size>..     
-00001420: 2020 2020 2020 3c77 6964 7468 3e31 3637        <width>167
-00001430: 3737 3231 353c 2f77 6964 7468 3e0d 0a20  77215</width>.. 
-00001440: 2020 2020 2020 2020 2020 3c68 6569 6768            <heigh
-00001450: 743e 3530 3c2f 6865 6967 6874 3e0d 0a20  t>50</height>.. 
-00001460: 2020 2020 2020 2020 203c 2f73 697a 653e           </size>
-00001470: 0d0a 2020 2020 2020 2020 203c 2f70 726f  ..         </pro
-00001480: 7065 7274 793e 0d0a 2020 2020 2020 2020  perty>..        
-00001490: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
-000014a0: 2274 6578 7422 3e0d 0a20 2020 2020 2020  "text">..       
-000014b0: 2020 203c 7374 7269 6e67 3e20 205a 3a3c     <string>  Z:<
-000014c0: 2f73 7472 696e 673e 0d0a 2020 2020 2020  /string>..      
-000014d0: 2020 203c 2f70 726f 7065 7274 793e 0d0a     </property>..
-000014e0: 2020 2020 2020 2020 3c2f 7769 6467 6574          </widget
-000014f0: 3e0d 0a20 2020 2020 2020 3c2f 6974 656d  >..       </item
-00001500: 3e0d 0a20 2020 2020 2020 3c69 7465 6d20  >..       <item 
-00001510: 726f 773d 2231 3122 2063 6f6c 756d 6e3d  row="11" column=
-00001520: 2230 223e 0d0a 2020 2020 2020 2020 3c77  "0">..        <w
-00001530: 6964 6765 7420 636c 6173 733d 2251 4c61  idget class="QLa
-00001540: 6265 6c22 206e 616d 653d 226c 6162 656c  bel" name="label
-00001550: 5f37 223e 0d0a 2020 2020 2020 2020 203c  _7">..         <
-00001560: 7072 6f70 6572 7479 206e 616d 653d 226d  property name="m
-00001570: 6178 696d 756d 5369 7a65 223e 0d0a 2020  aximumSize">..  
-00001580: 2020 2020 2020 2020 3c73 697a 653e 0d0a          <size>..
-00001590: 2020 2020 2020 2020 2020 203c 7769 6474             <widt
-000015a0: 683e 3136 3737 3732 3135 3c2f 7769 6474  h>16777215</widt
-000015b0: 683e 0d0a 2020 2020 2020 2020 2020 203c  h>..           <
-000015c0: 6865 6967 6874 3e35 303c 2f68 6569 6768  height>50</heigh
-000015d0: 743e 0d0a 2020 2020 2020 2020 2020 3c2f  t>..          </
-000015e0: 7369 7a65 3e0d 0a20 2020 2020 2020 2020  size>..         
-000015f0: 3c2f 7072 6f70 6572 7479 3e0d 0a20 2020  </property>..   
-00001600: 2020 2020 2020 3c70 726f 7065 7274 7920        <property 
-00001610: 6e61 6d65 3d22 7465 7874 223e 0d0a 2020  name="text">..  
-00001620: 2020 2020 2020 2020 3c73 7472 696e 673e          <string>
-00001630: 2020 5a3a 3c2f 7374 7269 6e67 3e0d 0a20    Z:</string>.. 
-00001640: 2020 2020 2020 2020 3c2f 7072 6f70 6572          </proper
-00001650: 7479 3e0d 0a20 2020 2020 2020 203c 2f77  ty>..        </w
-00001660: 6964 6765 743e 0d0a 2020 2020 2020 203c  idget>..       <
-00001670: 2f69 7465 6d3e 0d0a 2020 2020 2020 203c  /item>..       <
-00001680: 6974 656d 2072 6f77 3d22 3922 2063 6f6c  item row="9" col
-00001690: 756d 6e3d 2230 223e 0d0a 2020 2020 2020  umn="0">..      
-000016a0: 2020 3c77 6964 6765 7420 636c 6173 733d    <widget class=
-000016b0: 2251 4c61 6265 6c22 206e 616d 653d 226c  "QLabel" name="l
-000016c0: 6162 656c 5f35 223e 0d0a 2020 2020 2020  abel_5">..      
-000016d0: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
-000016e0: 653d 226d 6178 696d 756d 5369 7a65 223e  e="maximumSize">
-000016f0: 0d0a 2020 2020 2020 2020 2020 3c73 697a  ..          <siz
-00001700: 653e 0d0a 2020 2020 2020 2020 2020 203c  e>..           <
-00001710: 7769 6474 683e 3136 3737 3732 3135 3c2f  width>16777215</
-00001720: 7769 6474 683e 0d0a 2020 2020 2020 2020  width>..        
-00001730: 2020 203c 6865 6967 6874 3e35 303c 2f68     <height>50</h
-00001740: 6569 6768 743e 0d0a 2020 2020 2020 2020  eight>..        
-00001750: 2020 3c2f 7369 7a65 3e0d 0a20 2020 2020    </size>..     
-00001760: 2020 2020 3c2f 7072 6f70 6572 7479 3e0d      </property>.
-00001770: 0a20 2020 2020 2020 2020 3c70 726f 7065  .         <prope
-00001780: 7274 7920 6e61 6d65 3d22 7465 7874 223e  rty name="text">
-00001790: 0d0a 2020 2020 2020 2020 2020 3c73 7472  ..          <str
-000017a0: 696e 673e 2020 583a 3c2f 7374 7269 6e67  ing>  X:</string
-000017b0: 3e0d 0a20 2020 2020 2020 2020 3c2f 7072  >..         </pr
-000017c0: 6f70 6572 7479 3e0d 0a20 2020 2020 2020  operty>..       
-000017d0: 203c 2f77 6964 6765 743e 0d0a 2020 2020   </widget>..    
-000017e0: 2020 203c 2f69 7465 6d3e 0d0a 2020 2020     </item>..    
-000017f0: 2020 203c 6974 656d 2072 6f77 3d22 3130     <item row="10
-00001800: 2220 636f 6c75 6d6e 3d22 3222 3e0d 0a20  " column="2">.. 
-00001810: 2020 2020 2020 203c 7769 6467 6574 2063         <widget c
-00001820: 6c61 7373 3d22 514c 6162 656c 2220 6e61  lass="QLabel" na
-00001830: 6d65 3d22 6c61 6265 6c5f 3137 223e 0d0a  me="label_17">..
-00001840: 2020 2020 2020 2020 203c 7072 6f70 6572           <proper
-00001850: 7479 206e 616d 653d 2274 6578 7422 3e0d  ty name="text">.
-00001860: 0a20 2020 2020 2020 2020 203c 7374 7269  .          <stri
-00001870: 6e67 3e20 cebc 6d3c 2f73 7472 696e 673e  ng> ..m</string>
-00001880: 0d0a 2020 2020 2020 2020 203c 2f70 726f  ..         </pro
-00001890: 7065 7274 793e 0d0a 2020 2020 2020 2020  perty>..        
-000018a0: 3c2f 7769 6467 6574 3e0d 0a20 2020 2020  </widget>..     
-000018b0: 2020 3c2f 6974 656d 3e0d 0a20 2020 2020    </item>..     
-000018c0: 2020 3c69 7465 6d20 726f 773d 2234 2220    <item row="4" 
-000018d0: 636f 6c75 6d6e 3d22 3222 3e0d 0a20 2020  column="2">..   
-000018e0: 2020 2020 203c 7769 6467 6574 2063 6c61       <widget cla
-000018f0: 7373 3d22 514c 6162 656c 2220 6e61 6d65  ss="QLabel" name
-00001900: 3d22 6c61 6265 6c5f 3133 223e 0d0a 2020  ="label_13">..  
-00001910: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
-00001920: 206e 616d 653d 226d 696e 696d 756d 5369   name="minimumSi
-00001930: 7a65 223e 0d0a 2020 2020 2020 2020 2020  ze">..          
-00001940: 3c73 697a 653e 0d0a 2020 2020 2020 2020  <size>..        
-00001950: 2020 203c 7769 6474 683e 3530 3c2f 7769     <width>50</wi
-00001960: 6474 683e 0d0a 2020 2020 2020 2020 2020  dth>..          
-00001970: 203c 6865 6967 6874 3e30 3c2f 6865 6967   <height>0</heig
-00001980: 6874 3e0d 0a20 2020 2020 2020 2020 203c  ht>..          <
-00001990: 2f73 697a 653e 0d0a 2020 2020 2020 2020  /size>..        
-000019a0: 203c 2f70 726f 7065 7274 793e 0d0a 2020   </property>..  
-000019b0: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
-000019c0: 206e 616d 653d 226d 6178 696d 756d 5369   name="maximumSi
-000019d0: 7a65 223e 0d0a 2020 2020 2020 2020 2020  ze">..          
-000019e0: 3c73 697a 653e 0d0a 2020 2020 2020 2020  <size>..        
-000019f0: 2020 203c 7769 6474 683e 3530 3c2f 7769     <width>50</wi
-00001a00: 6474 683e 0d0a 2020 2020 2020 2020 2020  dth>..          
-00001a10: 203c 6865 6967 6874 3e31 3637 3737 3231   <height>1677721
-00001a20: 353c 2f68 6569 6768 743e 0d0a 2020 2020  5</height>..    
-00001a30: 2020 2020 2020 3c2f 7369 7a65 3e0d 0a20        </size>.. 
-00001a40: 2020 2020 2020 2020 3c2f 7072 6f70 6572          </proper
-00001a50: 7479 3e0d 0a20 2020 2020 2020 2020 3c70  ty>..         <p
-00001a60: 726f 7065 7274 7920 6e61 6d65 3d22 7465  roperty name="te
-00001a70: 7874 223e 0d0a 2020 2020 2020 2020 2020  xt">..          
-00001a80: 3c73 7472 696e 673e 20ce bc6d 3c2f 7374  <string> ..m</st
-00001a90: 7269 6e67 3e0d 0a20 2020 2020 2020 2020  ring>..         
-00001aa0: 3c2f 7072 6f70 6572 7479 3e0d 0a20 2020  </property>..   
-00001ab0: 2020 2020 203c 2f77 6964 6765 743e 0d0a       </widget>..
-00001ac0: 2020 2020 2020 203c 2f69 7465 6d3e 0d0a         </item>..
-00001ad0: 2020 2020 2020 203c 6974 656d 2072 6f77         <item row
-00001ae0: 3d22 3622 2063 6f6c 756d 6e3d 2231 2220  ="6" column="1" 
-00001af0: 616c 6967 6e6d 656e 743d 2251 743a 3a41  alignment="Qt::A
-00001b00: 6c69 676e 5269 6768 7422 3e0d 0a20 2020  lignRight">..   
-00001b10: 2020 2020 203c 7769 6467 6574 2063 6c61       <widget cla
-00001b20: 7373 3d22 514c 6162 656c 2220 6e61 6d65  ss="QLabel" name
-00001b30: 3d22 6c6f 6361 6c5f 636f 6f72 6473 5f7a  ="local_coords_z
-00001b40: 223e 0d0a 2020 2020 2020 2020 203c 7072  ">..         <pr
-00001b50: 6f70 6572 7479 206e 616d 653d 2274 6578  operty name="tex
-00001b60: 7422 3e0d 0a20 2020 2020 2020 2020 203c  t">..          <
-00001b70: 7374 7269 6e67 3e2d 3c2f 7374 7269 6e67  string>-</string
-00001b80: 3e0d 0a20 2020 2020 2020 2020 3c2f 7072  >..         </pr
-00001b90: 6f70 6572 7479 3e0d 0a20 2020 2020 2020  operty>..       
-00001ba0: 203c 2f77 6964 6765 743e 0d0a 2020 2020   </widget>..    
-00001bb0: 2020 203c 2f69 7465 6d3e 0d0a 2020 2020     </item>..    
-00001bc0: 2020 203c 6974 656d 2072 6f77 3d22 3130     <item row="10
-00001bd0: 2220 636f 6c75 6d6e 3d22 3122 2061 6c69  " column="1" ali
-00001be0: 676e 6d65 6e74 3d22 5174 3a3a 416c 6967  gnment="Qt::Alig
-00001bf0: 6e52 6967 6874 223e 0d0a 2020 2020 2020  nRight">..      
-00001c00: 2020 3c77 6964 6765 7420 636c 6173 733d    <widget class=
-00001c10: 2251 4c61 6265 6c22 206e 616d 653d 2267  "QLabel" name="g
-00001c20: 6c6f 6261 6c5f 636f 6f72 6473 5f79 223e  lobal_coords_y">
-00001c30: 0d0a 2020 2020 2020 2020 203c 7072 6f70  ..         <prop
-00001c40: 6572 7479 206e 616d 653d 2274 6578 7422  erty name="text"
-00001c50: 3e0d 0a20 2020 2020 2020 2020 203c 7374  >..          <st
-00001c60: 7269 6e67 3e2d 3c2f 7374 7269 6e67 3e0d  ring>-</string>.
-00001c70: 0a20 2020 2020 2020 2020 3c2f 7072 6f70  .         </prop
-00001c80: 6572 7479 3e0d 0a20 2020 2020 2020 203c  erty>..        <
-00001c90: 2f77 6964 6765 743e 0d0a 2020 2020 2020  /widget>..      
-00001ca0: 203c 2f69 7465 6d3e 0d0a 2020 2020 2020   </item>..      
-00001cb0: 203c 6974 656d 2072 6f77 3d22 3522 2063   <item row="5" c
-00001cc0: 6f6c 756d 6e3d 2231 2220 616c 6967 6e6d  olumn="1" alignm
-00001cd0: 656e 743d 2251 743a 3a41 6c69 676e 5269  ent="Qt::AlignRi
-00001ce0: 6768 7422 3e0d 0a20 2020 2020 2020 203c  ght">..        <
-00001cf0: 7769 6467 6574 2063 6c61 7373 3d22 514c  widget class="QL
-00001d00: 6162 656c 2220 6e61 6d65 3d22 6c6f 6361  abel" name="loca
-00001d10: 6c5f 636f 6f72 6473 5f79 223e 0d0a 2020  l_coords_y">..  
-00001d20: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
-00001d30: 206e 616d 653d 2274 6578 7422 3e0d 0a20   name="text">.. 
-00001d40: 2020 2020 2020 2020 203c 7374 7269 6e67           <string
-00001d50: 3e2d 3c2f 7374 7269 6e67 3e0d 0a20 2020  >-</string>..   
-00001d60: 2020 2020 2020 3c2f 7072 6f70 6572 7479        </property
-00001d70: 3e0d 0a20 2020 2020 2020 203c 2f77 6964  >..        </wid
-00001d80: 6765 743e 0d0a 2020 2020 2020 203c 2f69  get>..       </i
-00001d90: 7465 6d3e 0d0a 2020 2020 2020 203c 6974  tem>..       <it
-00001da0: 656d 2072 6f77 3d22 3922 2063 6f6c 756d  em row="9" colum
-00001db0: 6e3d 2231 2220 616c 6967 6e6d 656e 743d  n="1" alignment=
-00001dc0: 2251 743a 3a41 6c69 676e 5269 6768 7422  "Qt::AlignRight"
-00001dd0: 3e0d 0a20 2020 2020 2020 203c 7769 6467  >..        <widg
-00001de0: 6574 2063 6c61 7373 3d22 514c 6162 656c  et class="QLabel
-00001df0: 2220 6e61 6d65 3d22 676c 6f62 616c 5f63  " name="global_c
-00001e00: 6f6f 7264 735f 7822 3e0d 0a20 2020 2020  oords_x">..     
-00001e10: 2020 2020 3c70 726f 7065 7274 7920 6e61      <property na
-00001e20: 6d65 3d22 7465 7874 223e 0d0a 2020 2020  me="text">..    
-00001e30: 2020 2020 2020 3c73 7472 696e 673e 2d3c        <string>-<
-00001e40: 2f73 7472 696e 673e 0d0a 2020 2020 2020  /string>..      
-00001e50: 2020 203c 2f70 726f 7065 7274 793e 0d0a     </property>..
-00001e60: 2020 2020 2020 2020 3c2f 7769 6467 6574          </widget
-00001e70: 3e0d 0a20 2020 2020 2020 3c2f 6974 656d  >..       </item
-00001e80: 3e0d 0a20 2020 2020 2020 3c69 7465 6d20  >..       <item 
-00001e90: 726f 773d 2238 2220 636f 6c75 6d6e 3d22  row="8" column="
-00001ea0: 3022 2063 6f6c 7370 616e 3d22 3322 3e0d  0" colspan="3">.
-00001eb0: 0a20 2020 2020 2020 203c 7769 6467 6574  .        <widget
-00001ec0: 2063 6c61 7373 3d22 514c 6162 656c 2220   class="QLabel" 
-00001ed0: 6e61 6d65 3d22 676c 6f62 616c 5f63 6f6f  name="global_coo
-00001ee0: 7264 7322 3e0d 0a20 2020 2020 2020 2020  rds">..         
-00001ef0: 3c70 726f 7065 7274 7920 6e61 6d65 3d22  <property name="
-00001f00: 6d69 6e69 6d75 6d53 697a 6522 3e0d 0a20  minimumSize">.. 
-00001f10: 2020 2020 2020 2020 203c 7369 7a65 3e0d           <size>.
-00001f20: 0a20 2020 2020 2020 2020 2020 3c77 6964  .           <wid
-00001f30: 7468 3e30 3c2f 7769 6474 683e 0d0a 2020  th>0</width>..  
-00001f40: 2020 2020 2020 2020 203c 6865 6967 6874           <height
-00001f50: 3e37 303c 2f68 6569 6768 743e 0d0a 2020  >70</height>..  
-00001f60: 2020 2020 2020 2020 3c2f 7369 7a65 3e0d          </size>.
-00001f70: 0a20 2020 2020 2020 2020 3c2f 7072 6f70  .         </prop
-00001f80: 6572 7479 3e0d 0a20 2020 2020 2020 2020  erty>..         
-00001f90: 3c70 726f 7065 7274 7920 6e61 6d65 3d22  <property name="
-00001fa0: 6d61 7869 6d75 6d53 697a 6522 3e0d 0a20  maximumSize">.. 
-00001fb0: 2020 2020 2020 2020 203c 7369 7a65 3e0d           <size>.
-00001fc0: 0a20 2020 2020 2020 2020 2020 3c77 6964  .           <wid
-00001fd0: 7468 3e31 3637 3737 3231 353c 2f77 6964  th>16777215</wid
-00001fe0: 7468 3e0d 0a20 2020 2020 2020 2020 2020  th>..           
-00001ff0: 3c68 6569 6768 743e 3730 3c2f 6865 6967  <height>70</heig
-00002000: 6874 3e0d 0a20 2020 2020 2020 2020 203c  ht>..          <
-00002010: 2f73 697a 653e 0d0a 2020 2020 2020 2020  /size>..        
-00002020: 203c 2f70 726f 7065 7274 793e 0d0a 2020   </property>..  
-00002030: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
-00002040: 206e 616d 653d 2274 6578 7422 3e0d 0a20   name="text">.. 
-00002050: 2020 2020 2020 2020 203c 7374 7269 6e67           <string
-00002060: 3e20 476c 6f62 616c 2063 6f6f 7264 733c  > Global coords<
-00002070: 2f73 7472 696e 673e 0d0a 2020 2020 2020  /string>..      
-00002080: 2020 203c 2f70 726f 7065 7274 793e 0d0a     </property>..
-00002090: 2020 2020 2020 2020 3c2f 7769 6467 6574          </widget
-000020a0: 3e0d 0a20 2020 2020 2020 3c2f 6974 656d  >..       </item
-000020b0: 3e0d 0a20 2020 2020 2020 3c69 7465 6d20  >..       <item 
-000020c0: 726f 773d 2235 2220 636f 6c75 6d6e 3d22  row="5" column="
-000020d0: 3022 3e0d 0a20 2020 2020 2020 203c 7769  0">..        <wi
-000020e0: 6467 6574 2063 6c61 7373 3d22 514c 6162  dget class="QLab
-000020f0: 656c 2220 6e61 6d65 3d22 6c61 6265 6c5f  el" name="label_
-00002100: 3130 223e 0d0a 2020 2020 2020 2020 203c  10">..         <
-00002110: 7072 6f70 6572 7479 206e 616d 653d 226d  property name="m
-00002120: 6178 696d 756d 5369 7a65 223e 0d0a 2020  aximumSize">..  
-00002130: 2020 2020 2020 2020 3c73 697a 653e 0d0a          <size>..
-00002140: 2020 2020 2020 2020 2020 203c 7769 6474             <widt
-00002150: 683e 3136 3737 3732 3135 3c2f 7769 6474  h>16777215</widt
-00002160: 683e 0d0a 2020 2020 2020 2020 2020 203c  h>..           <
-00002170: 6865 6967 6874 3e35 303c 2f68 6569 6768  height>50</heigh
-00002180: 743e 0d0a 2020 2020 2020 2020 2020 3c2f  t>..          </
-00002190: 7369 7a65 3e0d 0a20 2020 2020 2020 2020  size>..         
-000021a0: 3c2f 7072 6f70 6572 7479 3e0d 0a20 2020  </property>..   
-000021b0: 2020 2020 2020 3c70 726f 7065 7274 7920        <property 
-000021c0: 6e61 6d65 3d22 7465 7874 223e 0d0a 2020  name="text">..  
-000021d0: 2020 2020 2020 2020 3c73 7472 696e 673e          <string>
-000021e0: 2020 593a 3c2f 7374 7269 6e67 3e0d 0a20    Y:</string>.. 
-000021f0: 2020 2020 2020 2020 3c2f 7072 6f70 6572          </proper
-00002200: 7479 3e0d 0a20 2020 2020 2020 203c 2f77  ty>..        </w
-00002210: 6964 6765 743e 0d0a 2020 2020 2020 203c  idget>..       <
-00002220: 2f69 7465 6d3e 0d0a 2020 2020 2020 203c  /item>..       <
-00002230: 6974 656d 2072 6f77 3d22 3131 2220 636f  item row="11" co
-00002240: 6c75 6d6e 3d22 3122 2061 6c69 676e 6d65  lumn="1" alignme
-00002250: 6e74 3d22 5174 3a3a 416c 6967 6e52 6967  nt="Qt::AlignRig
-00002260: 6874 223e 0d0a 2020 2020 2020 2020 3c77  ht">..        <w
-00002270: 6964 6765 7420 636c 6173 733d 2251 4c61  idget class="QLa
-00002280: 6265 6c22 206e 616d 653d 2267 6c6f 6261  bel" name="globa
-00002290: 6c5f 636f 6f72 6473 5f7a 223e 0d0a 2020  l_coords_z">..  
-000022a0: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
-000022b0: 206e 616d 653d 2274 6578 7422 3e0d 0a20   name="text">.. 
-000022c0: 2020 2020 2020 2020 203c 7374 7269 6e67           <string
-000022d0: 3e2d 3c2f 7374 7269 6e67 3e0d 0a20 2020  >-</string>..   
-000022e0: 2020 2020 2020 3c2f 7072 6f70 6572 7479        </property
-000022f0: 3e0d 0a20 2020 2020 2020 203c 2f77 6964  >..        </wid
-00002300: 6765 743e 0d0a 2020 2020 2020 203c 2f69  get>..       </i
-00002310: 7465 6d3e 0d0a 2020 2020 2020 203c 6974  tem>..       <it
-00002320: 656d 2072 6f77 3d22 3122 2063 6f6c 756d  em row="1" colum
-00002330: 6e3d 2230 2220 636f 6c73 7061 6e3d 2233  n="0" colspan="3
-00002340: 223e 0d0a 2020 2020 2020 2020 3c77 6964  ">..        <wid
-00002350: 6765 7420 636c 6173 733d 2251 436f 6d62  get class="QComb
-00002360: 6f42 6f78 2220 6e61 6d65 3d22 7374 6167  oBox" name="stag
-00002370: 655f 7365 6c65 6374 6f72 223e 0d0a 2020  e_selector">..  
-00002380: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
-00002390: 206e 616d 653d 226d 6178 696d 756d 5369   name="maximumSi
-000023a0: 7a65 223e 0d0a 2020 2020 2020 2020 2020  ze">..          
-000023b0: 3c73 697a 653e 0d0a 2020 2020 2020 2020  <size>..        
-000023c0: 2020 203c 7769 6474 683e 3136 3737 3732     <width>167772
-000023d0: 3135 3c2f 7769 6474 683e 0d0a 2020 2020  15</width>..    
-000023e0: 2020 2020 2020 203c 6865 6967 6874 3e37         <height>7
-000023f0: 303c 2f68 6569 6768 743e 0d0a 2020 2020  0</height>..    
-00002400: 2020 2020 2020 3c2f 7369 7a65 3e0d 0a20        </size>.. 
-00002410: 2020 2020 2020 2020 3c2f 7072 6f70 6572          </proper
-00002420: 7479 3e0d 0a20 2020 2020 2020 203c 2f77  ty>..        </w
-00002430: 6964 6765 743e 0d0a 2020 2020 2020 203c  idget>..       <
-00002440: 2f69 7465 6d3e 0d0a 2020 2020 2020 203c  /item>..       <
-00002450: 6974 656d 2072 6f77 3d22 3130 2220 636f  item row="10" co
-00002460: 6c75 6d6e 3d22 3022 3e0d 0a20 2020 2020  lumn="0">..     
-00002470: 2020 203c 7769 6467 6574 2063 6c61 7373     <widget class
-00002480: 3d22 514c 6162 656c 2220 6e61 6d65 3d22  ="QLabel" name="
-00002490: 6c61 6265 6c5f 3622 3e0d 0a20 2020 2020  label_6">..     
-000024a0: 2020 2020 3c70 726f 7065 7274 7920 6e61      <property na
-000024b0: 6d65 3d22 6d61 7869 6d75 6d53 697a 6522  me="maximumSize"
-000024c0: 3e0d 0a20 2020 2020 2020 2020 203c 7369  >..          <si
-000024d0: 7a65 3e0d 0a20 2020 2020 2020 2020 2020  ze>..           
-000024e0: 3c77 6964 7468 3e31 3637 3737 3231 353c  <width>16777215<
-000024f0: 2f77 6964 7468 3e0d 0a20 2020 2020 2020  /width>..       
-00002500: 2020 2020 3c68 6569 6768 743e 3530 3c2f      <height>50</
-00002510: 6865 6967 6874 3e0d 0a20 2020 2020 2020  height>..       
-00002520: 2020 203c 2f73 697a 653e 0d0a 2020 2020     </size>..    
-00002530: 2020 2020 203c 2f70 726f 7065 7274 793e       </property>
-00002540: 0d0a 2020 2020 2020 2020 203c 7072 6f70  ..         <prop
-00002550: 6572 7479 206e 616d 653d 2274 6578 7422  erty name="text"
-00002560: 3e0d 0a20 2020 2020 2020 2020 203c 7374  >..          <st
-00002570: 7269 6e67 3e20 2059 3a3c 2f73 7472 696e  ring>  Y:</strin
-00002580: 673e 0d0a 2020 2020 2020 2020 203c 2f70  g>..         </p
-00002590: 726f 7065 7274 793e 0d0a 2020 2020 2020  roperty>..      
-000025a0: 2020 3c2f 7769 6467 6574 3e0d 0a20 2020    </widget>..   
-000025b0: 2020 2020 3c2f 6974 656d 3e0d 0a20 2020      </item>..   
-000025c0: 2020 2020 3c69 7465 6d20 726f 773d 2235      <item row="5
-000025d0: 2220 636f 6c75 6d6e 3d22 3222 3e0d 0a20  " column="2">.. 
-000025e0: 2020 2020 2020 203c 7769 6467 6574 2063         <widget c
-000025f0: 6c61 7373 3d22 514c 6162 656c 2220 6e61  lass="QLabel" na
-00002600: 6d65 3d22 6c61 6265 6c5f 3134 223e 0d0a  me="label_14">..
-00002610: 2020 2020 2020 2020 203c 7072 6f70 6572           <proper
-00002620: 7479 206e 616d 653d 2274 6578 7422 3e0d  ty name="text">.
-00002630: 0a20 2020 2020 2020 2020 203c 7374 7269  .          <stri
-00002640: 6e67 3e20 cebc 6d3c 2f73 7472 696e 673e  ng> ..m</string>
-00002650: 0d0a 2020 2020 2020 2020 203c 2f70 726f  ..         </pro
-00002660: 7065 7274 793e 0d0a 2020 2020 2020 2020  perty>..        
-00002670: 3c2f 7769 6467 6574 3e0d 0a20 2020 2020  </widget>..     
-00002680: 2020 3c2f 6974 656d 3e0d 0a20 2020 2020    </item>..     
-00002690: 2020 3c69 7465 6d20 726f 773d 2231 3222    <item row="12"
-000026a0: 2063 6f6c 756d 6e3d 2230 2220 636f 6c73   column="0" cols
-000026b0: 7061 6e3d 2233 223e 0d0a 2020 2020 2020  pan="3">..      
-000026c0: 2020 3c77 6964 6765 7420 636c 6173 733d    <widget class=
-000026d0: 2251 4c61 6265 6c22 206e 616d 653d 226c  "QLabel" name="l
-000026e0: 6162 656c 5f34 223e 0d0a 2020 2020 2020  abel_4">..      
-000026f0: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
-00002700: 653d 226d 6178 696d 756d 5369 7a65 223e  e="maximumSize">
-00002710: 0d0a 2020 2020 2020 2020 2020 3c73 697a  ..          <siz
-00002720: 653e 0d0a 2020 2020 2020 2020 2020 203c  e>..           <
-00002730: 7769 6474 683e 3136 3737 3732 3135 3c2f  width>16777215</
-00002740: 7769 6474 683e 0d0a 2020 2020 2020 2020  width>..        
-00002750: 2020 203c 6865 6967 6874 3e31 303c 2f68     <height>10</h
-00002760: 6569 6768 743e 0d0a 2020 2020 2020 2020  eight>..        
-00002770: 2020 3c2f 7369 7a65 3e0d 0a20 2020 2020    </size>..     
-00002780: 2020 2020 3c2f 7072 6f70 6572 7479 3e0d      </property>.
-00002790: 0a20 2020 2020 2020 2020 3c70 726f 7065  .         <prope
-000027a0: 7274 7920 6e61 6d65 3d22 7465 7874 223e  rty name="text">
-000027b0: 0d0a 2020 2020 2020 2020 2020 3c73 7472  ..          <str
-000027c0: 696e 672f 3e0d 0a20 2020 2020 2020 2020  ing/>..         
-000027d0: 3c2f 7072 6f70 6572 7479 3e0d 0a20 2020  </property>..   
-000027e0: 2020 2020 203c 2f77 6964 6765 743e 0d0a       </widget>..
-000027f0: 2020 2020 2020 203c 2f69 7465 6d3e 0d0a         </item>..
-00002800: 2020 2020 2020 203c 6974 656d 2072 6f77         <item row
-00002810: 3d22 3622 2063 6f6c 756d 6e3d 2232 223e  ="6" column="2">
-00002820: 0d0a 2020 2020 2020 2020 3c77 6964 6765  ..        <widge
-00002830: 7420 636c 6173 733d 2251 4c61 6265 6c22  t class="QLabel"
-00002840: 206e 616d 653d 226c 6162 656c 5f31 3522   name="label_15"
-00002850: 3e0d 0a20 2020 2020 2020 2020 3c70 726f  >..         <pro
-00002860: 7065 7274 7920 6e61 6d65 3d22 6d61 7869  perty name="maxi
-00002870: 6d75 6d53 697a 6522 3e0d 0a20 2020 2020  mumSize">..     
-00002880: 2020 2020 203c 7369 7a65 3e0d 0a20 2020       <size>..   
-00002890: 2020 2020 2020 2020 3c77 6964 7468 3e34          <width>4
-000028a0: 303c 2f77 6964 7468 3e0d 0a20 2020 2020  0</width>..     
-000028b0: 2020 2020 2020 3c68 6569 6768 743e 3136        <height>16
-000028c0: 3737 3732 3135 3c2f 6865 6967 6874 3e0d  777215</height>.
-000028d0: 0a20 2020 2020 2020 2020 203c 2f73 697a  .          </siz
-000028e0: 653e 0d0a 2020 2020 2020 2020 203c 2f70  e>..         </p
-000028f0: 726f 7065 7274 793e 0d0a 2020 2020 2020  roperty>..      
-00002900: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
-00002910: 653d 2274 6578 7422 3e0d 0a20 2020 2020  e="text">..     
-00002920: 2020 2020 203c 7374 7269 6e67 3e20 cebc       <string> ..
-00002930: 6d3c 2f73 7472 696e 673e 0d0a 2020 2020  m</string>..    
-00002940: 2020 2020 203c 2f70 726f 7065 7274 793e       </property>
-00002950: 0d0a 2020 2020 2020 2020 3c2f 7769 6467  ..        </widg
-00002960: 6574 3e0d 0a20 2020 2020 2020 3c2f 6974  et>..       </it
-00002970: 656d 3e0d 0a20 2020 2020 203c 2f6c 6179  em>..      </lay
-00002980: 6f75 743e 0d0a 2020 2020 203c 2f69 7465  out>..     </ite
-00002990: 6d3e 0d0a 2020 2020 3c2f 6c61 796f 7574  m>..    </layout
-000029a0: 3e0d 0a20 2020 3c2f 6974 656d 3e0d 0a20  >..   </item>.. 
-000029b0: 203c 2f6c 6179 6f75 743e 0d0a 203c 2f77   </layout>.. </w
-000029c0: 6964 6765 743e 0d0a 203c 7265 736f 7572  idget>.. <resour
-000029d0: 6365 732f 3e0d 0a20 3c63 6f6e 6e65 6374  ces/>.. <connect
-000029e0: 696f 6e73 2f3e 0d0a 3c2f 7569 3e0d 0a    ions/>..</ui>..
+00000020: 462d 3822 3f3e 0a3c 7569 2076 6572 7369  F-8"?>.<ui versi
+00000030: 6f6e 3d22 342e 3022 3e0a 203c 636c 6173  on="4.0">. <clas
+00000040: 733e 466f 726d 3c2f 636c 6173 733e 0a20  s>Form</class>. 
+00000050: 3c77 6964 6765 7420 636c 6173 733d 2251  <widget class="Q
+00000060: 5769 6467 6574 2220 6e61 6d65 3d22 466f  Widget" name="Fo
+00000070: 726d 223e 0a20 203c 7072 6f70 6572 7479  rm">.  <property
+00000080: 206e 616d 653d 2267 656f 6d65 7472 7922   name="geometry"
+00000090: 3e0a 2020 203c 7265 6374 3e0a 2020 2020  >.   <rect>.    
+000000a0: 3c78 3e30 3c2f 783e 0a20 2020 203c 793e  <x>0</x>.    <y>
+000000b0: 303c 2f79 3e0a 2020 2020 3c77 6964 7468  0</y>.    <width
+000000c0: 3e35 3235 3c2f 7769 6474 683e 0a20 2020  >525</width>.   
+000000d0: 203c 6865 6967 6874 3e37 3534 3c2f 6865   <height>754</he
+000000e0: 6967 6874 3e0a 2020 203c 2f72 6563 743e  ight>.   </rect>
+000000f0: 0a20 203c 2f70 726f 7065 7274 793e 0a20  .  </property>. 
+00000100: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
+00000110: 2277 696e 646f 7754 6974 6c65 223e 0a20  "windowTitle">. 
+00000120: 2020 3c73 7472 696e 673e 466f 726d 3c2f    <string>Form</
+00000130: 7374 7269 6e67 3e0a 2020 3c2f 7072 6f70  string>.  </prop
+00000140: 6572 7479 3e0a 2020 3c6c 6179 6f75 7420  erty>.  <layout 
+00000150: 636c 6173 733d 2251 4772 6964 4c61 796f  class="QGridLayo
+00000160: 7574 2220 6e61 6d65 3d22 6772 6964 4c61  ut" name="gridLa
+00000170: 796f 7574 223e 0a20 2020 3c69 7465 6d20  yout">.   <item 
+00000180: 726f 773d 2230 2220 636f 6c75 6d6e 3d22  row="0" column="
+00000190: 3022 3e0a 2020 2020 3c6c 6179 6f75 7420  0">.    <layout 
+000001a0: 636c 6173 733d 2251 5642 6f78 4c61 796f  class="QVBoxLayo
+000001b0: 7574 2220 6e61 6d65 3d22 7374 6167 655f  ut" name="stage_
+000001c0: 7374 6174 7573 5f75 6922 3e0a 2020 2020  status_ui">.    
+000001d0: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
+000001e0: 2273 7061 6369 6e67 223e 0a20 2020 2020  "spacing">.     
+000001f0: 203c 6e75 6d62 6572 3e31 3c2f 6e75 6d62   <number>1</numb
+00000200: 6572 3e0a 2020 2020 203c 2f70 726f 7065  er>.     </prope
+00000210: 7274 793e 0a20 2020 2020 3c70 726f 7065  rty>.     <prope
+00000220: 7274 7920 6e61 6d65 3d22 7369 7a65 436f  rty name="sizeCo
+00000230: 6e73 7472 6169 6e74 223e 0a20 2020 2020  nstraint">.     
+00000240: 203c 656e 756d 3e51 4c61 796f 7574 3a3a   <enum>QLayout::
+00000250: 5365 7444 6566 6175 6c74 436f 6e73 7472  SetDefaultConstr
+00000260: 6169 6e74 3c2f 656e 756d 3e0a 2020 2020  aint</enum>.    
+00000270: 203c 2f70 726f 7065 7274 793e 0a20 2020   </property>.   
+00000280: 2020 3c70 726f 7065 7274 7920 6e61 6d65    <property name
+00000290: 3d22 6c65 6674 4d61 7267 696e 223e 0a20  ="leftMargin">. 
+000002a0: 2020 2020 203c 6e75 6d62 6572 3e30 3c2f       <number>0</
+000002b0: 6e75 6d62 6572 3e0a 2020 2020 203c 2f70  number>.     </p
+000002c0: 726f 7065 7274 793e 0a20 2020 2020 3c70  roperty>.     <p
+000002d0: 726f 7065 7274 7920 6e61 6d65 3d22 746f  roperty name="to
+000002e0: 704d 6172 6769 6e22 3e0a 2020 2020 2020  pMargin">.      
+000002f0: 3c6e 756d 6265 723e 313c 2f6e 756d 6265  <number>1</numbe
+00000300: 723e 0a20 2020 2020 3c2f 7072 6f70 6572  r>.     </proper
+00000310: 7479 3e0a 2020 2020 203c 7072 6f70 6572  ty>.     <proper
+00000320: 7479 206e 616d 653d 2272 6967 6874 4d61  ty name="rightMa
+00000330: 7267 696e 223e 0a20 2020 2020 203c 6e75  rgin">.      <nu
+00000340: 6d62 6572 3e31 3c2f 6e75 6d62 6572 3e0a  mber>1</number>.
+00000350: 2020 2020 203c 2f70 726f 7065 7274 793e       </property>
+00000360: 0a20 2020 2020 3c70 726f 7065 7274 7920  .     <property 
+00000370: 6e61 6d65 3d22 626f 7474 6f6d 4d61 7267  name="bottomMarg
+00000380: 696e 223e 0a20 2020 2020 203c 6e75 6d62  in">.      <numb
+00000390: 6572 3e30 3c2f 6e75 6d62 6572 3e0a 2020  er>0</number>.  
+000003a0: 2020 203c 2f70 726f 7065 7274 793e 0a20     </property>. 
+000003b0: 2020 2020 3c69 7465 6d3e 0a20 2020 2020      <item>.     
+000003c0: 203c 6c61 796f 7574 2063 6c61 7373 3d22   <layout class="
+000003d0: 5147 7269 644c 6179 6f75 7422 206e 616d  QGridLayout" nam
+000003e0: 653d 2273 7461 6765 5f73 7461 7475 735f  e="stage_status_
+000003f0: 7569 5f67 7269 6422 3e0a 2020 2020 2020  ui_grid">.      
+00000400: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
+00000410: 2272 6967 6874 4d61 7267 696e 223e 0a20  "rightMargin">. 
+00000420: 2020 2020 2020 203c 6e75 6d62 6572 3e32         <number>2
+00000430: 3c2f 6e75 6d62 6572 3e0a 2020 2020 2020  </number>.      
+00000440: 203c 2f70 726f 7065 7274 793e 0a20 2020   </property>.   
+00000450: 2020 2020 3c70 726f 7065 7274 7920 6e61      <property na
+00000460: 6d65 3d22 686f 7269 7a6f 6e74 616c 5370  me="horizontalSp
+00000470: 6163 696e 6722 3e0a 2020 2020 2020 2020  acing">.        
+00000480: 3c6e 756d 6265 723e 313c 2f6e 756d 6265  <number>1</numbe
+00000490: 723e 0a20 2020 2020 2020 3c2f 7072 6f70  r>.       </prop
+000004a0: 6572 7479 3e0a 2020 2020 2020 203c 7072  erty>.       <pr
+000004b0: 6f70 6572 7479 206e 616d 653d 2276 6572  operty name="ver
+000004c0: 7469 6361 6c53 7061 6369 6e67 223e 0a20  ticalSpacing">. 
+000004d0: 2020 2020 2020 203c 6e75 6d62 6572 3e32         <number>2
+000004e0: 3c2f 6e75 6d62 6572 3e0a 2020 2020 2020  </number>.      
+000004f0: 203c 2f70 726f 7065 7274 793e 0a20 2020   </property>.   
+00000500: 2020 2020 3c69 7465 6d20 726f 773d 2232      <item row="2
+00000510: 2220 636f 6c75 6d6e 3d22 3222 3e0a 2020  " column="2">.  
+00000520: 2020 2020 2020 3c77 6964 6765 7420 636c        <widget cl
+00000530: 6173 733d 2251 5075 7368 4275 7474 6f6e  ass="QPushButton
+00000540: 2220 6e61 6d65 3d22 7075 7368 4275 7474  " name="pushButt
+00000550: 6f6e 223e 0a20 2020 2020 2020 2020 3c70  on">.         <p
+00000560: 726f 7065 7274 7920 6e61 6d65 3d22 6d61  roperty name="ma
+00000570: 7869 6d75 6d53 697a 6522 3e0a 2020 2020  ximumSize">.    
+00000580: 2020 2020 2020 3c73 697a 653e 0a20 2020        <size>.   
+00000590: 2020 2020 2020 2020 3c77 6964 7468 3e34          <width>4
+000005a0: 303c 2f77 6964 7468 3e0a 2020 2020 2020  0</width>.      
+000005b0: 2020 2020 203c 6865 6967 6874 3e33 393c       <height>39<
+000005c0: 2f68 6569 6768 743e 0a20 2020 2020 2020  /height>.       
+000005d0: 2020 203c 2f73 697a 653e 0a20 2020 2020     </size>.     
+000005e0: 2020 2020 3c2f 7072 6f70 6572 7479 3e0a      </property>.
+000005f0: 2020 2020 2020 2020 203c 7072 6f70 6572           <proper
+00000600: 7479 206e 616d 653d 2273 7479 6c65 5368  ty name="styleSh
+00000610: 6565 7422 3e0a 2020 2020 2020 2020 2020  eet">.          
+00000620: 3c73 7472 696e 6720 6e6f 7472 3d22 7472  <string notr="tr
+00000630: 7565 223e 6261 636b 6772 6f75 6e64 2d63  ue">background-c
+00000640: 6f6c 6f72 203a 2079 656c 6c6f 773c 2f73  olor : yellow</s
+00000650: 7472 696e 673e 0a20 2020 2020 2020 2020  tring>.         
+00000660: 3c2f 7072 6f70 6572 7479 3e0a 2020 2020  </property>.    
+00000670: 2020 2020 203c 7072 6f70 6572 7479 206e       <property n
+00000680: 616d 653d 2274 6578 7422 3e0a 2020 2020  ame="text">.    
+00000690: 2020 2020 2020 3c73 7472 696e 672f 3e0a        <string/>.
+000006a0: 2020 2020 2020 2020 203c 2f70 726f 7065           </prope
+000006b0: 7274 793e 0a20 2020 2020 2020 203c 2f77  rty>.        </w
+000006c0: 6964 6765 743e 0a20 2020 2020 2020 3c2f  idget>.       </
+000006d0: 6974 656d 3e0a 2020 2020 2020 203c 6974  item>.       <it
+000006e0: 656d 2072 6f77 3d22 3222 2063 6f6c 756d  em row="2" colum
+000006f0: 6e3d 2230 2220 636f 6c73 7061 6e3d 2232  n="0" colspan="2
+00000700: 223e 0a20 2020 2020 2020 203c 7769 6467  ">.        <widg
+00000710: 6574 2063 6c61 7373 3d22 514c 6162 656c  et class="QLabel
+00000720: 2220 6e61 6d65 3d22 7374 6167 655f 736e  " name="stage_sn
+00000730: 223e 0a20 2020 2020 2020 2020 3c70 726f  ">.         <pro
+00000740: 7065 7274 7920 6e61 6d65 3d22 6d69 6e69  perty name="mini
+00000750: 6d75 6d53 697a 6522 3e0a 2020 2020 2020  mumSize">.      
+00000760: 2020 2020 3c73 697a 653e 0a20 2020 2020      <size>.     
+00000770: 2020 2020 2020 3c77 6964 7468 3e30 3c2f        <width>0</
+00000780: 7769 6474 683e 0a20 2020 2020 2020 2020  width>.         
+00000790: 2020 3c68 6569 6768 743e 3530 3c2f 6865    <height>50</he
+000007a0: 6967 6874 3e0a 2020 2020 2020 2020 2020  ight>.          
+000007b0: 3c2f 7369 7a65 3e0a 2020 2020 2020 2020  </size>.        
+000007c0: 203c 2f70 726f 7065 7274 793e 0a20 2020   </property>.   
+000007d0: 2020 2020 2020 3c70 726f 7065 7274 7920        <property 
+000007e0: 6e61 6d65 3d22 6d61 7869 6d75 6d53 697a  name="maximumSiz
+000007f0: 6522 3e0a 2020 2020 2020 2020 2020 3c73  e">.          <s
+00000800: 697a 653e 0a20 2020 2020 2020 2020 2020  ize>.           
+00000810: 3c77 6964 7468 3e31 3637 3737 3231 353c  <width>16777215<
+00000820: 2f77 6964 7468 3e0a 2020 2020 2020 2020  /width>.        
+00000830: 2020 203c 6865 6967 6874 3e37 303c 2f68     <height>70</h
+00000840: 6569 6768 743e 0a20 2020 2020 2020 2020  eight>.         
+00000850: 203c 2f73 697a 653e 0a20 2020 2020 2020   </size>.       
+00000860: 2020 3c2f 7072 6f70 6572 7479 3e0a 2020    </property>.  
+00000870: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
+00000880: 206e 616d 653d 2274 6578 7422 3e0a 2020   name="text">.  
+00000890: 2020 2020 2020 2020 3c73 7472 696e 673e          <string>
+000008a0: 2053 4e3c 2f73 7472 696e 673e 0a20 2020   SN</string>.   
+000008b0: 2020 2020 2020 3c2f 7072 6f70 6572 7479        </property
+000008c0: 3e0a 2020 2020 2020 2020 3c2f 7769 6467  >.        </widg
+000008d0: 6574 3e0a 2020 2020 2020 203c 2f69 7465  et>.       </ite
+000008e0: 6d3e 0a20 2020 2020 2020 3c69 7465 6d20  m>.       <item 
+000008f0: 726f 773d 2230 2220 636f 6c75 6d6e 3d22  row="0" column="
+00000900: 3022 2063 6f6c 7370 616e 3d22 3322 3e0a  0" colspan="3">.
+00000910: 2020 2020 2020 2020 3c77 6964 6765 7420          <widget 
+00000920: 636c 6173 733d 2251 4c61 6265 6c22 206e  class="QLabel" n
+00000930: 616d 653d 226c 6162 656c 223e 0a20 2020  ame="label">.   
+00000940: 2020 2020 2020 3c70 726f 7065 7274 7920        <property 
+00000950: 6e61 6d65 3d22 6d69 6e69 6d75 6d53 697a  name="minimumSiz
+00000960: 6522 3e0a 2020 2020 2020 2020 2020 3c73  e">.          <s
+00000970: 697a 653e 0a20 2020 2020 2020 2020 2020  ize>.           
+00000980: 3c77 6964 7468 3e30 3c2f 7769 6474 683e  <width>0</width>
+00000990: 0a20 2020 2020 2020 2020 2020 3c68 6569  .           <hei
+000009a0: 6768 743e 3330 3c2f 6865 6967 6874 3e0a  ght>30</height>.
+000009b0: 2020 2020 2020 2020 2020 3c2f 7369 7a65            </size
+000009c0: 3e0a 2020 2020 2020 2020 203c 2f70 726f  >.         </pro
+000009d0: 7065 7274 793e 0a20 2020 2020 2020 2020  perty>.         
+000009e0: 3c70 726f 7065 7274 7920 6e61 6d65 3d22  <property name="
+000009f0: 6d61 7869 6d75 6d53 697a 6522 3e0a 2020  maximumSize">.  
+00000a00: 2020 2020 2020 2020 3c73 697a 653e 0a20          <size>. 
+00000a10: 2020 2020 2020 2020 2020 3c77 6964 7468            <width
+00000a20: 3e31 3637 3737 3231 353c 2f77 6964 7468  >16777215</width
+00000a30: 3e0a 2020 2020 2020 2020 2020 203c 6865  >.           <he
+00000a40: 6967 6874 3e33 303c 2f68 6569 6768 743e  ight>30</height>
+00000a50: 0a20 2020 2020 2020 2020 203c 2f73 697a  .          </siz
+00000a60: 653e 0a20 2020 2020 2020 2020 3c2f 7072  e>.         </pr
+00000a70: 6f70 6572 7479 3e0a 2020 2020 2020 2020  operty>.        
+00000a80: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
+00000a90: 2274 6578 7422 3e0a 2020 2020 2020 2020  "text">.        
+00000aa0: 2020 3c73 7472 696e 672f 3e0a 2020 2020    <string/>.    
+00000ab0: 2020 2020 203c 2f70 726f 7065 7274 793e       </property>
+00000ac0: 0a20 2020 2020 2020 203c 2f77 6964 6765  .        </widge
+00000ad0: 743e 0a20 2020 2020 2020 3c2f 6974 656d  t>.       </item
+00000ae0: 3e0a 2020 2020 2020 203c 6974 656d 2072  >.       <item r
+00000af0: 6f77 3d22 3722 2063 6f6c 756d 6e3d 2230  ow="7" column="0
+00000b00: 2220 636f 6c73 7061 6e3d 2233 223e 0a20  " colspan="3">. 
+00000b10: 2020 2020 2020 203c 7769 6467 6574 2063         <widget c
+00000b20: 6c61 7373 3d22 514c 6162 656c 2220 6e61  lass="QLabel" na
+00000b30: 6d65 3d22 6c61 6265 6c5f 3322 3e0a 2020  me="label_3">.  
+00000b40: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
+00000b50: 206e 616d 653d 226d 6178 696d 756d 5369   name="maximumSi
+00000b60: 7a65 223e 0a20 2020 2020 2020 2020 203c  ze">.          <
+00000b70: 7369 7a65 3e0a 2020 2020 2020 2020 2020  size>.          
+00000b80: 203c 7769 6474 683e 3135 303c 2f77 6964   <width>150</wid
+00000b90: 7468 3e0a 2020 2020 2020 2020 2020 203c  th>.           <
+00000ba0: 6865 6967 6874 3e33 303c 2f68 6569 6768  height>30</heigh
+00000bb0: 743e 0a20 2020 2020 2020 2020 203c 2f73  t>.          </s
+00000bc0: 697a 653e 0a20 2020 2020 2020 2020 3c2f  ize>.         </
+00000bd0: 7072 6f70 6572 7479 3e0a 2020 2020 2020  property>.      
+00000be0: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
+00000bf0: 653d 2274 6578 7422 3e0a 2020 2020 2020  e="text">.      
+00000c00: 2020 2020 3c73 7472 696e 672f 3e0a 2020      <string/>.  
+00000c10: 2020 2020 2020 203c 2f70 726f 7065 7274         </propert
+00000c20: 793e 0a20 2020 2020 2020 203c 2f77 6964  y>.        </wid
+00000c30: 6765 743e 0a20 2020 2020 2020 3c2f 6974  get>.       </it
+00000c40: 656d 3e0a 2020 2020 2020 203c 6974 656d  em>.       <item
+00000c50: 2072 6f77 3d22 3422 2063 6f6c 756d 6e3d   row="4" column=
+00000c60: 2231 2220 616c 6967 6e6d 656e 743d 2251  "1" alignment="Q
+00000c70: 743a 3a41 6c69 676e 5269 6768 7422 3e0a  t::AlignRight">.
+00000c80: 2020 2020 2020 2020 3c77 6964 6765 7420          <widget 
+00000c90: 636c 6173 733d 2251 4c61 6265 6c22 206e  class="QLabel" n
+00000ca0: 616d 653d 226c 6f63 616c 5f63 6f6f 7264  ame="local_coord
+00000cb0: 735f 7822 3e0a 2020 2020 2020 2020 203c  s_x">.         <
+00000cc0: 7072 6f70 6572 7479 206e 616d 653d 226d  property name="m
+00000cd0: 6178 696d 756d 5369 7a65 223e 0a20 2020  aximumSize">.   
+00000ce0: 2020 2020 2020 203c 7369 7a65 3e0a 2020         <size>.  
+00000cf0: 2020 2020 2020 2020 203c 7769 6474 683e           <width>
+00000d00: 3136 3737 3732 3135 3c2f 7769 6474 683e  16777215</width>
+00000d10: 0a20 2020 2020 2020 2020 2020 3c68 6569  .           <hei
+00000d20: 6768 743e 3136 3737 3732 3135 3c2f 6865  ght>16777215</he
+00000d30: 6967 6874 3e0a 2020 2020 2020 2020 2020  ight>.          
+00000d40: 3c2f 7369 7a65 3e0a 2020 2020 2020 2020  </size>.        
+00000d50: 203c 2f70 726f 7065 7274 793e 0a20 2020   </property>.   
+00000d60: 2020 2020 2020 3c70 726f 7065 7274 7920        <property 
+00000d70: 6e61 6d65 3d22 7465 7874 223e 0a20 2020  name="text">.   
+00000d80: 2020 2020 2020 203c 7374 7269 6e67 3e2d         <string>-
+00000d90: 3c2f 7374 7269 6e67 3e0a 2020 2020 2020  </string>.      
+00000da0: 2020 203c 2f70 726f 7065 7274 793e 0a20     </property>. 
+00000db0: 2020 2020 2020 203c 2f77 6964 6765 743e         </widget>
+00000dc0: 0a20 2020 2020 2020 3c2f 6974 656d 3e0a  .       </item>.
+00000dd0: 2020 2020 2020 203c 6974 656d 2072 6f77         <item row
+00000de0: 3d22 3131 2220 636f 6c75 6d6e 3d22 3222  ="11" column="2"
+00000df0: 3e0a 2020 2020 2020 2020 3c77 6964 6765  >.        <widge
+00000e00: 7420 636c 6173 733d 2251 4c61 6265 6c22  t class="QLabel"
+00000e10: 206e 616d 653d 226c 6162 656c 5f31 3822   name="label_18"
+00000e20: 3e0a 2020 2020 2020 2020 203c 7072 6f70  >.         <prop
+00000e30: 6572 7479 206e 616d 653d 2274 6578 7422  erty name="text"
+00000e40: 3e0a 2020 2020 2020 2020 2020 3c73 7472  >.          <str
+00000e50: 696e 673e 20ce bc6d 3c2f 7374 7269 6e67  ing> ..m</string
+00000e60: 3e0a 2020 2020 2020 2020 203c 2f70 726f  >.         </pro
+00000e70: 7065 7274 793e 0a20 2020 2020 2020 203c  perty>.        <
+00000e80: 2f77 6964 6765 743e 0a20 2020 2020 2020  /widget>.       
+00000e90: 3c2f 6974 656d 3e0a 2020 2020 2020 203c  </item>.       <
+00000ea0: 6974 656d 2072 6f77 3d22 3322 2063 6f6c  item row="3" col
+00000eb0: 756d 6e3d 2230 2220 636f 6c73 7061 6e3d  umn="0" colspan=
+00000ec0: 2233 223e 0a20 2020 2020 2020 203c 7769  "3">.        <wi
+00000ed0: 6467 6574 2063 6c61 7373 3d22 514c 6162  dget class="QLab
+00000ee0: 656c 2220 6e61 6d65 3d22 6c6f 6361 6c5f  el" name="local_
+00000ef0: 636f 6f72 6473 223e 0a20 2020 2020 2020  coords">.       
+00000f00: 2020 3c70 726f 7065 7274 7920 6e61 6d65    <property name
+00000f10: 3d22 6d69 6e69 6d75 6d53 697a 6522 3e0a  ="minimumSize">.
+00000f20: 2020 2020 2020 2020 2020 3c73 697a 653e            <size>
+00000f30: 0a20 2020 2020 2020 2020 2020 3c77 6964  .           <wid
+00000f40: 7468 3e30 3c2f 7769 6474 683e 0a20 2020  th>0</width>.   
+00000f50: 2020 2020 2020 2020 3c68 6569 6768 743e          <height>
+00000f60: 3730 3c2f 6865 6967 6874 3e0a 2020 2020  70</height>.    
+00000f70: 2020 2020 2020 3c2f 7369 7a65 3e0a 2020        </size>.  
+00000f80: 2020 2020 2020 203c 2f70 726f 7065 7274         </propert
+00000f90: 793e 0a20 2020 2020 2020 2020 3c70 726f  y>.         <pro
+00000fa0: 7065 7274 7920 6e61 6d65 3d22 6d61 7869  perty name="maxi
+00000fb0: 6d75 6d53 697a 6522 3e0a 2020 2020 2020  mumSize">.      
+00000fc0: 2020 2020 3c73 697a 653e 0a20 2020 2020      <size>.     
+00000fd0: 2020 2020 2020 3c77 6964 7468 3e31 3637        <width>167
+00000fe0: 3737 3231 353c 2f77 6964 7468 3e0a 2020  77215</width>.  
+00000ff0: 2020 2020 2020 2020 203c 6865 6967 6874           <height
+00001000: 3e37 303c 2f68 6569 6768 743e 0a20 2020  >70</height>.   
+00001010: 2020 2020 2020 203c 2f73 697a 653e 0a20         </size>. 
+00001020: 2020 2020 2020 2020 3c2f 7072 6f70 6572          </proper
+00001030: 7479 3e0a 2020 2020 2020 2020 203c 7072  ty>.         <pr
+00001040: 6f70 6572 7479 206e 616d 653d 2274 6578  operty name="tex
+00001050: 7422 3e0a 2020 2020 2020 2020 2020 3c73  t">.          <s
+00001060: 7472 696e 673e 204c 6f63 616c 2063 6f6f  tring> Local coo
+00001070: 7264 733c 2f73 7472 696e 673e 0a20 2020  rds</string>.   
+00001080: 2020 2020 2020 3c2f 7072 6f70 6572 7479        </property
+00001090: 3e0a 2020 2020 2020 2020 3c2f 7769 6467  >.        </widg
+000010a0: 6574 3e0a 2020 2020 2020 203c 2f69 7465  et>.       </ite
+000010b0: 6d3e 0a20 2020 2020 2020 3c69 7465 6d20  m>.       <item 
+000010c0: 726f 773d 2234 2220 636f 6c75 6d6e 3d22  row="4" column="
+000010d0: 3022 3e0a 2020 2020 2020 2020 3c77 6964  0">.        <wid
+000010e0: 6765 7420 636c 6173 733d 2251 4c61 6265  get class="QLabe
+000010f0: 6c22 206e 616d 653d 226c 6162 656c 5f32  l" name="label_2
+00001100: 223e 0a20 2020 2020 2020 2020 3c70 726f  ">.         <pro
+00001110: 7065 7274 7920 6e61 6d65 3d22 6d61 7869  perty name="maxi
+00001120: 6d75 6d53 697a 6522 3e0a 2020 2020 2020  mumSize">.      
+00001130: 2020 2020 3c73 697a 653e 0a20 2020 2020      <size>.     
+00001140: 2020 2020 2020 3c77 6964 7468 3e31 3637        <width>167
+00001150: 3737 3231 353c 2f77 6964 7468 3e0a 2020  77215</width>.  
+00001160: 2020 2020 2020 2020 203c 6865 6967 6874           <height
+00001170: 3e35 303c 2f68 6569 6768 743e 0a20 2020  >50</height>.   
+00001180: 2020 2020 2020 203c 2f73 697a 653e 0a20         </size>. 
+00001190: 2020 2020 2020 2020 3c2f 7072 6f70 6572          </proper
+000011a0: 7479 3e0a 2020 2020 2020 2020 203c 7072  ty>.         <pr
+000011b0: 6f70 6572 7479 206e 616d 653d 2274 6578  operty name="tex
+000011c0: 7422 3e0a 2020 2020 2020 2020 2020 3c73  t">.          <s
+000011d0: 7472 696e 673e 2020 583a 3c2f 7374 7269  tring>  X:</stri
+000011e0: 6e67 3e0a 2020 2020 2020 2020 203c 2f70  ng>.         </p
+000011f0: 726f 7065 7274 793e 0a20 2020 2020 2020  roperty>.       
+00001200: 203c 2f77 6964 6765 743e 0a20 2020 2020   </widget>.     
+00001210: 2020 3c2f 6974 656d 3e0a 2020 2020 2020    </item>.      
+00001220: 203c 6974 656d 2072 6f77 3d22 3922 2063   <item row="9" c
+00001230: 6f6c 756d 6e3d 2232 223e 0a20 2020 2020  olumn="2">.     
+00001240: 2020 203c 7769 6467 6574 2063 6c61 7373     <widget class
+00001250: 3d22 514c 6162 656c 2220 6e61 6d65 3d22  ="QLabel" name="
+00001260: 6c61 6265 6c5f 3136 223e 0a20 2020 2020  label_16">.     
+00001270: 2020 2020 3c70 726f 7065 7274 7920 6e61      <property na
+00001280: 6d65 3d22 7465 7874 223e 0a20 2020 2020  me="text">.     
+00001290: 2020 2020 203c 7374 7269 6e67 3e20 cebc       <string> ..
+000012a0: 6d3c 2f73 7472 696e 673e 0a20 2020 2020  m</string>.     
+000012b0: 2020 2020 3c2f 7072 6f70 6572 7479 3e0a      </property>.
+000012c0: 2020 2020 2020 2020 3c2f 7769 6467 6574          </widget
+000012d0: 3e0a 2020 2020 2020 203c 2f69 7465 6d3e  >.       </item>
+000012e0: 0a20 2020 2020 2020 3c69 7465 6d20 726f  .       <item ro
+000012f0: 773d 2236 2220 636f 6c75 6d6e 3d22 3022  w="6" column="0"
+00001300: 3e0a 2020 2020 2020 2020 3c77 6964 6765  >.        <widge
+00001310: 7420 636c 6173 733d 2251 4c61 6265 6c22  t class="QLabel"
+00001320: 206e 616d 653d 226c 6162 656c 5f31 3122   name="label_11"
+00001330: 3e0a 2020 2020 2020 2020 203c 7072 6f70  >.         <prop
+00001340: 6572 7479 206e 616d 653d 226d 6178 696d  erty name="maxim
+00001350: 756d 5369 7a65 223e 0a20 2020 2020 2020  umSize">.       
+00001360: 2020 203c 7369 7a65 3e0a 2020 2020 2020     <size>.      
+00001370: 2020 2020 203c 7769 6474 683e 3136 3737       <width>1677
+00001380: 3732 3135 3c2f 7769 6474 683e 0a20 2020  7215</width>.   
+00001390: 2020 2020 2020 2020 3c68 6569 6768 743e          <height>
+000013a0: 3530 3c2f 6865 6967 6874 3e0a 2020 2020  50</height>.    
+000013b0: 2020 2020 2020 3c2f 7369 7a65 3e0a 2020        </size>.  
+000013c0: 2020 2020 2020 203c 2f70 726f 7065 7274         </propert
+000013d0: 793e 0a20 2020 2020 2020 2020 3c70 726f  y>.         <pro
+000013e0: 7065 7274 7920 6e61 6d65 3d22 7465 7874  perty name="text
+000013f0: 223e 0a20 2020 2020 2020 2020 203c 7374  ">.          <st
+00001400: 7269 6e67 3e20 205a 3a3c 2f73 7472 696e  ring>  Z:</strin
+00001410: 673e 0a20 2020 2020 2020 2020 3c2f 7072  g>.         </pr
+00001420: 6f70 6572 7479 3e0a 2020 2020 2020 2020  operty>.        
+00001430: 3c2f 7769 6467 6574 3e0a 2020 2020 2020  </widget>.      
+00001440: 203c 2f69 7465 6d3e 0a20 2020 2020 2020   </item>.       
+00001450: 3c69 7465 6d20 726f 773d 2231 3122 2063  <item row="11" c
+00001460: 6f6c 756d 6e3d 2230 223e 0a20 2020 2020  olumn="0">.     
+00001470: 2020 203c 7769 6467 6574 2063 6c61 7373     <widget class
+00001480: 3d22 514c 6162 656c 2220 6e61 6d65 3d22  ="QLabel" name="
+00001490: 6c61 6265 6c5f 3722 3e0a 2020 2020 2020  label_7">.      
+000014a0: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
+000014b0: 653d 226d 6178 696d 756d 5369 7a65 223e  e="maximumSize">
+000014c0: 0a20 2020 2020 2020 2020 203c 7369 7a65  .          <size
+000014d0: 3e0a 2020 2020 2020 2020 2020 203c 7769  >.           <wi
+000014e0: 6474 683e 3136 3737 3732 3135 3c2f 7769  dth>16777215</wi
+000014f0: 6474 683e 0a20 2020 2020 2020 2020 2020  dth>.           
+00001500: 3c68 6569 6768 743e 3530 3c2f 6865 6967  <height>50</heig
+00001510: 6874 3e0a 2020 2020 2020 2020 2020 3c2f  ht>.          </
+00001520: 7369 7a65 3e0a 2020 2020 2020 2020 203c  size>.         <
+00001530: 2f70 726f 7065 7274 793e 0a20 2020 2020  /property>.     
+00001540: 2020 2020 3c70 726f 7065 7274 7920 6e61      <property na
+00001550: 6d65 3d22 7465 7874 223e 0a20 2020 2020  me="text">.     
+00001560: 2020 2020 203c 7374 7269 6e67 3e20 205a       <string>  Z
+00001570: 3a3c 2f73 7472 696e 673e 0a20 2020 2020  :</string>.     
+00001580: 2020 2020 3c2f 7072 6f70 6572 7479 3e0a      </property>.
+00001590: 2020 2020 2020 2020 3c2f 7769 6467 6574          </widget
+000015a0: 3e0a 2020 2020 2020 203c 2f69 7465 6d3e  >.       </item>
+000015b0: 0a20 2020 2020 2020 3c69 7465 6d20 726f  .       <item ro
+000015c0: 773d 2239 2220 636f 6c75 6d6e 3d22 3022  w="9" column="0"
+000015d0: 3e0a 2020 2020 2020 2020 3c77 6964 6765  >.        <widge
+000015e0: 7420 636c 6173 733d 2251 4c61 6265 6c22  t class="QLabel"
+000015f0: 206e 616d 653d 226c 6162 656c 5f35 223e   name="label_5">
+00001600: 0a20 2020 2020 2020 2020 3c70 726f 7065  .         <prope
+00001610: 7274 7920 6e61 6d65 3d22 6d61 7869 6d75  rty name="maximu
+00001620: 6d53 697a 6522 3e0a 2020 2020 2020 2020  mSize">.        
+00001630: 2020 3c73 697a 653e 0a20 2020 2020 2020    <size>.       
+00001640: 2020 2020 3c77 6964 7468 3e31 3637 3737      <width>16777
+00001650: 3231 353c 2f77 6964 7468 3e0a 2020 2020  215</width>.    
+00001660: 2020 2020 2020 203c 6865 6967 6874 3e35         <height>5
+00001670: 303c 2f68 6569 6768 743e 0a20 2020 2020  0</height>.     
+00001680: 2020 2020 203c 2f73 697a 653e 0a20 2020       </size>.   
+00001690: 2020 2020 2020 3c2f 7072 6f70 6572 7479        </property
+000016a0: 3e0a 2020 2020 2020 2020 203c 7072 6f70  >.         <prop
+000016b0: 6572 7479 206e 616d 653d 2274 6578 7422  erty name="text"
+000016c0: 3e0a 2020 2020 2020 2020 2020 3c73 7472  >.          <str
+000016d0: 696e 673e 2020 583a 3c2f 7374 7269 6e67  ing>  X:</string
+000016e0: 3e0a 2020 2020 2020 2020 203c 2f70 726f  >.         </pro
+000016f0: 7065 7274 793e 0a20 2020 2020 2020 203c  perty>.        <
+00001700: 2f77 6964 6765 743e 0a20 2020 2020 2020  /widget>.       
+00001710: 3c2f 6974 656d 3e0a 2020 2020 2020 203c  </item>.       <
+00001720: 6974 656d 2072 6f77 3d22 3130 2220 636f  item row="10" co
+00001730: 6c75 6d6e 3d22 3222 3e0a 2020 2020 2020  lumn="2">.      
+00001740: 2020 3c77 6964 6765 7420 636c 6173 733d    <widget class=
+00001750: 2251 4c61 6265 6c22 206e 616d 653d 226c  "QLabel" name="l
+00001760: 6162 656c 5f31 3722 3e0a 2020 2020 2020  abel_17">.      
+00001770: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
+00001780: 653d 2274 6578 7422 3e0a 2020 2020 2020  e="text">.      
+00001790: 2020 2020 3c73 7472 696e 673e 20ce bc6d      <string> ..m
+000017a0: 3c2f 7374 7269 6e67 3e0a 2020 2020 2020  </string>.      
+000017b0: 2020 203c 2f70 726f 7065 7274 793e 0a20     </property>. 
+000017c0: 2020 2020 2020 203c 2f77 6964 6765 743e         </widget>
+000017d0: 0a20 2020 2020 2020 3c2f 6974 656d 3e0a  .       </item>.
+000017e0: 2020 2020 2020 203c 6974 656d 2072 6f77         <item row
+000017f0: 3d22 3422 2063 6f6c 756d 6e3d 2232 223e  ="4" column="2">
+00001800: 0a20 2020 2020 2020 203c 7769 6467 6574  .        <widget
+00001810: 2063 6c61 7373 3d22 514c 6162 656c 2220   class="QLabel" 
+00001820: 6e61 6d65 3d22 6c61 6265 6c5f 3133 223e  name="label_13">
+00001830: 0a20 2020 2020 2020 2020 3c70 726f 7065  .         <prope
+00001840: 7274 7920 6e61 6d65 3d22 6d69 6e69 6d75  rty name="minimu
+00001850: 6d53 697a 6522 3e0a 2020 2020 2020 2020  mSize">.        
+00001860: 2020 3c73 697a 653e 0a20 2020 2020 2020    <size>.       
+00001870: 2020 2020 3c77 6964 7468 3e35 303c 2f77      <width>50</w
+00001880: 6964 7468 3e0a 2020 2020 2020 2020 2020  idth>.          
+00001890: 203c 6865 6967 6874 3e30 3c2f 6865 6967   <height>0</heig
+000018a0: 6874 3e0a 2020 2020 2020 2020 2020 3c2f  ht>.          </
+000018b0: 7369 7a65 3e0a 2020 2020 2020 2020 203c  size>.         <
+000018c0: 2f70 726f 7065 7274 793e 0a20 2020 2020  /property>.     
+000018d0: 2020 2020 3c70 726f 7065 7274 7920 6e61      <property na
+000018e0: 6d65 3d22 6d61 7869 6d75 6d53 697a 6522  me="maximumSize"
+000018f0: 3e0a 2020 2020 2020 2020 2020 3c73 697a  >.          <siz
+00001900: 653e 0a20 2020 2020 2020 2020 2020 3c77  e>.           <w
+00001910: 6964 7468 3e35 303c 2f77 6964 7468 3e0a  idth>50</width>.
+00001920: 2020 2020 2020 2020 2020 203c 6865 6967             <heig
+00001930: 6874 3e31 3637 3737 3231 353c 2f68 6569  ht>16777215</hei
+00001940: 6768 743e 0a20 2020 2020 2020 2020 203c  ght>.          <
+00001950: 2f73 697a 653e 0a20 2020 2020 2020 2020  /size>.         
+00001960: 3c2f 7072 6f70 6572 7479 3e0a 2020 2020  </property>.    
+00001970: 2020 2020 203c 7072 6f70 6572 7479 206e       <property n
+00001980: 616d 653d 2274 6578 7422 3e0a 2020 2020  ame="text">.    
+00001990: 2020 2020 2020 3c73 7472 696e 673e 20ce        <string> .
+000019a0: bc6d 3c2f 7374 7269 6e67 3e0a 2020 2020  .m</string>.    
+000019b0: 2020 2020 203c 2f70 726f 7065 7274 793e       </property>
+000019c0: 0a20 2020 2020 2020 203c 2f77 6964 6765  .        </widge
+000019d0: 743e 0a20 2020 2020 2020 3c2f 6974 656d  t>.       </item
+000019e0: 3e0a 2020 2020 2020 203c 6974 656d 2072  >.       <item r
+000019f0: 6f77 3d22 3622 2063 6f6c 756d 6e3d 2231  ow="6" column="1
+00001a00: 2220 616c 6967 6e6d 656e 743d 2251 743a  " alignment="Qt:
+00001a10: 3a41 6c69 676e 5269 6768 7422 3e0a 2020  :AlignRight">.  
+00001a20: 2020 2020 2020 3c77 6964 6765 7420 636c        <widget cl
+00001a30: 6173 733d 2251 4c61 6265 6c22 206e 616d  ass="QLabel" nam
+00001a40: 653d 226c 6f63 616c 5f63 6f6f 7264 735f  e="local_coords_
+00001a50: 7a22 3e0a 2020 2020 2020 2020 203c 7072  z">.         <pr
+00001a60: 6f70 6572 7479 206e 616d 653d 2274 6578  operty name="tex
+00001a70: 7422 3e0a 2020 2020 2020 2020 2020 3c73  t">.          <s
+00001a80: 7472 696e 673e 2d3c 2f73 7472 696e 673e  tring>-</string>
+00001a90: 0a20 2020 2020 2020 2020 3c2f 7072 6f70  .         </prop
+00001aa0: 6572 7479 3e0a 2020 2020 2020 2020 3c2f  erty>.        </
+00001ab0: 7769 6467 6574 3e0a 2020 2020 2020 203c  widget>.       <
+00001ac0: 2f69 7465 6d3e 0a20 2020 2020 2020 3c69  /item>.       <i
+00001ad0: 7465 6d20 726f 773d 2231 3022 2063 6f6c  tem row="10" col
+00001ae0: 756d 6e3d 2231 2220 616c 6967 6e6d 656e  umn="1" alignmen
+00001af0: 743d 2251 743a 3a41 6c69 676e 5269 6768  t="Qt::AlignRigh
+00001b00: 7422 3e0a 2020 2020 2020 2020 3c77 6964  t">.        <wid
+00001b10: 6765 7420 636c 6173 733d 2251 4c61 6265  get class="QLabe
+00001b20: 6c22 206e 616d 653d 2267 6c6f 6261 6c5f  l" name="global_
+00001b30: 636f 6f72 6473 5f79 223e 0a20 2020 2020  coords_y">.     
+00001b40: 2020 2020 3c70 726f 7065 7274 7920 6e61      <property na
+00001b50: 6d65 3d22 7465 7874 223e 0a20 2020 2020  me="text">.     
+00001b60: 2020 2020 203c 7374 7269 6e67 3e2d 3c2f       <string>-</
+00001b70: 7374 7269 6e67 3e0a 2020 2020 2020 2020  string>.        
+00001b80: 203c 2f70 726f 7065 7274 793e 0a20 2020   </property>.   
+00001b90: 2020 2020 203c 2f77 6964 6765 743e 0a20       </widget>. 
+00001ba0: 2020 2020 2020 3c2f 6974 656d 3e0a 2020        </item>.  
+00001bb0: 2020 2020 203c 6974 656d 2072 6f77 3d22       <item row="
+00001bc0: 3522 2063 6f6c 756d 6e3d 2231 2220 616c  5" column="1" al
+00001bd0: 6967 6e6d 656e 743d 2251 743a 3a41 6c69  ignment="Qt::Ali
+00001be0: 676e 5269 6768 7422 3e0a 2020 2020 2020  gnRight">.      
+00001bf0: 2020 3c77 6964 6765 7420 636c 6173 733d    <widget class=
+00001c00: 2251 4c61 6265 6c22 206e 616d 653d 226c  "QLabel" name="l
+00001c10: 6f63 616c 5f63 6f6f 7264 735f 7922 3e0a  ocal_coords_y">.
+00001c20: 2020 2020 2020 2020 203c 7072 6f70 6572           <proper
+00001c30: 7479 206e 616d 653d 2274 6578 7422 3e0a  ty name="text">.
+00001c40: 2020 2020 2020 2020 2020 3c73 7472 696e            <strin
+00001c50: 673e 2d3c 2f73 7472 696e 673e 0a20 2020  g>-</string>.   
+00001c60: 2020 2020 2020 3c2f 7072 6f70 6572 7479        </property
+00001c70: 3e0a 2020 2020 2020 2020 3c2f 7769 6467  >.        </widg
+00001c80: 6574 3e0a 2020 2020 2020 203c 2f69 7465  et>.       </ite
+00001c90: 6d3e 0a20 2020 2020 2020 3c69 7465 6d20  m>.       <item 
+00001ca0: 726f 773d 2239 2220 636f 6c75 6d6e 3d22  row="9" column="
+00001cb0: 3122 2061 6c69 676e 6d65 6e74 3d22 5174  1" alignment="Qt
+00001cc0: 3a3a 416c 6967 6e52 6967 6874 223e 0a20  ::AlignRight">. 
+00001cd0: 2020 2020 2020 203c 7769 6467 6574 2063         <widget c
+00001ce0: 6c61 7373 3d22 514c 6162 656c 2220 6e61  lass="QLabel" na
+00001cf0: 6d65 3d22 676c 6f62 616c 5f63 6f6f 7264  me="global_coord
+00001d00: 735f 7822 3e0a 2020 2020 2020 2020 203c  s_x">.         <
+00001d10: 7072 6f70 6572 7479 206e 616d 653d 2274  property name="t
+00001d20: 6578 7422 3e0a 2020 2020 2020 2020 2020  ext">.          
+00001d30: 3c73 7472 696e 673e 2d3c 2f73 7472 696e  <string>-</strin
+00001d40: 673e 0a20 2020 2020 2020 2020 3c2f 7072  g>.         </pr
+00001d50: 6f70 6572 7479 3e0a 2020 2020 2020 2020  operty>.        
+00001d60: 3c2f 7769 6467 6574 3e0a 2020 2020 2020  </widget>.      
+00001d70: 203c 2f69 7465 6d3e 0a20 2020 2020 2020   </item>.       
+00001d80: 3c69 7465 6d20 726f 773d 2238 2220 636f  <item row="8" co
+00001d90: 6c75 6d6e 3d22 3022 2063 6f6c 7370 616e  lumn="0" colspan
+00001da0: 3d22 3322 3e0a 2020 2020 2020 2020 3c77  ="3">.        <w
+00001db0: 6964 6765 7420 636c 6173 733d 2251 4c61  idget class="QLa
+00001dc0: 6265 6c22 206e 616d 653d 2267 6c6f 6261  bel" name="globa
+00001dd0: 6c5f 636f 6f72 6473 223e 0a20 2020 2020  l_coords">.     
+00001de0: 2020 2020 3c70 726f 7065 7274 7920 6e61      <property na
+00001df0: 6d65 3d22 6d69 6e69 6d75 6d53 697a 6522  me="minimumSize"
+00001e00: 3e0a 2020 2020 2020 2020 2020 3c73 697a  >.          <siz
+00001e10: 653e 0a20 2020 2020 2020 2020 2020 3c77  e>.           <w
+00001e20: 6964 7468 3e30 3c2f 7769 6474 683e 0a20  idth>0</width>. 
+00001e30: 2020 2020 2020 2020 2020 3c68 6569 6768            <heigh
+00001e40: 743e 3730 3c2f 6865 6967 6874 3e0a 2020  t>70</height>.  
+00001e50: 2020 2020 2020 2020 3c2f 7369 7a65 3e0a          </size>.
+00001e60: 2020 2020 2020 2020 203c 2f70 726f 7065           </prope
+00001e70: 7274 793e 0a20 2020 2020 2020 2020 3c70  rty>.         <p
+00001e80: 726f 7065 7274 7920 6e61 6d65 3d22 6d61  roperty name="ma
+00001e90: 7869 6d75 6d53 697a 6522 3e0a 2020 2020  ximumSize">.    
+00001ea0: 2020 2020 2020 3c73 697a 653e 0a20 2020        <size>.   
+00001eb0: 2020 2020 2020 2020 3c77 6964 7468 3e31          <width>1
+00001ec0: 3637 3737 3231 353c 2f77 6964 7468 3e0a  6777215</width>.
+00001ed0: 2020 2020 2020 2020 2020 203c 6865 6967             <heig
+00001ee0: 6874 3e37 303c 2f68 6569 6768 743e 0a20  ht>70</height>. 
+00001ef0: 2020 2020 2020 2020 203c 2f73 697a 653e           </size>
+00001f00: 0a20 2020 2020 2020 2020 3c2f 7072 6f70  .         </prop
+00001f10: 6572 7479 3e0a 2020 2020 2020 2020 203c  erty>.         <
+00001f20: 7072 6f70 6572 7479 206e 616d 653d 2274  property name="t
+00001f30: 6578 7422 3e0a 2020 2020 2020 2020 2020  ext">.          
+00001f40: 3c73 7472 696e 673e 2047 6c6f 6261 6c20  <string> Global 
+00001f50: 636f 6f72 6473 3c2f 7374 7269 6e67 3e0a  coords</string>.
+00001f60: 2020 2020 2020 2020 203c 2f70 726f 7065           </prope
+00001f70: 7274 793e 0a20 2020 2020 2020 203c 2f77  rty>.        </w
+00001f80: 6964 6765 743e 0a20 2020 2020 2020 3c2f  idget>.       </
+00001f90: 6974 656d 3e0a 2020 2020 2020 203c 6974  item>.       <it
+00001fa0: 656d 2072 6f77 3d22 3522 2063 6f6c 756d  em row="5" colum
+00001fb0: 6e3d 2230 223e 0a20 2020 2020 2020 203c  n="0">.        <
+00001fc0: 7769 6467 6574 2063 6c61 7373 3d22 514c  widget class="QL
+00001fd0: 6162 656c 2220 6e61 6d65 3d22 6c61 6265  abel" name="labe
+00001fe0: 6c5f 3130 223e 0a20 2020 2020 2020 2020  l_10">.         
+00001ff0: 3c70 726f 7065 7274 7920 6e61 6d65 3d22  <property name="
+00002000: 6d61 7869 6d75 6d53 697a 6522 3e0a 2020  maximumSize">.  
+00002010: 2020 2020 2020 2020 3c73 697a 653e 0a20          <size>. 
+00002020: 2020 2020 2020 2020 2020 3c77 6964 7468            <width
+00002030: 3e31 3637 3737 3231 353c 2f77 6964 7468  >16777215</width
+00002040: 3e0a 2020 2020 2020 2020 2020 203c 6865  >.           <he
+00002050: 6967 6874 3e35 303c 2f68 6569 6768 743e  ight>50</height>
+00002060: 0a20 2020 2020 2020 2020 203c 2f73 697a  .          </siz
+00002070: 653e 0a20 2020 2020 2020 2020 3c2f 7072  e>.         </pr
+00002080: 6f70 6572 7479 3e0a 2020 2020 2020 2020  operty>.        
+00002090: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
+000020a0: 2274 6578 7422 3e0a 2020 2020 2020 2020  "text">.        
+000020b0: 2020 3c73 7472 696e 673e 2020 593a 3c2f    <string>  Y:</
+000020c0: 7374 7269 6e67 3e0a 2020 2020 2020 2020  string>.        
+000020d0: 203c 2f70 726f 7065 7274 793e 0a20 2020   </property>.   
+000020e0: 2020 2020 203c 2f77 6964 6765 743e 0a20       </widget>. 
+000020f0: 2020 2020 2020 3c2f 6974 656d 3e0a 2020        </item>.  
+00002100: 2020 2020 203c 6974 656d 2072 6f77 3d22       <item row="
+00002110: 3131 2220 636f 6c75 6d6e 3d22 3122 2061  11" column="1" a
+00002120: 6c69 676e 6d65 6e74 3d22 5174 3a3a 416c  lignment="Qt::Al
+00002130: 6967 6e52 6967 6874 223e 0a20 2020 2020  ignRight">.     
+00002140: 2020 203c 7769 6467 6574 2063 6c61 7373     <widget class
+00002150: 3d22 514c 6162 656c 2220 6e61 6d65 3d22  ="QLabel" name="
+00002160: 676c 6f62 616c 5f63 6f6f 7264 735f 7a22  global_coords_z"
+00002170: 3e0a 2020 2020 2020 2020 203c 7072 6f70  >.         <prop
+00002180: 6572 7479 206e 616d 653d 2274 6578 7422  erty name="text"
+00002190: 3e0a 2020 2020 2020 2020 2020 3c73 7472  >.          <str
+000021a0: 696e 673e 2d3c 2f73 7472 696e 673e 0a20  ing>-</string>. 
+000021b0: 2020 2020 2020 2020 3c2f 7072 6f70 6572          </proper
+000021c0: 7479 3e0a 2020 2020 2020 2020 3c2f 7769  ty>.        </wi
+000021d0: 6467 6574 3e0a 2020 2020 2020 203c 2f69  dget>.       </i
+000021e0: 7465 6d3e 0a20 2020 2020 2020 3c69 7465  tem>.       <ite
+000021f0: 6d20 726f 773d 2231 2220 636f 6c75 6d6e  m row="1" column
+00002200: 3d22 3022 2063 6f6c 7370 616e 3d22 3322  ="0" colspan="3"
+00002210: 3e0a 2020 2020 2020 2020 3c77 6964 6765  >.        <widge
+00002220: 7420 636c 6173 733d 2251 436f 6d62 6f42  t class="QComboB
+00002230: 6f78 2220 6e61 6d65 3d22 7374 6167 655f  ox" name="stage_
+00002240: 7365 6c65 6374 6f72 223e 0a20 2020 2020  selector">.     
+00002250: 2020 2020 3c70 726f 7065 7274 7920 6e61      <property na
+00002260: 6d65 3d22 6d61 7869 6d75 6d53 697a 6522  me="maximumSize"
+00002270: 3e0a 2020 2020 2020 2020 2020 3c73 697a  >.          <siz
+00002280: 653e 0a20 2020 2020 2020 2020 2020 3c77  e>.           <w
+00002290: 6964 7468 3e31 3637 3737 3231 353c 2f77  idth>16777215</w
+000022a0: 6964 7468 3e0a 2020 2020 2020 2020 2020  idth>.          
+000022b0: 203c 6865 6967 6874 3e37 303c 2f68 6569   <height>70</hei
+000022c0: 6768 743e 0a20 2020 2020 2020 2020 203c  ght>.          <
+000022d0: 2f73 697a 653e 0a20 2020 2020 2020 2020  /size>.         
+000022e0: 3c2f 7072 6f70 6572 7479 3e0a 2020 2020  </property>.    
+000022f0: 2020 2020 3c2f 7769 6467 6574 3e0a 2020      </widget>.  
+00002300: 2020 2020 203c 2f69 7465 6d3e 0a20 2020       </item>.   
+00002310: 2020 2020 3c69 7465 6d20 726f 773d 2231      <item row="1
+00002320: 3022 2063 6f6c 756d 6e3d 2230 223e 0a20  0" column="0">. 
+00002330: 2020 2020 2020 203c 7769 6467 6574 2063         <widget c
+00002340: 6c61 7373 3d22 514c 6162 656c 2220 6e61  lass="QLabel" na
+00002350: 6d65 3d22 6c61 6265 6c5f 3622 3e0a 2020  me="label_6">.  
+00002360: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
+00002370: 206e 616d 653d 226d 6178 696d 756d 5369   name="maximumSi
+00002380: 7a65 223e 0a20 2020 2020 2020 2020 203c  ze">.          <
+00002390: 7369 7a65 3e0a 2020 2020 2020 2020 2020  size>.          
+000023a0: 203c 7769 6474 683e 3136 3737 3732 3135   <width>16777215
+000023b0: 3c2f 7769 6474 683e 0a20 2020 2020 2020  </width>.       
+000023c0: 2020 2020 3c68 6569 6768 743e 3530 3c2f      <height>50</
+000023d0: 6865 6967 6874 3e0a 2020 2020 2020 2020  height>.        
+000023e0: 2020 3c2f 7369 7a65 3e0a 2020 2020 2020    </size>.      
+000023f0: 2020 203c 2f70 726f 7065 7274 793e 0a20     </property>. 
+00002400: 2020 2020 2020 2020 3c70 726f 7065 7274          <propert
+00002410: 7920 6e61 6d65 3d22 7465 7874 223e 0a20  y name="text">. 
+00002420: 2020 2020 2020 2020 203c 7374 7269 6e67           <string
+00002430: 3e20 2059 3a3c 2f73 7472 696e 673e 0a20  >  Y:</string>. 
+00002440: 2020 2020 2020 2020 3c2f 7072 6f70 6572          </proper
+00002450: 7479 3e0a 2020 2020 2020 2020 3c2f 7769  ty>.        </wi
+00002460: 6467 6574 3e0a 2020 2020 2020 203c 2f69  dget>.       </i
+00002470: 7465 6d3e 0a20 2020 2020 2020 3c69 7465  tem>.       <ite
+00002480: 6d20 726f 773d 2235 2220 636f 6c75 6d6e  m row="5" column
+00002490: 3d22 3222 3e0a 2020 2020 2020 2020 3c77  ="2">.        <w
+000024a0: 6964 6765 7420 636c 6173 733d 2251 4c61  idget class="QLa
+000024b0: 6265 6c22 206e 616d 653d 226c 6162 656c  bel" name="label
+000024c0: 5f31 3422 3e0a 2020 2020 2020 2020 203c  _14">.         <
+000024d0: 7072 6f70 6572 7479 206e 616d 653d 2274  property name="t
+000024e0: 6578 7422 3e0a 2020 2020 2020 2020 2020  ext">.          
+000024f0: 3c73 7472 696e 673e 20ce bc6d 3c2f 7374  <string> ..m</st
+00002500: 7269 6e67 3e0a 2020 2020 2020 2020 203c  ring>.         <
+00002510: 2f70 726f 7065 7274 793e 0a20 2020 2020  /property>.     
+00002520: 2020 203c 2f77 6964 6765 743e 0a20 2020     </widget>.   
+00002530: 2020 2020 3c2f 6974 656d 3e0a 2020 2020      </item>.    
+00002540: 2020 203c 6974 656d 2072 6f77 3d22 3132     <item row="12
+00002550: 2220 636f 6c75 6d6e 3d22 3022 2063 6f6c  " column="0" col
+00002560: 7370 616e 3d22 3322 3e0a 2020 2020 2020  span="3">.      
+00002570: 2020 3c77 6964 6765 7420 636c 6173 733d    <widget class=
+00002580: 2251 4c61 6265 6c22 206e 616d 653d 226c  "QLabel" name="l
+00002590: 6162 656c 5f34 223e 0a20 2020 2020 2020  abel_4">.       
+000025a0: 2020 3c70 726f 7065 7274 7920 6e61 6d65    <property name
+000025b0: 3d22 6d61 7869 6d75 6d53 697a 6522 3e0a  ="maximumSize">.
+000025c0: 2020 2020 2020 2020 2020 3c73 697a 653e            <size>
+000025d0: 0a20 2020 2020 2020 2020 2020 3c77 6964  .           <wid
+000025e0: 7468 3e31 3637 3737 3231 353c 2f77 6964  th>16777215</wid
+000025f0: 7468 3e0a 2020 2020 2020 2020 2020 203c  th>.           <
+00002600: 6865 6967 6874 3e31 303c 2f68 6569 6768  height>10</heigh
+00002610: 743e 0a20 2020 2020 2020 2020 203c 2f73  t>.          </s
+00002620: 697a 653e 0a20 2020 2020 2020 2020 3c2f  ize>.         </
+00002630: 7072 6f70 6572 7479 3e0a 2020 2020 2020  property>.      
+00002640: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
+00002650: 653d 2274 6578 7422 3e0a 2020 2020 2020  e="text">.      
+00002660: 2020 2020 3c73 7472 696e 672f 3e0a 2020      <string/>.  
+00002670: 2020 2020 2020 203c 2f70 726f 7065 7274         </propert
+00002680: 793e 0a20 2020 2020 2020 203c 2f77 6964  y>.        </wid
+00002690: 6765 743e 0a20 2020 2020 2020 3c2f 6974  get>.       </it
+000026a0: 656d 3e0a 2020 2020 2020 203c 6974 656d  em>.       <item
+000026b0: 2072 6f77 3d22 3622 2063 6f6c 756d 6e3d   row="6" column=
+000026c0: 2232 223e 0a20 2020 2020 2020 203c 7769  "2">.        <wi
+000026d0: 6467 6574 2063 6c61 7373 3d22 514c 6162  dget class="QLab
+000026e0: 656c 2220 6e61 6d65 3d22 6c61 6265 6c5f  el" name="label_
+000026f0: 3135 223e 0a20 2020 2020 2020 2020 3c70  15">.         <p
+00002700: 726f 7065 7274 7920 6e61 6d65 3d22 6d61  roperty name="ma
+00002710: 7869 6d75 6d53 697a 6522 3e0a 2020 2020  ximumSize">.    
+00002720: 2020 2020 2020 3c73 697a 653e 0a20 2020        <size>.   
+00002730: 2020 2020 2020 2020 3c77 6964 7468 3e34          <width>4
+00002740: 303c 2f77 6964 7468 3e0a 2020 2020 2020  0</width>.      
+00002750: 2020 2020 203c 6865 6967 6874 3e31 3637       <height>167
+00002760: 3737 3231 353c 2f68 6569 6768 743e 0a20  77215</height>. 
+00002770: 2020 2020 2020 2020 203c 2f73 697a 653e           </size>
+00002780: 0a20 2020 2020 2020 2020 3c2f 7072 6f70  .         </prop
+00002790: 6572 7479 3e0a 2020 2020 2020 2020 203c  erty>.         <
+000027a0: 7072 6f70 6572 7479 206e 616d 653d 2274  property name="t
+000027b0: 6578 7422 3e0a 2020 2020 2020 2020 2020  ext">.          
+000027c0: 3c73 7472 696e 673e 20ce bc6d 3c2f 7374  <string> ..m</st
+000027d0: 7269 6e67 3e0a 2020 2020 2020 2020 203c  ring>.         <
+000027e0: 2f70 726f 7065 7274 793e 0a20 2020 2020  /property>.     
+000027f0: 2020 203c 2f77 6964 6765 743e 0a20 2020     </widget>.   
+00002800: 2020 2020 3c2f 6974 656d 3e0a 2020 2020      </item>.    
+00002810: 2020 3c2f 6c61 796f 7574 3e0a 2020 2020    </layout>.    
+00002820: 203c 2f69 7465 6d3e 0a20 2020 203c 2f6c   </item>.    </l
+00002830: 6179 6f75 743e 0a20 2020 3c2f 6974 656d  ayout>.   </item
+00002840: 3e0a 2020 3c2f 6c61 796f 7574 3e0a 203c  >.  </layout>. <
+00002850: 2f77 6964 6765 743e 0a20 3c72 6573 6f75  /widget>. <resou
+00002860: 7263 6573 2f3e 0a20 3c63 6f6e 6e65 6374  rces/>. <connect
+00002870: 696f 6e73 2f3e 0a3c 2f75 693e 0a         ions/>.</ui>.
```

