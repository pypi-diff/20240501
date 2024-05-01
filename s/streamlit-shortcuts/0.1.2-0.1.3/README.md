# Comparing `tmp/streamlit-shortcuts-0.1.2.tar.gz` & `tmp/streamlit-shortcuts-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-shortcuts-0.1.2.tar", last modified: Sat Apr 27 21:22:17 2024, max compression
+gzip compressed data, was "streamlit-shortcuts-0.1.3.tar", last modified: Wed May  1 05:57:32 2024, max compression
```

## Comparing `streamlit-shortcuts-0.1.2.tar` & `streamlit-shortcuts-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 adrian     (501) staff       (20)        0 2024-04-27 21:22:17.501723 streamlit-shortcuts-0.1.2/
--rw-r--r--   0 adrian     (501) staff       (20)     1063 2023-11-28 21:52:39.000000 streamlit-shortcuts-0.1.2/LICENSE
--rw-r--r--   0 adrian     (501) staff       (20)     2014 2024-04-27 21:22:17.501504 streamlit-shortcuts-0.1.2/PKG-INFO
--rw-r--r--   0 adrian     (501) staff       (20)     1661 2024-04-27 21:20:50.000000 streamlit-shortcuts-0.1.2/README.md
--rw-r--r--   0 adrian     (501) staff       (20)       38 2024-04-27 21:22:17.501763 streamlit-shortcuts-0.1.2/setup.cfg
--rw-r--r--   0 adrian     (501) staff       (20)      556 2024-04-27 21:22:13.000000 streamlit-shortcuts-0.1.2/setup.py
-drwxr-xr-x   0 adrian     (501) staff       (20)        0 2024-04-27 21:22:17.499984 streamlit-shortcuts-0.1.2/src/
-drwxr-xr-x   0 adrian     (501) staff       (20)        0 2024-04-27 21:22:17.500599 streamlit-shortcuts-0.1.2/src/streamlit_shortcuts/
--rw-r--r--   0 adrian     (501) staff       (20)       65 2024-04-27 21:06:01.000000 streamlit-shortcuts-0.1.2/src/streamlit_shortcuts/__init__.py
--rw-r--r--   0 adrian     (501) staff       (20)     1932 2024-04-27 21:10:49.000000 streamlit-shortcuts-0.1.2/src/streamlit_shortcuts/streamlit_shortcuts.py
-drwxr-xr-x   0 adrian     (501) staff       (20)        0 2024-04-27 21:22:17.501320 streamlit-shortcuts-0.1.2/src/streamlit_shortcuts.egg-info/
--rw-r--r--   0 adrian     (501) staff       (20)     2014 2024-04-27 21:22:17.000000 streamlit-shortcuts-0.1.2/src/streamlit_shortcuts.egg-info/PKG-INFO
--rw-r--r--   0 adrian     (501) staff       (20)      343 2024-04-27 21:22:17.000000 streamlit-shortcuts-0.1.2/src/streamlit_shortcuts.egg-info/SOURCES.txt
--rw-r--r--   0 adrian     (501) staff       (20)        1 2024-04-27 21:22:17.000000 streamlit-shortcuts-0.1.2/src/streamlit_shortcuts.egg-info/dependency_links.txt
--rw-r--r--   0 adrian     (501) staff       (20)       10 2024-04-27 21:22:17.000000 streamlit-shortcuts-0.1.2/src/streamlit_shortcuts.egg-info/requires.txt
--rw-r--r--   0 adrian     (501) staff       (20)       20 2024-04-27 21:22:17.000000 streamlit-shortcuts-0.1.2/src/streamlit_shortcuts.egg-info/top_level.txt
+drwxr-xr-x   0 adrian     (501) staff       (20)        0 2024-05-01 05:57:32.682662 streamlit-shortcuts-0.1.3/
+-rw-r--r--   0 adrian     (501) staff       (20)     1063 2023-11-28 21:52:39.000000 streamlit-shortcuts-0.1.3/LICENSE
+-rw-r--r--   0 adrian     (501) staff       (20)     2040 2024-05-01 05:57:32.682458 streamlit-shortcuts-0.1.3/PKG-INFO
+-rw-r--r--   0 adrian     (501) staff       (20)     1687 2024-05-01 05:54:59.000000 streamlit-shortcuts-0.1.3/README.md
+-rw-r--r--   0 adrian     (501) staff       (20)       38 2024-05-01 05:57:32.682713 streamlit-shortcuts-0.1.3/setup.cfg
+-rw-r--r--   0 adrian     (501) staff       (20)      556 2024-05-01 05:55:15.000000 streamlit-shortcuts-0.1.3/setup.py
+drwxr-xr-x   0 adrian     (501) staff       (20)        0 2024-05-01 05:57:32.680468 streamlit-shortcuts-0.1.3/src/
+drwxr-xr-x   0 adrian     (501) staff       (20)        0 2024-05-01 05:57:32.681328 streamlit-shortcuts-0.1.3/src/streamlit_shortcuts/
+-rw-r--r--   0 adrian     (501) staff       (20)       65 2024-04-27 21:06:01.000000 streamlit-shortcuts-0.1.3/src/streamlit_shortcuts/__init__.py
+-rw-r--r--   0 adrian     (501) staff       (20)     1878 2024-05-01 05:54:59.000000 streamlit-shortcuts-0.1.3/src/streamlit_shortcuts/streamlit_shortcuts.py
+drwxr-xr-x   0 adrian     (501) staff       (20)        0 2024-05-01 05:57:32.682217 streamlit-shortcuts-0.1.3/src/streamlit_shortcuts.egg-info/
+-rw-r--r--   0 adrian     (501) staff       (20)     2040 2024-05-01 05:57:32.000000 streamlit-shortcuts-0.1.3/src/streamlit_shortcuts.egg-info/PKG-INFO
+-rw-r--r--   0 adrian     (501) staff       (20)      343 2024-05-01 05:57:32.000000 streamlit-shortcuts-0.1.3/src/streamlit_shortcuts.egg-info/SOURCES.txt
+-rw-r--r--   0 adrian     (501) staff       (20)        1 2024-05-01 05:57:32.000000 streamlit-shortcuts-0.1.3/src/streamlit_shortcuts.egg-info/dependency_links.txt
+-rw-r--r--   0 adrian     (501) staff       (20)       10 2024-05-01 05:57:32.000000 streamlit-shortcuts-0.1.3/src/streamlit_shortcuts.egg-info/requires.txt
+-rw-r--r--   0 adrian     (501) staff       (20)       20 2024-05-01 05:57:32.000000 streamlit-shortcuts-0.1.3/src/streamlit_shortcuts.egg-info/top_level.txt
```

### Comparing `streamlit-shortcuts-0.1.2/LICENSE` & `streamlit-shortcuts-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-shortcuts-0.1.2/PKG-INFO` & `streamlit-shortcuts-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-shortcuts
-Version: 0.1.2
+Version: 0.1.3
 Summary: Streamlit keyboard shortcuts for your buttons.
 Home-page: https://github.com/adriangalilea/streamlit-shortcuts
 Author: Adrian Galilea Delgado
 Author-email: adriangalilea@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -20,26 +20,26 @@
 ```bash
 pip install streamlit-shortcuts
 ```
 
 ## Example
 
 ⭐ NEW! thanks to @quantum-ernest 
