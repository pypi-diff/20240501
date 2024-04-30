# Comparing `tmp/coherence_client-1.0rc2.tar.gz` & `tmp/coherence_client-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coherence_client-1.0rc2.tar", max compression
+gzip compressed data, was "coherence_client-1.1.0.tar", max compression
```

## Comparing `coherence_client-1.0rc2.tar` & `coherence_client-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1839 2023-06-16 15:02:06.453365 coherence_client-1.0rc2/LICENSE.txt
--rw-r--r--   0        0        0     4548 2023-06-16 15:02:06.455855 coherence_client-1.0rc2/README.md
--rw-r--r--   0        0        0     1995 2023-06-23 17:54:28.141523 coherence_client-1.0rc2/pyproject.toml
--rw-r--r--   0        0        0      986 2023-06-23 17:54:28.144153 coherence_client-1.0rc2/src/coherence/__init__.py
--rw-r--r--   0        0        0    33819 2023-06-16 15:02:06.482799 coherence_client-1.0rc2/src/coherence/aggregator.py
--rw-r--r--   0        0        0    62507 2023-06-21 16:52:55.727619 coherence_client-1.0rc2/src/coherence/client.py
--rw-r--r--   0        0        0     1060 2023-06-16 15:02:06.484749 coherence_client-1.0rc2/src/coherence/comparator.py
--rw-r--r--   0        0        0    31397 2023-06-16 15:02:06.485414 coherence_client-1.0rc2/src/coherence/event.py
--rw-r--r--   0        0        0    11175 2023-06-16 15:02:06.486394 coherence_client-1.0rc2/src/coherence/extractor.py
--rw-r--r--   0        0        0    36712 2023-06-16 15:02:06.487527 coherence_client-1.0rc2/src/coherence/filter.py
--rw-r--r--   0        0        0    11698 2023-06-16 15:02:06.489543 coherence_client-1.0rc2/src/coherence/messages_pb2.py
--rw-r--r--   0        0        0      159 2023-06-16 15:02:06.490115 coherence_client-1.0rc2/src/coherence/messages_pb2_grpc.py
--rw-r--r--   0        0        0    33851 2023-06-16 15:02:06.491241 coherence_client-1.0rc2/src/coherence/processor.py
--rw-r--r--   0        0        0     9917 2023-06-16 15:02:06.492224 coherence_client-1.0rc2/src/coherence/serialization.py
--rw-r--r--   0        0        0     4040 2023-06-16 15:02:06.492853 coherence_client-1.0rc2/src/coherence/services_pb2.py
--rw-r--r--   0        0        0    45397 2023-06-16 15:02:06.493204 coherence_client-1.0rc2/src/coherence/services_pb2_grpc.py
--rw-r--r--   0        0        0    11918 2023-06-16 15:02:06.493808 coherence_client-1.0rc2/src/coherence/util.py
--rw-r--r--   0        0        0     5487 1970-01-01 00:00:00.000000 coherence_client-1.0rc2/PKG-INFO
+-rw-r--r--   0        0        0     1839 2024-04-30 22:39:15.460961 coherence_client-1.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     4794 2024-04-30 22:39:15.460961 coherence_client-1.1.0/README.md
+-rw-r--r--   0        0        0     2053 2024-04-30 22:39:15.460961 coherence_client-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1090 2024-04-30 22:39:15.460961 coherence_client-1.1.0/src/coherence/__init__.py
+-rw-r--r--   0        0        0    33785 2024-04-30 22:39:15.460961 coherence_client-1.1.0/src/coherence/aggregator.py
+-rw-r--r--   0        0        0    71570 2024-04-30 22:39:15.460961 coherence_client-1.1.0/src/coherence/client.py
+-rw-r--r--   0        0        0     1468 2024-04-30 22:39:15.460961 coherence_client-1.1.0/src/coherence/comparator.py
+-rw-r--r--   0        0        0    31490 2024-04-30 22:39:15.460961 coherence_client-1.1.0/src/coherence/event.py
+-rw-r--r--   0        0        0    13494 2024-04-30 22:39:15.464961 coherence_client-1.1.0/src/coherence/extractor.py
+-rw-r--r--   0        0        0    36730 2024-04-30 22:39:15.464961 coherence_client-1.1.0/src/coherence/filter.py
+-rw-r--r--   0        0        0    11698 2024-04-30 22:39:15.464961 coherence_client-1.1.0/src/coherence/messages_pb2.py
+-rw-r--r--   0        0        0      159 2024-04-30 22:39:15.464961 coherence_client-1.1.0/src/coherence/messages_pb2_grpc.py
+-rw-r--r--   0        0        0    33984 2024-04-30 22:39:15.464961 coherence_client-1.1.0/src/coherence/processor.py
+-rw-r--r--   0        0        0    10395 2024-04-30 22:39:15.464961 coherence_client-1.1.0/src/coherence/serialization.py
+-rw-r--r--   0        0        0     4040 2024-04-30 22:39:15.464961 coherence_client-1.1.0/src/coherence/services_pb2.py
+-rw-r--r--   0        0        0    45397 2024-04-30 22:39:15.464961 coherence_client-1.1.0/src/coherence/services_pb2_grpc.py
+-rw-r--r--   0        0        0    12807 2024-04-30 22:39:15.464961 coherence_client-1.1.0/src/coherence/util.py
+-rw-r--r--   0        0        0     5993 1970-01-01 00:00:00.000000 coherence_client-1.1.0/PKG-INFO
```

### Comparing `coherence_client-1.0rc2/LICENSE.txt` & `coherence_client-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `coherence_client-1.0rc2/README.md` & `coherence_client-1.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Coherence Python Client
 
 ![CI/CD](https://github.com/oracle/coherence-py-client/actions/workflows/validate.yml/badge.svg)
+[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=oracle_coherence-py-client&metric=alert_status)](https://sonarcloud.io/project/overview?id=oracle_coherence-py-client)
 [![License](http://img.shields.io/badge/license-UPL%201.0-blue.svg)](https://oss.oracle.com/licenses/upl/)
 
 <img src=https://oracle.github.io/coherence/assets/images/logo-red.png width="30%"><img>
 
 The Coherence Python Client allows Python applications to act as cache clients to an Oracle Coherence cluster using gRPC as the network transport.
 
 #### Features
@@ -16,25 +17,25 @@
     * mutations such as insert, update and delete on Maps
     * map lifecycle events such as truncated, released or destroyed
     * session lifecycle events such as connected, disconnected, reconnected and closed
 * Support for storing Python objects as JSON as well as the ability to serialize to Java objects on the server for access from other Coherence language API's
 
 #### Requirements
 * [Coherence CE](https://github.com/oracle/coherence) 22.06.4+ or Coherence 14.1.1.2206.4+ Commercial edition with a configured [gRPCProxy](https://docs.oracle.com/en/middleware/standalone/coherence/14.1.1.2206/develop-remote-clients/using-coherence-grpc-server.html).
-* Python 3.11.x
+* Python 3.8.x
 
 
 #### Starting a Coherence Cluster
 
 Before testing the Python client, you must ensure a Coherence cluster is available.
 For local development, we recommend using the Coherence CE Docker image; it contains
 everything necessary for the client to operate correctly.
 
 ```bash
-docker run -d -p 1408:1408 ghcr.io/oracle/coherence-ce:22.06.4
+docker run -d -p 1408:1408 ghcr.io/oracle/coherence-ce:24.03
 ```
 
 ## Installation
 
 ```bash
 python3 -m pip install coherence-client
 ```
@@ -48,23 +49,24 @@
 The following example connects to a Coherence cluster running gRPC Proxy on default
 port of 1408, creates a new `NamedCache` with key `str` and value of a `str|int` and
 issues `put()`, `get()`, `size()` and `remove` operations.
 
 ```python
 from coherence import NamedCache, Session
 import asyncio
+from typing import Union
 
 
 async def run_test():
 
     # create a new Session to the Coherence server
     session: Session = await Session.create()
 
     # create a new NamedCache with key of string|int and value of string|int
-    cache: NamedCache[str, str|int] = await session.get_cache("test")
+    cache: NamedCache[str, Union[str,int]] = await session.get_cache("test")
 
     # put a new key/value
     k: str = "one"
     v: str = "only-one"
     await cache.put(k, v)
 
     # get the value for a key in the cache
@@ -87,15 +89,15 @@
 
 
 # run the test
 asyncio.run(run_test())
 ```
 ## Help
 
-We have a **public Slack channel** where you can get in touch with us to ask questions about using the Coherence CLI
+We have a **public Slack channel** where you can get in touch with us to ask questions about using the Coherence Python Client
 or give us feedback or suggestions about what features and improvements you would like to see. We would love
 to hear from you. To join our channel,
 please [visit this site to get an invitation](https://join.slack.com/t/oraclecoherence/shared_invite/enQtNzcxNTQwMTAzNjE4LTJkZWI5ZDkzNGEzOTllZDgwZDU3NGM2YjY5YWYwMzM3ODdkNTU2NmNmNDFhOWIxMDZlNjg2MzE3NmMxZWMxMWE).
 The invitation email will include details of how to access our Slack
 workspace.  After you are logged in, please come to `#coherence` and say, "hello!"
 
 If you would like to raise an issue please see [here](https://github.com/oracle/coherence-py-client/issues/new/choose).
@@ -106,11 +108,11 @@
 
 ## Security
 
 Please consult the [security guide](./SECURITY.md) for our responsible security vulnerability disclosure process
 
 ## License
 
-Copyright (c) 2023 Oracle and/or its affiliates.
+Copyright (c) 2023, 2024, Oracle and/or its affiliates.
 
 Released under the Universal Permissive License v1.0 as shown at
 <https://oss.oracle.com/licenses/upl/>.
```

### Comparing `coherence_client-1.0rc2/pyproject.toml` & `coherence_client-1.1.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,45 +1,46 @@
-# Copyright (c) 2022, Oracle and/or its affiliates.
+# Copyright (c) 2022, 2024, Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at
 # https://oss.oracle.com/licenses/upl.
 [tool.poetry]
 name = "coherence-client"
-version = "1.0rc2"
+version = "1.1.0"
 description = """The Coherence Python Client allows Python applications to act as cache clients to a \
 Coherence Cluster using Google's gRPC framework as the network transport."""
 packages = [
     { include = "coherence", from = "./src"},
 ]
 readme = "README.md"
 authors = ["Oracle <dhiru.pandey@oracle.com>"]
 homepage = "https://github.com/oracle/coherence-py-client"
 repository = "https://github.com/oracle/coherence-py-client"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Universal Permissive License (UPL)",
     "Operating System :: OS Independent",
-    "Development Status :: 4 - Beta",
+    "Development Status :: 5 - Production/Stable",
 ]
 
 [tool.poetry.dependencies]
-python = "~3.11"
-protobuf = "~4.23"
-grpcio = ">=1.54,<1.57"
-grpcio-tools = ">=1.54,<1.57"
+python = "^3.8"
+protobuf = ">=4.23,<4.26"
+grpcio = ">=1.54,<1.63"
+grpcio-tools = ">=1.54,<1.63"
 jsonpickle = "~3.0"
-pymitter = "~0.4"
+pymitter = ">=0.4,<0.6"
+typing-extensions = "~4.11"
 
 [tool.poetry.dev-dependencies]
