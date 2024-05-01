# Comparing `tmp/nqrduck-0.0.7.tar.gz` & `tmp/nqrduck-0.0.8.tar.gz`

## Comparing `nqrduck-0.0.7.tar` & `nqrduck-0.0.8.tar`

### file list

```diff
@@ -1,63 +1,64 @@
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 nqrduck-0.0.7/CHANGELOG.md
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 nqrduck-0.0.7/.github/workflows/main.yml
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 nqrduck-0.0.7/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 nqrduck-0.0.7/.github/workflows/ubuntu-python-package.yml
--rw-r--r--   0        0        0  1509874 2020-02-02 00:00:00.000000 nqrduck-0.0.7/docs/img/ui_structure_v2.png
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/__init__.py
--rw-r--r--   0        0        0     3165 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/__main__.py
--rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/assets/animations.py
--rw-r--r--   0        0        0     7236 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/assets/icons.py
--rw-r--r--   0        0        0    27758 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/assets/animations/DuckKick_128x128.gif
--rw-r--r--   0        0        0   115443 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/assets/animations/DuckSleep_128x128.gif
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/assets/logos/ArrowLeft_12x12.png
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/assets/logos/ArrowRight_12x12.png
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/assets/logos/Attention_16x16.png
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/assets/logos/Error_16x16.png
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/assets/logos/Garbage_12x12.png
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/assets/logos/Info_16x16.png
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/assets/logos/LabMallardnbg_32x32.png
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/assets/logos/Load_16x16.png
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/assets/logos/Logo_64x32.png
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/assets/logos/Logo_full.png
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/assets/logos/New_16x16.png
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/assets/logos/Pen_12x12.png
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/assets/logos/Play_16x16.png
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/assets/logos/QuestionMark_16x16.png
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/assets/logos/Save_16x16.png
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/assets/logos/Settings_16x16.png
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/assets/pulseparameters/GateOff.png
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/assets/pulseparameters/GateOn.png
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/assets/pulseparameters/RXOff.png
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/assets/pulseparameters/RXOn.png
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/assets/pulseparameters/TXCustom.png
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/assets/pulseparameters/TXGauss.png
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/assets/pulseparameters/TXOff.png
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/assets/pulseparameters/TXRect.png
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/assets/pulseparameters/TXSinc.png
--rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/contrib/mplwidget.py
--rw-r--r--   0        0        0     4131 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/core/main_controller.py
--rw-r--r--   0        0        0     6948 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/core/main_model.py
--rw-r--r--   0        0        0    31369 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/core/main_view.py
--rw-r--r--   0        0        0     4402 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/core/main_window.py
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/core/resources/logo.png
--rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/core/resources/main_window.ui
--rw-r--r--   0        0        0    28916 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/core/resources/font/AsepriteFont.ttf
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/core/resources/font/LICENCE
--rw-r--r--   0        0        0     7172 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/helpers/duckwidgets.py
--rw-r--r--   0        0        0    18881 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/helpers/formbuilder.py
--rw-r--r--   0        0        0    12683 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/helpers/functions.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/helpers/serializer.py
--rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/helpers/signalprocessing.py
--rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/helpers/unitconverter.py
--rw-r--r--   0        0        0     3669 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/helpers/validators.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/module/__init__.py
--rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/module/module.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/module/module_controller.py
--rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/module/module_model.py
--rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/module/module_view.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 nqrduck-0.0.7/tests/test_load_module.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 nqrduck-0.0.7/.gitignore
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 nqrduck-0.0.7/LICENSE
--rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 nqrduck-0.0.7/README.md
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 nqrduck-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     5451 2020-02-02 00:00:00.000000 nqrduck-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 nqrduck-0.0.8/CHANGELOG.md
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 nqrduck-0.0.8/.github/workflows/main.yml
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 nqrduck-0.0.8/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 nqrduck-0.0.8/.github/workflows/ubuntu-python-package.yml
+-rw-r--r--   0        0        0  1509874 2020-02-02 00:00:00.000000 nqrduck-0.0.8/docs/img/ui_structure_v2.png
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/__init__.py
+-rw-r--r--   0        0        0     3649 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/__main__.py
+-rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/assets/animations.py
+-rw-r--r--   0        0        0     7236 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/assets/icons.py
+-rw-r--r--   0        0        0    27758 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/assets/animations/DuckKick_128x128.gif
+-rw-r--r--   0        0        0   115443 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/assets/animations/DuckSleep_128x128.gif
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/assets/logos/ArrowLeft_12x12.png
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/assets/logos/ArrowRight_12x12.png
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/assets/logos/Attention_16x16.png
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/assets/logos/Error_16x16.png
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/assets/logos/Garbage_12x12.png
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/assets/logos/Info_16x16.png
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/assets/logos/LabMallardnbg_32x32.png
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/assets/logos/Load_16x16.png
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/assets/logos/Logo_64x32.png
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/assets/logos/Logo_full.png
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/assets/logos/New_16x16.png
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/assets/logos/Pen_12x12.png
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/assets/logos/Play_16x16.png
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/assets/logos/QuestionMark_16x16.png
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/assets/logos/Save_16x16.png
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/assets/logos/Settings_16x16.png
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/assets/pulseparameters/GateOff.png
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/assets/pulseparameters/GateOn.png
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/assets/pulseparameters/RXOff.png
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/assets/pulseparameters/RXOn.png
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/assets/pulseparameters/TXCustom.png
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/assets/pulseparameters/TXGauss.png
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/assets/pulseparameters/TXOff.png
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/assets/pulseparameters/TXRect.png
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/assets/pulseparameters/TXSinc.png
+-rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/contrib/mplwidget.py
+-rw-r--r--   0        0        0    15929 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/core/install_wizard.py
+-rw-r--r--   0        0        0     4587 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/core/main_controller.py
+-rw-r--r--   0        0        0     6948 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/core/main_model.py
+-rw-r--r--   0        0        0    31514 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/core/main_view.py
+-rw-r--r--   0        0        0     4706 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/core/main_window.py
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/core/resources/logo.png
+-rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/core/resources/main_window.ui
+-rw-r--r--   0        0        0    28916 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/core/resources/font/AsepriteFont.ttf
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/core/resources/font/LICENCE
+-rw-r--r--   0        0        0     7172 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/helpers/duckwidgets.py
+-rw-r--r--   0        0        0    18853 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/helpers/formbuilder.py
+-rw-r--r--   0        0        0    12683 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/helpers/functions.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/helpers/serializer.py
+-rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/helpers/signalprocessing.py
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/helpers/unitconverter.py
+-rw-r--r--   0        0        0     3669 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/helpers/validators.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/module/__init__.py
+-rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/module/module.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/module/module_controller.py
+-rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/module/module_model.py
+-rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 nqrduck-0.0.8/src/nqrduck/module/module_view.py
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 nqrduck-0.0.8/tests/test_load_module.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 nqrduck-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 nqrduck-0.0.8/LICENSE
+-rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 nqrduck-0.0.8/README.md
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 nqrduck-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     5456 2020-02-02 00:00:00.000000 nqrduck-0.0.8/PKG-INFO
```

