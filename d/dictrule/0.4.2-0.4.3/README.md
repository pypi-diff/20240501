# Comparing `tmp/dictrule-0.4.2.tar.gz` & `tmp/dictrule-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dictrule-0.4.2.tar", last modified: Mon Apr 29 10:10:28 2024, max compression
+gzip compressed data, was "dictrule-0.4.3.tar", last modified: Wed May  1 17:02:44 2024, max compression
```

## Comparing `dictrule-0.4.2.tar` & `dictrule-0.4.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:10:28.700837 dictrule-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-29 10:10:25.000000 dictrule-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12887 2024-04-29 10:10:28.700837 dictrule-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11590 2024-04-29 10:10:25.000000 dictrule-0.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 10:10:28.700837 dictrule-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-29 10:10:25.000000 dictrule-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:10:28.692836 dictrule-0.4.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:10:28.696836 dictrule-0.4.2/src/dictrule/
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-29 10:10:25.000000 dictrule-0.4.2/src/dictrule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-29 10:10:25.000000 dictrule-0.4.2/src/dictrule/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:10:28.700837 dictrule-0.4.2/src/dictrule/built_in_rules/
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-29 10:10:25.000000 dictrule-0.4.2/src/dictrule/built_in_rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-04-29 10:10:25.000000 dictrule-0.4.2/src/dictrule/built_in_rules/block_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     9198 2024-04-29 10:10:25.000000 dictrule-0.4.2/src/dictrule/built_in_rules/comment_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     7895 2024-04-29 10:10:25.000000 dictrule-0.4.2/src/dictrule/built_in_rules/eval_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     7339 2024-04-29 10:10:25.000000 dictrule-0.4.2/src/dictrule/built_in_rules/for_in_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-04-29 10:10:25.000000 dictrule-0.4.2/src/dictrule/built_in_rules/format_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-04-29 10:10:25.000000 dictrule-0.4.2/src/dictrule/built_in_rules/indent_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-29 10:10:25.000000 dictrule-0.4.2/src/dictrule/built_in_rules/inline_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-29 10:10:25.000000 dictrule-0.4.2/src/dictrule/built_in_rules/join_block_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-04-29 10:10:25.000000 dictrule-0.4.2/src/dictrule/built_in_rules/join_eval_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-29 10:10:25.000000 dictrule-0.4.2/src/dictrule/built_in_rules/stringify_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-29 10:10:25.000000 dictrule-0.4.2/src/dictrule/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-04-29 10:10:25.000000 dictrule-0.4.2/src/dictrule/dr_property.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-29 10:10:25.000000 dictrule-0.4.2/src/dictrule/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-04-29 10:10:25.000000 dictrule-0.4.2/src/dictrule/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-29 10:10:25.000000 dictrule-0.4.2/src/dictrule/rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-04-29 10:10:25.000000 dictrule-0.4.2/src/dictrule/var_property.py
--rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-04-29 10:10:25.000000 dictrule-0.4.2/src/dictrule/variable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:10:28.700837 dictrule-0.4.2/src/dictrule.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12887 2024-04-29 10:10:28.000000 dictrule-0.4.2/src/dictrule.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-29 10:10:28.000000 dictrule-0.4.2/src/dictrule.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 10:10:28.000000 dictrule-0.4.2/src/dictrule.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 10:10:28.000000 dictrule-0.4.2/src/dictrule.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-29 10:10:28.000000 dictrule-0.4.2/src/dictrule.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:44.837292 dictrule-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-01 17:02:38.000000 dictrule-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12887 2024-05-01 17:02:44.837292 dictrule-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11590 2024-05-01 17:02:38.000000 dictrule-0.4.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 17:02:44.837292 dictrule-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-05-01 17:02:38.000000 dictrule-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:44.829292 dictrule-0.4.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:44.833292 dictrule-0.4.3/src/dictrule/
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-01 17:02:38.000000 dictrule-0.4.3/src/dictrule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-01 17:02:38.000000 dictrule-0.4.3/src/dictrule/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:44.833292 dictrule-0.4.3/src/dictrule/built_in_rules/
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-01 17:02:38.000000 dictrule-0.4.3/src/dictrule/built_in_rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-01 17:02:38.000000 dictrule-0.4.3/src/dictrule/built_in_rules/block_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9198 2024-05-01 17:02:38.000000 dictrule-0.4.3/src/dictrule/built_in_rules/comment_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7895 2024-05-01 17:02:38.000000 dictrule-0.4.3/src/dictrule/built_in_rules/eval_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7339 2024-05-01 17:02:38.000000 dictrule-0.4.3/src/dictrule/built_in_rules/for_in_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-05-01 17:02:38.000000 dictrule-0.4.3/src/dictrule/built_in_rules/format_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-05-01 17:02:38.000000 dictrule-0.4.3/src/dictrule/built_in_rules/indent_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-01 17:02:38.000000 dictrule-0.4.3/src/dictrule/built_in_rules/inline_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-05-01 17:02:38.000000 dictrule-0.4.3/src/dictrule/built_in_rules/join_block_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-01 17:02:38.000000 dictrule-0.4.3/src/dictrule/built_in_rules/join_eval_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-01 17:02:38.000000 dictrule-0.4.3/src/dictrule/built_in_rules/stringify_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-01 17:02:38.000000 dictrule-0.4.3/src/dictrule/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-05-01 17:02:38.000000 dictrule-0.4.3/src/dictrule/dr_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-05-01 17:02:38.000000 dictrule-0.4.3/src/dictrule/eo_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-05-01 17:02:38.000000 dictrule-0.4.3/src/dictrule/eval_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-01 17:02:38.000000 dictrule-0.4.3/src/dictrule/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-05-01 17:02:38.000000 dictrule-0.4.3/src/dictrule/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-01 17:02:38.000000 dictrule-0.4.3/src/dictrule/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:44.833292 dictrule-0.4.3/src/dictrule.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12887 2024-05-01 17:02:44.000000 dictrule-0.4.3/src/dictrule.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-01 17:02:44.000000 dictrule-0.4.3/src/dictrule.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 17:02:44.000000 dictrule-0.4.3/src/dictrule.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 17:02:44.000000 dictrule-0.4.3/src/dictrule.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-01 17:02:44.000000 dictrule-0.4.3/src/dictrule.egg-info/top_level.txt
```

### Comparing `dictrule-0.4.2/LICENSE` & `dictrule-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dictrule-0.4.2/PKG-INFO` & `dictrule-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dictrule
-Version: 0.4.2
+Version: 0.4.3
 Summary: Python rules defined by a dict and a text generator from the rules
 Home-page: https://github.com/elhoangvu/dictrule
 Author: Zooxy Le
 Author-email: elhoangvu@gmail.com
 License: MIT License
 Project-URL: Documentation, https://github.com/elhoangvu/dictrule
 Project-URL: Source, https://github.com/elhoangvu/dictrule
