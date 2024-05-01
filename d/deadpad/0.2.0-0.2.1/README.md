# Comparing `tmp/deadpad-0.2.0.tar.gz` & `tmp/deadpad-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deadpad-0.2.0.tar", last modified: Tue Apr 30 06:49:24 2024, max compression
+gzip compressed data, was "deadpad-0.2.1.tar", last modified: Wed May  1 05:21:02 2024, max compression
```

## Comparing `deadpad-0.2.0.tar` & `deadpad-0.2.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 06:49:24.524896 deadpad-0.2.0/
--rw-rw-rw-   0        0        0     1070 2024-04-28 02:53:30.000000 deadpad-0.2.0/LICENSE
--rw-rw-rw-   0        0        0      861 2024-04-30 06:49:24.523899 deadpad-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      280 2024-04-29 00:26:13.000000 deadpad-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-30 06:49:24.502127 deadpad-0.2.0/deadpad/
--rw-rw-rw-   0        0        0     6920 2024-04-30 05:56:30.000000 deadpad-0.2.0/deadpad/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 06:49:24.497126 deadpad-0.2.0/deadpad/extensions/
-drwxrwxrwx   0        0        0        0 2024-04-30 06:49:24.507130 deadpad-0.2.0/deadpad/extensions/python/
--rw-rw-rw-   0        0        0    11064 2024-04-30 06:38:35.000000 deadpad-0.2.0/deadpad/extensions/python/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 06:49:24.515125 deadpad-0.2.0/deadpad/parts/
--rw-rw-rw-   0        0        0        0 2024-04-28 08:06:59.000000 deadpad-0.2.0/deadpad/parts/__init__.py
--rw-rw-rw-   0        0        0     7263 2024-04-30 06:13:50.000000 deadpad-0.2.0/deadpad/parts/document.py
--rw-rw-rw-   0        0        0      591 2024-04-30 04:42:56.000000 deadpad-0.2.0/deadpad/parts/extension.py
--rw-rw-rw-   0        0        0      933 2024-04-28 08:18:12.000000 deadpad-0.2.0/deadpad/parts/input_handler.py
--rw-rw-rw-   0        0        0      570 2024-04-29 00:26:06.000000 deadpad-0.2.0/deadpad/parts/keys.py
--rw-rw-rw-   0        0        0     1052 2024-04-28 08:15:11.000000 deadpad-0.2.0/deadpad/parts/linux_input.py
--rw-rw-rw-   0        0        0    10363 2024-04-30 06:29:28.000000 deadpad-0.2.0/deadpad/parts/textscreen.py
--rw-rw-rw-   0        0        0      700 2024-04-27 21:52:30.000000 deadpad-0.2.0/deadpad/parts/themes.py
--rw-rw-rw-   0        0        0      947 2024-04-28 08:12:42.000000 deadpad-0.2.0/deadpad/parts/windows_input.py
-drwxrwxrwx   0        0        0        0 2024-04-30 06:49:24.516124 deadpad-0.2.0/deadpad/themes/
--rw-rw-rw-   0        0        0      284 2024-04-30 06:08:03.000000 deadpad-0.2.0/deadpad/themes/default.json
-drwxrwxrwx   0        0        0        0 2024-04-30 06:49:24.522897 deadpad-0.2.0/deadpad.egg-info/
--rw-rw-rw-   0        0        0      861 2024-04-30 06:49:24.000000 deadpad-0.2.0/deadpad.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      562 2024-04-30 06:49:24.000000 deadpad-0.2.0/deadpad.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 06:49:24.000000 deadpad-0.2.0/deadpad.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2024-04-30 06:49:24.000000 deadpad-0.2.0/deadpad.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       21 2024-04-30 06:49:24.000000 deadpad-0.2.0/deadpad.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-30 06:49:24.519124 deadpad-0.2.0/preview/
--rw-rw-rw-   0        0        0  1655531 2024-04-27 07:05:58.000000 deadpad-0.2.0/preview/DeadPad1.gif
--rw-rw-rw-   0        0        0  1224693 2024-04-28 03:41:41.000000 deadpad-0.2.0/preview/deadpad2.gif
--rw-rw-rw-   0        0        0      838 2024-04-30 06:49:05.000000 deadpad-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-30 06:49:24.524896 deadpad-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-01 05:21:02.394461 deadpad-0.2.1/
+-rw-rw-rw-   0        0        0     1070 2024-04-28 02:53:30.000000 deadpad-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0      861 2024-05-01 05:21:02.393466 deadpad-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2024-04-29 00:26:13.000000 deadpad-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-01 05:21:02.371996 deadpad-0.2.1/deadpad/
+-rw-rw-rw-   0        0        0     6969 2024-05-01 05:16:41.000000 deadpad-0.2.1/deadpad/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 05:21:02.366987 deadpad-0.2.1/deadpad/extensions/
+drwxrwxrwx   0        0        0        0 2024-05-01 05:21:02.376995 deadpad-0.2.1/deadpad/extensions/python/
+-rw-rw-rw-   0        0        0    13920 2024-05-01 05:10:08.000000 deadpad-0.2.1/deadpad/extensions/python/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 05:21:02.383995 deadpad-0.2.1/deadpad/parts/
+-rw-rw-rw-   0        0        0        0 2024-04-28 08:06:59.000000 deadpad-0.2.1/deadpad/parts/__init__.py
+-rw-rw-rw-   0        0        0     7219 2024-05-01 05:18:16.000000 deadpad-0.2.1/deadpad/parts/document.py
+-rw-rw-rw-   0        0        0      591 2024-04-30 04:42:56.000000 deadpad-0.2.1/deadpad/parts/extension.py
+-rw-rw-rw-   0        0        0      933 2024-04-28 08:18:12.000000 deadpad-0.2.1/deadpad/parts/input_handler.py
+-rw-rw-rw-   0        0        0      570 2024-04-29 00:26:06.000000 deadpad-0.2.1/deadpad/parts/keys.py
+-rw-rw-rw-   0        0        0     1052 2024-04-28 08:15:11.000000 deadpad-0.2.1/deadpad/parts/linux_input.py
+-rw-rw-rw-   0        0        0    10742 2024-05-01 05:17:26.000000 deadpad-0.2.1/deadpad/parts/textscreen.py
+-rw-rw-rw-   0        0        0      700 2024-04-27 21:52:30.000000 deadpad-0.2.1/deadpad/parts/themes.py
+-rw-rw-rw-   0        0        0      947 2024-04-28 08:12:42.000000 deadpad-0.2.1/deadpad/parts/windows_input.py
+drwxrwxrwx   0        0        0        0 2024-05-01 05:21:02.383995 deadpad-0.2.1/deadpad/themes/
+-rw-rw-rw-   0        0        0     1798 2024-05-01 05:14:53.000000 deadpad-0.2.1/deadpad/themes/default.json
+drwxrwxrwx   0        0        0        0 2024-05-01 05:21:02.392464 deadpad-0.2.1/deadpad.egg-info/
+-rw-rw-rw-   0        0        0      861 2024-05-01 05:21:02.000000 deadpad-0.2.1/deadpad.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      562 2024-05-01 05:21:02.000000 deadpad-0.2.1/deadpad.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 05:21:02.000000 deadpad-0.2.1/deadpad.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-05-01 05:21:02.000000 deadpad-0.2.1/deadpad.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       21 2024-05-01 05:21:02.000000 deadpad-0.2.1/deadpad.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-01 05:21:02.389459 deadpad-0.2.1/preview/
+-rw-rw-rw-   0        0        0  1655531 2024-04-27 07:05:58.000000 deadpad-0.2.1/preview/DeadPad1.gif
+-rw-rw-rw-   0        0        0  1224693 2024-04-28 03:41:41.000000 deadpad-0.2.1/preview/deadpad2.gif
+-rw-rw-rw-   0        0        0      838 2024-05-01 05:20:51.000000 deadpad-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-01 05:21:02.394461 deadpad-0.2.1/setup.cfg
```

### Comparing `deadpad-0.2.0/LICENSE` & `deadpad-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deadpad-0.2.0/PKG-INFO` & `deadpad-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deadpad
-Version: 0.2.0
+Version: 0.2.1
 Summary: A customizeable lightweight CLI/TUI text editor made without curses or any TUI framework.
 Author: William L.
 Project-URL: Homepage, https://github.com/FrewtyPebbles/DeadPad-CLI-Text-Editor
 Project-URL: Issues, https://github.com/FrewtyPebbles/DeadPad-CLI-Text-Editor/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `deadpad-0.2.0/deadpad/__init__.py` & `deadpad-0.2.1/deadpad/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,30 +10,32 @@
 import shutil
 from deadpad.parts.document import Document
 try:
     from deadpad.parts.windows_input import InputHandler
 except ModuleNotFoundError:
     from deadpad.parts.linux_input import InputHandler
 
