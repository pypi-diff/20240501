# Comparing `tmp/tool2schema-2.0.0.tar.gz` & `tmp/tool2schema-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tool2schema-2.0.0.tar", max compression
+gzip compressed data, was "tool2schema-2.1.0.tar", max compression
```

## Comparing `tool2schema-2.0.0.tar` & `tool2schema-2.1.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11338 2024-04-30 21:06:23.446210 tool2schema-2.0.0/LICENSE
--rw-r--r--   0        0        0     9157 2024-04-30 21:06:23.446210 tool2schema-2.0.0/README.md
--rw-r--r--   0        0        0      886 2024-04-30 21:06:31.730218 tool2schema-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      378 2024-04-30 21:06:31.730218 tool2schema-2.0.0/tool2schema/__init__.py
--rw-r--r--   0        0        0     3478 2024-04-30 21:06:23.450210 tool2schema-2.0.0/tool2schema/config.py
--rw-r--r--   0        0        0     3865 2024-04-30 21:06:23.450210 tool2schema-2.0.0/tool2schema/parameter_schema.py
--rw-r--r--   0        0        0    15237 2024-04-30 21:06:23.450210 tool2schema-2.0.0/tool2schema/schema.py
--rw-r--r--   0        0        0     9449 2024-04-30 21:06:23.450210 tool2schema-2.0.0/tool2schema/type_schema.py
--rw-r--r--   0        0        0     9890 1970-01-01 00:00:00.000000 tool2schema-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11338 2024-05-01 17:19:03.810756 tool2schema-2.1.0/LICENSE
+-rw-r--r--   0        0        0     9157 2024-05-01 17:19:03.810756 tool2schema-2.1.0/README.md
+-rw-r--r--   0        0        0      835 2024-05-01 17:19:11.474845 tool2schema-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0      378 2024-05-01 17:19:11.470845 tool2schema-2.1.0/tool2schema/__init__.py
+-rw-r--r--   0        0        0     4243 2024-05-01 17:19:03.810756 tool2schema-2.1.0/tool2schema/config.py
+-rw-r--r--   0        0        0     3949 2024-05-01 17:19:03.810756 tool2schema-2.1.0/tool2schema/parameter_schema.py
+-rw-r--r--   0        0        0    15480 2024-05-01 17:19:03.810756 tool2schema-2.1.0/tool2schema/schema.py
+-rw-r--r--   0        0        0     9670 2024-05-01 17:19:03.810756 tool2schema-2.1.0/tool2schema/type_schema.py
+-rw-r--r--   0        0        0     9896 1970-01-01 00:00:00.000000 tool2schema-2.1.0/PKG-INFO
```

### Comparing `tool2schema-2.0.0/LICENSE` & `tool2schema-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tool2schema-2.0.0/README.md` & `tool2schema-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `tool2schema-2.0.0/pyproject.toml` & `tool2schema-2.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -8,22 +8,19 @@
 
 [tool.pyright]
 include = ["tool2schema"]
 reportMissingImports = true
 reportMissingModuleSource = false
 pythonVersion = "3.11"
 pythonPlatform = "Windows"
-executionEnvironments = [
-    { root = "tool2schema" }
-]
 
 [tool.poetry]
 name = "tool2schema"
-version = "v2.0.0"
-description = "A library to generate function schemas for use in the OpenAI API."
+version = "v2.1.0"
+description = "A library to generate function schemas for use in LLM function calling."
 authors = ["Angus Stewart <siliconlad@protonmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository="https://github.com/cadifyai/tool2schema"
 keywords=["openai", "llm"]
 
 [tool.poetry.dependencies]
```

### Comparing `tool2schema-2.0.0/tool2schema/config.py` & `tool2schema-2.1.0/tool2schema/config.py`

 * *Files 24% similar despite different names*

