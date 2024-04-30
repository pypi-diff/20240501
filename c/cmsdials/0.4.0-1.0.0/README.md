# Comparing `tmp/cmsdials-0.4.0.tar.gz` & `tmp/cmsdials-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmsdials-0.4.0.tar", max compression
+gzip compressed data, was "cmsdials-1.0.0.tar", max compression
```

## Comparing `cmsdials-0.4.0.tar` & `cmsdials-1.0.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0    35149 2024-02-28 16:14:27.566813 cmsdials-0.4.0/LICENSE
--rw-r--r--   0        0        0     5345 2024-04-11 21:19:49.049949 cmsdials-0.4.0/README.md
--rw-r--r--   0        0        0       49 2024-03-06 14:04:55.052320 cmsdials-0.4.0/cmsdials/__init__.py
--rw-r--r--   0        0        0        0 2024-03-01 11:33:02.539393 cmsdials-0.4.0/cmsdials/auth/__init__.py
--rw-r--r--   0        0        0     4136 2024-03-06 14:44:11.087545 cmsdials-0.4.0/cmsdials/auth/_base.py
--rw-r--r--   0        0        0     4998 2024-04-09 11:53:11.488972 cmsdials-0.4.0/cmsdials/auth/bearer.py
--rw-r--r--   0        0        0     3491 2024-03-06 14:44:11.092545 cmsdials-0.4.0/cmsdials/auth/client.py
--rw-r--r--   0        0        0      107 2024-03-06 14:46:20.706557 cmsdials-0.4.0/cmsdials/auth/exceptions.py
--rw-r--r--   0        0        0      425 2024-03-01 14:52:11.874008 cmsdials-0.4.0/cmsdials/auth/models.py
--rw-r--r--   0        0        0     1041 2024-04-09 10:09:21.911337 cmsdials-0.4.0/cmsdials/auth/secret_key.py
--rw-r--r--   0        0        0        0 2024-02-29 13:09:10.635273 cmsdials-0.4.0/cmsdials/clients/__init__.py
--rw-r--r--   0        0        0        0 2024-02-29 13:10:09.799214 cmsdials-0.4.0/cmsdials/clients/file_index/__init__.py
--rw-r--r--   0        0        0      318 2024-03-07 16:12:57.394240 cmsdials-0.4.0/cmsdials/clients/file_index/client.py
--rw-r--r--   0        0        0      988 2024-04-11 21:19:49.049949 cmsdials-0.4.0/cmsdials/clients/file_index/models.py
--rw-r--r--   0        0        0        0 2024-02-29 13:10:14.034210 cmsdials-0.4.0/cmsdials/clients/h1d/__init__.py
--rw-r--r--   0        0        0      414 2024-03-07 16:12:57.394240 cmsdials-0.4.0/cmsdials/clients/h1d/client.py
--rw-r--r--   0        0        0     1143 2024-04-11 21:19:49.050949 cmsdials-0.4.0/cmsdials/clients/h1d/models.py
--rw-r--r--   0        0        0        0 2024-02-29 13:10:18.548206 cmsdials-0.4.0/cmsdials/clients/h2d/__init__.py
--rw-r--r--   0        0        0      414 2024-03-07 16:12:57.394240 cmsdials-0.4.0/cmsdials/clients/h2d/client.py
--rw-r--r--   0        0        0     1188 2024-04-11 21:19:49.050949 cmsdials-0.4.0/cmsdials/clients/h2d/models.py
--rw-r--r--   0        0        0        0 2024-02-29 13:10:24.058200 cmsdials-0.4.0/cmsdials/clients/lumisection/__init__.py
--rw-r--r--   0        0        0      333 2024-04-11 21:19:49.050949 cmsdials-0.4.0/cmsdials/clients/lumisection/client.py
--rw-r--r--   0        0        0      671 2024-04-11 21:19:49.050949 cmsdials-0.4.0/cmsdials/clients/lumisection/models.py
--rw-r--r--   0        0        0        0 2024-02-29 13:10:29.247195 cmsdials-0.4.0/cmsdials/clients/run/__init__.py
--rw-r--r--   0        0        0      269 2024-03-07 16:12:57.394240 cmsdials-0.4.0/cmsdials/clients/run/client.py
--rw-r--r--   0        0        0      452 2024-04-11 21:19:49.050949 cmsdials-0.4.0/cmsdials/clients/run/models.py
--rw-r--r--   0        0        0      943 2024-04-11 21:19:49.050949 cmsdials-0.4.0/cmsdials/cmsdials.py
--rw-r--r--   0        0        0      439 2024-04-11 21:19:49.050949 cmsdials-0.4.0/cmsdials/filters.py
--rw-r--r--   0        0        0        0 2024-03-01 09:40:35.448258 cmsdials-0.4.0/cmsdials/utils/__init__.py
--rw-r--r--   0        0        0      671 2024-03-06 14:48:21.185636 cmsdials-0.4.0/cmsdials/utils/_json.py
--rw-r--r--   0        0        0     4827 2024-04-11 21:19:49.050949 cmsdials-0.4.0/cmsdials/utils/api_client.py
--rw-r--r--   0        0        0      174 2024-03-01 09:40:15.133277 cmsdials-0.4.0/cmsdials/utils/base_model.py
--rw-r--r--   0        0        0      145 2024-03-06 14:44:10.568545 cmsdials-0.4.0/cmsdials/utils/logger.py
--rw-r--r--   0        0        0      784 2024-04-11 21:19:49.050949 cmsdials-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     6279 1970-01-01 00:00:00.000000 cmsdials-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-28 10:36:23.872227 cmsdials-1.0.0/LICENSE
+-rw-r--r--   0        0        0     5484 2024-04-29 19:09:44.714827 cmsdials-1.0.0/README.md
+-rw-r--r--   0        0        0       49 2024-04-28 10:36:23.872227 cmsdials-1.0.0/cmsdials/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 10:36:23.872227 cmsdials-1.0.0/cmsdials/auth/__init__.py
+-rw-r--r--   0        0        0     4136 2024-04-28 10:36:23.873227 cmsdials-1.0.0/cmsdials/auth/_base.py
+-rw-r--r--   0        0        0     4998 2024-04-28 10:36:23.873227 cmsdials-1.0.0/cmsdials/auth/bearer.py
+-rw-r--r--   0        0        0     3491 2024-04-28 10:36:23.873227 cmsdials-1.0.0/cmsdials/auth/client.py
+-rw-r--r--   0        0        0      107 2024-04-28 10:36:23.873227 cmsdials-1.0.0/cmsdials/auth/exceptions.py
+-rw-r--r--   0        0        0      425 2024-04-28 10:36:23.874227 cmsdials-1.0.0/cmsdials/auth/models.py
+-rw-r--r--   0        0        0     1041 2024-04-28 10:36:23.874227 cmsdials-1.0.0/cmsdials/auth/secret_key.py
+-rw-r--r--   0        0        0        0 2024-04-28 10:36:23.874227 cmsdials-1.0.0/cmsdials/clients/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 10:36:23.874227 cmsdials-1.0.0/cmsdials/clients/file_index/__init__.py
+-rw-r--r--   0        0        0      318 2024-04-28 10:36:23.874227 cmsdials-1.0.0/cmsdials/clients/file_index/client.py
+-rw-r--r--   0        0        0      962 2024-04-29 19:06:30.058424 cmsdials-1.0.0/cmsdials/clients/file_index/models.py
+-rw-r--r--   0        0        0        0 2024-04-28 10:36:23.875227 cmsdials-1.0.0/cmsdials/clients/h1d/__init__.py
+-rw-r--r--   0        0        0      402 2024-04-29 11:53:55.385012 cmsdials-1.0.0/cmsdials/clients/h1d/client.py
+-rw-r--r--   0        0        0     1360 2024-04-29 19:06:46.571391 cmsdials-1.0.0/cmsdials/clients/h1d/models.py
+-rw-r--r--   0        0        0        0 2024-04-28 10:36:23.875227 cmsdials-1.0.0/cmsdials/clients/h2d/__init__.py
+-rw-r--r--   0        0        0      402 2024-04-29 11:53:59.860011 cmsdials-1.0.0/cmsdials/clients/h2d/client.py
+-rw-r--r--   0        0        0     1411 2024-04-29 19:06:54.307376 cmsdials-1.0.0/cmsdials/clients/h2d/models.py
+-rw-r--r--   0        0        0        0 2024-04-28 10:36:23.877227 cmsdials-1.0.0/cmsdials/clients/lumisection/__init__.py
+-rw-r--r--   0        0        0      946 2024-04-29 13:18:14.360705 cmsdials-1.0.0/cmsdials/clients/lumisection/client.py
+-rw-r--r--   0        0        0      871 2024-04-29 19:07:02.068360 cmsdials-1.0.0/cmsdials/clients/lumisection/models.py
+-rw-r--r--   0        0        0        0 2024-04-28 10:36:23.877227 cmsdials-1.0.0/cmsdials/clients/run/__init__.py
+-rw-r--r--   0        0        0      854 2024-04-29 13:18:14.362705 cmsdials-1.0.0/cmsdials/clients/run/client.py
+-rw-r--r--   0        0        0      667 2024-04-29 19:07:09.219346 cmsdials-1.0.0/cmsdials/clients/run/models.py
+-rw-r--r--   0        0        0      847 2024-04-29 19:13:59.398882 cmsdials-1.0.0/cmsdials/cmsdials.py
+-rw-r--r--   0        0        0      439 2024-04-28 10:36:23.878227 cmsdials-1.0.0/cmsdials/filters.py
+-rw-r--r--   0        0        0        0 2024-04-28 10:36:23.878227 cmsdials-1.0.0/cmsdials/utils/__init__.py
+-rw-r--r--   0        0        0      671 2024-04-28 10:36:23.878227 cmsdials-1.0.0/cmsdials/utils/_json.py
+-rw-r--r--   0        0        0     3557 2024-04-29 19:13:59.688881 cmsdials-1.0.0/cmsdials/utils/api_client.py
+-rw-r--r--   0        0        0      174 2024-04-28 10:36:23.878227 cmsdials-1.0.0/cmsdials/utils/base_model.py
+-rw-r--r--   0        0        0      145 2024-04-28 10:36:23.878227 cmsdials-1.0.0/cmsdials/utils/logger.py
+-rw-r--r--   0        0        0     2720 2024-04-30 23:36:22.164299 cmsdials-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     6431 1970-01-01 00:00:00.000000 cmsdials-1.0.0/PKG-INFO
```

### Comparing `cmsdials-0.4.0/LICENSE` & `cmsdials-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cmsdials-0.4.0/README.md` & `cmsdials-1.0.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -49,40 +49,40 @@
 
 ```python
 from cmsdials.auth.bearer import Credentials
 from cmsdials import Dials
 from cmsdials.filters import LumisectionHistogram1DFilters
 
 creds = Credentials.from_creds_file()
-dials = Dials(creds, nthreads=2)
+dials = Dials(creds)
 
 # Getting h1d data
-data = dials.h1d.list_all(LumisectionHistogram1DFilters(title="PixelPhase1/Tracks/PXBarrel/charge_PXLayer_2"), max_pages=5)
+data = dials.h1d.list_all(LumisectionHistogram1DFilters(me="PixelPhase1/Tracks/PXBarrel/charge_PXLayer_2"), max_pages=5)
 ```
 
 ### Workspace
 
 Users are automatically routed to a workspace based on e-groups, but it is possible to overwrite this configuration and inspect data from others workspaces:
 
 ```python
-dials = Dials(creds, workspace="jetmet", nthreads=2)
+dials = Dials(creds, workspace="jetmet")
 ```
 
 ## Available endpoints
 
 This package interacts with DIALS api endpoints using underlying classes in `Dials` object.
 
 ### Retrieving a specific object using `get`
 
 ```python
-dials.file_index.get(id=1)
+dials.file_index.get(id=3386119397)
 dials.h1d.get(id=1)
 dials.h2d.get(id=1)
-dials.lumi.get(id=1)
-dials.run.get(id=1)
+dials.lumi.get(dataset_id=14677060, run_number=367094, ls_number=1)
+dials.run.get(dataset_id=14677060, run_number=367094)
 ```
 
 ### Retrieving a list of objects per page using `list`
 
 It is possible to get a list of entries from those endpoint using the `list` and `list_all` methods, the `list` method will fetch only one page and the `list_all` will fetch all available pages:
 
 ```python
@@ -91,14 +91,16 @@
 dials.h2d.list()
 dials.lumi.list()
 dials.run.list()
 ```
 
 ### Retrieving all available pages of a list of objects using `list_all`
 
