# Comparing `tmp/magictk-1.0.1.60.tar.gz` & `tmp/magictk-1.0.1.61.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magictk-1.0.1.60.tar", last modified: Tue Apr 30 13:33:29 2024, max compression
+gzip compressed data, was "magictk-1.0.1.61.tar", last modified: Wed May  1 03:09:42 2024, max compression
```

## Comparing `magictk-1.0.1.60.tar` & `magictk-1.0.1.61.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 13:33:29.811309 magictk-1.0.1.60/
--rw-r--r--   0 root         (0) root         (0)       47 2024-04-30 13:33:29.000000 magictk-1.0.1.60/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      597 2024-04-30 13:33:29.807309 magictk-1.0.1.60/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1683 2024-04-30 13:33:29.000000 magictk-1.0.1.60/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 13:33:29.807309 magictk-1.0.1.60/magictk/
--rw-r--r--   0 root         (0) root         (0)      514 2024-04-30 13:33:29.000000 magictk-1.0.1.60/magictk/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9695 2024-04-30 13:33:29.000000 magictk-1.0.1.60/magictk/_window_ctl.py
--rw-r--r--   0 root         (0) root         (0)    13250 2024-04-30 13:33:29.000000 magictk-1.0.1.60/magictk/_window_size.py
--rw-r--r--   0 root         (0) root         (0)     3363 2024-04-30 13:33:29.000000 magictk-1.0.1.60/magictk/basicwindow.py
--rw-r--r--   0 root         (0) root         (0)    17577 2024-04-30 13:33:29.000000 magictk-1.0.1.60/magictk/button.py
--rw-r--r--   0 root         (0) root         (0)    11247 2024-04-30 13:33:29.000000 magictk-1.0.1.60/magictk/checkbox.py
--rw-r--r--   0 root         (0) root         (0)     2069 2024-04-30 13:33:29.000000 magictk-1.0.1.60/magictk/color_tmpl.py
--rw-r--r--   0 root         (0) root         (0)    12242 2024-04-30 13:33:29.000000 magictk-1.0.1.60/magictk/entry.py
--rw-r--r--   0 root         (0) root         (0)      578 2024-04-30 13:33:29.000000 magictk-1.0.1.60/magictk/fontconfig.py
--rw-r--r--   0 root         (0) root         (0)     3725 2024-04-30 13:33:29.000000 magictk-1.0.1.60/magictk/frame.py
--rw-r--r--   0 root         (0) root         (0)    15906 2024-04-30 13:33:29.000000 magictk-1.0.1.60/magictk/icon.ico
--rw-r--r--   0 root         (0) root         (0)     1890 2024-04-30 13:33:29.000000 magictk-1.0.1.60/magictk/icon.py
--rw-r--r--   0 root         (0) root         (0)       70 2024-04-30 13:33:29.000000 magictk-1.0.1.60/magictk/mtk.py
--rw-r--r--   0 root         (0) root         (0)      720 2024-04-30 13:33:29.000000 magictk-1.0.1.60/magictk/photoload.py
--rw-r--r--   0 root         (0) root         (0)     5995 2024-04-30 13:33:29.000000 magictk-1.0.1.60/magictk/progressbar.py
--rw-r--r--   0 root         (0) root         (0) 11073665 2024-04-30 13:33:29.000000 magictk-1.0.1.60/magictk/res.pickle
--rw-r--r--   0 root         (0) root         (0)     8106 2024-04-30 13:33:29.000000 magictk-1.0.1.60/magictk/scrollbar.py
--rw-r--r--   0 root         (0) root         (0)     6178 2024-04-30 13:33:29.000000 magictk-1.0.1.60/magictk/select.py
--rw-r--r--   0 root         (0) root         (0)      372 2024-04-30 13:33:29.000000 magictk-1.0.1.60/magictk/style.py
--rw-r--r--   0 root         (0) root         (0)    11076 2024-04-30 13:33:29.000000 magictk-1.0.1.60/magictk/submenu.py
--rw-r--r--   0 root         (0) root         (0)    10245 2024-04-30 13:33:29.000000 magictk-1.0.1.60/magictk/window.py
--rw-r--r--   0 root         (0) root         (0)     2647 2024-04-30 13:33:29.000000 magictk-1.0.1.60/magictk/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 13:33:29.807309 magictk-1.0.1.60/magictk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      597 2024-04-30 13:33:29.000000 magictk-1.0.1.60/magictk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      629 2024-04-30 13:33:29.000000 magictk-1.0.1.60/magictk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 13:33:29.000000 magictk-1.0.1.60/magictk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-30 13:33:29.000000 magictk-1.0.1.60/magictk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-30 13:33:29.811309 magictk-1.0.1.60/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1130 2024-04-30 13:33:29.000000 magictk-1.0.1.60/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 03:09:42.021014 magictk-1.0.1.61/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-05-01 03:09:41.000000 magictk-1.0.1.61/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      597 2024-05-01 03:09:42.021014 magictk-1.0.1.61/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1683 2024-05-01 03:09:41.000000 magictk-1.0.1.61/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 03:09:42.021014 magictk-1.0.1.61/magictk/
+-rw-r--r--   0 root         (0) root         (0)      514 2024-05-01 03:09:41.000000 magictk-1.0.1.61/magictk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9695 2024-05-01 03:09:41.000000 magictk-1.0.1.61/magictk/_window_ctl.py
+-rw-r--r--   0 root         (0) root         (0)    13250 2024-05-01 03:09:41.000000 magictk-1.0.1.61/magictk/_window_size.py
+-rw-r--r--   0 root         (0) root         (0)     3363 2024-05-01 03:09:41.000000 magictk-1.0.1.61/magictk/basicwindow.py
+-rw-r--r--   0 root         (0) root         (0)    17861 2024-05-01 03:09:41.000000 magictk-1.0.1.61/magictk/button.py
+-rw-r--r--   0 root         (0) root         (0)    11247 2024-05-01 03:09:41.000000 magictk-1.0.1.61/magictk/checkbox.py
+-rw-r--r--   0 root         (0) root         (0)     2069 2024-05-01 03:09:41.000000 magictk-1.0.1.61/magictk/color_tmpl.py
+-rw-r--r--   0 root         (0) root         (0)    12242 2024-05-01 03:09:41.000000 magictk-1.0.1.61/magictk/entry.py
+-rw-r--r--   0 root         (0) root         (0)      578 2024-05-01 03:09:41.000000 magictk-1.0.1.61/magictk/fontconfig.py
+-rw-r--r--   0 root         (0) root         (0)     3725 2024-05-01 03:09:41.000000 magictk-1.0.1.61/magictk/frame.py
+-rw-r--r--   0 root         (0) root         (0)    15906 2024-05-01 03:09:41.000000 magictk-1.0.1.61/magictk/icon.ico
+-rw-r--r--   0 root         (0) root         (0)     1890 2024-05-01 03:09:41.000000 magictk-1.0.1.61/magictk/icon.py
+-rw-r--r--   0 root         (0) root         (0)       70 2024-05-01 03:09:41.000000 magictk-1.0.1.61/magictk/mtk.py
+-rw-r--r--   0 root         (0) root         (0)      720 2024-05-01 03:09:41.000000 magictk-1.0.1.61/magictk/photoload.py
+-rw-r--r--   0 root         (0) root         (0)     5995 2024-05-01 03:09:41.000000 magictk-1.0.1.61/magictk/progressbar.py
+-rw-r--r--   0 root         (0) root         (0) 11073665 2024-05-01 03:09:41.000000 magictk-1.0.1.61/magictk/res.pickle
+-rw-r--r--   0 root         (0) root         (0)     8106 2024-05-01 03:09:41.000000 magictk-1.0.1.61/magictk/scrollbar.py
+-rw-r--r--   0 root         (0) root         (0)     6396 2024-05-01 03:09:41.000000 magictk-1.0.1.61/magictk/select.py
+-rw-r--r--   0 root         (0) root         (0)      372 2024-05-01 03:09:41.000000 magictk-1.0.1.61/magictk/style.py
+-rw-r--r--   0 root         (0) root         (0)    11076 2024-05-01 03:09:41.000000 magictk-1.0.1.61/magictk/submenu.py
+-rw-r--r--   0 root         (0) root         (0)    10245 2024-05-01 03:09:41.000000 magictk-1.0.1.61/magictk/window.py
+-rw-r--r--   0 root         (0) root         (0)     2647 2024-05-01 03:09:41.000000 magictk-1.0.1.61/magictk/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 03:09:42.021014 magictk-1.0.1.61/magictk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      597 2024-05-01 03:09:41.000000 magictk-1.0.1.61/magictk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      629 2024-05-01 03:09:41.000000 magictk-1.0.1.61/magictk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-01 03:09:41.000000 magictk-1.0.1.61/magictk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-01 03:09:41.000000 magictk-1.0.1.61/magictk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-01 03:09:42.021014 magictk-1.0.1.61/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1130 2024-05-01 03:09:41.000000 magictk-1.0.1.61/setup.py
```

### Comparing `magictk-1.0.1.60/PKG-INFO` & `magictk-1.0.1.61/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: magictk
-Version: 1.0.1.60
+Version: 1.0.1.61
 Summary: Some tkinter weights look like element-plus
 Home-page: http://git.hmtsai.cn/cxykevin/magictk.git
 Author: cxykevin|git.hmtsai.cn
 Author-email: cxykevin@yeah.net
 License: GPLv2
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `magictk-1.0.1.60/README.md` & `magictk-1.0.1.61/README.md`

 * *Files identical despite different names*