```

### Comparing `dictrule-0.4.2/README.md` & `dictrule-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `dictrule-0.4.2/setup.py` & `dictrule-0.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `dictrule-0.4.2/src/dictrule/__init__.py` & `dictrule-0.4.3/src/dictrule/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 \__,_/_/\___/\__/_/   \__,_/_/\___/ 
 
 """
 
 from .generator import Generator
 from .rule import Rule
 from .context import Context
-from .var_property import var_property
-from .variable import Variable
+from .eo_property import eo_property
+from .eval_object import EvalObject
 from .__version__ import (
     __title__,
     __description__,
     __url__,
     __version__,
     __author__,
     __author_email__,
@@ -53,16 +53,16 @@
     "EvalRule",
     "InlineRule",
     "IndentRule",
     "ForInRule",
     "JoinBlockRule",
     "JoinEvalRule",
     "FormatRule",
-    "var_property",
-    "Variable",
+    "eo_property",
+    "EvalObject",
     "__title__",
     "__description__",
     "__url__",
     "__version__",
     "__author__",
     "__author_email__",
     "__license__",
```

### Comparing `dictrule-0.4.2/src/dictrule/__version__.py` & `dictrule-0.4.3/src/dictrule/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,12 +6,12 @@
 \__,_/_/\___/\__/_/   \__,_/_/\___/    |___/\___/_/  /____/_/\____/_/ /_/ 
                                                                           
 """
 
 __title__ = "dictrule"
 __description__ = "Python rules defined by a dict and a text generator from the rules"
 __url__ = "https://github.com/elhoangvu/dictrule"
-__version__ = "0.4.2"
+__version__ = "0.4.3"
 __author__ = "Zooxy Le"
 __author_email__ = "elhoangvu@gmail.com"
 __license__ = "MIT License"
 __copyright__ = "Copyright Zooxy Le"
