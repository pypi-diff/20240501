# Comparing `tmp/rofi_rbw-1.4.0.tar.gz` & `tmp/rofi_rbw-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rofi_rbw-1.4.0.tar", max compression
+gzip compressed data, was "rofi_rbw-1.4.1.tar", max compression
```

## Comparing `rofi_rbw-1.4.0.tar` & `rofi_rbw-1.4.1.tar`

### file list

```diff
@@ -1,52 +1,34 @@
--rw-r--r--   0        0        0     1075 2023-01-03 08:16:30.965044 rofi_rbw-1.4.0/LICENSE
--rw-r--r--   0        0        0     8498 2024-04-19 16:55:25.616396 rofi_rbw-1.4.0/README.md
--rw-r--r--   0        0        0     4530 2024-04-27 13:48:57.528553 rofi_rbw-1.4.0/docs/rofi-rbw.1
--rw-r--r--   0        0        0      748 2024-04-27 13:47:26.175425 rofi_rbw-1.4.0/pyproject.toml
--rw-r--r--   0        0        0      206 2022-12-22 13:31:28.675750 rofi_rbw-1.4.0/src/rofi_rbw/__init__.py
--rw-r--r--   0        0        0      105 2022-12-22 13:31:28.675750 rofi_rbw-1.4.0/src/rofi_rbw/__main__.py
--rw-r--r--   0        0        0      197 2022-12-22 13:31:28.675750 rofi_rbw-1.4.0/src/rofi_rbw/abstractionhelper.py
--rw-r--r--   0        0        0     4890 2024-04-19 16:55:25.616396 rofi_rbw-1.4.0/src/rofi_rbw/argument_parsing.py
--rw-r--r--   0        0        0     1182 2023-12-05 12:35:22.072945 rofi_rbw-1.4.0/src/rofi_rbw/cache.py
--rw-r--r--   0        0        0        0 2024-01-18 18:50:19.810170 rofi_rbw-1.4.0/src/rofi_rbw/clipboarder/__init__.py
--rw-r--r--   0        0        0      169 2024-03-06 08:45:01.276552 rofi_rbw-1.4.0/src/rofi_rbw/clipboarder/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3213 2024-03-06 08:45:01.276552 rofi_rbw-1.4.0/src/rofi_rbw/clipboarder/__pycache__/clipboarder.cpython-311.pyc
--rw-r--r--   0        0        0     1384 2024-03-06 08:45:01.286552 rofi_rbw-1.4.0/src/rofi_rbw/clipboarder/__pycache__/noop.cpython-311.pyc
--rw-r--r--   0        0        0     1815 2024-03-06 08:45:01.286552 rofi_rbw-1.4.0/src/rofi_rbw/clipboarder/__pycache__/wlclip.cpython-311.pyc
--rw-r--r--   0        0        0     2441 2024-04-01 17:27:58.635344 rofi_rbw-1.4.0/src/rofi_rbw/clipboarder/__pycache__/xclip.cpython-311.pyc
--rw-r--r--   0        0        0     2452 2024-03-06 08:45:01.286552 rofi_rbw-1.4.0/src/rofi_rbw/clipboarder/__pycache__/xsel.cpython-311.pyc
--rw-r--r--   0        0        0     1194 2024-01-18 18:50:19.810170 rofi_rbw-1.4.0/src/rofi_rbw/clipboarder/clipboarder.py
--rw-r--r--   0        0        0      440 2024-01-18 18:50:32.079752 rofi_rbw-1.4.0/src/rofi_rbw/clipboarder/noop.py
--rw-r--r--   0        0        0      610 2024-01-18 18:50:37.116248 rofi_rbw-1.4.0/src/rofi_rbw/clipboarder/wlclip.py
--rw-r--r--   0        0        0     1106 2024-03-24 12:11:07.281774 rofi_rbw-1.4.0/src/rofi_rbw/clipboarder/xclip.py
--rw-r--r--   0        0        0     1210 2024-01-18 18:50:37.116248 rofi_rbw-1.4.0/src/rofi_rbw/clipboarder/xsel.py
--rw-r--r--   0        0        0     1592 2024-04-19 16:55:25.616396 rofi_rbw-1.4.0/src/rofi_rbw/credentials.py
--rw-r--r--   0        0        0      516 2023-12-05 12:35:22.072945 rofi_rbw-1.4.0/src/rofi_rbw/entry.py
--rw-r--r--   0        0        0     1473 2024-04-19 16:55:25.616396 rofi_rbw-1.4.0/src/rofi_rbw/models.py
--rw-r--r--   0        0        0      641 2023-12-05 12:35:22.072945 rofi_rbw-1.4.0/src/rofi_rbw/paths.py
--rw-r--r--   0        0        0     2512 2023-12-05 12:41:31.229807 rofi_rbw-1.4.0/src/rofi_rbw/rbw.py
--rwxr-xr-x   0        0        0     4465 2024-04-19 16:55:25.616396 rofi_rbw-1.4.0/src/rofi_rbw/rofi_rbw.py
--rw-r--r--   0        0        0        0 2024-01-18 18:50:19.810170 rofi_rbw-1.4.0/src/rofi_rbw/selector/__init__.py
--rw-r--r--   0        0        0      166 2024-03-06 08:45:01.279885 rofi_rbw-1.4.0/src/rofi_rbw/selector/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     5045 2024-03-06 08:45:01.283219 rofi_rbw-1.4.0/src/rofi_rbw/selector/__pycache__/bemenu.cpython-311.pyc
--rw-r--r--   0        0        0     8086 2024-03-06 08:45:01.283219 rofi_rbw-1.4.0/src/rofi_rbw/selector/__pycache__/rofi.cpython-311.pyc
--rw-r--r--   0        0        0     8762 2024-03-21 18:59:51.620840 rofi_rbw-1.4.0/src/rofi_rbw/selector/__pycache__/selector.cpython-311.pyc
--rw-r--r--   0        0        0     5083 2024-03-06 08:45:01.283219 rofi_rbw-1.4.0/src/rofi_rbw/selector/__pycache__/wofi.cpython-311.pyc
--rw-r--r--   0        0        0     2506 2024-01-18 18:51:27.594529 rofi_rbw-1.4.0/src/rofi_rbw/selector/bemenu.py
--rw-r--r--   0        0        0     4627 2024-01-18 18:50:19.810170 rofi_rbw-1.4.0/src/rofi_rbw/selector/rofi.py
--rw-r--r--   0        0        0     3967 2024-03-21 18:01:21.271335 rofi_rbw-1.4.0/src/rofi_rbw/selector/selector.py
--rw-r--r--   0        0        0     2523 2024-01-18 18:50:19.810170 rofi_rbw-1.4.0/src/rofi_rbw/selector/wofi.py
--rw-r--r--   0        0        0        0 2024-01-18 18:50:19.810170 rofi_rbw-1.4.0/src/rofi_rbw/typer/__init__.py
--rw-r--r--   0        0        0      163 2024-03-06 08:45:01.279885 rofi_rbw-1.4.0/src/rofi_rbw/typer/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2171 2024-04-13 19:26:05.823685 rofi_rbw-1.4.0/src/rofi_rbw/typer/__pycache__/dotool.cpython-311.pyc
--rw-r--r--   0        0        0     1576 2024-04-01 17:27:58.632010 rofi_rbw-1.4.0/src/rofi_rbw/typer/__pycache__/noop.cpython-311.pyc
--rw-r--r--   0        0        0     3672 2024-04-01 17:27:58.628676 rofi_rbw-1.4.0/src/rofi_rbw/typer/__pycache__/typer.cpython-311.pyc
--rw-r--r--   0        0        0     2141 2024-04-01 17:27:58.632010 rofi_rbw-1.4.0/src/rofi_rbw/typer/__pycache__/wtype.cpython-311.pyc
--rw-r--r--   0        0        0     2524 2024-04-01 17:27:58.632010 rofi_rbw-1.4.0/src/rofi_rbw/typer/__pycache__/xdotool.cpython-311.pyc
--rw-r--r--   0        0        0     2262 2024-04-01 17:27:58.632010 rofi_rbw-1.4.0/src/rofi_rbw/typer/__pycache__/ydotool.cpython-311.pyc
--rw-r--r--   0        0        0      838 2024-04-19 16:55:25.616396 rofi_rbw-1.4.0/src/rofi_rbw/typer/dotool.py
--rw-r--r--   0        0        0      502 2024-04-19 16:55:25.616396 rofi_rbw-1.4.0/src/rofi_rbw/typer/noop.py
--rw-r--r--   0        0        0     1313 2024-04-19 16:55:25.616396 rofi_rbw-1.4.0/src/rofi_rbw/typer/typer.py
--rw-r--r--   0        0        0      800 2024-04-19 16:55:25.616396 rofi_rbw-1.4.0/src/rofi_rbw/typer/wtype.py
--rw-r--r--   0        0        0     1286 2024-04-19 16:55:25.619729 rofi_rbw-1.4.0/src/rofi_rbw/typer/xdotool.py
--rw-r--r--   0        0        0      861 2024-04-19 16:55:25.619729 rofi_rbw-1.4.0/src/rofi_rbw/typer/ydotool.py
--rw-r--r--   0        0        0     9240 1970-01-01 00:00:00.000000 rofi_rbw-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-01-03 08:16:30.965044 rofi_rbw-1.4.1/LICENSE
+-rw-r--r--   0        0        0     8619 2024-05-01 07:52:31.725921 rofi_rbw-1.4.1/README.md
+-rw-r--r--   0        0        0     4528 2024-05-01 07:52:07.045951 rofi_rbw-1.4.1/docs/rofi-rbw.1
+-rw-r--r--   0        0        0      748 2024-05-01 07:50:58.462700 rofi_rbw-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0      206 2022-12-22 13:31:28.675750 rofi_rbw-1.4.1/src/rofi_rbw/__init__.py
+-rw-r--r--   0        0        0      105 2022-12-22 13:31:28.675750 rofi_rbw-1.4.1/src/rofi_rbw/__main__.py
+-rw-r--r--   0        0        0      197 2022-12-22 13:31:28.675750 rofi_rbw-1.4.1/src/rofi_rbw/abstractionhelper.py
+-rw-r--r--   0        0        0     4890 2024-04-19 16:55:25.616396 rofi_rbw-1.4.1/src/rofi_rbw/argument_parsing.py
+-rw-r--r--   0        0        0     1182 2023-12-05 12:35:22.072945 rofi_rbw-1.4.1/src/rofi_rbw/cache.py
+-rw-r--r--   0        0        0        0 2024-01-18 18:50:19.810170 rofi_rbw-1.4.1/src/rofi_rbw/clipboarder/__init__.py
+-rw-r--r--   0        0        0     1194 2024-01-18 18:50:19.810170 rofi_rbw-1.4.1/src/rofi_rbw/clipboarder/clipboarder.py
+-rw-r--r--   0        0        0      440 2024-01-18 18:50:32.079752 rofi_rbw-1.4.1/src/rofi_rbw/clipboarder/noop.py
+-rw-r--r--   0        0        0      610 2024-01-18 18:50:37.116248 rofi_rbw-1.4.1/src/rofi_rbw/clipboarder/wlclip.py
+-rw-r--r--   0        0        0     1106 2024-03-24 12:11:07.281774 rofi_rbw-1.4.1/src/rofi_rbw/clipboarder/xclip.py
+-rw-r--r--   0        0        0     1210 2024-01-18 18:50:37.116248 rofi_rbw-1.4.1/src/rofi_rbw/clipboarder/xsel.py
+-rw-r--r--   0        0        0     1592 2024-04-19 16:55:25.616396 rofi_rbw-1.4.1/src/rofi_rbw/credentials.py
+-rw-r--r--   0        0        0      516 2023-12-05 12:35:22.072945 rofi_rbw-1.4.1/src/rofi_rbw/entry.py
+-rw-r--r--   0        0        0     1473 2024-04-19 16:55:25.616396 rofi_rbw-1.4.1/src/rofi_rbw/models.py
+-rw-r--r--   0        0        0      641 2023-12-05 12:35:22.072945 rofi_rbw-1.4.1/src/rofi_rbw/paths.py
+-rw-r--r--   0        0        0     2512 2023-12-05 12:41:31.229807 rofi_rbw-1.4.1/src/rofi_rbw/rbw.py
+-rwxr-xr-x   0        0        0     4442 2024-04-29 18:46:51.932565 rofi_rbw-1.4.1/src/rofi_rbw/rofi_rbw.py
+-rw-r--r--   0        0        0        0 2024-01-18 18:50:19.810170 rofi_rbw-1.4.1/src/rofi_rbw/selector/__init__.py
+-rw-r--r--   0        0        0     2506 2024-01-18 18:51:27.594529 rofi_rbw-1.4.1/src/rofi_rbw/selector/bemenu.py
+-rw-r--r--   0        0        0     4627 2024-01-18 18:50:19.810170 rofi_rbw-1.4.1/src/rofi_rbw/selector/rofi.py
+-rw-r--r--   0        0        0     3967 2024-03-21 18:01:21.271335 rofi_rbw-1.4.1/src/rofi_rbw/selector/selector.py
+-rw-r--r--   0        0        0     2523 2024-01-18 18:50:19.810170 rofi_rbw-1.4.1/src/rofi_rbw/selector/wofi.py
+-rw-r--r--   0        0        0        0 2024-01-18 18:50:19.810170 rofi_rbw-1.4.1/src/rofi_rbw/typer/__init__.py
+-rw-r--r--   0        0        0      838 2024-04-19 16:55:25.616396 rofi_rbw-1.4.1/src/rofi_rbw/typer/dotool.py
+-rw-r--r--   0        0        0      502 2024-04-19 16:55:25.616396 rofi_rbw-1.4.1/src/rofi_rbw/typer/noop.py
+-rw-r--r--   0        0        0     1313 2024-04-19 16:55:25.616396 rofi_rbw-1.4.1/src/rofi_rbw/typer/typer.py
+-rw-r--r--   0        0        0      800 2024-04-19 16:55:25.616396 rofi_rbw-1.4.1/src/rofi_rbw/typer/wtype.py
+-rw-r--r--   0        0        0     1287 2024-04-29 18:46:51.932565 rofi_rbw-1.4.1/src/rofi_rbw/typer/xdotool.py
+-rw-r--r--   0        0        0      861 2024-04-19 16:55:25.619729 rofi_rbw-1.4.1/src/rofi_rbw/typer/ydotool.py
+-rw-r--r--   0        0        0     9361 1970-01-01 00:00:00.000000 rofi_rbw-1.4.1/PKG-INFO
```

### Comparing `rofi_rbw-1.4.0/LICENSE` & `rofi_rbw-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rofi_rbw-1.4.0/README.md` & `rofi_rbw-1.4.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # rbw-rofi
 ## A rofi frontend for Bitwarden
 
 Based on the alternative [Bitwarden](https://bitwarden.com/) CLI [rbw](https://github.com/doy/rbw/) and inspired by [rofi-pass](https://github.com/carnager/rofi-pass), `rbw-rofi` is a simplistic password typer/copier using [rofi](https://github.com/davatorium/rofi) and [wofi](https://hg.sr.ht/~scoopta/wofi).
 
+![Screenshot of rofi-rbw](screenshot.png?raw=true)
+![Screenshot of a rofi-rbw entry menu](screenshot-menu.png?raw=true)
+
 ## Features
 - Autotype password or username (`Enter`/`Alt+3` and `Alt+2`, respectively)
 - Autotype username and password (with a `tab` character in between) with `Alt+1` (and copy TOTP to clipboard)
 - Configure autotyping either as a keybinding or by having a `_autotype` field in your credential
 - Copy username, password or TOTP to the clipboard (`Alt+u`, `Alt+p` and `Alt+t`, respectively)
 - Show an autotype menu with all fields
```

### Comparing `rofi_rbw-1.4.0/docs/rofi-rbw.1` & `rofi_rbw-1.4.1/docs/rofi-rbw.1`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Automatically generated by Pandoc 3.1.12.2
 .\"
-.TH "ROFI\-RBW" "1" "April 27, 2024" "Version 1.4.0" "Rofi Third\-party Add\-on Documentation"
+.TH "ROFI\-RBW" "1" "May 01, 2024" "Version 1.4.1" "Rofi Third\-party Add\-on Documentation"
 .SH NAME
 \f[B]rofi\-rbw\f[R] \- A rofi frontend for the alternative Bitwarden
 client rbw
 .SH SYNOPSIS
 .PP
 \f[B]rofi\-rbw\f[R] [\f[B]\-h\f[R]] [\f[B]\-\-version\f[R]]
 [\f[B]\-\-action\f[R] {\f[I]type\f[R],\f[I]copy\f[R],\f[I]print\f[R]}]
```

### Comparing `rofi_rbw-1.4.0/pyproject.toml` & `rofi_rbw-1.4.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rofi-rbw"
-version = "1.4.0"
+version = "1.4.1"
 description = "Rofi frontend for Bitwarden"
 authors = ["Fabian Winter <5821180+fdw@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/fdw/rofi-rbw"
 repository = "https://github.com/fdw/rofi-rbw"
 packages =[
```

### Comparing `rofi_rbw-1.4.0/src/rofi_rbw/argument_parsing.py` & `rofi_rbw-1.4.1/src/rofi_rbw/argument_parsing.py`

 * *Files identical despite different names*

### Comparing `rofi_rbw-1.4.0/src/rofi_rbw/cache.py` & `rofi_rbw-1.4.1/src/rofi_rbw/cache.py`

 * *Files identical despite different names*

### Comparing `rofi_rbw-1.4.0/src/rofi_rbw/clipboarder/clipboarder.py` & `rofi_rbw-1.4.1/src/rofi_rbw/clipboarder/clipboarder.py`

 * *Files identical despite different names*

### Comparing `rofi_rbw-1.4.0/src/rofi_rbw/clipboarder/wlclip.py` & `rofi_rbw-1.4.1/src/rofi_rbw/clipboarder/wlclip.py`

 * *Files identical despite different names*

### Comparing `rofi_rbw-1.4.0/src/rofi_rbw/clipboarder/xclip.py` & `rofi_rbw-1.4.1/src/rofi_rbw/clipboarder/xclip.py`

 * *Files identical despite different names*

### Comparing `rofi_rbw-1.4.0/src/rofi_rbw/clipboarder/xsel.py` & `rofi_rbw-1.4.1/src/rofi_rbw/clipboarder/xsel.py`

 * *Files identical despite different names*

### Comparing `rofi_rbw-1.4.0/src/rofi_rbw/credentials.py` & `rofi_rbw-1.4.1/src/rofi_rbw/credentials.py`

 * *Files identical despite different names*

### Comparing `rofi_rbw-1.4.0/src/rofi_rbw/entry.py` & `rofi_rbw-1.4.1/src/rofi_rbw/entry.py`

 * *Files identical despite different names*

### Comparing `rofi_rbw-1.4.0/src/rofi_rbw/models.py` & `rofi_rbw-1.4.1/src/rofi_rbw/models.py`

 * *Files identical despite different names*

### Comparing `rofi_rbw-1.4.0/src/rofi_rbw/paths.py` & `rofi_rbw-1.4.1/src/rofi_rbw/paths.py`

 * *Files identical despite different names*

### Comparing `rofi_rbw-1.4.0/src/rofi_rbw/rbw.py` & `rofi_rbw-1.4.1/src/rofi_rbw/rbw.py`

 * *Files identical despite different names*

### Comparing `rofi_rbw-1.4.0/src/rofi_rbw/rofi_rbw.py` & `rofi_rbw-1.4.1/src/rofi_rbw/rofi_rbw.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,14 @@
                 return cred.autotype_sequence
             else:
                 return [Targets.USERNAME, TypeTargets.TAB, Targets.PASSWORD]
 
         return [Targets.USERNAME, Targets.PASSWORD]
 
     def __type_targets(self, cred: Credentials, targets: List[Target]):
-        print(targets)
         for target in targets:
             if target == TypeTargets.DELAY:
                 time.sleep(1)
             elif target == TypeTargets.ENTER:
                 self.typer.press_key(Key.ENTER)
             elif target == TypeTargets.TAB:
                 self.typer.press_key(Key.TAB)
```

### Comparing `rofi_rbw-1.4.0/src/rofi_rbw/selector/bemenu.py` & `rofi_rbw-1.4.1/src/rofi_rbw/selector/bemenu.py`

 * *Files identical despite different names*

### Comparing `rofi_rbw-1.4.0/src/rofi_rbw/selector/rofi.py` & `rofi_rbw-1.4.1/src/rofi_rbw/selector/rofi.py`

 * *Files identical despite different names*

### Comparing `rofi_rbw-1.4.0/src/rofi_rbw/selector/selector.py` & `rofi_rbw-1.4.1/src/rofi_rbw/selector/selector.py`

 * *Files identical despite different names*

### Comparing `rofi_rbw-1.4.0/src/rofi_rbw/selector/wofi.py` & `rofi_rbw-1.4.1/src/rofi_rbw/selector/wofi.py`

 * *Files identical despite different names*

### Comparing `rofi_rbw-1.4.0/src/rofi_rbw/typer/dotool.py` & `rofi_rbw-1.4.1/src/rofi_rbw/typer/dotool.py`

 * *Files identical despite different names*

### Comparing `rofi_rbw-1.4.0/src/rofi_rbw/typer/typer.py` & `rofi_rbw-1.4.1/src/rofi_rbw/typer/typer.py`

 * *Files identical despite different names*

### Comparing `rofi_rbw-1.4.0/src/rofi_rbw/typer/wtype.py` & `rofi_rbw-1.4.1/src/rofi_rbw/typer/wtype.py`

 * *Files identical despite different names*

### Comparing `rofi_rbw-1.4.0/src/rofi_rbw/typer/xdotool.py` & `rofi_rbw-1.4.1/src/rofi_rbw/typer/xdotool.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,14 +31,14 @@
             ]
         )
         # workaround for https://github.com/jordansissel/xdotool/issues/43
         run(["xdotool", "keyup", "Shift_L", "Shift_R", "Alt_L", "Alt_R"])
 
     def press_key(self, key: Key) -> None:
         if key == Key.ENTER:
-            key_name = "enter"
+            key_name = "Return"
         elif key == Key.TAB:
-            key_name = "tab"
+            key_name = "Tab"
         else:
             raise Exception("Unknown key")
 
         run(["xdotool", "key", key_name])
```

### Comparing `rofi_rbw-1.4.0/src/rofi_rbw/typer/ydotool.py` & `rofi_rbw-1.4.1/src/rofi_rbw/typer/ydotool.py`

 * *Files identical despite different names*

### Comparing `rofi_rbw-1.4.0/PKG-INFO` & `rofi_rbw-1.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rofi-rbw
-Version: 1.4.0
+Version: 1.4.1
 Summary: Rofi frontend for Bitwarden
 Home-page: https://github.com/fdw/rofi-rbw
 License: MIT
 Author: Fabian Winter
 Author-email: 5821180+fdw@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -19,14 +19,17 @@
 Description-Content-Type: text/markdown
 
 # rbw-rofi
 ## A rofi frontend for Bitwarden
 
 Based on the alternative [Bitwarden](https://bitwarden.com/) CLI [rbw](https://github.com/doy/rbw/) and inspired by [rofi-pass](https://github.com/carnager/rofi-pass), `rbw-rofi` is a simplistic password typer/copier using [rofi](https://github.com/davatorium/rofi) and [wofi](https://hg.sr.ht/~scoopta/wofi).
 
+![Screenshot of rofi-rbw](screenshot.png?raw=true)
+![Screenshot of a rofi-rbw entry menu](screenshot-menu.png?raw=true)
+
 ## Features
 - Autotype password or username (`Enter`/`Alt+3` and `Alt+2`, respectively)
 - Autotype username and password (with a `tab` character in between) with `Alt+1` (and copy TOTP to clipboard)
 - Configure autotyping either as a keybinding or by having a `_autotype` field in your credential
 - Copy username, password or TOTP to the clipboard (`Alt+u`, `Alt+p` and `Alt+t`, respectively)
 - Show an autotype menu with all fields
```