```diff
@@ -24,63 +24,83 @@
         self._initial_settings = copy.deepcopy(settings)
 
     @property
     def schema_type(self) -> SchemaType:
         """
         Type of the schema to create.
         """
-        return self._get_setting(Config.schema_type.fget.__name__, SchemaType.OPENAI_API)
+        default_value = SchemaType.OPENAI_API
+        if (fget := Config.schema_type.fget) is not None:
+            return self._get_setting(fget.__name__, default_value)
+        return default_value
 
     @schema_type.setter
     def schema_type(self, value: SchemaType):
-        self._set_setting(Config.schema_type.fget.__name__, value)
+        if (fget := Config.schema_type.fget) is not None:
+            self._set_setting(fget.__name__, value)
 
     @property
     def ignore_parameters(self) -> list[str]:
         """
         List of parameter names to ignore when creating a schema.
         """
-        return self._get_setting(Config.ignore_parameters.fget.__name__, ["self", "args", "kwargs"])
+        default_value = ["self", "args", "kwargs"]
+        if (fget := Config.ignore_parameters.fget) is not None:
+            return self._get_setting(fget.__name__, default_value)
+        return default_value
 
     @ignore_parameters.setter
     def ignore_parameters(self, value: list[str]):
-        self._set_setting(Config.ignore_parameters.fget.__name__, value)
+        if (fget := Config.ignore_parameters.fget) is not None:
+            self._set_setting(fget.__name__, value)
 
     @property
     def ignore_function_description(self) -> bool:
         """
         When true, omit the function description from the schema.
         """
-        return self._get_setting(Config.ignore_function_description.fget.__name__, False)
+        default_value = False
+        if (fget := Config.ignore_function_description.fget) is not None:
+            return self._get_setting(fget.__name__, default_value)
+        return default_value
 
     @ignore_function_description.setter
     def ignore_function_description(self, value: bool):
-        self._set_setting(Config.ignore_function_description.fget.__name__, value)
+        if (fget := Config.ignore_function_description.fget) is not None:
+            self._set_setting(fget.__name__, value)
 
     @property
     def ignore_parameter_descriptions(self) -> bool:
         """
         When true, omit the parameter descriptions from the schema.
         """
-        return self._get_setting(Config.ignore_parameter_descriptions.fget.__name__, False)
+        default_value = False
+        if (fget := Config.ignore_parameter_descriptions.fget) is not None:
+            return self._get_setting(fget.__name__, default_value)
+        return default_value
 
     @ignore_parameter_descriptions.setter
     def ignore_parameter_descriptions(self, value: bool):
-        self._set_setting(Config.ignore_parameter_descriptions.fget.__name__, value)
+        if (fget := Config.ignore_parameter_descriptions.fget) is not None:
+            self._set_setting(fget.__name__, value)
 
     @property
     def ignore_all_parameters(self) -> bool:
         """
         When true, omit all parameters from the schema.
         """
-        return self._get_setting(Config.ignore_all_parameters.fget.__name__, False)
+        default_value = False
+        if (fget := Config.ignore_all_parameters.fget) is not None:
+            return self._get_setting(fget.__name__, default_value)
+        return default_value
 
     @ignore_all_parameters.setter
     def ignore_all_parameters(self, value: bool):
-        self._set_setting(Config.ignore_all_parameters.fget.__name__, value)
+        if (fget := Config.ignore_all_parameters.fget) is not None:
+            self._set_setting(fget.__name__, value)
 
     def reset_default(self):
         """
         Reset the configuration to the default settings.
         """
         self._settings = copy.deepcopy(self._initial_settings)
```