```

### Comparing `dictrule-0.4.2/src/dictrule/built_in_rules/__init__.py` & `dictrule-0.4.3/src/dictrule/built_in_rules/__init__.py`

 * *Files identical despite different names*

### Comparing `dictrule-0.4.2/src/dictrule/built_in_rules/block_rule.py` & `dictrule-0.4.3/src/dictrule/built_in_rules/block_rule.py`

 * *Files identical despite different names*

### Comparing `dictrule-0.4.2/src/dictrule/built_in_rules/comment_rule.py` & `dictrule-0.4.3/src/dictrule/built_in_rules/comment_rule.py`

 * *Files identical despite different names*

### Comparing `dictrule-0.4.2/src/dictrule/built_in_rules/eval_rule.py` & `dictrule-0.4.3/src/dictrule/built_in_rules/eval_rule.py`

 * *Files identical despite different names*

### Comparing `dictrule-0.4.2/src/dictrule/built_in_rules/for_in_rule.py` & `dictrule-0.4.3/src/dictrule/built_in_rules/for_in_rule.py`

 * *Files identical despite different names*

### Comparing `dictrule-0.4.2/src/dictrule/built_in_rules/format_rule.py` & `dictrule-0.4.3/src/dictrule/built_in_rules/format_rule.py`

 * *Files identical despite different names*

### Comparing `dictrule-0.4.2/src/dictrule/built_in_rules/indent_rule.py` & `dictrule-0.4.3/src/dictrule/built_in_rules/indent_rule.py`

 * *Files identical despite different names*

### Comparing `dictrule-0.4.2/src/dictrule/built_in_rules/inline_rule.py` & `dictrule-0.4.3/src/dictrule/built_in_rules/inline_rule.py`

 * *Files identical despite different names*

### Comparing `dictrule-0.4.2/src/dictrule/built_in_rules/join_block_rule.py` & `dictrule-0.4.3/src/dictrule/built_in_rules/join_block_rule.py`

 * *Files identical despite different names*

### Comparing `dictrule-0.4.2/src/dictrule/built_in_rules/join_eval_rule.py` & `dictrule-0.4.3/src/dictrule/built_in_rules/join_eval_rule.py`

 * *Files identical despite different names*

### Comparing `dictrule-0.4.2/src/dictrule/built_in_rules/stringify_rule.py` & `dictrule-0.4.3/src/dictrule/built_in_rules/stringify_rule.py`

 * *Files identical despite different names*

### Comparing `dictrule-0.4.2/src/dictrule/context.py` & `dictrule-0.4.3/src/dictrule/context.py`

 * *Files identical despite different names*

### Comparing `dictrule-0.4.2/src/dictrule/dr_property.py` & `dictrule-0.4.3/src/dictrule/dr_property.py`

 * *Files identical despite different names*

### Comparing `dictrule-0.4.2/src/dictrule/generator.py` & `dictrule-0.4.3/src/dictrule/generator.py`

 * *Files identical despite different names*

### Comparing `dictrule-0.4.2/src/dictrule/rule.py` & `dictrule-0.4.3/src/dictrule/rule.py`

 * *Files identical despite different names*

### Comparing `dictrule-0.4.2/src/dictrule/var_property.py` & `dictrule-0.4.3/src/dictrule/eo_property.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-"""var_property decorator module"""
+"""eo_property decorator module"""
 
 from typing import (
     List,
     Any,
     Callable,
     Optional,
 )
 
 
-class var_property:
-    """var_property decorator that defines property for dictrule.Variable.
+class eo_property:
+    """eo_property decorator that defines property for dictrule.EvalObject.
 
     Examples:
     ---------
     >>> class Person:
-    ...     @var_property
+    ...     @eo_property
     ...     def name(self) -> str:
     ...         return "Zooxy"
     ...     def age(self) -> int:
     ...         return 20
-    >>> var = dictrule.Variable.from_object(Person())
-    >>> print(isinstance(var, Variable))
+    >>> obj = dictrule.EvalObject.from_object(Person())
+    >>> print(isinstance(var, EvalObject))
     True
-    >>> print(var.name)
+    >>> print(obj.name)
     Zooxy
-    >>> print(var.age)
+    >>> print(obj.age)
     20
     """
 
     def __init__(
         self,
         fget: Optional[Callable[[Any], Any]] = None,
         fset: Optional[Callable[[Any, Any], None]] = None,
         fdel: Optional[Callable[[Any], None]] = None,
         doc: Optional[str] = None,
     ):
-        """var_property decorator
+        """eo_property decorator
 
         Args:
             fget (Optional[Callable[[Any], Any]], optional): Getter method. Defaults to None.
             fset (Optional[Callable[[Any, Any], None]], optional): Setter method. Defaults to None.
             fdel (Optional[Callable[[Any], None]], optional): Delete method. Defaults to None.
             doc (Optional[str], optional): Document string. Defaults to None.
         """