+Note: Keep in mind that running `list_all` without any filter can take too much time, since you will be retrieving all rows in the database.
+
 ```python
 dials.file_index.list_all()
 dials.h1d.list_all()
 dials.h2d.list_all()
 dials.lumi.list_all()
 dials.run.list_all()
 ```
@@ -118,24 +120,23 @@
     FileIndexFilters,
     LumisectionHistogram1DFilters,
     LumisectionHistogram2DFilters,
     LumisectionFilters,
     RunFilters
 )
 
+dials.file_index.list(FileIndexFilters(dataset__regex="2024B"))
 
-dials.file_index.list(FileIndexFilters(page="10"))
-
-dials.h1d.list(LumisectionHistogram1DFilters(title="PixelPhase1/Tracks/PXBarrel/charge_PXLayer_2", page="15"))
+dials.h1d.list(LumisectionHistogram1DFilters(me="PixelPhase1/Tracks/PXBarrel/charge_PXLayer_2"))
 
-dials.h2d.list_all(LumisectionHistogram2DFilters(title_contains="EEOT digi occupancy EE +", min_entries=100, min_run_number=360392, max_run_number=365000), max_pages=5)
+dials.h2d.list_all(LumisectionHistogram2DFilters(me__regex="PXBarrel", ls_number=78, entries__gte=100), max_pages=5)
 
 dials.lumi.list_all(LumisectionFilters(run_number=360392), max_pages=5)
 
