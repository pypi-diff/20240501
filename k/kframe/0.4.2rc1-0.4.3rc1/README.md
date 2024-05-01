# Comparing `tmp/kframe-0.4.2rc1.tar.gz` & `tmp/kframe-0.4.3rc1.tar.gz`

## Comparing `kframe-0.4.2rc1.tar` & `kframe-0.4.3rc1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 kframe-0.4.2rc1/.pre-commit-config.yaml
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 kframe-0.4.2rc1/.tool-versions
--rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 kframe-0.4.2rc1/CHANGELOG.md
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 kframe-0.4.2rc1/.github/workflows/main_ci.yml
--rw-r--r--   0        0        0     4086 2020-02-02 00:00:00.000000 kframe-0.4.2rc1/.github/workflows/main_pre_release.yml
--rw-r--r--   0        0        0     4042 2020-02-02 00:00:00.000000 kframe-0.4.2rc1/.github/workflows/main_release.yml
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 kframe-0.4.2rc1/src/kframe/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kframe-0.4.2rc1/src/kframe/__init__.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 kframe-0.4.2rc1/src/kframe/config/__init__.py
--rw-r--r--   0        0        0     5775 2020-02-02 00:00:00.000000 kframe-0.4.2rc1/src/kframe/config/configattr.py
--rw-r--r--   0        0        0     8259 2020-02-02 00:00:00.000000 kframe-0.4.2rc1/src/kframe/config/configentity.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 kframe-0.4.2rc1/tests/__init__.py
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 kframe-0.4.2rc1/tests/test_secretattr.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 kframe-0.4.2rc1/.gitignore
--rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 kframe-0.4.2rc1/LICENSE.txt
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 kframe-0.4.2rc1/README.md
--rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 kframe-0.4.2rc1/pyproject.toml
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 kframe-0.4.2rc1/PKG-INFO
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 kframe-0.4.3rc1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 kframe-0.4.3rc1/.tool-versions
+-rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 kframe-0.4.3rc1/CHANGELOG.md
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 kframe-0.4.3rc1/.github/workflows/main_ci.yml
+-rw-r--r--   0        0        0     4086 2020-02-02 00:00:00.000000 kframe-0.4.3rc1/.github/workflows/main_pre_release.yml
+-rw-r--r--   0        0        0     4042 2020-02-02 00:00:00.000000 kframe-0.4.3rc1/.github/workflows/main_release.yml
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 kframe-0.4.3rc1/src/kframe/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kframe-0.4.3rc1/src/kframe/__init__.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 kframe-0.4.3rc1/src/kframe/config/__init__.py
+-rw-r--r--   0        0        0     6048 2020-02-02 00:00:00.000000 kframe-0.4.3rc1/src/kframe/config/configattr.py
+-rw-r--r--   0        0        0    10496 2020-02-02 00:00:00.000000 kframe-0.4.3rc1/src/kframe/config/configentity.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 kframe-0.4.3rc1/tests/__init__.py
+-rw-r--r--   0        0        0     4481 2020-02-02 00:00:00.000000 kframe-0.4.3rc1/tests/test_config.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 kframe-0.4.3rc1/tests/test_secretattr.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 kframe-0.4.3rc1/.gitignore
+-rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 kframe-0.4.3rc1/LICENSE.txt
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 kframe-0.4.3rc1/README.md
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 kframe-0.4.3rc1/pyproject.toml
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 kframe-0.4.3rc1/PKG-INFO
```

### Comparing `kframe-0.4.2rc1/CHANGELOG.md` & `kframe-0.4.3rc1/CHANGELOG.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+## v0.4.3a1 (2024-05-01)
+
+### Fix
+
+- Update CLI argument help message in ConfigAttr class to show required and env_var
+- Update .gitignore and pyproject.toml
+
+### Refactor
+
+- Remove parse_args and include load method to ConfigEntity
+
+## v0.4.2 (2024-05-01)
+
+## v0.4.2rc1 (2024-05-01)
+
 ## v0.4.2a1 (2024-05-01)
 
 ### Fix
 
 - Update README.md: Remove empty lines
 
 ## v0.4.1 (2024-05-01)
