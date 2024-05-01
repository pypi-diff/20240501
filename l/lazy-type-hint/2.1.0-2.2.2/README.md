# Comparing `tmp/lazy_type_hint-2.1.0.tar.gz` & `tmp/lazy_type_hint-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazy_type_hint-2.1.0.tar", max compression
+gzip compressed data, was "lazy_type_hint-2.2.2.tar", max compression
```

## Comparing `lazy_type_hint-2.1.0.tar` & `lazy_type_hint-2.2.2.tar`

### file list

```diff
@@ -1,42 +1,43 @@
--rw-r--r--   0        0        0      257 2024-04-03 13:39:39.210757 lazy_type_hint-2.1.0/lazy_type_hint/__init__.py
--rw-r--r--   0        0        0      495 2024-04-03 08:50:18.646693 lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/__init__.py
--rw-r--r--   0        0        0    12297 2024-04-20 12:20:31.948128 lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/data_type_tree.py
--rw-r--r--   0        0        0     7268 2024-04-19 13:25:22.421859 lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/factory.py
--rw-r--r--   0        0        0     1118 2024-04-19 13:25:22.427858 lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/generic_type/__init__.py
--rw-r--r--   0        0        0    17314 2024-04-19 13:25:22.433858 lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/generic_type/dict_data_type_tree.py
--rw-r--r--   0        0        0     2963 2024-04-20 12:20:31.948128 lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/generic_type/generic_data_type_tree.py
--rw-r--r--   0        0        0      775 2024-04-19 13:25:22.439859 lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/generic_type/iterator_data_type_tree.py
--rw-r--r--   0        0        0     1094 2024-04-19 13:25:22.445857 lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/generic_type/list_data_type_tree.py
--rw-r--r--   0        0        0     5872 2024-04-20 12:20:31.949822 lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/generic_type/mapping_data_type_tree.py
--rw-r--r--   0        0        0      601 2024-04-19 13:25:22.452857 lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/generic_type/mapping_proxy_data_type_tree.py
--rw-r--r--   0        0        0     7038 2024-04-20 12:20:31.950322 lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/generic_type/pandas_data_frame_data_type_tree.py
--rw-r--r--   0        0        0     1309 2024-04-20 12:20:31.951328 lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/generic_type/sequence_data_type_tree.py
--rw-r--r--   0        0        0     6506 2024-04-19 13:25:22.458858 lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/generic_type/set_and_sequence_operations.py
--rw-r--r--   0        0        0     1949 2024-04-20 12:20:31.951328 lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/generic_type/set_data_type_tree.py
--rw-r--r--   0        0        0     2101 2024-04-19 13:25:22.464857 lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/generic_type/tuple_data_type_tree.py
--rw-r--r--   0        0        0     1061 2024-04-15 15:41:02.091078 lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/simple_data_type_tree/__init__.py
--rw-r--r--   0        0        0     3013 2024-04-19 13:25:22.470858 lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/simple_data_type_tree/function_data_type_tree.py
--rw-r--r--   0        0        0     1060 2024-04-15 15:41:02.097066 lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/simple_data_type_tree/instance_data_type_tree.py
--rw-r--r--   0        0        0      368 2024-04-19 13:25:22.475858 lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/simple_data_type_tree/io_data_type_tree.py
--rw-r--r--   0        0        0      404 2024-04-19 13:25:22.480858 lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/simple_data_type_tree/module_data_type_tree.py
--rw-r--r--   0        0        0      439 2024-04-19 13:25:22.487019 lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/simple_data_type_tree/pandas_series_data_type_tree.py
--rw-r--r--   0        0        0     1003 2024-04-14 10:39:38.880313 lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/simple_data_type_tree/simple_data_type_tree.py
--rw-r--r--   0        0        0      755 2024-04-19 13:25:22.492857 lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/simple_data_type_tree/type_data_type_tree.py
--rw-r--r--   0        0        0      192 2024-04-03 08:50:18.656845 lazy_type_hint-2.1.0/lazy_type_hint/file_modifiers/__init__.py
--rw-r--r--   0        0        0    11392 2024-04-03 15:48:14.641664 lazy_type_hint-2.1.0/lazy_type_hint/file_modifiers/py_file_modifier.py
--rw-r--r--   0        0        0    17473 2024-04-03 08:50:18.657845 lazy_type_hint-2.1.0/lazy_type_hint/file_modifiers/yaml_file_modifier.py
--rw-r--r--   0        0        0     2340 2024-04-15 06:56:34.375018 lazy_type_hint-2.1.0/lazy_type_hint/generators/lazy_type_hint.py
--rw-r--r--   0        0        0     3137 2024-04-18 17:00:26.789320 lazy_type_hint-2.1.0/lazy_type_hint/generators/lazy_type_hint_abc.py
--rw-r--r--   0        0        0    10092 2024-04-20 12:20:31.952328 lazy_type_hint-2.1.0/lazy_type_hint/generators/lazy_type_hint_live.py
--rw-r--r--   0        0        0        0 2024-04-03 08:50:18.658845 lazy_type_hint-2.1.0/lazy_type_hint/py.typed
--rw-r--r--   0        0        0     2222 2024-04-19 13:25:22.505265 lazy_type_hint-2.1.0/lazy_type_hint/strategies.py
--rw-r--r--   0        0        0      732 2024-04-19 13:25:22.511264 lazy_type_hint-2.1.0/lazy_type_hint/utils/__init__.py
--rw-r--r--   0        0        0     2303 2024-04-03 08:50:18.660845 lazy_type_hint-2.1.0/lazy_type_hint/utils/docstring_formatter.py
--rw-r--r--   0        0        0     5655 2024-04-15 15:41:02.110072 lazy_type_hint-2.1.0/lazy_type_hint/utils/import_manager.py
--rw-r--r--   0        0        0     5008 2024-04-14 13:10:20.018341 lazy_type_hint-2.1.0/lazy_type_hint/utils/mypy.py
--rw-r--r--   0        0        0     1275 2024-04-03 08:50:18.662845 lazy_type_hint-2.1.0/lazy_type_hint/utils/ordered_set.py
--rw-r--r--   0        0        0      669 2024-04-03 08:50:18.662845 lazy_type_hint-2.1.0/lazy_type_hint/utils/test_ordered_set.py
--rw-r--r--   0        0        0     3712 2024-04-20 12:20:31.953328 lazy_type_hint-2.1.0/lazy_type_hint/utils/utils.py
--rw-r--r--   0        0        0     2602 2024-04-20 12:14:56.856217 lazy_type_hint-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     7335 2024-04-20 12:20:31.946128 lazy_type_hint-2.1.0/README.md
--rw-r--r--   0        0        0     7711 1970-01-01 00:00:00.000000 lazy_type_hint-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0      257 2024-04-03 13:39:39.210757 lazy_type_hint-2.2.2/lazy_type_hint/__init__.py
+-rw-r--r--   0        0        0      495 2024-04-03 08:50:18.646693 lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/__init__.py
+-rw-r--r--   0        0        0    12413 2024-04-29 13:45:53.508452 lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/data_type_tree.py
+-rw-r--r--   0        0        0     7793 2024-04-29 13:45:53.517325 lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/factory.py
+-rw-r--r--   0        0        0     1279 2024-04-29 13:45:53.522867 lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/generic_type/__init__.py
+-rw-r--r--   0        0        0    17314 2024-04-19 13:25:22.433858 lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/generic_type/dict_data_type_tree.py
+-rw-r--r--   0        0        0     2963 2024-04-20 12:20:31.948128 lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/generic_type/generic_data_type_tree.py
+-rw-r--r--   0        0        0      803 2024-04-23 15:02:40.562766 lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/generic_type/iterator_data_type_tree.py
+-rw-r--r--   0        0        0     1144 2024-04-23 15:02:40.563766 lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/generic_type/list_data_type_tree.py
+-rw-r--r--   0        0        0     5922 2024-04-23 15:02:40.570766 lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/generic_type/mapping_data_type_tree.py
+-rw-r--r--   0        0        0      601 2024-04-19 13:25:22.452857 lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/generic_type/mapping_proxy_data_type_tree.py
+-rw-r--r--   0        0        0     7814 2024-05-01 13:21:10.135455 lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/generic_type/pandas_data_frame_data_type_tree.py
+-rw-r--r--   0        0        0     1779 2024-04-29 13:45:53.534808 lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/generic_type/pandas_series_data_type_tree.py
+-rw-r--r--   0        0        0     1309 2024-04-20 12:20:31.951328 lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/generic_type/sequence_data_type_tree.py
+-rw-r--r--   0        0        0     6646 2024-04-29 13:45:53.539888 lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/generic_type/set_and_sequence_operations.py
+-rw-r--r--   0        0        0     1988 2024-04-23 15:02:40.576999 lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/generic_type/set_data_type_tree.py
+-rw-r--r--   0        0        0     2129 2024-04-23 15:02:40.576999 lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/generic_type/tuple_data_type_tree.py
+-rw-r--r--   0        0        0     1039 2024-04-29 13:45:53.548265 lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/simple_data_type_tree/__init__.py
+-rw-r--r--   0        0        0     3114 2024-04-23 15:02:40.585280 lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/simple_data_type_tree/function_data_type_tree.py
+-rw-r--r--   0        0        0     1478 2024-04-23 15:02:40.585280 lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/simple_data_type_tree/instance_data_type_tree.py
+-rw-r--r--   0        0        0      396 2024-04-23 15:02:40.591280 lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/simple_data_type_tree/io_data_type_tree.py
+-rw-r--r--   0        0        0      432 2024-04-23 15:02:40.597509 lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/simple_data_type_tree/module_data_type_tree.py
+-rw-r--r--   0        0        0      511 2024-04-23 15:02:40.606702 lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/simple_data_type_tree/numpy_data_type_tree.py
+-rw-r--r--   0        0        0     1003 2024-04-14 10:39:38.880313 lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/simple_data_type_tree/simple_data_type_tree.py
+-rw-r--r--   0        0        0      794 2024-04-23 15:02:40.615914 lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/simple_data_type_tree/type_data_type_tree.py
+-rw-r--r--   0        0        0      192 2024-04-03 08:50:18.656845 lazy_type_hint-2.2.2/lazy_type_hint/file_modifiers/__init__.py
+-rw-r--r--   0        0        0    11392 2024-04-03 15:48:14.641664 lazy_type_hint-2.2.2/lazy_type_hint/file_modifiers/py_file_modifier.py
+-rw-r--r--   0        0        0    17473 2024-04-03 08:50:18.657845 lazy_type_hint-2.2.2/lazy_type_hint/file_modifiers/yaml_file_modifier.py
+-rw-r--r--   0        0        0     2340 2024-04-29 13:45:49.656127 lazy_type_hint-2.2.2/lazy_type_hint/generators/lazy_type_hint.py
+-rw-r--r--   0        0        0     3137 2024-04-29 13:45:49.662517 lazy_type_hint-2.2.2/lazy_type_hint/generators/lazy_type_hint_abc.py
+-rw-r--r--   0        0        0    10092 2024-04-29 13:45:49.712316 lazy_type_hint-2.2.2/lazy_type_hint/generators/lazy_type_hint_live.py
+-rw-r--r--   0        0        0        0 2024-04-03 08:50:18.658845 lazy_type_hint-2.2.2/lazy_type_hint/py.typed
+-rw-r--r--   0        0        0     2222 2024-04-23 15:02:15.663344 lazy_type_hint-2.2.2/lazy_type_hint/strategies.py
+-rw-r--r--   0        0        0      732 2024-04-19 13:25:22.511264 lazy_type_hint-2.2.2/lazy_type_hint/utils/__init__.py
+-rw-r--r--   0        0        0     2303 2024-04-03 08:50:18.660845 lazy_type_hint-2.2.2/lazy_type_hint/utils/docstring_formatter.py
+-rw-r--r--   0        0        0     5900 2024-04-29 13:45:53.555265 lazy_type_hint-2.2.2/lazy_type_hint/utils/import_manager.py
+-rw-r--r--   0        0        0     5008 2024-04-14 13:10:20.018341 lazy_type_hint-2.2.2/lazy_type_hint/utils/mypy.py
+-rw-r--r--   0        0        0     1275 2024-04-03 08:50:18.662845 lazy_type_hint-2.2.2/lazy_type_hint/utils/ordered_set.py
+-rw-r--r--   0        0        0      669 2024-04-03 08:50:18.662845 lazy_type_hint-2.2.2/lazy_type_hint/utils/test_ordered_set.py
+-rw-r--r--   0        0        0     3712 2024-04-20 12:20:31.953328 lazy_type_hint-2.2.2/lazy_type_hint/utils/utils.py
+-rw-r--r--   0        0        0     2625 2024-05-01 13:21:10.136456 lazy_type_hint-2.2.2/pyproject.toml
+-rw-r--r--   0        0        0    12338 2024-04-29 13:45:49.641764 lazy_type_hint-2.2.2/README.md
+-rw-r--r--   0        0        0    12602 1970-01-01 00:00:00.000000 lazy_type_hint-2.2.2/PKG-INFO
```

### Comparing `lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/data_type_tree.py` & `lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/data_type_tree.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """`DataTypeTree` object that creates a tree representing all container types within the data type given.
 
 This data can then be parsed to a .py compatible file that will type hint your code.
 """
