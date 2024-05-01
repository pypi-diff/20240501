# Comparing `tmp/graphique-1.5.tar.gz` & `tmp/graphique-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphique-1.5.tar", last modified: Thu Jan 25 01:41:14 2024, max compression
+gzip compressed data, was "graphique-1.6.tar", last modified: Wed May  1 00:42:29 2024, max compression
```

## Comparing `graphique-1.5.tar` & `graphique-1.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 01:41:14.393681 graphique-1.5/
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-01-25 01:40:38.000000 graphique-1.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8241 2024-01-25 01:41:14.393681 graphique-1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6002 2024-01-25 01:40:38.000000 graphique-1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 01:41:14.389681 graphique-1.5/graphique/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-01-25 01:40:38.000000 graphique-1.5/graphique/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29316 2024-01-25 01:40:38.000000 graphique-1.5/graphique/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    29942 2024-01-25 01:40:38.000000 graphique-1.5/graphique/inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    26026 2024-01-25 01:40:38.000000 graphique-1.5/graphique/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     5860 2024-01-25 01:40:38.000000 graphique-1.5/graphique/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)    10800 2024-01-25 01:40:38.000000 graphique-1.5/graphique/models.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 01:40:38.000000 graphique-1.5/graphique/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-01-25 01:40:38.000000 graphique-1.5/graphique/scalars.py
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-01-25 01:40:38.000000 graphique-1.5/graphique/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-01-25 01:40:38.000000 graphique-1.5/graphique/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 01:41:14.393681 graphique-1.5/graphique.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8241 2024-01-25 01:41:14.000000 graphique-1.5/graphique.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-01-25 01:41:14.000000 graphique-1.5/graphique.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-25 01:41:14.000000 graphique-1.5/graphique.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-01-25 01:41:14.000000 graphique-1.5/graphique.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-01-25 01:41:14.000000 graphique-1.5/graphique.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-01-25 01:40:38.000000 graphique-1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-01-25 01:40:38.000000 graphique-1.5/requirements.in
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-25 01:41:14.393681 graphique-1.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 01:41:14.393681 graphique-1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    11278 2024-01-25 01:40:38.000000 graphique-1.5/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    14179 2024-01-25 01:40:38.000000 graphique-1.5/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    21190 2024-01-25 01:40:38.000000 graphique-1.5/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    25556 2024-01-25 01:40:38.000000 graphique-1.5/tests/test_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:42:29.570685 graphique-1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-01 00:41:53.000000 graphique-1.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8241 2024-05-01 00:42:29.570685 graphique-1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6002 2024-05-01 00:41:53.000000 graphique-1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:42:29.566686 graphique-1.6/graphique/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-01 00:41:53.000000 graphique-1.6/graphique/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29328 2024-05-01 00:41:53.000000 graphique-1.6/graphique/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29910 2024-05-01 00:41:53.000000 graphique-1.6/graphique/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26020 2024-05-01 00:41:53.000000 graphique-1.6/graphique/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5832 2024-05-01 00:41:53.000000 graphique-1.6/graphique/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10791 2024-05-01 00:41:53.000000 graphique-1.6/graphique/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 00:41:53.000000 graphique-1.6/graphique/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-05-01 00:41:53.000000 graphique-1.6/graphique/scalars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-01 00:41:53.000000 graphique-1.6/graphique/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-01 00:41:53.000000 graphique-1.6/graphique/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:42:29.566686 graphique-1.6/graphique.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8241 2024-05-01 00:42:29.000000 graphique-1.6/graphique.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-01 00:42:29.000000 graphique-1.6/graphique.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 00:42:29.000000 graphique-1.6/graphique.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-01 00:42:29.000000 graphique-1.6/graphique.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-01 00:42:29.000000 graphique-1.6/graphique.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-05-01 00:41:53.000000 graphique-1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-01 00:41:53.000000 graphique-1.6/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 00:42:29.570685 graphique-1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:42:29.566686 graphique-1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    12302 2024-05-01 00:41:53.000000 graphique-1.6/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14209 2024-05-01 00:41:53.000000 graphique-1.6/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21216 2024-05-01 00:41:53.000000 graphique-1.6/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25701 2024-05-01 00:41:53.000000 graphique-1.6/tests/test_service.py
```

### Comparing `graphique-1.5/LICENSE.txt` & `graphique-1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `graphique-1.5/PKG-INFO` & `graphique-1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphique
-Version: 1.5
+Version: 1.6
 Summary: GraphQL service for arrow tables and parquet data sets.
 Author-email: Aric Coady <aric.coady@gmail.com>
 License: Copyright 2022 Aric Coady
         
            Licensed under the Apache License, Version 2.0 (the "License");
            you may not use this file except in compliance with the License.
            You may obtain a copy of the License at
@@ -36,16 +36,16 @@
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: pyarrow>=15
-Requires-Dist: strawberry-graphql[asgi,cli]>=0.198
+Requires-Dist: pyarrow>=16
+Requires-Dist: strawberry-graphql[asgi,cli]>=0.221
 Provides-Extra: server
 Requires-Dist: uvicorn[standard]; extra == "server"
 Provides-Extra: cli
 Requires-Dist: tqdm; extra == "cli"
 
 [![image](https://img.shields.io/pypi/v/graphique.svg)](https://pypi.org/project/graphique/)
 ![image](https://img.shields.io/pypi/pyversions/graphique.svg)
```

### Comparing `graphique-1.5/README.md` & `graphique-1.6/README.md`

 * *Files identical despite different names*

### Comparing `graphique-1.5/graphique/core.py` & `graphique-1.6/graphique/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import inspect
 import itertools
 import operator
 import json
 from collections.abc import Callable, Iterable, Iterator, Sequence
 from dataclasses import dataclass
 from typing import Optional, Union, get_type_hints
-import numpy as np  # type: ignore
+import numpy as np
 import pyarrow as pa
 import pyarrow.acero as ac
 import pyarrow.compute as pc
 import pyarrow.dataset as ds
 from typing_extensions import Self
 
 Array = Union[pa.Array, pa.ChunkedArray]
@@ -398,18 +398,18 @@
 
         Args:
             *names: columns to partition by `not_equal` which will return scalars
             **predicates: pairwise predicates with optional args which will return list arrays;
                 if the predicate has args, it will be called on the differences
         """
         offsets = pa.chunked_array(
-            Column.run_offsets(self[name], *predicates.get(name, (pc.not_equal,)))
+            Column.run_offsets(self[name], *predicates.get(name, ()))
             for name in names + tuple(predicates)
-        ).unique()
-        offsets = offsets.take(pc.sort_indices(offsets))
+        )
+        offsets = offsets.unique().sort()
         scalars = self.select(names).take(offsets[:-1])
         lists = self.select(set(self.schema.names) - set(names))
         table = Table.union(scalars, Table.from_offsets(lists, offsets))
         return table, Column.diff(offsets)
 
     def group(self, *names: str, counts: str = '', **funcs: Sequence[Agg]) -> pa.Table:
         """Group by and aggregate.