-dials.run.list_all(RunFilters(min_run_number=360392, max_run_number=365000), max_pages=5)
+dials.run.list_all(RunFilters(run_number__gte=360392, run_number__lte=365000), max_pages=5)
 ```
 
 ### Dials MEs
 
 It is possible to inspect the list of selected MEs considered in DIALS during ETL requesting the endpoint `configured-mes` trough the method:
 
 ```python
@@ -153,11 +154,11 @@
 from cmsdials.filters import LumisectionHistogram2DFilters
 
 DEV_URL = "http://localhost:8000/"
 DEV_CACHE_DIR = ".cache-dev"
 
 auth = AuthClient(base_url=DEV_URL)
 creds = Credentials.from_creds_file(cache_dir=DEV_CACHE_DIR, client=auth)  # Make sure to specify the auth client with overwritten values, using another cache_dir is recommended
-dials = Dials(creds, nthreads=2, base_url=DEV_URL)
+dials = Dials(creds, base_url=DEV_URL)
 
-dials.h2d.list_all(LumisectionHistogram2DFilters(title_contains="EEOT digi occupancy EE +", min_entries=100, min_run_number=360392, max_run_number=365000), max_pages=5)
+dials.h2d.list_all(LumisectionHistogram2DFilters(me__regex="EEOT digi occupancy EE +", entries__gte=100, run_number__gte=360392, run_number__lte=365000), max_pages=5)
 ```
```

