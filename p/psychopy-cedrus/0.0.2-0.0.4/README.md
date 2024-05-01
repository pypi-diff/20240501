# Comparing `tmp/psychopy-cedrus-0.0.2.tar.gz` & `tmp/psychopy_cedrus-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psychopy-cedrus-0.0.2.tar", last modified: Fri Feb  3 16:02:53 2023, max compression
+gzip compressed data, was "psychopy_cedrus-0.0.4.tar", last modified: Wed May  1 10:23:27 2024, max compression
```

## Comparing `psychopy-cedrus-0.0.2.tar` & `psychopy_cedrus-0.0.4.tar`

### file list

```diff
@@ -1,36 +1,47 @@
-drwxr-xr-x   0 lpzjwp     (503) staff       (20)        0 2023-02-03 16:02:53.341206 psychopy-cedrus-0.0.2/
--rw-r--r--   0 lpzjwp     (503) staff       (20)    35149 2023-02-03 16:01:05.000000 psychopy-cedrus-0.0.2/LICENSE
--rw-r--r--   0 lpzjwp     (503) staff       (20)     1719 2023-02-03 16:02:53.341420 psychopy-cedrus-0.0.2/PKG-INFO
--rw-r--r--   0 lpzjwp     (503) staff       (20)      649 2023-02-03 16:01:05.000000 psychopy-cedrus-0.0.2/README.md
-drwxr-xr-x   0 lpzjwp     (503) staff       (20)        0 2023-02-03 16:02:53.333472 psychopy-cedrus-0.0.2/docs/
--rw-r--r--   0 lpzjwp     (503) staff       (20)     2260 2023-02-03 16:01:05.000000 psychopy-cedrus-0.0.2/docs/conf.py
--rw-r--r--   0 lpzjwp     (503) staff       (20)     2944 2023-02-03 16:01:05.000000 psychopy-cedrus-0.0.2/docs/favicon.png
-drwxr-xr-x   0 lpzjwp     (503) staff       (20)        0 2023-02-03 16:02:53.330074 psychopy-cedrus-0.0.2/docs/themes/
-drwxr-xr-x   0 lpzjwp     (503) staff       (20)        0 2023-02-03 16:02:53.330177 psychopy-cedrus-0.0.2/docs/themes/psychopy_plugin/
-drwxr-xr-x   0 lpzjwp     (503) staff       (20)        0 2023-02-03 16:02:53.334697 psychopy-cedrus-0.0.2/docs/themes/psychopy_plugin/static/
--rw-r--r--   0 lpzjwp     (503) staff       (20)    65201 2023-02-03 16:01:05.000000 psychopy-cedrus-0.0.2/docs/themes/psychopy_plugin/static/Nottingham Supported.png
--rw-r--r--   0 lpzjwp     (503) staff       (20)    22964 2023-02-03 16:01:05.000000 psychopy-cedrus-0.0.2/docs/themes/psychopy_plugin/static/Psychopy Plugin Header Large.png
--rw-r--r--   0 lpzjwp     (503) staff       (20)     9576 2023-02-03 16:01:05.000000 psychopy-cedrus-0.0.2/docs/themes/psychopy_plugin/static/Psychopy Plugin Header Small.png
--rw-r--r--   0 lpzjwp     (503) staff       (20)     5173 2023-02-03 16:01:05.000000 psychopy-cedrus-0.0.2/docs/utils.py
-drwxr-xr-x   0 lpzjwp     (503) staff       (20)        0 2023-02-03 16:02:53.335477 psychopy-cedrus-0.0.2/psychopy_cedrus/
--rw-r--r--   0 lpzjwp     (503) staff       (20)      367 2023-02-03 16:02:16.000000 psychopy-cedrus-0.0.2/psychopy_cedrus/__init__.py
--rw-r--r--   0 lpzjwp     (503) staff       (20)     6876 2023-02-03 16:01:05.000000 psychopy-cedrus-0.0.2/psychopy_cedrus/cedrus.py
-drwxr-xr-x   0 lpzjwp     (503) staff       (20)        0 2023-02-03 16:02:53.337934 psychopy-cedrus-0.0.2/psychopy_cedrus/cedrusBox/
--rwxr-xr-x   0 lpzjwp     (503) staff       (20)    13132 2023-02-03 16:01:05.000000 psychopy-cedrus-0.0.2/psychopy_cedrus/cedrusBox/__init__.py
-drwxr-xr-x   0 lpzjwp     (503) staff       (20)        0 2023-02-03 16:02:53.338882 psychopy-cedrus-0.0.2/psychopy_cedrus/cedrusBox/classic/
--rw-r--r--   0 lpzjwp     (503) staff       (20)     4997 2023-02-03 16:01:05.000000 psychopy-cedrus-0.0.2/psychopy_cedrus/cedrusBox/classic/cedrus@2x.png
--rw-r--r--   0 lpzjwp     (503) staff       (20)     1426 2023-02-03 16:01:05.000000 psychopy-cedrus-0.0.2/psychopy_cedrus/cedrusBox/classic/cedrusBox.png
-drwxr-xr-x   0 lpzjwp     (503) staff       (20)        0 2023-02-03 16:02:53.339880 psychopy-cedrus-0.0.2/psychopy_cedrus/cedrusBox/dark/
--rw-r--r--   0 lpzjwp     (503) staff       (20)      855 2023-02-03 16:01:05.000000 psychopy-cedrus-0.0.2/psychopy_cedrus/cedrusBox/dark/cedrusBox.png
--rw-r--r--   0 lpzjwp     (503) staff       (20)     1606 2023-02-03 16:01:05.000000 psychopy-cedrus-0.0.2/psychopy_cedrus/cedrusBox/dark/cedrusBox@2x.png
-drwxr-xr-x   0 lpzjwp     (503) staff       (20)        0 2023-02-03 16:02:53.340842 psychopy-cedrus-0.0.2/psychopy_cedrus/cedrusBox/light/
--rw-r--r--   0 lpzjwp     (503) staff       (20)      841 2023-02-03 16:01:05.000000 psychopy-cedrus-0.0.2/psychopy_cedrus/cedrusBox/light/cedrusBox.png
--rw-r--r--   0 lpzjwp     (503) staff       (20)     1606 2023-02-03 16:01:05.000000 psychopy-cedrus-0.0.2/psychopy_cedrus/cedrusBox/light/cedrusBox@2x.png
-drwxr-xr-x   0 lpzjwp     (503) staff       (20)        0 2023-02-03 16:02:53.337529 psychopy-cedrus-0.0.2/psychopy_cedrus.egg-info/
--rw-r--r--   0 lpzjwp     (503) staff       (20)     1719 2023-02-03 16:02:53.000000 psychopy-cedrus-0.0.2/psychopy_cedrus.egg-info/PKG-INFO
--rw-r--r--   0 lpzjwp     (503) staff       (20)      856 2023-02-03 16:02:53.000000 psychopy-cedrus-0.0.2/psychopy_cedrus.egg-info/SOURCES.txt
--rw-r--r--   0 lpzjwp     (503) staff       (20)        1 2023-02-03 16:02:53.000000 psychopy-cedrus-0.0.2/psychopy_cedrus.egg-info/dependency_links.txt
--rw-r--r--   0 lpzjwp     (503) staff       (20)      101 2023-02-03 16:02:53.000000 psychopy-cedrus-0.0.2/psychopy_cedrus.egg-info/entry_points.txt
--rw-r--r--   0 lpzjwp     (503) staff       (20)       26 2023-02-03 16:02:53.000000 psychopy-cedrus-0.0.2/psychopy_cedrus.egg-info/top_level.txt
--rw-r--r--   0 lpzjwp     (503) staff       (20)     1363 2023-02-03 16:02:08.000000 psychopy-cedrus-0.0.2/pyproject.toml
--rw-r--r--   0 lpzjwp     (503) staff       (20)      103 2023-02-03 16:02:53.342082 psychopy-cedrus-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:23:27.432434 psychopy_cedrus-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-01 10:23:19.000000 psychopy_cedrus-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-01 10:23:27.432434 psychopy_cedrus-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-01 10:23:19.000000 psychopy_cedrus-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:23:27.428434 psychopy_cedrus-0.0.4/docs_src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-01 10:23:19.000000 psychopy_cedrus-0.0.4/docs_src/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-05-01 10:23:19.000000 psychopy_cedrus-0.0.4/docs_src/favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:23:27.424434 psychopy_cedrus-0.0.4/docs_src/themes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:23:27.428434 psychopy_cedrus-0.0.4/docs_src/themes/psychopy_plugin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:23:27.428434 psychopy_cedrus-0.0.4/docs_src/themes/psychopy_plugin/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    65201 2024-05-01 10:23:19.000000 psychopy_cedrus-0.0.4/docs_src/themes/psychopy_plugin/static/Nottingham Supported.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22964 2024-05-01 10:23:19.000000 psychopy_cedrus-0.0.4/docs_src/themes/psychopy_plugin/static/Psychopy Plugin Header Large.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9576 2024-05-01 10:23:19.000000 psychopy_cedrus-0.0.4/docs_src/themes/psychopy_plugin/static/Psychopy Plugin Header Small.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:23:27.428434 psychopy_cedrus-0.0.4/psychopy_cedrus/
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-01 10:23:19.000000 psychopy_cedrus-0.0.4/psychopy_cedrus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6876 2024-05-01 10:23:19.000000 psychopy_cedrus-0.0.4/psychopy_cedrus/cedrus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:23:27.432434 psychopy_cedrus-0.0.4/psychopy_cedrus/components/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 10:23:19.000000 psychopy_cedrus-0.0.4/psychopy_cedrus/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:23:27.432434 psychopy_cedrus-0.0.4/psychopy_cedrus/components/cedrusBox/
+-rw-r--r--   0 runner    (1001) docker     (127)    13268 2024-05-01 10:23:19.000000 psychopy_cedrus-0.0.4/psychopy_cedrus/components/cedrusBox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:23:27.432434 psychopy_cedrus-0.0.4/psychopy_cedrus/components/cedrusBox/classic/
+-rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-05-01 10:23:19.000000 psychopy_cedrus-0.0.4/psychopy_cedrus/components/cedrusBox/classic/cedrus@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-01 10:23:19.000000 psychopy_cedrus-0.0.4/psychopy_cedrus/components/cedrusBox/classic/cedrusBox.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:23:27.432434 psychopy_cedrus-0.0.4/psychopy_cedrus/components/cedrusBox/dark/
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-01 10:23:19.000000 psychopy_cedrus-0.0.4/psychopy_cedrus/components/cedrusBox/dark/cedrusBox.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-01 10:23:19.000000 psychopy_cedrus-0.0.4/psychopy_cedrus/components/cedrusBox/dark/cedrusBox@2x.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:23:27.432434 psychopy_cedrus-0.0.4/psychopy_cedrus/components/cedrusBox/light/
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-01 10:23:19.000000 psychopy_cedrus-0.0.4/psychopy_cedrus/components/cedrusBox/light/cedrusBox.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-01 10:23:19.000000 psychopy_cedrus-0.0.4/psychopy_cedrus/components/cedrusBox/light/cedrusBox@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-01 10:23:19.000000 psychopy_cedrus-0.0.4/psychopy_cedrus/components/riponda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9571 2024-05-01 10:23:19.000000 psychopy_cedrus-0.0.4/psychopy_cedrus/riponda.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:23:27.432434 psychopy_cedrus-0.0.4/psychopy_cedrus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-01 10:23:27.000000 psychopy_cedrus-0.0.4/psychopy_cedrus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-01 10:23:27.000000 psychopy_cedrus-0.0.4/psychopy_cedrus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 10:23:27.000000 psychopy_cedrus-0.0.4/psychopy_cedrus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-01 10:23:27.000000 psychopy_cedrus-0.0.4/psychopy_cedrus.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-01 10:23:27.000000 psychopy_cedrus-0.0.4/psychopy_cedrus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-01 10:23:27.000000 psychopy_cedrus-0.0.4/psychopy_cedrus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-01 10:23:19.000000 psychopy_cedrus-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 10:23:27.432434 psychopy_cedrus-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:23:27.432434 psychopy_cedrus-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-01 10:23:19.000000 psychopy_cedrus-0.0.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:23:27.432434 psychopy_cedrus-0.0.4/tests/test_builder/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 10:23:19.000000 psychopy_cedrus-0.0.4/tests/test_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-01 10:23:19.000000 psychopy_cedrus-0.0.4/tests/test_builder/test_ExampleComponent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:23:27.432434 psychopy_cedrus-0.0.4/tests/test_coder/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 10:23:19.000000 psychopy_cedrus-0.0.4/tests/test_coder/__init__.py
```

### Comparing `psychopy-cedrus-0.0.2/LICENSE` & `psychopy_cedrus-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `psychopy-cedrus-0.0.2/README.md` & `psychopy_cedrus-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `psychopy-cedrus-0.0.2/docs/favicon.png` & `psychopy_cedrus-0.0.4/docs_src/favicon.png`

 * *Files identical despite different names*

### Comparing `psychopy-cedrus-0.0.2/docs/themes/psychopy_plugin/static/Nottingham Supported.png` & `psychopy_cedrus-0.0.4/docs_src/themes/psychopy_plugin/static/Nottingham Supported.png`

 * *Files identical despite different names*

### Comparing `psychopy-cedrus-0.0.2/docs/themes/psychopy_plugin/static/Psychopy Plugin Header Large.png` & `psychopy_cedrus-0.0.4/docs_src/themes/psychopy_plugin/static/Psychopy Plugin Header Large.png`

 * *Files identical despite different names*

### Comparing `psychopy-cedrus-0.0.2/docs/themes/psychopy_plugin/static/Psychopy Plugin Header Small.png` & `psychopy_cedrus-0.0.4/docs_src/themes/psychopy_plugin/static/Psychopy Plugin Header Small.png`

 * *Files identical despite different names*

### Comparing `psychopy-cedrus-0.0.2/psychopy_cedrus/cedrus.py` & `psychopy_cedrus-0.0.4/psychopy_cedrus/cedrus.py`

 * *Files identical despite different names*

### Comparing `psychopy-cedrus-0.0.2/psychopy_cedrus/cedrusBox/__init__.py` & `psychopy_cedrus-0.0.4/psychopy_cedrus/components/cedrusBox/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,16 @@
 # Distributed under the terms of the GNU General Public License (GPL).
 
 from pathlib import Path
 
 from psychopy.experiment.components import Param, _translate
 from psychopy.experiment.components.keyboard import KeyboardComponent
 from psychopy.experiment import CodeGenerationException, valid_var_re