-```
+```python
 import streamlit as st
-from streamlit_shortcuts import button
+import streamlit_shortcuts
 
 def delete_callback():
     st.write("DELETED!")
 
-streamlit_shortcuts.button("delete", on_click=delete_callback, shortcut,="Ctrl+Shift+X")
+streamlit_shortcuts.button("delete", on_click=delete_callback, shortcut="Ctrl+Shift+X")
 ```
 
 🥱 Old 
-```python
+```
 import streamlit as st
 from streamlit_shortcuts import add_keyboard_shortcuts
 
 def delete_callback():
     st.write("DELETED!")
 
 st.button("delete", on_click=delete_callback)
@@ -48,35 +48,38 @@
     'Ctrl+Shift+X': 'delete',
 })
 ```
 
 The 'Ctrl+Shift+X' combination will trigger "Another Button".
 
 ## Keys
-- Modifiers: 'Control', 'Shift', 'Alt', 'Meta' ('Cmd' on Mac or 'Win' on Windows, thanks to @toolittlecakes)  
+- Modifiers: 'Ctrl', 'Shift', 'Alt', 'Meta' ('Cmd' on Mac or 'Win' on Windows, thanks to @toolittlecakes)  
 - Common Keys: 'Enter', 'Escape', 'Space'
 - Arrow Keys: 'ArrowLeft', 'ArrowRight', 'ArrowUp', 'ArrowDown'
 
 Examples of Key Combinations:
-- 'Control+Enter'
+- 'Ctrl+Enter'
 - 'Shift+ArrowUp'
 - 'Alt+Space'
 
 For a complete list of key values, refer to:
 https://developer.mozilla.org/en-US/docs/Web/API/KeyboardEvent/key/Key_Values
 
 
 ## Contributing
 
 Contributions are welcome! If you have suggestions for improvements or bug fixes, please feel free to make a pull request or open an issue.
 
 ## Contributors
 @toolittlecakes - Added 'Meta' modifier
+
 @quantum-ernest - Improved usage ergonomics
 
+@taylor-ennen - Fixed usage `flow` of code
+
 ## Credits
 Solution seen on:
 https://github.com/streamlit/streamlit/issues/1291
 
 https://gist.github.com/brunomsantiago/e0ab366fc0dbc092c1a5946b30caa9a0
 
 @brunomsantiago
```

### Comparing `streamlit-shortcuts-0.1.2/README.md` & `streamlit-shortcuts-0.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -8,26 +8,26 @@
 ```bash
 pip install streamlit-shortcuts
 ```
 
 ## Example
 
 ⭐ NEW! thanks to @quantum-ernest 
-```
+```python
 import streamlit as st
-from streamlit_shortcuts import button
+import streamlit_shortcuts
 
 def delete_callback():
     st.write("DELETED!")
 
-streamlit_shortcuts.button("delete", on_click=delete_callback, shortcut,="Ctrl+Shift+X")
+streamlit_shortcuts.button("delete", on_click=delete_callback, shortcut="Ctrl+Shift+X")
 ```
 
 🥱 Old 
-```python
+```
 import streamlit as st
 from streamlit_shortcuts import add_keyboard_shortcuts
 
 def delete_callback():
     st.write("DELETED!")
 
 st.button("delete", on_click=delete_callback)
@@ -36,35 +36,38 @@
     'Ctrl+Shift+X': 'delete',
 })
 ```
 
 The 'Ctrl+Shift+X' combination will trigger "Another Button".
 
 ## Keys
-- Modifiers: 'Control', 'Shift', 'Alt', 'Meta' ('Cmd' on Mac or 'Win' on Windows, thanks to @toolittlecakes)  
+- Modifiers: 'Ctrl', 'Shift', 'Alt', 'Meta' ('Cmd' on Mac or 'Win' on Windows, thanks to @toolittlecakes)  
 - Common Keys: 'Enter', 'Escape', 'Space'
 - Arrow Keys: 'ArrowLeft', 'ArrowRight', 'ArrowUp', 'ArrowDown'
 
 Examples of Key Combinations:
-- 'Control+Enter'
+- 'Ctrl+Enter'
 - 'Shift+ArrowUp'
 - 'Alt+Space'
 
 For a complete list of key values, refer to:
 https://developer.mozilla.org/en-US/docs/Web/API/KeyboardEvent/key/Key_Values
 
 
 ## Contributing
 
 Contributions are welcome! If you have suggestions for improvements or bug fixes, please feel free to make a pull request or open an issue.
 
 ## Contributors
 @toolittlecakes - Added 'Meta' modifier
+
 @quantum-ernest - Improved usage ergonomics
 
+@taylor-ennen - Fixed usage `flow` of code
+
 ## Credits
 Solution seen on:
 https://github.com/streamlit/streamlit/issues/1291
 
 https://gist.github.com/brunomsantiago/e0ab366fc0dbc092c1a5946b30caa9a0
 
 @brunomsantiago
```

### Comparing `streamlit-shortcuts-0.1.2/setup.py` & `streamlit-shortcuts-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='streamlit-shortcuts',
-    version='0.1.2',
+    version='0.1.3',
     author='Adrian Galilea Delgado',
     author_email='adriangalilea@gmail.com',
     packages=find_packages(where="src"),
     package_dir={"": "src"},
     url='https://github.com/adriangalilea/streamlit-shortcuts',
     license='MIT',
     description='Streamlit keyboard shortcuts for your buttons.',
```

### Comparing `streamlit-shortcuts-0.1.2/src/streamlit_shortcuts/streamlit_shortcuts.py` & `streamlit-shortcuts-0.1.3/src/streamlit_shortcuts/streamlit_shortcuts.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 from typing import Callable
 
 import streamlit.components.v1 as components
 import streamlit as st
 
 