### Comparing `cmsdials-0.4.0/cmsdials/auth/_base.py` & `cmsdials-1.0.0/cmsdials/auth/_base.py`

 * *Files identical despite different names*

### Comparing `cmsdials-0.4.0/cmsdials/auth/bearer.py` & `cmsdials-1.0.0/cmsdials/auth/bearer.py`

 * *Files identical despite different names*

### Comparing `cmsdials-0.4.0/cmsdials/auth/client.py` & `cmsdials-1.0.0/cmsdials/auth/client.py`

 * *Files identical despite different names*

### Comparing `cmsdials-0.4.0/cmsdials/auth/secret_key.py` & `cmsdials-1.0.0/cmsdials/auth/secret_key.py`

 * *Files identical despite different names*

### Comparing `cmsdials-0.4.0/cmsdials/clients/file_index/models.py` & `cmsdials-1.0.0/cmsdials/clients/file_index/models.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,34 +3,33 @@
 
 from pydantic import AnyUrl, BaseModel, Field
 
 from ...utils.base_model import OBaseModel
 
 
 class FileIndex(BaseModel):
+    dataset_id: int
+    dataset: str = Field(..., max_length=255)
     file_id: int
     file_size: int
-    era: str = Field(..., max_length=5)
-    campaign: str = Field(..., max_length=15)
-    primary_dataset: str = Field(..., max_length=50)
     creation_date: datetime
     last_modification_date: datetime
     logical_file_name: str
     status: str = Field(..., max_length=15)
     err_trace: Optional[str] = Field(..., max_length=5000)
 
 
 class PaginatedFileIndexList(BaseModel):
-    count: int
     next: Optional[AnyUrl]
     previous: Optional[AnyUrl]
     results: List[FileIndex]
 
 
 class FileIndexFilters(OBaseModel):
-    page: Optional[str] = None
-    min_size: Optional[int] = None
-    era: Optional[str] = None
-    campaign: Optional[str] = None
-    primary_dataset: Optional[str] = None
+    next_token: Optional[str] = None
+    dataset_id: Optional[int] = None
     logical_file_name: Optional[str] = None