@@ -419,17 +419,18 @@
             counts: alias for optional row counts
             **funcs: aggregate funcs with columns options
         """
         if isinstance(self, pa.Table):
             self = self.unify_dictionaries()
         prefix = 'hash_' if names else ''
         aggs = [agg.astuple(prefix + func) for func in funcs for agg in funcs[func]]
+        columns = list(names) + [agg[0] for agg in aggs]
         if counts:
             aggs.append(([], 'hash_count_all', None, counts))
-        return Declarations(self).aggregate(aggs, names).to_table()
+        return Declarations(self, columns).aggregate(aggs, names).to_table()
 
     def aggregate(self, counts: str = '', **funcs: Sequence[Agg]) -> dict:
         """Return aggregated scalars as a row of data."""
         row = {counts: len(self)} if counts else {}
         for key in ('one', 'list', 'distinct'):  # hash only functions
             func, aggs = getattr(Agg, key), funcs.pop(key, [])
             row |= {agg.alias: func(self[agg.name], **agg.options) for agg in aggs}
@@ -464,15 +465,15 @@
     def sort_indices(
         self, *names: str, length: Optional[int] = None, null_placement: str = 'at_end'
     ) -> pa.Array:
         """Return indices which would sort the table by columns, optimized for fixed length."""
         func = functools.partial(pc.sort_indices, null_placement=null_placement)
         if length is not None and length < len(self):
             func = functools.partial(pc.select_k_unstable, k=length)
-        keys = dict(map(sort_key, names))  # type: ignore
+        keys = dict(map(sort_key, names))
         table = pa.table({name: Column.sort_values(self[name]) for name in keys})
         return func(table, sort_keys=keys.items()) if table else pa.array([], 'int64')
 
     def sort(
         self,
         *names: str,
         length: Optional[int] = None,
@@ -556,15 +557,15 @@
 
         Args:
             k: max dense rank or length
             *names: columns to rank by
             dense: use dense rank; false indicates sorting
         """
         schema = set(Table.fragment_keys(self))
-        keys = dict(itertools.takewhile(lambda key: key[0] in schema, map(sort_key, names)))  # type: ignore
+        keys = dict(itertools.takewhile(lambda key: key[0] in schema, map(sort_key, names)))
         if not keys:
             return None, names
         parts = []
         for fragment in Table.get_fragments(self):
             parts.append(ds.get_partition_keys(fragment.partition_expression))
             if not dense:
                 parts[-1][''] = fragment.count_rows()
@@ -638,18 +639,18 @@
         'filter': ac.FilterNodeOptions,
         'project': ac.ProjectNodeOptions,
         'aggregate': ac.AggregateNodeOptions,
         'order_by': ac.OrderByNodeOptions,
         'hashjoin': ac.HashJoinNodeOptions,
     }
 
-    def __init__(self, source: Union[pa.Table, ds.Dataset]):
+    def __init__(self, source: Union[pa.Table, ds.Dataset], columns=None):
         if isinstance(source, ds.Dataset):
             expr = source._scan_options.get('filter')
-            self.scan(source, filter=expr)
+            self.scan(source, filter=expr, columns=columns)
             if expr is not None:
                 self.filter(expr)
         else:
             self.table_source(source)
 
     def apply(self, name: str, *args, **kwargs) -> Self:
         self.append(ac.Declaration(name, self.option_map[name](*args, **kwargs)))
```

### Comparing `graphique-1.5/graphique/inputs.py` & `graphique-1.6/graphique/inputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -373,19 +373,19 @@
                     field, _ = exprs
                     field = field.is_null() if op == 'eq' else field.is_valid()
                 else:
                     field = self.getfunc(op)(*exprs)
                 fields.append(field)
         for group in operator.attrgetter(*self.groups)(self):
             if group is not UNSET:
-                fields += group.to_fields()  # type: ignore
+                fields += group.to_fields()
         for op in self.unaries:
             expr = getattr(self, op)
             if expr is not UNSET:
-                fields.append(self.getfunc(op)(expr.to_arrow()))  # type: ignore
+                fields.append(self.getfunc(op)(expr.to_arrow()))
         if not fields:
             return None
         if len(fields) > 1:
             raise ValueError(f"conflicting inputs: {', '.join(map(str, fields))}")
         (field,) = fields
         cast = self.cast and isinstance(field, ds.Expression)
         return field.cast(self.cast, self.safe) if cast else field
```

### Comparing `graphique-1.5/graphique/interface.py` & `graphique-1.6/graphique/interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 from collections.abc import Callable, Iterable, Iterator, Mapping
 from datetime import timedelta
 from typing import Annotated, Optional, Union, no_type_check
 import pyarrow as pa
 import pyarrow.compute as pc
 import pyarrow.dataset as ds
 import strawberry.asgi
+from strawberry import Info
 from strawberry.extensions.utils import get_path_from_info
-from strawberry.types import Info
 from typing_extensions import Self
 from .core import Batch, Column as C, ListChunk, Table as T
 from .inputs import CountAggregate, Cumulative, Diff, Expression, Field, Filter
 from .inputs import HashAggregates, ListFunction, Pairwise, Projection, Rank
 from .inputs import ScalarAggregate, TDigestAggregate, VarianceAggregate, links, provisional
 from .models import Column, doc_field, selections
 from .scalars import Long
```

### Comparing `graphique-1.5/graphique/middleware.py` & `graphique-1.6/graphique/middleware.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,18 +5,17 @@
 import warnings
 from collections.abc import Iterable, Mapping
 from datetime import timedelta
 from keyword import iskeyword
 from typing import Optional
 import pyarrow.dataset as ds
 import strawberry.asgi
-from strawberry import UNSET
+from strawberry import Info, UNSET
 from strawberry.extensions import tracing
 from strawberry.utils.str_converters import to_camel_case
-from strawberry.types import Info
 from .core import Column as C
 from .inputs import Filter
 from .interface import Dataset, Root
 from .models import Column, doc_field
 from .scalars import Long, scalar_map, type_map
```

### Comparing `graphique-1.5/graphique/models.py` & `graphique-1.6/graphique/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 from collections.abc import Callable
 from datetime import date, datetime, time, timedelta
 from decimal import Decimal
 from typing import Annotated, Generic, Optional, TypeVar, TYPE_CHECKING, get_args
 import pyarrow as pa
 import pyarrow.compute as pc
 import strawberry
+from strawberry import Info
 from strawberry.field import StrawberryField
-from strawberry.types import Info
 from .core import Column as C
 from .inputs import links
-from .scalars import Interval, Long, scalar_map, type_map
+from .scalars import Long, scalar_map, type_map
 
 if TYPE_CHECKING:  # pragma: no cover
     from .interface import Dataset
 T = TypeVar('T')
 
 
 def _selections(field):
@@ -116,15 +116,15 @@
 
     @doc_field
     def values(self) -> list[Optional[T]]:
         """list of values"""
         return self.array.to_pylist()
 
 
-@Column.register(timedelta, Interval)
+@Column.register(timedelta, pa.MonthDayNano)
 @strawberry.type(name='Column', description="column of elapsed times")
 class NominalColumn(Generic[T], Column):
     values = doc_field(Set.values)
 
     @compute_field
     def count_distinct(self, mode: str = 'only_valid') -> Long:
         return pc.count_distinct(self.array, mode=mode).as_py()