### Comparing `magictk-1.0.1.60/magictk/__init__.py` & `magictk-1.0.1.61/magictk/__init__.py`

 * *Files identical despite different names*

### Comparing `magictk-1.0.1.60/magictk/_window_ctl.py` & `magictk-1.0.1.61/magictk/_window_ctl.py`

 * *Files identical despite different names*

### Comparing `magictk-1.0.1.60/magictk/_window_size.py` & `magictk-1.0.1.61/magictk/_window_size.py`

 * *Files identical despite different names*

### Comparing `magictk-1.0.1.60/magictk/basicwindow.py` & `magictk-1.0.1.61/magictk/basicwindow.py`

 * *Files identical despite different names*

### Comparing `magictk-1.0.1.60/magictk/button.py` & `magictk-1.0.1.61/magictk/button.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,14 +162,23 @@
 
     def grid(self, *args, **kwargs):
         self.canvas.grid(*args, **kwargs)
 
     def place(self, *args, **kwargs):
         self.canvas.place(*args, **kwargs)
 
+    def pack_forget(self, *args, **kwargs):
+        self.canvas.pack_forget(*args, **kwargs)
+
+    def grid_forget(self, *args, **kwargs):
+        self.canvas.grid_forget(*args, **kwargs)
+
+    def place_forget(self, *args, **kwargs):
+        self.canvas.place_forget(*args, **kwargs)
+
     def _draw(self, _use_self_text=None):
         self._draw_corner(0, 0, 0, 0)
         self._draw_corner(1, 0, self.w-4, 0)
         self._draw_corner(0, 1, 0, self.h-5)
         self._draw_corner(1, 1, self.w-4, self.h-5)
 
         def update_color(obj, g_color, f_color, h_color):