+# TODO make a system for saving the editor config.
+
 opsys = platform.system()
 
 class Editor:
     "The main class for the python based CLI text editor Dead Pad"
     def __init__(self) -> None:
         self.in_handler = InputHandler()
         self.term_size = shutil.get_terminal_size()
         self.themes_path = f"{os.path.dirname(__file__)}/themes/"
         self.settings = {
             # Toggleables
-            "show_paragraphs": False,
+            "show_newlines": False,
             "show_tabs": False,
-            "line_numbers": True,
+            "show_line_numbers": True,
             # General config
             "theme": f"default",
-            "tab_replace": "\t",
+            "tab": "\t",
         }
         self.extensions:dict[str, Extension] = self.get_extensions()
 
         self.screen = TextScreen(self, self.term_size.columns, self.term_size.lines, Document(self, self.term_size.columns, sys.argv[1]))
         
 
     def get_extensions(self):
```

### Comparing `deadpad-0.2.0/deadpad/parts/document.py` & `deadpad-0.2.1/deadpad/parts/document.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import TYPE_CHECKING
 
 from deadpad.parts import keys
 if TYPE_CHECKING:
     from deadpad.parts.textscreen import TextScreen
     from deadpad import Editor
 
-# TODO Make a property for the state that runs all activated extensions on the code before the state is used by the TextScreen
+# TODO Add line class to keep track of line numbers (should have all string functions implemented)
 
 
 def chrweight(char:str):
     match char:
         case "\t":
             return 3
         case None: # equivalent of space in textscreen