-pytest = "~7.3"
-pytest-asyncio = "~0.21"
-pytest-cov = "~4.1"
-pytest-unordered = "~0.5"
-pre-commit = "~3.3"
-Sphinx = "~6.2"
-sphinx-rtd-theme = "~1.2"
+pytest = "~8.2"
+pytest-asyncio = "~0.23"
+pytest-cov = "~5.0"
+pytest-unordered = "~0.6"
+pre-commit = "~3.5"
+Sphinx = "~7.1"
+sphinx-rtd-theme = "~2.0"
 sphinxcontrib-napoleon = "~0.7"
 m2r = "~0.3"
 third-party-license-file-generator = "~2023.2"
 
 [tool.pytest.ini_options]
 pythonpath = ["src"]
```

### Comparing `coherence_client-1.0rc2/src/coherence/__init__.py` & `coherence_client-1.1.0/src/coherence/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 Oracle and/or its affiliates.
+# Copyright (c) 2022, 2024, Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at
 # https://oss.oracle.com/licenses/upl.
 
 from __future__ import annotations
 
 __version__ = "1.0rc2"
 
@@ -12,14 +12,16 @@
 from .aggregator import Aggregators as Aggregators
 from .client import MapEntry as MapEntry
 from .client import NamedCache as NamedCache
 from .client import NamedMap as NamedMap
 from .client import Options as Options
 from .client import Session as Session
 from .client import TlsOptions as TlsOptions