### Comparing `tool2schema-2.0.0/tool2schema/parameter_schema.py` & `tool2schema-2.1.0/tool2schema/parameter_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,18 @@
         :param config: Configuration settings to use when creating the schema
         :param docstring: The docstring for the function containing the parameter
         :return: An instance of `ParameterSchema`, or None if the parameter type is not supported.
         """
         if type_schema := TypeSchema.create(parameter.annotation):
             return ParameterSchema(type_schema, parameter, index, config, docstring)
 
-    def _get_description(self) -> Union[str, Parameter.empty]:
+    def _test(self) -> type[Parameter.empty]:
+        return Parameter.empty
+
+    def _get_description(self) -> Union[str, type[Parameter.empty]]:
         """
         Get the description of this parameter, extracted from the function docstring,
         to be added to the JSON schema. Return `Parameter.empty` to omit the description
         from the schema.
         """
         if self.docstring is None or self.config.ignore_parameter_descriptions:
             return Parameter.empty
```

### Comparing `tool2schema-2.0.0/tool2schema/schema.py` & `tool2schema-2.1.0/tool2schema/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import functools
 import inspect
 import json
 import re
 import sys
 from inspect import Parameter
 from types import ModuleType
-from typing import Any, Callable, Generic, Optional, TypeVar, overload
+from typing import Any, Callable, Generic, Literal, Optional, TypeVar, Union, overload
 
 import tool2schema
 from tool2schema.config import Config, SchemaType
 from tool2schema.parameter_schema import ParameterSchema
 
 if sys.version_info < (3, 10):
     from typing_extensions import ParamSpec
@@ -44,14 +44,15 @@
 def FindToolEnabledByName(module: ModuleType, name: str) -> Optional[ToolEnabled]:
     """
     Find a function with the EnableTool decorator by name.
 
     :param module: Module to search for ToolEnabled functions
     :param name: Name of the function to find
     """
+    func: ToolEnabled
     for func in FindToolEnabled(module):
         if func.__name__ == name:
             return func
     return None
 
 
 def FindToolEnabledByNameSchema(
@@ -220,32 +221,33 @@
 
 class ToolEnabled(Generic[P, T]):
     def __init__(self, func: Callable[P, T], **kwargs) -> None:
         self.func = func
         self.tags = kwargs.pop("tags", [])
         self.config = Config(tool2schema.CONFIG, **kwargs)
         self.schema = FunctionSchema(func, self.config)
+        self.__name__ = func.__name__
         functools.update_wrapper(self, func)
 
     def __call__(self, *args: P.args, **kwargs: P.kwargs) -> T:
 
-        args = list(args)  # Tuple is immutable, thus convert to list
+        args_list = list(args)  # Tuple is immutable, thus convert to list
 
-        for i, arg in enumerate(args):
+        for i, arg in enumerate(args_list):
             for p in self.schema.parameter_schemas.values():
                 if p.index == i:
                     # Convert the JSON value to the type expected by the method
-                    args[i] = p.type_schema.decode(arg)
+                    args_list[i] = p.type_schema.decode(arg)
 
         for key in kwargs:
             if key in self.schema.parameter_schemas:
                 # Convert the JSON value to the type expected by the method
                 kwargs[key] = self.schema.parameter_schemas[key].type_schema.decode(kwargs[key])
 
-        return self.func(*args, **kwargs)
+        return self.func(*args_list, **kwargs)  # type: ignore
 
     def tool_enabled(self) -> bool:
         return True
 
     def to_json(self, schema_type: Optional[SchemaType] = None) -> dict:
         """
         Return JSON schema for the function.
@@ -260,18 +262,18 @@
 
 
 @overload
 def EnableTool(func: Callable[P, T], **kwargs) -> ToolEnabled[P, T]: ...
 
 
 @overload
-def EnableTool(**kwargs) -> Callable[[Callable[P, T]], ToolEnabled[P, T]]: ...
+def EnableTool(func: Literal[None] = None, **kwargs) -> Callable[[Callable[P, T]], ToolEnabled[P, T]]: ...
 
 
-def EnableTool(func=None, **kwargs):
+def EnableTool(func: Optional[Callable[P, T]] = None, **kwargs) -> Union[ToolEnabled[P, T], Callable[[Callable[P, T]], ToolEnabled[P, T]]]:
     """Decorator to generate a function schema for OpenAI."""
     if func is not None:
         return ToolEnabled(func, **kwargs)
     else:
 
         def wrapper(function: Callable[P, T]) -> ToolEnabled[P, T]:
             return ToolEnabled(function, **kwargs)
```

### Comparing `tool2schema-2.0.0/tool2schema/type_schema.py` & `tool2schema-2.1.0/tool2schema/type_schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,22 +89,22 @@
 
     def _get_type(self) -> dict:
         """
         Get the type dictionary to be merged in the JSON schema.
         """
         return {}
 
-    def _get_items(self) -> Union[dict, Parameter.empty]:
+    def _get_items(self) -> Union[dict, type[Parameter.empty]]:
         """
         Get the items property to be added to the JSON schema.
         Return `Parameter.empty` to omit the items from the schema.
         """
         return Parameter.empty
 
