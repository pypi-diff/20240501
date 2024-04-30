# Comparing `tmp/vatsim-0.1.0.tar.gz` & `tmp/vatsim-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vatsim-0.1.0.tar", max compression
+gzip compressed data, was "vatsim-0.1.1.tar", max compression
```

## Comparing `vatsim-0.1.0.tar` & `vatsim-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1068 2024-01-31 15:42:07.906197 vatsim-0.1.0/LICENSE
--rw-r--r--   0        0        0      510 2024-01-31 15:42:07.906197 vatsim-0.1.0/README.md
--rw-r--r--   0        0        0     1017 2024-01-31 15:42:07.906197 vatsim-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      192 2024-01-31 15:42:07.906197 vatsim-0.1.0/vatsim/__init__.py
--rw-r--r--   0        0        0       58 2024-01-31 15:42:07.906197 vatsim-0.1.0/vatsim/constants.py
--rw-r--r--   0        0        0      594 2024-01-31 15:42:07.906197 vatsim-0.1.0/vatsim/fetchers.py
--rw-r--r--   0        0        0        0 2024-01-31 15:42:07.906197 vatsim-0.1.0/vatsim/py.typed
--rw-r--r--   0        0        0     3993 2024-01-31 15:42:07.906197 vatsim-0.1.0/vatsim/types.py
--rw-r--r--   0        0        0     1347 1970-01-01 00:00:00.000000 vatsim-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-30 22:37:54.587182 vatsim-0.1.1/LICENSE
+-rw-r--r--   0        0        0      510 2024-04-30 22:37:54.587182 vatsim-0.1.1/README.md
+-rw-r--r--   0        0        0     1882 2024-04-30 22:37:54.587182 vatsim-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      229 2024-04-30 22:37:54.587182 vatsim-0.1.1/vatsim/__init__.py
+-rw-r--r--   0        0        0      146 2024-04-30 22:37:54.591182 vatsim-0.1.1/vatsim/constants.py
+-rw-r--r--   0        0        0      599 2024-04-30 22:37:54.591182 vatsim-0.1.1/vatsim/fetchers.py
+-rw-r--r--   0        0        0        0 2024-04-30 22:37:54.591182 vatsim-0.1.1/vatsim/py.typed
+-rw-r--r--   0        0        0     4129 2024-04-30 22:37:54.591182 vatsim-0.1.1/vatsim/types.py
+-rw-r--r--   0        0        0     1347 1970-01-01 00:00:00.000000 vatsim-0.1.1/PKG-INFO
```

### Comparing `vatsim-0.1.0/LICENSE` & `vatsim-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vatsim-0.1.0/vatsim/fetchers.py` & `vatsim-0.1.1/vatsim/fetchers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 from functools import cache
-from typing import Optional
 
 import requests
+from pydantic import HttpUrl
 
 from .constants import STATUS_JSON_URL
 from .types import VatsimData, VatsimEndpoints
 
 
 @cache
-def fetch_vatsim_endpoints(url=STATUS_JSON_URL):
-    return VatsimEndpoints.model_validate_json(requests.get(url).text)
+def fetch_vatsim_endpoints(url: HttpUrl = STATUS_JSON_URL):
+    return VatsimEndpoints.model_validate_json(requests.get(str(url)).text)
 
 
-def fetch_vatsim_data(
-    url: Optional[str] = None, endpoints: Optional[VatsimEndpoints] = None
-):
+def fetch_vatsim_data(url: str | None = None, endpoints: VatsimEndpoints | None = None):
     if url is None:
         if endpoints is None:
             endpoints = fetch_vatsim_endpoints()
 
         url = endpoints.data.v3[0]
 
     return VatsimData.model_validate_json(requests.get(url).text)
```

### Comparing `vatsim-0.1.0/vatsim/types.py` & `vatsim-0.1.1/vatsim/types.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,55 +1,56 @@
 import itertools
 from datetime import datetime
-from typing import Any, List, Optional
+from typing import Any, cast
 
 import regex
 from pydantic import AwareDatetime, BaseModel, HttpUrl, field_validator, model_validator
 
 
 class Atis(BaseModel):
     cid: int
     name: str
     callsign: str
     frequency: str
     facility: int
     rating: int
     server: str
     visual_range: int
-    atis_code: Optional[str]
+    atis_code: str | None
     logon_time: AwareDatetime
     last_updated: AwareDatetime