@@ -185,16 +185,16 @@
                         self.cursor.x -= line_len
                     else:
                         self.state[self.cursor.y] = self.state[self.cursor.y][:self.cursor.x-1] + self.state[self.cursor.y][self.cursor.x:]
                         self.cursor.x -= 1
                         self.update_state()
                 case b'\t':
                     
-                    self._insert_character(self.master.settings["tab_replace"].encode(), self.cursor.x, self.cursor.y)
-                    self.cursor.x += len(self.master.settings["tab_replace"])
+                    self._insert_character(self.master.settings["tab"].encode(), self.cursor.x, self.cursor.y)
+                    self.cursor.x += len(self.master.settings["tab"])
                     self.update_state()
                 case _:
                     try:
                         
                         key = key.translate(None, escapes)
                         self._insert_character(key, self.cursor.x, self.cursor.y)
                         self.cursor.x += 1
```

### Comparing `deadpad-0.2.0/deadpad/parts/extension.py` & `deadpad-0.2.1/deadpad/parts/extension.py`

 * *Files identical despite different names*

### Comparing `deadpad-0.2.0/deadpad/parts/input_handler.py` & `deadpad-0.2.1/deadpad/parts/input_handler.py`

 * *Files identical despite different names*

### Comparing `deadpad-0.2.0/deadpad/parts/keys.py` & `deadpad-0.2.1/deadpad/parts/keys.py`

 * *Files identical despite different names*

### Comparing `deadpad-0.2.0/deadpad/parts/linux_input.py` & `deadpad-0.2.1/deadpad/parts/linux_input.py`

 * *Files identical despite different names*

### Comparing `deadpad-0.2.0/deadpad/parts/textscreen.py` & `deadpad-0.2.1/deadpad/parts/textscreen.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,14 +83,15 @@
         for extension in self.master.extensions.values():
             if extension.FILE_EXT == file_ext:
                 if extension.parser:
                     self.highlight = extension.parser.highlight
                     
     
     def refresh(self):
+        # TODO: make theme_data an attribute of Editor instead.
         self.theme_data = json.load(f_p:=open(f"{self.master.themes_path}{self.master.settings['theme']}.json", "r", encoding="utf8"))
         f_p.close()
         self.updated = True
 
     @property
     def y_pos(self):
         return self._y_pos
@@ -136,51 +137,59 @@
             # add spaces to rhs of text accounting for tabs
             
             self.state[ln].extend([None for _ in range(self.width - str_weight(self.state[ln]))])
             ln += 1
             
 
         for y, row in enumerate(self.state):
