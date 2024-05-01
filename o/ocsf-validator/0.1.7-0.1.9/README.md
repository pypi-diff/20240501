# Comparing `tmp/ocsf_validator-0.1.7.tar.gz` & `tmp/ocsf_validator-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocsf_validator-0.1.7.tar", max compression
+gzip compressed data, was "ocsf_validator-0.1.9.tar", max compression
```

## Comparing `ocsf_validator-0.1.7.tar` & `ocsf_validator-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    10173 2024-01-08 22:46:31.782602 ocsf_validator-0.1.7/LICENSE
--rw-r--r--   0        0        0     4209 2024-03-22 16:43:23.019386 ocsf_validator-0.1.7/README.md
--rw-r--r--   0        0        0      241 2024-01-08 22:46:31.762238 ocsf_validator-0.1.7/ocsf_validator/__init__.py
--rw-r--r--   0        0        0      584 2024-03-22 16:43:23.019731 ocsf_validator-0.1.7/ocsf_validator/__main__.py
--rw-r--r--   0        0        0     6728 2024-04-01 21:43:22.127009 ocsf_validator-0.1.7/ocsf_validator/errors.py
--rw-r--r--   0        0        0     2875 2024-01-08 22:46:31.766194 ocsf_validator-0.1.7/ocsf_validator/matchers.py
--rw-r--r--   0        0        0    16630 2024-03-22 16:43:23.020467 ocsf_validator-0.1.7/ocsf_validator/processor.py
--rw-r--r--   0        0        0     6956 2024-03-22 16:43:23.020718 ocsf_validator-0.1.7/ocsf_validator/reader.py
--rw-r--r--   0        0        0        0 2024-01-08 22:46:31.766272 ocsf_validator-0.1.7/ocsf_validator/repository.py
--rw-r--r--   0        0        0    12831 2024-03-22 16:43:23.020982 ocsf_validator-0.1.7/ocsf_validator/runner.py
--rw-r--r--   0        0        0     1641 2024-01-08 22:46:31.761487 ocsf_validator-0.1.7/ocsf_validator/type_mapping.py
--rw-r--r--   0        0        0     5080 2024-03-22 16:43:23.021178 ocsf_validator-0.1.7/ocsf_validator/types.py
--rw-r--r--   0        0        0    24002 2024-04-01 21:43:22.127216 ocsf_validator-0.1.7/ocsf_validator/validators.py
--rw-r--r--   0        0        0      594 2024-04-01 21:43:22.128038 ocsf_validator-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     4607 1970-01-01 00:00:00.000000 ocsf_validator-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    10173 2024-01-08 22:46:31.782602 ocsf_validator-0.1.9/LICENSE
+-rw-r--r--   0        0        0     4209 2024-03-22 16:43:23.019386 ocsf_validator-0.1.9/README.md
+-rw-r--r--   0        0        0      241 2024-01-08 22:46:31.762238 ocsf_validator-0.1.9/ocsf_validator/__init__.py
+-rw-r--r--   0        0        0      584 2024-03-22 16:43:23.019731 ocsf_validator-0.1.9/ocsf_validator/__main__.py
+-rw-r--r--   0        0        0     6728 2024-05-01 13:34:34.222601 ocsf_validator-0.1.9/ocsf_validator/errors.py
+-rw-r--r--   0        0        0     3184 2024-05-01 13:34:34.223463 ocsf_validator-0.1.9/ocsf_validator/matchers.py
+-rw-r--r--   0        0        0    16941 2024-05-01 13:34:34.224122 ocsf_validator-0.1.9/ocsf_validator/processor.py
+-rw-r--r--   0        0        0     6956 2024-03-22 16:43:23.020718 ocsf_validator-0.1.9/ocsf_validator/reader.py
+-rw-r--r--   0        0        0        0 2024-01-08 22:46:31.766272 ocsf_validator-0.1.9/ocsf_validator/repository.py
+-rw-r--r--   0        0        0    12859 2024-05-01 13:34:34.224698 ocsf_validator-0.1.9/ocsf_validator/runner.py
+-rw-r--r--   0        0        0     1647 2024-05-01 13:34:34.224869 ocsf_validator-0.1.9/ocsf_validator/type_mapping.py
+-rw-r--r--   0        0        0     5128 2024-05-01 13:34:34.225448 ocsf_validator-0.1.9/ocsf_validator/types.py
+-rw-r--r--   0        0        0    22446 2024-05-01 13:34:34.226368 ocsf_validator-0.1.9/ocsf_validator/validators.py
+-rw-r--r--   0        0        0      594 2024-05-01 13:34:34.226570 ocsf_validator-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     4607 1970-01-01 00:00:00.000000 ocsf_validator-0.1.9/PKG-INFO
```

### Comparing `ocsf_validator-0.1.7/LICENSE` & `ocsf_validator-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ocsf_validator-0.1.7/README.md` & `ocsf_validator-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `ocsf_validator-0.1.7/ocsf_validator/__main__.py` & `ocsf_validator-0.1.9/ocsf_validator/__main__.py`

 * *Files identical despite different names*