```

### Comparing `magictk-1.0.1.60/magictk/checkbox.py` & `magictk-1.0.1.61/magictk/checkbox.py`

 * *Files identical despite different names*

### Comparing `magictk-1.0.1.60/magictk/color_tmpl.py` & `magictk-1.0.1.61/magictk/color_tmpl.py`

 * *Files identical despite different names*

### Comparing `magictk-1.0.1.60/magictk/entry.py` & `magictk-1.0.1.61/magictk/entry.py`

 * *Files identical despite different names*

### Comparing `magictk-1.0.1.60/magictk/fontconfig.py` & `magictk-1.0.1.61/magictk/fontconfig.py`

 * *Files identical despite different names*

### Comparing `magictk-1.0.1.60/magictk/frame.py` & `magictk-1.0.1.61/magictk/frame.py`

 * *Files identical despite different names*

### Comparing `magictk-1.0.1.60/magictk/icon.ico` & `magictk-1.0.1.61/magictk/icon.ico`

 * *Files identical despite different names*

### Comparing `magictk-1.0.1.60/magictk/icon.py` & `magictk-1.0.1.61/magictk/icon.py`

 * *Files identical despite different names*

### Comparing `magictk-1.0.1.60/magictk/photoload.py` & `magictk-1.0.1.61/magictk/photoload.py`

 * *Files identical despite different names*

### Comparing `magictk-1.0.1.60/magictk/progressbar.py` & `magictk-1.0.1.61/magictk/progressbar.py`

 * *Files identical despite different names*

### Comparing `magictk-1.0.1.60/magictk/res.pickle` & `magictk-1.0.1.61/magictk/res.pickle`

 * *Files identical despite different names*

### Comparing `magictk-1.0.1.60/magictk/scrollbar.py` & `magictk-1.0.1.61/magictk/scrollbar.py`

 * *Files identical despite different names*

### Comparing `magictk-1.0.1.60/magictk/select.py` & `magictk-1.0.1.61/magictk/select.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,14 +64,21 @@
         self.__last = 0
         for i in self.items:
             self.__menuobj.addmenu(i, self._callback_menu)
 
         for event, eventfunc in master.p_event_list:
             self.canvas.bind(event, eventfunc)
 
+    def change_menu(self, items):
+        self.items = items
+        self.__menuobj = submenu.MenuObjs()
+        self.__last = 0
+        for i in self.items:
+            self.__menuobj.addmenu(i, self._callback_menu)
+
     def _draw(self):
         super()._draw(True)
 
         def update_color(obj, g_color, f_color, h_color):
             if (self._is_hover == 2):
                 self.canvas.itemconfig(
                     obj, fill=h_color)
```

### Comparing `magictk-1.0.1.60/magictk/submenu.py` & `magictk-1.0.1.61/magictk/submenu.py`

 * *Files identical despite different names*

### Comparing `magictk-1.0.1.60/magictk/window.py` & `magictk-1.0.1.61/magictk/window.py`

 * *Files identical despite different names*

### Comparing `magictk-1.0.1.60/magictk/workspace.py` & `magictk-1.0.1.61/magictk/workspace.py`

 * *Files identical despite different names*

### Comparing `magictk-1.0.1.60/magictk.egg-info/PKG-INFO` & `magictk-1.0.1.61/magictk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: magictk
-Version: 1.0.1.60
+Version: 1.0.1.61
 Summary: Some tkinter weights look like element-plus
 Home-page: http://git.hmtsai.cn/cxykevin/magictk.git
 Author: cxykevin|git.hmtsai.cn
 Author-email: cxykevin@yeah.net
 License: GPLv2
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `magictk-1.0.1.60/magictk.egg-info/SOURCES.txt` & `magictk-1.0.1.61/magictk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `magictk-1.0.1.60/setup.py` & `magictk-1.0.1.61/setup.py`

 * *Files identical despite different names*