```

### Comparing `graphique-1.5/graphique/service.py` & `graphique-1.6/graphique/service.py`

 * *Files identical despite different names*

### Comparing `graphique-1.5/graphique/shell.py` & `graphique-1.6/graphique/shell.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 multiple parts per fragment.
 
 Second, the partitioned dataset is rewritten to merge parts. Often the built-in `write_dataset` is
 sufficient once partitioned, but there is a `fragments` option to optimize for memory or show
 progress on the second pass.
 """
 
-import argparse
 import shutil
-from collections.abc import Iterable
 from pathlib import Path
+from typing import Annotated
 import pyarrow.dataset as ds
+import typer  # type: ignore
 from tqdm import tqdm  # type: ignore
 
 
 def sort_key(name: str) -> tuple:
     """Parse sort order."""
     return name.lstrip('-'), ('descending' if name.startswith('-') else 'ascending')
 
@@ -41,38 +41,29 @@
     for path in tqdm(exprs, desc="Fragments"):
         part_dir = Path(base_dir, *path.parts[-offset:])
         part = dataset.filter(exprs[path])
         ds.write_dataset(part.sort_by(sorting) if sorting else part, part_dir, **options)
 
 
 def partition(
-    scanner: ds.Scanner,
-    base_dir: str,
-    *partitioning: str,
-    fragments: bool = False,
-    sort: Iterable[str] = (),
-    **options,
+    src: Annotated[str, typer.Argument(help="source path")],
+    dest: Annotated[str, typer.Argument(help="destination path")],
+    partitioning: Annotated[list[str], typer.Argument(help="partition keys")],
+    fragments: Annotated[bool, typer.Option(help="iterate over fragments")] = False,
+    sort: Annotated[list[str], typer.Option(help="sort keys; will load fragments")] = [],
 ):
     """Partition dataset by keys."""
-    temp = Path(base_dir) / 'temp'
-    write_batches(scanner, str(temp), *partitioning)
+    temp = Path(dest) / 'temp'
+    write_batches(ds.dataset(src, partitioning='hive'), str(temp), *partitioning)
     dataset = ds.dataset(temp, partitioning='hive')
+    options = dict(partitioning_flavor='hive', existing_data_behavior='overwrite_or_ignore')
     if fragments or sort:
-        write_fragments(dataset, base_dir, tuple(map(sort_key, sort)), **options)
+        write_fragments(dataset, dest, tuple(map(sort_key, sort)))
     else:
-        options.update(partitioning_flavor='hive', existing_data_behavior='overwrite_or_ignore')
         with tqdm(desc="Partitions"):
-            ds.write_dataset(dataset, base_dir, partitioning=partitioning, **options)
+            ds.write_dataset(dataset, dest, partitioning=partitioning, **options)
     shutil.rmtree(temp)
 
 
-parser = argparse.ArgumentParser(description=__doc__)
-parser.add_argument('src', help="source path")
-parser.add_argument('dest', help="destination path")
-parser.add_argument('partitioning', nargs='+', help="partition keys")
-parser.add_argument('--fragments', action='store_true', help="iterate over fragments")
-parser.add_argument('--sort', nargs='*', default=(), help="sort keys; will load fragments")
-
 if __name__ == '__main__':
-    args = parser.parse_args()
-    dataset = ds.dataset(args.src, partitioning='hive')
-    partition(dataset, args.dest, *args.partitioning, fragments=args.fragments, sort=args.sort)
+    partition.__doc__ = __doc__
+    typer.run(partition)
```

### Comparing `graphique-1.5/graphique.egg-info/PKG-INFO` & `graphique-1.6/graphique.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphique
-Version: 1.5
+Version: 1.6
 Summary: GraphQL service for arrow tables and parquet data sets.
 Author-email: Aric Coady <aric.coady@gmail.com>
 License: Copyright 2022 Aric Coady
         
            Licensed under the Apache License, Version 2.0 (the "License");
            you may not use this file except in compliance with the License.
            You may obtain a copy of the License at
@@ -36,16 +36,16 @@
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: pyarrow>=15
-Requires-Dist: strawberry-graphql[asgi,cli]>=0.198
+Requires-Dist: pyarrow>=16
+Requires-Dist: strawberry-graphql[asgi,cli]>=0.221
 Provides-Extra: server
 Requires-Dist: uvicorn[standard]; extra == "server"
 Provides-Extra: cli
 Requires-Dist: tqdm; extra == "cli"
 
 [![image](https://img.shields.io/pypi/v/graphique.svg)](https://pypi.org/project/graphique/)
 ![image](https://img.shields.io/pypi/pyversions/graphique.svg)
```

### Comparing `graphique-1.5/pyproject.toml` & `graphique-1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -54,14 +54,14 @@
 extend-include = ["*.ipynb"]
 
 [tool.ruff.format]
 preview = true
 quote-style = "preserve"
 
 [[tool.mypy.overrides]]
-module = ["pyarrow.*", "strawberry.*", "starlette.*"]
+module = ["numpy.*", "pyarrow.*", "strawberry.*", "starlette.*"]
 ignore_missing_imports = true
 
 [tool.coverage.run]
 source = ["graphique"]
 branch = true
 omit = ["graphique/shell.py"]
```

### Comparing `graphique-1.5/tests/test_core.py` & `graphique-1.6/tests/test_core.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,29 @@
 import pyarrow as pa
 import pyarrow.compute as pc
 import pytest
 from graphique.core import Agg, ListChunk, Column as C, Table as T
+from graphique.scalars import parse_duration, duration_isoformat
+
+
+def test_duration():
+    assert duration_isoformat(parse_duration('P1Y1M1DT1H1M1.1S')) == 'P13M1DT3661.100000000S'
+    assert duration_isoformat(parse_duration('P1M1DT1H1M1.1S')) == 'P1M1DT3661.100000000S'
+    assert duration_isoformat(parse_duration('P1DT1H1M1.1S')) == 'P1DT3661.100000S'
+    assert duration_isoformat(parse_duration('PT1H1M1.1S')) == 'PT3661.100000S'
+    assert duration_isoformat(parse_duration('PT1M1.1S')) == 'PT61.100000S'
+    assert duration_isoformat(parse_duration('PT1.1S')) == 'PT1.100000S'
+    assert duration_isoformat(parse_duration('PT1S')) == 'PT1S'
+    assert duration_isoformat(parse_duration('P0D')) == 'PT0S'
+    assert duration_isoformat(parse_duration('PT0S')) == 'PT0S'
+    assert duration_isoformat(parse_duration('P-1DT-1H')) == 'P-2DT82800S'
+    with pytest.raises(ValueError):
+        duration_isoformat(parse_duration('T1H'))
+    with pytest.raises(ValueError):
+        duration_isoformat(parse_duration('P1H'))
 
 
 def test_dictionary(table):
     array = table['state'].dictionary_encode()
     assert C.min(array) == 'AK'
     assert C.max(array) == 'WY'
     assert C.min_max(array[:0]) == {'min': None, 'max': None}
```

### Comparing `graphique-1.5/tests/test_dataset.py` & `graphique-1.6/tests/test_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,31 +81,34 @@
     assert data == {'group': {'row': {'county': 'Suffolk'}}}
     data = dsclient.execute(
         '{ group(by: ["state"], aggregate: {one: {name: "county"}}) { row { county } } }'
     )
     assert data['group']['row']['county']
     data = dsclient.execute(
         """{ group(by: ["state"], aggregate: {mean: {name: "zipcode"}}) { slice(length: 1) {
-        column(name: "zipcode") { ... on FloatColumn { values } } } } }""")
+        column(name: "zipcode") { ... on FloatColumn { values } } } } }"""
+    )
     assert data == {'group': {'slice': {'column': {'values': [pytest.approx(12614.62721)]}}}}
     data = dsclient.execute(
         """{ group(by: ["state"], aggregate: {list: {name: "zipcode"}}) { aggregate(mean: {name: "zipcode"}) {
-        slice(length: 1) { column(name: "zipcode") { ... on FloatColumn { values } } } } } }""")
+        slice(length: 1) { column(name: "zipcode") { ... on FloatColumn { values } } } } } }"""
+    )
     assert data == {
         'group': {'aggregate': {'slice': {'column': {'values': [pytest.approx(12614.62721)]}}}}
     }
     data = dsclient.execute("""{ group(aggregate: {min: {alias: "st", name: "state"}}) {
         column(name: "st") { ... on StringColumn { values } } } }""")
     assert data == {'group': {'column': {'values': ['AK']}}}
 
 
 def test_list(partclient):
     data = partclient.execute(
         """{ group(by: "state", aggregate: {distinct: {alias: "counties", name: "county"}}) {
-        tables { row { state } column(name: "counties") { length } } } } """)
+        tables { row { state } column(name: "counties") { length } } } } """
+    )
     (table,) = [table for table in data['group']['tables'] if table['row']['state'] == 'PR']
     assert table == {'row': {'state': 'PR'}, 'column': {'length': 78}}
     data = partclient.execute("""{ group(by: "north", aggregate: {distinct: {name: "west"}}) {
         tables { row { north } columns { west { length } } } } }""")
     tables = data['group']['tables']
     assert {table['row']['north'] for table in tables} == {0, 1}
     assert [table['columns'] for table in tables] == [{'west': {'length': 2}}] * 2