+    logical_file_name__regex: Optional[str] = None
     status: Optional[str] = None
+    min_size: Optional[int] = None
+    dataset: Optional[str] = None
+    dataset__regex: Optional[str] = None
```

### Comparing `cmsdials-0.4.0/cmsdials/clients/h1d/models.py` & `cmsdials-1.0.0/cmsdials/clients/h1d/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,41 +3,47 @@
 from pydantic import AnyUrl, BaseModel, Field
 
 from ...utils.base_model import OBaseModel
 
 
 class LumisectionHistogram1D(BaseModel):
     hist_id: int
+    dataset: str = Field(..., max_length=255)
+    me: str = Field(..., max_length=255)
+    dataset_id: int
     file_id: int
     run_number: int
+    ls_number: int
+    me_id: int
     ls_id: int
-    title: str = Field(..., max_length=220)
     x_min: float
     x_max: float
     x_bin: float
     entries: int
     data: list[float]
 
 
 class PaginatedLumisectionHistogram1DList(BaseModel):
-    count: int
     next: Optional[AnyUrl]
     previous: Optional[AnyUrl]
     results: List[LumisectionHistogram1D]
 
 
 class LumisectionHistogram1DFilters(OBaseModel):
-    page: Optional[str] = None
+    next_token: Optional[str] = None
+    dataset_id: Optional[int] = None
+    file_id: Optional[int] = None
     run_number: Optional[int] = None
+    run_number__lte: Optional[int] = None
+    run_number__gte: Optional[int] = None
     ls_number: Optional[int] = None
+    ls_numbet__lte: Optional[int] = None
+    ls_number__gte: Optional[int] = None
+    me_id: Optional[int] = None
     ls_id: Optional[int] = None
-    title: Optional[str] = None
-    min_run_number: Optional[int] = None
-    max_run_number: Optional[int] = None
-    min_ls_number: Optional[int] = None
-    max_ls_number: Optional[int] = None
-    title_contains: Optional[str] = None
-    min_entries: Optional[int] = None
-    era: Optional[str] = None
-    campaign: Optional[str] = None
-    primary_dataset: Optional[str] = None
-    file_id: Optional[int] = None
+    entries__gte: Optional[int] = None
+    dataset: Optional[str] = None
+    dataset__regex: Optional[str] = None
+    logical_file_name: Optional[str] = None
+    logical_file_name__regex: Optional[str] = None
+    me: Optional[str] = None
+    me__regex: Optional[str] = None
```

### Comparing `cmsdials-0.4.0/cmsdials/clients/h2d/models.py` & `cmsdials-1.0.0/cmsdials/clients/h2d/models.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,44 +3,50 @@
 from pydantic import AnyUrl, BaseModel, Field
 
 from ...utils.base_model import OBaseModel
 
 
 class LumisectionHistogram2D(BaseModel):
     hist_id: int
+    dataset: str = Field(..., max_length=255)
+    me: str = Field(..., max_length=255)
+    dataset_id: int
     file_id: int
     run_number: int
+    ls_number: int
+    me_id: int
     ls_id: int
-    title: str = Field(..., max_length=220)
     x_min: float
     x_max: float
     x_bin: float
     y_min: float
     y_max: float
     y_bin: float
     entries: int
-    data: list[float]
+    data: list[list[float]]
 
 
 class PaginatedLumisectionHistogram2DList(BaseModel):
-    count: int
     next: Optional[AnyUrl]
     previous: Optional[AnyUrl]
     results: list[LumisectionHistogram2D]
 
 
 class LumisectionHistogram2DFilters(OBaseModel):
-    page: Optional[str] = None
+    next_token: Optional[str] = None
+    dataset_id: Optional[int] = None
+    file_id: Optional[int] = None
     run_number: Optional[int] = None
+    run_number__lte: Optional[int] = None
+    run_number__gte: Optional[int] = None
     ls_number: Optional[int] = None
+    ls_numbet__lte: Optional[int] = None
+    ls_number__gte: Optional[int] = None
+    me_id: Optional[int] = None
     ls_id: Optional[int] = None