### Comparing `nqrduck-0.0.7/CHANGELOG.md` & `nqrduck-0.0.8/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # Changelog
 
+### Version 0.0.8 (01-05-2024)
+- Added install wizard for the different NQRduck modules
+
 ### Version 0.0.7 (26-04-2024)
 - Implemented Formbuilder for the GUI which can be used to create easy input fields for the user
 
 ### Version 0.0.6 (23-04-2024)
 - Fixed bug with platform dependency in the pyproject.toml file
 
 ### Version 0.0.5 (23-04-2024)
```

### Comparing `nqrduck-0.0.7/.github/workflows/main.yml` & `nqrduck-0.0.8/.github/workflows/main.yml`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
       options: --privileged
 
     steps:
     - uses: actions/checkout@v3
 
     - name: Install system and Python dependencies
       run: |
-        yes | pacman -Sy --needed python python-pip git python-pyqt5 xorg-server-xvfb libgl mesa libxkbcommon fontconfig xcb-util-cursor libegl
+        yes | pacman -Sy --needed python python-pip git python-pyqt5 xorg-server-xvfb libgl mesa libxkbcommon fontconfig xcb-util-cursor libegl expat
         pip install pytest --break-system-packages
 
     - name: Install test module and dependencies
       run: |
         pip install nqrduck-module --break-system-packages
 
     - name: Run all the tests
```

