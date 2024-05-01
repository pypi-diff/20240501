# Comparing `tmp/Wendigo-0.1.0.tar.gz` & `tmp/Wendigo-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\Wendigo-0.1.0.tar", last modified: Sun Oct 11 02:34:05 2020, max compression
+gzip compressed data, was "dist\Wendigo-0.1.1.tar", last modified: Wed May  1 16:21:00 2024, max compression
```

## Comparing `Wendigo-0.1.0.tar` & `Wendigo-0.1.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxrwx   0        0        0        0 2020-10-11 02:34:05.609249 Wendigo-0.1.0/
--rw-rw-rw-   0        0        0       31 2020-10-10 13:48:43.000000 Wendigo-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     5760 2020-10-11 02:34:05.607231 Wendigo-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     4380 2020-10-11 02:09:38.000000 Wendigo-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2020-10-11 02:34:05.379201 Wendigo-0.1.0/Wendigo.egg-info/
--rw-rw-rw-   0        0        0     5760 2020-10-11 02:34:05.000000 Wendigo-0.1.0/Wendigo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1108 2020-10-11 02:34:05.000000 Wendigo-0.1.0/Wendigo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-10-11 02:34:05.000000 Wendigo-0.1.0/Wendigo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       74 2020-10-11 02:34:05.000000 Wendigo-0.1.0/Wendigo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2020-10-11 02:34:05.000000 Wendigo-0.1.0/Wendigo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2020-10-11 02:34:05.609249 Wendigo-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      820 2020-10-11 02:32:24.000000 Wendigo-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2020-10-11 02:34:05.393164 Wendigo-0.1.0/wendigo/
--rw-rw-rw-   0        0        0      115 2020-10-03 07:56:48.000000 Wendigo-0.1.0/wendigo/__init__.py
-drwxrwxrwx   0        0        0        0 2020-10-11 02:34:05.403137 Wendigo-0.1.0/wendigo/application/
--rw-rw-rw-   0        0        0       24 2020-10-10 13:16:05.000000 Wendigo-0.1.0/wendigo/application/__init__.py
--rw-rw-rw-   0        0        0       31 2020-09-06 07:43:09.000000 Wendigo-0.1.0/wendigo/application/dll.py
-drwxrwxrwx   0        0        0        0 2020-10-11 02:34:05.367234 Wendigo-0.1.0/wendigo/bin/
-drwxrwxrwx   0        0        0        0 2020-10-11 02:34:05.408124 Wendigo-0.1.0/wendigo/bin/x64/
--rw-rw-rw-   0        0        0    12800 2020-10-09 13:02:15.000000 Wendigo-0.1.0/wendigo/bin/x64/Application.dll
--rw-rw-rw-   0        0        0    26112 2020-10-10 10:57:07.000000 Wendigo-0.1.0/wendigo/bin/x64/Device.dll
--rw-rw-rw-   0        0        0     4608 2020-10-09 13:02:15.000000 Wendigo-0.1.0/wendigo/bin/x64/Process.dll
--rw-rw-rw-   0        0        0    17408 2020-10-10 10:57:08.000000 Wendigo-0.1.0/wendigo/bin/x64/Screen.dll
--rw-rw-rw-   0        0        0     2463 2020-10-10 09:06:19.000000 Wendigo-0.1.0/wendigo/core.py
-drwxrwxrwx   0        0        0        0 2020-10-11 02:34:05.426080 Wendigo-0.1.0/wendigo/device/
--rw-rw-rw-   0        0        0      185 2020-10-10 13:27:25.000000 Wendigo-0.1.0/wendigo/device/__init__.py
--rw-rw-rw-   0        0        0     3483 2020-10-09 12:19:16.000000 Wendigo-0.1.0/wendigo/device/core.py
--rw-rw-rw-   0        0        0      181 2020-10-08 12:02:20.000000 Wendigo-0.1.0/wendigo/device/dll.py
--rw-rw-rw-   0        0        0     7633 2020-10-09 11:07:08.000000 Wendigo-0.1.0/wendigo/device/event_dispatcher.py
--rw-rw-rw-   0        0        0      984 2020-10-03 07:00:32.000000 Wendigo-0.1.0/wendigo/device/event_imitator.py
--rw-rw-rw-   0        0        0     2474 2020-10-09 12:12:22.000000 Wendigo-0.1.0/wendigo/device/event_simulator.py
--rw-rw-rw-   0        0        0      112 2020-10-03 09:13:33.000000 Wendigo-0.1.0/wendigo/exceptions.py
--rw-rw-rw-   0        0        0      344 2020-10-03 09:14:09.000000 Wendigo-0.1.0/wendigo/logger.py
-drwxrwxrwx   0        0        0        0 2020-10-11 02:34:05.438044 Wendigo-0.1.0/wendigo/process/
--rw-rw-rw-   0        0        0       35 2020-10-10 13:16:16.000000 Wendigo-0.1.0/wendigo/process/__init__.py
--rw-rw-rw-   0        0        0       30 2020-08-23 06:03:22.000000 Wendigo-0.1.0/wendigo/process/dll.py
--rw-rw-rw-   0        0        0      768 2020-10-03 07:11:25.000000 Wendigo-0.1.0/wendigo/process/time_keeper.py
-drwxrwxrwx   0        0        0        0 2020-10-11 02:34:05.585358 Wendigo-0.1.0/wendigo/screen/
--rw-rw-rw-   0        0        0      199 2020-10-10 13:28:22.000000 Wendigo-0.1.0/wendigo/screen/__init__.py
--rw-rw-rw-   0        0        0      109 2020-10-03 07:48:30.000000 Wendigo-0.1.0/wendigo/screen/dll.py
--rw-rw-rw-   0        0        0     4740 2020-10-03 08:21:56.000000 Wendigo-0.1.0/wendigo/screen/form_controller.py
--rw-rw-rw-   0        0        0      977 2020-10-03 07:52:59.000000 Wendigo-0.1.0/wendigo/screen/target_form.py
--rw-rw-rw-   0        0        0     2094 2020-10-03 08:08:05.000000 Wendigo-0.1.0/wendigo/screen/target_marker.py
--rw-rw-rw-   0        0        0     8371 2020-10-03 08:42:01.000000 Wendigo-0.1.0/wendigo/screen/target_seeker.py
--rw-rw-rw-   0        0        0     2090 2020-10-03 08:51:52.000000 Wendigo-0.1.0/wendigo/screen/text_reader.py
-drwxrwxrwx   0        0        0        0 2020-10-11 02:34:05.601249 Wendigo-0.1.0/wendigo/setup/
--rw-rw-rw-   0        0        0       68 2020-08-22 06:57:53.000000 Wendigo-0.1.0/wendigo/setup/__init__.py
--rw-rw-rw-   0        0        0      937 2020-10-03 08:56:03.000000 Wendigo-0.1.0/wendigo/setup/check.py
--rw-rw-rw-   0        0        0      646 2020-10-03 08:59:49.000000 Wendigo-0.1.0/wendigo/setup/cleanup.py
--rw-rw-rw-   0        0        0      367 2020-10-10 13:33:24.000000 Wendigo-0.1.0/wendigo/setup/import_.py
-drwxrwxrwx   0        0        0        0 2020-10-11 02:34:05.606232 Wendigo-0.1.0/wendigo/system/
--rw-rw-rw-   0        0        0      175 2020-10-03 07:55:16.000000 Wendigo-0.1.0/wendigo/system/__init__.py
--rw-rw-rw-   0        0        0     5885 2020-10-03 09:04:13.000000 Wendigo-0.1.0/wendigo/system/color.py
--rw-rw-rw-   0        0        0     4052 2020-10-10 08:12:58.000000 Wendigo-0.1.0/wendigo/system/keys.py
--rw-rw-rw-   0        0        0      110 2020-08-22 06:52:10.000000 Wendigo-0.1.0/wendigo/warnings.py
--rw-rw-rw-   0        0        0     2625 2020-10-10 13:29:13.000000 Wendigo-0.1.0/wendigo/wendigo.py
+drwxrwxrwx   0        0        0        0 2024-05-01 16:21:00.763290 Wendigo-0.1.1/
+-rw-rw-rw-   0        0        0       31 2020-10-10 13:48:43.000000 Wendigo-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     5721 2024-05-01 16:21:00.762304 Wendigo-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4349 2024-05-01 15:25:12.000000 Wendigo-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-01 16:21:00.667290 Wendigo-0.1.1/Wendigo.egg-info/
+-rw-rw-rw-   0        0        0     5721 2024-05-01 16:21:00.000000 Wendigo-0.1.1/Wendigo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1108 2024-05-01 16:21:00.000000 Wendigo-0.1.1/Wendigo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 16:21:00.000000 Wendigo-0.1.1/Wendigo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2024-05-01 16:21:00.000000 Wendigo-0.1.1/Wendigo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-01 16:21:00.000000 Wendigo-0.1.1/Wendigo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-01 16:21:00.764291 Wendigo-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      645 2024-05-01 13:19:06.000000 Wendigo-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 16:21:00.680290 Wendigo-0.1.1/wendigo/
+-rw-rw-rw-   0        0        0      115 2020-10-03 07:56:48.000000 Wendigo-0.1.1/wendigo/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 16:21:00.684292 Wendigo-0.1.1/wendigo/application/
+-rw-rw-rw-   0        0        0       24 2020-10-10 13:16:05.000000 Wendigo-0.1.1/wendigo/application/__init__.py
+-rw-rw-rw-   0        0        0       31 2020-09-06 07:43:09.000000 Wendigo-0.1.1/wendigo/application/dll.py
+drwxrwxrwx   0        0        0        0 2024-05-01 16:21:00.629743 Wendigo-0.1.1/wendigo/bin/
+drwxrwxrwx   0        0        0        0 2024-05-01 16:21:00.696292 Wendigo-0.1.1/wendigo/bin/x64/
+-rw-rw-rw-   0        0        0    12800 2020-10-09 13:02:15.000000 Wendigo-0.1.1/wendigo/bin/x64/Application.dll
+-rw-rw-rw-   0        0        0    26112 2020-10-10 10:57:07.000000 Wendigo-0.1.1/wendigo/bin/x64/Device.dll
+-rw-rw-rw-   0        0        0     4608 2020-10-09 13:02:15.000000 Wendigo-0.1.1/wendigo/bin/x64/Process.dll
+-rw-rw-rw-   0        0        0    17408 2020-10-10 10:57:08.000000 Wendigo-0.1.1/wendigo/bin/x64/Screen.dll
+-rw-rw-rw-   0        0        0     2463 2020-10-10 09:06:19.000000 Wendigo-0.1.1/wendigo/core.py
+drwxrwxrwx   0        0        0        0 2024-05-01 16:21:00.711292 Wendigo-0.1.1/wendigo/device/
+-rw-rw-rw-   0        0        0      185 2020-10-10 13:27:25.000000 Wendigo-0.1.1/wendigo/device/__init__.py
+-rw-rw-rw-   0        0        0     3768 2024-05-01 15:23:14.000000 Wendigo-0.1.1/wendigo/device/core.py
+-rw-rw-rw-   0        0        0      181 2020-10-08 12:02:20.000000 Wendigo-0.1.1/wendigo/device/dll.py
+-rw-rw-rw-   0        0        0     7710 2024-05-01 15:21:12.000000 Wendigo-0.1.1/wendigo/device/event_dispatcher.py
+-rw-rw-rw-   0        0        0     1041 2024-05-01 15:17:57.000000 Wendigo-0.1.1/wendigo/device/event_imitator.py
+-rw-rw-rw-   0        0        0     2510 2024-05-01 14:54:17.000000 Wendigo-0.1.1/wendigo/device/event_simulator.py
+-rw-rw-rw-   0        0        0      112 2020-10-03 09:13:33.000000 Wendigo-0.1.1/wendigo/exceptions.py
+-rw-rw-rw-   0        0        0      344 2020-10-03 09:14:09.000000 Wendigo-0.1.1/wendigo/logger.py
+drwxrwxrwx   0        0        0        0 2024-05-01 16:21:00.717296 Wendigo-0.1.1/wendigo/process/
+-rw-rw-rw-   0        0        0       35 2020-10-10 13:16:16.000000 Wendigo-0.1.1/wendigo/process/__init__.py
+-rw-rw-rw-   0        0        0       30 2020-08-23 06:03:22.000000 Wendigo-0.1.1/wendigo/process/dll.py
+-rw-rw-rw-   0        0        0      777 2024-05-01 15:21:16.000000 Wendigo-0.1.1/wendigo/process/time_keeper.py
+drwxrwxrwx   0        0        0        0 2024-05-01 16:21:00.748290 Wendigo-0.1.1/wendigo/screen/
+-rw-rw-rw-   0        0        0      199 2020-10-10 13:28:22.000000 Wendigo-0.1.1/wendigo/screen/__init__.py
+-rw-rw-rw-   0        0        0      109 2020-10-03 07:48:30.000000 Wendigo-0.1.1/wendigo/screen/dll.py
+-rw-rw-rw-   0        0        0     4705 2024-05-01 15:31:17.000000 Wendigo-0.1.1/wendigo/screen/form_controller.py
+-rw-rw-rw-   0        0        0      977 2020-10-03 07:52:59.000000 Wendigo-0.1.1/wendigo/screen/target_form.py
+-rw-rw-rw-   0        0        0     2130 2024-05-01 15:24:16.000000 Wendigo-0.1.1/wendigo/screen/target_marker.py
+-rw-rw-rw-   0        0        0     8318 2024-05-01 15:31:39.000000 Wendigo-0.1.1/wendigo/screen/target_seeker.py
+-rw-rw-rw-   0        0        0     2090 2020-10-03 08:51:52.000000 Wendigo-0.1.1/wendigo/screen/text_reader.py
+drwxrwxrwx   0        0        0        0 2024-05-01 16:21:00.755290 Wendigo-0.1.1/wendigo/setup/
+-rw-rw-rw-   0        0        0       68 2020-08-22 06:57:53.000000 Wendigo-0.1.1/wendigo/setup/__init__.py
+-rw-rw-rw-   0        0        0      937 2020-10-03 08:56:03.000000 Wendigo-0.1.1/wendigo/setup/check.py
+-rw-rw-rw-   0        0        0      646 2020-10-03 08:59:49.000000 Wendigo-0.1.1/wendigo/setup/cleanup.py
+-rw-rw-rw-   0        0        0      367 2020-10-10 13:33:24.000000 Wendigo-0.1.1/wendigo/setup/import_.py
+drwxrwxrwx   0        0        0        0 2024-05-01 16:21:00.760306 Wendigo-0.1.1/wendigo/system/
+-rw-rw-rw-   0        0        0      175 2020-10-03 07:55:16.000000 Wendigo-0.1.1/wendigo/system/__init__.py
+-rw-rw-rw-   0        0        0     5885 2020-10-03 09:04:13.000000 Wendigo-0.1.1/wendigo/system/color.py
+-rw-rw-rw-   0        0        0     4052 2024-05-01 13:31:21.000000 Wendigo-0.1.1/wendigo/system/keys.py
+-rw-rw-rw-   0        0        0      110 2020-08-22 06:52:10.000000 Wendigo-0.1.1/wendigo/warnings.py
+-rw-rw-rw-   0        0        0     2586 2024-05-01 15:16:18.000000 Wendigo-0.1.1/wendigo/wendigo.py
```

### Comparing `Wendigo-0.1.0/PKG-INFO` & `Wendigo-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,75 +1,74 @@
 Metadata-Version: 2.1
 Name: Wendigo
