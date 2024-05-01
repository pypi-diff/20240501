# Comparing `tmp/harmony-py-0.4.9.tar.gz` & `tmp/harmony_py-1756b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harmony-py-0.4.9.tar", last modified: Tue Jun  6 17:06:23 2023, max compression
+gzip compressed data, was "harmony_py-1756b0.tar", last modified: Wed May  1 18:06:52 2024, max compression
```

## Comparing `harmony-py-0.4.9.tar` & `harmony_py-1756b0.tar`

### file list

```diff
@@ -1,26 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:06:23.718888 harmony-py-0.4.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-06 17:05:22.000000 harmony-py-0.4.9/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     9772 2023-06-06 17:05:22.000000 harmony-py-0.4.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-06 17:05:22.000000 harmony-py-0.4.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-06-06 17:06:23.718888 harmony-py-0.4.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-06-06 17:05:22.000000 harmony-py-0.4.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:06:23.714888 harmony-py-0.4.9/harmony/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-06 17:06:16.000000 harmony-py-0.4.9/harmony/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-06-06 17:05:22.000000 harmony-py-0.4.9/harmony/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-06-06 17:05:22.000000 harmony-py-0.4.9/harmony/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    51525 2023-06-06 17:05:22.000000 harmony-py-0.4.9/harmony/harmony.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-06 17:05:22.000000 harmony-py-0.4.9/harmony/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:06:23.718888 harmony-py-0.4.9/harmony_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-06-06 17:06:23.000000 harmony-py-0.4.9/harmony_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-06 17:06:23.000000 harmony-py-0.4.9/harmony_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 17:06:23.000000 harmony-py-0.4.9/harmony_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-06 17:06:23.000000 harmony-py-0.4.9/harmony_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-06 17:06:23.000000 harmony-py-0.4.9/harmony_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-06 17:06:23.718888 harmony-py-0.4.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-06-06 17:05:22.000000 harmony-py-0.4.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:06:23.718888 harmony-py-0.4.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-06-06 17:05:22.000000 harmony-py-0.4.9/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    49438 2023-06-06 17:05:22.000000 harmony-py-0.4.9/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-06-06 17:05:22.000000 harmony-py-0.4.9/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-06-06 17:05:22.000000 harmony-py-0.4.9/tests/test_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-06 17:05:22.000000 harmony-py-0.4.9/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:06:52.731970 harmony_py-1756b0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-01 18:06:16.000000 harmony_py-1756b0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9772 2024-05-01 18:06:16.000000 harmony_py-1756b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-01 18:06:16.000000 harmony_py-1756b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-05-01 18:06:52.731970 harmony_py-1756b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4590 2024-05-01 18:06:16.000000 harmony_py-1756b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:06:52.727970 harmony_py-1756b0/harmony/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-01 18:06:47.000000 harmony_py-1756b0/harmony/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5916 2024-05-01 18:06:16.000000 harmony_py-1756b0/harmony/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-05-01 18:06:16.000000 harmony_py-1756b0/harmony/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57965 2024-05-01 18:06:16.000000 harmony_py-1756b0/harmony/harmony.py
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-01 18:06:16.000000 harmony_py-1756b0/harmony/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:06:52.731970 harmony_py-1756b0/harmony_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-05-01 18:06:52.000000 harmony_py-1756b0/harmony_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-01 18:06:52.000000 harmony_py-1756b0/harmony_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 18:06:52.000000 harmony_py-1756b0/harmony_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-01 18:06:52.000000 harmony_py-1756b0/harmony_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-01 18:06:52.000000 harmony_py-1756b0/harmony_py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:06:52.731970 harmony_py-1756b0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-01 18:06:16.000000 harmony_py-1756b0/requirements/core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-01 18:06:16.000000 harmony_py-1756b0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-01 18:06:16.000000 harmony_py-1756b0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-01 18:06:16.000000 harmony_py-1756b0/requirements/examples.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-01 18:06:52.731970 harmony_py-1756b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-01 18:06:16.000000 harmony_py-1756b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:06:52.731970 harmony_py-1756b0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-05-01 18:06:16.000000 harmony_py-1756b0/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59975 2024-05-01 18:06:16.000000 harmony_py-1756b0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-01 18:06:16.000000 harmony_py-1756b0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8911 2024-05-01 18:06:16.000000 harmony_py-1756b0/tests/test_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-01 18:06:16.000000 harmony_py-1756b0/tests/test_util.py
```

### Comparing `harmony-py-0.4.9/CONTRIBUTING.md` & `harmony_py-1756b0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `harmony-py-0.4.9/LICENSE` & `harmony_py-1756b0/LICENSE`

 * *Files identical despite different names*