-            if self.master.settings["line_numbers"]:
-
-                screen += f"{get_style(bg=self.theme_data['line_number_bg'])}{(y+self.y_pos+1):^4}{RESET_STYLE}|"
             src_line = ""
             for x, col in enumerate(row):
                 if col != None:
                     if y == self.cursor_y and x == self.cursor_x:
                         if col in {'\n', ' '}:
                             src_line += self.theme_data["cursor_sym"]
                         elif col == '\t':
                             src_line += self.theme_data["cursor_sym"] + self.theme_data["tab_sym"][1:len(self.theme_data["tab_sym"])] if self.master.settings["show_tabs"] else self.theme_data["cursor_sym"] + (' ' * (len(self.theme_data["tab_sym"])-1))
                         else:
                             src_line += self.theme_data["cursor_sym"] + col
                     else:
                         match col:
                             case '\n':
-                                src_line += self.theme_data["paragraph_sym"] if self.master.settings["show_paragraphs"] else ''
+                                src_line += self.theme_data["paragraph_sym"] if self.master.settings["show_newlines"] else ''
 
                             case '\t':
                                 src_line += self.theme_data["tab_sym"] if self.master.settings["show_tabs"] else (' ' * len(self.theme_data["tab_sym"]))
                             case _:
                                 src_line += col
                 elif y == self.cursor_y and x == self.cursor_x:
                     src_line += self.theme_data["cursor_sym"]
-            screen += self.highlight(src_line).replace(" ", " ")
+            screen += src_line
             if col != '\n':
-                screen += f'\n{RESET_STYLE}'
-
-        
+                screen += f'\n'
+    
+        screen = self.highlight(screen).replace(" ", " ")
+        screen = self._render_second_pass(screen)
 
         # command bar
         bchar = self.theme_data['CLI_bar_filler_char']
         footer_bg = bchar * (self.width - len(self.footer_string)-5)
         padding = ' ' if self.footer_string != "" else ''
         
         return f"{screen}\033[K{self.theme_data['emblem']} {bchar}{padding}{self.footer_string}{padding}{footer_bg}\n\033[K{' '*self.width}"
 
+    def _render_second_pass(self, src:str):
+        lines = src.split('\n')
+        lines.pop()
+        ret_screen = ""
+        for l_n, line in enumerate(lines):
+            if self.master.settings["show_line_numbers"]:
+                ret_screen += f"{get_style(bg=self.theme_data['line_number_bg'])}{(l_n+self.y_pos+1):^4}{RESET_STYLE}|"
+            ret_screen += line + '\n'
+        return ret_screen + RESET_STYLE
+
     def handle_key(self, key:bytes):
         if key != None:
             self.updated = True
         if self.edit_mode:
             self.footer_string = self.document.file_path if self.footer_string in {"COMMAND MODE",self.document.file_path} else self.footer_string
             
             match key:
```

### Comparing `deadpad-0.2.0/deadpad/parts/themes.py` & `deadpad-0.2.1/deadpad/parts/themes.py`

 * *Files identical despite different names*

### Comparing `deadpad-0.2.0/deadpad/parts/windows_input.py` & `deadpad-0.2.1/deadpad/parts/windows_input.py`

 * *Files identical despite different names*

### Comparing `deadpad-0.2.0/deadpad.egg-info/PKG-INFO` & `deadpad-0.2.1/deadpad.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deadpad
-Version: 0.2.0
+Version: 0.2.1
 Summary: A customizeable lightweight CLI/TUI text editor made without curses or any TUI framework.
 Author: William L.
 Project-URL: Homepage, https://github.com/FrewtyPebbles/DeadPad-CLI-Text-Editor
 Project-URL: Issues, https://github.com/FrewtyPebbles/DeadPad-CLI-Text-Editor/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `deadpad-0.2.0/deadpad.egg-info/SOURCES.txt` & `deadpad-0.2.1/deadpad.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deadpad-0.2.0/preview/DeadPad1.gif` & `deadpad-0.2.1/preview/DeadPad1.gif`

 * *Files identical despite different names*

### Comparing `deadpad-0.2.0/preview/deadpad2.gif` & `deadpad-0.2.1/preview/deadpad2.gif`

 * *Files identical despite different names*

### Comparing `deadpad-0.2.0/pyproject.toml` & `deadpad-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "deadpad"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="William L." },
 ]
 description = "A customizeable lightweight CLI/TUI text editor made without curses or any TUI framework."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