### Comparing `nqrduck-0.0.7/.github/workflows/python-publish.yml` & `nqrduck-0.0.8/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.7/.github/workflows/ubuntu-python-package.yml` & `nqrduck-0.0.8/.github/workflows/ubuntu-python-package.yml`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.7/docs/img/ui_structure_v2.png` & `nqrduck-0.0.8/docs/img/ui_structure_v2.png`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.7/src/nqrduck/__main__.py` & `nqrduck-0.0.8/src/nqrduck/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,99 +1,125 @@
 """Main entry point for the NQRduck application."""
+
 import sys
 import traceback
 import os
 import logging
 import logging.handlers
-import  tempfile
+import tempfile
 from PyQt6.QtWidgets import QApplication, QMessageBox
 from .core.main_model import MainModel
 from .core.main_controller import MainController
 from .core.main_view import MainView
+from .core.install_wizard import DuckWizard
 
 logger = logging.getLogger(__name__)
 
+
 class NQRduck(QApplication):
     """Main application for the NQRduck.
-    
+
     Args:
         sys_argv (list): The system arguments
     """
+
     def __init__(self, sys_argv):
         """Initializes the NQRduck application."""
         super().__init__(sys_argv)
 
         self._main_model = MainModel()
         self._main_controller = MainController(self._main_model)
         self._main_view = MainView(self._main_model, self._main_controller)
 
         # Wait for the splash screen to close before starting the rest of the application
         self.processEvents()
 
         # Here the modules are loaded and signals connected
         self._main_controller.load_modules(self._main_view)
         # Get the first loaded module and set it as active
-        self._main_model.active_module = self._main_model.loaded_modules[list(self._main_model.loaded_modules.keys())[0]]
+        try:
+            self._main_model.active_module = self._main_model.loaded_modules[
+                list(self._main_model.loaded_modules.keys())[0]
+            ]
+        except IndexError:
+            logger.warning("No modules loaded")
+            # Start the install wizard if no modules are loaded
+            self._main_view.install_wizard = DuckWizard(
+                [], self._main_view
+            )
+            self._main_view.install_wizard.show()
+            self._main_view.install_wizard.exec()
 
         self._main_view.setWindowTitle("NQRduck")
         self._main_view.showMaximized()
 
         self._main_view.on_settings_changed()
 
+
 def handle_exception(exc_type, exc_value, exc_traceback):
     """Handle uncaught exceptions.
-    
+
     Args:
         exc_type (type): The type of the exception
         exc_value (Exception): The exception object
         exc_traceback (traceback): The traceback object
     """
-    logger.exception("An unhandled exception occurred: ", exc_info=(exc_type, exc_value, exc_traceback))
-    error_msg = ''.join(traceback.format_exception(exc_type, exc_value, exc_traceback))
+    logger.exception(
+        "An unhandled exception occurred: ",
+        exc_info=(exc_type, exc_value, exc_traceback),
+    )
+    error_msg = "".join(traceback.format_exception(exc_type, exc_value, exc_traceback))
+
+    QMessageBox.critical(
+        None, "Error", "An unhandled exception occurred:\n" + error_msg
+    )
 
-    QMessageBox.critical(None, "Error", "An unhandled exception occurred:\n" + error_msg)
-        
     sys.exit(1)
 
+
 def main():
     """Main entry point for the NQRduck application."""
     # Install the exception handler
-    sys.excepthook = handle_exception  
+    sys.excepthook = handle_exception
 
     # create logger
     logger = logging.getLogger()
     logger.setLevel(logging.DEBUG)
 
     # create console handler and set level to debug
     ch = logging.StreamHandler()
     ch.setLevel(logging.DEBUG)
 
     # create formatter
-    formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
+    formatter = logging.Formatter(
+        "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
+    )
 
     # add formatter to ch
     ch.setFormatter(formatter)
 
     # add ch to logger
     logger.addHandler(ch)
     # Stop matplotlib from spamming the DEBUG log level
-    logging.getLogger('matplotlib').setLevel(logging.WARNING)
+    logging.getLogger("matplotlib").setLevel(logging.WARNING)
 
     # Output log to log file to temp folder
     temp_folder = tempfile.gettempdir()
     # Rotate log files
-    fh = logging.handlers.RotatingFileHandler(os.path.join(temp_folder, 'nqrduck.log'), maxBytes=1000000, backupCount=5)
+    fh = logging.handlers.RotatingFileHandler(
+        os.path.join(temp_folder, "nqrduck.log"), maxBytes=1000000, backupCount=5
+    )
     fh.setLevel(logging.DEBUG)
     fh.setFormatter(formatter)
     fh.doRollover()
     logger.addHandler(fh)
 