-    title: Optional[str] = None
-    min_run_number: Optional[int] = None
-    max_run_number: Optional[int] = None
-    min_ls_number: Optional[int] = None
-    max_ls_number: Optional[int] = None
-    title_contains: Optional[str] = None
-    min_entries: Optional[int] = None
-    era: Optional[str] = None
-    campaign: Optional[str] = None
-    primary_dataset: Optional[str] = None
-    file_id: Optional[int] = None
+    entries__gte: Optional[int] = None
+    dataset: Optional[str] = None
+    dataset__regex: Optional[str] = None
+    logical_file_name: Optional[str] = None
+    logical_file_name__regex: Optional[str] = None
+    me: Optional[str] = None
+    me__regex: Optional[str] = None
```

### Comparing `cmsdials-0.4.0/cmsdials/clients/lumisection/models.py` & `cmsdials-1.0.0/cmsdials/clients/lumisection/models.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 from typing import Optional
 
-from pydantic import AnyUrl, BaseModel
+from pydantic import AnyUrl, BaseModel, Field
 
 from ...utils.base_model import OBaseModel
 
 
 class Lumisection(BaseModel):
-    ls_id: int
+    dataset_id: int
+    dataset: str = Field(..., max_length=255)
+    run_number: int
     ls_number: int
+    ls_id: int
     th1_count: int
     th2_count: int
 
 
 class PaginatedLumisectionList(BaseModel):
-    count: int
     next: Optional[AnyUrl]
     previous: Optional[AnyUrl]
     results: list[Lumisection]
 
 
 class LumisectionFilters(OBaseModel):
-    page: Optional[str] = None
+    next_token: Optional[str] = None
+    dataset_id: Optional[int] = None
     run_number: Optional[int] = None
+    run_number__lte: Optional[int] = None
+    run_number__gte: Optional[int] = None
     ls_number: Optional[int] = None
-    min_ls_number: Optional[int] = None
-    max_ls_number: Optional[int] = None
-    min_run_number: Optional[int] = None
-    max_run_number: Optional[int] = None
+    ls_number__lte: Optional[int] = None
+    ls_number__gte: Optional[int] = None
+    dataset: Optional[str] = None
+    dataset__regex: Optional[str] = None
```

### Comparing `cmsdials-0.4.0/cmsdials/cmsdials.py` & `cmsdials-1.0.0/cmsdials/cmsdials.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,13 @@
 from .clients.h1d.client import LumisectionHistogram1DClient
 from .clients.h2d.client import LumisectionHistogram2DClient
 from .clients.lumisection.client import LumisectionClient
 from .clients.run.client import RunClient
 
 
 class Dials:
-    def __init__(
-        self, creds: BaseCredentials, workspace: Optional[str] = None, nthreads: Optional[int] = None, *args, **kwargs
-    ) -> None:
-        self.file_index = FileIndexClient(creds, workspace, nthreads, *args, **kwargs)
-        self.h1d = LumisectionHistogram1DClient(creds, workspace, nthreads, *args, **kwargs)
-        self.h2d = LumisectionHistogram2DClient(creds, workspace, nthreads, *args, **kwargs)
-        self.lumi = LumisectionClient(creds, workspace, nthreads, *args, **kwargs)
-        self.run = RunClient(creds, workspace, nthreads, *args, **kwargs)
+    def __init__(self, creds: BaseCredentials, workspace: Optional[str] = None, *args, **kwargs) -> None:
+        self.file_index = FileIndexClient(creds, workspace, *args, **kwargs)
+        self.h1d = LumisectionHistogram1DClient(creds, workspace, *args, **kwargs)
+        self.h2d = LumisectionHistogram2DClient(creds, workspace, *args, **kwargs)
+        self.lumi = LumisectionClient(creds, workspace, *args, **kwargs)
+        self.run = RunClient(creds, workspace, *args, **kwargs)
```

### Comparing `cmsdials-0.4.0/cmsdials/utils/_json.py` & `cmsdials-1.0.0/cmsdials/utils/_json.py`

 * *Files identical despite different names*

### Comparing `cmsdials-0.4.0/cmsdials/utils/api_client.py` & `cmsdials-1.0.0/cmsdials/utils/api_client.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-from concurrent.futures import ThreadPoolExecutor
-from math import ceil
 from typing import Optional
+from urllib.parse import parse_qs, urlparse
 
 import requests
 from requests.exceptions import HTTPError
 
 from ..auth._base import BaseCredentials
 from ..utils.logger import logger
 
@@ -38,104 +37,73 @@
     filter_class = None
     lookup_url = None
 
     def __init__(
         self,
         creds: BaseCredentials,
         workspace: Optional[str] = None,
-        nthreads: Optional[int] = None,
         *args: str,
         **kwargs: str,
     ) -> None:
         super().__init__(*args, **kwargs)
         self.creds = creds
         self.workspace = workspace