```

### Comparing `kframe-0.4.2rc1/.github/workflows/main_ci.yml` & `kframe-0.4.3rc1/.github/workflows/main_ci.yml`

 * *Files identical despite different names*

### Comparing `kframe-0.4.2rc1/.github/workflows/main_pre_release.yml` & `kframe-0.4.3rc1/.github/workflows/main_pre_release.yml`

 * *Files identical despite different names*

### Comparing `kframe-0.4.2rc1/.github/workflows/main_release.yml` & `kframe-0.4.3rc1/.github/workflows/main_release.yml`

 * *Files identical despite different names*

### Comparing `kframe-0.4.2rc1/src/kframe/config/configattr.py` & `kframe-0.4.3rc1/src/kframe/config/configattr.py`

 * *Files 3% similar despite different names*

```diff
@@ -128,15 +128,22 @@
         """Return the environment variable for the attribute."""
         return getattr(self, "_env_var", None)
 
     @property
     def cli_args(self):
         """Return the CLI arguments for the attribute."""
         if self._cli_args is not None:
-            attrs = {"help": self.description, "dest": self._name}
+            desc_attrs = []
+            if self.required:
+                desc_attrs.append("required")
+            if self.env_var is not None:
+                desc_attrs.append(f"env: {self.env_var}")
+            description = f"{self.description} ({', '.join(desc_attrs)})"
+
+            attrs = {"help": description, "dest": self._name}
             if self.attr_type is bool:
                 attrs |= {"action": "store_const", "const": True}
             return (self._cli_args, attrs)
         return None
 
     @property
     def required(self):
```

### Comparing `kframe-0.4.2rc1/src/kframe/config/configentity.py` & `kframe-0.4.3rc1/src/kframe/config/configentity.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+import logging
 import os
 import sys
-from argparse import ArgumentParser, Namespace
+from argparse import ArgumentError, ArgumentParser, ArgumentTypeError, Namespace
 from collections import ChainMap
 from enum import Enum
 
 from .configattr import ConfigAttr, Secret
 
+logger = logging.getLogger("kframe.config")
+
 
 class ConfigEntityType(Enum):
     base = "base"
     module = "Module"
     command = "Command"
 
 
@@ -18,14 +21,16 @@
     _submodules: set
     _attribute_names: set
     _sources: ChainMap
     show_config: ConfigAttr
     attr: Namespace
     attrs: dict[str, ConfigAttr]
     entity_type: ConfigEntityType
+    parent_module: "ConfigEntity"
+    root_module: "ConfigEntity"
 
     def show(cls, file=sys.stdout):
         """Prints entity configuration"""
 
     def __new__(cls, _name, bases, dct, name=None, parent_entity=None, description=None):
         sources = {}
 
@@ -39,14 +44,23 @@
                 v._name = k
                 sources[k] = {"default": Secret[v.attr_type](v.default_value) if v.secret else v.default_value}
                 v.__doc__ = v.description
 
                 if v.env_var is not None and v.env_var in os.environ:
                     sources[k]["env"] = Secret[v.attr_type](v.env_var) if v.secret else os.environ[v.env_var]
 
+                if (
+                    v.cli_args is None
+                    and v.required
+                    and v.default_value is None
+                    and isinstance(v.env_var, str)
+                    and os.getenv(v.env_var) is None
+                ):
+                    raise AttributeError(f"Required attribute {v} must have a default value or environment variable")
+
         dct["_sources"] = ChainMap(sources, dct["_sources"])
         dct["_commands"] = set()
         dct["_submodules"] = set()
 
         dct["_attribute_names"] = {k for k, v in dct.items() if isinstance(v, ConfigAttr)}
 
         attr = {k: dct[k] for k in dct["_attribute_names"]}
