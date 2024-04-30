# Comparing `tmp/cmsdials-1.0.0.tar.gz` & `tmp/cmsdials-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmsdials-1.0.0.tar", max compression
+gzip compressed data, was "cmsdials-1.0.1.tar", max compression
```

## Comparing `cmsdials-1.0.0.tar` & `cmsdials-1.0.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0    35149 2024-04-28 10:36:23.872227 cmsdials-1.0.0/LICENSE
--rw-r--r--   0        0        0     5484 2024-04-29 19:09:44.714827 cmsdials-1.0.0/README.md
--rw-r--r--   0        0        0       49 2024-04-28 10:36:23.872227 cmsdials-1.0.0/cmsdials/__init__.py
--rw-r--r--   0        0        0        0 2024-04-28 10:36:23.872227 cmsdials-1.0.0/cmsdials/auth/__init__.py
--rw-r--r--   0        0        0     4136 2024-04-28 10:36:23.873227 cmsdials-1.0.0/cmsdials/auth/_base.py
--rw-r--r--   0        0        0     4998 2024-04-28 10:36:23.873227 cmsdials-1.0.0/cmsdials/auth/bearer.py
--rw-r--r--   0        0        0     3491 2024-04-28 10:36:23.873227 cmsdials-1.0.0/cmsdials/auth/client.py
--rw-r--r--   0        0        0      107 2024-04-28 10:36:23.873227 cmsdials-1.0.0/cmsdials/auth/exceptions.py
--rw-r--r--   0        0        0      425 2024-04-28 10:36:23.874227 cmsdials-1.0.0/cmsdials/auth/models.py
--rw-r--r--   0        0        0     1041 2024-04-28 10:36:23.874227 cmsdials-1.0.0/cmsdials/auth/secret_key.py
--rw-r--r--   0        0        0        0 2024-04-28 10:36:23.874227 cmsdials-1.0.0/cmsdials/clients/__init__.py
--rw-r--r--   0        0        0        0 2024-04-28 10:36:23.874227 cmsdials-1.0.0/cmsdials/clients/file_index/__init__.py
--rw-r--r--   0        0        0      318 2024-04-28 10:36:23.874227 cmsdials-1.0.0/cmsdials/clients/file_index/client.py
--rw-r--r--   0        0        0      962 2024-04-29 19:06:30.058424 cmsdials-1.0.0/cmsdials/clients/file_index/models.py
--rw-r--r--   0        0        0        0 2024-04-28 10:36:23.875227 cmsdials-1.0.0/cmsdials/clients/h1d/__init__.py
--rw-r--r--   0        0        0      402 2024-04-29 11:53:55.385012 cmsdials-1.0.0/cmsdials/clients/h1d/client.py
--rw-r--r--   0        0        0     1360 2024-04-29 19:06:46.571391 cmsdials-1.0.0/cmsdials/clients/h1d/models.py
--rw-r--r--   0        0        0        0 2024-04-28 10:36:23.875227 cmsdials-1.0.0/cmsdials/clients/h2d/__init__.py
--rw-r--r--   0        0        0      402 2024-04-29 11:53:59.860011 cmsdials-1.0.0/cmsdials/clients/h2d/client.py
--rw-r--r--   0        0        0     1411 2024-04-29 19:06:54.307376 cmsdials-1.0.0/cmsdials/clients/h2d/models.py
--rw-r--r--   0        0        0        0 2024-04-28 10:36:23.877227 cmsdials-1.0.0/cmsdials/clients/lumisection/__init__.py
--rw-r--r--   0        0        0      946 2024-04-29 13:18:14.360705 cmsdials-1.0.0/cmsdials/clients/lumisection/client.py
--rw-r--r--   0        0        0      871 2024-04-29 19:07:02.068360 cmsdials-1.0.0/cmsdials/clients/lumisection/models.py
--rw-r--r--   0        0        0        0 2024-04-28 10:36:23.877227 cmsdials-1.0.0/cmsdials/clients/run/__init__.py
--rw-r--r--   0        0        0      854 2024-04-29 13:18:14.362705 cmsdials-1.0.0/cmsdials/clients/run/client.py
--rw-r--r--   0        0        0      667 2024-04-29 19:07:09.219346 cmsdials-1.0.0/cmsdials/clients/run/models.py
--rw-r--r--   0        0        0      847 2024-04-29 19:13:59.398882 cmsdials-1.0.0/cmsdials/cmsdials.py
--rw-r--r--   0        0        0      439 2024-04-28 10:36:23.878227 cmsdials-1.0.0/cmsdials/filters.py
--rw-r--r--   0        0        0        0 2024-04-28 10:36:23.878227 cmsdials-1.0.0/cmsdials/utils/__init__.py
--rw-r--r--   0        0        0      671 2024-04-28 10:36:23.878227 cmsdials-1.0.0/cmsdials/utils/_json.py
--rw-r--r--   0        0        0     3557 2024-04-29 19:13:59.688881 cmsdials-1.0.0/cmsdials/utils/api_client.py
--rw-r--r--   0        0        0      174 2024-04-28 10:36:23.878227 cmsdials-1.0.0/cmsdials/utils/base_model.py
--rw-r--r--   0        0        0      145 2024-04-28 10:36:23.878227 cmsdials-1.0.0/cmsdials/utils/logger.py
--rw-r--r--   0        0        0     2720 2024-04-30 23:36:22.164299 cmsdials-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     6431 1970-01-01 00:00:00.000000 cmsdials-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-28 10:36:23.872227 cmsdials-1.0.1/LICENSE
+-rw-r--r--   0        0        0     5484 2024-04-29 19:09:44.714827 cmsdials-1.0.1/README.md
+-rw-r--r--   0        0        0       49 2024-04-28 10:36:23.872227 cmsdials-1.0.1/cmsdials/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 10:36:23.872227 cmsdials-1.0.1/cmsdials/auth/__init__.py
+-rw-r--r--   0        0        0     4136 2024-04-28 10:36:23.873227 cmsdials-1.0.1/cmsdials/auth/_base.py
+-rw-r--r--   0        0        0     4998 2024-04-28 10:36:23.873227 cmsdials-1.0.1/cmsdials/auth/bearer.py
+-rw-r--r--   0        0        0     3491 2024-04-28 10:36:23.873227 cmsdials-1.0.1/cmsdials/auth/client.py
+-rw-r--r--   0        0        0      107 2024-04-28 10:36:23.873227 cmsdials-1.0.1/cmsdials/auth/exceptions.py
+-rw-r--r--   0        0        0      425 2024-04-28 10:36:23.874227 cmsdials-1.0.1/cmsdials/auth/models.py
+-rw-r--r--   0        0        0     1041 2024-04-28 10:36:23.874227 cmsdials-1.0.1/cmsdials/auth/secret_key.py
+-rw-r--r--   0        0        0        0 2024-04-28 10:36:23.874227 cmsdials-1.0.1/cmsdials/clients/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 10:36:23.874227 cmsdials-1.0.1/cmsdials/clients/file_index/__init__.py
+-rw-r--r--   0        0        0      318 2024-04-28 10:36:23.874227 cmsdials-1.0.1/cmsdials/clients/file_index/client.py
+-rw-r--r--   0        0        0      962 2024-04-29 19:06:30.058424 cmsdials-1.0.1/cmsdials/clients/file_index/models.py
+-rw-r--r--   0        0        0        0 2024-04-28 10:36:23.875227 cmsdials-1.0.1/cmsdials/clients/h1d/__init__.py
+-rw-r--r--   0        0        0      402 2024-04-29 11:53:55.385012 cmsdials-1.0.1/cmsdials/clients/h1d/client.py
+-rw-r--r--   0        0        0     1313 2024-04-30 23:50:22.265289 cmsdials-1.0.1/cmsdials/clients/h1d/models.py
+-rw-r--r--   0        0        0        0 2024-04-28 10:36:23.875227 cmsdials-1.0.1/cmsdials/clients/h2d/__init__.py
+-rw-r--r--   0        0        0      402 2024-04-29 11:53:59.860011 cmsdials-1.0.1/cmsdials/clients/h2d/client.py
+-rw-r--r--   0        0        0     1364 2024-04-30 23:50:22.265289 cmsdials-1.0.1/cmsdials/clients/h2d/models.py
+-rw-r--r--   0        0        0        0 2024-04-28 10:36:23.877227 cmsdials-1.0.1/cmsdials/clients/lumisection/__init__.py
+-rw-r--r--   0        0        0      946 2024-04-29 13:18:14.360705 cmsdials-1.0.1/cmsdials/clients/lumisection/client.py
+-rw-r--r--   0        0        0      856 2024-04-30 23:50:22.265289 cmsdials-1.0.1/cmsdials/clients/lumisection/models.py
+-rw-r--r--   0        0        0        0 2024-04-28 10:36:23.877227 cmsdials-1.0.1/cmsdials/clients/run/__init__.py
+-rw-r--r--   0        0        0      854 2024-04-29 13:18:14.362705 cmsdials-1.0.1/cmsdials/clients/run/client.py
+-rw-r--r--   0        0        0      667 2024-04-29 19:07:09.219346 cmsdials-1.0.1/cmsdials/clients/run/models.py
+-rw-r--r--   0        0        0      847 2024-04-29 19:13:59.398882 cmsdials-1.0.1/cmsdials/cmsdials.py
+-rw-r--r--   0        0        0      439 2024-04-28 10:36:23.878227 cmsdials-1.0.1/cmsdials/filters.py
+-rw-r--r--   0        0        0        0 2024-04-28 10:36:23.878227 cmsdials-1.0.1/cmsdials/utils/__init__.py
+-rw-r--r--   0        0        0      671 2024-04-28 10:36:23.878227 cmsdials-1.0.1/cmsdials/utils/_json.py
+-rw-r--r--   0        0        0     3557 2024-04-29 19:13:59.688881 cmsdials-1.0.1/cmsdials/utils/api_client.py
+-rw-r--r--   0        0        0      174 2024-04-28 10:36:23.878227 cmsdials-1.0.1/cmsdials/utils/base_model.py
+-rw-r--r--   0        0        0      145 2024-04-28 10:36:23.878227 cmsdials-1.0.1/cmsdials/utils/logger.py
+-rw-r--r--   0        0        0     2720 2024-04-30 23:50:22.265289 cmsdials-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     6431 1970-01-01 00:00:00.000000 cmsdials-1.0.1/PKG-INFO
```

### Comparing `cmsdials-1.0.0/LICENSE` & `cmsdials-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cmsdials-1.0.0/README.md` & `cmsdials-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `cmsdials-1.0.0/cmsdials/auth/_base.py` & `cmsdials-1.0.1/cmsdials/auth/_base.py`

 * *Files identical despite different names*