-        self.nthreads = nthreads or 1
 
-    def __build_headers(self) -> dict:
+    def _build_headers(self) -> dict:
         base = {"accept": "application/json"}
         if self.workspace is not None:
             base["Workspace"] = self.workspace
         self.creds.before_request(base)
         return base
 
-    def get(self, id: str):
+    def get(self, id: int):
         endpoint_url = self.api_url + self.lookup_url + str(id) + "/"
-        headers = self.__build_headers()
+        headers = self._build_headers()
         response = requests.get(endpoint_url, headers=headers)
 
         try:
             response.raise_for_status()
         except HTTPError as err:
             logger.info(f"Api raw response: {response.text}")
             raise err
 
         response = response.json()
         return self.data_model(**response)
 
     def list(self, filters=None):
         filters = filters or self.filter_class()
         endpoint_url = self.api_url + self.lookup_url
-        headers = self.__build_headers()
+        headers = self._build_headers()
         response = requests.get(endpoint_url, headers=headers, params=filters.cleandict())
 
         try:
             response.raise_for_status()
         except HTTPError as err:
             logger.info(f"Api raw response: {response.text}")
             raise err
 
         response = response.json()
         return self.pagination_model(**response)
 
     def __list_sync(self, filters, max_pages: Optional[int] = None):
-        page = 1
+        next_token = None
         results = []
         is_last_page = False
+        total_pages = 0
 
         while is_last_page is False:
             curr_filters = self.filter_class(**filters.dict())
-            curr_filters.page = str(page)
+            curr_filters.next_token = next_token
             response = self.list(curr_filters)
             results.extend(response.results)
             is_last_page = response.next is None
-            page += 1
-            if max_pages and page > max_pages:
+            next_token = parse_qs(urlparse(response.next).query).get("next_token") if response.next else None
+            total_pages += 1
+            if max_pages and total_pages > max_pages:
                 break
 
         return self.pagination_model(
-            count=response.count, next=None, previous=None, results=results  # No problem re-using last response count
+            next=None, previous=None, results=results  # No problem re-using last response count
         )
 
-    def __list_multithreaded(self, filters, max_pages: Optional[int] = None):
-        results = []
-
-        # Request the first page to compute number of pages
-        curr_filters = self.filter_class(**filters.dict())
-        curr_filters.page = "1"
-        response = self.list(curr_filters)
-        results.extend(response.results)
-        count = response.count
-        n_pages = ceil(response.count / 10)
-        n_pages = max_pages if max_pages is not None and n_pages > max_pages else n_pages
-
-        # If there isn't another page, just return current results
-        if response.next is None:
-            return response
-
-        # Request other pages
-        all_filters = [{**filters.dict(), "page": str(page)} for page in range(2, n_pages + 1)]
-        all_filters = [self.filter_class(**filter) for filter in all_filters]
-        with ThreadPoolExecutor(max_workers=self.nthreads) as executor:
-            jobs = executor.map(self.list, all_filters)
-            del all_filters
-            [results.extend(job_result.results) for job_result in jobs]
-            del jobs
-
-        return self.pagination_model(count=count, next=None, previous=None, results=results)
-
     def list_all(self, filters, max_pages: Optional[int] = None):