### Comparing `ocsf_validator-0.1.7/ocsf_validator/errors.py` & `ocsf_validator-0.1.9/ocsf_validator/errors.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,17 +192,17 @@
 class IncludeTypeMismatchError(ValidationError):
     def __init__(
         self, file: str, include: str, t: type | str, directive: str = "$include"
     ):
         self.file = file
         self.include = include
         if isinstance(t, str):
-            self.cls = t
+            self.cls: str = t
         else:
-            self.cls: str = t.__name__
+            self.cls = t.__name__
         self.directive = directive
         super().__init__(
             f"`{directive}` type mismatch in {file}: expected type `{self.cls}` for {include}"
         )
 
 
 class TypeNameCollisionError(ValidationError):
```

### Comparing `ocsf_validator-0.1.7/ocsf_validator/matchers.py` & `ocsf_validator-0.1.9/ocsf_validator/matchers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,22 @@
+from __future__ import annotations
+
 import re
-from abc import ABC
 from pathlib import Path
 from typing import Optional
 
 from ocsf_validator.types import *
 
 
 class Matcher:
     def match(self, value: str) -> bool:
         raise NotImplementedError()
 
     @staticmethod
-    def make(pattern):
+    def make(pattern) -> Matcher:
         if isinstance(pattern, Matcher):
             return pattern
         else:
             return RegexMatcher(pattern)
 
 
 class TypeMatcher:
@@ -117,7 +118,17 @@
 
 class CategoriesMatcher(RegexMatcher, TypeMatcher):
     def __init__(self):
         self._pattern = re.compile(r".*categories.json")
 
     def get_type(self):
         return OcsfCategories
+
+class ExcludeMatcher(Matcher):
+    """
+    A matcher that produces the opposite result of the matcher it's given.
+    """
+    def __init__(self, matcher: Matcher):
+        self.matcher = matcher
+
+    def match(self, value: str) -> bool:
+        return not self.matcher.match(value)
```

### Comparing `ocsf_validator-0.1.7/ocsf_validator/processor.py` & `ocsf_validator-0.1.9/ocsf_validator/processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 from pathlib import Path
 from typing import Any, Callable, Optional
 
 from ocsf_validator.errors import *
+from ocsf_validator.matchers import (
+    CategoriesMatcher,
+    ExcludeMatcher
+)
 from ocsf_validator.reader import Reader
 from ocsf_validator.type_mapping import TypeMapping
 from ocsf_validator.types import (
     ATTRIBUTES_KEY,
     EXTENDS_KEY,
     INCLUDE_KEY,
     PROFILES_KEY,
@@ -409,18 +413,18 @@
     def apply(self, path: str) -> None:
         self._parse_includes(self._reader[path], path, update=True, remove=False)
 
 
 class Dependencies:
     """A friendly list of dependencies."""
 
-    def __init__(self):
+    def __init__(self) -> None:
         self._dependencies: dict[str, list[tuple[str, str]]] = {}
 
-    def add(self, child: str, parent: str, label: str = ""):
+    def add(self, child: str, parent: str, label: str = "") -> None:
         if child not in self._dependencies:
             self._dependencies[child] = []
         self._dependencies[child].append((parent, label))
 
     def __iter__(self):
         return iter(self._dependencies)
 
@@ -458,15 +462,21 @@
         PROFILES_KEY: ProfilesParser(reader, resolver, collector, types),
         INCLUDE_KEY: IncludeParser(reader, resolver, collector, types),
         ATTRIBUTES_KEY: AttributesParser(reader, resolver, collector, types),
     }
     fulfilled: set[str] = set()
     dependencies = Dependencies()
 
