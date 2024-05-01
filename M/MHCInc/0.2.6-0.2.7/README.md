# Comparing `tmp/mhcinc-0.2.6.tar.gz` & `tmp/mhcinc-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mhcinc-0.2.6.tar", last modified: Tue Apr 30 15:50:31 2024, max compression
+gzip compressed data, was "mhcinc-0.2.7.tar", last modified: Tue Apr 30 15:56:52 2024, max compression
```

## Comparing `mhcinc-0.2.6.tar` & `mhcinc-0.2.7.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-30 15:50:31.650340 mhcinc-0.2.6/
--rw-r--r--   0 mac        (501) staff       (20)     1074 2024-04-30 14:10:51.000000 mhcinc-0.2.6/LICENSE
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-30 15:50:31.645223 mhcinc-0.2.6/MHCInc/
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-30 15:50:31.649092 mhcinc-0.2.6/MHCInc/MHCInc/
--rw-r--r--   0 mac        (501) staff       (20)     5891 2022-12-23 19:29:10.000000 mhcinc-0.2.6/MHCInc/MHCInc/GuessGame.py
--rw-r--r--   0 mac        (501) staff       (20)    15461 2022-12-23 19:29:10.000000 mhcinc-0.2.6/MHCInc/MHCInc/GuessGameEasy.py
--rw-r--r--   0 mac        (501) staff       (20)    11622 2022-12-23 19:29:10.000000 mhcinc-0.2.6/MHCInc/MHCInc/GuessGameSecondary.py
--rw-r--r--   0 mac        (501) staff       (20)     1211 2022-12-23 19:29:10.000000 mhcinc-0.2.6/MHCInc/MHCInc/MITLicense.py
--rw-r--r--   0 mac        (501) staff       (20)     3751 2024-04-30 14:03:53.000000 mhcinc-0.2.6/MHCInc/MHCInc/PHYSICAL_CONDITION_APPLET.py
--rw-r--r--   0 mac        (501) staff       (20)      808 2022-12-23 19:29:10.000000 mhcinc-0.2.6/MHCInc/MHCInc/Python3学习示例.py
--rw-r--r--   0 mac        (501) staff       (20)     4084 2022-12-23 19:29:10.000000 mhcinc-0.2.6/MHCInc/MHCInc/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     1028 2022-12-23 19:29:10.000000 mhcinc-0.2.6/MHCInc/MHCInc/animal_guess.py
--rw-r--r--   0 mac        (501) staff       (20)     4058 2022-12-23 19:29:10.000000 mhcinc-0.2.6/MHCInc/MHCInc/caterpillar.py
--rw-r--r--   0 mac        (501) staff       (20)     2891 2022-12-23 19:29:10.000000 mhcinc-0.2.6/MHCInc/MHCInc/caterpillar2.py
--rw-r--r--   0 mac        (501) staff       (20)     1148 2022-12-23 19:29:10.000000 mhcinc-0.2.6/MHCInc/MHCInc/copyright.py
--rw-r--r--   0 mac        (501) staff       (20)     3274 2022-12-23 19:29:10.000000 mhcinc-0.2.6/MHCInc/MHCInc/egg_catcher.py
--rw-r--r--   0 mac        (501) staff       (20)     3533 2024-04-30 14:02:46.000000 mhcinc-0.2.6/MHCInc/MHCInc/egg_catcher_perfect.py
--rw-r--r--   0 mac        (501) staff       (20)     1953 2024-04-30 14:03:06.000000 mhcinc-0.2.6/MHCInc/MHCInc/matchmaker.py
--rw-r--r--   0 mac        (501) staff       (20)     2917 2022-12-23 19:29:10.000000 mhcinc-0.2.6/MHCInc/MHCInc/random.py
--rw-r--r--   0 mac        (501) staff       (20)      846 2022-12-23 19:29:10.000000 mhcinc-0.2.6/MHCInc/MHCInc/rectangle.py
--rw-r--r--   0 mac        (501) staff       (20)     1211 2022-12-23 19:29:10.000000 mhcinc-0.2.6/MHCInc/MHCInc/robot_builder.py
--rw-r--r--   0 mac        (501) staff       (20)     4608 2022-12-23 19:29:10.000000 mhcinc-0.2.6/MHCInc/MHCInc/screen_pet.py
--rw-r--r--   0 mac        (501) staff       (20)     4285 2022-12-23 19:29:10.000000 mhcinc-0.2.6/MHCInc/MHCInc/swift.py
--rw-r--r--   0 mac        (501) staff       (20)     1570 2022-12-23 19:29:10.000000 mhcinc-0.2.6/MHCInc/MHCInc/加密消息.py
--rw-r--r--   0 mac        (501) staff       (20)     4373 2022-12-23 19:29:10.000000 mhcinc-0.2.6/MHCInc/MHCInc/单词九连猜.py
--rw-r--r--   0 mac        (501) staff       (20)      413 2022-12-23 19:29:10.000000 mhcinc-0.2.6/MHCInc/MHCInc/圆筒万花筒.py
--rw-r--r--   0 mac        (501) staff       (20)     3245 2022-12-23 19:29:10.000000 mhcinc-0.2.6/MHCInc/MHCInc/快照抓拍.py
--rw-r--r--   0 mac        (501) staff       (20)      805 2022-12-23 19:29:10.000000 mhcinc-0.2.6/MHCInc/MHCInc/星光夜空.py
--rw-r--r--   0 mac        (501) staff       (20)      576 2022-12-23 19:29:10.000000 mhcinc-0.2.6/MHCInc/MHCInc/螺旋万花筒.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-30 15:50:31.649900 mhcinc-0.2.6/MHCInc/MHCInc.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)     2853 2024-04-30 15:50:31.000000 mhcinc-0.2.6/MHCInc/MHCInc.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      985 2024-04-30 15:50:31.000000 mhcinc-0.2.6/MHCInc/MHCInc.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2024-04-30 15:50:31.000000 mhcinc-0.2.6/MHCInc/MHCInc.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)       25 2024-04-30 15:50:31.000000 mhcinc-0.2.6/MHCInc/MHCInc.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)        7 2024-04-30 15:50:31.000000 mhcinc-0.2.6/MHCInc/MHCInc.egg-info/top_level.txt
--rw-r--r--   0 mac        (501) staff       (20)     2853 2024-04-30 15:50:31.650124 mhcinc-0.2.6/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     2257 2024-04-30 15:41:38.000000 mhcinc-0.2.6/README.md
--rw-r--r--   0 mac        (501) staff       (20)       87 2022-12-23 19:29:10.000000 mhcinc-0.2.6/pyproject.toml
--rw-r--r--   0 mac        (501) staff       (20)       38 2024-04-30 15:50:31.650388 mhcinc-0.2.6/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)      894 2024-04-30 15:50:12.000000 mhcinc-0.2.6/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-30 15:56:52.160429 mhcinc-0.2.7/
+-rw-r--r--   0 mac        (501) staff       (20)     1074 2024-04-30 14:10:51.000000 mhcinc-0.2.7/LICENSE
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-30 15:56:52.155448 mhcinc-0.2.7/MHCInc/
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-30 15:56:52.159177 mhcinc-0.2.7/MHCInc/MHCInc/
+-rw-r--r--   0 mac        (501) staff       (20)     5891 2022-12-23 19:29:10.000000 mhcinc-0.2.7/MHCInc/MHCInc/GuessGame.py
+-rw-r--r--   0 mac        (501) staff       (20)    15461 2022-12-23 19:29:10.000000 mhcinc-0.2.7/MHCInc/MHCInc/GuessGameEasy.py
+-rw-r--r--   0 mac        (501) staff       (20)    11622 2022-12-23 19:29:10.000000 mhcinc-0.2.7/MHCInc/MHCInc/GuessGameSecondary.py
+-rw-r--r--   0 mac        (501) staff       (20)     1211 2022-12-23 19:29:10.000000 mhcinc-0.2.7/MHCInc/MHCInc/MITLicense.py
+-rw-r--r--   0 mac        (501) staff       (20)     3751 2024-04-30 14:03:53.000000 mhcinc-0.2.7/MHCInc/MHCInc/PHYSICAL_CONDITION_APPLET.py
+-rw-r--r--   0 mac        (501) staff       (20)      808 2022-12-23 19:29:10.000000 mhcinc-0.2.7/MHCInc/MHCInc/Python3学习示例.py
+-rw-r--r--   0 mac        (501) staff       (20)     4084 2022-12-23 19:29:10.000000 mhcinc-0.2.7/MHCInc/MHCInc/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     1028 2022-12-23 19:29:10.000000 mhcinc-0.2.7/MHCInc/MHCInc/animal_guess.py
+-rw-r--r--   0 mac        (501) staff       (20)     4058 2022-12-23 19:29:10.000000 mhcinc-0.2.7/MHCInc/MHCInc/caterpillar.py
+-rw-r--r--   0 mac        (501) staff       (20)     2891 2022-12-23 19:29:10.000000 mhcinc-0.2.7/MHCInc/MHCInc/caterpillar2.py
+-rw-r--r--   0 mac        (501) staff       (20)     1148 2022-12-23 19:29:10.000000 mhcinc-0.2.7/MHCInc/MHCInc/copyright.py
+-rw-r--r--   0 mac        (501) staff       (20)     3274 2022-12-23 19:29:10.000000 mhcinc-0.2.7/MHCInc/MHCInc/egg_catcher.py
+-rw-r--r--   0 mac        (501) staff       (20)     3543 2024-04-30 15:56:16.000000 mhcinc-0.2.7/MHCInc/MHCInc/egg_catcher_perfect.py
+-rw-r--r--   0 mac        (501) staff       (20)     1963 2024-04-30 15:56:16.000000 mhcinc-0.2.7/MHCInc/MHCInc/matchmaker.py
+-rw-r--r--   0 mac        (501) staff       (20)     2917 2022-12-23 19:29:10.000000 mhcinc-0.2.7/MHCInc/MHCInc/random.py
+-rw-r--r--   0 mac        (501) staff       (20)      846 2022-12-23 19:29:10.000000 mhcinc-0.2.7/MHCInc/MHCInc/rectangle.py
+-rw-r--r--   0 mac        (501) staff       (20)     1211 2022-12-23 19:29:10.000000 mhcinc-0.2.7/MHCInc/MHCInc/robot_builder.py
+-rw-r--r--   0 mac        (501) staff       (20)     4608 2022-12-23 19:29:10.000000 mhcinc-0.2.7/MHCInc/MHCInc/screen_pet.py
+-rw-r--r--   0 mac        (501) staff       (20)     4285 2022-12-23 19:29:10.000000 mhcinc-0.2.7/MHCInc/MHCInc/swift.py
+-rw-r--r--   0 mac        (501) staff       (20)     1570 2022-12-23 19:29:10.000000 mhcinc-0.2.7/MHCInc/MHCInc/加密消息.py
+-rw-r--r--   0 mac        (501) staff       (20)     4373 2022-12-23 19:29:10.000000 mhcinc-0.2.7/MHCInc/MHCInc/单词九连猜.py
+-rw-r--r--   0 mac        (501) staff       (20)      413 2022-12-23 19:29:10.000000 mhcinc-0.2.7/MHCInc/MHCInc/圆筒万花筒.py
+-rw-r--r--   0 mac        (501) staff       (20)     3245 2022-12-23 19:29:10.000000 mhcinc-0.2.7/MHCInc/MHCInc/快照抓拍.py
+-rw-r--r--   0 mac        (501) staff       (20)      805 2022-12-23 19:29:10.000000 mhcinc-0.2.7/MHCInc/MHCInc/星光夜空.py
+-rw-r--r--   0 mac        (501) staff       (20)      576 2022-12-23 19:29:10.000000 mhcinc-0.2.7/MHCInc/MHCInc/螺旋万花筒.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-30 15:56:52.159994 mhcinc-0.2.7/MHCInc/MHCInc.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)     2853 2024-04-30 15:56:52.000000 mhcinc-0.2.7/MHCInc/MHCInc.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      985 2024-04-30 15:56:52.000000 mhcinc-0.2.7/MHCInc/MHCInc.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2024-04-30 15:56:52.000000 mhcinc-0.2.7/MHCInc/MHCInc.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)       25 2024-04-30 15:56:52.000000 mhcinc-0.2.7/MHCInc/MHCInc.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)        7 2024-04-30 15:56:52.000000 mhcinc-0.2.7/MHCInc/MHCInc.egg-info/top_level.txt
+-rw-r--r--   0 mac        (501) staff       (20)     2853 2024-04-30 15:56:52.160210 mhcinc-0.2.7/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     2257 2024-04-30 15:41:38.000000 mhcinc-0.2.7/README.md
+-rw-r--r--   0 mac        (501) staff       (20)       87 2022-12-23 19:29:10.000000 mhcinc-0.2.7/pyproject.toml
+-rw-r--r--   0 mac        (501) staff       (20)       38 2024-04-30 15:56:52.160479 mhcinc-0.2.7/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)      894 2024-04-30 15:56:49.000000 mhcinc-0.2.7/setup.py
```

### Comparing `mhcinc-0.2.6/LICENSE` & `mhcinc-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mhcinc-0.2.6/MHCInc/MHCInc/GuessGame.py` & `mhcinc-0.2.7/MHCInc/MHCInc/GuessGame.py`

 * *Files identical despite different names*

### Comparing `mhcinc-0.2.6/MHCInc/MHCInc/GuessGameEasy.py` & `mhcinc-0.2.7/MHCInc/MHCInc/GuessGameEasy.py`

 * *Files identical despite different names*

### Comparing `mhcinc-0.2.6/MHCInc/MHCInc/GuessGameSecondary.py` & `mhcinc-0.2.7/MHCInc/MHCInc/GuessGameSecondary.py`

 * *Files identical despite different names*

### Comparing `mhcinc-0.2.6/MHCInc/MHCInc/MITLicense.py` & `mhcinc-0.2.7/MHCInc/MHCInc/MITLicense.py`

 * *Files identical despite different names*

### Comparing `mhcinc-0.2.6/MHCInc/MHCInc/PHYSICAL_CONDITION_APPLET.py` & `mhcinc-0.2.7/MHCInc/MHCInc/PHYSICAL_CONDITION_APPLET.py`

 * *Files identical despite different names*

### Comparing `mhcinc-0.2.6/MHCInc/MHCInc/Python3学习示例.py` & `mhcinc-0.2.7/MHCInc/MHCInc/Python3学习示例.py`

 * *Files identical despite different names*

### Comparing `mhcinc-0.2.6/MHCInc/MHCInc/__init__.py` & `mhcinc-0.2.7/MHCInc/MHCInc/__init__.py`

 * *Files identical despite different names*

### Comparing `mhcinc-0.2.6/MHCInc/MHCInc/animal_guess.py` & `mhcinc-0.2.7/MHCInc/MHCInc/animal_guess.py`

 * *Files identical despite different names*

### Comparing `mhcinc-0.2.6/MHCInc/MHCInc/caterpillar.py` & `mhcinc-0.2.7/MHCInc/MHCInc/caterpillar.py`

 * *Files identical despite different names*

### Comparing `mhcinc-0.2.6/MHCInc/MHCInc/caterpillar2.py` & `mhcinc-0.2.7/MHCInc/MHCInc/caterpillar2.py`

 * *Files identical despite different names*

### Comparing `mhcinc-0.2.6/MHCInc/MHCInc/copyright.py` & `mhcinc-0.2.7/MHCInc/MHCInc/copyright.py`

 * *Files identical despite different names*

### Comparing `mhcinc-0.2.6/MHCInc/MHCInc/egg_catcher.py` & `mhcinc-0.2.7/MHCInc/MHCInc/egg_catcher.py`

 * *Files identical despite different names*

### Comparing `mhcinc-0.2.6/MHCInc/MHCInc/egg_catcher_perfect.py` & `mhcinc-0.2.7/MHCInc/MHCInc/egg_catcher_perfect.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from itertools import cycle
 from random import randrange
 from tkinter import Canvas,Tk,messagebox,font,PhotoImage
 from pygame import mixer
 import time