-
     logger.debug("Starting QApplication ...")
-    
+
     application = NQRduck(sys.argv)
 
     exit_code = application.exec()
     sys.exit(exit_code)
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     main()
```

### Comparing `nqrduck-0.0.7/src/nqrduck/assets/animations.py` & `nqrduck-0.0.8/src/nqrduck/assets/animations.py`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.7/src/nqrduck/assets/icons.py` & `nqrduck-0.0.8/src/nqrduck/assets/icons.py`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.7/src/nqrduck/assets/animations/DuckKick_128x128.gif` & `nqrduck-0.0.8/src/nqrduck/assets/animations/DuckKick_128x128.gif`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.7/src/nqrduck/assets/animations/DuckSleep_128x128.gif` & `nqrduck-0.0.8/src/nqrduck/assets/animations/DuckSleep_128x128.gif`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.7/src/nqrduck/assets/logos/LabMallardnbg_32x32.png` & `nqrduck-0.0.8/src/nqrduck/assets/logos/LabMallardnbg_32x32.png`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.7/src/nqrduck/assets/logos/Logo_64x32.png` & `nqrduck-0.0.8/src/nqrduck/assets/logos/Logo_64x32.png`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.7/src/nqrduck/assets/logos/Logo_full.png` & `nqrduck-0.0.8/src/nqrduck/assets/logos/Logo_full.png`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.7/src/nqrduck/contrib/mplwidget.py` & `nqrduck-0.0.8/src/nqrduck/contrib/mplwidget.py`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.7/src/nqrduck/core/main_controller.py` & `nqrduck-0.0.8/src/nqrduck/core/main_controller.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 import logging
 import importlib
 import importlib.metadata
 
 import importlib
 from PyQt6.QtCore import QObject, pyqtSlot, pyqtSignal
 
+from .install_wizard import DuckWizard
+
 logger = logging.getLogger(__name__)
 
 
 class MainController(QObject):
     """The main controller of the application.
     
     This class loads all modules with entry points in the nqrduck group.
@@ -30,15 +32,15 @@
 
     def load_modules(self, main_view) -> None:
         """Loads all modules with entry points in the nqrduck group.
 
         Also connects the nqrduck_signal to the dispatch_signals slot and creates the menu bar entries.
 
         Args:
-        main_view (MainView): The main view of the application
+            main_view (MainView): The main view of the application
         """
         # Get the modules with entry points in the nqrduck group
         modules = self._get_modules()
         logger.debug("Found modules: %s", modules)
 
         for module_name, module in modules.items():
             # Connect the nqrduck_signal to the dispatch_signals slot
@@ -59,15 +61,15 @@
             module.view.add_menubar_item.connect(main_view.on_menu_bar_item_added)
 
             module.controller.on_loading()
 
         main_view.on_settings_changed()
 
     @pyqtSlot(str, object)
-    def dispatch_signals(self, key: str, value: object):
+    def dispatch_signals(self, key: str, value: object) -> None:
         """Dispatches the signals to the according module.
 
         This method is connected to the nqrduck_signal of the modules.
         It's the main way of communication between the modules.
 
         Args:
             key (str): The key of the signal
@@ -84,16 +86,28 @@
                 logger.debug("Showing notification: %s", value)
                 self.create_notification_dialog.emit(value)
                 break
 
             logger.debug("Dispatching signal %s to module: %s", key, module)
             module.controller.process_signals(key, value)
 
+    def on_install_wizard(self, main_view) -> None:
+        """Creates the install wizard.
+        
+        The main view is used as a parent for the wizard.
+        
+        Args:
+            main_view (MainView): The main view of the application
+        """
+        installed_modules = self._get_modules()
+        wizard = DuckWizard(installed_modules, parent=main_view)
+        wizard.exec()
+
     @staticmethod
-    def _get_modules():
+    def _get_modules() -> dict:
         """Returns a dictionary of all modules found in the entry points with 'nqrduck'.
 
         Returns dict: Dictionary of modules
         """
         modules = {}
 
         try:
```

### Comparing `nqrduck-0.0.7/src/nqrduck/core/main_model.py` & `nqrduck-0.0.8/src/nqrduck/core/main_model.py`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.7/src/nqrduck/core/main_view.py` & `nqrduck-0.0.8/src/nqrduck/core/main_view.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,14 +102,17 @@
 
         # Settings Changed
         self._main_model.settings.settings_changed.connect(self.on_settings_changed)
 
         # Preferences
         self._ui.actionPreferences.triggered.connect(self.on_preferences)
 
+        # Install Wizard
+        self._ui.actionInstall_Wizard.triggered.connect(lambda: self._main_controller.on_install_wizard(self))
+        
     @pyqtSlot(list)
     def create_notification_dialog(self, notification: list) -> None:
         """Creates a notification dialog with the given message and type.
 
         The type can be 'Info', 'Warning' or 'Error' and changes the color and symbol of the dialog.
 
         Args:
```

### Comparing `nqrduck-0.0.7/src/nqrduck/core/main_window.py` & `nqrduck-0.0.8/src/nqrduck/core/main_window.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-# Form implementation generated from reading ui file 'src/nqrduck/core/resources/main_window.ui'
+# Form implementation generated from reading ui file 'main_window.ui'
 #
-# Created by: PyQt6 UI code generator 6.5.1
+# Created by: PyQt6 UI code generator 6.7.0
 #
 # WARNING: Any manual changes made to this file will be lost when pyuic6 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
 from PyQt6 import QtCore, QtGui, QtWidgets
 
 
-class Ui_MainWindow:
+class Ui_MainWindow(object):
     def setupUi(self, MainWindow):
         MainWindow.setObjectName("MainWindow")
         MainWindow.resize(428, 296)
         self.centralwidget = QtWidgets.QWidget(parent=MainWindow)
         self.centralwidget.setObjectName("centralwidget")
         self.verticalLayout = QtWidgets.QVBoxLayout(self.centralwidget)
         self.verticalLayout.setObjectName("verticalLayout")
@@ -51,19 +51,23 @@
         self.actionAbout_Modules.setObjectName("actionAbout_Modules")
         self.actionAbout_NQRduck = QtGui.QAction(parent=MainWindow)
         self.actionAbout_NQRduck.setObjectName("actionAbout_NQRduck")
         self.actionLogger = QtGui.QAction(parent=MainWindow)
         self.actionLogger.setObjectName("actionLogger")
         self.actionPreferences = QtGui.QAction(parent=MainWindow)
         self.actionPreferences.setObjectName("actionPreferences")
+        self.actionInstall_Wizard = QtGui.QAction(parent=MainWindow)
+        self.actionInstall_Wizard.setObjectName("actionInstall_Wizard")
         self.menuFile.addSeparator()
         self.menuFile.addAction(self.actionAbout_Modules)
         self.menuFile.addAction(self.actionAbout_NQRduck)
         self.menuFile.addSeparator()
         self.menuFile.addAction(self.actionLogger)
+        self.menuFile.addSeparator()
+        self.menuFile.addAction(self.actionInstall_Wizard)
         self.menuPreferences.addAction(self.actionPreferences)
         self.menubar.addAction(self.menuPreferences.menuAction())
         self.menubar.addAction(self.menuFile.menuAction())
 
         self.retranslateUi(MainWindow)
         self.stackedWidget.setCurrentIndex(0)
         QtCore.QMetaObject.connectSlotsByName(MainWindow)
@@ -77,7 +81,8 @@
         self.actionNew.setText(_translate("MainWindow", "New"))
         self.actionSave_as.setText(_translate("MainWindow", "Save as ..."))
         self.actionLoad.setText(_translate("MainWindow", "Load"))
         self.actionAbout_Modules.setText(_translate("MainWindow", "About Modules"))
         self.actionAbout_NQRduck.setText(_translate("MainWindow", "About NQRduck"))
         self.actionLogger.setText(_translate("MainWindow", "Logger"))
         self.actionPreferences.setText(_translate("MainWindow", "Preferences"))
+        self.actionInstall_Wizard.setText(_translate("MainWindow", "Install Wizard"))
```

### Comparing `nqrduck-0.0.7/src/nqrduck/core/resources/logo.png` & `nqrduck-0.0.8/src/nqrduck/core/resources/logo.png`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.7/src/nqrduck/core/resources/main_window.ui` & `nqrduck-0.0.8/src/nqrduck/core/resources/main_window.ui`

 * *Files 3% similar despite different names*

#### Comparing `nqrduck-0.0.7/src/nqrduck/core/resources/main_window.ui` & `nqrduck-0.0.8/src/nqrduck/core/resources/main_window.ui`

