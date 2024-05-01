# Comparing `tmp/deadpad-0.2.1.tar.gz` & `tmp/deadpad-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deadpad-0.2.1.tar", last modified: Wed May  1 05:21:02 2024, max compression
+gzip compressed data, was "deadpad-0.2.2.tar", last modified: Wed May  1 05:29:37 2024, max compression
```

## Comparing `deadpad-0.2.1.tar` & `deadpad-0.2.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 05:21:02.394461 deadpad-0.2.1/
--rw-rw-rw-   0        0        0     1070 2024-04-28 02:53:30.000000 deadpad-0.2.1/LICENSE
--rw-rw-rw-   0        0        0      861 2024-05-01 05:21:02.393466 deadpad-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      280 2024-04-29 00:26:13.000000 deadpad-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-01 05:21:02.371996 deadpad-0.2.1/deadpad/
--rw-rw-rw-   0        0        0     6969 2024-05-01 05:16:41.000000 deadpad-0.2.1/deadpad/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 05:21:02.366987 deadpad-0.2.1/deadpad/extensions/
-drwxrwxrwx   0        0        0        0 2024-05-01 05:21:02.376995 deadpad-0.2.1/deadpad/extensions/python/
--rw-rw-rw-   0        0        0    13920 2024-05-01 05:10:08.000000 deadpad-0.2.1/deadpad/extensions/python/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 05:21:02.383995 deadpad-0.2.1/deadpad/parts/
--rw-rw-rw-   0        0        0        0 2024-04-28 08:06:59.000000 deadpad-0.2.1/deadpad/parts/__init__.py
--rw-rw-rw-   0        0        0     7219 2024-05-01 05:18:16.000000 deadpad-0.2.1/deadpad/parts/document.py
--rw-rw-rw-   0        0        0      591 2024-04-30 04:42:56.000000 deadpad-0.2.1/deadpad/parts/extension.py
--rw-rw-rw-   0        0        0      933 2024-04-28 08:18:12.000000 deadpad-0.2.1/deadpad/parts/input_handler.py
--rw-rw-rw-   0        0        0      570 2024-04-29 00:26:06.000000 deadpad-0.2.1/deadpad/parts/keys.py
--rw-rw-rw-   0        0        0     1052 2024-04-28 08:15:11.000000 deadpad-0.2.1/deadpad/parts/linux_input.py
--rw-rw-rw-   0        0        0    10742 2024-05-01 05:17:26.000000 deadpad-0.2.1/deadpad/parts/textscreen.py
--rw-rw-rw-   0        0        0      700 2024-04-27 21:52:30.000000 deadpad-0.2.1/deadpad/parts/themes.py
--rw-rw-rw-   0        0        0      947 2024-04-28 08:12:42.000000 deadpad-0.2.1/deadpad/parts/windows_input.py
-drwxrwxrwx   0        0        0        0 2024-05-01 05:21:02.383995 deadpad-0.2.1/deadpad/themes/
--rw-rw-rw-   0        0        0     1798 2024-05-01 05:14:53.000000 deadpad-0.2.1/deadpad/themes/default.json
-drwxrwxrwx   0        0        0        0 2024-05-01 05:21:02.392464 deadpad-0.2.1/deadpad.egg-info/
--rw-rw-rw-   0        0        0      861 2024-05-01 05:21:02.000000 deadpad-0.2.1/deadpad.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      562 2024-05-01 05:21:02.000000 deadpad-0.2.1/deadpad.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 05:21:02.000000 deadpad-0.2.1/deadpad.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2024-05-01 05:21:02.000000 deadpad-0.2.1/deadpad.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       21 2024-05-01 05:21:02.000000 deadpad-0.2.1/deadpad.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-01 05:21:02.389459 deadpad-0.2.1/preview/
--rw-rw-rw-   0        0        0  1655531 2024-04-27 07:05:58.000000 deadpad-0.2.1/preview/DeadPad1.gif
--rw-rw-rw-   0        0        0  1224693 2024-04-28 03:41:41.000000 deadpad-0.2.1/preview/deadpad2.gif
--rw-rw-rw-   0        0        0      838 2024-05-01 05:20:51.000000 deadpad-0.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-01 05:21:02.394461 deadpad-0.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-01 05:29:37.322091 deadpad-0.2.2/
+-rw-rw-rw-   0        0        0     1070 2024-04-28 02:53:30.000000 deadpad-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0      861 2024-05-01 05:29:37.321091 deadpad-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2024-04-29 00:26:13.000000 deadpad-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-01 05:29:37.301088 deadpad-0.2.2/deadpad/
+-rw-rw-rw-   0        0        0     6969 2024-05-01 05:16:41.000000 deadpad-0.2.2/deadpad/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 05:29:37.297094 deadpad-0.2.2/deadpad/extensions/
+drwxrwxrwx   0        0        0        0 2024-05-01 05:29:37.307093 deadpad-0.2.2/deadpad/extensions/python/
+-rw-rw-rw-   0        0        0    13920 2024-05-01 05:10:08.000000 deadpad-0.2.2/deadpad/extensions/python/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 05:29:37.314089 deadpad-0.2.2/deadpad/parts/
+-rw-rw-rw-   0        0        0        0 2024-04-28 08:06:59.000000 deadpad-0.2.2/deadpad/parts/__init__.py
+-rw-rw-rw-   0        0        0     7304 2024-05-01 05:27:58.000000 deadpad-0.2.2/deadpad/parts/document.py
+-rw-rw-rw-   0        0        0      591 2024-04-30 04:42:56.000000 deadpad-0.2.2/deadpad/parts/extension.py
+-rw-rw-rw-   0        0        0      933 2024-04-28 08:18:12.000000 deadpad-0.2.2/deadpad/parts/input_handler.py
+-rw-rw-rw-   0        0        0      570 2024-04-29 00:26:06.000000 deadpad-0.2.2/deadpad/parts/keys.py
+-rw-rw-rw-   0        0        0     1052 2024-04-28 08:15:11.000000 deadpad-0.2.2/deadpad/parts/linux_input.py
+-rw-rw-rw-   0        0        0    10742 2024-05-01 05:17:26.000000 deadpad-0.2.2/deadpad/parts/textscreen.py
+-rw-rw-rw-   0        0        0      700 2024-04-27 21:52:30.000000 deadpad-0.2.2/deadpad/parts/themes.py
+-rw-rw-rw-   0        0        0      947 2024-04-28 08:12:42.000000 deadpad-0.2.2/deadpad/parts/windows_input.py
+drwxrwxrwx   0        0        0        0 2024-05-01 05:29:37.315090 deadpad-0.2.2/deadpad/themes/
+-rw-rw-rw-   0        0        0     1798 2024-05-01 05:14:53.000000 deadpad-0.2.2/deadpad/themes/default.json
+drwxrwxrwx   0        0        0        0 2024-05-01 05:29:37.320090 deadpad-0.2.2/deadpad.egg-info/
+-rw-rw-rw-   0        0        0      861 2024-05-01 05:29:37.000000 deadpad-0.2.2/deadpad.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      562 2024-05-01 05:29:37.000000 deadpad-0.2.2/deadpad.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 05:29:37.000000 deadpad-0.2.2/deadpad.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-05-01 05:29:37.000000 deadpad-0.2.2/deadpad.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       21 2024-05-01 05:29:37.000000 deadpad-0.2.2/deadpad.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-01 05:29:37.318090 deadpad-0.2.2/preview/
+-rw-rw-rw-   0        0        0  1655531 2024-04-27 07:05:58.000000 deadpad-0.2.2/preview/DeadPad1.gif
+-rw-rw-rw-   0        0        0  1224693 2024-04-28 03:41:41.000000 deadpad-0.2.2/preview/deadpad2.gif
+-rw-rw-rw-   0        0        0      838 2024-05-01 05:29:29.000000 deadpad-0.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-01 05:29:37.322091 deadpad-0.2.2/setup.cfg
```

### Comparing `deadpad-0.2.1/LICENSE` & `deadpad-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `deadpad-0.2.1/PKG-INFO` & `deadpad-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deadpad
-Version: 0.2.1
+Version: 0.2.2
 Summary: A customizeable lightweight CLI/TUI text editor made without curses or any TUI framework.
 Author: William L.
 Project-URL: Homepage, https://github.com/FrewtyPebbles/DeadPad-CLI-Text-Editor
 Project-URL: Issues, https://github.com/FrewtyPebbles/DeadPad-CLI-Text-Editor/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `deadpad-0.2.1/deadpad/__init__.py` & `deadpad-0.2.2/deadpad/__init__.py`

 * *Files identical despite different names*

### Comparing `deadpad-0.2.1/deadpad/extensions/python/__init__.py` & `deadpad-0.2.2/deadpad/extensions/python/__init__.py`

 * *Files identical despite different names*

### Comparing `deadpad-0.2.1/deadpad/parts/document.py` & `deadpad-0.2.2/deadpad/parts/document.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,18 @@
         self.file_path = file_path
         self.state:list[str] = [""]
         self.cursor = CursorPosition(0,0,self)
         self._recording_arrow = False
         self.render_width = render_width - 2
         self.file = open(self.file_path, "r+", encoding="utf8")
         t_str_state = self.file.read()