@@ -55,60 +69,59 @@
             """Entity attributes"""
             return attr
 
         dct["attr"] = property(lambda self: Namespace(**attr), doc="Entity attributes namespace")
         dct["attrs"] = property(attrs, doc="Entity attributes dictionary")
         dct["namespace"] = property(lambda self: ".".join(dct["_namespace"]), doc="Entity namespace")
 
-        dct["parent_module"] = property(lambda self: parent_entity, doc=f"{dct['type'].value} parent module ")
+        dct["parent_module"] = property(lambda self: parent_entity, doc=f"{dct['entity_type'].value} parent module ")
 
         def run(self):
             """Execute command"""
             self.execute()
 
-        if dct["type"] == ConfigEntityType.command:
+        if dct["entity_type"] == ConfigEntityType.command:
             if "__call__" in dct:
                 raise AttributeError("Command class cannot have __call__ method")
             dct["__call__"] = run
 
         new_cls = super().__new__(cls, _name, bases, dct)
         if parent_entity is not None:
-            # if new_cls.type == AppModuleType.command:
             if new_cls.entity_type == ConfigEntityType.module:
                 parent_entity._submodules.add(new_cls)
             if new_cls.entity_type == ConfigEntityType.command:
                 parent_entity._commands.add(new_cls)
         elif len(bases) > 0:
             bases[0].root_module = new_cls
 
         return new_cls
 
     def __prepare__(cls, bases, name=None, parent_entity=None, description=None):  # noqa: PLW3201
         match len(bases):
             case 0:
-                type_ = ConfigEntityType.base
+                entity_type = ConfigEntityType.base
             case 1:
                 match bases[0].__name__:
                     case "AppModule":
-                        type_ = ConfigEntityType.module
+                        entity_type = ConfigEntityType.module
                     case "AppCommand":
-                        type_ = ConfigEntityType.command
+                        entity_type = ConfigEntityType.command
                     case _:
                         raise AttributeError("Entity parent class must be AppModule or AppCommand")
             case _:
                 raise AttributeError("Command inheritance is not permitted, only one base class is allowed")
 
         dct = {
             "__name__": (name or cls).casefold(),
-            "type": type_,
+            "entity_type": entity_type,
         }
 