### Comparing `harmony-py-0.4.9/PKG-INFO` & `harmony_py-1756b0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,22 @@
-Metadata-Version: 2.1
-Name: harmony-py
-Version: 0.4.9
-Summary: The NASA Harmony Python library
-Home-page: https://github.com/nasa/harmony-py
-Keywords: nasa,harmony,remote-sensing,science,geoscience
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.6, <4
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # harmony-py
 
 [![Documentation Status](https://readthedocs.org/projects/harmony-py/badge/?version=latest)](https://harmony-py.readthedocs.io/en/latest/?badge=latest)
 
 Harmony-Py is a Python library for integrating with NASA's [Harmony](https://harmony.earthdata.nasa.gov/) Services.
 
 Harmony-Py provides a Python alternative to directly using [Harmony's RESTful API](https://harmony.earthdata.nasa.gov/docs/api/). It handles NASA [Earthdata Login (EDL)](https://urs.earthdata.nasa.gov/home) authentication and optionally integrates with the [CMR Python Wrapper](https://github.com/nasa/eo-metadata-tools) by accepting collection results as a request parameter. It's convenient for scientists who wish to use Harmony from Jupyter notebooks as well as machine-to-machine communication with larger Python applications.
 
 We welcome feedback on Harmony-Py via [GitHub Issues](https://github.com/nasa/harmony-py/issues)
 
 # Using Harmony Py
 
 ## Prerequisites
 
-* Python 3.7+
+* Python 3.8+
 
 
 ## Installing
 
 The library is available from [PyPI](https://pypi.org/project/harmony-py/) and can be installed with pip:
 
         $ pip install -U harmony-py
```

### Comparing `harmony-py-0.4.9/harmony/auth.py` & `harmony_py-1756b0/harmony/auth.py`

 * *Files identical despite different names*

### Comparing `harmony-py-0.4.9/harmony/config.py` & `harmony_py-1756b0/harmony/config.py`

 * *Files identical despite different names*

### Comparing `harmony-py-0.4.9/harmony/harmony.py` & `harmony_py-1756b0/harmony/harmony.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,23 +22,24 @@
 from http.client import ResponseNotReady
 import os
 import shutil
 import sys
 from tabnanny import check
 import time
 import platform
+from uuid import UUID
 from requests import Response
 from requests.exceptions import JSONDecodeError
 import requests.models
 from concurrent.futures import Future, ThreadPoolExecutor
 from contextlib import contextmanager
 from datetime import date, datetime
 from enum import Enum
 from typing import Any, ContextManager, IO, Iterator, List, Mapping, NamedTuple, Optional, \
-    Tuple, Generator
+    Tuple, Generator, Union
 
 import curlify
 import dateutil.parser
 import progressbar
 
 from harmony.auth import create_session, validate_auth
 from harmony.config import Config, Environment
@@ -169,28 +170,61 @@
     'kml': 'application/vnd.google-earth.kml+xml',
     'shz': 'application/shapefile+zip',
     'zip': 'application/shapefile+zip',
 }
 _valid_shapefile_exts = ', '.join((_shapefile_exts_to_mimes.keys()))
 
 
-class Request:
+class BaseRequest:
+    """A Harmony base request with the CMR collection. It is the base class of all harmony
+    requests.
+
+    Args:
+        collection: The CMR collection that should be queried
+
+    Returns:
+        A Harmony Request instance
+    """
+
+    def __init__(self,
+                 *,
+                 collection: Collection):
+        self.collection = collection
+        self.variable_name_to_query_param = {}
+
+    def error_messages(self) -> List[str]:
+        return []
+
+    def is_valid(self) -> bool:
+        """Determines if the request and its parameters are valid."""
+        return len(self.error_messages()) == 0
+
+    def parameter_values(self) -> List[Tuple[str, Any]]:
+        """Returns tuples of each query parameter that has been set and its value."""
+        pvs = [(param, getattr(self, variable))
+               for variable, param in self.variable_name_to_query_param.items()]
+        return [(p, v) for p, v in pvs if v is not None]
+
+
+class Request(BaseRequest):
     """A Harmony request with the CMR collection and various parameters expressing
     how the data is to be transformed.
 
     Args:
         collection: The CMR collection that should be queried
 
         spatial: Bounding box spatial constraints on the data
 
         temporal: Date/time constraints on the data provided as a dict mapping "start" and "stop"
           keys to corresponding start/stop datetime.datetime objects
 
         dimensions: A list of dimensions to use for subsetting the data
 
+        extend: A list of dimensions to extend
+
         crs: reproject the output coverage to the given CRS.  Recognizes CRS types that can be
           inferred by gdal, including EPSG codes, Proj4 strings, and OGC URLs
           (http://www.opengis.net/def/crs/...)
 
         interpolation: specify the interpolation method used during reprojection and scaling
 
         scale_extent: scale the resulting coverage either among one axis to a given extent
@@ -224,23 +258,24 @@
         destination_url: Destination URL specified by the client
           (only S3 is supported, e.g. s3://my-bucket-name/mypath)
 
         grid: The name of the output grid to use for regridding requests. The name must
           match the UMM grid name in the CMR.
 
     Returns:
-        A Harmony Request instance
+        A Harmony Transformation Request instance
     """
 
     def __init__(self,
                  collection: Collection,
                  *,
                  spatial: BBox = None,
                  temporal: Mapping[str, datetime] = None,
                  dimensions: List[Dimension] = None,
+                 extend: List[str] = None,
                  crs: str = None,
                  destination_url: str = None,
                  format: str = None,
                  granule_id: List[str] = None,
                  granule_name: List[str] = None,
                  height: int = None,
                  interpolation: str = None,
@@ -252,18 +287,19 @@
                  width: int = None,
                  concatenate: bool = None,
                  skip_preview: bool = None,
                  ignore_errors: bool = None,
                  grid: str = None):
         """Creates a new Request instance from all specified criteria.'
         """
-        self.collection = collection
+        super().__init__(collection=collection)
         self.spatial = spatial
         self.temporal = temporal
         self.dimensions = dimensions
+        self.extend = extend
         self.crs = crs
         self.destination_url = destination_url
         self.format = format
         self.granule_id = granule_id
         self.granule_name = granule_name
         self.height = height
         self.interpolation = interpolation
@@ -291,14 +327,15 @@
             'height': 'height',
             'format': 'format',
             'max_results': 'maxResults',
             'concatenate': 'concatenate',
             'skip_preview': 'skipPreview',
             'ignore_errors': 'ignoreErrors',
             'grid': 'grid',
+            'extend': 'extend'
         }
 
         self.spatial_validations = [
             (lambda bb: bb.s <= bb.n, ('Southern latitude must be less than '
                                        'or equal to Northern latitude')),
             (lambda bb: bb.s >= -90.0, 'Southern latitude must be greater than -90.0'),
             (lambda bb: bb.n >= -90.0, 'Northern latitude must be greater than -90.0'),
@@ -327,24 +364,14 @@
              ('Dimension minimum value must be less than or equal to the maximum value'))
         ]
         self.parameter_validations = [  # for simple, one-off validations
             (True if self.destination_url is None else self.destination_url.startswith('s3://'),
              ('Destination URL must be an S3 location'))
         ]
 
-    def parameter_values(self) -> List[Tuple[str, Any]]:
-        """Returns tuples of each query parameter that has been set and its value."""
-        pvs = [(param, getattr(self, variable))
-               for variable, param in self.variable_name_to_query_param.items()]
-        return [(p, v) for p, v in pvs if v is not None]
-
-    def is_valid(self) -> bool:
-        """Determines if the request and its parameters are valid."""
-        return len(self.error_messages()) == 0
-
     def _shape_error_messages(self, shape) -> List[str]:
         """Returns a list of error message for the provided shape."""
         if not shape:
             return []
         if not os.path.exists(shape):
             return [f'The provided shape path "{shape}" does not exist']
         if not os.path.isfile(shape):
@@ -371,14 +398,58 @@
                 msgs = [m for v, m in self.dimension_validations if not v(dim)]
                 if msgs:
                     dimension_msgs += msgs
 
         return spatial_msgs + temporal_msgs + shape_msgs + dimension_msgs + parameter_msgs
 
 
+class CapabilitiesRequest(BaseRequest):
+    """A Harmony request to get the harmony capabilities of a CMR collection
+    Args:
+        Keyword arguments with optional collection_id, short_name and capabilities_version fields
+        - collection_id: The CMR collection Id that should be queried
+        - short_name: The CMR collection shortName that should be queried
+        - capabilities_version: the version of the collection capabilities request api
+
+    Returns:
+        A Harmony Capability Request instance
+    """
+
+    def __init__(self,
+                 **request_params
+                 ):
+
+        coll_identifier = request_params.get('collection_id', request_params.get('short_name'))
+
+        super().__init__(collection=coll_identifier)
+        self.collection_id = request_params.get('collection_id')
+        self.short_name = request_params.get('short_name')
+        self.capabilities_version = request_params.get('capabilities_version')
+
+        self.variable_name_to_query_param = {
+            'collection_id': 'collectionid',
+            'short_name': 'shortname',
+            'capabilities_version': 'version',
+        }
+
+    def error_messages(self) -> List[str]:
+        """A list of error messages, if any, for the request."""
+        error_msgs = []
+        if self.collection_id is None and self.short_name is None:
+            error_msgs = [
+                'Must specify either collection_id or short_name for CapabilitiesRequest'
+            ]
+        elif self.collection_id and self.short_name:
+            error_msgs = [
+                'CapabilitiesRequest cannot have both collection_id and short_name values'
+            ]
+
+        return error_msgs
+
+
 class LinkType(Enum):
     """The type of URL to provide when returning links to data.
 
     s3: Returns an Amazon Web Services (AWS) S3 URL
     https: Returns a standard HTTP URL
     """
     s3 = 's3'
@@ -449,23 +520,31 @@
         if self.session is None:
             if self.token:
                 self.session = create_session(self.config, token=self.token)
             else:
                 self.session = create_session(self.config, auth=self.auth)
         return self.session
 
-    def _submit_url(self, request: Request) -> str:
+    def _http_method(self, request: BaseRequest) -> str:
+        """Returns the HTTP method to use for the given request."""
+        method = 'GET' if isinstance(request, CapabilitiesRequest) else 'POST'
+        return method
+
+    def _submit_url(self, request: BaseRequest) -> str:
         """Constructs the URL for the request that is used to submit a new Harmony Job."""
-        variables = [v.replace('/', '%2F') for v in request.variables]
-        vars = ','.join(variables)
-        return (
-            f'{self.config.root_url}'
-            f'/{request.collection.id}'
-            f'/ogc-api-coverages/1.0.0/collections/{vars}/coverage/rangeset'
-        )
+        if isinstance(request, CapabilitiesRequest):
+            return (f'{self.config.root_url}/capabilities')
+        else:
+            variables = [v.replace('/', '%2F') for v in request.variables]
+            vars = ','.join(variables)
+            return (
+                f'{self.config.root_url}'
+                f'/{request.collection.id}'
+                f'/ogc-api-coverages/1.0.0/collections/{vars}/coverage/rangeset'
+            )
 
     def _status_url(self, job_id: str, link_type: LinkType = LinkType.https) -> str:
         """Constructs the URL for the Job that is used to get its status."""
         return f'{self.config.root_url}/jobs/{job_id}?linktype={link_type.value}'
 
     def _pause_url(self, job_id: str, link_type: LinkType = LinkType.https) -> str:
         """Constructs the URL for the Job that is used to pause it."""
@@ -474,27 +553,29 @@
     def _resume_url(self, job_id: str, link_type: LinkType = LinkType.https) -> str:
         """Constructs the URL for the Job that is used to resume it."""
         return f'{self.config.root_url}/jobs/{job_id}/resume?linktype={link_type.value}'
 
     def _cloud_access_url(self) -> str:
         return f'{self.config.root_url}/cloud-access'
 
-    def _params(self, request: Request) -> dict:
+    def _params(self, request: BaseRequest) -> dict:
         """Creates a dictionary of request query parameters from the given request."""
-        params = {'forceAsync': 'true'}
-
-        subset = self._spatial_subset_params(request) + \
-            self._temporal_subset_params(request) + \
-            self._dimension_subset_params(request)
+        params = {}
+        if not isinstance(request, CapabilitiesRequest):
+            params['forceAsync'] = 'true'
+
+            subset = self._spatial_subset_params(request) + \
+                self._temporal_subset_params(request) + \
+                self._dimension_subset_params(request)
 
-        if len(subset) > 0:
-            params['subset'] = subset
+            if len(subset) > 0:
+                params['subset'] = subset
 
-        file_param_names = ['shapefile']
-        query_params = [pv for pv in request.parameter_values() if pv[0] not in file_param_names]
+        skipped_params = ['shapefile']
+        query_params = [pv for pv in request.parameter_values() if pv[0] not in skipped_params]
         for p, val in query_params:
             if type(val) == str:
                 params[p] = val
             elif type(val) == bool:
                 params[p] = str(val).lower()
             elif type(val) == list and type(val[0]) != str:
                 params[p] = ','.join([str(v) for v in val])
@@ -544,42 +625,42 @@
             if user_agent_content:
                 self.headers = {'User-Agent': ' '.join(user_agent_content)}
             else:
                 self.headers = {}
 
         return self.headers
 
-    def _spatial_subset_params(self, request: Request) -> list:
+    def _spatial_subset_params(self, request: BaseRequest) -> list:
         """Creates a dictionary of spatial subset query parameters."""
         if request.spatial:
             lon_left, lat_lower, lon_right, lat_upper = request.spatial
             return [f'lat({lat_lower}:{lat_upper})', f'lon({lon_left}:{lon_right})']
         else:
             return []
 
-    def _temporal_subset_params(self, request: Request) -> list:
+    def _temporal_subset_params(self, request: BaseRequest) -> list:
         """Creates a dictionary of temporal subset query parameters."""
         if request.temporal:
             t = request.temporal
             start = t['start'].isoformat() if 'start' in t else None
             stop = t['stop'].isoformat() if 'stop' in t else None
             start_quoted = f'"{start}"' if start else '*'
             stop_quoted = f'"{stop}"' if stop else '*'
             return [f'time({start_quoted}:{stop_quoted})']
         else:
             return []
 
-    def _dimension_subset_params(self, request: Request) -> list:
+    def _dimension_subset_params(self, request: BaseRequest) -> list:
         """Creates a list of dimension subset query parameters."""
         if request.dimensions and len(request.dimensions) > 0:
             dimensions = []
             for dim in request.dimensions:
                 dim_min = dim.min if dim.min is not None else '*'
                 dim_max = dim.max if dim.max is not None else '*'
-                dim_query_param = [f'{dim.name}({dim_min}:{dim_max})']
+                dim_query_param = f'{dim.name}({dim_min}:{dim_max})'
                 dimensions.append(dim_query_param)
             return dimensions
         else:
             return []
 
     @contextmanager
     def _files(self, request) -> ContextManager[Mapping[str, Any]]:
@@ -601,77 +682,89 @@
             yield result
         finally:
             for f in files:
                 f.close()
 
     def _params_dict_to_files(self, params: Mapping[str, Any]) -> List[Tuple[None, str, None]]:
         """Returns the given parameter mapping as a list of tuples suitable for multipart POST
-
-        This method is a temporary need until HARMONY-290 is implemented, since we cannot
-        currently pass query parameters to a shapefile POST request.  Because we need to pass
-        them as a multipart POST body, we need to inflate them into a list of tuples, one for
-        each parameter value to allow us to call requests.post(..., files=params)
-
         Args:
             params: A dictionary of parameter mappings as returned by self._params(request)
 
         Returns:
             A list of tuples suitable for passing to a requests multipart upload corresponding
             to the provided parameters
         """
-        # TODO: remove / refactor after HARMONY-290 is complete
         result = []
         for key, values in params.items():
-            if not isinstance(values, list):
-                values = [values]
-            result += [(key, (None, str(value), None)) for value in values]
+            if key == 'granuleId' and isinstance(values, list):
+                # Include all granuleId values in a single file boundary as a comma separated
+                # list to avoid creating too many file boundaries
+                concatenated_values = ','.join(map(str, values))
+                result.append((key, (None, concatenated_values, None)))
+            else:
+                if not isinstance(values, list):
+                    values = [values]
+                result += [(key, (None, str(value), None)) for value in values]
         return result
 
-    def _get_prepared_request(self, request: Request) -> requests.models.PreparedRequest:
+    def _get_prepared_request(
+            self, request: BaseRequest, for_browser=False) -> requests.models.PreparedRequest:
         """Returns a :requests.models.PreparedRequest: object for the given harmony Request
 
         Args:
             request: The Harmony Request to prepare
+            for_browser: if True only the url with query params will be returned
 
         Returns:
             A PreparedRequest
 
         """
         session = self._session()
         params = self._params(request)
         headers = self._headers()
 
+        method = self._http_method(request)
         with self._files(request) as files:
-            if files:
+            if (files or method == 'POST') and not for_browser:
                 # Ideally this should just be files=files, params=params but Harmony
                 # cannot accept both files and query params now.  (HARMONY-290)
                 # Inflate params to a list of tuples that can be passed as multipart
                 # form-data.  This must be done this way due to e.g. "subset" having
                 # multiple values
 
+                # Note: harmony only supports multipart/form-data which is why we use
+                # the workaround with files rather than `data=params` even when there
+                # is no shapefile to send
+
                 param_items = self._params_dict_to_files(params)
                 file_items = [(k, v) for k, v in files.items()]
+                all_files = param_items + file_items
 
                 r = requests.models.Request('POST',
                                             self._submit_url(request),
-                                            files=param_items + file_items,
+                                            files=all_files,
                                             headers=headers)
-                prepped_request = session.prepare_request(r)
             else:
+                if files:
+                    raise Exception("Cannot include shapefile as URL query parameter")
+
                 r = requests.models.Request('GET',
                                             self._submit_url(request),
                                             params=params,
                                             headers=headers)
-                prepped_request = session.prepare_request(r)
+
+            prepped_request = session.prepare_request(r)
+            if for_browser:
+                prepped_request.headers = None
 
         return prepped_request
 
     def _handle_error_response(self, response: Response):
         """Raises the appropriate exception based on the response
-        received from Harmony. Trys to pull out an error message
+        received from Harmony. Tries to pull out an error message
         from a Harmony JSON response when possible.
 
         Args:
             response: The Response from Harmony
 
         Raises:
             Exception with a Harmony error message or a more generic
@@ -687,15 +780,15 @@
                         exception_message = response_json.get('error')
             except JSONDecodeError:
                 pass
             if exception_message:
                 raise Exception(response.reason, exception_message)
         response.raise_for_status()
 
-    def request_as_curl(self, request: Request) -> str:
+    def request_as_curl(self, request: BaseRequest) -> str:
         """Returns a curl command representation of the given request.
         **Note** Authorization headers will be masked to reduce risk of
         accidental exposure. Also, cookies containing the string 'token'
         will be removed from the curl command.
 
         Args:
             request: The Request to build a curl command for
@@ -709,39 +802,58 @@
         if 'Cookie' in prepped_request.headers and 'token' in prepped_request.headers['Cookie']:
             cooks = self._session().cookies.get_dict()
             del prepped_request.headers['Cookie']
             cooks['token'] = '*****'
             prepped_request.prepare_cookies(cooks)
         return curlify.to_curl(prepped_request)
 
-    def submit(self, request: Request) -> Optional[str]:
+    def request_as_url(self, request: BaseRequest) -> str:
+        """Returns a URL string representation of the given request.
+        **Note** Headers and cookies are not included, just the URL.
+        Shapefiles are not supported.
+
+        Args:
+            request: The Request to build the URL string for
+
+        Returns:
+            A URL string that can be pasted into a browser.
+        :raises
+            Exception: if a shapefile is included in the request.
+        """
+        return self._get_prepared_request(request, for_browser=True).url
+
+    def submit(self, request: BaseRequest) -> any:
         """Submits a request to Harmony and returns the Harmony Job ID.
 
         Args:
             request: The Request to submit to Harmony (will be validated before sending)
 
         Returns:
-            The Harmony Job ID
+            The Harmony Job ID for request done through async jobs
+            The JSON response for direct download request
+            The capabilities response for capabilities request
         """
         if not request.is_valid():
             msgs = ', '.join(request.error_messages())
             raise Exception(f"Cannot submit the request due to the following errors: [{msgs}]")
 
-        job_id = None
         session = self._session()
 
         response = session.send(self._get_prepared_request(request))
 
         if response.ok:
-            job_id = (response.json())['jobID']
+            if isinstance(request, CapabilitiesRequest):
+                return response.json()
+            elif response.json()['status'] == 'successful':
+                return response.json()
+            else:
+                return response.json()['jobID']
         else:
             self._handle_error_response(response)
 
-        return job_id
-
     def status(self, job_id: str) -> dict:
         """Retrieve a submitted job's metadata from Harmony.
 
         Args:
             job_id: UUID string for the job you wish to interrogate.
 
         Returns:
@@ -986,36 +1098,80 @@
             The job's complete list of data URLs.
         """
         for page in self._result_pages(job_id, show_progress, link_type):
             for link in page.get('links', []):
                 if link['rel'] == 'data':
                     yield link['href']
 
+    def _is_staged_result(self, url: str) -> str:
+        """Check if the URL indicates that the data is associated with actual
+        service ouputs (as opposed to a download link for example).
+
+        Args:
+            url: The location (URL) of the file to be downloaded
+
+        Returns:
+            A boolean indicating whether the data is staged data.
+        """
+        url_parts = url.split('/')
+        possible_uuid = url_parts[-3]
+        possible_item_id = url_parts[-2]
+        try:
+            uuid_obj = UUID(possible_uuid, version=4)
+        except ValueError:
+            return False
+        if str(uuid_obj) != possible_uuid:
+            return False
+        if not possible_item_id.isnumeric():
+            return False
+        return True
+
+    def get_download_filename_from_url(self, url: str) -> str:
+        """For a given URL, returns the filename that will be used for download.
+        It will include a Harmony generated ID prefix if the data is staged.
+
+        Args:
+            url: The location (URL) of the file to be downloaded
+
+        Returns:
+            The filename that will be used to name the downloaded file.
+        """
+        url_parts = url.split('/')
+        original_filename = url_parts[-1]
+
+        is_staged_result = self._is_staged_result(url)
+        if not is_staged_result:
+            return original_filename
+        item_id = url_parts[-2]
+        return f'{item_id}_{original_filename}'
+
     def _download_file(self, url: str, directory: str = '', overwrite: bool = False) -> str:
         """Downloads data, saves it to a file, and returns the filename.
 
         Performance should be close to native with an appropriate chunk size. This can be changed
         via environment variable DOWNLOAD_CHUNK_SIZE.
 
-        Filenames are automatically determined by using the latter portion of the provided URL.
+        Filenames are automatically determined by using the latter portion of the provided URL
+        and will be prefixed by the item id generated by Harmony when data was transformed
+        from the original.
 
         Args:
             url: The location (URL) of the file to be downloaded
             directory: Optional. If specified, saves files there. Saves files to the current
             working directory by default.
             overwrite: If True, will overwrite a local file that shares a filename with the
             downloaded file. Defaults to False. If you're seeing malformed data or truncated
             files from incomplete downloads, set overwrite to True.
 
         Returns:
             The filename and path.
         """
         chunksize = int(self.config.DOWNLOAD_CHUNK_SIZE)
         session = self._session()
-        filename = url.split('/')[-1]
+        filename = self.get_download_filename_from_url(url)
 
         if directory:
             filename = os.path.join(directory, filename)
 
         verbose = os.getenv('VERBOSE', 'TRUE')
         if not overwrite and os.path.isfile(filename):
             if verbose and verbose.upper() == 'TRUE':
@@ -1048,15 +1204,15 @@
         """
         if url.endswith('zarr'):
             raise self.zarr_download_exception
         future = self.executor.submit(self._download_file, url, directory, overwrite)
         return future
 
     def download_all(self,
-                     job_id: str,
+                     job_id_or_result_json: Union[str, dict],
                      directory: str = '',
                      overwrite: bool = False) -> Generator[Future, None, None]:
         """Using a job_id, fetches all the data files from a finished job.
 
         After this method is able to contact Harmony and query a finished job, it will
         immediately return with a list of python concurrent.Futures corresponding to each of the
         files to be downloaded. Call the result() method to block until the downloading of that
@@ -1080,39 +1236,49 @@
             downloaded file. Defaults to False. If you're seeing malformed data or truncated
             files from incomplete downloads, set overwrite to True.
 
         Returns:
             A list of Futures, each of which will return the filename (with path) for each
             result.
         """
-        for url in self.result_urls(job_id, show_progress=False) or []:
-            if url.endswith('zarr'):
-                raise self.zarr_download_exception
-            yield self.executor.submit(self._download_file, url, directory, overwrite)
+        if isinstance(job_id_or_result_json, str):
+            for url in self.result_urls(job_id_or_result_json, show_progress=False) or []:
+                if url.endswith('zarr'):
+                    raise self.zarr_download_exception
+                yield self.executor.submit(self._download_file, url, directory, overwrite)
+        else:
+            for link in job_id_or_result_json.get('links', []):
+                if link['rel'] == 'data':
+                    url = link['href']
+                    if url.endswith('zarr'):
+                        raise self.zarr_download_exception
+                    yield self.executor.submit(self._download_file, url, directory, overwrite)
 
     def iterator(
         self,
         job_id: str,
         directory: str = '',
         overwrite: bool = False
     ) -> Iterator:
         """Create an iterator that will poll for data in the background and download it as
         it is available and requested via `next()`.
 
         Each iteration returns a dictionary, or `None` when all granules have been iterated.
         The dictionary has the following form:
 
-        {
-            'path': Future
-            'bbox': BBox object containing the bounding box for the granule,
-            'temporal': {
-                'start': '2020-01-11T14:00:00.000Z',
-                'end': '2020-01-11T15:59:59.000Z'
+        .. code-block:: python
+
+            {
+                'path': Future
+                'bbox': BBox object containing the bounding box for the granule,
+                'temporal': {
+                    'start': '2020-01-11T14:00:00.000Z',
+                    'end': '2020-01-11T15:59:59.000Z'
+                }
             }
-        }
 
         The Future resolves to the path to the downloaded file.
 
         If the job is paused and all processed granules have already been returned in
         the iteration, the status returned will be GranuleStatus.PAUSED until the job
         is resumed.
```

### Comparing `harmony-py-0.4.9/harmony/util.py` & `harmony_py-1756b0/harmony/util.py`

 * *Files identical despite different names*

### Comparing `harmony-py-0.4.9/harmony_py.egg-info/PKG-INFO` & `harmony_py-1756b0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: harmony-py
-Version: 0.4.9
+Version: 1756b0
 Summary: The NASA Harmony Python library
 Home-page: https://github.com/nasa/harmony-py
 Keywords: nasa,harmony,remote-sensing,science,geoscience
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
@@ -14,16 +14,39 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: python-dateutil~=2.8.2
+Requires-Dist: python-dotenv~=0.20.0
+Requires-Dist: progressbar2~=4.2.0
+Requires-Dist: requests~=2.28
+Requires-Dist: sphinxcontrib-napoleon~=0.7
+Requires-Dist: curlify~=2.2.1
+Provides-Extra: dev
+Requires-Dist: autopep8~=1.4; extra == "dev"
+Requires-Dist: camel-case-switcher~=2.0; extra == "dev"
+Requires-Dist: coverage~=5.4; extra == "dev"
+Requires-Dist: flake8~=3.8; extra == "dev"
+Requires-Dist: hypothesis~=6.2; extra == "dev"
+Requires-Dist: importlib-metadata<5.0; extra == "dev"
+Requires-Dist: mypy~=0.812; extra == "dev"
+Requires-Dist: nose~=1.3; extra == "dev"
+Requires-Dist: PyYAML~=6.0.1; extra == "dev"
+Requires-Dist: pytest~=6.2; extra == "dev"
+Requires-Dist: pytest-cov~=2.11; extra == "dev"
+Requires-Dist: pytest-mock~=3.5; extra == "dev"
+Requires-Dist: pytest-watch~=4.2; extra == "dev"
+Requires-Dist: responses~=0.12; extra == "dev"
+Requires-Dist: setuptools>=54.2; extra == "dev"
+Requires-Dist: sphinx~=7.1.2; extra == "dev"
+Requires-Dist: wheel>=0.36; extra == "dev"
 
 # harmony-py
 
 [![Documentation Status](https://readthedocs.org/projects/harmony-py/badge/?version=latest)](https://harmony-py.readthedocs.io/en/latest/?badge=latest)
 
 Harmony-Py is a Python library for integrating with NASA's [Harmony](https://harmony.earthdata.nasa.gov/) Services.
 
@@ -31,15 +54,15 @@
 
 We welcome feedback on Harmony-Py via [GitHub Issues](https://github.com/nasa/harmony-py/issues)
 
 # Using Harmony Py
 
 ## Prerequisites
 
-* Python 3.7+
+* Python 3.8+
 
 
 ## Installing
 
 The library is available from [PyPI](https://pypi.org/project/harmony-py/) and can be installed with pip:
 
         $ pip install -U harmony-py
```

### Comparing `harmony-py-0.4.9/setup.py` & `harmony_py-1756b0/setup.py`

 * *Files identical despite different names*

### Comparing `harmony-py-0.4.9/tests/test_auth.py` & `harmony_py-1756b0/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `harmony-py-0.4.9/tests/test_client.py` & `harmony_py-1756b0/tests/test_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,82 +7,164 @@
 import urllib.parse
 import pathlib
 
 import dateutil.parser
 import pytest
 import responses
 
-from harmony.harmony import BBox, Client, Collection, LinkType, ProcessingFailedException, Request, Dimension
+from harmony.harmony import BBox, Client, Collection, LinkType, ProcessingFailedException, Dimension
+from harmony.harmony import Request, CapabilitiesRequest
 
 
 @pytest.fixture()
 def examples_dir():
     return pathlib.Path(__file__).parent.parent.joinpath('examples').absolute()
 
 
 def expected_submit_url(collection_id, variables='all'):
     return (f'https://harmony.earthdata.nasa.gov/{collection_id}'
             f'/ogc-api-coverages/1.0.0/collections/{variables}/coverage/rangeset')
 
-
 def expected_status_url(job_id, link_type: LinkType = LinkType.https):
     return f'https://harmony.earthdata.nasa.gov/jobs/{job_id}?linktype={link_type.value}'
 
 def expected_pause_url(job_id, link_type: LinkType = LinkType.https):
     return f'https://harmony.earthdata.nasa.gov/jobs/{job_id}/pause?linktype={link_type.value}'
 
 def expected_resume_url(job_id, link_type: LinkType = LinkType.https):
     return f'https://harmony.earthdata.nasa.gov/jobs/{job_id}/resume?linktype={link_type.value}'
 
-def expected_full_submit_url(request):
+def parse_multipart_data(request):
+    """Parses multipart/form-data request to extract fields as strings."""
+    body_bytes = request.body
+    content_type = request.headers['Content-Type']
+
+    # Extract boundary from Content-Type header
+    boundary = content_type.split("boundary=")[1]
+    boundary_bytes = ('--' + boundary).encode()
+
+    parts = body_bytes.split(boundary_bytes)
+
+    form_data = {}
+    cd_regex = re.compile(rb'Content-Disposition: form-data; name="([^"]+)"(?:; filename="([^"]+)")?', re.IGNORECASE)
+
+    for part in parts:
+        if part.strip():
+            # Splitting headers and body
+            parts_split = part.split(b'\r\n\r\n', 1)
+            if len(parts_split) == 2:
+                headers, body = parts_split
+                body = body.strip(b'\r\n')
+
+                cd_match = cd_regex.search(headers)
+                if cd_match:
+                    field_name = cd_match.group(1).decode('utf-8')
+                    filename = cd_match.group(2)
+
+                    if filename:
+                        filename = filename.decode('utf-8')
+                        form_data[field_name] = {'filename': filename, 'content': body}
+                    else:  # It's a regular form field
+                        value = body.decode('utf-8').strip()
+                        if field_name in form_data:
+                            # If it's already a list, append to it
+                            if isinstance(form_data[field_name], list):
+                                form_data[field_name].append(value)
+                            else:
+                                # If it's not a list, make it a list with the old and new value
+                                form_data[field_name] = [form_data[field_name], value]
+                        else:
+                            # If the field doesn't exist, add it normally
+                            form_data[field_name] = value
+
+    return form_data
+
+def construct_expected_params(query_string):
+    """Returns the expected parameters from a query string. Needed a custom function to
+    handle multiple values for the same parameter name such as `subset`.
+    """
+    parsed_params = urllib.parse.parse_qsl(query_string)
+    expected_params = {}
+    for key, value in parsed_params:
+        if key in expected_params:
+            # If the key already exists, and it's not a list, convert it to a list
+            if not isinstance(expected_params[key], list):
+                expected_params[key] = [expected_params[key]]
+            # Append the new value to the existing list
+            expected_params[key].append(value)
+        else:
+            # Add the key-value pair to the dictionary
+            expected_params[key] = value
+    return expected_params
+
+def is_expected_url_and_form_encoded_body(harmony_request, http_request):
+    """Returns True if the URL and form encoded body match what is expected based
+    on the harmony request object.
+    """
+    form_data_params = parse_multipart_data(http_request)
     async_params = ['forceAsync=true']
 
     spatial_params = []
-    if request.spatial:
-        w, s, e, n = request.spatial
+    if harmony_request.spatial:
+        w, s, e, n = harmony_request.spatial
         spatial_params = [f'subset=lat({s}:{n})', f'subset=lon({w}:{e})']
 
     temporal_params = []
-    if request.temporal:
-        start = request.temporal['start']
-        stop = request.temporal['stop']
+    if harmony_request.temporal:
+        start = harmony_request.temporal['start']
+        stop = harmony_request.temporal['stop']
         temporal_params = [f'subset=time("{start.isoformat()}":"{stop.isoformat()}")']
 
     dimension_params = []
-    if request.dimensions:
-        for dim in request.dimensions:
+    if harmony_request.dimensions:
+        for dim in harmony_request.dimensions:
             name = dim.name
             min = dim.min if dim.min is not None else '*'
             max = dim.max if dim.max is not None else '*'
             dimension_params += [f'subset={name}({min}:{max})']
 
     query_params = '&'.join(async_params + spatial_params + temporal_params + dimension_params)
-    if request.format is not None:
-        query_params += f'&format{request.format}'
-    if request.skip_preview is not None:
-        query_params += f'&skipPreview={str(request.skip_preview).lower()}'
+    if harmony_request.format is not None:
+        query_params += f'&format{harmony_request.format}'
+    if harmony_request.skip_preview is not None:
+        query_params += f'&skipPreview={str(harmony_request.skip_preview).lower()}'
+
+    expected_params = construct_expected_params(query_params)
+
+    return form_data_params == expected_params and http_request.url ==  expected_submit_url(harmony_request.collection.id)
+
+def expected_capabilities_url(request_params: dict):
+    collection_id = request_params.get('collection_id')
+    short_name = request_params.get('short_name')
+    capabilities_version = request_params.get('capabilities_version')
+    url = 'https://harmony.earthdata.nasa.gov/capabilities'
+    if collection_id:
+        url = (f'{url}?collectionid={collection_id}')
+    elif short_name:
+        url = (f'{url}?shortname={short_name}')
 
-    return f'{expected_submit_url(request.collection.id)}?{query_params}'
+    if capabilities_version:
+        url = (f'{url}&version={capabilities_version}')
+
+    return url
 
 
 def fake_data_url(link_type: LinkType = LinkType.https):
     if link_type == LinkType.s3:
         fake_data_url = f'{link_type.value}://fakebucket/public/harmony/foo'
     else:
         fake_data_url = f'{link_type.value}://harmony.earthdata.nasa.gov/service-results'
     return f'{fake_data_url}/fake.tif'
 
-
 def expected_user_agent_header_regex():
     # Since it's kinda overkill to find the exact character set
     #   allowed in platform/implementation/version/etc,
     #   the following regex may be a little bit more tolerant
     return r"\s*([^/\s]+/[^/\s]+)(\s+[^/\s]+/[^/\s]+)*\s*"
 
-
 def expected_job(collection_id, job_id, link_type: LinkType = LinkType.https, extra_links=[]):
     return {
         'username': 'rfeynman',
         'status': 'running',
         'message': 'The job is being processed',
         'progress': 0,
         'createdAt': '2021-02-19T18:47:31.291Z',
@@ -133,14 +215,54 @@
 
 def expected_paused_job(collection_id, job_id, link_type: LinkType = LinkType.https, extra_links=[]):
     job = expected_job(collection_id, job_id, link_type, extra_links)
     job['status'] = 'paused'
     job['progress'] = 10
     return job
 
+def expected_capabilities(collection_id):
+    return {
+        'conceptId': 'C1940468263-POCLOUD',
+        'shortName': 'SMAP_RSS_L3_SSS_SMI_8DAY-RUNNINGMEAN_V4',
+        'variableSubset': False,
+        'bboxSubset': False,
+        'shapeSubset': False,
+        'concatenate': True,
+        'reproject': False,
+        'outputFormats': [
+            'application/x-zarr'
+        ],
+        'services': [
+            {
+                'name': 'harmony/netcdf-to-zarr',
+                'href': 'https://cmr.earthdata.nasa.gov/search/concepts/S2009180097-POCLOUD',
+                'capabilities': {
+                        'concatenation': True,
+                        'concatenate_by_default': False,
+                        'subsetting': {
+                            'variable': False
+                        },
+                    'output_formats': [
+                            'application/x-zarr'
+                        ]
+                }
+            }
+        ],
+        'variables': [
+            {
+                'name': 'fland',
+                'href': 'https://cmr.earthdata.nasa.gov/search/concepts/V2093907988-POCLOUD'
+            },
+            {
+                'name': 'time',
+                'href': 'https://cmr.earthdata.nasa.gov/search/concepts/V2112018545-POCLOUD'
+            }
+        ],
+        'capabilitiesVersion': '2'
+    }
 
 @responses.activate
 def test_when_multiple_submits_it_only_authenticates_once():
     collection = Collection(id='C1940468263-POCLOUD')
     request = Request(
         collection=collection,
         spatial=BBox(-107, 40, -105, 42)
@@ -149,80 +271,74 @@
     auth_url = 'https://harmony.earthdata.nasa.gov/jobs'
     responses.add(
         responses.GET,
         auth_url,
         status=200
     )
     responses.add(
-        responses.GET,
+        responses.POST,
         expected_submit_url(collection.id),
         status=200,
         json=expected_job(collection.id, job_id)
     )
 
     client = Client()
     client.submit(request)
     client.submit(request)
 
     assert len(responses.calls) == 3
     assert responses.calls[0].request.url == auth_url
     assert urllib.parse.unquote(responses.calls[0].request.url) == auth_url
-    assert urllib.parse.unquote(
-        responses.calls[1].request.url) == expected_full_submit_url(request)
-    assert urllib.parse.unquote(
-        responses.calls[2].request.url) == expected_full_submit_url(request)
-
+    assert is_expected_url_and_form_encoded_body(request, responses.calls[1].request)
+    assert is_expected_url_and_form_encoded_body(request, responses.calls[2].request)
 
 @responses.activate
 def test_with_bounding_box():
     collection = Collection(id='C1940468263-POCLOUD')
     request = Request(
         collection=collection,
         spatial=BBox(-107, 40, -105, 42)
     )
     job_id = '21469294-d6f7-42cc-89f2-c81990a5d7f4'
     responses.add(
-        responses.GET,
+        responses.POST,
         expected_submit_url(collection.id),
         status=200,
         json=expected_job(collection.id, job_id)
     )
 
     actual_job_id = Client(should_validate_auth=False).submit(request)
 
     assert len(responses.calls) == 1
     assert responses.calls[0].request is not None
-    assert urllib.parse.unquote(
-        responses.calls[0].request.url) == expected_full_submit_url(request)
+    assert is_expected_url_and_form_encoded_body(request, responses.calls[0].request)
     assert actual_job_id == job_id
 
 @responses.activate
 def test_with_single_dimension():
     collection = Collection(id='C1940468263-POCLOUD')
     request = Request(
         collection=collection,
         dimensions=[Dimension('foo', 0, 20.5)]
     )
     job_id = '21469294-d6f7-42cc-89f2-c81990a5d7f4'
     responses.add(
-        responses.GET,
+        responses.POST,
         expected_submit_url(collection.id),
         status=200,
         json=expected_job(collection.id, job_id)
     )
 
     actual_job_id = Client(should_validate_auth=False).submit(request)
 
     assert len(responses.calls) == 1
     assert responses.calls[0].request is not None
-    assert urllib.parse.unquote(
-        responses.calls[0].request.url) == expected_full_submit_url(request)
+    assert is_expected_url_and_form_encoded_body(request, responses.calls[0].request)
     assert actual_job_id == job_id
 
-
 @responses.activate
 def test_with_multiple_dimensions():
     collection = Collection(id='C1940468263-POCLOUD')
     request = Request(
         collection=collection,
         dimensions=[
             Dimension('foo', None, 20.5),
@@ -232,83 +348,78 @@
             Dimension('bravo', max=30),
             Dimension('charlie', min=20),
             Dimension('delta', 0, 20.5),
         ]
     )
     job_id = '21469294-d6f7-42cc-89f2-c81990a5d7f4'
     responses.add(
-        responses.GET,
+        responses.POST,
         expected_submit_url(collection.id),
         status=200,
         json=expected_job(collection.id, job_id)
     )
 
     actual_job_id = Client(should_validate_auth=False).submit(request)
 
     assert len(responses.calls) == 1
     assert responses.calls[0].request is not None
-    assert urllib.parse.unquote(
-        responses.calls[0].request.url) == expected_full_submit_url(request)
+    assert is_expected_url_and_form_encoded_body(request, responses.calls[0].request)
     assert actual_job_id == job_id
 
 @responses.activate
 def test_with_temporal_range():
     collection = Collection(id='C1234-TATOOINE')
     request = Request(
         collection=collection,
         temporal={
             'start': dt.datetime(2010, 12, 1),
             'stop': dt.datetime(2010, 12, 31)
         },
     )
     job_id = '1234abcd-deed-9876-c001-f00dbad'
     responses.add(
-        responses.GET,
+        responses.POST,
         expected_submit_url(collection.id),
         status=200,
         json=expected_job(collection.id, job_id)
     )
 
     actual_job_id = Client(should_validate_auth=False).submit(request)
 
     assert len(responses.calls) == 1
     assert responses.calls[0].request is not None
-    assert urllib.parse.unquote(
-        responses.calls[0].request.url) == expected_full_submit_url(request)
+    assert is_expected_url_and_form_encoded_body(request, responses.calls[0].request)
     assert actual_job_id == job_id
 
-
 @responses.activate
 def test_with_bounding_box_and_temporal_range():
     collection = Collection(id='C333666999-EOSDIS')
     request = Request(
         collection=collection,
         spatial=BBox(-107, 40, -105, 42),
         temporal={
             'start': dt.datetime(2001, 1, 1),
             'stop': dt.datetime(2003, 3, 31)
         },
     )
     job_id = '1234abcd-1234-9876-6666-999999abcd'
     responses.add(
-        responses.GET,
+        responses.POST,
         expected_submit_url(collection.id),
         status=200,
         json=expected_job(collection.id, job_id)
     )
 
     actual_job_id = Client(should_validate_auth=False).submit(request)
 
     assert len(responses.calls) == 1
     assert responses.calls[0].request is not None
-    assert urllib.parse.unquote(
-        responses.calls[0].request.url) == expected_full_submit_url(request)
+    assert is_expected_url_and_form_encoded_body(request, responses.calls[0].request)
     assert actual_job_id == job_id
 
-
 @responses.activate
 def test_with_shapefile(examples_dir):
     collection = Collection(id='C333666999-EOSDIS')
     request = Request(
         collection=collection,
         shape=os.path.join(examples_dir, 'asf_example.json'),
         spatial=BBox(-107, 40, -105, 42),
@@ -340,34 +451,32 @@
     # Would-be query params are in the POST body
     assert 'Content-Disposition: form-data; name="forceAsync"\r\n\r\ntrue' in post_body
     assert 'Content-Disposition: form-data; name="subset"\r\n\r\nlat(40:42)' in post_body
     assert 'Content-Disposition: form-data; name="subset"\r\n\r\nlon(-107:-105)' in post_body
 
     assert actual_job_id == job_id
 
-
 def test_with_invalid_request():
     collection = Collection(id='C333666999-EOSDIS')
     request = Request(
         collection=collection,
         spatial=BBox(-190, -100, 100, 190)
     )
 
     with pytest.raises(Exception):
         Client(should_validate_auth=False).submit(request)
 
-
 @responses.activate
 def test_get_request_has_user_agent_headers():
     collection = Collection('foobar')
     request = Request(
         collection=collection,
     )
     responses.add(
-        responses.GET,
+        responses.POST,
         expected_submit_url(collection.id),
         status=200,
         json=expected_job(collection.id, 'abcd-1234'),
     )
 
     Client(should_validate_auth=False).submit(request)
 
@@ -377,102 +486,106 @@
     headers = responses.calls[0].request.headers
     assert "User-Agent" in headers
     user_agent_header = headers["User-Agent"]
     assert re.match(
         expected_user_agent_header_regex(), user_agent_header
     )
 
-
 @responses.activate
 def test_post_request_has_user_agent_headers(examples_dir):
     collection = Collection('foobar')
     request = Request(
         collection=collection,
         shape=os.path.join(examples_dir, 'asf_example.json'),
         spatial=BBox(-107, 40, -105, 42),
     )
-    job_id = '1234abcd-1234-9876-6666-999999abcd'
     responses.add(
         responses.POST,
         expected_submit_url(collection.id),
         status=200,
         json=expected_job(collection.id, 'abcd-1234'),
     )
 
-    actual_job_id = Client(should_validate_auth=False).submit(request)
+    Client(should_validate_auth=False).submit(request)
 
     assert len(responses.calls) == 1
     assert len(responses.calls) == 1
     assert responses.calls[0].request is not None
     assert responses.calls[0].request.headers is not None
     headers = responses.calls[0].request.headers
     assert "User-Agent" in headers
     user_agent_header = headers["User-Agent"]
     assert re.match(
         expected_user_agent_header_regex(), user_agent_header
     )
 
-
 @pytest.mark.parametrize('param,expected', [
     ({'crs': 'epsg:3141'}, 'outputcrs=epsg:3141'),
     ({'destination_url': 's3://bucket'}, 'destinationUrl=s3://bucket'),
     ({'format': 'r2d2/hologram'}, 'format=r2d2/hologram'),
-    ({'granule_id': ['G1', 'G2', 'G3']}, 'granuleId=G1&granuleId=G2&granuleId=G3'),
-    ({'granule_name': ['abc*123', 'ab?d123', 'abcd123']}, 'granuleName=abc*123&granuleName=ab?d123&granuleName=abcd123'),
+    ({'granule_id': ['G1', 'G2', 'G3']}, 'granuleId=G1,G2,G3'),
+    ({'granule_name': ['abc*123', 'ab?d123', 'abcd123']},
+     'granuleName=abc*123&granuleName=ab?d123&granuleName=abcd123'),
     ({'height': 200}, 'height=200'),
     ({'interpolation': 'nearest'}, 'interpolation=nearest'),
     ({'max_results': 7}, 'maxResults=7'),
     ({'scale_extent': [1.0, 2.0, 1.0, 4.0]}, 'scaleExtent=1.0,2.0,1.0,4.0'),
     ({'scale_size': [1.0, 2.0]}, 'scaleSize=1.0,2.0'),
     ({'width': 100}, 'width=100'),
     ({'concatenate': True}, 'concatenate=true'),
     ({'grid': 'theGridName'}, 'grid=theGridName'),
+    ({'extend': ['lat', 'lon']}, 'extend=lat&extend=lon'),
+    ({'extend': ['singleDimension']}, 'extend=singleDimension'),
 ])
+
 @responses.activate
 def test_request_has_query_param(param, expected):
+    expected += '&forceAsync=true'
     collection = Collection('foobar')
     request = Request(
         collection=collection,
         **param
     )
     responses.add(
-        responses.GET,
+        responses.POST,
         expected_submit_url(collection.id),
         status=200,
         json=expected_job(collection.id, 'abcd-1234'),
     )
 
     Client(should_validate_auth=False).submit(request)
 
     assert len(responses.calls) == 1
-    assert urllib.parse.unquote(responses.calls[0].request.url).index(expected) >= 0
 
+    body_params = parse_multipart_data(responses.calls[0].request)
+    expected_params = construct_expected_params(expected)
+
+    assert body_params == expected_params
 
 @responses.activate
 @pytest.mark.parametrize('variables,expected', [
     (['one'], 'one'),
     (['red_var', 'green_var', 'blue_var'], 'red_var,green_var,blue_var'),
     (['/var/with/a/path'], '%2Fvar%2Fwith%2Fa%2Fpath')
 ])
 def test_request_has_variables(variables, expected):
     collection = Collection('foobar')
     request = Request(
         collection=collection,
         variables=variables
     )
     responses.add(
-        responses.GET,
+        responses.POST,
         expected_submit_url(collection.id, expected),
         status=200,
         json=expected_job(collection.id, 'abcd-1234'),
     )
 
     Client(should_validate_auth=False).submit(request)
 
-
 @responses.activate
 def test_status():
     collection = Collection(id='C333666999-EOSDIS')
     job_id = '21469294-d6f7-42cc-89f2-c81990a5d7f4'
     exp_job = expected_job(collection.id, job_id)
     expected_status = {
         'status': exp_job['status'],
@@ -602,15 +715,15 @@
         'description': 'Error: Job status cannot be updated from successful to paused.'
     }
 
     responses.add(
         responses.GET,
         expected_pause_url(job_id),
         status=409,
-        json = exp_json
+        json=exp_json
     )
 
     with pytest.raises(Exception) as e:
         Client(should_validate_auth=False).pause(job_id)
     assert str(e.value) == "('Conflict', 'Error: Job status cannot be updated from successful to paused.')"
 
 @responses.activate
@@ -639,15 +752,15 @@
         'description': 'Error: Job status is running - only paused jobs can be resumed.'
     }
 
     responses.add(
         responses.GET,
         expected_resume_url(job_id),
         status=409,
-        json = exp_json
+        json=exp_json
     )
 
     with pytest.raises(Exception) as e:
         Client(should_validate_auth=False).resume(job_id)
     assert str(e.value) == "('Conflict', 'Error: Job status is running - only paused jobs can be resumed.')"
 
 @pytest.mark.parametrize('show_progress', [
@@ -679,15 +792,14 @@
     progress_mock.assert_called_with(job_id)
     if show_progress:
         for n, _, _ in expected_progress:
             progressbar_mock.update.assert_any_call(int(n))
     else:
         assert sleep_mock.call_count == len(expected_progress)
 
-
 @pytest.mark.parametrize('show_progress', [
     (True),
     (False),
 ])
 def test_wait_for_processing_with_failed_status(mocker, show_progress):
     expected_progress = [(0, 'failed', 'Pod exploded')]
     job_id = '12345'
@@ -759,15 +871,14 @@
     )
     client = Client(should_validate_auth=False)
     actual_json = client.result_json(job_id, show_progress=show_progress, link_type=link_type)
 
     assert actual_json == expected_json
     wait_mock.assert_called_with(job_id, show_progress)
 
-
 @responses.activate
 @pytest.mark.parametrize('show_progress', [
     (True),
     (False),
 ])
 @pytest.mark.parametrize('link_type', [LinkType.http, LinkType.https, LinkType.s3])
 def test_result_json_with_failed_request_doesnt_throw_exception(mocker, show_progress, link_type):
@@ -803,18 +914,20 @@
 
     result_json_mock = mocker.Mock(return_value=expected_json)
     processing_mock = mocker.Mock(return_value=None)
     mocker.patch('harmony.harmony.Client._get_json', result_json_mock)
     mocker.patch('harmony.harmony.Client.wait_for_processing', processing_mock)
 
     client = Client(should_validate_auth=False)
-    actual_urls = list(client.result_urls(job_id, show_progress=show_progress, link_type=link_type))
+    actual_urls = list(client.result_urls(
+        job_id, show_progress=show_progress, link_type=link_type))
 
     assert actual_urls == expected_urls
-    result_json_mock.assert_called_with(f'https://harmony.earthdata.nasa.gov/jobs/{job_id}?linktype={link_type.value}')
+    result_json_mock.assert_called_with(
+        f'https://harmony.earthdata.nasa.gov/jobs/{job_id}?linktype={link_type.value}')
 
 
 @pytest.mark.parametrize('show_progress', [
     (True),
     (False),
 ])
 @pytest.mark.parametrize('link_type', [LinkType.http, LinkType.https, LinkType.s3])
@@ -831,19 +944,22 @@
 
     get_json_mock = mocker.Mock(side_effect=[expected_json_first_page, expected_json_last_page])
     processing_mock = mocker.Mock(return_value=None)
     mocker.patch('harmony.harmony.Client._get_json', get_json_mock)
     mocker.patch('harmony.harmony.Client.wait_for_processing', processing_mock)
 
     client = Client(should_validate_auth=False)
-    actual_urls = list(client.result_urls(job_id, show_progress=show_progress, link_type=link_type))
+    actual_urls = list(client.result_urls(
+        job_id, show_progress=show_progress, link_type=link_type))
 
     assert actual_urls == expected_urls
-    get_json_mock.assert_any_call(f'https://harmony.earthdata.nasa.gov/jobs/{job_id}?linktype={link_type.value}')
-    get_json_mock.assert_any_call(f'https://harmony.earthdata.nasa.gov/jobs/{job_id}?linktype={link_type.value}&page=2')
+    get_json_mock.assert_any_call(
+        f'https://harmony.earthdata.nasa.gov/jobs/{job_id}?linktype={link_type.value}')
+    get_json_mock.assert_any_call(
+        f'https://harmony.earthdata.nasa.gov/jobs/{job_id}?linktype={link_type.value}&page=2')
 
 
 @pytest.mark.parametrize('overwrite', [
     (True),
     (False),
 ])
 def test_download_file(overwrite):
@@ -905,14 +1021,15 @@
     )
 
     client = Client(should_validate_auth=False)
     actual_file_names = [f.result() for f in client.download_all('abcd-1234')]
 
     assert actual_file_names == expected_file_names
 
+
 def test_download_all_zarr(mocker):
     expected_urls = [
         'http://www.example.com/1',
         'http://www.example.com/2.zarr',
         'http://www.example.com/3',
     ]
 
@@ -1041,30 +1158,42 @@
     status_resumed['status'] = 'running'
     status_successful = copy.deepcopy(status_resumed)
     status_successful['links'].append(extra_links[4])
     status_successful['status'] = 'successful'
 
     return [status_running1, status_running2, status_paused, status_resumed, status_successful, status_successful]
 
+def test_get_file_name_staged_link():
+    # For staged results, the filename should get prefixed with the work item id, to avoid collisions
+    client = Client(should_validate_auth=False)
+    actual_file_name = client.get_download_filename_from_url('https://harmony.earthdata.nasa.gov/service-results/staging-bucket/a7aee059-7531-4388-86e0-85af1de9c31a/1047412/C1254854453-LARC_CLOUD_merged.nc4')
+    assert actual_file_name == '1047412_C1254854453-LARC_CLOUD_merged.nc4'
+
+def test_get_file_name_non_staged_link():
+    # In this case, e.g. for a direct download data link, the filename should just be the last part of the URL path
+    client = Client(should_validate_auth=False)
+    actual_file_name = client.get_download_filename_from_url('https://harmony.earthdata.nasa.gov/service-results/test-data/C1261703151-EEDTEST/ATL08_20181014001049_02350102_006_02.h5')
+    assert actual_file_name == 'ATL08_20181014001049_02350102_006_02.h5'
+
 @pytest.mark.parametrize('link_type', [LinkType.http, LinkType.https, LinkType.s3])
 def test_iterator(link_type, mocker):
     extra_links = extra_links_for_iteration(link_type.value)
     status_page_json = expected_job('C123', 'abc123')
     status_page_json['status'] = 'successful'
-    download_file_mock = mocker.Mock(side_effect = side_effect_func_for_download_file)
+    download_file_mock = mocker.Mock(side_effect=side_effect_func_for_download_file)
     mocker.patch('harmony.harmony.Client._download_file', download_file_mock)
-    get_json_mock = mocker.Mock(side_effect = side_effect_for_get_json(extra_links))
+    get_json_mock = mocker.Mock(side_effect=side_effect_for_get_json(extra_links))
     mocker.patch('harmony.harmony.Client._get_json', get_json_mock)
     # speed up test by not waiting between polling the status page
     client = Client(should_validate_auth=False, check_interval=0)
 
     # first iteration in which job state is 'running' and two granules have completed
     iter = client.iterator(status_page_json['jobID'], '/tmp')
     granule_data = next(iter)
-    assert granule_data['bbox'] == BBox(-179.95,-89.95,179.95,89.95)
+    assert granule_data['bbox'] == BBox(-179.95, -89.95, 179.95, 89.95)
     assert granule_data['path'].result() == '/tmp/fake.tif'
 
     granule_data = next(iter)
     assert granule_data['bbox'] == BBox(*extra_links[0]['bbox'])
     assert granule_data['path'].result() == '/tmp/fake2.tif'
 
     # job is still running and has another completed granule
@@ -1081,15 +1210,15 @@
     granule_data = next(iter, None)
     assert granule_data == None
 
     # need to start a new iterator after resuming
     iter = client.iterator(status_page_json['jobID'], '/tmp')
     # initial granules returned are the same as before (they are not re-downloaded by default)
     granule_data = next(iter)
-    assert granule_data['bbox'] == BBox(-179.95,-89.95,179.95,89.95)
+    assert granule_data['bbox'] == BBox(-179.95, -89.95, 179.95, 89.95)
     assert granule_data['path'].result() == '/tmp/fake.tif'
     granule_data = next(iter)
     assert granule_data['bbox'] == BBox(*extra_links[0]['bbox'])
     assert granule_data['path'].result() == '/tmp/fake2.tif'
     granule_data = next(iter)
     assert granule_data['bbox'] == BBox(*extra_links[1]['bbox'])
     assert granule_data['path'].result() == '/tmp/fake3.tif'
@@ -1122,22 +1251,22 @@
 
     return [status_running, status_failed]
 
 @pytest.mark.parametrize('link_type', [LinkType.http, LinkType.https, LinkType.s3])
 def test_iterator_failed_job(link_type, mocker):
     # test with two successful work items followed by a failed job
     extra_links = extra_links_for_iteration(link_type.value)
-    get_json_mock = mocker.Mock(side_effect =
-        side_effect_for_get_json_failed_job(extra_links=extra_links))
+    get_json_mock = mocker.Mock(
+        side_effect=side_effect_for_get_json_failed_job(extra_links=extra_links))
     mocker.patch('harmony.harmony.Client._get_json', get_json_mock)
     client = Client(should_validate_auth=False, check_interval=0)
 
     iter = client.iterator('foo123', '/tmp')
     granule_data = next(iter)
-    assert granule_data['bbox'] == BBox(-179.95,-89.95,179.95,89.95)
+    assert granule_data['bbox'] == BBox(-179.95, -89.95, 179.95, 89.95)
     assert granule_data['path'].result() == '/tmp/fake.tif'
 
     granule_data = next(iter)
     assert granule_data['bbox'] == BBox(*extra_links[0]['bbox'])
     assert granule_data['path'].result() == '/tmp/fake2.tif'
 
     with pytest.raises(Exception) as exc_info:
@@ -1146,15 +1275,15 @@
 
 def side_effect_func_for_get_json_with_error(url: str):
     raise Exception('something bad happened')
 
 def test_iterator_retry(mocker):
     os.environ['GET_JSON_RETRY_SLEEP'] = '0'
     os.environ['GET_JSON_RETRY_LIMIT'] = '2'
-    get_json_mock = mocker.Mock(side_effect = side_effect_func_for_get_json_with_error)
+    get_json_mock = mocker.Mock(side_effect=side_effect_func_for_get_json_with_error)
     mocker.patch('harmony.harmony.Client._get_json', get_json_mock)
     client = Client(should_validate_auth=False)
 
     # first iteration in which job state is 'running' and two granules have completed
     iter = client.iterator('foo', '/tmp')
     with pytest.raises(Exception) as exc_info:
         next(iter)
@@ -1173,15 +1302,14 @@
                                  f'/{job_id}/?linktype={link_type.value}')
 
     client = Client(should_validate_auth=False)
     actual_stac_catalog_url = client.stac_catalog_url(job_id, link_type=link_type)
 
     assert actual_stac_catalog_url == expected_stac_catalog_url
 
-
 @responses.activate
 def test_read_text(mocker):
     url = 'http://www.example.com/1234'
     expected_text = '5678'
     responses.add(
         responses.GET,
         url,
@@ -1198,17 +1326,17 @@
 def test_handle_error_response_with_description_key():
     job_id = '3141592653-abcd-1234'
     collection = Collection(id='C1940468263-POCLOUD')
     request = Request(
         collection=collection,
         spatial=BBox(-107, 40, -105, 42)
     )
-    error = { 'code': 'harmony.ServerError', 'description': 'Error: Harmony had an internal issue.' }
+    error = {'code': 'harmony.ServerError', 'description': 'Error: Harmony had an internal issue.'}
     responses.add(
-        responses.GET,
+        responses.POST,
         expected_submit_url(collection.id),
         status=500,
         json=error
     )
     responses.add(
         responses.GET,
         expected_status_url(job_id),
@@ -1229,26 +1357,25 @@
         Client(should_validate_auth=False).status(job_id)
     assert str(e.value) == f"('Internal Server Error', '{error['description']}')"
 
     with pytest.raises(Exception) as e:
         Client(should_validate_auth=False).progress(job_id)
     assert str(e.value) == f"('Internal Server Error', '{error['description']}')"
 
-
 @responses.activate
 def test_handle_error_response_no_description_key():
     job_id = '3141592653-abcd-1234'
     collection = Collection(id='C1940468263-POCLOUD')
     request = Request(
         collection=collection,
         spatial=BBox(-107, 40, -105, 42)
     )
-    error = { 'unrecognizable_key': 'Some information.' }
+    error = {'unrecognizable_key': 'Some information.'}
     responses.add(
-        responses.GET,
+        responses.POST,
         expected_submit_url(collection.id),
         status=500,
         json=error
     )
     responses.add(
         responses.GET,
         expected_status_url(job_id),
@@ -1278,15 +1405,15 @@
     job_id = '3141592653-abcd-1234'
     collection = Collection(id='C1940468263-POCLOUD')
     request = Request(
         collection=collection,
         spatial=BBox(-107, 40, -105, 42)
     )
     responses.add(
-        responses.GET,
+        responses.POST,
         expected_submit_url(collection.id),
         status=500,
         body='error'
     )
     responses.add(
         responses.GET,
         expected_status_url(job_id),
@@ -1316,15 +1443,15 @@
     job_id = '3141592653-abcd-1234'
     collection = Collection(id='C1940468263-POCLOUD')
     request = Request(
         collection=collection,
         spatial=BBox(-107, 40, -105, 42)
     )
     responses.add(
-        responses.GET,
+        responses.POST,
         expected_submit_url(collection.id),
         status=500,
         json='error'
     )
     responses.add(
         responses.GET,
         expected_status_url(job_id),
@@ -1355,22 +1482,140 @@
         collection=collection,
         spatial=BBox(-107, 40, -105, 42)
     )
 
     curl_command = Client(should_validate_auth=False).request_as_curl(request)
     assert f'https://harmony.earthdata.nasa.gov/{collection.id}' \
            f'/ogc-api-coverages/1.0.0/collections/all/coverage/rangeset' in curl_command
-    assert '-X GET' in curl_command
+    assert '-X POST' in curl_command
 
 
 def test_request_as_curl_post(examples_dir):
     collection = Collection(id='C1940468263-POCLOUD')
     request = Request(
         collection=collection,
         shape=os.path.join(examples_dir, 'asf_example.json'),
         spatial=BBox(-107, 40, -105, 42)
     )
 
     curl_command = Client(should_validate_auth=False).request_as_curl(request)
     assert f'https://harmony.earthdata.nasa.gov/{collection.id}' \
            f'/ogc-api-coverages/1.0.0/collections/all/coverage/rangeset' in curl_command
     assert '-X POST' in curl_command
+
+def test_request_as_url():
+    collection = Collection(id='C1940468263-POCLOUD')
+    request = Request(
+        collection=collection,
+        spatial=BBox(-107, 40, -105, 42)
+    )
+
+    url = Client(should_validate_auth=False).request_as_url(request)
+    assert url == 'https://harmony.earthdata.nasa.gov/C1940468263-POCLOUD/ogc-api-coverages/1.0.0/collections/all/coverage/rangeset?forceAsync=true&subset=lat%2840%3A42%29&subset=lon%28-107%3A-105%29'
+
+def test_request_with_shapefile_as_url(examples_dir):
+    collection = Collection(id='C1940468263-POCLOUD')
+    request = Request(
+        collection=collection,
+        shape=os.path.join(examples_dir, 'asf_example.json'),
+        spatial=BBox(-107, 40, -105, 42)
+    )
+
+    with pytest.raises(Exception) as e:
+        Client(should_validate_auth=False).request_as_url(request)
+    assert str(e.value) == "Cannot include shapefile as URL query parameter"
+
+@responses.activate
+def test_collection_capabilities():
+    collection_id='C1940468263-POCLOUD'
+    params = {'collection_id': collection_id}
+    request = CapabilitiesRequest(collection_id=collection_id)
+    responses.add(
+        responses.GET,
+        expected_capabilities_url(params),
+        status=200,
+        json=expected_capabilities(collection_id)
+    )
+
+    result = Client(should_validate_auth=False).submit(request)
+
+    assert len(responses.calls) == 1
+    assert responses.calls[0].request is not None
+    assert responses.calls[0].request.url == expected_capabilities_url(params)
+    assert result['conceptId'] == collection_id
+    assert ('services' in result.keys())
+    assert result['capabilitiesVersion'] == '2'
+
+
+@responses.activate
+def test_collection_capabilities_with_version():
+    collection_id = 'C1940468263-POCLOUD'
+    capabilitiesVersion = '2'
+    params = {'collection_id': collection_id,
+              'capabilities_version': capabilitiesVersion}
+    request = CapabilitiesRequest(collection_id=collection_id,
+                                  capabilities_version=capabilitiesVersion)
+    responses.add(
+        responses.GET,
+        expected_capabilities_url(params),
+        status=200,
+        json=expected_capabilities(collection_id)
+    )
+
+    result = Client(should_validate_auth=False).submit(request)
+
+    assert len(responses.calls) == 1
+    assert responses.calls[0].request is not None
+    assert responses.calls[0].request.url == expected_capabilities_url(params)
+    assert result['conceptId'] == collection_id
+    assert ('services' in result.keys())
+    assert result['capabilitiesVersion'] == capabilitiesVersion
+
+@responses.activate
+def test_collection_capabilities_shortname():
+    collection_id='C1940468263-POCLOUD'
+    short_name='SMAP_RSS_L3_SSS_SMI_8DAY-RUNNINGMEAN_V4'
+    params = {'short_name': short_name}
+    request = CapabilitiesRequest(short_name=short_name)
+    responses.add(
+        responses.GET,
+        expected_capabilities_url(params),
+        status=200,
+        json=expected_capabilities(collection_id)
+    )
+
+    result = Client(should_validate_auth=False).submit(request)
+
+    assert len(responses.calls) == 1
+    assert responses.calls[0].request is not None
+    assert responses.calls[0].request.url == expected_capabilities_url(params)
+    assert result['conceptId'] == collection_id
+    assert result['shortName'] == short_name
+    assert ('services' in result.keys())
+    assert result['capabilitiesVersion'] == '2'
+
+
+@responses.activate
+def test_collection_capabilities_with_shortname_version():
+    collection_id = 'C1940468263-POCLOUD'
+    short_name='SMAP_RSS_L3_SSS_SMI_8DAY-RUNNINGMEAN_V4'
+    capabilitiesVersion = '2'
+    params = {'short_name': short_name,
+              'capabilities_version': capabilitiesVersion}
+    request = CapabilitiesRequest(short_name=short_name,
+                                  capabilities_version=capabilitiesVersion)
+    responses.add(
+        responses.GET,
+        expected_capabilities_url(params),
+        status=200,
+        json=expected_capabilities(collection_id)
+    )
+
+    result = Client(should_validate_auth=False).submit(request)
+
+    assert len(responses.calls) == 1
+    assert responses.calls[0].request is not None
+    assert responses.calls[0].request.url == expected_capabilities_url(params)
+    assert result['conceptId'] == collection_id
+    assert result['shortName'] == short_name
+    assert ('services' in result.keys())
+    assert result['capabilitiesVersion'] == capabilitiesVersion
```

### Comparing `harmony-py-0.4.9/tests/test_config.py` & `harmony_py-1756b0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `harmony-py-0.4.9/tests/test_request.py` & `harmony_py-1756b0/tests/test_request.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import datetime as dt
 
 from hypothesis import given, settings, strategies as st
 import pytest
 
-from harmony.harmony import BBox, Collection, Request, Dimension
+from harmony.harmony import BBox, Collection, BaseRequest, Request, CapabilitiesRequest, Dimension
 
 
 def test_request_has_collection_with_id():
     collection = Collection('foobar')
+    request = BaseRequest(collection=collection)
+    assert request.collection.id == 'foobar'
+    assert request.is_valid()
 
+def test_transformation_request_has_collection_with_id():
+    collection = Collection('foobar')
     request = Request(collection)
-
     assert request.collection.id == 'foobar'
 
-
 def test_request_with_only_a_collection():
     request = Request(collection=Collection('foobar'))
     assert request.is_valid()
 
 def test_request_with_skip_preview_false():
     request = Request(collection=Collection('foobar'), skip_preview=False)
     assert request.is_valid()
@@ -193,7 +196,41 @@
 
 def test_request_destination_url_error_message():
     request = Request(Collection('foo'), destination_url='http://somesite.com')
     messages = request.error_messages()
 
     assert not request.is_valid()
     assert 'Destination URL must be an S3 location' in messages
+
+def test_collection_capabilities_without_coll_identifier():
+    request = CapabilitiesRequest(capabilities_version='2')
+    messages = request.error_messages()
+
+    assert not request.is_valid()
+    assert 'Must specify either collection_id or short_name for CapabilitiesRequest' in messages
+
+def test_collection_capabilities_two_coll_identifier():
+    request = CapabilitiesRequest(collection_id='C1234-PROV',
+                                  short_name='foobar',
+                                  capabilities_version='2')
+    messages = request.error_messages()
+
+    assert not request.is_valid()
+    assert 'CapabilitiesRequest cannot have both collection_id and short_name values' in messages
+
+def test_collection_capabilities_request_coll_id():
+    request = CapabilitiesRequest(collection_id='C1234-PROV')
+    assert request.is_valid()
+
+def test_collection_capabilities_request_shortname():
+    request = CapabilitiesRequest(short_name='foobar')
+    assert request.is_valid()
+
+def test_collection_capabilities_request_coll_id_version():
+    request = CapabilitiesRequest(collection_id='C1234-PROV',
+                                  capabilities_version='2')
+    assert request.is_valid()
+
+def test_collection_capabilities_request_shortname_version():
+    request = CapabilitiesRequest(short_name='foobar',
+                                  capabilities_version='2')
+    assert request.is_valid()
```