+import os
 
 mixer.init()
 
 beep=mixer.Sound(os.path.abspath('MHCInc/200bpm%E6%AD%BB%E4%BA%A1%E4%B9%8B%E6%9B%B2 2.flac'))
 beep.play()
 time.sleep(5)
```

### Comparing `mhcinc-0.2.6/MHCInc/MHCInc/matchmaker.py` & `mhcinc-0.2.7/MHCInc/MHCInc/matchmaker.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import random
 import time
 from tkinter import Tk,Button,DISABLED,messagebox
 from pygame import mixer
+import os
 
 mixer.init()
 beep=mixer.Sound(os.path.abspath('MHCInc/200bpm%E6%AD%BB%E4%BA%A1%E4%B9%8B%E6%9B%B2 2.flac'))
 beep.play()
 time.sleep(5)
 
 def show_symbol(x,y):
```

### Comparing `mhcinc-0.2.6/MHCInc/MHCInc/random.py` & `mhcinc-0.2.7/MHCInc/MHCInc/random.py`

 * *Files identical despite different names*

### Comparing `mhcinc-0.2.6/MHCInc/MHCInc/rectangle.py` & `mhcinc-0.2.7/MHCInc/MHCInc/rectangle.py`

 * *Files identical despite different names*

### Comparing `mhcinc-0.2.6/MHCInc/MHCInc/robot_builder.py` & `mhcinc-0.2.7/MHCInc/MHCInc/robot_builder.py`

 * *Files identical despite different names*

### Comparing `mhcinc-0.2.6/MHCInc/MHCInc/screen_pet.py` & `mhcinc-0.2.7/MHCInc/MHCInc/screen_pet.py`

 * *Files identical despite different names*

### Comparing `mhcinc-0.2.6/MHCInc/MHCInc/swift.py` & `mhcinc-0.2.7/MHCInc/MHCInc/swift.py`

 * *Files identical despite different names*

### Comparing `mhcinc-0.2.6/MHCInc/MHCInc/加密消息.py` & `mhcinc-0.2.7/MHCInc/MHCInc/加密消息.py`

 * *Files identical despite different names*

### Comparing `mhcinc-0.2.6/MHCInc/MHCInc/单词九连猜.py` & `mhcinc-0.2.7/MHCInc/MHCInc/单词九连猜.py`

 * *Files identical despite different names*

### Comparing `mhcinc-0.2.6/MHCInc/MHCInc/快照抓拍.py` & `mhcinc-0.2.7/MHCInc/MHCInc/快照抓拍.py`

 * *Files identical despite different names*

### Comparing `mhcinc-0.2.6/MHCInc/MHCInc/星光夜空.py` & `mhcinc-0.2.7/MHCInc/MHCInc/星光夜空.py`

 * *Files identical despite different names*

### Comparing `mhcinc-0.2.6/MHCInc/MHCInc/螺旋万花筒.py` & `mhcinc-0.2.7/MHCInc/MHCInc/螺旋万花筒.py`

 * *Files identical despite different names*

### Comparing `mhcinc-0.2.6/MHCInc/MHCInc.egg-info/PKG-INFO` & `mhcinc-0.2.7/MHCInc/MHCInc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MHCInc
-Version: 0.2.6
+Version: 0.2.7
 Summary: 改进漏洞：将使用模块功能时找不到文件优化
 Home-page: https://pypi.org/project/MHCInc/
 Author: Mhc-inc
 Author-email: Wf6350177@163.com
 Project-URL: Bug Tracker, https://github.com/Mhc-inc/MHCInc/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mhcinc-0.2.6/MHCInc/MHCInc.egg-info/SOURCES.txt` & `mhcinc-0.2.7/MHCInc/MHCInc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mhcinc-0.2.6/PKG-INFO` & `mhcinc-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MHCInc
-Version: 0.2.6
+Version: 0.2.7
 Summary: 改进漏洞：将使用模块功能时找不到文件优化
 Home-page: https://pypi.org/project/MHCInc/
 Author: Mhc-inc
 Author-email: Wf6350177@163.com
 Project-URL: Bug Tracker, https://github.com/Mhc-inc/MHCInc/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mhcinc-0.2.6/README.md` & `mhcinc-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `mhcinc-0.2.6/setup.py` & `mhcinc-0.2.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r",encoding = "UTF-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="MHCInc",
-    version="0.2.6",
+    version="0.2.7",
     author="Mhc-inc",
     author_email="Wf6350177@163.com",
     description="改进漏洞：将使用模块功能时找不到文件优化",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://pypi.org/project/MHCInc/",
     project_urls={
```