@@ -129,15 +132,16 @@
     assert data == {'group': {'row': {'north': 0, 'zipcode': 96898}}}
     data = partclient.execute(
         '{ group(by: [], aggregate: {min: {name: "state"}}) { length row { state } } }'
     )
     assert data == {'group': {'length': 1, 'row': {'state': 'AK'}}}
     data = partclient.execute(
         """{ group(by: ["north", "west"], aggregate: {distinct: {name: "city"}, mean: {name: "zipcode"}}) {
-        length column(name: "city") { type } } }""")
+        length column(name: "city") { type } } }"""
+    )
     assert data == {'group': {'length': 4, 'column': {'type': 'large_list<item: string>'}}}
     data = partclient.execute("""{ group(by: "north", aggregate: {countDistinct: {name: "west"}}) { 
         column(name: "west") { ... on LongColumn { values } } } }""")
     assert data == {'group': {'column': {'values': [2, 2]}}}
     data = partclient.execute(
         '{ group(by: "north", counts: "c") { column(name: "c") { ... on LongColumn { values } } } }'
     )
@@ -236,22 +240,24 @@
     data = fedclient.execute("""{ zipcodes { scan(columns: {name: "zipcode", cast: "int64"}) {
         join(right: "zip_db", keys: "zipcode", rightKeys: "zip") { length schema { names } } } } }""")
     table = data['zipcodes']['scan']['join']
     assert table['length'] == 41700
     assert set(table['schema']['names']) > {'zipcode', 'timezone', 'latitude'}
     data = fedclient.execute(
         """{ zipcodes { scan(columns: {alias: "zip", name: "zipcode", cast: "int64"}) {
-        join(right: "zip_db", keys: "zip", joinType: "right outer") { length schema { names } } } } }""")
+        join(right: "zip_db", keys: "zip", joinType: "right outer") { length schema { names } } } } }"""
+    )
     table = data['zipcodes']['scan']['join']
     assert table['length'] == 42724
     assert set(table['schema']['names']) > {'zip', 'timezone', 'latitude'}
 
     data = fedclient.execute(
         """{ _entities(representations: {__typename: "ZipcodesTable", zipcode: 90001}) {
-        ... on ZipcodesTable { length row { state } schema { names } } } }""")
+        ... on ZipcodesTable { length row { state } schema { names } } } }"""
+    )
     assert data == {
         '_entities': [{'length': 1, 'row': {'state': 'CA'}, 'schema': {'names': ['state']}}]
     }
     data = fedclient.execute("""{ states { filter(state: {eq: "CA"}) { columns { indices {
         takeFrom(field: "zipcodes") { __typename column(name: "state") { length } } } } } } }""")
     table = data['states']['filter']['columns']['indices']['takeFrom']
     assert table == {'__typename': 'ZipcodesTable', 'column': {'length': 2647}}
```

### Comparing `graphique-1.5/tests/test_models.py` & `graphique-1.6/tests/test_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,16 @@
     assert execute('{ bool { any all } }') == {'bool': {'any': False, 'all': False}}
     assert execute('{ bool { indicesNonzero } }') == {'bool': {'indicesNonzero': []}}
 
     data = executor('{ scan(filter: {xor: [{name: "bool"}, {inv: {name: "bool"}}]}) { length } }')
     assert data == {'scan': {'length': 1}}
     data = executor(
         """{ scan(columns: {alias: "bool", andNot: [{inv: {name: "bool"}}, {name: "bool"}], kleene: true})
-        { columns { bool { values } } } }""")
+        { columns { bool { values } } } }"""
+    )
     assert data == {'scan': {'columns': {'bool': {'values': [True, None]}}}}
 
 
 def test_decimal(executor):
     def execute(query):
         return executor(f'{{ columns {query} }}')['columns']
 