@@ -65,40 +65,40 @@
         self.fset(obj, value)
 
     def __delete__(self, obj) -> None:
         if self.fdel is None:
             raise AttributeError("can't delete attribute")
         self.fdel(obj)
 
-    def getter(self, fget) -> "var_property":
+    def getter(self, fget) -> "eo_property":
         """Getter decorator
 
         Examples:
         ---------
         >>> class Sample:
-        ...     @var_property
+        ...     @eo_property
         ...     def name(self):
         ...         return "Zooxy"
         >>> Sample().name
         Zooxy
         """
         return type(self)(fget, self.fset, self.fdel, self.__doc__)
 
-    def setter(self, fset) -> "var_property":
+    def setter(self, fset) -> "eo_property":
         """Setter decorator
 
         Examples:
         ---------
         >>> @name.setter
         ... def name(self, value: Any):
         ...     self._name = value
         """
         return type(self)(self.fget, fset, self.fdel, self.__doc__)
 
-    def deleter(self, fdel) -> "var_property":
+    def deleter(self, fdel) -> "eo_property":
         """Deleter decorator
 
         Examples:
         ---------
         >>> @name.deleter
         ... def name(self):
         ...     del self._name
@@ -106,24 +106,24 @@
         return type(self)(self.fget, self.fset, fdel, self.__doc__)
 
     @classmethod
     def properties(
         cls,
         instance: Any,
     ) -> List[Callable[[Any], Any]]:
-        """Fetches all `var_property` of `instance`.
+        """Fetches all `eo_property` of `instance`.
 
         Args:
-            instance (Any): Instance using `var_property`.
+            instance (Any): Instance using `eo_property`.
 
         Returns:
-            List[Callable]: List of `var_property` functions
+            List[Callable]: List of `eo_property` functions
         """
         properties: List[Callable] = []
         for name in dir(instance.__class__):
             attr = getattr(instance.__class__, name, None)
-            is_prop = isinstance(attr, var_property)
+            is_prop = isinstance(attr, eo_property)
             if not is_prop:
                 continue
 
             properties.append(attr)
         return properties
```

### Comparing `dictrule-0.4.2/src/dictrule/variable.py` & `dictrule-0.4.3/src/dictrule/eval_object.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,78 +1,78 @@
-"""Variable module"""
+"""EvalObject module"""
 
 from typing import (
     Any,
     List,
     Dict,
     Set,
     Optional,
 )
 
-from .var_property import var_property
+from .eo_property import eo_property
 
 
-class Variable:
+class EvalObject:
     """Parses instances with nested values.
 
     Supported value types:
-    - An item in Variable.PRIMITIVE_TYPES: [
+    - An item in EvalObject.PRIMITIVE_TYPES: [
         int,
         float,
         str,
     ]
     - list
     - set
     - dict
-    - Variable
+    - EvalObject
 
     Examples:
     ---------
     >>> class Sample:
-    ...     @var_property
+    ...     @eo_property
     ...     def name(self) -> str:
     ...         return "Zooxy"
     ...     def age(self) -> int:
     ...         return 20
-    >>> var = Variable.from_var_property_object(Sample())
-    >>> print(var.name)
+    >>> obj = EvalObject.from_eo_property_object(Sample())
+    >>> print(obj.name)
     Zooxy
-    >>> print(hasattr(var, "age"))
+    >>> print(hasattr(obj, "age"))
     False
     """
 
     PRIMITIVE_TYPES = set(
         [
             int,
             float,
             str,
         ]
     )
 
     @staticmethod