-    def _get_enum(self) -> Union[list, Parameter.empty]:
+    def _get_enum(self) -> Union[list, type[Parameter.empty]]:
         """
         Get the enum property to be added to the JSON schema.
         Return `Parameter.empty` to omit the enum from the schema.
         """
         return Parameter.empty
 
     def to_json(self) -> dict:
@@ -141,27 +141,29 @@
     def validate(self, value) -> bool:
         # Allow implicit conversion from int to float
         if self.type is float and type(value) is int:
             return True
         return self.type == type(value)
 
     def _get_type(self) -> dict:
-        return {"type": self.TYPE_MAP.get(self.type.__name__, "object")}
+        if self.type is not None:
+            return {"type": self.TYPE_MAP.get(self.type.__name__, "object")}
+        return {"type": "null"}
 
 
 class GenericTypeSchema(TypeSchema):
     """
     Base class for generic types supporting subscription.
     """
 
     def _get_sub_types(self) -> list[TypeSchema]:
         """
         :return: A list of type schemas corresponding to the generic type arguments.
         """
-        return [TypeSchema.create(arg) for arg in typing.get_args(self.type)]
+        return [t for arg in typing.get_args(self.type) if (t := TypeSchema.create(arg)) is not None]
 
     def _get_sub_type(self) -> Optional[TypeSchema]:
         """
         :return: A type schema corresponding to the single generic type argument,
             or None if there is none. If there are multiple arguments, the first
             one is returned.
         """
@@ -178,15 +180,15 @@
     @staticmethod
     def matches(p_type: Type) -> bool:
         return p_type != Parameter.empty and (p_type is list or typing.get_origin(p_type) is list)
 
     def _get_type(self) -> dict:
         return {"type": "array"}
 
-    def _get_items(self) -> Union[dict, Parameter.empty]:
+    def _get_items(self) -> Union[dict, type[Parameter.empty]]:
         if sub_type := self._get_sub_type():
             return sub_type.to_json()
 
         return Parameter.empty
 
     def encode(self, value):
         if sub_type := self._get_sub_type():
@@ -256,35 +258,37 @@
     """
 
     def __init__(self, enum_values, type: Optional[Type] = None):
         super().__init__(type)
         self.enum_values = enum_values
 
     def _get_type(self) -> dict:
-        return TypeSchema.create(type(self.enum_values[0]))._get_type()
+        if (t := TypeSchema.create(type(self.enum_values[0]))) is not None:
+            return t._get_type()
+        return {"type": "object"}
 
-    def _get_enum(self) -> Union[list, Parameter.empty]:
+    def _get_enum(self) -> Union[list, type[Parameter.empty]]:
         return self.enum_values
 
     def validate(self, value) -> bool:
         return value in self.enum_values
 
 
 @ToolTypeSchema
 class EnumClassTypeSchema(EnumTypeSchema):
     """
     Type schema for enum.Enum types.
     """
 
-    def __init__(self, p_type: Enum):
+    def __init__(self, p_type: Type[Enum]):
         super().__init__([e.name for e in p_type], p_type)
 
     @staticmethod
-    def matches(type_p: Type) -> bool:
-        return type_p != Parameter.empty and isclass(type_p) and issubclass(type_p, Enum)
+    def matches(p_type: Type) -> bool:
+        return p_type != Parameter.empty and isclass(p_type) and issubclass(p_type, Enum)
 
     def encode(self, value):
         """
         Convert an enum instance to its name.
 
         :param value: The enum instance to be converted.
         """
@@ -292,15 +296,15 @@
 
     def decode(self, value):
         """
         Convert an enum name to an instance of the enum type.
 
         :param value: The enum name to be converted
         """
-        if value in self.enum_values:
+        if value in self.enum_values and self.type is not None:
             # Convert to an enum instance
             return self.type[value]
 
         # The user is invoking the method directly passing the enum instance
         return value
```

### Comparing `tool2schema-2.0.0/PKG-INFO` & `tool2schema-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: tool2schema
-Version: 2.0.0
-Summary: A library to generate function schemas for use in the OpenAI API.
+Version: 2.1.0
+Summary: A library to generate function schemas for use in LLM function calling.
 Home-page: https://github.com/cadifyai/tool2schema
 License: Apache-2.0
 Keywords: openai,llm
 Author: Angus Stewart
 Author-email: siliconlad@protonmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