-Version: 0.1.0
+Version: 0.1.1
 Summary: Wendigo is a RPA library for Windows (64 bit).
 Home-page: https://github.com/medmsyk/wendigopy
 Author: medmsyk
 Author-email: michael.lee.maeda@gmail.com
 License: Apache License 2.0
 Description: # WendigoPy
         <p align="center">
           <img src="https://raw.githubusercontent.com/medmsyk/wendigopy/master/img/logo.png" alt="Wendigo"/>
         </p>
         
         WendigoPy is a RPA library for Windows (64 bit).  
         
         ## Caution
         
-        ### About Simulation
+        ### Simulation
         WendigoPy uses [SendInput](https://docs.microsoft.com/en-us/windows/win32/api/winuser/nf-winuser-sendinput) to simulate inputs (implemented as [WendigoCs](https://github.com/medmsyk/wendigocs)).  
         If you're new to it, please be careful of the things below.  
         
         * It does NOT wait until the inputs are processed.  
         * The inputs which you sent can NOT be cancelled.  
         * So do NOT send many inputs at once, nor at the same time.  
         Once you've done it, the inputs which you sent will be unstoppable.  
         * Pressed keys must be released.  
         If you left some keys pressed in your program, press and release the keys manually to recover.  
         * Some kinds of applications ignore this type of simulation.  
         
-        ### About Exit
+        ### Exit
         If something went wrong, you should stop Wendigo immediately.  
         These are the ways to exit.  
         
         * Press the keys to exit which are shown in the console.  
         The keys are two shift keys (LShift+RShift) if you didn't change them.  
         * Right click on the tasktray icon indicates "W" and Choose "Exit".  
         * If it's urgent, press Ctrl+Alt+Del and kill the process by Task Manager.  
         This way blocks sending new inputs, but remember what I told you before "the inputs which you sent will be unstoppable".
         
         ## Requirements
         * Windows (64 bit)  
         Testing on Windows 10.  
         * Python 3  
-        Testing on 3.8.0.  
+        Testing on 3.12.3.  
         * [Tesseract](https://github.com/tesseract-ocr/tesseract)  
         If you wanna use the OCR functions.  
         
         ## Installation
         ```
         pip install wendigo
         ```
         
         ## Usage
         Wendigo is an event driven application.  
-        ```
+        ```python
         from wendigo import Wendigo as w
         
         # Do something here
         
         # Blocks until Wendigo is stopped.
         w.run()
         ```
         
         ### Hook
         Hook events of keyboard or mouse like this.  
         It works even if another form is active.  
-        ```
-        from typing import List
+        ```python
         from wendigo import Keys, Wendigo as w
         from wendigo.device import DeviceState
         from wendigo.screen import TargetForm
         
         def key_up(state: DeviceState):
             # Shows which keys are pressed.
             print(state.key.keys)
@@ -77,29 +76,29 @@
             print(state.mouse.position)
             # Shows the state of wheel.
             print(state.mouse.scroll)
         
         # Runs key_up when you release Ctrl+Alt+W.
         w.event_dispatcher.key_up("key_up", [Keys.ControlKey, Keys.AltKey, Keys.W], key_up)
         
-        def mark_by_drag(targets: List[TargetForm]):
+        def mark_by_drag(targets: list[TargetForm]):
             # Shows area where you marked.
             print(targets[0].area)
         
-        # Runs mark_by_drag when you drag with Ctrl.
-        w.target_marker.mark_by_drag(mark_by_drag, keys=[Keys.ControlKey])
+        # Runs mark_by_drag when you drag.
+        w.target_marker.mark_by_drag(mark_by_drag, keys=[Keys.LButton])
         
         # Blocks until Wendigo is stopped.
         w.run()
         ```
         
         ### Simulation
         Simulate events of keyboard or mouse like this.  
         Make sure that you activated a text editor before you press the keys.  
-        ```
+        ```python
         from wendigo import Keys, Point, Wendigo as w
         from wendigo.device import DeviceState, Inputs
         
         def key_up(state: DeviceState):
             # Types "Hello World!".
             w.event_simulator.type_text("Hello World!")
             # Need more manual way?
```

### Comparing `Wendigo-0.1.0/README.md` & `Wendigo-0.1.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -3,65 +3,64 @@
   <img src="https://raw.githubusercontent.com/medmsyk/wendigopy/master/img/logo.png" alt="Wendigo"/>
 </p>
 
 WendigoPy is a RPA library for Windows (64 bit).  
 
 ## Caution
 
-### About Simulation
+### Simulation
 WendigoPy uses [SendInput](https://docs.microsoft.com/en-us/windows/win32/api/winuser/nf-winuser-sendinput) to simulate inputs (implemented as [WendigoCs](https://github.com/medmsyk/wendigocs)).  
 If you're new to it, please be careful of the things below.  
 
 * It does NOT wait until the inputs are processed.  
 * The inputs which you sent can NOT be cancelled.  
 * So do NOT send many inputs at once, nor at the same time.  
 Once you've done it, the inputs which you sent will be unstoppable.  
 * Pressed keys must be released.  
 If you left some keys pressed in your program, press and release the keys manually to recover.  
 * Some kinds of applications ignore this type of simulation.  
 
-### About Exit
+### Exit
 If something went wrong, you should stop Wendigo immediately.  
 These are the ways to exit.  
 
 * Press the keys to exit which are shown in the console.  
 The keys are two shift keys (LShift+RShift) if you didn't change them.  
 * Right click on the tasktray icon indicates "W" and Choose "Exit".  
 * If it's urgent, press Ctrl+Alt+Del and kill the process by Task Manager.  
 This way blocks sending new inputs, but remember what I told you before "the inputs which you sent will be unstoppable".
 
 ## Requirements
 * Windows (64 bit)  
 Testing on Windows 10.  
 * Python 3  
-Testing on 3.8.0.  
+Testing on 3.12.3.  
 * [Tesseract](https://github.com/tesseract-ocr/tesseract)  
 If you wanna use the OCR functions.  
 
 ## Installation
 ```
 pip install wendigo
 ```
 
 ## Usage
 Wendigo is an event driven application.  
-```
+```python
 from wendigo import Wendigo as w
 
 # Do something here
 
 # Blocks until Wendigo is stopped.
 w.run()
 ```
 
 ### Hook
 Hook events of keyboard or mouse like this.  
 It works even if another form is active.  
-```
-from typing import List
+```python
 from wendigo import Keys, Wendigo as w
 from wendigo.device import DeviceState
 from wendigo.screen import TargetForm
 
 def key_up(state: DeviceState):
     # Shows which keys are pressed.
     print(state.key.keys)
@@ -69,29 +68,29 @@
     print(state.mouse.position)
     # Shows the state of wheel.
     print(state.mouse.scroll)
 
 # Runs key_up when you release Ctrl+Alt+W.
 w.event_dispatcher.key_up("key_up", [Keys.ControlKey, Keys.AltKey, Keys.W], key_up)
 
-def mark_by_drag(targets: List[TargetForm]):
+def mark_by_drag(targets: list[TargetForm]):
     # Shows area where you marked.
     print(targets[0].area)
 
-# Runs mark_by_drag when you drag with Ctrl.
-w.target_marker.mark_by_drag(mark_by_drag, keys=[Keys.ControlKey])
+# Runs mark_by_drag when you drag.
+w.target_marker.mark_by_drag(mark_by_drag, keys=[Keys.LButton])
 
 # Blocks until Wendigo is stopped.
 w.run()
 ```
 
 ### Simulation
 Simulate events of keyboard or mouse like this.  
 Make sure that you activated a text editor before you press the keys.  
-```
+```python
 from wendigo import Keys, Point, Wendigo as w
 from wendigo.device import DeviceState, Inputs
 
 def key_up(state: DeviceState):
     # Types "Hello World!".
     w.event_simulator.type_text("Hello World!")
     # Need more manual way?
```

### Comparing `Wendigo-0.1.0/Wendigo.egg-info/PKG-INFO` & `Wendigo-0.1.1/Wendigo.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,75 +1,74 @@
 Metadata-Version: 2.1
 Name: Wendigo
-Version: 0.1.0
+Version: 0.1.1
 Summary: Wendigo is a RPA library for Windows (64 bit).
 Home-page: https://github.com/medmsyk/wendigopy
 Author: medmsyk
 Author-email: michael.lee.maeda@gmail.com
 License: Apache License 2.0
 Description: # WendigoPy
         <p align="center">
           <img src="https://raw.githubusercontent.com/medmsyk/wendigopy/master/img/logo.png" alt="Wendigo"/>
         </p>
         
         WendigoPy is a RPA library for Windows (64 bit).  
         
         ## Caution
         
-        ### About Simulation
+        ### Simulation
         WendigoPy uses [SendInput](https://docs.microsoft.com/en-us/windows/win32/api/winuser/nf-winuser-sendinput) to simulate inputs (implemented as [WendigoCs](https://github.com/medmsyk/wendigocs)).  
         If you're new to it, please be careful of the things below.  
         
         * It does NOT wait until the inputs are processed.  
         * The inputs which you sent can NOT be cancelled.  
         * So do NOT send many inputs at once, nor at the same time.  
         Once you've done it, the inputs which you sent will be unstoppable.  
         * Pressed keys must be released.  
         If you left some keys pressed in your program, press and release the keys manually to recover.  
         * Some kinds of applications ignore this type of simulation.  
         
-        ### About Exit
+        ### Exit
         If something went wrong, you should stop Wendigo immediately.  
         These are the ways to exit.  
         
         * Press the keys to exit which are shown in the console.  
         The keys are two shift keys (LShift+RShift) if you didn't change them.  
         * Right click on the tasktray icon indicates "W" and Choose "Exit".  
         * If it's urgent, press Ctrl+Alt+Del and kill the process by Task Manager.  
         This way blocks sending new inputs, but remember what I told you before "the inputs which you sent will be unstoppable".
         
         ## Requirements
         * Windows (64 bit)  
         Testing on Windows 10.  
         * Python 3  
-        Testing on 3.8.0.  
+        Testing on 3.12.3.  
         * [Tesseract](https://github.com/tesseract-ocr/tesseract)  
         If you wanna use the OCR functions.  
         
         ## Installation
         ```
         pip install wendigo
         ```
         
         ## Usage
         Wendigo is an event driven application.  
-        ```
+        ```python
         from wendigo import Wendigo as w
         
         # Do something here
         
         # Blocks until Wendigo is stopped.
         w.run()
         ```
         
         ### Hook
         Hook events of keyboard or mouse like this.  
         It works even if another form is active.  
-        ```
-        from typing import List
+        ```python
         from wendigo import Keys, Wendigo as w
         from wendigo.device import DeviceState
         from wendigo.screen import TargetForm
         
         def key_up(state: DeviceState):
             # Shows which keys are pressed.
             print(state.key.keys)
@@ -77,29 +76,29 @@
             print(state.mouse.position)
             # Shows the state of wheel.
             print(state.mouse.scroll)
         
         # Runs key_up when you release Ctrl+Alt+W.
         w.event_dispatcher.key_up("key_up", [Keys.ControlKey, Keys.AltKey, Keys.W], key_up)
         
-        def mark_by_drag(targets: List[TargetForm]):
+        def mark_by_drag(targets: list[TargetForm]):
             # Shows area where you marked.
             print(targets[0].area)
         
-        # Runs mark_by_drag when you drag with Ctrl.
-        w.target_marker.mark_by_drag(mark_by_drag, keys=[Keys.ControlKey])
+        # Runs mark_by_drag when you drag.
+        w.target_marker.mark_by_drag(mark_by_drag, keys=[Keys.LButton])
         
         # Blocks until Wendigo is stopped.
         w.run()
         ```
         
         ### Simulation
         Simulate events of keyboard or mouse like this.  
         Make sure that you activated a text editor before you press the keys.  
-        ```
+        ```python
         from wendigo import Keys, Point, Wendigo as w
         from wendigo.device import DeviceState, Inputs
         
         def key_up(state: DeviceState):
             # Types "Hello World!".
             w.event_simulator.type_text("Hello World!")
             # Need more manual way?
```

### Comparing `Wendigo-0.1.0/Wendigo.egg-info/SOURCES.txt` & `Wendigo-0.1.1/Wendigo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Wendigo-0.1.0/setup.py` & `Wendigo-0.1.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,17 @@
-from glob import glob
 from setuptools import find_packages, setup
 from pip._internal.req import parse_requirements
 
-if __name__ == "__main__":
-    install_requires = [
-        str(ir.requirement)
-        for ir in parse_requirements("./requirements.txt", session=False)
-    ]
-
-    setup(
-        name="Wendigo",
-        version="0.1.0",
-        description="Wendigo is a RPA library for Windows (64 bit).",
-        long_description=open("README.md").read(),
-        long_description_content_type="text/markdown",
-        author="medmsyk",
-        author_email="michael.lee.maeda@gmail.com",
-        install_requires=install_requires,
-        url="https://github.com/medmsyk/wendigopy",
-        license="Apache License 2.0",
-        packages=find_packages(),
-        include_package_data=True
-    )
+setup(
+    name="Wendigo",
+    version="0.1.1",
+    description="Wendigo is a RPA library for Windows (64 bit).",
+    long_description=open("README.md").read(),
+    long_description_content_type="text/markdown",
+    author="medmsyk",
+    author_email="michael.lee.maeda@gmail.com",
+    install_requires=[str(ir.requirement) for ir in parse_requirements("./requirements.txt", session=False)],
+    url="https://github.com/medmsyk/wendigopy",
+    license="Apache License 2.0",
+    packages=find_packages(),
+    include_package_data=True
+)
```

### Comparing `Wendigo-0.1.0/wendigo/bin/x64/Application.dll` & `Wendigo-0.1.1/wendigo/bin/x64/Application.dll`

 * *Files identical despite different names*

### Comparing `Wendigo-0.1.0/wendigo/bin/x64/Device.dll` & `Wendigo-0.1.1/wendigo/bin/x64/Device.dll`

 * *Files identical despite different names*

### Comparing `Wendigo-0.1.0/wendigo/bin/x64/Process.dll` & `Wendigo-0.1.1/wendigo/bin/x64/Process.dll`

 * *Files identical despite different names*

### Comparing `Wendigo-0.1.0/wendigo/bin/x64/Screen.dll` & `Wendigo-0.1.1/wendigo/bin/x64/Screen.dll`

 * *Files identical despite different names*

### Comparing `Wendigo-0.1.0/wendigo/core.py` & `Wendigo-0.1.1/wendigo/core.py`

 * *Files identical despite different names*

### Comparing `Wendigo-0.1.0/wendigo/device/core.py` & `Wendigo-0.1.1/wendigo/device/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from collections import namedtuple
 from enum import IntEnum
-from typing import List, Union
+from System.Windows.Forms import Keys as FormKey
 from wendigo import Keys
 from wendigo.core import Point
 from wendigo.device.dll import DeviceEventArgs, Inputs as DllInputs
 
 class DeviceEvent(IntEnum):
     """
     Device event.
@@ -13,67 +13,78 @@
     KeyDown    =  0
     KeyPress   =  1
     KeyUp      =  2
     MouseMove  =  3
     MouseWheel =  4
     MouseTilt  =  5
 
+class FormKeys(list[FormKey]):
+    def __init__(self, keys: Keys | list[Keys]) -> None:
+        """
+        Constructor.
+
+        Parameters
+        ----------
+        keys: Keys.
+        """
+        self.extend([FormKey(key) for key in ([keys] if isinstance(keys, Keys) else keys)])
+
 class Inputs(DllInputs):
     """
     Inputs.
     """
-    def key_down(self, keys: Union[Keys, List[Keys]], n: int=1) -> "Inputs":
+    def key_down(self, keys: Keys | list[Keys], n: int=1) -> "Inputs":
         """
         Define inputs for key down.
 
         Parameters
         ----------
         keys: Keys.
         n: Number of inputs.
 
         Returns
         -------
         inputs: Inputs.
         """
-        super().KeyDown(keys, n)
+        super().KeyDown(FormKeys(keys), n)
         return self
-        
-    def key_up(self, keys: Union[Keys, List[Keys]], n: int=1) -> "Inputs":
+
+    def key_up(self, keys: Keys | list[Keys], n: int=1) -> "Inputs":
         """
         Define inputs for key up.
 
         Parameters
         ----------
         keys: Keys.
         n: Number of inputs.
 
         Returns
         -------
         inputs: Inputs.
         """
-        super().KeyUp(keys, n)
+        super().KeyUp(FormKeys(keys), n)
         return self
-        
-    def key_press(self, keys: Union[Keys, List[Keys]], n: int=1) -> "Inputs":
+
+    def key_press(self, keys: Keys | list[Keys], n: int=1) -> "Inputs":
         """
         Define inputs for key press.
 
         Parameters
         ----------
         keys: Keys.
         n: Number of inputs.
 
         Returns
         -------
         inputs: Inputs.
         """
-        super().KeyPress(keys, n)
+        super().KeyPress(FormKeys(keys), n)
         return self
-        
-    def key_press_text(self, texts: Union[str, List[str]], n: int=1) -> "Inputs":
+
+    def key_press_text(self, texts: str | list[str], n: int=1) -> "Inputs":
         """
         Define inputs for key press by texts.
 
         Parameters
         ----------
         texts: Texts.
         n: Number of inputs.
@@ -96,15 +107,15 @@
 
         Returns
         -------
         inputs: Inputs.
         """
         super().Tilt(value, n)
         return self
-        
+
     def wheel(self, value: int, n: int=1) -> "Inputs":
         """
         Define inputs for mouse wheel.
 
         Parameters
         ----------
         value: Value.
@@ -130,21 +141,21 @@
 
         Parameters
         ----------
         e: Device event args.
         """
         state = e.State
 
-        self.event_type = DeviceEvent(state.DeviceEvent)
+        self.event_type = DeviceEvent(int(state.DeviceEvent))
         self.key = key_state(
             target=state.Key.Target,
             keys={entry.Key: entry.Value for entry in state.Key.Keys},
         )
 
         position = state.Mouse.Position
         scroll = state.Mouse.Scroll
-        
+
         self.mouse = mouse_state(
             target=state.Mouse.Target,
             position=Point(position.X, position.Y),
             scroll=Point(scroll.X, scroll.Y),
         )
```

### Comparing `Wendigo-0.1.0/wendigo/device/event_dispatcher.py` & `Wendigo-0.1.1/wendigo/device/event_dispatcher.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from typing import Callable, List
+from collections.abc import Callable
 from wendigo import Keys
 from wendigo.device import DeviceState
+from wendigo.device.core import FormKeys
 from wendigo.device.dll import EventDispatcher as DllEventDispatcher, \
      DeviceEventArgs, DeviceEventHandler
 from wendigo.logger import Logger
 
 class EventDispatcher:
     """
     Event dispatcher.
@@ -48,162 +49,162 @@
                 cls.unlisten(name)
                 event_handler(DeviceState(e))
             except:
                 Logger.exception("An exception raised in event hadler")
         return DeviceEventHandler(wrapper)
 
     @classmethod
-    def key_down(cls, name: str, keys: List[Keys], event_handler: Callable[[DeviceState], None], for_system: bool=False):
+    def key_down(cls, name: str, keys: list[Keys], event_handler: Callable[[DeviceState], None], for_system: bool=False):
         """
         Listen for key down.
 
         Parameters
         ----------
         name: Name.
         keys: Keys.
         event_handler: Event handler.
         for_system: The event is for system or not.
         """
-        DllEventDispatcher.KeyDown(name, keys, cls.get_event_handler(event_handler), for_system)
+        DllEventDispatcher.KeyDown(name, FormKeys(keys), cls.get_event_handler(event_handler), for_system)
 
     @classmethod
-    def key_down_once(cls, name: str, keys: List[Keys], event_handler: Callable[[DeviceState], None], for_system: bool=False):
+    def key_down_once(cls, name: str, keys: list[Keys], event_handler: Callable[[DeviceState], None], for_system: bool=False):
         """
         Listen for key down which is called only once.
 
         Parameters
         ----------
         name: Name.
         keys: Keys.
         event_handler: Event handler.
         for_system: The event is for system or not.
         """
-        DllEventDispatcher.KeyDown(name, keys, cls.get_event_handler_once(name, event_handler), for_system)
+        DllEventDispatcher.KeyDown(name, FormKeys(keys), cls.get_event_handler_once(name, event_handler), for_system)
 
     @classmethod
-    def key_up(cls, name: str, keys: List[Keys], event_handler: Callable[[DeviceState], None], for_system: bool=False):
+    def key_up(cls, name: str, keys: list[Keys], event_handler: Callable[[DeviceState], None], for_system: bool=False):
         """
         Listen for key up.
 
         Parameters
         ----------
         name: Name.
         keys: Keys.
         event_handler: Event handler.
         for_system: The event is for system or not.
         """
-        DllEventDispatcher.KeyUp(name, keys, cls.get_event_handler(event_handler), for_system)
+        DllEventDispatcher.KeyUp(name, FormKeys(keys), cls.get_event_handler(event_handler), for_system)
 
     @classmethod
-    def key_up_once(cls, name: str, keys: List[Keys], event_handler: Callable[[DeviceState], None], for_system: bool=False):
+    def key_up_once(cls, name: str, keys: list[Keys], event_handler: Callable[[DeviceState], None], for_system: bool=False):
         """
         Listen for key up which is called only once.
 
         Parameters
         ----------
         name: Name.
         keys: Keys.
         event_handler: Event handler.
         for_system: The event is for system or not.
         """
-        DllEventDispatcher.KeyUp(name, keys, cls.get_event_handler_once(name, event_handler), for_system)
-    
+        DllEventDispatcher.KeyUp(name, FormKeys(keys), cls.get_event_handler_once(name, event_handler), for_system)
+
     @classmethod
-    def key_press(cls, name: str, keys: List[Keys], event_handler: Callable[[DeviceState], None], for_system: bool=False):
+    def key_press(cls, name: str, keys: list[Keys], event_handler: Callable[[DeviceState], None], for_system: bool=False):
         """
         Listen for key press.
 
         Parameters
         ----------
         name: Name.
         keys: Keys.
         event_handler: Event handler.
         for_system: The event is for system or not.
         """
-        DllEventDispatcher.KeyPress(name, keys, cls.get_event_handler(event_handler), for_system)
-    
+        DllEventDispatcher.KeyPress(name, FormKeys(keys), cls.get_event_handler(event_handler), for_system)
+
     @classmethod
-    def key_press_once(cls, name: str, keys: List[Keys], event_handler: Callable[[DeviceState], None], for_system: bool=False):
+    def key_press_once(cls, name: str, keys: list[Keys], event_handler: Callable[[DeviceState], None], for_system: bool=False):
         """
         Listen for key press which is called only once.
 
         Parameters
         ----------
         name: Name.
         keys: Keys.
         event_handler: Event handler.
         for_system: The event is for system or not.
         """
-        DllEventDispatcher.KeyPress(name, keys, cls.get_event_handler_once(name, event_handler), for_system)
+        DllEventDispatcher.KeyPress(name, FormKeys(keys), cls.get_event_handler_once(name, event_handler), for_system)
 
     @classmethod
     def mouse_move(cls, name: str, event_handler: Callable[[DeviceState], None], for_system: bool=False):
         """
         Listen for mouse move.
 
         Parameters
         ----------
         name: Name.
         event_handler: Event handler.
         for_system: The event is for system or not.
         """
         DllEventDispatcher.MouseMove(name, cls.get_event_handler(event_handler), for_system)
-    
+
     @classmethod
     def mouse_move_once(cls, name: str, event_handler: Callable[[DeviceState], None], for_system: bool=False):
         """
         Listen for mouse move which is called only once.
 
         Parameters
         ----------
         name: Name.
         event_handler: Event handler.
         for_system: The event is for system or not.
         """
         DllEventDispatcher.MouseMove(name, cls.get_event_handler_once(name, event_handler), for_system)
-    
+
     @classmethod
     def mouse_wheel(cls, name: str, event_handler: Callable[[DeviceState], None], for_system: bool=False):
         """
         Listen for mouse wheel.
 
         Parameters
         ----------
         name: Name.
         event_handler: Event handler.
         for_system: The event is for system or not.
         """
         DllEventDispatcher.MouseWheel(name, cls.get_event_handler(event_handler), for_system)
-    
+
     @classmethod
     def mouse_wheel_once(cls, name: str, event_handler: Callable[[DeviceState], None], for_system: bool=False):
         """
         Listen for mouse wheel which is called only once.
 
         Parameters
         ----------
         name: Name.
         event_handler: Event handler.
         for_system: The event is for system or not.
         """
         DllEventDispatcher.MouseWheel(name, cls.get_event_handler_once(name, event_handler), for_system)
-    
+
     @classmethod
     def mouse_tilt(cls, name: str, event_handler: Callable[[DeviceState], None], for_system: bool=False):
         """
         Listen for mouse tilt.
 
         Parameters
         ----------
         name: Name.
         event_handler: Event handler.
         for_system: The event is for system or not.
         """
         DllEventDispatcher.MouseTilt(name, cls.get_event_handler(event_handler), for_system)
-    
+
     @classmethod
     def mouse_tilt_once(cls, name: str, event_handler: Callable[[DeviceState], None], for_system: bool=False):
         """
         Listen for mouse tilt which is called only once.
 
         Parameters
         ----------
```

### Comparing `Wendigo-0.1.0/wendigo/device/event_imitator.py` & `Wendigo-0.1.1/wendigo/device/event_imitator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-from typing import List
 from wendigo import Keys
+from wendigo.device.core import FormKeys
 from wendigo.device.dll import EventImitator as DllEventImitator
 
 class EventImitator():
     """
     Event imitator.
     """
     @classmethod
-    def record(cls, path: str, start_keys: List[Keys], stop_keys: List[Keys]):
+    def record(cls, path: str, start_keys: list[Keys], stop_keys: list[Keys]):
         """
         Record device events.
         Key events for start_keys and stop_keys are ignored.
 
         Parameters
         ----------
         path: File path.
         start_keys: Keys to start recording.
         stop_keys: Keys to stop recording.
         """
-        DllEventImitator.Record(path, start_keys, stop_keys)
+        DllEventImitator.Record(path, FormKeys(start_keys), FormKeys(stop_keys))
 
     @classmethod
-    def play(cls, path: str, start_keys: List[Keys], stop_keys: List[Keys]):
+    def play(cls, path: str, start_keys: list[Keys], stop_keys: list[Keys]):
         """
         Play device events.
 
         Parameters
         ----------
         path: File path.
         start_keys: Keys to start playing.
         stop_keys: Keys to stop playing.
         """
-        DllEventImitator.Play(path, start_keys, stop_keys)
+        DllEventImitator.Play(path, FormKeys(start_keys), FormKeys(stop_keys))
```

### Comparing `Wendigo-0.1.0/wendigo/device/event_simulator.py` & `Wendigo-0.1.1/wendigo/device/event_simulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from wendigo import Keys, Point
-from wendigo.device.core import Inputs
+from wendigo.device.core import FormKey, Inputs
 from wendigo.device.dll import EventSimulator as DllEventSimulator
 
 class EventSimulator():
     """
     Event simulator.
     """
     @classmethod
@@ -23,39 +23,39 @@
         Simulate key down.
 
         Parameters
         ----------
         key: Key.
         n: Number of inputs.
         """
-        DllEventSimulator.KeyDown(key, n)
+        DllEventSimulator.KeyDown(FormKey(key), n)
 
     @classmethod
     def key_up(cls, key: Keys, n: int=1):
         """
         Simulate key up.
 
         Parameters
         ----------
         key: Key.
         n: Number of inputs.
         """
-        DllEventSimulator.KeyUp(key, n)
+        DllEventSimulator.KeyUp(FormKey(key), n)
 
     @classmethod
     def key_press(cls, key: Keys, n: int=1):
         """
         Simulate key press.
 
         Parameters
         ----------
         key: Key.
         n: Number of inputs.
         """
-        DllEventSimulator.KeyPress(key, n)
+        DllEventSimulator.KeyPress(FormKey(key), n)
 
     @classmethod
     def type_text(cls, text: str, n: int=1):
         """
         Type text.
 
         Parameters
```

### Comparing `Wendigo-0.1.0/wendigo/process/time_keeper.py` & `Wendigo-0.1.1/wendigo/process/time_keeper.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Callable
+from collections.abc import Callable
 from wendigo.system import Action
 from wendigo.process.dll import TimeKeeper as DllTimeKeeper
 
 class TimeKeeper(DllTimeKeeper):
     """
     Time keeper.
     """
```

### Comparing `Wendigo-0.1.0/wendigo/screen/form_controller.py` & `Wendigo-0.1.1/wendigo/screen/form_controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import numpy as np
 import warnings
 from collections import namedtuple
 from PIL import ImageGrab
+from PIL.Image import Image
 from time import sleep
-from typing import List, Union
 from wendigo import IS_ADMIN, Colors, Point
 from wendigo.core import Area, Point
 from wendigo.screen.dll import FormController as DllFormController
 from wendigo.system.color import Color
 from wendigo.warnings import AdministrationWarning
 
 FormInfo = namedtuple("FormInfo", ("form_class", "form_title"))
 
 class FormController:
     """
     Form controller.
     """
     @classmethod
-    def get_form_info(cls) -> List[FormInfo]:
+    def get_form_info(cls) -> list[FormInfo]:
         """
         Get form information.
 
         Returns
         -------
         form_info: Form information.
         """
@@ -74,15 +74,15 @@
         Returns
         -------
         color: Color.
         """
         return Colors.to_color(DllFormController.GetColor(position.x, position.y))
 
     @classmethod
-    def _capture(cls, area: Area, scale: float, grayscale: bool, as_array: bool) -> Union["Image", np.ndarray]:
+    def _capture(cls, area: Area, scale: float, grayscale: bool, as_array: bool) -> Image | np.ndarray:
         """
         Capture screen.
 
         Parameters
         ----------
         area: Area.
         scale: Scale.
@@ -98,15 +98,15 @@
         if scale != 1.0:
             image = image.resize((round(image.width * scale), round(image.height * scale)))
         if grayscale:
             image = image.convert("L")
         return np.array(image) if as_array else image
 
     @classmethod
-    def capture(cls, area: Area=None, scale: float=1.0, grayscale: bool=False, as_array: bool=False) -> Union["Image", np.ndarray]:
+    def capture(cls, area: Area=None, scale: float=1.0, grayscale: bool=False, as_array: bool=False) -> Image | np.ndarray:
         """
         Capture screen.
 
         Parameters
         ----------
         area: Area.
         scale: Scale.
@@ -117,15 +117,15 @@
         -------
         image: Image.
         """
         return cls._capture(area, scale, grayscale, as_array)
 
     @classmethod
     def capture_window(cls, form_class: str=None, form_title: str=None, client_only: bool=False,
-        scale: float=1.0, grayscale: bool=False, as_array: bool=False) -> Union["Image", np.ndarray]:
+        scale: float=1.0, grayscale: bool=False, as_array: bool=False) -> Image | np.ndarray:
         """
         Capture window.
 
         Parameters
         ----------
         form_class: Form class.
         form_title: Form title.
@@ -140,9 +140,9 @@
         """
         if form_class is None and form_title is None:
             raise ValueError("Form class or title must be specified.")
 
         cls.activate_form(form_class=form_class, form_title=form_title)
         area = cls.get_area(form_class=form_class, form_title=form_title, client_only=client_only)
         if area is None: return None    # Form doesn't exist.
-        
+
         return cls._capture(area, scale, grayscale, as_array)
```

### Comparing `Wendigo-0.1.0/wendigo/screen/target_form.py` & `Wendigo-0.1.1/wendigo/screen/target_form.py`

 * *Files identical despite different names*

### Comparing `Wendigo-0.1.0/wendigo/screen/target_marker.py` & `Wendigo-0.1.1/wendigo/screen/target_marker.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from typing import Callable, List, Union
+from collections.abc import Callable
 from wendigo import Area, Colors, Keys
 from wendigo.logger import Logger
+from wendigo.device.core import FormKeys
 from wendigo.screen.dll import TargetMarker as DllTargetMarker, TargetMarkEventHandler
 from wendigo.screen.target_form import TargetForm
 from wendigo.system import Rectangle
 
 class TargetMarker(DllTargetMarker):
     """
     Target marker.
@@ -23,15 +24,15 @@
         Returns
         -------
         target: Target.
         """
         return TargetForm(cls.Mark(Rectangle(area.x, area.y, area.width, area.height), border_width, border_color))
 
     @classmethod
-    def get_event_handler(cls, event_handler: Callable[[List[TargetForm]], None]) -> TargetMarkEventHandler:
+    def get_event_handler(cls, event_handler: Callable[[list[TargetForm]], None]) -> TargetMarkEventHandler:
         """
         Get an event handler.
 
         Parameters
         ----------
         event_handler: Event handler.
 
@@ -43,21 +44,21 @@
             try:
                 event_handler([TargetForm(target) for target in event_args.Targets])
             except:
                 Logger.exception("An exception raised in event hadler")
         return TargetMarkEventHandler(wrapper)
 
     @classmethod
-    def mark_by_drag(cls, event_handler: Callable[[List[TargetForm]], None],
-        keys: List[Keys]=None, n: int=1, border_width: Union[int, List[int]]=None, border_color: Union[Colors, List[Colors]]=None):
+    def mark_by_drag(cls, event_handler: Callable[[list[TargetForm]], None],
+        keys: list[Keys]=None, n: int=1, border_width: int | list[int]=None, border_color: Colors | list[Colors]=None):
         """
         Mark areas by drag.
 
         Parameters
         ----------
         event_handler: Event handler.
         keys: Keys.
         n: Number of targets.
         border_width: Border width(s).
         border_color: Border color(s).
         """
-        cls.MarkByDrag(cls.get_event_handler(event_handler), keys, n, border_width, border_color)
+        cls.MarkByDrag(cls.get_event_handler(event_handler), FormKeys(keys), n, border_width, border_color)
```

### Comparing `Wendigo-0.1.0/wendigo/screen/target_seeker.py` & `Wendigo-0.1.1/wendigo/screen/target_seeker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import cv2
 import numpy as np
 from enum import Enum
 from pathlib import Path
-from typing import List, Tuple
+from PIL.Image import Image
 from wendigo.core import Area
 from wendigo.screen.form_controller import FormController
 
 class HaarCascade(Enum):
     """
     Haar cascade classifiers.
     """
@@ -17,15 +17,15 @@
 
 class TargetSeeker:
     """
     Target seeker.
     """
     @classmethod
     def seek(cls, template: str, scale: float=1.0, threshold: float=0.8,
-        form_class: str=None, form_title: str=None, client_only: bool=False) -> Tuple[Area, float]:
+        form_class: str=None, form_title: str=None, client_only: bool=False) -> tuple[Area, float]:
         """
         Seek a target.
 
         Parameters
         ----------
         template: Template file path.
         scale: Scale.
@@ -47,20 +47,20 @@
 
         if scale != 1.0:
             template = cv2.resize(template, (round(width * scale), round(height * scale)))
 
         res = cv2.matchTemplate(image, template, cv2.TM_CCOEFF_NORMED)
         pt = np.unravel_index(np.argmax(res), res.shape)[::-1]
         probability = res[pt[1]][pt[0]]
-        
+
         s = 1 / scale
         return Area(pt[0] * s, pt[1] * s, width, height) if probability >= threshold else None, probability
 
     @classmethod
-    def _detect(cls, haar_cascade: HaarCascade, image: "Image", scale: float, **kwargs) -> List[Area]:
+    def _detect(cls, haar_cascade: HaarCascade, image: Image, scale: float, **kwargs) -> list[Area]:
         """
         Detect something.
 
         Parameters
         ----------
         haar_cascade: Haar cascade classifier.
         image: Image.
@@ -74,74 +74,74 @@
         path = str(Path(cv2.__path__[0]).joinpath("data", haar_cascade.value))
         detected = cv2.CascadeClassifier(path).detectMultiScale(image, **kwargs)
 
         s = 1 / scale
         return [Area(x * s, y * s, w * s, h * s) for x, y, w, h in detected]
 
     @classmethod
-    def _detect_area(cls, haar_cascade: HaarCascade, area: Area, scale: float, **kwargs) -> List[Area]:
+    def _detect_area(cls, haar_cascade: HaarCascade, area: Area, scale: float, **kwargs) -> list[Area]:
         """
         Detect something in an area.
-        
+
         Parameters
         ----------
         haar_cascade: Haar cascade classifier.
         area: Area.
         scale: Scale.
         kwargs: Args for detectMultiScale.
-        
+
         Returns
         -------
         areas: Areas.
         """
         image = FormController.capture(area=area, scale=scale, grayscale=True, as_array=True)
         return cls._detect(haar_cascade, image, scale, **kwargs)
 
     @classmethod
     def _detect_window(cls, haar_cascade: HaarCascade,
-        form_class: str, form_title: str, client_only: bool, scale: float, **kwargs) -> List[Area]:
+        form_class: str, form_title: str, client_only: bool, scale: float, **kwargs) -> list[Area]:
         """
         Detect something in a window.
 
         Parameters
         ----------
         haar_cascade: Haar cascade classifier.
         form_class: Form class.
         form_title: Form title.
         client_only: Only the client area or not.
         scale: Scale.
         kwargs: Args for detectMultiScale.
-        
+
         Returns
         -------
         areas: Areas.
         """
         image = FormController.capture_window(form_class=form_class, form_title=form_title, client_only=client_only, scale=scale, grayscale=True, as_array=True)
         return cls._detect(haar_cascade, image, scale, **kwargs) if image is not None else []
 
     @classmethod
-    def detect_frontalfaces(cls, area: Area=None, scale: float=1.0, **kwargs) -> List[Area]:
+    def detect_frontalfaces(cls, area: Area=None, scale: float=1.0, **kwargs) -> list[Area]:
         """
         Detect frontal faces.
 
         Parameters
         ----------
         area: Area.
         scale: Scale.
         kwargs: Args for detectMultiScale.
 
         Returns
         -------
         areas: Areas.
         """
         return cls._detect_area(HaarCascade.Frontalface, area, scale, **kwargs)
-    
+
     @classmethod
     def detect_frontalfaces_window(cls, form_class: str=None, form_title: str=None, client_only: bool=False,
-        scale: float=1.0, **kwargs) -> List[Area]:
+        scale: float=1.0, **kwargs) -> list[Area]:
         """
         Detect frontal faces in a window.
 
         Parameters
         ----------
         form_class: Form class.
         form_title: Form title.
@@ -152,33 +152,33 @@
         Returns
         -------
         areas: Areas.
         """
         return cls._detect_window(HaarCascade.Frontalface, form_class, form_title, client_only, scale, **kwargs)
 
     @classmethod
-    def detect_upperbodies(cls, area: Area=None, scale: float=1.0, **kwargs) -> List[Area]:
+    def detect_upperbodies(cls, area: Area=None, scale: float=1.0, **kwargs) -> list[Area]:
         """
         Detect upper bodies.
 
         Parameters
         ----------
         area: Area.
         scale: Scale.
         kwargs: Args for detectMultiScale.
 
         Returns
         -------
         areas: Areas.
         """
         return cls._detect_area(HaarCascade.Upperbody, area, scale, **kwargs)
-    
+
     @classmethod
     def detect_upperbodies_window(cls, form_class: str=None, form_title: str=None, client_only: bool=False,
-        scale: float=1.0, **kwargs) -> List[Area]:
+        scale: float=1.0, **kwargs) -> list[Area]:
         """
         Detect upper bodies in a window.
 
         Parameters
         ----------
         form_class: Form class.
         form_title: Form title.
@@ -189,33 +189,33 @@
         Returns
         -------
         areas: Areas.
         """
         return cls._detect_window(HaarCascade.Upperbody, form_class, form_title, client_only, scale, **kwargs)
 
     @classmethod
-    def detect_lowerbodies(cls, area: Area=None, scale: float=1.0, **kwargs) -> List[Area]:
+    def detect_lowerbodies(cls, area: Area=None, scale: float=1.0, **kwargs) -> list[Area]:
         """
         Detect lower bodies.
 
         Parameters
         ----------
         area: Area.
         scale: Scale.
         kwargs: Args for detectMultiScale.
 
         Returns
         -------
         areas: Areas.
         """
         return cls._detect_area(HaarCascade.Lower_body, area, scale, **kwargs)
-    
+
     @classmethod
     def detect_lowerbodies_window(cls, form_class: str=None, form_title: str=None, client_only: bool=False,
-        scale: float=1.0, **kwargs) -> List[Area]:
+        scale: float=1.0, **kwargs) -> list[Area]:
         """
         Detect lower bodies in a window.
 
         Parameters
         ----------
         form_class: Form class.
         form_title: Form title.
@@ -226,33 +226,33 @@
         Returns
         -------
         areas: Areas.
         """
         return cls._detect_window(HaarCascade.Lower_body, form_class, form_title, client_only, scale, **kwargs)
 
     @classmethod
-    def detect_fullbodies(cls, area: Area=None, scale: float=1.0, **kwargs) -> List[Area]:
+    def detect_fullbodies(cls, area: Area=None, scale: float=1.0, **kwargs) -> list[Area]:
         """
         Detect full bodies.
 
         Parameters
         ----------
         area: Area.
         scale: Scale.
         kwargs: Args for detectMultiScale.
 
         Returns
         -------
         areas: Areas.
         """
         return cls._detect_area(HaarCascade.Fullbody, area, scale, **kwargs)
-    
+
     @classmethod
     def detect_fullbodies_window(cls, form_class: str=None, form_title: str=None, client_only: bool=False,
-        scale: float=1.0, **kwargs) -> List[Area]:
+        scale: float=1.0, **kwargs) -> list[Area]:
         """
         Detect full bodies in a window.
 
         Parameters
         ----------
         form_class: Form class.
         form_title: Form title.
```

### Comparing `Wendigo-0.1.0/wendigo/screen/text_reader.py` & `Wendigo-0.1.1/wendigo/screen/text_reader.py`

 * *Files identical despite different names*

### Comparing `Wendigo-0.1.0/wendigo/setup/check.py` & `Wendigo-0.1.1/wendigo/setup/check.py`

 * *Files identical despite different names*

### Comparing `Wendigo-0.1.0/wendigo/setup/cleanup.py` & `Wendigo-0.1.1/wendigo/setup/cleanup.py`

 * *Files identical despite different names*

### Comparing `Wendigo-0.1.0/wendigo/system/color.py` & `Wendigo-0.1.1/wendigo/system/color.py`

 * *Files identical despite different names*

### Comparing `Wendigo-0.1.0/wendigo/system/keys.py` & `Wendigo-0.1.1/wendigo/system/keys.py`

 * *Files identical despite different names*

### Comparing `Wendigo-0.1.0/wendigo/wendigo.py` & `Wendigo-0.1.1/wendigo/wendigo.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-from typing import List
 from wendigo import Keys
 from wendigo.application import Wendigo as DllWendigo
 from wendigo.device import EventDispatcher, EventImitator, EventSimulator
 from wendigo.logger import Logger
 from wendigo.process import TimeKeeper
 from wendigo.screen import FormController, TargetMarker, TargetSeeker, TextReader
-from wendigo.system import EventHandler, Keys
+from wendigo.system import Keys
 
 class Wendigo:
     """
     Wendigo.
     """
     event_dispatcher = EventDispatcher
     event_imitator = EventImitator
@@ -32,15 +31,15 @@
         title: Title.
         text: Text.
         timeout: Timeout.
         """
         DllWendigo.Notify(title, text, timeout)
 
     @classmethod
-    def add_exit(cls, keys: List[Keys], caption_tasktray: str, caption_handler: str) -> str:
+    def add_exit(cls, keys: list[Keys], caption_tasktray: str, caption_handler: str) -> str:
         """
         Add exit.
 
         Parameters
         ----------
         keys: Keys to exit.
         caption_tasktray: Caption for the tasktray item to exit.
@@ -55,15 +54,15 @@
         # Add a key down event handler to exit.
         Logger.info(caption_handler.format(keys=caption))
         cls.event_dispatcher.key_down("exit", keys, lambda state: cls.exit(), for_system=True)
 
         return caption_tasktray.format(keys=caption)
 
     @classmethod
-    def run(cls, name: str=None, icon_path: str=None, exit_keys: List[Keys]=[Keys.LShiftKey, Keys.RShiftKey],
+    def run(cls, name: str=None, icon_path: str=None, exit_keys: list[Keys]=[Keys.LShiftKey, Keys.RShiftKey],
         exit_caption_tasktray: str="Exit ({keys})", exit_caption_handler: str="* Press {keys} to exit"):
         """
         Run.
 
         Parameters
         ----------
         name: Name.
```