-    for path in reader.match():
+    # categories cannot be extended with dependencies, and it causes problems
+    # if we try to include dictionary attributes in categories
+    matcher = ExcludeMatcher(
+        CategoriesMatcher()
+    )
+
+    for path in reader.match(matcher):
         for directive, parser in parsers.items():
             if parser.found_in(path):
                 for target in parser.extract_targets(path):
                     dependencies.add(path, target, directive)
 
     def process(path: str):
         if path not in fulfilled:
```

### Comparing `ocsf_validator-0.1.7/ocsf_validator/reader.py` & `ocsf_validator-0.1.9/ocsf_validator/reader.py`

 * *Files identical despite different names*

### Comparing `ocsf_validator-0.1.7/ocsf_validator/runner.py` & `ocsf_validator-0.1.9/ocsf_validator/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Validate OCSF Schema definitions.
 """
 
 import traceback
 from dataclasses import dataclass
 from enum import IntEnum
 from pathlib import Path
-from typing import Callable
+from typing import Callable, Optional
 
 from termcolor import colored
 
 import ocsf_validator.errors as errors
 from ocsf_validator.processor import process_includes
 from ocsf_validator.reader import FileReader, ReaderOptions
 from ocsf_validator.type_mapping import TypeMapping
@@ -38,15 +38,15 @@
 @dataclass
 class ValidatorOptions:
     """Configure validator behavior."""
 
     base_path: str = "."
     """The base path of the schema."""
 
-    metaschema_path: str = None
+    metaschema_path: Optional[str] = None
     """The path to the schema's metaschema."""
 
     extensions: bool = True
     """Include the contents of extensions."""
 
     strict: bool = False
     """When True, exit with a non-zero exit code when warnings are encountered."""
@@ -200,15 +200,15 @@
             case Severity.ERROR:
                 return self.txt_fail("ERROR")
             case Severity.FATAL:
                 return self.txt_crash("FATAL")
             case _:
                 return self.txt_emphasize("???")
 
-    def validate(self):
+    def validate(self) -> None:
         exit_code = 0
         messages: dict[str, dict[int, set[str]]] = {}
         collector = errors.Collector(throw=False)
 
         def test(label: str, code: Callable):
             failures: int = 0
             message = code()
```

### Comparing `ocsf_validator-0.1.7/ocsf_validator/type_mapping.py` & `ocsf_validator-0.1.9/ocsf_validator/type_mapping.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pathlib import Path
 
 from ocsf_validator.errors import Collector, UndetectableTypeError
 from ocsf_validator.matchers import *
 from ocsf_validator.reader import Reader
 from ocsf_validator.types import *
 