@@ -149,82 +150,91 @@
     data = executor('{ column(name: "float", cast: "int32") { type } }')
     assert data == {'column': {'type': 'int32'}}
     data = executor("""{ scan(columns: {alias: "int32", negate: {checked: true, name: "int32"}}) {
         columns { int32 { values } } } }""")
     assert data == {'scan': {'columns': {'int32': {'values': [0, None]}}}}
     data = executor(
         """{ scan(columns: {alias: "float", coalesce: [{name: "float"}, {name: "int32"}]}) {
-        columns { float { values } } } }""")
+        columns { float { values } } } }"""
+    )
     assert data == {'scan': {'columns': {'float': {'values': [0.0, None]}}}}
     data = executor("""{ scan(columns: {bitWise: {not: {name: "int32"}}, alias: "int32"}) {
         columns { int32 { values } } } }""")
     assert data == {'scan': {'columns': {'int32': {'values': [-1, None]}}}}
     data = executor(
         """{ scan(columns: {bitWise: {or: [{name: "int32"}, {name: "int64"}]}, alias: "int64"}) {
-        columns { int64 { values } } } }""")
+        columns { int64 { values } } } }"""
+    )
     assert data == {'scan': {'columns': {'int64': {'values': [0, None]}}}}
 
 
 @pytest.mark.skipif(sys.version_info < (3, 9), reason="requires python3.9 or pytz")
 def test_datetime(executor):
     for name in ('timestamp', 'date32'):
         data = executor(
             f"""{{ scan(columns: {{alias: "year", temporal: {{year: {{name: "{name}"}}}}}})
-            {{ column(name: "year") {{ ... on LongColumn {{ values }} }} }} }}""")
+            {{ column(name: "year") {{ ... on LongColumn {{ values }} }} }} }}"""
+        )
         assert data == {'scan': {'column': {'values': [1970, None]}}}
         data = executor(
             f"""{{ scan(columns: {{alias: "quarter", temporal: {{quarter: {{name: "{name}"}}}}}})
-            {{ column(name: "quarter") {{ ... on LongColumn {{ values }} }} }} }}""")
+            {{ column(name: "quarter") {{ ... on LongColumn {{ values }} }} }} }}"""
+        )
         assert data == {'scan': {'column': {'values': [1, None]}}}
         data = executor(f"""{{ scan(columns: {{alias: "{name}",
             temporal: {{yearsBetween: [{{name: "{name}"}}, {{name: "{name}"}}]}}}})
             {{ column(name: "{name}") {{ ... on LongColumn {{ values }} }} }} }}""")
         assert data == {'scan': {'column': {'values': [0, None]}}}
     data = executor(
         """{ scan(columns: {alias: "timestamp", temporal: {strftime: {name: "timestamp"}}}) {
-        column(name: "timestamp") { type } } }""")
+        column(name: "timestamp") { type } } }"""
+    )
     assert data == {'scan': {'column': {'type': 'string'}}}
     for name in ('timestamp', 'time32'):
         data = executor(
             f"""{{ scan(columns: {{alias: "hour", temporal: {{hour: {{name: "{name}"}}}}}})
-            {{ column(name: "hour") {{ ... on LongColumn {{ values }} }} }} }}""")
+            {{ column(name: "hour") {{ ... on LongColumn {{ values }} }} }} }}"""
+        )
         assert data == {'scan': {'column': {'values': [0, None]}}}
         data = executor(
             f"""{{ scan(columns: {{alias: "subsecond", temporal: {{subsecond: {{name: "{name}"}}}}}})
-            {{ column(name: "subsecond") {{ ... on FloatColumn {{ values }} }} }} }}""")
+            {{ column(name: "subsecond") {{ ... on FloatColumn {{ values }} }} }} }}"""
+        )
         assert data == {'scan': {'column': {'values': [0.0, None]}}}
         data = executor(f"""{{ scan(columns: {{alias: "hours",
             temporal: {{hoursBetween: [{{name: "{name}"}}, {{name: "{name}"}}]}}}})
             {{ column(name: "hours") {{ ... on LongColumn {{ values }} }} }} }}""")
         assert data == {'scan': {'column': {'values': [0, None]}}}
     with pytest.raises(ValueError):
         executor('{ columns { time64 { between(unit: "hours") { values } } } }')
     data = executor(
         """{ scan(columns: {alias: "timestamp", temporal: {assumeTimezone: {name: "timestamp"}, timezone: "UTC"}}) {
-        columns { timestamp { values } } } }""")
+        columns { timestamp { values } } } }"""
+    )
     dates = data['scan']['columns']['timestamp']['values']
     assert dates == ['1970-01-01T00:00:00+00:00', None]
     data = executor(
         """{ scan(columns: {alias: "time32", temporal: {round: {name: "time32"}, unit: "hour"}}) {
-        columns { time32 { values } } } }""")
+        columns { time32 { values } } } }"""
+    )
     assert data == {'scan': {'columns': {'time32': {'values': ['00:00:00', None]}}}}
 
 
 def test_duration(executor):
     data = executor(
         """{ scan(columns: {alias: "diff", checked: true, subtract: [{name: "timestamp"}, {name: "timestamp"}]})
-        { column(name: "diff") { ... on DurationColumn { unique { values  } } } } }""")
-    assert data == {'scan': {'column': {'unique': {'values': [0.0, None]}}}}
+        { column(name: "diff") { ... on DurationColumn { unique { values } } } } }"""
+    )
+    assert data == {'scan': {'column': {'unique': {'values': ['PT0S', None]}}}}
     data = executor('{ runs(split: [{name: "timestamp", gt: 0.0}]) { length } }')
     assert data == {'runs': {'length': 1}}
     data = executor("""{ scan(columns: {alias: "diff", temporal:
         {monthDayNanoIntervalBetween: [{name: "timestamp"}, {name: "timestamp"}]}})
-        { column(name: "diff") { ... on IntervalColumn { values { months days nanoseconds } } } } }""")
-    value = {'months': 0, 'days': 0, 'nanoseconds': 0}
-    assert data == {'scan': {'column': {'values': [value, None]}}}
+        { column(name: "diff") { ... on DurationColumn { values } } } }""")
+    assert data == {'scan': {'column': {'values': ['PT0S', None]}}}
 
 
 def test_list(executor):
     data = executor('{ columns { list { length type } } }')
     assert data == {'columns': {'list': {'length': 2, 'type': 'list<item: int32>'}}}
     data = executor('{ columns { list { values { length } } } }')
     assert data == {'columns': {'list': {'values': [{'length': 3}, None]}}}
@@ -246,15 +256,16 @@
         columns { list { flatten { ... on FloatColumn { values } } } } } }""")
     assert data == {'apply': {'columns': {'list': {'flatten': {'values': [1.0, None]}}}}}
     data = executor("""{ apply(list: {index: {name: "list", value: 1}}) {
         column(name: "list") { ... on LongColumn { values } } } }""")
     assert data == {'apply': {'column': {'values': [1, -1]}}}
     data = executor(
         """{ scan(columns: {list: {element: [{name: "list"}, {value: 1}]}, alias: "value"}) {
-        column(name: "value") { ... on IntColumn { values } } } }""")
+        column(name: "value") { ... on IntColumn { values } } } }"""
+    )
     assert data == {'scan': {'column': {'values': [1, None]}}}
     data = executor("""{ scan(columns: {list: {slice: {name: "list"}, stop: 1}, alias: "value"}) {
         column(name: "value") { ... on ListColumn { flatten { ... on IntColumn { values } } } } } }""")
     assert data == {'scan': {'column': {'flatten': {'values': [0]}}}}
     data = executor("""{ aggregate(distinct: {name: "list", mode: "only_null"})
         { columns { list { flatten { length } } } } }""")
     assert data['aggregate']['columns']['list'] == {'flatten': {'length': 0}}
@@ -263,20 +274,22 @@
     column = data['apply']['columns']['list']
     assert column == {'values': [{'values': [0, 2]}, None]}
     data = executor('{ apply(list: {mode: {name: "list"}}) { column(name: "list") { type } } }')
     assert data['apply']['column']['type'] == 'large_list<item: struct<mode: int32, count: int64>>'
     data = executor(
         """{ aggregate(stddev: {name: "list"}, variance: {name: "list", alias: "var", ddof: 1}) {
         column(name: "list") { ... on FloatColumn { values } }
-        var: column(name: "var") { ... on FloatColumn { values } } } }""")
+        var: column(name: "var") { ... on FloatColumn { values } } } }"""
+    )
     assert data['aggregate']['column']['values'] == [pytest.approx((2 / 3) ** 0.5), None]
     assert data['aggregate']['var']['values'] == [1, None]
     data = executor(
         """{ runs(by: "int32") { scan(columns: {binary: {join: [{name: "binary"}, {base64: ""}]}, alias: "binary"}) {
-        column(name: "binary") { ... on Base64Column { values } } } } }""")
+        column(name: "binary") { ... on Base64Column { values } } } } }"""
+    )
     assert data == {'runs': {'scan': {'column': {'values': [None]}}}}
     data = executor('{ columns { list { value { type } } } }')
     assert data == {'columns': {'list': {'value': {'type': 'int32'}}}}
     data = executor('{ tables { column(name: "list") { type } } }')
     assert data == {'tables': [{'column': {'type': 'int32'}}, None]}
     data = executor(
         '{ apply(list: {rank: {by: "list"}}) { columns { list { values { length } } } } }'
@@ -314,15 +327,16 @@
         {'columns': {'string': {'values': [None]}}, 'column': {'length': 1}},
     ]
     data = executor("""{ group(by: ["camelId"], aggregate: {countDistinct: {name: "string"}}) {
         column(name: "string") { ... on LongColumn { values } } } }""")
     assert data == {'group': {'column': {'values': [1, 0]}}}
     data = executor(
         """{ scan(columns: {alias: "string", coalesce: [{name: "string"}, {value: ""}]}) {
-        columns { string { values } } } }""")
+        columns { string { values } } } }"""
+    )
     assert data == {'scan': {'columns': {'string': {'values': ['', '']}}}}
 
 
 def test_selections(executor):
     data = executor('{ slice { length } slice { sort(by: "snake_id") { length } } }')
     assert data == {'slice': {'length': 2, 'sort': {'length': 2}}}
     data = executor('{ dropNull { length } }')