-    def from_var_property_object(
+    def from_eo_property_object(
         obj: Any,
-    ) -> "Variable":
-        """Parses a Variable from obj where properties are decorated with @var_property.
+    ) -> "EvalObject":
+        """Parses a EvalObject from obj where properties are decorated with @eo_property.
 
         Args:
-            obj (Any): The object to parse from @var_property and supported values.
+            obj (Any): The object to parse from @eo_property and supported values.
 
         Returns:
-            Variable: The parsed variable.
+            EvalObject: The parsed object.
         """
 
-        return Variable._parse_value(obj)
+        return EvalObject._parse_value(obj)
 
     def add_object(
         self,
         obj: Any,
         name: str,
     ):
-        """Adds a new object to the Variable instance with a given name.
+        """Adds a new object to the EvalObject instance with a given name.
 
         Args:
             obj (Any): The object to be added.
             name (str): The name for the object.
         """
 
         value = self._parse_value(obj)
@@ -91,34 +91,34 @@
             Optional[Any]: The parsed value.
         """
 
         if value is None:
             return
 
         parsed_value = None
-        if type(value) in Variable.PRIMITIVE_TYPES or isinstance(value, Variable):
+        if type(value) in EvalObject.PRIMITIVE_TYPES or isinstance(value, EvalObject):
             parsed_value = value
         elif isinstance(value, list):
-            parsed_value = Variable._parse_list(
+            parsed_value = EvalObject._parse_list(
                 value=value,
             )
         elif isinstance(value, set):
-            parsed_value = Variable._parse_set(
+            parsed_value = EvalObject._parse_set(
                 value=value,
             )
         elif isinstance(value, dict):
-            parsed_value = Variable._parse_dict(
+            parsed_value = EvalObject._parse_dict(
                 value=value,
             )
         else:
-            attrs = var_property.properties(value)
+            attrs = eo_property.properties(value)
             if not attrs:
                 return None
 
-            parsed_value = Variable()
+            parsed_value = EvalObject()
             for attr in attrs:
                 setattr(parsed_value, attr.__name__, attr.__get__(value))
 
         return parsed_value
 
     @staticmethod
     def _parse_list(
@@ -131,15 +131,15 @@
 
         Returns:
             Optional[List[Any]]: The parsed list.
         """
 
         new_list: List[Any] = []
         for v in value:
-            parsed_value = Variable._parse_value(v)
+            parsed_value = EvalObject._parse_value(v)
             if parsed_value:
                 new_list.append(parsed_value)
         return new_list
 
     @staticmethod
     def _parse_set(
         value: Set[Any],
@@ -151,15 +151,15 @@
 
         Returns:
             Optional[Set[Any]]: The parsed set.
         """
 
         new_set: Set[Any] = set()
         for v in value:
-            parsed_value = Variable._parse_value(v)
+            parsed_value = EvalObject._parse_value(v)
             if not parsed_value:
                 continue
 
             new_set.add(parsed_value)
 
         return new_set
 
@@ -174,18 +174,18 @@
 
         Returns:
             Optional[Dict[str, Any]]: The parsed dictionary.
         """
 
         new_dict: Dict[str, Any] = {}
         for k, v in value.items():
-            parsed_key = Variable._parse_value(k)
+            parsed_key = EvalObject._parse_value(k)
             if not parsed_key:
                 continue
 
-            parsed_value = Variable._parse_value(v)
+            parsed_value = EvalObject._parse_value(v)
             if not parsed_value:
                 continue
 
             new_dict[parsed_key] = parsed_value
 
         return new_dict
```

### Comparing `dictrule-0.4.2/src/dictrule.egg-info/PKG-INFO` & `dictrule-0.4.3/src/dictrule.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dictrule
-Version: 0.4.2
+Version: 0.4.3
 Summary: Python rules defined by a dict and a text generator from the rules
 Home-page: https://github.com/elhoangvu/dictrule
 Author: Zooxy Le
 Author-email: elhoangvu@gmail.com
 License: MIT License
 Project-URL: Documentation, https://github.com/elhoangvu/dictrule
 Project-URL: Source, https://github.com/elhoangvu/dictrule
```

### Comparing `dictrule-0.4.2/src/dictrule.egg-info/SOURCES.txt` & `dictrule-0.4.3/src/dictrule.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 LICENSE
 README.md
 setup.py
 src/dictrule/__init__.py
 src/dictrule/__version__.py
 src/dictrule/context.py
 src/dictrule/dr_property.py
+src/dictrule/eo_property.py
+src/dictrule/eval_object.py
 src/dictrule/exceptions.py
 src/dictrule/generator.py
 src/dictrule/rule.py
-src/dictrule/var_property.py
-src/dictrule/variable.py
 src/dictrule.egg-info/PKG-INFO
 src/dictrule.egg-info/SOURCES.txt
 src/dictrule.egg-info/dependency_links.txt
 src/dictrule.egg-info/not-zip-safe
 src/dictrule.egg-info/top_level.txt
 src/dictrule/built_in_rules/__init__.py
 src/dictrule/built_in_rules/block_rule.py
```