```diff
@@ -40,14 +40,16 @@
           <string>Help</string>
         </property>
         <addaction name="separator"/>
         <addaction name="actionAbout_Modules"/>
         <addaction name="actionAbout_NQRduck"/>
         <addaction name="separator"/>
         <addaction name="actionLogger"/>
+        <addaction name="separator"/>
+        <addaction name="actionInstall_Wizard"/>
       </widget>
       <widget class="QMenu" name="menuPreferences">
         <property name="title">
           <string>Settings</string>
         </property>
         <addaction name="actionPreferences"/>
       </widget>
@@ -97,11 +99,16 @@
       </property>
     </action>
     <action name="actionPreferences">
       <property name="text">
         <string>Preferences</string>
       </property>
     </action>
+    <action name="actionInstall_Wizard">
+      <property name="text">
+        <string>Install Wizard</string>
+      </property>
+    </action>
   </widget>
   <resources/>
   <connections/>
 </ui>
```

### Comparing `nqrduck-0.0.7/src/nqrduck/core/resources/font/AsepriteFont.ttf` & `nqrduck-0.0.8/src/nqrduck/core/resources/font/AsepriteFont.ttf`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.7/src/nqrduck/helpers/duckwidgets.py` & `nqrduck-0.0.8/src/nqrduck/helpers/duckwidgets.py`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.7/src/nqrduck/helpers/formbuilder.py` & `nqrduck-0.0.8/src/nqrduck/helpers/formbuilder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """A module that allows for easy creation of form views in the NQRduck framework."""
 
 import logging
 import functools
-from decimal import Decimal
 from PyQt6.QtCore import pyqtSlot
 from PyQt6.QtWidgets import (
     QDialog,
     QVBoxLayout,
     QHBoxLayout,
     QLabel,
     QWidget,
```

### Comparing `nqrduck-0.0.7/src/nqrduck/helpers/functions.py` & `nqrduck-0.0.8/src/nqrduck/helpers/functions.py`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.7/src/nqrduck/helpers/serializer.py` & `nqrduck-0.0.8/src/nqrduck/helpers/serializer.py`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.7/src/nqrduck/helpers/signalprocessing.py` & `nqrduck-0.0.8/src/nqrduck/helpers/signalprocessing.py`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.7/src/nqrduck/helpers/unitconverter.py` & `nqrduck-0.0.8/src/nqrduck/helpers/unitconverter.py`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.7/src/nqrduck/helpers/validators.py` & `nqrduck-0.0.8/src/nqrduck/helpers/validators.py`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.7/src/nqrduck/module/module.py` & `nqrduck-0.0.8/src/nqrduck/module/module.py`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.7/src/nqrduck/module/module_controller.py` & `nqrduck-0.0.8/src/nqrduck/module/module_controller.py`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.7/src/nqrduck/module/module_model.py` & `nqrduck-0.0.8/src/nqrduck/module/module_model.py`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.7/src/nqrduck/module/module_view.py` & `nqrduck-0.0.8/src/nqrduck/module/module_view.py`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.7/tests/test_load_module.py` & `nqrduck-0.0.8/tests/test_load_module.py`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.7/LICENSE` & `nqrduck-0.0.8/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 jupfi
+Copyright (c) 2023-2024 jupfi
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `nqrduck-0.0.7/README.md` & `nqrduck-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.7/pyproject.toml` & `nqrduck-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [project]
 name = "nqrduck"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="jupfi", email="support@nqrduck.cool" },
 ]
 
 description = "Simple Python script to interact with various python modules used for magnetic resonance spectroscopy."
 readme = "README.md"
 license = { file="LICENSE" }
```

### Comparing `nqrduck-0.0.7/PKG-INFO` & `nqrduck-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.3
 Name: nqrduck
-Version: 0.0.7
+Version: 0.0.8
 Summary: Simple Python script to interact with various python modules used for magnetic resonance spectroscopy.
 Project-URL: Homepage, https://nqrduck.cool
 Project-URL: Bug Tracker, https://github.com/nqrduck/nqrduck/issues
 Project-URL: Source Code, https://github.com/nqrduck/nqrduck
 Author-email: jupfi <support@nqrduck.cool>
 License: MIT License
         
-        Copyright (c) 2023 jupfi
+        Copyright (c) 2023-2024 jupfi
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
```