-
 from __future__ import annotations
 
 import re
 from abc import ABC, abstractmethod
 from typing import (
     TYPE_CHECKING,
     Any,
@@ -183,14 +182,15 @@
         """
         if self.parent is None:
             return True
         return bool(self.height > self.strategies.min_height_to_define_type_alias)
 
     @final
     def get_str_top_node_without_lvalue(self) -> str:
+        """This method will return either the type alias or its content depending on the permissions of the tree."""
         return self.get_str_top_node().split("=")[-1].strip()
 
     @final
     def get_str_top_node(self) -> str:
         return self._get_str_top_node()
 
     @final
```

### Comparing `lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/factory.py` & `lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,36 +14,52 @@
         Optional,
         Sequence,
         Set,
         TextIO,
         Tuple,
     )
 
+    import numpy as np
     import pandas as pd
+    from numpy.typing import NDArray
 
     from lazy_type_hint.data_type_tree.generic_type.dict_data_type_tree import DictDataTypeTree
     from lazy_type_hint.data_type_tree.generic_type.iterator_data_type_tree import IteratorDataTypeTree
     from lazy_type_hint.data_type_tree.generic_type.list_data_type_tree import ListDataTypeTree
     from lazy_type_hint.data_type_tree.generic_type.mapping_data_type_tree import MappingDataTypeTree
     from lazy_type_hint.data_type_tree.generic_type.mapping_proxy_data_type_tree import MappingProxyDataTypeTree
     from lazy_type_hint.data_type_tree.generic_type.pandas_data_frame_data_type_tree import PandasDataFrameDataTypeTree
+    from lazy_type_hint.data_type_tree.generic_type.pandas_series_data_type_tree import (
+        PandasSeriesDataTypeTree,
+    )
     from lazy_type_hint.data_type_tree.generic_type.sequence_data_type_tree import SequenceDataTypeTree
     from lazy_type_hint.data_type_tree.generic_type.set_data_type_tree import SetDataTypeTree
     from lazy_type_hint.data_type_tree.generic_type.tuple_data_type_tree import TupleDataTypeTree
     from lazy_type_hint.data_type_tree.simple_data_type_tree.io_data_type_tree import IoDataTypeTree
     from lazy_type_hint.data_type_tree.simple_data_type_tree.module_data_type_tree import ModuleTypeDataTypeTree
-    from lazy_type_hint.data_type_tree.simple_data_type_tree.pandas_series_data_type_tree import (
-        PandasSeriesDataTypeTree,
-    )
+    from lazy_type_hint.data_type_tree.simple_data_type_tree.numpy_data_type_tree import NumpyDataTypeTree
     from lazy_type_hint.data_type_tree.simple_data_type_tree.simple_data_type_tree import SimpleDataTypeTree
     from lazy_type_hint.utils import ImportManager
 
 
 @overload
 def data_type_tree_factory(  # type: ignore[overload-overlap]
+    data: "NDArray[np.generic]",
+    name: str,
+    *,
+    imports: "Optional[ImportManager]" = None,
+    depth: int = 0,
+    strategies: ParsingStrategies = ParsingStrategies(),  # noqa: B008
+    parent: "Optional[DataTypeTree]" = None,
+) -> "NumpyDataTypeTree":
+    ...
+
+
+@overload
+def data_type_tree_factory(  # type: ignore[overload-overlap]
     data: "MappingProxyType[Any, Any]",
     name: str,
     *,
     imports: "Optional[ImportManager]" = None,
     depth: int = 0,
     strategies: ParsingStrategies = ParsingStrategies(),  # noqa: B008
     parent: "Optional[DataTypeTree]" = None,
@@ -88,15 +104,15 @@
     parent: "Optional[DataTypeTree]" = None,
 ) -> "IoDataTypeTree":
     ...
 
 
 @overload
 def data_type_tree_factory(
-    data: "pd.Series",
+    data: "pd.Series[Any]",
     name: str,
     *,
     imports: "Optional[ImportManager]" = None,
     depth: int = 0,
     strategies: ParsingStrategies = ParsingStrategies(),  # noqa: B008
     parent: "Optional[DataTypeTree]" = None,
 ) -> "PandasSeriesDataTypeTree":
```

### Comparing `lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/generic_type/__init__.py` & `lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/generic_type/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,14 +6,17 @@
     MappingDataTypeTree as MappingDataTypeTree,
 )
 
 with suppress(ImportError):
     from lazy_type_hint.data_type_tree.generic_type.pandas_data_frame_data_type_tree import (
         PandasDataFrameDataTypeTree as PandasDataFrameDataTypeTree,
     )
+    from lazy_type_hint.data_type_tree.generic_type.pandas_series_data_type_tree import (
+        PandasSeriesDataTypeTree as PandasSeriesDataTypeTree,
+    )
 from lazy_type_hint.data_type_tree.generic_type.iterator_data_type_tree import (
     IteratorDataTypeTree as IteratorDataTypeTree,
 )
 from lazy_type_hint.data_type_tree.generic_type.mapping_proxy_data_type_tree import (
     MappingProxyDataTypeTree as MappingProxyDataTypeTree,
 )
 from lazy_type_hint.data_type_tree.generic_type.set_data_type_tree import SetDataTypeTree as SetDataTypeTree
```

### Comparing `lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/generic_type/dict_data_type_tree.py` & `lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/generic_type/dict_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/generic_type/generic_data_type_tree.py` & `lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/generic_type/generic_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/generic_type/iterator_data_type_tree.py` & `lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/generic_type/iterator_data_type_tree.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,10 +13,10 @@
 
     @override
     def _instantiate_children(self, data: Sequence[Any]) -> Tuple[DataTypeTree, ...]:  # type: ignore
         return self.operations.instantiate_children(data, allow_repeated_children=False)
 
     @override
     def _get_str_top_node(self) -> str:
-        self.imports.add("Iterator")
+        self.imports.add("Iterator").add("TypeAlias")
         container = "Iterator"
-        return f"{self.name} = {container}[{self.get_type_alias_children()}]"
+        return f"{self.name}: TypeAlias = {container}[{self.get_type_alias_children()}]"
```

### Comparing `lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/generic_type/list_data_type_tree.py` & `lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/generic_type/list_data_type_tree.py`

 * *Files 17% similar despite different names*

```diff
@@ -21,8 +21,9 @@
             self.imports.add("list")
             container = "List"
         elif self.strategies.list_strategy == "Sequence":
             self.imports.add("Sequence")
             container = "Sequence"
         else:
             raise DataTypeTreeError(f"The chosen strategy ({self.strategies.list_strategy}) is not available.")
-        return f"{self.name} = {container}[{self.get_type_alias_children()}]"
+        self.imports.add("TypeAlias")
+        return f"{self.name}: TypeAlias = {container}[{self.get_type_alias_children()}]"
```

### Comparing `lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/generic_type/mapping_data_type_tree.py` & `lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/generic_type/mapping_data_type_tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,16 @@
             self.imports.add(container)
 
         keys = self._get_types(iterable=children.keys(), remove_repeated=True)
         keys_str = self._format_types(keys)
         value_types = self.get_type_alias_children()
 
         container_ = "Dict" if container == "dict" else container
-        return f"{self.name} = {container_}[{keys_str}, {value_types}]"
+        self.imports.add("TypeAlias")
+        return f"{self.name}: TypeAlias = {container_}[{keys_str}, {value_types}]"
 
     @staticmethod
     def _to_camel_case(string: str) -> str:
         """Make it camel case and compatible with Python keywords."""
         # Remove any initial number within the string
         match = re.match(r"^\d+", string)
         if match:
```

### Comparing `lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/generic_type/mapping_proxy_data_type_tree.py` & `lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/generic_type/mapping_proxy_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/generic_type/pandas_data_frame_data_type_tree.py` & `lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/generic_type/pandas_data_frame_data_type_tree.py`

 * *Files 8% similar despite different names*

```diff
@@ -109,49 +109,58 @@
     def are_column_same_type(self) -> bool:
         return len({type(column) for column in self.data.columns}) == 1
 
     def all_columns_are(self, type_: Type[object]) -> bool:
         return all(isinstance(column, type_) for column in self.data.columns)
 
     @property
-    def are_columns_either_all_str_or_all_tuple(self) -> bool:
-        if self.are_column_same_type:
-            return all(isinstance(column, (str, int, tuple)) for column in self.data.columns)
-        return False
+    def literal_compatible_types(self) -> Tuple[Type[str], Type[bool], Type[int]]:
+        return str, bool, int
+
+    @property
+    def are_all_columns_literal_compatible(self) -> bool:
+        column: Hashable
+        for column in self.data.columns:
+            if isinstance(column, tuple):
+                column = column[0]
+            if not isinstance(column, self.literal_compatible_types):
+                return False
+        return True
 
     def _create_child(self, column: Hashable) -> DataTypeTree:
         suffix = self._to_camel_case(str(column))
+        suffix = suffix if suffix else "WSpace"
         return data_type_tree_factory(  # type: ignore
             data=self.data[column],
             name=f"{self.name}{suffix}",
             imports=self.imports,
             depth=self.depth + 1,
             strategies=self.strategies,
             parent=self,
         )
 
     @override
     def _instantiate_children(self, data: pd.DataFrame) -> Mapping[Hashable, DataTypeTree]:
         children: Dict[Hashable, DataTypeTree] = {}
-        if not self.are_columns_either_all_str_or_all_tuple:
+        if not self.are_all_columns_literal_compatible:
             return {}
 
         # Corner case to avoid infinite recursion
         if all(isinstance(column, tuple) and len(column) == 1 for column in self.data.columns):
             return {}
 
         for column in data.columns:
             if not self.can_be_accessed_multilevel:  # Here all columns will  be Hashable
                 column = cast(Hashable, column)
                 children[column] = self._create_child(column)
             else:  # Here all columns will be tuple
                 multi_column = cast(Tuple[Hashable, ...], column)
                 columns_processed: Set[Union[bool, str, int]] = set()
                 if multi_column[0] not in columns_processed:
-                    if isinstance(multi_column[0], (str, int, bool)):
+                    if isinstance(multi_column[0], self.literal_compatible_types):
                         columns_processed.add(multi_column[0])
                         children[column[0]] = self._create_child(column[0])
         return children
 
     @override
     def _get_hash(self) -> str:
         if self.strategies.pandas_strategies == "Do not type hint columns":
@@ -172,20 +181,29 @@
         self.imports.add("list")
         self.imports.add("Hashable")
         self.imports.add("numpy")
         self.imports.add("pd.Scalar")
 
         overloads: List[str] = []
         for literal, child in self.children.items():
-            if child.permission_to_be_created_as_type_alias:
-                overloads.append(LITERAL_OVERLOAD_TEMPLATE.format(literal=repr(literal), rtype=child.name))
-            else:
-                rtype = "pd.Series" if isinstance(self.data[literal], pd.Series) else "pd.DataFrame"
-                overloads.append(LITERAL_OVERLOAD_TEMPLATE.format(literal=repr(literal), rtype=rtype))
+            if isinstance(literal, self.literal_compatible_types):
+                if child.permission_to_be_created_as_type_alias:
+                    overloads.append(LITERAL_OVERLOAD_TEMPLATE.format(literal=repr(literal), rtype=child.name))
+                else:
+                    rtype = child.get_str_top_node_without_lvalue()
+                    overloads.append(LITERAL_OVERLOAD_TEMPLATE.format(literal=repr(literal), rtype=rtype))
         if self.strategies.pandas_strategies == "Full type hint":
-            all_literals = ", ".join(repr(key) for key in self.children)
-            allowed_types = f"Literal[{all_literals}]"
+            literal_compatible_keys: List[str] = []
+            extra_types = ""
+            for key in self.children:
+                if isinstance(key, self.literal_compatible_types):
+                    literal_compatible_keys.append(repr(key))
+                else:
+                    self.imports.add("Hashable")
+                    extra_types = ", Hashable"  # This can be more precise, but not supported yet
+            all_literals = ", ".join(literal_compatible_keys)
+            allowed_types = f"Literal[{all_literals}]" + extra_types
             template = TEMPLATE_NO_PD
         else:
             allowed_types = "str"
             template = TEMPLATE
         return template.format(class_name=self.name, overloads="\n".join(overloads), allowed_types=allowed_types)
```

### Comparing `lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/generic_type/sequence_data_type_tree.py` & `lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/generic_type/sequence_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/generic_type/set_and_sequence_operations.py` & `lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/generic_type/set_and_sequence_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,21 +19,22 @@
 )
 
 from lazy_type_hint.data_type_tree.factory import data_type_tree_factory
 from lazy_type_hint.data_type_tree.generic_type.dict_data_type_tree import DictDataTypeTree
 
 if TYPE_CHECKING:
     from lazy_type_hint.data_type_tree.data_type_tree import DataTypeTree
+    from lazy_type_hint.data_type_tree.generic_type.pandas_series_data_type_tree import PandasSeriesDataTypeTree
     from lazy_type_hint.data_type_tree.generic_type.sequence_data_type_tree import SequenceDataTypeTree
     from lazy_type_hint.data_type_tree.generic_type.set_data_type_tree import SetDataTypeTree
 
 
 @dataclass(frozen=True)
 class SetAndSequenceOperations:
-    data_type_tree: "Union[SetDataTypeTree, SequenceDataTypeTree]"
+    data_type_tree: "Union[SetDataTypeTree, SequenceDataTypeTree, PandasSeriesDataTypeTree]"
 
     def instantiate_children(self, data: Sequence[Any], *, allow_repeated_children: bool) -> Tuple["DataTypeTree", ...]:
         """Instantiate the children for sets and sequences.
 
         If `allow_repeated_children` is set to True, all children will be returned even if they are repeated.
         """
         if allow_repeated_children:
```

### Comparing `lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/generic_type/set_data_type_tree.py` & `lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/generic_type/set_data_type_tree.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,19 +23,19 @@
     @override
     def _instantiate_children(self, data: Sequence[Any]) -> Tuple[DataTypeTree, ...]:  # type: ignore
         return self.operations.instantiate_children(data, allow_repeated_children=False)
 
     @override
     def _get_str_top_node(self) -> str:
         container: Literal["FrozenSet", "set"] = "FrozenSet" if self.holding_type is frozenset else "set"
-        self.imports.add(container)
+        self.imports.add(container).add("TypeAlias")
 
         if container == "FrozenSet":
-            return f"{self.name} = FrozenSet[{self.get_type_alias_children()}]"
-        return f"{self.name} = Set[{self.get_type_alias_children()}]"
+            return f"{self.name}: TypeAlias = FrozenSet[{self.get_type_alias_children()}]"
+        return f"{self.name}: TypeAlias = Set[{self.get_type_alias_children()}]"
 
     @override
     def _get_hash(self) -> Hashable:
         hashes: Set[object] = set()
         for child in self:
             hashes.add(child._get_hash())
         return frozenset(hashes)
```

### Comparing `lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/generic_type/tuple_data_type_tree.py` & `lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/generic_type/tuple_data_type_tree.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,16 +14,16 @@
         if self.strategies.tuple_size_strategy == "fixed":
             return self.operations.instantiate_children(data, allow_repeated_children=True)
         else:
             return self.operations.instantiate_children(data, allow_repeated_children=False)
 
     @override
     def _get_str_top_node(self) -> str:
-        self.imports.add("tuple")
-        return f"{self.name} = Tuple[{self.get_type_alias_children()}]"
+        self.imports.add("tuple").add("TypeAlias")
+        return f"{self.name}: TypeAlias = Tuple[{self.get_type_alias_children()}]"
 
     @override
     def get_type_alias_children(self) -> str:
         if self.strategies.tuple_size_strategy == "fixed":
             child_types = self._get_types(remove_repeated=False)
         else:
             child_types = self._get_types(remove_repeated=True)
```

### Comparing `lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/simple_data_type_tree/__init__.py` & `lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/simple_data_type_tree/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,16 +4,16 @@
     FunctionDataTypeTree as FunctionDataTypeTree,
 )
 from lazy_type_hint.data_type_tree.simple_data_type_tree.instance_data_type_tree import (
     InstanceDataTypeTree as InstanceDataTypeTree,
 )
 
 with suppress(ImportError):
-    from lazy_type_hint.data_type_tree.simple_data_type_tree.pandas_series_data_type_tree import (
-        PandasSeriesDataTypeTree as PandasSeriesDataTypeTree,
+    from lazy_type_hint.data_type_tree.simple_data_type_tree.numpy_data_type_tree import (
+        NumpyDataTypeTree as NumpyDataTypeTree,
     )
 from lazy_type_hint.data_type_tree.simple_data_type_tree.io_data_type_tree import IoDataTypeTree as IoDataTypeTree
 from lazy_type_hint.data_type_tree.simple_data_type_tree.module_data_type_tree import (
     ModuleTypeDataTypeTree as ModuleTypeDataTypeTree,
 )
 from lazy_type_hint.data_type_tree.simple_data_type_tree.simple_data_type_tree import (
     SimpleDataTypeTree as SimpleDataTypeTree,
```

### Comparing `lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/simple_data_type_tree/function_data_type_tree.py` & `lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/simple_data_type_tree/function_data_type_tree.py`

 * *Files 19% similar despite different names*

```diff
@@ -32,16 +32,16 @@
             inspect.signature(self.data)
             return True
         except ValueError:
             return False
 
     def _get_str_top_node(self) -> str:
         if not self.can_be_inspected:
-            self.imports.add("Callable")
-            return f"{self.name} = Callable"
+            self.imports.add("Callable").add("TypeAlias")
+            return f"{self.name}: TypeAlias = Callable"
         if self.is_lambda:
             return self._get_lambda_str()
         return self._get_protocol_str()
 
     def _get_protocol_str(self) -> str:
         args = str(inspect.signature(self.data))
         self.imports.add("Protocol")
@@ -55,18 +55,20 @@
         return f"""class {self.name}(Protocol):\n{TAB}def __call__{args}: ..."""
 
     def get_func_params(self) -> MappingProxyType[str, Parameter]:
         signature = inspect.signature(self.data)
         return signature.parameters
 
     def _get_lambda_str(self) -> str:
-        self.imports.add("Callable").add("Any")
+        self.imports.add("Callable").add("Any").add("TypeAlias")
         if self.can_be_inspected:
-            return f"{self.name} = Callable[[{', '.join(['Any']*len(self.get_func_params().values()))}], Any]"
-        return f"{self.name} = Callable"
+            return (
+                f"{self.name}: TypeAlias = Callable[[{', '.join(['Any']*len(self.get_func_params().values()))}], Any]"
+            )
+        return f"{self.name}: TypeAlias = Callable"
 
     @override
     def _get_hash(self) -> Hashable:
         if self.is_lambda and self.can_be_inspected:
             return str(f"Callable[[{', '.join(['Any']*len(self.get_func_params().values()))}], Any]")
         else:
             if self.can_be_inspected:
```

### Comparing `lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/simple_data_type_tree/instance_data_type_tree.py` & `lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/simple_data_type_tree/instance_data_type_tree.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,20 +8,30 @@
 class InstanceDataTypeTree(SimpleDataTypeTree):
     # Change it by `NoneType` once I drop support with Python 3.8
     wraps = (bool, int, float, range, slice, str, type(None))  # + Custom classes
 
     @override
     def _get_str_top_node(self) -> str:
         if self.holding_type == type(None):
+            self.imports.add("TypeAlias")
             self.imports.add("Optional")
-            return f"{self.name} = Optional[object]"
+            return f"{self.name}: TypeAlias = Optional[object]"
 
         if self._is_builtin_class():
-            return f"{self.name} = {self.holding_type.__name__}"
-        return f'{self.name} = "{self.holding_type.__name__}"'
+            if self.parent is None:
+                self.imports.add("TypeAlias")
+                return f"{self.name}: TypeAlias = {self.holding_type.__name__}"
+            else:
+                return f"{self.name} = {self.holding_type.__name__}"
+
+        if self.parent is None:
+            self.imports.add("TypeAlias")
+            return f'{self.name}: TypeAlias = "{self.holding_type.__name__}"'
+        else:
+            return f'{self.name} = "{self.holding_type.__name__}"'
 
     @override
     def _check_tree_is_correct_one(self, data: object) -> None:
         return
 
     def _is_builtin_class(self) -> bool:
         try:
```

### Comparing `lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/simple_data_type_tree/simple_data_type_tree.py` & `lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/simple_data_type_tree/simple_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/simple_data_type_tree/type_data_type_tree.py` & `lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/simple_data_type_tree/type_data_type_tree.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 
 class TypeDataTypeTree(SimpleDataTypeTree):
     wraps = (type,)
     data: Type[object]
 
     @override
     def _get_str_top_node(self) -> str:
-        self.imports.add("type")
+        self.imports.add("type").add("TypeAlias")
         if self.is_builtin_class():
-            return f"{self.name} = Type[{self.data.__name__}]"
-        return f'{self.name} = Type["{self.data.__name__}"]'
+            return f"{self.name}: TypeAlias = Type[{self.data.__name__}]"
+        return f'{self.name}: TypeAlias = Type["{self.data.__name__}"]'
 
     def is_builtin_class(self) -> bool:
         try:
             cls = getattr(builtins, self.data.__name__)
             return isinstance(cls, type)
         except AttributeError:
             return False
```

### Comparing `lazy_type_hint-2.1.0/lazy_type_hint/file_modifiers/py_file_modifier.py` & `lazy_type_hint-2.2.2/lazy_type_hint/file_modifiers/py_file_modifier.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.1.0/lazy_type_hint/file_modifiers/yaml_file_modifier.py` & `lazy_type_hint-2.2.2/lazy_type_hint/file_modifiers/yaml_file_modifier.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.1.0/lazy_type_hint/generators/lazy_type_hint.py` & `lazy_type_hint-2.2.2/lazy_type_hint/generators/lazy_type_hint.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.1.0/lazy_type_hint/generators/lazy_type_hint_abc.py` & `lazy_type_hint-2.2.2/lazy_type_hint/generators/lazy_type_hint_abc.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.1.0/lazy_type_hint/generators/lazy_type_hint_live.py` & `lazy_type_hint-2.2.2/lazy_type_hint/generators/lazy_type_hint_live.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.1.0/lazy_type_hint/strategies.py` & `lazy_type_hint-2.2.2/lazy_type_hint/strategies.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.1.0/lazy_type_hint/utils/__init__.py` & `lazy_type_hint-2.2.2/lazy_type_hint/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.1.0/lazy_type_hint/utils/docstring_formatter.py` & `lazy_type_hint-2.2.2/lazy_type_hint/utils/docstring_formatter.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.1.0/lazy_type_hint/utils/import_manager.py` & `lazy_type_hint-2.2.2/lazy_type_hint/utils/import_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,16 +33,18 @@
     "Iterator",
     "Literal",
     "overload",
     "pandas",
     "pd.Scalar",
     "npt",
     "numpy",
+    "NDArray",
     "ModuleType",
     "TextIO",
+    "annotations",
 ]
 
 
 @dataclass(frozen=True)
 class ImportManager:
     _set: Set[KEYWORDS_AVAILABLE] = field(default_factory=set)
 
@@ -68,19 +70,21 @@
             "Callable": ("typing", "Callable"),
             "ModuleType": ("types", "ModuleType"),
             "Protocol": ("typing", "Protocol"),
             "Literal": ("typing", "Literal"),
             "overload": ("typing", "overload"),
             "pandas": ("pandas", "pandas"),
             "npt": ("npt", "npt"),
+            "NDArray": ("numpy.typing", "NDArray"),
             "numpy": ("numpy", "numpy"),
-            "TypeAlias": ("typing_extenions", "TypeAlias"),
+            "TypeAlias": ("typing_extensions", "TypeAlias"),
             "pd.Scalar": ("pandas._typing", "Scalar"),
             "TextIO": ("typing", "TextIO"),
             "Iterator": ("typing", "Iterator"),
+            "annotations": ("__future__", "annotations"),
         }
     )
 
     def add(self, keyword: KEYWORDS_AVAILABLE) -> "Self":
         self._set.add(keyword)
         return self
 
@@ -131,14 +135,16 @@
                     f"{', '.join(self.PACKAGE.keys())}"
                 ) from error
             import_statements[".".join(reference[:-1])].append(reference[-1])
 
         imports_lst: List[str] = []
         for package, imports in sorted(import_statements.items(), key=lambda x: x[0]):
             imports_lst.append(self._format_single_package(package, imports, line_length=line_length))
+        if imports_lst and "__future__" in imports_lst[0]:
+            imports_lst[0] += "\n"
         return "\n".join(imports_lst)
 
     def _format_single_package(self, package: str, imports: Sequence[str], *, line_length: int) -> str:
         if imports[0] == "pandas":
             string = "import pandas as pd"
         elif imports[0] == "npt":
             string = "import numpy.typing as npt"
```

### Comparing `lazy_type_hint-2.1.0/lazy_type_hint/utils/mypy.py` & `lazy_type_hint-2.2.2/lazy_type_hint/utils/mypy.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.1.0/lazy_type_hint/utils/ordered_set.py` & `lazy_type_hint-2.2.2/lazy_type_hint/utils/ordered_set.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.1.0/lazy_type_hint/utils/test_ordered_set.py` & `lazy_type_hint-2.2.2/lazy_type_hint/utils/test_ordered_set.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.1.0/lazy_type_hint/utils/utils.py` & `lazy_type_hint-2.2.2/lazy_type_hint/utils/utils.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.1.0/pyproject.toml` & `lazy_type_hint-2.2.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lazy-type-hint"
-version = "2.1.0"
+version = "2.2.2"
 description = "Automate type hint generation in a single line."
 authors = ["Manuel Floriano Vázquez <mflovaa@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.urls]
 Source = "https://github.com/mflova/lazy-type-hint"
 
@@ -20,14 +20,15 @@
 black = "23.12.1"  # Autoformatter
 pytest-clarity = "^1.0.1"
 pyyaml = "*"  # Used by the `check_code.py` script
 types-pyyaml = "*"
 filelock = "*"
 pytest_xdist = "*"  # Parallel execution tests
 pandas = "*"
+numpy = "*"
 pyinstrument = "^4.6.2"
 pytest-benchmark = "^4.0.0"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
@@ -49,15 +50,15 @@
 explicit_package_bases = true
 
 [tool.ruff]
 line-length = 120
 target-version = "py38"
 exclude = ["*.pyi", "test_files"]
 lint.select = ["F", "E", "I", "N", "D", "UP", "YTT", "ASYNC", "BLE", "B", "A", "C4", "T10", "DJ", "EXE", "ISC", "ICN", "G", "PIE", "PYI", "PT", "Q", "RSE", "RET", "SLF", "SIM", "TID", "INT", "ARG", "FIX", "PD", "PGH", "PL", "FLY", "NPY", "AIR", "RUF", "TCH"]
-lint.ignore = ["SIM102", "EM101", "PLR", "D100", "D103", "C419", "D104", "D105", "D212", "PGH003", "RUF001", "D101", "PD901", "C405", "UP015", "PLC0414", "I001", "NPY002", "D102", "D107", "PT023", "B027", "UP007", "PIE808", "PD011", "SIM115", "PT006", "PT007", "F811", "UP006", "RET505", "PLW1510", "E731", "PLW2901", "SLF001"]
+lint.ignore = ["SIM102", "EM101", "PLR", "D100", "D103", "C419", "D104", "D105", "D212", "PGH003", "RUF001", "D101", "PD901", "C405", "UP015", "PLC0414", "I001", "NPY002", "D102", "D107", "PT023", "B027", "UP007", "PIE808", "PD011", "SIM115", "PT006", "PT007", "F811", "UP006", "RET505", "PLW1510", "E731", "PLW2901", "SLF001", "RUF018"]
 
 [tool.ruff.lint.pydocstyle]
 convention = "google"  # Docstring convention. Accepts: "google", "numpy", or "pep257".
 
 [tool.ruff.lint.flake8-pytest-style]
 fixture-parentheses = false
```