-        return (
-            self.__list_sync(filters, max_pages)
-            if self.nthreads is None
-            else self.__list_multithreaded(filters, max_pages)
-        )
+        return self.__list_sync(filters, max_pages)
```

### Comparing `cmsdials-0.4.0/PKG-INFO` & `cmsdials-1.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: cmsdials
-Version: 0.4.0
+Version: 1.0.0
 Summary: The Python api client interface to DIALS service
 Home-page: https://github.com/cms-DQM/dials-py
 Author: Gabriel Moreira
 Author-email: gabrielmscampos@gmail.com
 Requires-Python: >=3.9,<4.0
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -72,40 +72,40 @@
 
 ```python
 from cmsdials.auth.bearer import Credentials
 from cmsdials import Dials
 from cmsdials.filters import LumisectionHistogram1DFilters
 
 creds = Credentials.from_creds_file()
-dials = Dials(creds, nthreads=2)
+dials = Dials(creds)
 
 # Getting h1d data
-data = dials.h1d.list_all(LumisectionHistogram1DFilters(title="PixelPhase1/Tracks/PXBarrel/charge_PXLayer_2"), max_pages=5)
+data = dials.h1d.list_all(LumisectionHistogram1DFilters(me="PixelPhase1/Tracks/PXBarrel/charge_PXLayer_2"), max_pages=5)
 ```
 
 ### Workspace
 
 Users are automatically routed to a workspace based on e-groups, but it is possible to overwrite this configuration and inspect data from others workspaces:
 
 ```python
-dials = Dials(creds, workspace="jetmet", nthreads=2)
+dials = Dials(creds, workspace="jetmet")
 ```
 
 ## Available endpoints
 
 This package interacts with DIALS api endpoints using underlying classes in `Dials` object.
 
 ### Retrieving a specific object using `get`
 
 ```python
-dials.file_index.get(id=1)
+dials.file_index.get(id=3386119397)
 dials.h1d.get(id=1)
 dials.h2d.get(id=1)
-dials.lumi.get(id=1)
-dials.run.get(id=1)
+dials.lumi.get(dataset_id=14677060, run_number=367094, ls_number=1)
+dials.run.get(dataset_id=14677060, run_number=367094)
 ```
 
 ### Retrieving a list of objects per page using `list`
 
 It is possible to get a list of entries from those endpoint using the `list` and `list_all` methods, the `list` method will fetch only one page and the `list_all` will fetch all available pages:
 
 ```python
@@ -114,14 +114,16 @@
 dials.h2d.list()
 dials.lumi.list()
 dials.run.list()
 ```
 
 ### Retrieving all available pages of a list of objects using `list_all`
 
+Note: Keep in mind that running `list_all` without any filter can take too much time, since you will be retrieving all rows in the database.
+
 ```python
 dials.file_index.list_all()
 dials.h1d.list_all()
 dials.h2d.list_all()
 dials.lumi.list_all()
 dials.run.list_all()
 ```
@@ -141,24 +143,23 @@
     FileIndexFilters,
     LumisectionHistogram1DFilters,
     LumisectionHistogram2DFilters,
     LumisectionFilters,
     RunFilters
 )
 
+dials.file_index.list(FileIndexFilters(dataset__regex="2024B"))
 
-dials.file_index.list(FileIndexFilters(page="10"))
-
-dials.h1d.list(LumisectionHistogram1DFilters(title="PixelPhase1/Tracks/PXBarrel/charge_PXLayer_2", page="15"))
+dials.h1d.list(LumisectionHistogram1DFilters(me="PixelPhase1/Tracks/PXBarrel/charge_PXLayer_2"))
 
-dials.h2d.list_all(LumisectionHistogram2DFilters(title_contains="EEOT digi occupancy EE +", min_entries=100, min_run_number=360392, max_run_number=365000), max_pages=5)
+dials.h2d.list_all(LumisectionHistogram2DFilters(me__regex="PXBarrel", ls_number=78, entries__gte=100), max_pages=5)
 
 dials.lumi.list_all(LumisectionFilters(run_number=360392), max_pages=5)
 
-dials.run.list_all(RunFilters(min_run_number=360392, max_run_number=365000), max_pages=5)
+dials.run.list_all(RunFilters(run_number__gte=360392, run_number__lte=365000), max_pages=5)
 ```
 
 ### Dials MEs
 
 It is possible to inspect the list of selected MEs considered in DIALS during ETL requesting the endpoint `configured-mes` trough the method:
 
 ```python
@@ -176,12 +177,12 @@
 from cmsdials.filters import LumisectionHistogram2DFilters
 
 DEV_URL = "http://localhost:8000/"
 DEV_CACHE_DIR = ".cache-dev"
 
 auth = AuthClient(base_url=DEV_URL)
 creds = Credentials.from_creds_file(cache_dir=DEV_CACHE_DIR, client=auth)  # Make sure to specify the auth client with overwritten values, using another cache_dir is recommended
-dials = Dials(creds, nthreads=2, base_url=DEV_URL)
+dials = Dials(creds, base_url=DEV_URL)
 
-dials.h2d.list_all(LumisectionHistogram2DFilters(title_contains="EEOT digi occupancy EE +", min_entries=100, min_run_number=360392, max_run_number=365000), max_pages=5)
+dials.h2d.list_all(LumisectionHistogram2DFilters(me__regex="EEOT digi occupancy EE +", entries__gte=100, run_number__gte=360392, run_number__lte=365000), max_pages=5)
 ```
```