-    text_atis: str
-    runways_in_use: List[str]
+    text_atis: str | None
+    runways_in_use: list[str]
 
     @field_validator("callsign", mode="before")
     @classmethod
     def callsign_validator(cls, v: str) -> str:
         if v.endswith("_A_ATIS"):
             return v.removesuffix("_A_ATIS")
         return v.removesuffix("_ATIS")
 
     @model_validator(mode="before")
     @classmethod
-    def atis_validator(cls, data: Any) -> Any:
-        if isinstance(data, dict):
-            text_atis = data.get("text_atis", [])
-            data["text_atis"] = (
-                text_atis if isinstance(text_atis, str) else "\n".join(text_atis or "")
-            )
-
-            matches = regex.search(
-                r"(RWYS|RUNWAYS?)\sIN\sUSE\s(FOR\sLANDING\s)?((?P<first>[0-9]{2}[A-Z]?)\s)+(AND\s(TAKEOFF\s)?(?P<and>[0-9]{2}[A-Z]?))?",
-                data["text_atis"],
-            )
-            data["runways_in_use"] = (
-                []
-                if matches is None
-                else itertools.chain.from_iterable(matches.captures("first", "and"))
-            )
+    def atis_validator(cls, data: dict[str, Any] | Any) -> Any:
+        if isinstance(data, dict) and "text_atis" in data:
+            if data["text_atis"] is not None:
+                if not isinstance(data["text_atis"], str):
+                    data["text_atis"] = "\n".join(cast(list[str], data["text_atis"]))
+
+                matches = regex.search(
+                    r"(RWYS|RUNWAYS?)\sIN\sUSE\s(FOR\sLANDING\s)?((?P<first>[0-9]{2}[A-Z]?)\s)+(AND\s(TAKEOFF\s)?(?P<and>[0-9]{2}[A-Z]?))?",
+                    data["text_atis"],
+                )
+                data["runways_in_use"] = (
+                    itertools.chain.from_iterable(matches.captures("first", "and"))
+                    if matches is not None
+                    else []
+                )
+            else:
+                data["runways_in_use"] = []
 
         return data
 
 
 class Controller(BaseModel):
     cid: int
     name: str
@@ -61,15 +62,15 @@
     visual_range: int
     logon_time: AwareDatetime
     last_updated: AwareDatetime
     text_atis: str
 
     @field_validator("text_atis", mode="before")
     @classmethod
-    def atis_validator(cls, v: Optional[list[str]]) -> str:
+    def atis_validator(cls, v: list[str] | None) -> str:
         if v is None:
             return ""
         return "\n".join(v)
 
 
 class Facility(BaseModel):
     id: int
@@ -123,15 +124,15 @@
     longitude: float
     altitude: int
     groundspeed: int
     transponder: str
     heading: int
     qnh_i_hg: float
     qnh_mb: int
-    flight_plan: Optional[FlightPlan]
+    flight_plan: FlightPlan | None
     logon_time: datetime
     last_updated: datetime
 
 
 class Server(BaseModel):
     ident: str
     hostname_or_ip: str
@@ -169,17 +170,17 @@
     facilities: list[Facility]
     ratings: list[Rating]
     pilot_ratings: list[PilotRating]
     military_ratings: list[MilitaryRating]
 
 
 class VatsimDataEndpoints(BaseModel):
-    v3: List[str]
-    transceivers: List[HttpUrl]
-    servers: List[HttpUrl]
-    servers_sweatbox: List[HttpUrl]
+    v3: list[str]
+    transceivers: list[HttpUrl]
+    servers: list[HttpUrl]
+    servers_sweatbox: list[HttpUrl]
 
 
 class VatsimEndpoints(BaseModel):
     data: VatsimDataEndpoints
-    user: List[HttpUrl]
-    metar: List[HttpUrl]
+    user: list[HttpUrl]
+    metar: list[HttpUrl]
```

### Comparing `vatsim-0.1.0/PKG-INFO` & `vatsim-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vatsim
-Version: 0.1.0
+Version: 0.1.1
 Summary: Library for interacting with VATSIM APIs and data
 License: MIT
 Author: Franz Pletz
 Author-email: fpletz@fnordicwalking.de
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -12,15 +12,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Games/Entertainment :: Simulation
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: pydantic (>=2.5,<3.0)
-Requires-Dist: regex (>=2023.12.25,<2024.0.0)
+Requires-Dist: regex (>=2023.12.25,<2025.0.0)
 Requires-Dist: requests (>=2.28,<3.0)
 Description-Content-Type: text/markdown
 
 # python-vatsim
 
 This module aims to provide functionality to interact with VATSIM APIs and the datafeed. In the
 future, it will also include parsers for different file formats like Sectorfiles or ESE files
```

