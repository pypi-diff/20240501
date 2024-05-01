# Comparing `tmp/command_creator-1.1.2.tar.gz` & `tmp/command_creator-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "command_creator-1.1.2.tar", last modified: Wed Feb  7 20:46:36 2024, max compression
+gzip compressed data, was "command_creator-1.1.3.tar", last modified: Wed May  1 19:07:52 2024, max compression
```

## Comparing `command_creator-1.1.2.tar` & `command_creator-1.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 20:46:36.417951 command_creator-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-02-07 20:46:25.000000 command_creator-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-02-07 20:46:25.000000 command_creator-1.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    32616 2024-02-07 20:46:36.417951 command_creator-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-02-07 20:46:25.000000 command_creator-1.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-02-07 20:46:25.000000 command_creator-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-07 20:46:36.417951 command_creator-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-02-07 20:46:25.000000 command_creator-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 20:46:36.413951 command_creator-1.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 20:46:36.413951 command_creator-1.1.2/src/command_creator/
--rw-r--r--   0 runner    (1001) docker     (127)    10494 2024-02-07 20:46:25.000000 command_creator-1.1.2/src/command_creator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-02-07 20:46:25.000000 command_creator-1.1.2/src/command_creator/_info.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 20:46:25.000000 command_creator-1.1.2/src/command_creator/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 20:46:36.413951 command_creator-1.1.2/src/command_creator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    32616 2024-02-07 20:46:36.000000 command_creator-1.1.2/src/command_creator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-02-07 20:46:36.000000 command_creator-1.1.2/src/command_creator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-07 20:46:36.000000 command_creator-1.1.2/src/command_creator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-02-07 20:46:36.000000 command_creator-1.1.2/src/command_creator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-07 20:46:36.000000 command_creator-1.1.2/src/command_creator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 20:46:36.413951 command_creator-1.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-02-07 20:46:25.000000 command_creator-1.1.2/tests/test_creator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-02-07 20:46:25.000000 command_creator-1.1.2/tests/test_import.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:07:52.846481 command_creator-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-05-01 19:07:48.000000 command_creator-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-01 19:07:48.000000 command_creator-1.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    32616 2024-05-01 19:07:52.846481 command_creator-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-01 19:07:48.000000 command_creator-1.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-01 19:07:48.000000 command_creator-1.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 19:07:52.846481 command_creator-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-01 19:07:48.000000 command_creator-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:07:52.842481 command_creator-1.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:07:52.842481 command_creator-1.1.3/src/command_creator/
+-rw-r--r--   0 runner    (1001) docker     (127)    10508 2024-05-01 19:07:48.000000 command_creator-1.1.3/src/command_creator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-01 19:07:48.000000 command_creator-1.1.3/src/command_creator/_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 19:07:48.000000 command_creator-1.1.3/src/command_creator/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:07:52.846481 command_creator-1.1.3/src/command_creator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    32616 2024-05-01 19:07:52.000000 command_creator-1.1.3/src/command_creator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-01 19:07:52.000000 command_creator-1.1.3/src/command_creator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 19:07:52.000000 command_creator-1.1.3/src/command_creator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-01 19:07:52.000000 command_creator-1.1.3/src/command_creator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-01 19:07:52.000000 command_creator-1.1.3/src/command_creator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:07:52.846481 command_creator-1.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-05-01 19:07:48.000000 command_creator-1.1.3/tests/test_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-01 19:07:48.000000 command_creator-1.1.3/tests/test_import.py
```

### Comparing `command_creator-1.1.2/LICENSE` & `command_creator-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `command_creator-1.1.2/MANIFEST.in` & `command_creator-1.1.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `command_creator-1.1.2/PKG-INFO` & `command_creator-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: command_creator
-Version: 1.1.2
+Version: 1.1.3
 Summary: A package to simplify the creation of Python Command-Line tools
 Author-email: Benjamin Davis <allrisc.dev@gmail.com>
 License:                   GNU LESSER GENERAL PUBLIC LICENSE
                                Version 2.1, February 1999
         
          Copyright (C) 1991, 1999 Free Software Foundation, Inc.
          51 Franklin Street, Fifth Floor, Boston, MA  02110-1301  USA
```

### Comparing `command_creator-1.1.2/README.md` & `command_creator-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `command_creator-1.1.2/pyproject.toml` & `command_creator-1.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `command_creator-1.1.2/setup.py` & `command_creator-1.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `command_creator-1.1.2/src/command_creator/__init__.py` & `command_creator-1.1.3/src/command_creator/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; If not, see <https://www.gnu.org/licenses/>.
 #####################################################################################
 
 from __future__ import annotations
-import sys
-from typing import Any, Callable, Mapping, TypeVar, Type, ClassVar
+from typing import Any, Callable, Mapping, TypeVar, Type, ClassVar, NoReturn
 
+import sys
 from dataclasses import Field, dataclass, MISSING, fields
 from enum import Enum
 from abc import ABC, abstractmethod
 from argparse import ArgumentParser, Namespace
 import re
 
 #####################################################################################
@@ -302,15 +302,15 @@
       arg_dict["sub_command"] = cls.sub_commands[args.sub_command].from_args(args)
     else:
       arg_dict["sub_command"] = None
 
     return cls(**arg_dict)
 
   @classmethod
-  def execute(cls: Type[CommandT]) -> None:
+  def execute(cls: Type[CommandT]) -> NoReturn:
     """Execute the command and exit with the return code
     """
     parser = cls.create_parser()
     args = parser.parse_args()
     cmd = cls.from_args(args)
     exit(cmd())
```

### Comparing `command_creator-1.1.2/src/command_creator/_info.py` & `command_creator-1.1.3/src/command_creator/_info.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,9 +15,9 @@
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; If not, see <https://www.gnu.org/licenses/>.
 #####################################################################################
 
 from __future__ import annotations
 
 
-__version__: str = "1.1.2"
+__version__: str = "1.1.3"
 __author__: str = "Benjamin Davis"
```

### Comparing `command_creator-1.1.2/src/command_creator.egg-info/PKG-INFO` & `command_creator-1.1.3/src/command_creator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: command_creator
-Version: 1.1.2
+Version: 1.1.3
 Summary: A package to simplify the creation of Python Command-Line tools
 Author-email: Benjamin Davis <allrisc.dev@gmail.com>
 License:                   GNU LESSER GENERAL PUBLIC LICENSE
                                Version 2.1, February 1999
         
          Copyright (C) 1991, 1999 Free Software Foundation, Inc.
          51 Franklin Street, Fifth Floor, Boston, MA  02110-1301  USA
```

### Comparing `command_creator-1.1.2/tests/test_creator.py` & `command_creator-1.1.3/tests/test_creator.py`

 * *Files identical despite different names*

### Comparing `command_creator-1.1.2/tests/test_import.py` & `command_creator-1.1.3/tests/test_import.py`

 * *Files identical despite different names*