-MATCHERS = [
+MATCHERS: list = [
     VersionMatcher(),
     DictionaryMatcher(),
     CategoriesMatcher(),
     IncludeMatcher(),
     CategoriesMatcher(),
     ProfileMatcher(),
     ObjectMatcher(),
```

### Comparing `ocsf_validator-0.1.7/ocsf_validator/types.py` & `ocsf_validator-0.1.9/ocsf_validator/types.py`

 * *Files 18% similar despite different names*

```diff
@@ -109,28 +109,27 @@
     attributes: Dict[str, OcsfAttr]
     description: NotRequired[str]
     annotations: NotRequired[Dict[str, str]]
 
 
 class OcsfProfile(TypedDict):
     caption: str
-    caption: str
     description: str
     meta: str
     name: str
     attributes: Dict[str, OcsfAttr]
     annotations: NotRequired[Dict[str, str]]
 
 
 OcsfObject = TypedDict(
     "OcsfObject",
     {
-        "caption": str,
-        "description": str,
-        "name": str,
+        "caption": NotRequired[str],
+        "description": NotRequired[str],
+        "name": NotRequired[str],
         "attributes": Dict[str, OcsfAttr],
         "extends": NotRequired[Union[str, list[Optional[str]]]],
         "observable": NotRequired[int],
         "profiles": NotRequired[Sequence[str]],
         "constraints": NotRequired[Dict[str, Sequence[str]]],
         "observables": NotRequired[Dict[str, int]],
         "$include": NotRequired[Union[str, Sequence[str]]],
@@ -139,16 +138,16 @@
 )
 
 
 OcsfEvent = TypedDict(
     "OcsfEvent",
     {
         "attributes": Dict[str, OcsfAttr],
-        "caption": str,
-        "name": str,
+        "caption": NotRequired[str],
+        "name": NotRequired[str],
         "uid": NotRequired[int],
         "category": NotRequired[str],
         "description": NotRequired[str],
         "extends": NotRequired[Union[str, list[Optional[str]]]],
         "profiles": NotRequired[Sequence[str]],
         "associations": NotRequired[Dict[str, Sequence[str]]],
         "constraints": NotRequired[Dict[str, Sequence[str]]],
```

### Comparing `ocsf_validator-0.1.7/ocsf_validator/validators.py` & `ocsf_validator-0.1.9/ocsf_validator/validators.py`

 * *Files 11% similar despite different names*

```diff
@@ -249,29 +249,30 @@
     found: dict[str, dict[str, list[str]]] = {}
 
     def validate(reader: Reader, file: str):
         t = str(types[file])
         if t not in found:
             found[t] = {}
 
-        if "name" in reader[file]:
+        # The patch extends case _always_ has the the same name as its base
+        if "name" in reader[file] and not _is_patch_extends(reader[file]):
             name = reader[file]["name"]
             if name not in found[t]:
                 found[t][name] = []
             else:
                 collector.handle(
                     TypeNameCollisionError(name, t, file, found[t][name][0])
                 )
             found[t][name].append(file)
 
     reader.apply(validate, AnyMatcher([ObjectMatcher(), EventMatcher()]))
 
 
 def _default_get_registry(reader: Reader, base_uri: str) -> referencing.Registry:
-    registry = referencing.Registry()
+    registry: referencing.Registry = referencing.Registry()
     for schema_file_path in reader.metaschema_path.glob("*.schema.json"):
         with open(schema_file_path, "r") as file:
             schema = json.load(file)
             resource = referencing.Resource.from_contents(schema)
             registry = registry.with_resource(
                 base_uri + schema_file_path.name, resource=resource
             )
@@ -454,21 +455,21 @@
                 if OBSERVABLE_KEY in item:
                     check_collision(item[OBSERVABLE_KEY], name_fn(a_key, item), file)
 
     def validate_dictionaries(reader: Reader, file: str) -> None:
         if TYPES_KEY in reader[file]:
             check_attributes(
                 reader[file][TYPES_KEY],
-                lambda a_key, item: f"{item.get('caption')} (Dictionary Type)",
+                lambda a_key, item: f'"{a_key}" (Dictionary Type)',
                 file,
             )
 
         check_attributes(
             reader[file],
-            lambda a_key, item: f"{item.get('caption')} (Dictionary Attribute)",
+            lambda a_key, item: f'"{a_key}" (Dictionary Attribute)',
             file,
         )
 
     def validate_classes(reader: Reader, file: str) -> None:
         # Classes do not have top-level "observable" attribute -- you can't specify an
         # entire class as an observable.
 
@@ -497,47 +498,28 @@
                     f' "{file}": defining attribute path based observables in a hidden'
                     f' class (classes other than "base_event" without a "uid") causes'
                     f" collisions in child classes. Instead define observables (of any"
                     f" kind) in non-hidden child classes."
                 )
                 collector.handle(IllegalObservableTypeIDError(cause))
 
-        if _is_patch_extends(reader[file]):
-            if any_attribute_has_observable(reader[file]):
-                cause = (
-                    f"Illegal definition of one or more attributes with"
-                    f' "{OBSERVABLE_KEY}" in patch extends class, file "{file}":'
-                    f" observable definitions in patch extends are not supported."
-                    f" Please file an issue if you find this feature necessary."
-                )
-                collector.handle(IllegalObservableTypeIDError(cause))
-
-            if OBSERVABLES_KEY in reader[file]:
-                cause = (
-                    f'Illegal "{OBSERVABLES_KEY}" definition in patch extends class,'
-                    f' file "{file}": observable definitions in patch extends are not.'
-                    f" supported. Please file an issue if you find this feature"
-                    f" necessary."
-                )
-                collector.handle(IllegalObservableTypeIDError(cause))
-
         # Check class-specific attributes
         check_attributes(
             reader[file],
-            lambda a_key, item: f"{reader[file].get('caption')} Class: {a_key}"
+            lambda a_key, item: f"{_item_name(reader[file])} class: {a_key}"
             f" (Class-Specific Attribute)",
             file,
         )
 
         # Check class-specific attribute path observables
         if OBSERVABLES_KEY in reader[file]:
             for attribute_path in reader[file][OBSERVABLES_KEY]:
                 check_collision(
                     reader[file][OBSERVABLES_KEY][attribute_path],
-                    f"{reader[file]['caption']} Class: {attribute_path}"
+                    f"{_item_name(reader[file])} class: {attribute_path}"
                     f" (Class-Specific Attribute Path)",
                     file,
                 )
 
     def validate_objects(reader: Reader, file: str) -> None:
         # Special-case: the "observable" object model's type_id enum has the base for
         # observable type_id typically defining 0: "Unknown" and 99: "Other", which are
@@ -577,56 +559,51 @@
                     f' "{OBSERVABLE_KEY}" in hidden object, file "{file}": defining'
                     f" attribute observables in a hidden object (name with leading"
                     f" underscore) causes collisions in child objects. Instead define"
                     f" observables (of any kind) in non-hidden child objects."
                 )
                 collector.handle(IllegalObservableTypeIDError(cause))
 
-        if _is_patch_extends(reader[file]):
-            if any_attribute_has_observable(reader[file]):
-                cause = (
-                    f"Illegal definition of one or more attributes with"
-                    f' "{OBSERVABLE_KEY}" in patch extends object, file "{file}":'
-                    f" observable definitions in patch extends are not supported."
-                    f" Please file an issue if you find this feature necessary."
-                )
-                collector.handle(IllegalObservableTypeIDError(cause))
-
-            if OBSERVABLE_KEY in reader[file]:
-                cause = (
-                    f'Illegal "{OBSERVABLE_KEY}" definition in patch extends object,'
-                    f' file "{file}": observable definitions in patch extends are not.'
-                    f" supported. Please file an issue if you find this feature"
-                    f" necessary."
-                )
-                collector.handle(IllegalObservableTypeIDError(cause))
-
         # Check top-level observable -- entire object is an observable
         if OBSERVABLE_KEY in reader[file]:
             check_collision(
                 reader[file][OBSERVABLE_KEY],
-                f"{reader[file].get('caption')} (Object)",
+                f"{_item_name(reader[file])} (Object)",
                 file,
             )
 
         # Check object-specific attributes
         check_attributes(
             reader[file],
-            lambda a_key, item: f"{reader[file].get('caption')} Object: {a_key}"
+            lambda a_key, item: f"{_item_name(reader[file])} object: {a_key}"
             f" (Object-Specific Attribute)",
             file,
         )
 
     reader.apply(validate_dictionaries, DictionaryMatcher())
     reader.apply(validate_classes, EventMatcher())
     reader.apply(validate_objects, ObjectMatcher())
 
     return observables
 
 
+def _item_name(item):
+    if _is_patch_extends(item):
+        suffix = " [patch extends]"
+    else:
+        suffix = ""
+    name = item.get("name")
+    if name:
+        return f'"{name}"{suffix}'
+    extends = item.get("extends")
+    if extends:
+        return f'"{extends}"{suffix}'
+    return f"<unknown>{suffix}"
+
+
 def _is_patch_extends(item):
     """
     Returns True if class or object is a "special" patch extends, which allows
     extensions to modify core schema classes and objects.
     """
     name = item.get("name")
     if name is None:
```

### Comparing `ocsf_validator-0.1.7/pyproject.toml` & `ocsf_validator-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ocsf-validator"
-version = "0.1.7"
+version = "0.1.9"
 description = "OCSF Schema Validation"
 authors = [
     "Jeremy Fisher <jeremy@query.ai>",
     "Alan Pinkert <apinkert@cisco.com>",
     "Rick Mouritzen <rmouritzen@splunk.com>",
 ]
 readme = "README.md"
```

### Comparing `ocsf_validator-0.1.7/PKG-INFO` & `ocsf_validator-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocsf-validator
-Version: 0.1.7
+Version: 0.1.9
 Summary: OCSF Schema Validation
 Author: Jeremy Fisher
 Author-email: jeremy@query.ai
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: jsonschema (>=4.21.1,<5.0.0)
```