-        self.str_state = t_str_state if t_str_state[-1] == "\n" else t_str_state + "\n"
+        if t_str_state == "":
+            self.str_state = "\n"
+        else:
+            self.str_state = t_str_state if t_str_state[-1] == "\n" else t_str_state + "\n"
         self.state = newline_chunkstring(self.str_state, self.render_width)
         self.master = master
         self.updated = True
 
 
     def __del__(self):
         self.file.close()
```

### Comparing `deadpad-0.2.1/deadpad/parts/extension.py` & `deadpad-0.2.2/deadpad/parts/extension.py`

 * *Files identical despite different names*

### Comparing `deadpad-0.2.1/deadpad/parts/input_handler.py` & `deadpad-0.2.2/deadpad/parts/input_handler.py`

 * *Files identical despite different names*

### Comparing `deadpad-0.2.1/deadpad/parts/keys.py` & `deadpad-0.2.2/deadpad/parts/keys.py`

 * *Files identical despite different names*

### Comparing `deadpad-0.2.1/deadpad/parts/linux_input.py` & `deadpad-0.2.2/deadpad/parts/linux_input.py`

 * *Files identical despite different names*

### Comparing `deadpad-0.2.1/deadpad/parts/textscreen.py` & `deadpad-0.2.2/deadpad/parts/textscreen.py`

 * *Files identical despite different names*

### Comparing `deadpad-0.2.1/deadpad/parts/themes.py` & `deadpad-0.2.2/deadpad/parts/themes.py`

 * *Files identical despite different names*

### Comparing `deadpad-0.2.1/deadpad/parts/windows_input.py` & `deadpad-0.2.2/deadpad/parts/windows_input.py`

 * *Files identical despite different names*

### Comparing `deadpad-0.2.1/deadpad/themes/default.json` & `deadpad-0.2.2/deadpad/themes/default.json`

 * *Files identical despite different names*

### Comparing `deadpad-0.2.1/deadpad.egg-info/PKG-INFO` & `deadpad-0.2.2/deadpad.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deadpad
-Version: 0.2.1
+Version: 0.2.2
 Summary: A customizeable lightweight CLI/TUI text editor made without curses or any TUI framework.
 Author: William L.
 Project-URL: Homepage, https://github.com/FrewtyPebbles/DeadPad-CLI-Text-Editor
 Project-URL: Issues, https://github.com/FrewtyPebbles/DeadPad-CLI-Text-Editor/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `deadpad-0.2.1/deadpad.egg-info/SOURCES.txt` & `deadpad-0.2.2/deadpad.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deadpad-0.2.1/preview/DeadPad1.gif` & `deadpad-0.2.2/preview/DeadPad1.gif`

 * *Files identical despite different names*

### Comparing `deadpad-0.2.1/preview/deadpad2.gif` & `deadpad-0.2.2/preview/deadpad2.gif`

 * *Files identical despite different names*

### Comparing `deadpad-0.2.1/pyproject.toml` & `deadpad-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "deadpad"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
   { name="William L." },
 ]
 description = "A customizeable lightweight CLI/TUI text editor made without curses or any TUI framework."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