### Comparing `cmsdials-1.0.0/cmsdials/auth/bearer.py` & `cmsdials-1.0.1/cmsdials/auth/bearer.py`

 * *Files identical despite different names*

### Comparing `cmsdials-1.0.0/cmsdials/auth/client.py` & `cmsdials-1.0.1/cmsdials/auth/client.py`

 * *Files identical despite different names*

### Comparing `cmsdials-1.0.0/cmsdials/auth/secret_key.py` & `cmsdials-1.0.1/cmsdials/auth/secret_key.py`

 * *Files identical despite different names*

### Comparing `cmsdials-1.0.0/cmsdials/clients/file_index/models.py` & `cmsdials-1.0.1/cmsdials/clients/file_index/models.py`

 * *Files identical despite different names*

### Comparing `cmsdials-1.0.0/cmsdials/clients/h1d/models.py` & `cmsdials-1.0.1/cmsdials/clients/h1d/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,14 @@
     dataset: str = Field(..., max_length=255)
     me: str = Field(..., max_length=255)
     dataset_id: int
     file_id: int
     run_number: int
     ls_number: int
     me_id: int
-    ls_id: int
     x_min: float
     x_max: float
     x_bin: float
     entries: int
     data: list[float]
 
 
@@ -35,15 +34,14 @@
     run_number: Optional[int] = None
     run_number__lte: Optional[int] = None
     run_number__gte: Optional[int] = None
     ls_number: Optional[int] = None
     ls_numbet__lte: Optional[int] = None
     ls_number__gte: Optional[int] = None
     me_id: Optional[int] = None