@@ -330,15 +344,16 @@
     data = executor('{ dropNull { columns { float { values } } } }')
     assert data == {'dropNull': {'columns': {'float': {'values': [0.0]}}}}
 
 
 def test_conditions(executor):
     data = executor(
         """{ scan(columns: {alias: "bool", ifElse: [{name: "bool"}, {name: "int32"}, {name: "float"}]}) {
-        column(name: "bool") { type } } }""")
+        column(name: "bool") { type } } }"""
+    )
     assert data == {'scan': {'column': {'type': 'float'}}}
     with pytest.raises(ValueError, match="no kernel"):
         executor("""{ scan(columns: {alias: "bool",
             ifElse: [{name: "struct"}, {name: "int32"}, {name: "float"}]}) { type } }""")
 
 
 def test_long(executor):
@@ -348,23 +363,25 @@
 
 def test_base64(executor):
     data = executor("""{ scan(columns: {alias: "binary", binary: {length: {name: "binary"}}}) {
         column(name: "binary") { ...on IntColumn { values } } } }""")
     assert data == {'scan': {'column': {'values': [0, None]}}}
     data = executor(
         """{ scan(columns: {alias: "binary", binary: {repeat: [{name: "binary"}, {value: 2}]}}) {
-        columns { binary { values } } } }""")
+        columns { binary { values } } } }"""
+    )
     assert data == {'scan': {'columns': {'binary': {'values': ['', None]}}}}
     data = executor(
         '{ apply(fillNullForward: {name: "binary"}) { columns { binary { values } } } }'
     )
     assert data == {'apply': {'columns': {'binary': {'values': ['', '']}}}}
     data = executor(
         """{ scan(columns: {alias: "binary", coalesce: [{name: "binary"}, {base64: "Xw=="}]}) {
-        columns { binary { values } } } }""")
+        columns { binary { values } } } }"""
+    )
     assert data == {'scan': {'columns': {'binary': {'values': ['', 'Xw==']}}}}
     data = executor("""{ scan(columns: {alias: "binary", binary: {joinElementWise: [
         {name: "binary"}, {name: "binary"}, {base64: "Xw=="}], nullHandling: "replace"}}) {
         columns { binary { values } } } }""")
     assert data == {'scan': {'columns': {'binary': {'values': ['Xw==', 'Xw==']}}}}
     data = executor("""{ scan(columns: {alias: "binary", binary: {replaceSlice: {name: "binary"}
         start: 0, stop: 1, replacement: "Xw=="}}) { columns { binary { values } } } }""")
```

### Comparing `graphique-1.5/tests/test_service.py` & `graphique-1.6/tests/test_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,19 +44,21 @@
     assert longitudes['min'] == pytest.approx(-174.21333)
     assert longitudes['max'] == pytest.approx(-65.301389)
     data = client.execute('{ columns { latitude { quantile(q: [0.5]) } } }')
     (quantile,) = data['columns']['latitude']['quantile']
     assert quantile == pytest.approx(39.12054)
     data = client.execute(
         """{ scan(columns: {alias: "latitude", elementWise: {min: [{name: "latitude"}, {name: "longitude"}]}}) {
-        columns { latitude { min } } } }""")
+        columns { latitude { min } } } }"""
+    )
     assert data == {'scan': {'columns': {'latitude': {'min': pytest.approx(-174.213333)}}}}
     data = client.execute(
         """{scan(columns: {alias: "l", setLookup: {digitize: [{name: "latitude"}, {value: [40]}]}}) {
-        column(name: "l") { ... on LongColumn { unique { values counts } } } } }""")
+        column(name: "l") { ... on LongColumn { unique { values counts } } } } }"""
+    )
     assert data == {"scan": {"column": {"unique": {"values": [1, 0], "counts": [17955, 23745]}}}}
     data = client.execute(
         '{ scan(columns: {alias: "latitude", log: {logb: [{name: "latitude"}, {value: 3}]}}) { row { latitude } } }'
     )
     assert data == {'scan': {'row': {'latitude': pytest.approx(3.376188)}}}
     data = client.execute(
         '{ scan(columns: {alias: "latitude", rounding: {round: {name: "latitude"}}}) {row { latitude } } }'
@@ -102,62 +104,71 @@
     assert data == {'scan': {'row': {'state': 'Ny'}}}
     data = client.execute('{ scan(filter: {utf8: {isLower: {name: "city"}}}) { length } }')
     assert data == {'scan': {'length': 0}}
     data = client.execute('{ scan(filter: {utf8: {isTitle: {name: "city"}}}) { length } }')
     assert data == {'scan': {'length': 41700}}
     data = client.execute(
         """{ scan(columns: {alias: "city", substring: {match: {name: "city"}, pattern: "Mountain"}})
-        { scan(filter: {name: "city"}) { length } } }""")
+        { scan(filter: {name: "city"}) { length } } }"""
+    )
     assert data == {'scan': {'scan': {'length': 88}}}
     data = client.execute(
         """{ scan(filter: {substring: {match: {name: "city"}, pattern: "mountain", ignoreCase: true}})
-        { length } }""")
+        { length } }"""
+    )
     assert data == {'scan': {'length': 88}}
     data = client.execute(
         """{ scan(filter: {substring: {match: {name: "city"}, pattern: "^Mountain", regex: true}})
-        { length } }""")
+        { length } }"""
+    )
     assert data == {'scan': {'length': 42}}
     data = client.execute(
         """{ scan(columns: {alias: "idx", setLookup: {indexIn: [{name: "state"}, {value: ["CA", "OR"]}]}})
-        { column(name: "idx") { ... on IntColumn { unique { values } } } } }""")
+        { column(name: "idx") { ... on IntColumn { unique { values } } } } }"""
+    )
     assert data == {'scan': {'column': {'unique': {'values': [None, 0, 1]}}}}
 
 
 def test_string_methods(client):
     data = client.execute(
         """{ scan(columns: {alias: "split", substring: {split: {name: "city"}, pattern: "-", maxSplits: 1}}) {
-        column(name: "split") { type } } }""")
+        column(name: "split") { type } } }"""
+    )
     assert data == {'scan': {'column': {'type': 'list<item: string>'}}}
     data = client.execute("""{ scan(columns: {alias: "split", substring: {split: {name: "city"}}}) {
         column(name: "split") { type } } }""")
     assert data == {'scan': {'column': {'type': 'list<item: string>'}}}
     data = client.execute(
         """{ scan(columns: {alias: "state", utf8: {trim: {name: "state"}, characters: "C"}}) {
-        columns { state { values } } } }""")
+        columns { state { values } } } }"""
+    )
     states = data['scan']['columns']['state']['values']
     assert 'CA' not in states and 'A' in states
     data = client.execute(
         '{ scan(columns: {alias: "state", utf8: {ltrim: {name: "state"}}}) { length } }'
     )
     assert data == {'scan': {'length': 41700}}
     data = client.execute(
         """{ scan(columns: {alias: "state", utf8: {center: {name: "state"}, width: 4, padding: "_"}})
-        { row { state } } }""")
+        { row { state } } }"""
+    )
     assert data == {'scan': {'row': {'state': '_NY_'}}}
     data = client.execute(
         """{ scan(columns: {alias: "state", utf8: {replaceSlice: {name: "state"}, start: 0, stop: 2, replacement: ""}})
-        { columns { state { unique { values } } } } }""")
+        { columns { state { unique { values } } } } }"""
+    )
     assert data == {'scan': {'columns': {'state': {'unique': {'values': ['']}}}}}
     data = client.execute(
         '{ scan(columns: {alias: "state", utf8: {sliceCodeunits: {name: "state"}, start: 0, stop: 1}}) { row { state } } }'
     )
     assert data == {'scan': {'row': {'state': 'N'}}}
     data = client.execute(
         """{ scan(columns: {alias: "state", substring: {replace: {name: "state"}, pattern: "C", replacement: "A"}})
-        { columns { state { values } } } }""")
+        { columns { state { values } } } }"""
+    )
     assert 'AA' in data['scan']['columns']['state']['values']
 
 
 def test_search(client):
     data = client.execute('{ schema { index } filter { length } }')
     assert data == {'schema': {'index': ['zipcode']}, 'filter': {'length': 41700}}
     data = client.execute('{ filter(zipcode: {eq: 501}) { columns { zipcode { values } } } }')