-# TODO bump to v0.1.2 for 'Meta modifier' and 'Usage ergonomics'
-# TODO add keyboard tooltip to button (streamlit-extras)
+# TODO add keyboard hint to button (streamlit-extras)
 # https://arnaudmiribel.github.io/streamlit-extras/extras/keyboard_text/
 
 def add_keyboard_shortcuts(key_combinations: dict[str, str]):
     """
     Add keyboard shortcuts to trigger Streamlit buttons.
 
     Keys:
-    - Modifiers: 'Control', 'Shift', 'Alt'
+    - Modifiers: 'Ctrl', 'Shift', 'Alt'
     - Common Keys: 'Enter', 'Escape', 'Space'
     - Arrow Keys: 'ArrowLeft', 'ArrowRight', 'ArrowUp', 'ArrowDown'
 
     Examples of Key Combinations:
-    - 'Control+Enter'
+    - 'Ctrl+Enter'
     - 'Shift+ArrowUp'
     - 'Alt+Space'
 
     For a complete list of key values, refer to:
     https://developer.mozilla.org/en-US/docs/Web/API/KeyboardEvent/key/Key_Values
 
     Args:
@@ -54,10 +53,11 @@
     });
     </script>
     """
 
     components.html(js_code, height=0, width=0)
 
 
-def button(label: str, shortcut: dict[str, str], on_click: Callable[..., None]):
+def button(label: str, shortcut: str, on_click: Callable[..., None]):
+    shortcut={shortcut: label}
     st.button(label=label, on_click=on_click)
     add_keyboard_shortcuts(shortcut)
```

### Comparing `streamlit-shortcuts-0.1.2/src/streamlit_shortcuts.egg-info/PKG-INFO` & `streamlit-shortcuts-0.1.3/src/streamlit_shortcuts.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-shortcuts
-Version: 0.1.2
+Version: 0.1.3
 Summary: Streamlit keyboard shortcuts for your buttons.
 Home-page: https://github.com/adriangalilea/streamlit-shortcuts
 Author: Adrian Galilea Delgado
 Author-email: adriangalilea@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -20,26 +20,26 @@
 ```bash
 pip install streamlit-shortcuts
 ```
 
 ## Example
 
 ⭐ NEW! thanks to @quantum-ernest 
-```
+```python
 import streamlit as st
-from streamlit_shortcuts import button
+import streamlit_shortcuts
 
 def delete_callback():
     st.write("DELETED!")
 
-streamlit_shortcuts.button("delete", on_click=delete_callback, shortcut,="Ctrl+Shift+X")
+streamlit_shortcuts.button("delete", on_click=delete_callback, shortcut="Ctrl+Shift+X")
 ```
 
 🥱 Old 
-```python
+```
 import streamlit as st
 from streamlit_shortcuts import add_keyboard_shortcuts
 
 def delete_callback():
     st.write("DELETED!")
 
 st.button("delete", on_click=delete_callback)
@@ -48,35 +48,38 @@
     'Ctrl+Shift+X': 'delete',
 })
 ```
 
 The 'Ctrl+Shift+X' combination will trigger "Another Button".
 
 ## Keys
-- Modifiers: 'Control', 'Shift', 'Alt', 'Meta' ('Cmd' on Mac or 'Win' on Windows, thanks to @toolittlecakes)  
+- Modifiers: 'Ctrl', 'Shift', 'Alt', 'Meta' ('Cmd' on Mac or 'Win' on Windows, thanks to @toolittlecakes)  
 - Common Keys: 'Enter', 'Escape', 'Space'
 - Arrow Keys: 'ArrowLeft', 'ArrowRight', 'ArrowUp', 'ArrowDown'
 
 Examples of Key Combinations:
-- 'Control+Enter'
+- 'Ctrl+Enter'
 - 'Shift+ArrowUp'
 - 'Alt+Space'
 
 For a complete list of key values, refer to:
 https://developer.mozilla.org/en-US/docs/Web/API/KeyboardEvent/key/Key_Values
 
 
 ## Contributing
 
 Contributions are welcome! If you have suggestions for improvements or bug fixes, please feel free to make a pull request or open an issue.
 
 ## Contributors
 @toolittlecakes - Added 'Meta' modifier
+
 @quantum-ernest - Improved usage ergonomics
 
+@taylor-ennen - Fixed usage `flow` of code
+
 ## Credits
 Solution seen on:
 https://github.com/streamlit/streamlit/issues/1291
 
 https://gist.github.com/brunomsantiago/e0ab366fc0dbc092c1a5946b30caa9a0
 
 @brunomsantiago
```