-    ls_id: Optional[int] = None
     entries__gte: Optional[int] = None
     dataset: Optional[str] = None
     dataset__regex: Optional[str] = None
     logical_file_name: Optional[str] = None
     logical_file_name__regex: Optional[str] = None
     me: Optional[str] = None
     me__regex: Optional[str] = None
```

### Comparing `cmsdials-1.0.0/cmsdials/clients/h2d/models.py` & `cmsdials-1.0.1/cmsdials/clients/h2d/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,14 @@
     dataset: str = Field(..., max_length=255)
     me: str = Field(..., max_length=255)
     dataset_id: int
     file_id: int
     run_number: int
     ls_number: int
     me_id: int
-    ls_id: int
     x_min: float
     x_max: float
     x_bin: float
     y_min: float
     y_max: float
     y_bin: float
     entries: int
@@ -38,15 +37,14 @@
     run_number: Optional[int] = None
     run_number__lte: Optional[int] = None
     run_number__gte: Optional[int] = None
     ls_number: Optional[int] = None
     ls_numbet__lte: Optional[int] = None
     ls_number__gte: Optional[int] = None
     me_id: Optional[int] = None
-    ls_id: Optional[int] = None
     entries__gte: Optional[int] = None
     dataset: Optional[str] = None
     dataset__regex: Optional[str] = None
     logical_file_name: Optional[str] = None
     logical_file_name__regex: Optional[str] = None
     me: Optional[str] = None
     me__regex: Optional[str] = None