@@ -209,23 +220,26 @@
     data = client.execute('{ scan(filter: {eq: [{name: "county"}, {name: "city"}]}) { length } }')
     assert data['scan']['length'] == 2805
     data = client.execute("""{ scan(filter: {or: [{eq: [{name: "state"}, {name: "county"}]},
         {eq: [{name: "county"}, {name: "city"}]}]}) { length } }""")
     assert data['scan']['length'] == 2805
     data = client.execute(
         """{ scan(columns: {alias: "zipcode", add: [{name: "zipcode"}, {name: "zipcode"}]})
-        { columns { zipcode { min } } } }""")
+        { columns { zipcode { min } } } }"""
+    )
     assert data['scan']['columns']['zipcode']['min'] == 1002
     data = client.execute(
         """{ scan(columns: {alias: "zipcode", subtract: [{name: "zipcode"}, {name: "zipcode"}]})
-        { columns { zipcode { unique { values } } } } }""")
+        { columns { zipcode { unique { values } } } } }"""
+    )
     assert data['scan']['columns']['zipcode']['unique']['values'] == [0]
     data = client.execute(
         """{ scan(columns: {alias: "product", multiply: [{name: "latitude"}, {name: "longitude"}]})
-        { scan(filter: {gt: [{name: "product"}, {value: 0}]}) { length } } }""")
+        { scan(filter: {gt: [{name: "product"}, {value: 0}]}) { length } } }"""
+    )
     assert data['scan']['scan']['length'] == 0
     data = client.execute(
         '{ scan(columns: {name: "zipcode", cast: "float"}) { column(name: "zipcode") { type } } }'
     )
     assert data['scan']['column']['type'] == 'float'
     data = client.execute(
         '{ scan(filter: {inv: {eq: [{name: "state"}, {value: "CA"}]}}) { length } }'
@@ -233,34 +247,39 @@
     assert data == {'scan': {'length': 39053}}
     data = client.execute(
         '{ scan(columns: {name: "latitude", cast: "int32", safe: false}) { column(name: "latitude") { type } } }'
     )
     assert data == {'scan': {'column': {'type': 'int32'}}}
     data = client.execute(
         """{ scan(columns: {alias: "longitude", elementWise: {max: [{name: "longitude"}, {name: "latitude"}]}})
-        { columns { longitude { min } } } }""")
+        { columns { longitude { min } } } }"""
+    )
     assert data['scan']['columns']['longitude']['min'] == pytest.approx(17.963333)
     data = client.execute(
         """{ scan(columns: {alias: "latitude", elementWise: {min: [{name: "longitude"}, {name: "latitude"}]}})
-        { columns { latitude { max } } } }""")
+        { columns { latitude { max } } } }"""
+    )
     assert data['scan']['columns']['latitude']['max'] == pytest.approx(-65.301389)
     data = client.execute(
         """{ scan(columns: {alias: "state", elementWise: {min: [{name: "state"}, {name: "county"}], skipNulls: false}})
-        { columns { state { values } } } }""")
+        { columns { state { values } } } }"""
+    )
     assert data['scan']['columns']['state']['values'][0] == 'NY'
 
 
 def test_apply(client):
     data = client.execute(
         """{ scan(columns: {alias: "city", substring: {find: {name: "city"}, pattern: "mountain"}})
-        { column(name: "city") { ... on IntColumn { unique { values } } } } }""")
+        { column(name: "city") { ... on IntColumn { unique { values } } } } }"""
+    )
     assert data['scan']['column']['unique']['values'] == [-1]
     data = client.execute(
         """{ scan(columns: {alias: "city", substring: {count: {name: "city"}, pattern: "mountain", ignoreCase: true}})
-        { column(name: "city") { ... on IntColumn { unique { values } } } } }""")
+        { column(name: "city") { ... on IntColumn { unique { values } } } } }"""
+    )
     assert data['scan']['column']['unique']['values'] == [0, 1]
     data = client.execute("""{ scan(columns: {alias: "state", binary: {joinElementWise: [
         {name: "state"}, {name: "county"}, {value: " "}]}}) { columns { state { values } } } }""")
     assert data['scan']['columns']['state']['values'][0] == 'NY Suffolk'
     data = client.execute("""{ apply(cumulativeSum: {name: "zipcode", skipNulls: false})
         { columns { zipcode { value(index: -1) } } } }""")
     assert data == {'apply': {'columns': {'zipcode': {'value': 2066562337}}}}