+from .comparator import Comparator as Comparator
+from .extractor import Extractors as Extractors
 from .filter import Filters as Filters
 from .processor import Processors as Processors
 
 # default logging configuration for coherence
 handler: logging.StreamHandler = logging.StreamHandler()  # type: ignore
 handler.setFormatter(logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s"))
```

### Comparing `coherence_client-1.0rc2/src/coherence/aggregator.py` & `coherence_client-1.1.0/src/coherence/aggregator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,33 @@
-# Copyright (c) 2022, 2023, Oracle and/or its affiliates.
+# Copyright (c) 2022, 2024, Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at
 # https://oss.oracle.com/licenses/upl.
 
 from __future__ import annotations
 
 from abc import ABC
 from decimal import Decimal
 from enum import Enum, IntEnum
-from typing import Any, Dict, Generic, List, Optional, TypeAlias, TypeVar
+from typing import Any, Dict, Generic, List, Optional, TypeVar, Union
+
+from typing_extensions import TypeAlias
 
 from .comparator import Comparator, InverseComparator, SafeComparator
-from .extractor import ExtractorExpression, IdentityExtractor, ValueExtractor, extract
+from .extractor import ExtractorExpression, Extractors, ValueExtractor
 from .filter import Filter
 from .serialization import proxy
 
 E = TypeVar("E")
 G = TypeVar("G")
 K = TypeVar("K")
 R = TypeVar("R")
 T = TypeVar("T")
 V = TypeVar("V")
 
-ReducerResult: TypeAlias = Dict[K, Any | List[Any]]
+ReducerResult: TypeAlias = Dict[K, Union[Any, List[Any]]]
 
 
 class EntryAggregator(ABC, Generic[R]):
     """An EntryAggregator represents processing that can be directed to occur against some subset of the entries in
     n cache, resulting in an aggregated result. Common examples of aggregation include functions such as min(),
     max() and avg(). However, the concept of aggregation applies to any process that needs to evaluate a group of
     entries to come up with a single answer."""
@@ -41,15 +43,15 @@
             :class:`coherence.extractor.UniversalExtractor` objects; must not be `None`
         """
         super().__init__()
         if extractor_or_property is not None:
             if isinstance(extractor_or_property, ValueExtractor):
                 self.extractor = extractor_or_property
             else:
-                self.extractor = extract(extractor_or_property)
+                self.extractor = Extractors.extract(extractor_or_property)
 
     def and_then(self, aggregator: EntryAggregator[R]) -> EntryAggregator[List[R]]:
         """
         Returns a :class:`coherence.aggregator.CompositeAggregator` comprised of this and the provided aggregator.
 
         :param aggregator: the next aggregator
         :return: a :class:`coherence.aggregator.CompositeAggregator` comprised of this and the provided aggregator
@@ -237,15 +239,15 @@
     """`TopAggregator` aggregates the top *N* extracted values into an array.  The extracted values must not be
     `None`, but do not need to be unique."""
 
     def __init__(
         self,
         number: int = 0,
         inverse: bool = False,
-        extractor: ValueExtractor[Any, Any] = IdentityExtractor(),
+        extractor: ValueExtractor[Any, Any] = Extractors.identity(),
         comparator: Optional[Comparator] = None,
         property_name: Optional[str] = None,
     ):
         """
         Constructs a new `TopAggregator`.
 
         :param number: the maximum number of results to include in the aggregation result.
@@ -300,16 +302,15 @@
     def extract(self, property_name: str) -> TopAggregator[E, R]:
         """
         The property name of the value to extract.
 
         :param property_name: the property name
         :return:
         """
-        self.inverse = True  # TODO why is this True?
-        self.extractor = ValueExtractor.extract(property_name)
+        self.extractor = Extractors.extract(property_name)
         return self
 
 
 @proxy("aggregator.GroupAggregator")
 class GroupAggregator(EntryAggregator[R]):
     """The `GroupAggregator` provides an ability to split a subset of entries in a Map into a collection of
     non-intersecting subsets and then aggregate them separately and independently. The splitting (grouping) is
@@ -531,19 +532,18 @@
         :param query_type: the type for this aggregator
         """
         super().__init__()
         self.type = QueryRecorder.get_type(query_type)
 
     @classmethod
     def get_type(cls, query_type: RecordType) -> dict[str, str]:
-        match query_type:
-            case RecordType.EXPLAIN:
-                return {"enum": cls.EXPLAIN}
-            case RecordType.TRACE:
-                return {"enum": cls.TRACE}
+        if query_type == RecordType.EXPLAIN:
+            return {"enum": cls.EXPLAIN}
+        elif query_type == RecordType.TRACE:
+            return {"enum": cls.TRACE}
 
 
 @proxy("aggregator.ReducerAggregator")
 class ReducerAggregator(EntryAggregator[R]):
     """The `ReducerAggregator` is used to implement functionality similar to :class:`coherence.client.NamedMap.getAll(
     )` API.  Instead of returning the complete set of values, it will return a portion of value attributes based on
     the provided :class:`coherence.extractor.ValueExtractor`.
```

### Comparing `coherence_client-1.0rc2/src/coherence/client.py` & `coherence_client-1.1.0/src/coherence/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-# Copyright (c) 2022, 2023, Oracle and/or its affiliates.
+# Copyright (c) 2022, 2024, Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at
 # https://oss.oracle.com/licenses/upl.
 
 from __future__ import annotations
 
 import abc
 import asyncio
 import logging
 import os
+import time
+import uuid
 from asyncio import Condition, Task
 from threading import Lock
 from typing import (
     Any,
     AsyncIterator,
     Awaitable,
     Callable,
@@ -30,62 +32,66 @@
 # noinspection PyPackageRequirements
 import grpc
 from pymitter import EventEmitter
 
 from .aggregator import AverageAggregator, EntryAggregator, PriorityAggregator, SumAggregator
 from .comparator import Comparator
 from .event import MapLifecycleEvent, MapListener, SessionLifecycleEvent
+from .extractor import ValueExtractor
 from .filter import Filter
 from .messages_pb2 import PageRequest  # type: ignore
 from .processor import EntryProcessor
 from .serialization import Serializer, SerializerRegistry
 from .services_pb2_grpc import NamedCacheServiceStub
 from .util import RequestFactory
 
+E = TypeVar("E")
 K = TypeVar("K")
 V = TypeVar("V")
 R = TypeVar("R")
 T = TypeVar("T")
 
 COH_LOG = logging.getLogger("coherence")
 
 
 @no_type_check
 def _pre_call_cache(func):
     def inner(self, *args, **kwargs):
         if not self.active:
-            raise Exception("Cache [] has been " + "released" if self.released else "destroyed")
+            raise RuntimeError("Cache [] has been " + "released" if self.released else "destroyed")
 
         return func(self, *args, **kwargs)
 
     async def inner_async(self, *args, **kwargs):
         if not self.active:
-            raise Exception("Cache [{}] has been {}.".format(self.name, "released" if self.released else "destroyed"))
+            raise RuntimeError(
+                "Cache [{}] has been {}.".format(self.name, "released" if self.released else "destroyed")
+            )
 
         # noinspection PyProtectedMember
-        await self._session._wait_for_active()
+        await self._session._wait_for_ready()
 
         return await func(self, *args, **kwargs)
 
     if asyncio.iscoroutinefunction(func):
         return inner_async
     return inner
 
 
 @no_type_check
 def _pre_call_session(func):
     def inner(self, *args, **kwargs):
         if self._closed:
-            raise Exception("Session has been closed.")
+            raise RuntimeError("Session has been closed.")
 
         return func(self, *args, **kwargs)
 
     async def inner_async(self, *args, **kwargs):
         if self._closed:
-            raise Exception("Session has been closed.")
+            raise RuntimeError("Session has been closed.")
 
         return await func(self, *args, **kwargs)
 
     if asyncio.iscoroutinefunction(func):
         return inner_async
     return inner
 
@@ -448,14 +454,42 @@
         :param comparator: the Comparator object which imposes an ordering on entries in the resulting set; or `None`
          if the entries' values natural ordering should be used
         :param by_page: returns the keys in pages (transparently to the caller).  This option is only valid
          if no filter or comparator is provided.
         :return: an AsyncIterator of MapEntry instances that satisfy the specified criteria
         """
 
+    @abc.abstractmethod
+    def add_index(
+        self, extractor: ValueExtractor[T, E], ordered: bool = False, comparator: Optional[Comparator] = None
+    ) -> None:
+        """
+        Add an index to this map.
+
+        :param extractor: The :class:`coherence.extractor.ValueExtractor` object that is used to extract
+                   an indexable Object from a value stored in the
+                   indexed Map. Must not be 'None'.
+        :param ordered: true if the contents of the indexed information
+                   should be ordered false otherwise.
+        :param comparator: The :class:`coherence.comparator.Comparator` object which imposes an ordering
+                   on entries in the indexed map or None if the
+                   entries' values natural ordering should be used.
+        """
+
+    @abc.abstractmethod
+    def remove_index(self, extractor: ValueExtractor[T, E]) -> None:
+        """
+        Removes an index on this `NamedMap`.
+
+        :param extractor: The :class:`coherence.extractor.ValueExtractor` object that is used to extract
+                  an indexable Object from a value stored in the
+                  indexed Map. Must not be 'None'.
+
+        """
+
 
 class NamedCache(NamedMap[K, V]):
     """
     A Map-based data-structure that manages entries across one or more processes. Entries are typically managed in
     memory, and are often comprised of data that is also stored in an external system, for example, a database,
     or data that has been assembled or calculated at some significant cost.  Such entries are referred to as being
     `cached`.
@@ -573,14 +607,15 @@
 
     @_pre_call_cache
     async def clear(self) -> None:
         r = self._request_factory.clear_request()
         await self._client_stub.clear(r)
 
     async def destroy(self) -> None:
+        self.release()
         self._internal_emitter.once(MapLifecycleEvent.DESTROYED.value)
         self._internal_emitter.emit(MapLifecycleEvent.DESTROYED.value, self.name)
         r = self._request_factory.destroy_request()
         await self._client_stub.destroy(r)
 
     @_pre_call_cache
     def release(self) -> None:
@@ -666,17 +701,17 @@
         # for compatibility with 22.06
         if isinstance(aggregator, SumAggregator) and isinstance(value, str):
             return cast(R, float(value))
         elif isinstance(aggregator, AverageAggregator) and isinstance(value, str):
             return cast(R, float(value))
         elif isinstance(aggregator, PriorityAggregator):
             pri_agg: PriorityAggregator[R] = aggregator
-            if isinstance(pri_agg.aggregator, SumAggregator) and isinstance(value, str):
-                return cast(R, float(value))
-            elif isinstance(pri_agg.aggregator, AverageAggregator) and isinstance(value, str):
+            if (
+                isinstance(pri_agg.aggregator, AverageAggregator) or isinstance(pri_agg.aggregator, SumAggregator)
+            ) and isinstance(value, str):
                 return cast(R, float(value))
         # end compatibility with 22.06
 
         return cast(R, value)
 
     @_pre_call_cache
     def values(
@@ -734,47 +769,67 @@
             raise ValueError("A MapListener must be specified")
 
         if listener_for is None or isinstance(listener_for, Filter):
             await self._events_manager._remove_filter_listener(listener, listener_for)
         else:
             await self._events_manager._remove_key_listener(listener, listener_for)
 
+    @_pre_call_cache
+    async def add_index(
+        self, extractor: ValueExtractor[T, E], ordered: bool = False, comparator: Optional[Comparator] = None
+    ) -> None:
+        if extractor is None:
+            raise ValueError("A ValueExtractor must be specified")
+        r = self._request_factory.add_index_request(extractor, ordered, comparator)
+        await self._client_stub.addIndex(r)
+
+    @_pre_call_cache
+    async def remove_index(self, extractor: ValueExtractor[T, E]) -> None:
+        if extractor is None:
+            raise ValueError("A ValueExtractor must be specified")
+        r = self._request_factory.remove_index_request(extractor)
+        await self._client_stub.removeIndex(r)
+
     def _setup_event_handlers(self) -> None:
         """
         Setup handlers to notify cache-level handlers of events.
         """
         emitter: EventEmitter = self._emitter
         internal_emitter: EventEmitter = self._internal_emitter
         this: NamedCacheClient[K, V] = self
         cache_name = self._cache_name
 
         # noinspection PyProtectedMember
         def on_destroyed(name: str) -> None:
-            if name == cache_name:
-                if not this.destroyed:
-                    this._events_manager._close()
-                    this._destroyed = True
-                    emitter.emit(MapLifecycleEvent.DESTROYED.value, name)
+            if name == cache_name and not this.destroyed:
+                this._events_manager._close()
+                this._destroyed = True
+                emitter.emit(MapLifecycleEvent.DESTROYED.value, name)
 
         # noinspection PyProtectedMember
         def on_released(name: str) -> None:
-            if name == cache_name:
-                if not this.released:
-                    this._events_manager._close()
-                    this._released = True
-                    emitter.emit(MapLifecycleEvent.RELEASED.value, name)
+            if name == cache_name and not this.released:
+                this._events_manager._close()
+                this._released = True
+                emitter.emit(MapLifecycleEvent.RELEASED.value, name)
 
         def on_truncated(name: str) -> None:
             if name == cache_name:
                 emitter.emit(MapLifecycleEvent.TRUNCATED.value, name)
 
         internal_emitter.on(MapLifecycleEvent.DESTROYED.value, on_destroyed)
         internal_emitter.on(MapLifecycleEvent.RELEASED.value, on_released)
         internal_emitter.on(MapLifecycleEvent.TRUNCATED.value, on_truncated)
 
+    def __str__(self) -> str:
+        return (
+            f"NamedCache(name={self.name}, session={self._session.session_id}, serializer={self._serializer},"
+            f" released={self.released}, destroyed={self.destroyed})"
+        )
+
 
 class TlsOptions:
     """
     Options specific to the configuration of TLS.
     """
 
     ENV_CA_CERT = "COHERENCE_TLS_CERTS_PATH"
@@ -880,14 +935,20 @@
         Once called, no further mutations can be made.
         """
         self._locked = True
 
     def is_locked(self) -> bool:
         return self._locked
 
+    def __str__(self) -> str:
+        return (
+            f"TlsOptions(enabled={self.enabled}, ca-cert-path={self.ca_cert_path}, "
+            f"client-cert-path={self.client_cert_path}, client-key-path={self.client_key_path})"
+        )
+
 
 class Options:
     """
     Supported :func:`coherence.client.Session` options.
     """
 
     ENV_SERVER_ADDRESS = "COHERENCE_SERVER_ADDRESS"
@@ -898,29 +959,52 @@
     """
     ENV_REQUEST_TIMEOUT = "COHERENCE_CLIENT_REQUEST_TIMEOUT"
     """
     Environment variable to specify the request timeout for each remote call. The environment variable is used if
     request timeout is not passed as an argument in the constructor. If the environment variable is not set and
     request timeout is not passed as an argument then `DEFAULT_REQUEST_TIMEOUT` of 30 seconds is used
     """
+    ENV_READY_TIMEOUT = "COHERENCE_READY_TIMEOUT"
+    """
+    Environment variable to specify the maximum amount of time an NamedMap or NamedCache operations may wait for the
+    underlying gRPC channel to be ready.  This is independent of the request timeout which sets a deadline on how
+    long the call may take after being dispatched.
+    """
+    ENV_SESSION_DISCONNECT_TIMEOUT = "COHERENCE_SESSION_DISCONNECT_TIMEOUT"
+    """
+    Environment variable to specify the maximum amount of time, in seconds, a Session may remain in a disconnected
+    state without successfully reconnecting.
+    """
 
     DEFAULT_ADDRESS: Final[str] = "localhost:1408"
     """The default target address to connect to Coherence gRPC server."""
     DEFAULT_SCOPE: Final[str] = ""
     """The default scope."""
     DEFAULT_REQUEST_TIMEOUT: Final[float] = 30.0
     """The default request timeout."""
+    DEFAULT_READY_TIMEOUT: Final[float] = 0
+    """
+    The default ready timeout is 0 which disables the feature by default.  Explicitly configure the ready timeout
+    session option or use the environment variable to specify a positive value indicating how many seconds an RPC will
+    wait for the underlying channel to be ready before failing.
+    """
+    DEFAULT_SESSION_DISCONNECT_TIMEOUT: Final[float] = 30.0
+    """
+    The default maximum time a session may be in a disconnected state without having successfully reconnected.
+    """
     DEFAULT_FORMAT: Final[str] = "json"
     """The default serialization format"""
 
     def __init__(
         self,
         address: str = DEFAULT_ADDRESS,
         scope: str = DEFAULT_SCOPE,
         request_timeout_seconds: float = DEFAULT_REQUEST_TIMEOUT,
+        ready_timeout_seconds: float = DEFAULT_READY_TIMEOUT,
+        session_disconnect_seconds: float = DEFAULT_SESSION_DISCONNECT_TIMEOUT,
         ser_format: str = DEFAULT_FORMAT,
         channel_options: Optional[Sequence[Tuple[str, Any]]] = None,
         tls_options: Optional[TlsOptions] = None,
     ) -> None:
         """
         Construct a new :func:`coherence.client.Options`
 
@@ -928,37 +1012,40 @@
           to :func:`coherence.client.Options.DEFAULT_ADDRESS`. See
           also :func:`coherence.client.Options.ENV_SERVER_ADDRESS`
         :param scope: scope name used to link this :func:`coherence.client.Options` to the
           corresponding `ConfigurableCacheFactory` on the server.
         :param request_timeout_seconds: Defines the request timeout, in `seconds`, that will be applied to each
           remote call. If not explicitly set, this defaults to :func:`coherence.client.Options.DEFAULT_REQUEST_TIMEOUT`.
           See also :func:`coherence.client.Options.ENV_REQUEST_TIMEOUT`
+        :param ready_timeout_seconds: Defines the ready timeout, in `seconds`.  If this is a positive
+          float value, remote calls will not fail immediately if no connection is available.  If this is a value of zero
+          or less, then remote calls will fail-fast.  If not explicitly configured, the default of 0 is assumed.
+
+          See also :class:`coherence.client.Options.ENV_READY_TIMEOUT`
+        :param session_disconnect_seconds: Defines the maximum time, in `seconds`, that a session may remain in
+          a disconnected state without successfully reconnecting.
         :param ser_format: The serialization format.  Currently, this is always `json`
         :param channel_options: The `gRPC` `ChannelOptions`. See
             https://grpc.github.io/grpc/python/glossary.html#term-channel_arguments and
             https://github.com/grpc/grpc/blob/master/include/grpc/impl/grpc_types.h
         :param tls_options: Optional TLS configuration.
         """
         addr = os.getenv(Options.ENV_SERVER_ADDRESS)
         if addr is not None:
             self._address = addr
         else:
             self._address = address
 
-        timeout = os.getenv(Options.ENV_REQUEST_TIMEOUT)
-        if timeout is not None:
-            time_out: float
-            try:
-                time_out = float(timeout)
-            except ValueError:
-                COH_LOG.warning("The timeout value of [%s] cannot be converted to a float", Options.ENV_REQUEST_TIMEOUT)
-
-            self._request_timeout_seconds = time_out
-        else:
-            self._request_timeout_seconds = request_timeout_seconds
+        self._request_timeout_seconds = Options._get_float_from_env(
+            Options.ENV_REQUEST_TIMEOUT, request_timeout_seconds
+        )
+        self._ready_timeout_seconds = Options._get_float_from_env(Options.ENV_READY_TIMEOUT, ready_timeout_seconds)
+        self._session_disconnect_timeout_seconds = Options._get_float_from_env(
+            Options.ENV_READY_TIMEOUT, session_disconnect_seconds
+        )
 
         self._scope = scope
         self._ser_format = ser_format
 
         if channel_options is not None:
             self._channel_options = channel_options
 
@@ -1019,14 +1106,32 @@
         Returns the request timeout in `seconds`
 
         :return: the request timeout in `seconds`
         """
         return self._request_timeout_seconds
 
     @property
+    def ready_timeout_seconds(self) -> float:
+        """
+        Returns the ready timeout in `seconds`.
+
+        :return: the ready timeout in `seconds`
+        """
+        return self._ready_timeout_seconds
+
+    @property
+    def session_disconnect_timeout_seconds(self) -> float:
+        """
+        Returns the ready timeout in `seconds`.
+
+        :return: the ready timeout in `seconds`
+        """
+        return self._session_disconnect_timeout_seconds
+
+    @property
     def channel_options(self) -> Optional[Sequence[Tuple[str, Any]]]:
         """
         Return the `gRPC` `ChannelOptions`.
 
         :return: the `gRPC` `ChannelOptions`.
         """
         return getattr(self, "_channel_options", None)
@@ -1036,14 +1141,51 @@
         """
         Set the `gRPC` `ChannelOptions`.
 
         :param channel_options: the `gRPC` `ChannelOptions`.
         """
         self._channel_options = channel_options
 
+    @staticmethod
+    def _get_float_from_env(variable_name: str, default_value: float) -> float:
+        """
+        Return a float value parsed from the provided environment variable name.
+
+        :param variable_name: the environment variable name
+        :param default_value: the value to use if the environment variable is not set
+
+        :return: the float value from the environment or the default if the value can't be parsed
+          or the environment variable is not set
+        """
+        timeout = os.getenv(variable_name)
+        if timeout is not None:
+            time_out: float = default_value
+            try:
+                time_out = float(timeout)
+            except ValueError:
+                COH_LOG.warning(
+                    "The timeout value of [%s] specified by environment variable [%s] cannot be converted to a float",
+                    timeout,
+                    variable_name,
+                )
+
+            return time_out
+        else:
+            return default_value
+
+    def __str__(self) -> str:
+        return (
+            f"Options(address={self.address}, scope={self.scope}, format={self.format},"
+            f" request-timeout-seconds={self.request_timeout_seconds}, "
+            f"ready-timeout-seconds={self.ready_timeout_seconds}, "
+            f"session-disconnect-timeout-seconds={self.session_disconnect_timeout_seconds}, "
+            f"tls-options={self.tls_options}, "
+            f"channel-options={self.channel_options})"
+        )
+
 
 def _get_channel_creds(tls_options: TlsOptions) -> grpc.ChannelCredentials:
     client_cert: bytes | None = None
     client_key: bytes | None = None
     ca_cert: bytes | None = None
 
     if tls_options.client_cert_path is not None:
@@ -1086,63 +1228,74 @@
     def __init__(self, session_options: Optional[Options] = None):
         """
         Construct a new `Session` based on the provided :func:`coherence.client.Options`
 
         :param session_options: the provided :func:`coherence.client.Options`
         """
         self._closed: bool = False
-        self._active = False
-        self._active_condition: Condition = Condition()
+        self._session_id: str = str(uuid.uuid4())
+        self._ready = False
+        self._ready_condition: Condition = Condition()
         self._caches: dict[str, NamedCache[Any, Any]] = dict()
         self._lock: Lock = Lock()
         if session_options is not None:
             self._session_options = session_options
         else:
             self._session_options = Options()
 
+        self._ready_timeout_seconds: float = self._session_options.ready_timeout_seconds
+        self._ready_enabled: bool = self._ready_timeout_seconds > 0
+
+        interceptors = [
+            _InterceptorUnaryUnary(self),
+            _InterceptorUnaryStream(self),
+            _InterceptorStreamUnary(self),
+        ]
+
+        # only add the StreamStream interceptor if ready support is enabled as
+        # when added in the non-ready case, the call will not fail-fast
+        if self._ready_enabled:
+            interceptors.append(_InterceptorStreamStream(self))
+
         self._tasks: Set[Task[None]] = set()
 
+        options: Sequence[tuple[str, Any]] = [
+            ("grpc.min_reconnect_backoff_ms", 1100),
+            ("grpc.max_reconnect_backoff_ms", 3000),
+            ("grpc.lb_policy_name", "round_robin"),
+        ]
+
         if self._session_options.tls_options is None:
             self._channel: grpc.aio.Channel = grpc.aio.insecure_channel(
                 self._session_options.address,
-                options=None
-                if self._session_options.channel_options is None
-                else self._session_options.channel_options,
-                interceptors=[
-                    _InterceptorUnaryUnary(self),
-                    _InterceptorUnaryStream(self),
-                    _InterceptorStreamUnary(self),
-                    _InterceptorStreamStream(self),
-                ],
+                options=(
+                    options if self._session_options.channel_options is None else self._session_options.channel_options
+                ),
+                interceptors=interceptors,
             )
         else:
             creds: grpc.ChannelCredentials = _get_channel_creds(self._session_options.tls_options)
             self._channel = grpc.aio.secure_channel(
                 self._session_options.address,
                 creds,
-                options=None
-                if self._session_options.channel_options is None
-                else self._session_options.channel_options,
-                interceptors=[
-                    _InterceptorUnaryUnary(self),
-                    _InterceptorUnaryStream(self),
-                    _InterceptorStreamUnary(self),
-                    _InterceptorStreamStream(self),
-                ],
+                options=(
+                    options if self._session_options.channel_options is None else self._session_options.channel_options
+                ),
+                interceptors=interceptors,
             )
 
         watch_task: Task[None] = asyncio.create_task(watch_channel_state(self))
         self._tasks.add(watch_task)
         self._emitter: EventEmitter = EventEmitter()
         self._channel.get_state(True)  # trigger connect
 
     @staticmethod
     async def create(session_options: Optional[Options] = None) -> Session:
         session: Session = Session(session_options)
-        await session._set_active(False)
+        await session._set_ready(False)
         return session
 
     # noinspection PyTypeHints
     @_pre_call_session
     def on(
         self,
         event: Literal[MapLifecycleEvent.DESTROYED] | Literal[MapLifecycleEvent.RELEASED] | SessionLifecycleEvent,
@@ -1201,20 +1354,35 @@
         :return: the :func:`coherence.client.Options` (read-only) used to configure this session.
         """
         return self._session_options
 
     @property
     def closed(self) -> bool:
         """
-        Returns `True` if Session is closed else `False`
+        Returns `True` if Session is closed else `False`.
 
         :return: `True` if Session is closed else `False`
         """
         return self._closed
 
+    @property
+    def session_id(self) -> str:
+        """
+        Returns this Session's ID.
+
+        :return: this Session's ID
+        """
+        return self._session_id
+
+    def __str__(self) -> str:
+        return (
+            f"Session(id={self.session_id}, closed={self.closed}, state={self._channel.get_state(False)},"
+            f" caches/maps={len(self._caches)}, options={self.options})"
+        )
+
     # noinspection PyProtectedMember
     @_pre_call_session
     async def get_cache(self, name: str, ser_format: str = DEFAULT_FORMAT) -> "NamedCache[K, V]":
         """
         Returns a :func:`coherence.client.NamedCache` for the specified cache name.
 
         :param name: the cache name
@@ -1251,37 +1419,45 @@
                 c = NamedCacheClient(name, self, serializer)
                 # initialize the event stream now to ensure lifecycle listeners will work as expected
                 await c._events_manager._ensure_stream()
                 self._setup_event_handlers(c)
                 self._caches.update({name: c})
             return c
 
-    def is_active(self) -> bool:
+    def is_ready(self) -> bool:
         """
         Returns
         :return:
         """
-        return self._active
+        if self._closed:
+            return False
+
+        return True if not self._ready_enabled else self._ready
 
-    async def _set_active(self, active: bool) -> None:
-        self._active = active
-        if self._active:
-            if not self._active_condition.locked():
-                await self._active_condition.acquire()
-            self._active_condition.notify_all()
-            self._active_condition.release()
+    async def _set_ready(self, ready: bool) -> None:
+        self._ready = ready
+        if self._ready:
+            if not self._ready_condition.locked():
+                await self._ready_condition.acquire()
+            self._ready_condition.notify_all()
+            self._ready_condition.release()
         else:
-            await self._active_condition.acquire()
+            await self._ready_condition.acquire()
 
-    async def _wait_for_active(self) -> None:
-        if not self.is_active():
-            timeout: float = self._session_options.request_timeout_seconds
-            COH_LOG.debug("Waiting for session to become active; timeout=[%s seconds]", timeout)
-            async with asyncio.timeout(timeout):
-                await self._active_condition.wait()
+    async def _wait_for_ready(self) -> None:
+        if self._ready_enabled and not self.is_ready():
+            timeout: float = self._ready_timeout_seconds
+            COH_LOG.debug(f"Waiting for session {self.session_id} to become active; timeout=[{timeout} seconds]")
+            try:
+                await asyncio.wait_for(self._ready_condition.wait(), timeout)
+            except TimeoutError:
+                s = "Deadline [{0} seconds] exceeded " "waiting for session {1} to become active".format(
+                    str(timeout), self.session_id
+                )
+                raise TimeoutError(s)
 
     # noinspection PyUnresolvedReferences
     async def close(self) -> None:
         """
         Close the `Session`
         """
         if not self._closed:
@@ -1294,14 +1470,15 @@
             caches_copy: dict[str, NamedCache[Any, Any]] = self._caches.copy()
             for cache in caches_copy.values():
                 cache.release()
 
             self._caches.clear()
 
             await self._channel.close()  # TODO: consider grace period?
+            self._channel = None
 
     def _setup_event_handlers(self, client: NamedCacheClient[K, V]) -> None:
         this: Session = self
 
         def on_destroyed(name: str) -> None:
             if name in this._caches:
                 del this._caches[name]
@@ -1336,15 +1513,15 @@
         :return:                     the result of the call
         """
         new_details = grpc.aio.ClientCallDetails(
             client_call_details.method,
             self._session.options.request_timeout_seconds,
             client_call_details.metadata,
             client_call_details.credentials,
-            True,
+            True if self._session._ready_enabled else None,
         )
         return await continuation(new_details, request)
 
 
 class _InterceptorUnaryUnary(_BaseInterceptor, grpc.aio.UnaryUnaryClientInterceptor):
     """Interceptor for Unary/Unary calls."""
 
@@ -1387,45 +1564,80 @@
 
 
 # noinspection PyProtectedMember
 async def watch_channel_state(session: Session) -> None:
     emitter: EventEmitter = session._emitter
     channel: grpc.aio.Channel = session.channel
     first_connect: bool = True
+    connected: bool = False
     last_state: grpc.ChannelConnectivity = grpc.ChannelConnectivity.IDLE
+    disconnect_time: float = 0
+
+    def current_milli_time() -> float:
+        return round(time.time() * 1000)
 
     try:
         while True:
-            state: grpc.ChannelConnectivity = channel.get_state(False)
-            COH_LOG.debug("New Channel State: transitioning from [%s] to [%s]", last_state, state)
-            match state:
-                case grpc.ChannelConnectivity.SHUTDOWN:
-                    COH_LOG.info("Session to [%s] terminated", session.options.address)
-                    await session._set_active(False)
-                case grpc.ChannelConnectivity.READY:
-                    if not first_connect and not session.is_active():
-                        COH_LOG.info("Session re-established to [%s]", session.options.address)
-
-                        await emitter.emit_async(SessionLifecycleEvent.RECONNECTED.value)
-                        await session._set_active(True)
-                    elif first_connect and not session.is_active():
-                        COH_LOG.info("Session established to [%s]", session.options.address)
-
-                        first_connect = False
-                        await emitter.emit_async(SessionLifecycleEvent.CONNECTED.value)
-                        await session._set_active(True)
-                case _:
-                    if session.is_active():
-                        COH_LOG.warning("Session to [%s] disconnected; will attempt reconnect", session.options.address)
-
-                        await emitter.emit_async(SessionLifecycleEvent.DISCONNECTED.value)
-                        await session._set_active(False)
-
-            COH_LOG.debug("Waiting for state change from [%s]", state)
-            await channel.wait_for_state_change(channel.get_state(True))
+            state: grpc.ChannelConnectivity = channel.get_state(True)
+            if COH_LOG.isEnabledFor(logging.DEBUG):
+                COH_LOG.debug(f"New Channel State: transitioning from [{last_state}] to [{state}].")
+            if state == grpc.ChannelConnectivity.SHUTDOWN:
+                COH_LOG.info(f"Session [{session.session_id}] terminated.")
+                await session._set_ready(False)
+                await session.close()
+                return
+            elif state == grpc.ChannelConnectivity.READY:
+                if not first_connect and not connected:
+                    connected = True
+                    disconnect_time = 0
+                    COH_LOG.info(f"Session [{session.session_id} re-connected to [{session.options.address}].")
+                    await emitter.emit_async(SessionLifecycleEvent.RECONNECTED.value)
+                    await session._set_ready(True)
+                elif first_connect and not connected:
+                    connected = True
+                    COH_LOG.info(f"Session [{session.session_id}] connected to [{session.options.address}].")
+
+                    first_connect = False
+                    await emitter.emit_async(SessionLifecycleEvent.CONNECTED.value)
+                    await session._set_ready(True)
+            else:
+                if connected:
+                    connected = False
+                    disconnect_time = -1
+                    COH_LOG.warning(
+                        f"Session [{session.session_id}] disconnected from [{session.options.address}];"
+                        f" will attempt reconnect."
+                    )
+
+                    await emitter.emit_async(SessionLifecycleEvent.DISCONNECTED.value)
+                    await session._set_ready(False)
+
+                if disconnect_time != 0:
+                    if disconnect_time == -1:
+                        disconnect_time = current_milli_time()
+                    else:
+                        waited: float = current_milli_time() - disconnect_time
+                        timeout = session.options.session_disconnect_timeout_seconds
+                        if COH_LOG.isEnabledFor(logging.DEBUG):
+                            COH_LOG.debug(
+                                f"Waited [{waited / 1000} seconds] for session [{session.session_id}] to reconnect."
+                                f" [~{(round(timeout - (waited / 1000)))} seconds] remaining to reconnect."
+                            )
+                        if waited >= timeout:
+                            COH_LOG.error(
+                                f"session [{session.session_id}] unable to reconnect within [{timeout} seconds."
+                                f"  Closing session."
+                            )
+                            await session.close()
+                            return
+
+            state = channel.get_state(True)
+            if COH_LOG.isEnabledFor(logging.DEBUG):
+                COH_LOG.debug(f"Waiting for state change from [{state}]")
+            await channel.wait_for_state_change(state)
     except asyncio.CancelledError:
         return
 
 
 class _Stream(abc.ABC, AsyncIterator[T]):
     """
     A simple AsyncIterator that wraps a Callable that produces iteration
@@ -1505,15 +1717,14 @@
 
             async for item in self._stream:
                 if self._new_page:  # a new page has been loaded; the cookie will be the first result
                     self._new_page = False
                     self._cookie = item.value if self._keys else item.cookie
                     if self._cookie == b"":
                         self._exhausted = True  # processing the last page
-                    continue
                 else:
                     return self._result_handler(self._serializer, item)
 
             self._stream = None
             if self._exhausted:
                 raise StopAsyncIteration
```

### Comparing `coherence_client-1.0rc2/src/coherence/comparator.py` & `coherence_client-1.1.0/src/coherence/comparator.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,46 @@
-# Copyright (c) 2022, 2023, Oracle and/or its affiliates.
+# Copyright (c) 2022, 2024, Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at
 # https://oss.oracle.com/licenses/upl.
 
 from __future__ import annotations
 
 from abc import ABC
 from typing import Any
 
 from .extractor import UniversalExtractor
 from .serialization import proxy
 
 
 class Comparator(ABC):
+    """Comparator is used to control the ordering for collections of objects"""
+
     def __init__(self) -> None:
         super().__init__()
 
 
 @proxy("comparator.SafeComparator")
 class SafeComparator(Comparator):
+    """None-safe delegating comparator. None values are evaluated as "less then" any non None value."""
+
     def __init__(self, property_name: str) -> None:
         super().__init__()
         self.comparator = ExtractorComparator(property_name)
 
 
 @proxy("comparator.InverseComparator")
 class InverseComparator(Comparator):
+    """Comparator that reverses the result of another comparator."""
+
     def __init__(self, property_name: str) -> None:
         super().__init__()
         self.comparator = ExtractorComparator(property_name)
 
 
 @proxy("comparator.ExtractorComparator")
 class ExtractorComparator(Comparator):
+    """Comparator implementation that uses specified :class:`coherence.extractor.ValueExtractor` to
+    extract value(s) to be used for comparison."""
+
     def __init__(self, property_name: str) -> None:
         super().__init__()
         self.extractor = UniversalExtractor[Any](property_name)
```

### Comparing `coherence_client-1.0rc2/src/coherence/event.py` & `coherence_client-1.1.0/src/coherence/event.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022, 2023 Oracle and/or its affiliates.
+# Copyright (c) 2022, 2024, Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at
 # https://oss.oracle.com/licenses/upl.
 
 from __future__ import annotations
 
 import asyncio
 from abc import ABCMeta, abstractmethod
@@ -126,23 +126,22 @@
 
     @property
     def description(self) -> str:
         """
         Returns the event's description.
         :return: the event's description
         """
-        match self.type:
-            case MapEventType.ENTRY_INSERTED:
-                return "insert"
-            case MapEventType.ENTRY_UPDATED:
-                return "update"
-            case MapEventType.ENTRY_DELETED:
-                return "delete"
-            case _:
-                return "unknown"
+        if self.type == MapEventType.ENTRY_INSERTED:
+            return "insert"
+        elif self.type == MapEventType.ENTRY_UPDATED:
+            return "update"
+        elif self.type == MapEventType.ENTRY_DELETED:
+            return "delete"
+        else:
+            return "unknown"
 
     @property
     def type(self) -> MapEventType:
         """
         The MapEventType.  This may be one of:
         * MapEventType.ENTRY_INSERTED
         * MapEventType.ENTRY_UPDATED
@@ -202,23 +201,22 @@
             + str(self.new)
             + "}"
         )
 
     @staticmethod
     def _from_event_id(_id: int) -> MapEventType:
         """Return the MapEventType based on the on-wire value for the event."""
-        match _id:
-            case 1:
-                return MapEventType.ENTRY_INSERTED
-            case 2:
-                return MapEventType.ENTRY_UPDATED
-            case 3:
-                return MapEventType.ENTRY_DELETED
-            case _:
-                raise Exception("Unhandled MapEventType [" + str(_id) + "]")
+        if _id == 1:
+            return MapEventType.ENTRY_INSERTED
+        elif _id == 2:
+            return MapEventType.ENTRY_UPDATED
+        elif _id == 3:
+            return MapEventType.ENTRY_DELETED
+        else:
+            raise RuntimeError("Unhandled MapEventType [" + str(_id) + "]")
 
 
 MapListenerCallback = Callable[[MapEvent[K, V]], None]
 """A type alias for MapEventListener callback functions."""
 
 
 class MapListener(Generic[K, V]):
@@ -226,15 +224,14 @@
 
     _emitter: EventEmitter
     """The internal emitter used to emit events."""
 
     def __init__(self) -> None:
         """Constructs a new MapListener."""
         self._emitter = EventEmitter()
-        pass
 
     def _on(self, event: MapEventType, callback: MapListenerCallback[K, V]) -> MapListener[K, V]:
         """
         Define a callback for the specified event type.
 
         :param event:     the event type of interest
         :param callback:  the callback that will be invoked when the specified event has occurred
@@ -447,52 +444,50 @@
     @staticmethod
     def _get_emitter_label(event: MapEvent[K, V]) -> str:
         """
         The string label required by the internal event emitter.
         :param event:  the MapEvent whose label will be generated
         :return: the emitter-friendly event label
         """
-        match event.type:
-            case MapEventType.ENTRY_DELETED:
-                return MapEventType.ENTRY_DELETED.value
-            case MapEventType.ENTRY_INSERTED:
-                return MapEventType.ENTRY_INSERTED.value
-            case MapEventType.ENTRY_UPDATED:
-                return MapEventType.ENTRY_UPDATED.value
-            case _:
-                raise AssertionError(f"Unknown EventType [{event}]")
+        if event.type == MapEventType.ENTRY_DELETED:
+            return MapEventType.ENTRY_DELETED.value
+        elif event.type == MapEventType.ENTRY_INSERTED:
+            return MapEventType.ENTRY_INSERTED.value
+        elif event.type == MapEventType.ENTRY_UPDATED:
+            return MapEventType.ENTRY_UPDATED.value
+        else:
+            raise AssertionError(f"Unknown EventType [{event}]")
 
     @abstractmethod
     def _post_subscribe(self, request: MapListenerRequest) -> None:
         """
         Custom actions that implementations may need to make after a subscription has been completed.
         :param request:  the request that was used to subscribe
         """
-        return
+        pass
 
     @abstractmethod
     def _post_unsubscribe(self, request: MapListenerRequest) -> None:
         """
         Custom actions that implementations may need to make after an unsubscription has been completed.
         :param request:  the request that was used to unsubscribe
         """
-        return
+        pass
 
 
 class _KeyListenerGroup(_ListenerGroup[K, V]):
     """A ListenerGroup for key-based MapListeners"""
 
     def __init__(self, manager: _MapEventsManager[K, V], key: K) -> None:
         """
         Creates a new _KeyListenerGroup
         :param manager:  the _MapEventManager
         :param key:      the group key
         """
         super()._init_(manager, key)
-        pass
 
     # noinspection PyProtectedMember
     def _post_subscribe(self, request: MapListenerRequest) -> None:
         manager: _MapEventsManager[K, V] = self._manager
         key: K = manager._serializer.deserialize(request.key)
         self._manager._key_group_subscribed(key, self)
 
@@ -509,15 +504,14 @@
     def __init__(self, manager: _MapEventsManager[K, V], filter: Filter) -> None:
         """
         Creates a new _KeyListenerGroup
         :param manager:  the _MapEventManager
         :param filter:   the group Filter
         """
         super()._init_(manager, filter)
-        pass
 
     # noinspection PyProtectedMember
     def _post_subscribe(self, request: MapListenerRequest) -> None:
         self._manager._filter_group_subscribed(request.filterId, cast(Filter, self._key_or_filter), self)
 
     # noinspection PyProtectedMember
     def _post_unsubscribe(self, request: MapListenerRequest) -> None:
@@ -656,23 +650,26 @@
         """
         if self._event_stream is None:
             event_stream: grpc.aio.StreamStreamCall = self._client.events()
             await event_stream.write(self._request_factory.map_event_subscribe())
             self._event_stream = event_stream
             read_task: Task[None] = asyncio.create_task(self._handle_response())
             self._background_tasks.add(read_task)
+            # we use asyncio.timeout here instead of using the gRPC timeout
+            # as any deadline set on the stream will result in a loss of events
             try:
-                async with asyncio.timeout(self._session.options.request_timeout_seconds):
-                    await self._stream_waiter.wait()
+                await asyncio.wait_for(self._stream_waiter.wait(), self._session.options.request_timeout_seconds)
             except TimeoutError:
-                raise TimeoutError(
-                    "Unable to establish session with [{0}] within [{1}] seconds)".format(
-                        self._session.options.address, str(self._session.options.request_timeout_seconds)
+                s = (
+                    "Deadline [{0} seconds] exceeded waiting for event stream"
+                    " to become ready. Server address - {1})".format(
+                        str(self._session.options.request_timeout_seconds), self._session.options.address
                     )
                 )
+                raise TimeoutError(s)
 
         return self._event_stream
 
     async def _register_key_listener(self, listener: MapListener[K, V], key: K, lite: bool = False) -> None:
         """
         Registers the specified listener to listen for events matching the provided key.
         :param listener:  the MapListener to register
```

### Comparing `coherence_client-1.0rc2/src/coherence/filter.py` & `coherence_client-1.1.0/src/coherence/filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # https://oss.oracle.com/licenses/upl.
 
 from __future__ import annotations
 
 from abc import ABC
 from typing import Any, Generic, Set, TypeVar
 
-from .extractor import ExtractorExpression, ValueExtractor, extract
+from .extractor import ExtractorExpression, Extractors, ValueExtractor
 from .serialization import proxy
 
 E = TypeVar("E")
 K = TypeVar("K")
 R = TypeVar("R")
 T = TypeVar("T")
 V = TypeVar("V")
@@ -75,16 +75,16 @@
          method name to make a {@link UniversalExtractor} for; this parameter can also be a dot-delimited sequence of
          method names which would result in an ExtractorFilter based on the {@link ChainedExtractor} that is based on
          an array of corresponding ReflectionExtractor objects
         """
         super().__init__()
         if isinstance(extractor, ValueExtractor):
             self.extractor = extractor
-        elif type(extractor) == str:
-            self.extractor = extract(extractor)
+        elif isinstance(extractor, str):
+            self.extractor = Extractors.extract(extractor)
         else:
             raise ValueError("extractor cannot be any other type")
 
 
 @proxy("filter.ComparisonFilter")
 class ComparisonFilter(ExtractorFilter):
     def __init__(self, extractor: ExtractorExpression[T, E], value: V):
```

### Comparing `coherence_client-1.0rc2/src/coherence/messages_pb2.py` & `coherence_client-1.1.0/src/coherence/messages_pb2.py`

 * *Files identical despite different names*

### Comparing `coherence_client-1.0rc2/src/coherence/processor.py` & `coherence_client-1.1.0/src/coherence/processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,41 @@
-# Copyright (c) 2022, 2023, Oracle and/or its affiliates.
+# Copyright (c) 2022, 2024, Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at
 # https://oss.oracle.com/licenses/upl.
 
 from __future__ import annotations
 
 from abc import ABC
 from decimal import Decimal
-from typing import Any, Generic, List, Optional, TypeAlias, TypeVar, cast
+from typing import Any, Generic, List, Optional, TypeVar, Union, cast
+
+from typing_extensions import TypeAlias
 
 from .extractor import (
     CompositeUpdater,
     ExtractorExpression,
-    IdentityExtractor,
+    Extractors,
     ManipulatorExpression,
     UniversalExtractor,
     UniversalUpdater,
     UpdaterExpression,
     ValueExtractor,
     ValueManipulator,
     ValueUpdater,
-    extract,
 )
 from .filter import Filter
 from .serialization import mappings, proxy
 
 E = TypeVar("E")
 K = TypeVar("K")
 R = TypeVar("R")
 T = TypeVar("T")
 V = TypeVar("V")
 
-Numeric: TypeAlias = int | float | Decimal
+Numeric: TypeAlias = Union[int, float, Decimal]
 
 
 class EntryProcessor(ABC, Generic[R]):
     """
     An invocable agent that operates against the entries within a NamedMap
     """
 
@@ -87,20 +88,20 @@
 
         :param value_extractor: the :class:`coherence.extractor.ValueExtractor` or string expression
                                 to use by this filter or the name of the method to
                                 invoke via java reflection
         """
         super().__init__()
         if value_extractor is None:
-            self.extractor: ValueExtractor[V, R] = IdentityExtractor()
+            self.extractor: ValueExtractor[V, R] = Extractors.identity()
         else:
             if isinstance(value_extractor, ValueExtractor):
                 self.extractor = value_extractor
-            elif type(value_extractor) == str:
-                self.extractor = extract(value_extractor)
+            elif isinstance(value_extractor, str):
+                self.extractor = Extractors.extract(value_extractor)
             else:
                 raise ValueError("value_extractor cannot be any other type")
 
 
 @proxy("processor.CompositeProcessor")
 class CompositeProcessor(EntryProcessor[R]):
     """
@@ -167,27 +168,27 @@
 
 
 class PropertyProcessor(EntryProcessor[R]):
     """
     `PropertyProcessor` is a base class for EntryProcessor implementations that depend on a ValueManipulator.
     """
 
-    def __init__(self, manipulator: ManipulatorExpression, use_is: bool = False):
+    def __init__(self, manipulator: ManipulatorExpression[T, E], use_is: bool = False):
         """
         Construct a PropertyProcessor for the specified property name.
 
         This constructor assumes that the corresponding property getter will have a name of ("get" + sName) and the
         corresponding property setter's name will be ("set" + sName).
 
         :param manipulator: the manipulator or property name
         :param use_is: prefix with `is`
         """
         super().__init__()
         if type(manipulator) is str:
-            self.manipulator: ManipulatorExpression = PropertyManipulator(manipulator, use_is)
+            self.manipulator: ManipulatorExpression[T, E] = PropertyManipulator(manipulator, use_is)
         else:
             self.manipulator = manipulator
 
 
 @proxy("processor.PropertyManipulator")
 class PropertyManipulator(ValueManipulator[V, R]):
     """
@@ -206,39 +207,39 @@
         :param use_is: if true, the getter method will be prefixed with "is" rather than "get"
         """
         super().__init__()
         self.property_name = property_name
         self.useIsPrefix = use_is
 
     def get_extractor(self) -> ValueExtractor[V, R]:
-        raise Exception("Method not implemented")
+        raise NotImplementedError("Method not implemented")
 
     def get_updator(self) -> ValueUpdater[V, R]:
-        raise Exception("Method not implemented")
+        raise NotImplementedError("Method not implemented")
 
 
 @proxy("processor.NumberMultiplier")
 class NumberMultiplier(PropertyProcessor[Numeric]):
     """
     NumberMultiplier entry processor.
     """
 
     def __init__(
-        self, name_or_manipulator: ManipulatorExpression, multiplier: Numeric, post_multiplication: bool = False
+        self, name_or_manipulator: ManipulatorExpression[T, E], multiplier: Numeric, post_multiplication: bool = False
     ):
         """
         Construct an NumberMultiplier processor that will multiply a property value by a specified factor,
         returning either the old or the new value as specified.
 
         :param name_or_manipulator: the ValueManipulator or the property name
         :param multiplier: the Number representing the magnitude and sign of the multiplier
         :param post_multiplication: pass true to return the value as it was before it was multiplied, or pass false
          to return the value as it is after it is multiplied
         """
-        if type(name_or_manipulator) == str:
+        if isinstance(name_or_manipulator, str):
             manipulator: ValueManipulator[Any, Numeric] = self.create_custom_manipulator(name_or_manipulator)
             super().__init__(manipulator)
         else:
             super().__init__(name_or_manipulator)
         self.multiplier = multiplier
         self.postMultiplication = post_multiplication
 
@@ -253,25 +254,27 @@
 @proxy("processor.NumberIncrementor")
 class NumberIncrementor(PropertyProcessor[Numeric]):
     """
     The :class:`coherence.processor.NumberIncrementor` :class:`coherence.processor.EntryProcessor` is used to increment
     a property value of a numeric type.
     """
 
-    def __init__(self, name_or_manipulator: ManipulatorExpression, increment: Numeric, post_increment: bool = False):
+    def __init__(
+        self, name_or_manipulator: ManipulatorExpression[T, E], increment: Numeric, post_increment: bool = False
+    ):
         """
         Construct an :class:`coherence.processor.NumberIncrementor` processor that will increment a property
         value by a specified amount, returning either the old or the new value as specified.
 
         :param name_or_manipulator: the :class:`coherence.extractor.ValueManipulator` or string expression
         :param increment: the numeric value representing the magnitude and sign of the increment
         :param post_increment: pass `True` to return the value as it was before it was incremented, or pass `False`
          to return the value as it is after it is incremented
         """
-        if type(name_or_manipulator) == str:
+        if isinstance(name_or_manipulator, str):
             manipulator: ValueManipulator[Any, Numeric] = self.create_custom_manipulator(name_or_manipulator)
             super().__init__(manipulator)
         else:
             super().__init__(name_or_manipulator)
         self.increment = increment
         self.postInc = post_increment
 
@@ -474,15 +477,15 @@
         Construct an `UpdaterProcessor` based on the specified ValueUpdater.
 
         :param updater_or_property_name: a ValueUpdater object or the method name; passing null will simpy replace
          the entry's value with the specified one instead of updating it
         :param value: the value to update the target entry with
         """
         super().__init__()
-        if type(updater_or_property_name) == str:
+        if type(updater_or_property_name) == str:  # noqa: E721
             self.updater: ValueUpdater[V, bool]
             if updater_or_property_name.find(".") == -1:
                 self.updater = UniversalUpdater(updater_or_property_name)
             else:
                 self.updater = CompositeUpdater(updater_or_property_name)
         else:
             self.updater = cast(ValueUpdater[V, bool], updater_or_property_name)
@@ -611,20 +614,20 @@
         For clustered caches using the :class:`coherence.processor.ExtractorProcessor` could significantly reduce
         the amount of network traffic.
 
         :param extractor: the :class:`coherence.extractor.ValueExtractor` or string expression to use by this
                           processor or the name of the method to invoke via java reflection.  If `None`, an
                           :class:`coherence.extractor.IdentityExtractor` will be used.
         """
-        ext: ExtractorExpression[T, E] = extractor if extractor is not None else IdentityExtractor()
+        ext: ExtractorExpression[T, E] = extractor if extractor is not None else Extractors.identity()
         return ExtractorProcessor(ext)
 
     @staticmethod
     def increment(
-        name_or_manipulator: ManipulatorExpression, increment: Numeric, post_increment: bool = False
+        name_or_manipulator: ManipulatorExpression[T, E], increment: Numeric, post_increment: bool = False
     ) -> EntryProcessor[Numeric]:
         """
         Construct an :class:`coherence.processor.NumberIncrementor` processor that will increment a property
         value by a specified amount, returning either the old or the new value as specified.
 
         :param name_or_manipulator: the :class:`coherence.extractor.ValueManipulator` or string expression
         :param increment: the numeric value representing the magnitude and sign of the increment
@@ -658,15 +661,15 @@
         :return: a :class:`coherence.processor.MethodInvocationProcessor` that invokes the specified method on
                  a value of a cache entry and optionally updates the entry with a modified value
         """
         return MethodInvocationProcessor(method_name, True, args)
 
     @staticmethod
     def multiply(
-        name_or_manipulator: ManipulatorExpression, multiplier: Numeric, post_multiplication: bool = False
+        name_or_manipulator: ManipulatorExpression[T, E], multiplier: Numeric, post_multiplication: bool = False
     ) -> EntryProcessor[Numeric]:
         """
         Construct an NumberMultiplier processor that will multiply a property value by a specified factor,
         returning either the old or the new value as specified.
 
         :param name_or_manipulator: the ValueManipulator or the property name
         :param multiplier: the Number representing the magnitude and sign of the multiplier
```

### Comparing `coherence_client-1.0rc2/src/coherence/serialization.py` & `coherence_client-1.1.0/src/coherence/serialization.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,14 +8,27 @@
 from decimal import Decimal
 from typing import Any, Callable, Dict, Final, Optional, Type, TypeVar, cast
 
 import jsonpickle
 
 T = TypeVar("T", covariant=True)
 
+_BIG_DEC_ALIAS: Final[str] = "math.BigDec"
+_BIG_INT_ALIAS: Final[str] = "math.BigInt"
+
+_META_CLASS: Final[str] = "@class"
+_META_VERSION: Final[str] = "@version"
+_META_ENUM: Final[str] = "enum"
+
+_JSON_KEY = "key"
+_JSON_VALUE = "value"
+_JSON_ENTRIES = "entries"
+
+_JSON_PICKLE_OBJ = "py/object"
+
 MAGIC_BYTE: Final[bytes] = b"\x15"
 
 _type_to_alias: Final[Dict[Type[Any], str]] = dict()
 """A mapping of proxied Python types to their alias."""
 
 _alias_to_type: Final[Dict[str, Type[Any]]] = dict()
 """A mapping of aliases to their proxied Python type."""
@@ -32,20 +45,24 @@
     def serialize(self, obj: object) -> bytes:
         """documentation"""
 
     @abstractmethod
     def deserialize(self, value: bytes) -> T:  # type: ignore
         """documentation"""
 
+    @property
     def format(self) -> str:
         return self._ser_format
 
     def __init__(self, ser_format: str):
         self._ser_format = ser_format
 
+    def __str__(self) -> str:
+        return f"Serializer(format={self.format})"
+
 
 class JSONSerializer(Serializer):
     SER_FORMAT = "json"
 
     def __init__(self) -> None:
         super().__init__(JSONSerializer.SER_FORMAT)
         self._pickler = JavaProxyPickler()
@@ -53,15 +70,15 @@
 
     def serialize(self, obj: object) -> bytes:
         jsn: str = jsonpickle.encode(obj, context=self._pickler)
         b: bytes = MAGIC_BYTE + jsn.encode()
         return b
 
     def deserialize(self, value: bytes) -> T:  # type: ignore
-        if type(value) == bytes:
+        if isinstance(value, bytes):
             s = value.decode()
             if value.__len__() == 0:  # empty string
                 return cast(T, None)
             else:
                 if ord(s[0]) == ord(MAGIC_BYTE):
                     return jsonpickle.decode(s[1:], context=self._unpickler)
                 else:
@@ -87,28 +104,28 @@
 
     @staticmethod
     def serializer(ser_format: str) -> Serializer:
         s = SerializerRegistry.instance().serializers[ser_format]
         if s is not None:
             return s
         else:
-            raise Exception("No serializer registered for format: " + ser_format)
+            raise ValueError("No serializer registered for format: " + ser_format)
 
 
 class JavaProxyPickler(jsonpickle.Pickler):
     MAX_NUMERIC: Final[int] = (2**63) - 1
     MIN_NUMERIC: Final[int] = (-(2**63)) - 1
 
     def __init__(self) -> None:
         super().__init__(make_refs=False)
 
     def _flatten(self, obj: Any) -> dict[str, str] | None | dict[str, Any] | Decimal:
         if isinstance(obj, int):
             if obj > self.MAX_NUMERIC or obj < self.MIN_NUMERIC:
-                return {"@class": "math.BigInt", "value": str(obj)}
+                return {_META_CLASS: _BIG_INT_ALIAS, "value": str(obj)}
 
         if isinstance(obj, set):
             return super()._flatten(list(obj))
 
         return super()._flatten(obj)
 
     def _getstate(self, obj: Any, data: Any) -> Any:
@@ -120,21 +137,21 @@
         return data
 
     def _flatten_obj(self, obj: Any) -> dict[str, str | dict[str, list[dict[str, Any]]]] | None:
         result = super()._flatten_obj(obj)
         object_type = type(obj)
         alias: Optional[str] = _alias_for(object_type)
         if alias is not None:
-            marker = result.get("py/object", None)
+            marker = result.get(_JSON_PICKLE_OBJ, None)
             if marker is not None:
                 actual: dict[str, Any] = dict()
-                actual["@class"] = alias
+                actual[_META_CLASS] = alias
                 for key, value in result.items():
                     # ignore jsonpickle specific content as well as protected keys
-                    if key == "py/object" or str(key).startswith("_"):
+                    if key == _JSON_PICKLE_OBJ or str(key).startswith("_"):
                         continue
 
                     # store the original key/value pair as logic below may change them
                     key_ = key
                     value_ = value
 
                     # check for any attributes that need a different key name when serialized to JSON
@@ -143,21 +160,21 @@
                         mapping = mappings_.get(key, None)
                         if mapping is not None:
                             key_ = mapping
 
                     # if the value being serialized is a dict, serialize it as a list of key/value pairs
                     if (
                         isinstance(value_, dict)
-                        and "@class" not in value_
-                        and "@version" not in value_
-                        and "enum" not in value_
+                        and _META_CLASS not in value_
+                        and _META_VERSION not in value_
+                        and _META_ENUM not in value_
                     ):
                         entries = list()
                         for key_inner, value_inner in value.items():
-                            entries.append({"key": key_inner, "value": value_inner})
+                            entries.append({_JSON_KEY: key_inner, _JSON_VALUE: value_inner})
 
                         padding: dict[str, Any] = dict()
                         padding["entries"] = entries
                         value_ = padding
 
                     actual[key_] = value_
 
@@ -165,49 +182,49 @@
 
         return result
 
 
 @jsonpickle.handlers.register(Decimal)
 class DecimalHandler(jsonpickle.handlers.BaseHandler):
     def flatten(self, obj: object, data: dict[str, Any]) -> dict[str, Any]:
-        return {"@class": "math.BigDec", "value": str(obj)}
+        return {_META_CLASS: _BIG_DEC_ALIAS, _JSON_VALUE: str(obj)}
 
     def restore(self, obj: dict[str, Any]) -> Decimal:
-        return Decimal(obj["value"])
+        return Decimal(obj[_JSON_VALUE])
 
 
 @jsonpickle.handlers.register(int)
 class LargeIntHandler(jsonpickle.handlers.BaseHandler):
     def flatten(self, obj: object, data: dict[str, Any]) -> dict[str, Any]:
-        return {"@class": "math.BigInt", "value": str(obj)}
+        return {_META_CLASS: _BIG_INT_ALIAS, _JSON_VALUE: str(obj)}
 
     def restore(self, obj: dict[str, Any]) -> int:
-        return int(obj["value"])
+        return int(obj[_JSON_VALUE])
 
 
 class JavaProxyUnpickler(jsonpickle.Unpickler):
     # noinspection PyUnresolvedReferences
     def _restore(self, obj: Any) -> Any:
         if isinstance(obj, dict):
-            metadata: str = obj.get("@class", None)
+            metadata: str = obj.get(_META_CLASS, None)
             if metadata is not None:
                 type_: Optional[Type[Any]] = _type_for(metadata)
                 actual: dict[str, Any] = dict()
                 if type_ is None:
                     if "map" in metadata.lower():
-                        for entry in obj["entries"]:
-                            actual[entry["key"]] = entry["value"]
+                        for entry in obj[_JSON_ENTRIES]:
+                            actual[entry[_JSON_KEY]] = entry[_JSON_VALUE]
                     else:
                         return obj
                 else:
                     type_name = jsonpickle.util.importable_name(type_)
-                    actual["py/object"] = type_name
+                    actual[_JSON_PICKLE_OBJ] = type_name
                     rev_map = _attribute_mappings_rev.get(type_name, None)
                     for key, value in obj.items():
-                        if key == "@class":
+                        if key == _META_CLASS:
                             continue
 
                         key_ = rev_map.get(key, None) if rev_map is not None else None
                         actual[key_ if key_ is not None else key] = value
 
                 return super().restore(actual, reset=False)
 
@@ -283,9 +300,9 @@
         _register(type_, alias)
 
         return type_
 
     return _do_register
 
 
-_register(Decimal, "math.BigDec")
-_register(int, "math.BigInt")
+_register(Decimal, _BIG_DEC_ALIAS)
+_register(int, _BIG_INT_ALIAS)
```

### Comparing `coherence_client-1.0rc2/src/coherence/services_pb2.py` & `coherence_client-1.1.0/src/coherence/services_pb2.py`

 * *Files identical despite different names*

### Comparing `coherence_client-1.0rc2/src/coherence/services_pb2_grpc.py` & `coherence_client-1.1.0/src/coherence/services_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `coherence_client-1.0rc2/src/coherence/util.py` & `coherence_client-1.1.0/src/coherence/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,16 +5,18 @@
 from __future__ import annotations
 
 import time
 from typing import Optional, TypeVar
 
 from .aggregator import EntryAggregator
 from .comparator import Comparator
+from .extractor import ValueExtractor
 from .filter import Filter, Filters, MapEventFilter
 from .messages_pb2 import (  # type: ignore
+    AddIndexRequest,
     AggregateRequest,
     ClearRequest,
     ContainsKeyRequest,
     ContainsValueRequest,
     DestroyRequest,
     Entry,
     EntrySetRequest,
@@ -25,14 +27,15 @@
     IsEmptyRequest,
     KeySetRequest,
     MapListenerRequest,
     PageRequest,
     PutAllRequest,
     PutIfAbsentRequest,
     PutRequest,
+    RemoveIndexRequest,
     RemoveMappingRequest,
     RemoveRequest,
     ReplaceMappingRequest,
     ReplaceRequest,
     SizeRequest,
     TruncateRequest,
     ValuesRequest,
@@ -59,60 +62,60 @@
     def get_serializer(self) -> Serializer:
         return self._serializer
 
     def put_request(self, key: K, value: V, ttl: int = -1) -> PutRequest:
         p = PutRequest(
             scope=self._scope,
             cache=self._cache_name,
-            format=self._serializer.format(),
+            format=self._serializer.format,
             key=self._serializer.serialize(key),
             value=self._serializer.serialize(value),
             ttl=ttl,
         )
         return p
 
     def get_request(self, key: K) -> GetRequest:
         g = GetRequest(
             scope=self._scope,
             cache=self._cache_name,
-            format=self._serializer.format(),
+            format=self._serializer.format,
             key=self._serializer.serialize(key),
         )
         return g
 
     def get_all_request(self, keys: set[K]) -> GetRequest:
         if keys is None:
             raise ValueError("Must specify a set of keys")
 
-        g: GetAllRequest = GetAllRequest(scope=self._scope, cache=self._cache_name, format=self._serializer.format())
+        g: GetAllRequest = GetAllRequest(scope=self._scope, cache=self._cache_name, format=self._serializer.format)
 
         for key in keys:
             g.key.append(self._serializer.serialize(key))
 
         return g
 
     def put_if_absent_request(self, key: K, value: V, ttl: int = -1) -> PutIfAbsentRequest:
         p = PutIfAbsentRequest(
             scope=self._scope,
             cache=self._cache_name,
-            format=self._serializer.format(),
+            format=self._serializer.format,
             key=self._serializer.serialize(key),
             value=self._serializer.serialize(value),
             ttl=ttl,
         )
         return p
 
     def put_all_request(self, map: dict[K, V]) -> PutAllRequest:
         entry_list = list()
         for key, value in map.items():
             k = self._serializer.serialize(key)
             v = self._serializer.serialize(value)
             e = Entry(key=k, value=v)
             entry_list.append(e)
-        p = PutAllRequest(scope=self._scope, cache=self._cache_name, format=self._serializer.format(), entry=entry_list)
+        p = PutAllRequest(scope=self._scope, cache=self._cache_name, format=self._serializer.format, entry=entry_list)
         return p
 
     def clear_request(self) -> ClearRequest:
         r = ClearRequest(scope=self._scope, cache=self._cache_name)
         return r
 
     def destroy_request(self) -> DestroyRequest:
@@ -123,64 +126,64 @@
         r = TruncateRequest(scope=self._scope, cache=self._cache_name)
         return r
 
     def remove_request(self, key: K) -> RemoveRequest:
         r = RemoveRequest(
             scope=self._scope,
             cache=self._cache_name,
-            format=self._serializer.format(),
+            format=self._serializer.format,
             key=self._serializer.serialize(key),
         )
         return r
 
     def remove_mapping_request(self, key: K, value: V) -> RemoveMappingRequest:
         r = RemoveMappingRequest(
             scope=self._scope,
             cache=self._cache_name,
-            format=self._serializer.format(),
+            format=self._serializer.format,
             key=self._serializer.serialize(key),
             value=self._serializer.serialize(value),
         )
         return r
 
     def replace_request(self, key: K, value: V) -> ReplaceRequest:
         r = ReplaceRequest(
             scope=self._scope,
             cache=self._cache_name,
-            format=self._serializer.format(),
+            format=self._serializer.format,
             key=self._serializer.serialize(key),
             value=self._serializer.serialize(value),
         )
         return r
 
     def replace_mapping_request(self, key: K, old_value: V, new_value: V) -> ReplaceMappingRequest:
         r = ReplaceMappingRequest(
             scope=self._scope,
             cache=self._cache_name,
-            format=self._serializer.format(),
+            format=self._serializer.format,
             key=self._serializer.serialize(key),
             previousValue=self._serializer.serialize(old_value),
             newValue=self._serializer.serialize(new_value),
         )
         return r
 
     def contains_key_request(self, key: K) -> ContainsKeyRequest:
         r = ContainsKeyRequest(
             scope=self._scope,
             cache=self._cache_name,
-            format=self._serializer.format(),
+            format=self._serializer.format,
             key=self._serializer.serialize(key),
         )
         return r
 
     def contains_value_request(self, value: V) -> ContainsValueRequest:
         r = ContainsValueRequest(
             scope=self._scope,
             cache=self._cache_name,
-            format=self._serializer.format(),
+            format=self._serializer.format,
             value=self._serializer.serialize(value),
         )
         return r
 
     def is_empty_request(self) -> IsEmptyRequest:
         r = IsEmptyRequest(scope=self._scope, cache=self._cache_name)
         return r
@@ -189,30 +192,30 @@
         r = SizeRequest(scope=self._scope, cache=self._cache_name)
         return r
 
     def invoke_request(self, key: K, processor: EntryProcessor[R]) -> InvokeRequest:
         r = InvokeRequest(
             scope=self._scope,
             cache=self._cache_name,
-            format=self._serializer.format(),
+            format=self._serializer.format,
             processor=self._serializer.serialize(processor),
             key=self._serializer.serialize(key),
         )
         return r
 
     def invoke_all_request(
         self, processor: EntryProcessor[R], keys: Optional[set[K]] = None, filter: Optional[Filter] = None
     ) -> InvokeAllRequest:
         if keys is not None and filter is not None:
             raise ValueError("keys and filter are mutually exclusive")
 
         r = InvokeAllRequest(
             scope=self._scope,
             cache=self._cache_name,
-            format=self._serializer.format(),
+            format=self._serializer.format,
             processor=self._serializer.serialize(processor),
         )
 
         if keys is not None:
             for key in keys:
                 r.keys.append(self._serializer.serialize(key))
         else:
@@ -225,15 +228,15 @@
     ) -> AggregateRequest:
         if keys is not None and filter is not None:
             raise ValueError("keys and filter are mutually exclusive")
 
         r: AggregateRequest = AggregateRequest(
             scope=self._scope,
             cache=self._cache_name,
-            format=self._serializer.format(),
+            format=self._serializer.format,
             aggregator=self._serializer.serialize(aggregator),
         )
 
         if keys is not None:
             for key in keys:
                 r.keys.append(self._serializer.serialize(key))
         if filter is not None:
@@ -244,30 +247,30 @@
     def values_request(self, filter: Optional[Filter] = None, comparator: Optional[Comparator] = None) -> ValuesRequest:
         if filter is None and comparator is not None:
             raise ValueError("Filter cannot be None")
 
         r: ValuesRequest = ValuesRequest(
             scope=self._scope,
             cache=self._cache_name,
-            format=self._serializer.format(),
+            format=self._serializer.format,
         )
 
         if filter is not None:
             r.filter = self._serializer.serialize(filter)
 
         if comparator is not None:
             r.comparator = self._serializer.serialize(comparator)
 
         return r
 
     def keys_request(self, filter: Optional[Filter] = None) -> KeySetRequest:
         r: KeySetRequest = KeySetRequest(
             scope=self._scope,
             cache=self._cache_name,
-            format=self._serializer.format(),
+            format=self._serializer.format,
         )
 
         if filter is not None:
             r.filter = self._serializer.serialize(filter)
 
         return r
 
@@ -276,15 +279,15 @@
     ) -> EntrySetRequest:
         if filter is None and comparator is not None:
             raise ValueError("Filter cannot be None")
 
         r: EntrySetRequest = EntrySetRequest(
             scope=self._scope,
             cache=self._cache_name,
-            format=self._serializer.format(),
+            format=self._serializer.format,
         )
 
         if filter is not None:
             r.filter = self._serializer.serialize(filter)
 
         if comparator is not None:
             r.comparator = self._serializer.serialize(comparator)
@@ -296,29 +299,29 @@
         Creates a gRPC PageRequest.
 
         :param cookie: the cookie used for paging
         :return: a new PageRequest
         """
 
         r: PageRequest = PageRequest(
-            scope=self._scope, cache=self._cache_name, format=self._serializer.format(), cookie=cookie
+            scope=self._scope, cache=self._cache_name, format=self._serializer.format, cookie=cookie
         )
 
         return r
 
     def map_listener_request(
         self, subscribe: bool, lite: bool = False, *, key: Optional[K] = None, filter: Optional[Filter] = None
     ) -> MapListenerRequest:
         """Creates a gRPC generated MapListenerRequest"""
 
         if key is None and filter is None:
             raise AssertionError("Must specify a key or a filter")
 
         request: MapListenerRequest = MapListenerRequest(
-            cache=self._cache_name, scope=self._scope, format=self._serializer.format()
+            cache=self._cache_name, scope=self._scope, format=self._serializer.format
         )
 
         request.lite = lite
         request.subscribe = subscribe
         request.uid = self.__generate_next_request_id("key" if key is not None else "filter")
         request.trigger = bytes()
         request.priming = False
@@ -336,19 +339,45 @@
 
             request.filter = self._serializer.serialize(filter_local)
 
         return request
 
     def map_event_subscribe(self) -> MapListenerRequest:
         request: MapListenerRequest = MapListenerRequest(
-            cache=self._cache_name, scope=self._scope, format=self._serializer.format()
+            cache=self._cache_name, scope=self._scope, format=self._serializer.format
         )
         request.uid = self.__generate_next_request_id("init")
         request.subscribe = True
         request.type = MapListenerRequest.RequestType.INIT
 
         return request
 
     def __generate_next_request_id(self, prefix: str) -> str:
         """Generates a prefix map-specific prefix when starting a MapEvent gRPC stream."""
         self.__next_request_id += 1
         return prefix + self.__uidPrefix + str(self.__next_request_id)
+
+    def add_index_request(
+        self, extractor: ValueExtractor[T, E], ordered: bool = False, comparator: Optional[Comparator] = None
+    ) -> AddIndexRequest:
+        r = AddIndexRequest(
+            scope=self._scope,
+            cache=self._cache_name,
+            format=self._serializer.format,
+            extractor=self._serializer.serialize(extractor),
+        )
+        r.sorted = ordered
+
+        if comparator is not None:
+            r.comparator = self._serializer.serialize(comparator)
+
+        return r
+
+    def remove_index_request(self, extractor: ValueExtractor[T, E]) -> RemoveIndexRequest:
+        r = RemoveIndexRequest(
+            scope=self._scope,
+            cache=self._cache_name,
+            format=self._serializer.format,
+            extractor=self._serializer.serialize(extractor),
+        )
+
+        return r
```

### Comparing `coherence_client-1.0rc2/PKG-INFO` & `coherence_client-1.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 Metadata-Version: 2.1
 Name: coherence-client
-Version: 1.0rc2
+Version: 1.1.0
 Summary: The Coherence Python Client allows Python applications to act as cache clients to a Coherence Cluster using Google's gRPC framework as the network transport.
 Home-page: https://github.com/oracle/coherence-py-client
 Author: Oracle
 Author-email: dhiru.pandey@oracle.com
-Requires-Python: >=3.11,<3.12
-Classifier: Development Status :: 4 - Beta
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Universal Permissive License (UPL)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: grpcio (>=1.54,<1.57)
-Requires-Dist: grpcio-tools (>=1.54,<1.57)
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: grpcio (>=1.54,<1.63)
+Requires-Dist: grpcio-tools (>=1.54,<1.63)
 Requires-Dist: jsonpickle (>=3.0,<3.1)
-Requires-Dist: protobuf (>=4.23,<4.24)
-Requires-Dist: pymitter (>=0.4,<0.5)
+Requires-Dist: protobuf (>=4.23,<4.26)
+Requires-Dist: pymitter (>=0.4,<0.6)
+Requires-Dist: typing-extensions (>=4.11,<4.12)
 Project-URL: Repository, https://github.com/oracle/coherence-py-client
 Description-Content-Type: text/markdown
 
 # Coherence Python Client
 
 ![CI/CD](https://github.com/oracle/coherence-py-client/actions/workflows/validate.yml/badge.svg)
+[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=oracle_coherence-py-client&metric=alert_status)](https://sonarcloud.io/project/overview?id=oracle_coherence-py-client)
 [![License](http://img.shields.io/badge/license-UPL%201.0-blue.svg)](https://oss.oracle.com/licenses/upl/)
 
 <img src=https://oracle.github.io/coherence/assets/images/logo-red.png width="30%"><img>
 
 The Coherence Python Client allows Python applications to act as cache clients to an Oracle Coherence cluster using gRPC as the network transport.
 
 #### Features
@@ -37,25 +43,25 @@
     * mutations such as insert, update and delete on Maps
     * map lifecycle events such as truncated, released or destroyed
     * session lifecycle events such as connected, disconnected, reconnected and closed
 * Support for storing Python objects as JSON as well as the ability to serialize to Java objects on the server for access from other Coherence language API's
 
 #### Requirements
 * [Coherence CE](https://github.com/oracle/coherence) 22.06.4+ or Coherence 14.1.1.2206.4+ Commercial edition with a configured [gRPCProxy](https://docs.oracle.com/en/middleware/standalone/coherence/14.1.1.2206/develop-remote-clients/using-coherence-grpc-server.html).
-* Python 3.11.x
+* Python 3.8.x
 
 
 #### Starting a Coherence Cluster
 
 Before testing the Python client, you must ensure a Coherence cluster is available.
 For local development, we recommend using the Coherence CE Docker image; it contains
 everything necessary for the client to operate correctly.
 
 ```bash
-docker run -d -p 1408:1408 ghcr.io/oracle/coherence-ce:22.06.4
+docker run -d -p 1408:1408 ghcr.io/oracle/coherence-ce:24.03
 ```
 
 ## Installation
 
 ```bash
 python3 -m pip install coherence-client
 ```
@@ -69,23 +75,24 @@
 The following example connects to a Coherence cluster running gRPC Proxy on default
 port of 1408, creates a new `NamedCache` with key `str` and value of a `str|int` and
 issues `put()`, `get()`, `size()` and `remove` operations.
 
 ```python
 from coherence import NamedCache, Session
 import asyncio
+from typing import Union
 
 
 async def run_test():
 
     # create a new Session to the Coherence server
     session: Session = await Session.create()
 
     # create a new NamedCache with key of string|int and value of string|int
-    cache: NamedCache[str, str|int] = await session.get_cache("test")
+    cache: NamedCache[str, Union[str,int]] = await session.get_cache("test")
 
     # put a new key/value
     k: str = "one"
     v: str = "only-one"
     await cache.put(k, v)
 
     # get the value for a key in the cache
@@ -108,15 +115,15 @@
 
 
 # run the test
 asyncio.run(run_test())
 ```
 ## Help
 
-We have a **public Slack channel** where you can get in touch with us to ask questions about using the Coherence CLI
+We have a **public Slack channel** where you can get in touch with us to ask questions about using the Coherence Python Client
 or give us feedback or suggestions about what features and improvements you would like to see. We would love
 to hear from you. To join our channel,
 please [visit this site to get an invitation](https://join.slack.com/t/oraclecoherence/shared_invite/enQtNzcxNTQwMTAzNjE4LTJkZWI5ZDkzNGEzOTllZDgwZDU3NGM2YjY5YWYwMzM3ODdkNTU2NmNmNDFhOWIxMDZlNjg2MzE3NmMxZWMxMWE).
 The invitation email will include details of how to access our Slack
 workspace.  After you are logged in, please come to `#coherence` and say, "hello!"
 
 If you would like to raise an issue please see [here](https://github.com/oracle/coherence-py-client/issues/new/choose).
@@ -127,12 +134,12 @@
 
 ## Security
 
 Please consult the [security guide](./SECURITY.md) for our responsible security vulnerability disclosure process
 
 ## License
 
-Copyright (c) 2023 Oracle and/or its affiliates.
+Copyright (c) 2023, 2024, Oracle and/or its affiliates.
 
 Released under the Universal Permissive License v1.0 as shown at
 <https://oss.oracle.com/licenses/upl/>.
```