-from psychopy.localization import _localized as __localized
-_localized = __localized.copy()
 __author__ = 'Jon Peirce'
 
-# only use _localized values for label values, nothing functional:
-_localized.update({'deviceNumber': _translate('Device number'),
-                   'useBoxTimer': _translate("Use box timer")})
-
 
 class cedrusButtonBoxComponent(KeyboardComponent):
     """An event class for checking an Cedrus RBxxx button boxes
     using XID library
 
     This is based on keyboard component, several important differences:
     - no special response class analogous to event.BuilderKeyResponse()
@@ -76,36 +70,42 @@
 
         msg = _translate('Device number, if you have multiple devices which'
                          ' one do you want (0, 1, 2...)')
         self.params['deviceNumber'] = Param(
             deviceNumber, valType='int', inputType="spin", allowedTypes=[], categ='Hardware',
             updates='constant', allowedUpdates=[],
             hint=msg,
-            label=_localized['deviceNumber'])
+            label=_translate('deviceNumber'))
 
         # self.params['getReleaseTime'] = Param(getReleaseTime,
         #    valType='bool', allowedVals=[True, False],
         #    updates='constant', allowedUpdates=[],
         #    hint="Wait for the key to be released and store the time
         #       that it was held down",
         #    label="Get release time")
 
         msg = _translate('According to Cedrus the response box timer has '
                          'a drift - use with caution!')
         self.params['useBoxTimer'] = Param(
             getReleaseTime, valType='bool', inputType="bool", allowedVals=[True, False], categ='Hardware',
             updates='constant', allowedUpdates=[],
             hint=msg,
-            label=_localized['useBoxTimer'])
+            label=_translate('useBoxTimer'))
 
     def writeRunOnceInitCode(self, buff):
         code = ("try:  # to use the Cedrus response box\n"
-                "   import pyxid2 as pyxid\n"
+                "    import pyxid2 as pyxid\n"
                 "except ImportError:\n"
-                "   import pyxid\n"
+                "    import pyxid\n"
+                "except OSError as err:\n"
+                "    if 'd2xx' in str(err):\n"
+                "        # importing will raise an OSError if you're missing the D2XX drivers\n"
+                "        raise err from OSError('Cedrus Component needs the D2XX drivers to run. Please install from: https://ftdichip.com/drivers/d2xx-drivers/.')\n"
+                "    else:\n"
+                "        raise err\n"
                 "cedrusBox_%(deviceNumber)s = None\n"
                 "for n in range(10):  # doesn't always work first time!\n"
                 "    try:\n"
                 "        devices = pyxid.get_xid_devices()\n"
                 "        core.wait(0.1)\n"
                 "        cedrusBox_%(deviceNumber)s = devices[%(deviceNumber)s]\n"
                 "        cedrusBox_%(deviceNumber)s.clock = core.Clock()\n"
```

### Comparing `psychopy-cedrus-0.0.2/psychopy_cedrus/cedrusBox/classic/cedrus@2x.png` & `psychopy_cedrus-0.0.4/psychopy_cedrus/components/cedrusBox/classic/cedrus@2x.png`

 * *Files identical despite different names*

### Comparing `psychopy-cedrus-0.0.2/psychopy_cedrus/cedrusBox/classic/cedrusBox.png` & `psychopy_cedrus-0.0.4/psychopy_cedrus/components/cedrusBox/classic/cedrusBox.png`

 * *Files identical despite different names*

### Comparing `psychopy-cedrus-0.0.2/psychopy_cedrus/cedrusBox/dark/cedrusBox.png` & `psychopy_cedrus-0.0.4/psychopy_cedrus/components/cedrusBox/dark/cedrusBox.png`

 * *Files identical despite different names*

### Comparing `psychopy-cedrus-0.0.2/psychopy_cedrus/cedrusBox/dark/cedrusBox@2x.png` & `psychopy_cedrus-0.0.4/psychopy_cedrus/components/cedrusBox/dark/cedrusBox@2x.png`

 * *Files identical despite different names*

### Comparing `psychopy-cedrus-0.0.2/psychopy_cedrus/cedrusBox/light/cedrusBox.png` & `psychopy_cedrus-0.0.4/psychopy_cedrus/components/cedrusBox/light/cedrusBox.png`

 * *Files identical despite different names*

### Comparing `psychopy-cedrus-0.0.2/psychopy_cedrus/cedrusBox/light/cedrusBox@2x.png` & `psychopy_cedrus-0.0.4/psychopy_cedrus/components/cedrusBox/light/cedrusBox@2x.png`

 * *Files identical despite different names*

### Comparing `psychopy-cedrus-0.0.2/psychopy_cedrus.egg-info/SOURCES.txt` & `psychopy_cedrus-0.0.4/psychopy_cedrus.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 LICENSE
 README.md
 pyproject.toml
-setup.cfg
-docs/conf.py
-docs/favicon.png
-docs/utils.py
-docs/themes/psychopy_plugin/static/Nottingham Supported.png
-docs/themes/psychopy_plugin/static/Psychopy Plugin Header Large.png
-docs/themes/psychopy_plugin/static/Psychopy Plugin Header Small.png
+docs_src/conf.py
+docs_src/favicon.png
+docs_src/themes/psychopy_plugin/static/Nottingham Supported.png
+docs_src/themes/psychopy_plugin/static/Psychopy Plugin Header Large.png
+docs_src/themes/psychopy_plugin/static/Psychopy Plugin Header Small.png
 psychopy_cedrus/__init__.py
 psychopy_cedrus/cedrus.py
+psychopy_cedrus/riponda.py
 psychopy_cedrus.egg-info/PKG-INFO
 psychopy_cedrus.egg-info/SOURCES.txt
 psychopy_cedrus.egg-info/dependency_links.txt
 psychopy_cedrus.egg-info/entry_points.txt
+psychopy_cedrus.egg-info/requires.txt
 psychopy_cedrus.egg-info/top_level.txt
-psychopy_cedrus/cedrusBox/__init__.py
-psychopy_cedrus/cedrusBox/classic/cedrus@2x.png
-psychopy_cedrus/cedrusBox/classic/cedrusBox.png
-psychopy_cedrus/cedrusBox/dark/cedrusBox.png
-psychopy_cedrus/cedrusBox/dark/cedrusBox@2x.png
-psychopy_cedrus/cedrusBox/light/cedrusBox.png
-psychopy_cedrus/cedrusBox/light/cedrusBox@2x.png
+psychopy_cedrus/components/__init__.py
+psychopy_cedrus/components/riponda.py
+psychopy_cedrus/components/cedrusBox/__init__.py
+psychopy_cedrus/components/cedrusBox/classic/cedrus@2x.png
+psychopy_cedrus/components/cedrusBox/classic/cedrusBox.png
+psychopy_cedrus/components/cedrusBox/dark/cedrusBox.png
+psychopy_cedrus/components/cedrusBox/dark/cedrusBox@2x.png
+psychopy_cedrus/components/cedrusBox/light/cedrusBox.png
+psychopy_cedrus/components/cedrusBox/light/cedrusBox@2x.png
+tests/__init__.py
+tests/test_builder/__init__.py
+tests/test_builder/test_ExampleComponent.py
+tests/test_coder/__init__.py
```

### Comparing `psychopy-cedrus-0.0.2/pyproject.toml` & `psychopy_cedrus-0.0.4/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,59 @@
 [build-system]
 requires = ["setuptools>=40.8.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "psychopy-cedrus"
-version = "0.0.2"
+version = "0.0.4"
 description = "Extension package for PsychoPy which adds support for various hardware devices by the Cedrus Corporation."
 readme = "README.md"
 requires-python = ">= 3.7"
 license = { text = "GNU General Public License v3 (GPLv3)" }
 authors = [
   { name = "Jon Peirce", email = "jon@opensceincetools.org" },
   { name = "Matthew Cutone", email = "mcutone@opensceincetools.org" },
+  { name = "Todd Parsons", email = "todd@opensceincetools.org" },
 ]
 classifiers = [
   "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
 ]
-urls.homepage = "https://github.com/mdcutone/psychopy-cedrus"
-urls.changelog = "https://github.com/mdcutone/psychopy-cedrus/blob/main/CHANGELOG.txt"
+urls.homepage = "https://psychopy.github.io/psychopy-cedrus"
+urls.changelog = "https://github.com/psychopy/psychopy-cedrus/blob/main/CHANGELOG.txt"
+
+[project.optional-dependencies]
+# dependencies for building the docs
+docs = [
+  "psychopy",
+  "sphinx",
+  "furo",
+]
+# dependencies for running the test suite
+tests = [
+  "psychopy",
+  "pytest",
+]
 
 [tool.setuptools.packages.find]
 where = ["",]
 
 [tool.setuptools.package-data]
 "*" = ["*.png",]
 
 [project.entry-points."psychopy.experiment.components"]
-cedrusButtonBoxComponent = "psychopy_cedrus:cedrusButtonBoxComponent"
+cedrusButtonBoxComponent = "psychopy_cedrus.components.cedrusBox:cedrusButtonBoxComponent"
+RipondaButtonBoxBackend = "psychopy_cedrus.components.riponda:RipondaButtonBoxBackend"
+
+[project.entry-points."psychopy.hardware.cedrus"]
+RB730 = "psychopy_cedrus.cedrus:RB730"
+Riponda = "psychopy_cedrus.riponda:Riponda"
+RipondaPhotodiodeGroup = "psychopy_cedrus.riponda:RipondaPhotodiodeGroup"
+RipondaButtonGroup = "psychopy_cedrus.riponda:RipondaButtonGroup"
+RipondaVoicekey = "psychopy_cedrus.riponda:RipondaVoicekey"
```