@@ -271,15 +290,16 @@
         '{ apply(pairwiseDiff: {name: "zipcode"}) { columns { zipcode { value } } } }'
     )
     assert data == {'apply': {'columns': {'zipcode': {'value': None}}}}
     data = client.execute('{ apply(rank: {name: "zipcode"}) { row { zipcode } } }')
     assert data == {'apply': {'row': {'zipcode': 1}}}
     data = client.execute(
         """{ apply(rank: {name: "zipcode", sortKeys: "descending", nullPlacement: "at_start", tiebreaker: "dense"})
-        { row { zipcode } } }""")
+        { row { zipcode } } }"""
+    )
     assert data == {'apply': {'row': {'zipcode': 41700}}}
 
 
 def test_sort(client):
     with pytest.raises(ValueError, match="is required"):
         client.execute('{ sort { columns { state { values } } } }')
     data = client.execute('{ sort(by: ["state"]) { columns { state { values } } } }')
@@ -296,55 +316,61 @@
         """{ sort(by: ["-state", "-county"], length: 1) { columns { county { values } } } }"""
     )
     assert data['sort']['columns']['county']['values'] == ['Weston']
     data = client.execute('{ sort(by: ["state"], length: 2) { columns { state { values } } } }')
     assert data['sort']['columns']['state']['values'] == ['AK', 'AK']
     data = client.execute(
         """{ group(by: ["state"], aggregate: {list: {name: "county"}}) { apply(list: {sort: {by: ["county"]}})
-        { aggregate(first: [{name: "county"}]) { row { state county } } } } }""")
+        { aggregate(first: [{name: "county"}]) { row { state county } } } } }"""
+    )
     assert data['group']['apply']['aggregate']['row'] == {'state': 'NY', 'county': 'Albany'}
     data = client.execute(
         """{ group(by: ["state"], aggregate: {list: {name: "county"}}) { apply(list: {sort: {by: ["-county"], length: 1}})
-        { aggregate(first: [{name: "county"}]) { row { state county } } } } }""")
+        { aggregate(first: [{name: "county"}]) { row { state county } } } } }"""
+    )
     assert data['group']['apply']['aggregate']['row'] == {'state': 'NY', 'county': 'Yates'}
     data = client.execute(
         """{ group(by: ["state"], aggregate: {list: {name: "county"}}) { apply(list: {sort: {by: "county", length: 2}})
-        { row { state } column(name: "county") { ... on ListColumn { value { length } } } } } }""")
+        { row { state } column(name: "county") { ... on ListColumn { value { length } } } } } }"""
+    )
     assert data['group']['apply'] == {'row': {'state': 'NY'}, 'column': {'value': {'length': 2}}}
 
 
 def test_group(client):
     with pytest.raises(ValueError, match="list"):
         client.execute('{ group(by: ["state"]) { tables { length } } }')
     with pytest.raises(ValueError, match="cannot represent"):
         client.execute('{ group(by: "state", aggregate: {list: {name: "city"}}) { row { city } } }')
     data = client.execute(
         """{ group(by: ["state"], aggregate: {list: {name: "county"}}) { length tables { length
         columns { state { values } county { min max } } }
         scan(columns: {list: {valueLength: {name: "county"}}, alias: "c"}) {
-        column(name: "c") { ... on IntColumn { values } } } } }""")
+        column(name: "c") { ... on IntColumn { values } } } } }"""
+    )
     assert len(data['group']['tables']) == data['group']['length'] == 52
     table = data['group']['tables'][0]
     assert table['length'] == data['group']['scan']['column']['values'][0] == 2205
     assert set(table['columns']['state']['values']) == {'NY'}
     assert table['columns']['county'] == {'min': 'Albany', 'max': 'Yates'}
     data = client.execute(
         """{ group(by: ["state", "county"], counts: "counts", aggregate: {list: {name: "city"}}) {
         scan(filter: {gt: [{name: "counts"}, {value: 200}]}) {
         aggregate(min: [{name: "city", alias: "min"}], max: [{name: "city", alias: "max"}]) {
         min: column(name: "min") { ... on StringColumn { values } }
-        max: column(name: "max") { ... on StringColumn { values } } } } } }""")
+        max: column(name: "max") { ... on StringColumn { values } } } } } }"""
+    )
     agg = data['group']['scan']['aggregate']
     assert agg['min']['values'] == ['Naval Anacost Annex', 'Alsip', 'Alief', 'Acton']
     assert agg['max']['values'] == ['Washington Navy Yard', 'Worth', 'Webster', 'Woodland Hills']
     data = client.execute(
         """{ group(by: ["state", "county"], counts: "c", aggregate: {list: [{name: "zipcode"}, {name: "latitude"}, {name: "longitude"}]}) {
         sort(by: ["-c"], length: 4) { aggregate(sum: [{name: "latitude"}], mean: [{name: "longitude"}]) {
         columns { latitude { values } longitude { values } }
-        column(name: "zipcode") { type } } } } }""")
+        column(name: "zipcode") { type } } } } }"""
+    )
     agg = data['group']['sort']['aggregate']
     assert agg['column']['type'] == 'list<item: int32>'
     assert all(latitude > 1000 for latitude in agg['columns']['latitude']['values'])
     assert all(77 > longitude > -119 for longitude in agg['columns']['longitude']['values'])
     data = client.execute("""{ scan(columns: {name: "zipcode", cast: "bool"})
         { group(by: ["state"], aggregate: {list: {name: "zipcode"}}) { slice(length: 3) {
         scan(columns: [{alias: "a", list: {any: {name: "zipcode"}}}, {alias: "b", list: {all: {name: "zipcode"}}}]) {
@@ -364,41 +390,44 @@
 def test_flatten(client):
     data = client.execute(
         '{ group(by: "state", aggregate: {list: {name: "city"}}) { flatten { columns { city { type } } } } }'
     )
     assert data == {'group': {'flatten': {'columns': {'city': {'type': 'string'}}}}}
     data = client.execute(
         """{ group(by: "state", aggregate: {list: {name: "city"}}) { flatten(indices: "idx") { columns { city { type } }
-        column(name: "idx") { ... on LongColumn { unique { values counts } } } } } }""")
+        column(name: "idx") { ... on LongColumn { unique { values counts } } } } } }"""
+    )
     idx = data['group']['flatten']['column']['unique']
     assert idx['values'] == list(range(52))
     assert sum(idx['counts']) == 41700
     assert idx['counts'][0] == 2205
 
 
 def test_aggregate(client):
     data = client.execute(
         """{ group(by: ["state"] counts: "c", aggregate: {first: [{name: "county"}]
         countDistinct: [{name: "city", alias: "cd"}]}) { slice(length: 3) {
         c: column(name: "c") { ... on LongColumn { values } }
         cd: column(name: "cd") { ... on LongColumn { values } }
-        columns { state { values } county { values } } } } }""")
+        columns { state { values } county { values } } } } }"""
+    )
     assert data['group']['slice'] == {
         'c': {'values': [2205, 176, 703]},
         'cd': {'values': [1612, 99, 511]},
         'columns': {
             'state': {'values': ['NY', 'PR', 'MA']},
             'county': {'values': ['Suffolk', 'Adjuntas', 'Hampden']},
         },
     }
     data = client.execute(
         """{ group(by: ["state", "county"], aggregate: {list: {name: "city"}, min: {name: "city", alias: "first"}}) {
         aggregate(max: {name: "city", alias: "last"}) { slice(length: 3) {
         first: column(name: "first") { ... on StringColumn { values } }
-        last: column(name: "last") { ... on StringColumn { values } } } } } }""")
+        last: column(name: "last") { ... on StringColumn { values } } } } } }"""
+    )
     assert data['group']['aggregate']['slice'] == {
         'first': {'values': ['Amagansett', 'Adjuntas', 'Aguada']},
         'last': {'values': ['Yaphank', 'Adjuntas', 'Aguada']},
     }
 
 
 def test_runs(client):
```