```

### Comparing `cmsdials-1.0.0/cmsdials/clients/lumisection/client.py` & `cmsdials-1.0.1/cmsdials/clients/lumisection/client.py`

 * *Files identical despite different names*

### Comparing `cmsdials-1.0.0/cmsdials/clients/lumisection/models.py` & `cmsdials-1.0.1/cmsdials/clients/lumisection/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 
 class Lumisection(BaseModel):
     dataset_id: int
     dataset: str = Field(..., max_length=255)
     run_number: int
     ls_number: int
-    ls_id: int
     th1_count: int
     th2_count: int
 
 
 class PaginatedLumisectionList(BaseModel):
     next: Optional[AnyUrl]
     previous: Optional[AnyUrl]
```

### Comparing `cmsdials-1.0.0/cmsdials/clients/run/client.py` & `cmsdials-1.0.1/cmsdials/clients/run/client.py`

 * *Files identical despite different names*

### Comparing `cmsdials-1.0.0/cmsdials/clients/run/models.py` & `cmsdials-1.0.1/cmsdials/clients/run/models.py`

 * *Files identical despite different names*

### Comparing `cmsdials-1.0.0/cmsdials/cmsdials.py` & `cmsdials-1.0.1/cmsdials/cmsdials.py`

 * *Files identical despite different names*

### Comparing `cmsdials-1.0.0/cmsdials/utils/_json.py` & `cmsdials-1.0.1/cmsdials/utils/_json.py`

 * *Files identical despite different names*

### Comparing `cmsdials-1.0.0/cmsdials/utils/api_client.py` & `cmsdials-1.0.1/cmsdials/utils/api_client.py`

 * *Files identical despite different names*

### Comparing `cmsdials-1.0.0/pyproject.toml` & `cmsdials-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cmsdials"
-version = "1.0.0"
+version = "1.0.1"
 description = "The Python api client interface to DIALS service"
 authors = ["Gabriel Moreira <gabrielmscampos@gmail.com>"]
 readme = "README.md"
 include = ["LICENSE"]
 repository = "https://github.com/cms-DQM/dials-py"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `cmsdials-1.0.0/PKG-INFO` & `cmsdials-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmsdials
-Version: 1.0.0
+Version: 1.0.1
 Summary: The Python api client interface to DIALS service
 Home-page: https://github.com/cms-DQM/dials-py
 Author: Gabriel Moreira
 Author-email: gabrielmscampos@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
```