-        if type_ is ConfigEntityType.base:
+        if entity_type is ConfigEntityType.base:
             return dct | {
-                "__doc__": f"{type_.value.title()} base module",
+                "__doc__": f"{entity_type.value.title()} base module",
                 "_sources": ChainMap({}),
                 "_namespace": [],
             }
 
         dct |= {
             "__doc__": description or f"<{name or cls}> implementation",
             "_sources": parent_entity._sources if parent_entity is not None else ChainMap({}),
@@ -118,16 +131,80 @@
         if parent_entity is not None:
             dct["_namespace"] = (parent_entity._namespace or []) + dct["_namespace"]
             for k in parent_entity._sources:
                 if k not in dct:
                     dct[k] = parent_entity.__dict__[k]
         return dct
 
+    def load(
+        cls,
+        get_command: bool = True,
+        require_command: bool = False,
+        show_parser_help: bool = True,
+    ):
+        logger.debug("Loading %s", cls.__name__)
+
+        if cls.entity_type == ConfigEntityType.module:
+            base = cls.root_module
+        elif cls.entity_type == ConfigEntityType.command:
+            base = cls().parent_module.root_module
+        else:
+            base = None
+
+        if base is None:
+            raise AttributeError("Entity must have a base module")
+
+        arg_parser = build_parser(base)
+        try:
+            args = vars(arg_parser.parse_known_args()[0])
+        except (ArgumentError, ArgumentTypeError):
+            logger.exception("Error parsing arguments")
+            if show_parser_help:
+                arg_parser.print_help()
+
+        current_cls = cls()
+        while current_cls is not None:
+            logger.debug("Loading environment variables for %s: %s", current_cls.__name__, current_cls.attrs.keys())
+            for k, attr in current_cls.attrs.items():
+                if attr.cli_args is not None and attr.name in args and args[attr.name] is not None:
+                    current_cls._sources[k]["cli"] = (
+                        Secret[attr.attr_type](args[attr.name]) if attr.secret else args[attr.name]  # type: ignore
+                    )
+            current_cls = current_cls.parent_module() if current_cls.parent_module is not None else None
+
+        logger.debug("Sources for %s: %s", cls.__name__, cls._sources)
+
+        if get_command or require_command:
+            i = 0
+            current_cls = base()
+            while f"__level_{i}" in args and args[f"__level_{i}"] is not None:
+                entity_name = args[f"__level_{i}"]
+                for child in current_cls._submodules.union(current_cls._commands):
+                    if child().__name__ == entity_name:
+                        current_cls = child()
+                        break
+                i += 1
+            logger.debug("Highest level class found: %s", current_cls.__name__)
+
+            if require_command and current_cls.entity_type != ConfigEntityType.command:
+                if show_parser_help:
+                    arg_parser.print_help()
+                else:
+                    raise AttributeError("Command not found in CLI arguments")
+
+            if get_command and current_cls.entity_type == ConfigEntityType.command:
+                current_cls.__class__.load(get_command=False)
+                return current_cls
+
+        return None
+
 
 class AppCommand(metaclass=ConfigEntity):
+    root_module: "AppModule"
+
     show_config = ConfigAttr(
         default=False,
         description="Show configuration",
         cli_args=["--show-config"],
         attr_type=bool,
     )
 
@@ -166,66 +243,41 @@
 
         file.write("\nSubmodules:")
         for f in self._submodules:
             file.write(f"\n  * {f.__name__}")
         file.write("\n\n")
 
 
-def parse_args(entity: ConfigEntity = AppModule, level=0, arg_parser=None):
-    if entity is AppModule:
-        if entity().root_module is None:
-            raise AttributeError("Root module not set")
-        entity = entity().root_module()
+def build_parser(entity: ConfigEntity = AppModule, level=0, arg_parser=None):
+    _entity = entity()
+
+    if _entity.entity_type is ConfigEntityType.module and entity is entity.root_module:
+        logger.debug("Building parser for %s", entity.__name__)
         arg_parser = ArgumentParser(sys.argv[0], description=entity.__doc__)
-    else:
-        entity = entity()
 
-    for attr in entity._attribute_names:
-        if getattr(entity.attr, attr).cli_args is not None:
+    logger.debug("Adding arguments for %s", entity.__name__)
+
+    logger.debug(arg_parser)
+    for attr in _entity._attribute_names:
+        logger.debug("Adding argument %s to %s", attr, _entity.__name__)
+        logger.debug(_entity.attr)
+        if getattr(_entity.attr, attr).cli_args is not None:
             arg_parser.add_argument(
-                *getattr(entity.attr, attr).cli_args[0],
-                **getattr(entity.attr, attr).cli_args[1],
+                *getattr(_entity.attr, attr).cli_args[0],
+                **getattr(_entity.attr, attr).cli_args[1],
             )
 
     if len(entity._submodules) + len(entity._commands) > 0:
         subparsers = arg_parser.add_subparsers(metavar="", dest=f"__level_{level}", help="Commands and submodules")
 
     for module in entity._submodules:
         subparser = subparsers.add_parser(module().__name__, help=module.__doc__)
-        parse_args(module, level + 1, arg_parser=subparser)
+        build_parser(module, level + 1, arg_parser=subparser)
 
     for command in entity._commands:
         subparser = subparsers.add_parser(command().__name__, help=command.__doc__)
-        parse_args(command, level + 1, arg_parser=subparser)
-
-    if level == 0:
-        args = vars(arg_parser.parse_args())
-
-        command = None
-        i = 0
-        while f"__level_{i}" in args and args[f"__level_{i}"] is not None:
-            entity_name = args[f"__level_{i}"]
-            for child in entity._submodules.union(entity._commands):
-                if child().__name__ == entity_name:
-                    entity = child()
-                    break
-            i += 1
-
-        if entity.entity_type == ConfigEntityType.command:
-            for k, attr in entity.attrs.items():
-                if k in args and args[k] is not None:
-                    entity._sources[k]["cli"] = (
-                        Secret[attr.attr_type](args[k]) if attr.secret else args[k]  # type: ignore
-                    )
-                if attr.required and getattr(entity, k) is None:
-                    raise AttributeError(f"Required attribute {attr} not set")
-            runner = entity
-            command = entity.__name__
-        else:
-            arg_parser.print_help()
-
-        if entity.show_config:
-            entity.show()
+        build_parser(command, level + 1, arg_parser=subparser)
 
-        return runner, command
+    if level > 0:
+        return None
 
-    return None
+    return arg_parser
```

### Comparing `kframe-0.4.2rc1/tests/test_secretattr.py` & `kframe-0.4.3rc1/tests/test_secretattr.py`

 * *Files identical despite different names*

### Comparing `kframe-0.4.2rc1/LICENSE.txt` & `kframe-0.4.3rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kframe-0.4.2rc1/README.md` & `kframe-0.4.3rc1/README.md`

 * *Files identical despite different names*

### Comparing `kframe-0.4.2rc1/pyproject.toml` & `kframe-0.4.3rc1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "kframe"
-version = "0.4.2rc1"
+version = "0.4.3rc1"
 description = 'Kaeus development framework'
 readme = "README.md"
 requires-python = ">=3.10"
 license = "MS-PL"
 keywords = []
 authors = [
   { name = "Sebastian Garcia", email = "sgarcia@kaeusanalytics.com" },
@@ -30,14 +30,15 @@
 # TODO: Update these URLs
 Documentation = "https://github.com/kaeus-sgarcia/kframe#readme"
 Issues = "https://github.com/kaeus-sgarcia/kframe/issues"
 Source = "https://github.com/kaeus-sgarcia/kframe"
 
 # Development environment
 [tool.hatch.envs.default]
+python = "3.10"
 dependencies = [
   "coverage[toml]>=6.5",
   "pytest",
   "ruff",
   "pre-commit",
   "commitizen",
 ]
@@ -48,16 +49,15 @@
   "- coverage combine",
   "coverage report",
 ]
 cov = [
   "test-cov",
   "cov-report",
 ]
-check = "ruff check --fix"
-preview-version = "semantic-release version --print"
+
 
 [tool.hatch.envs.quality]
 dependencies = [
   "coverage[toml]>=6.5",
   "pytest",
 ]
 
@@ -79,15 +79,15 @@
 branch = true
 parallel = true
 omit = [
   "src/kframe/__about__.py",
 ]
 
 [tool.coverage.paths]
-kframe = ["src/kframe"]
+kframe = ["src/kframe", "*/kframe/src/kframe"]
 tests = ["tests", "*/kframe/tests"]
 
 [tool.coverage.report]
 exclude_lines = [
   "no cov",
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
```

### Comparing `kframe-0.4.2rc1/PKG-INFO` & `kframe-0.4.3rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: kframe
-Version: 0.4.2rc1
+Version: 0.4.3rc1
 Summary: Kaeus development framework
 Project-URL: Documentation, https://github.com/kaeus-sgarcia/kframe#readme
 Project-URL: Issues, https://github.com/kaeus-sgarcia/kframe/issues
 Project-URL: Source, https://github.com/kaeus-sgarcia/kframe
 Author-email: Sebastian Garcia <sgarcia@kaeusanalytics.com>
 License-Expression: MS-PL
 License-File: LICENSE.txt
```

