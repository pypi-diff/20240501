# Comparing `tmp/harmony-service-lib-1.0.9.tar.gz` & `tmp/harmony_service_lib-1756b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harmony-service-lib-1.0.9.tar", last modified: Wed Jul  7 19:25:26 2021, max compression
+gzip compressed data, was "harmony_service_lib-1756b0.tar", last modified: Wed May  1 17:20:05 2024, max compression
```

## Comparing `harmony-service-lib-1.0.9.tar` & `harmony_service_lib-1756b0.tar`

### file list

```diff
@@ -1,27 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-07 19:25:26.704805 harmony-service-lib-1.0.9/
--rw-r--r--   0 runner    (1001) docker     (121)     9772 2021-07-07 19:25:15.000000 harmony-service-lib-1.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      123 2021-07-07 19:25:15.000000 harmony-service-lib-1.0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6402 2021-07-07 19:25:26.704805 harmony-service-lib-1.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5758 2021-07-07 19:25:15.000000 harmony-service-lib-1.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-07 19:25:26.704805 harmony-service-lib-1.0.9/harmony/
--rw-r--r--   0 runner    (1001) docker     (121)      276 2021-07-07 19:25:24.000000 harmony-service-lib-1.0.9/harmony/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    31484 2021-07-07 19:25:15.000000 harmony-service-lib-1.0.9/harmony/adapter.py
--rw-r--r--   0 runner    (1001) docker     (121)     7914 2021-07-07 19:25:15.000000 harmony-service-lib-1.0.9/harmony/aws.py
--rw-r--r--   0 runner    (1001) docker     (121)    12348 2021-07-07 19:25:15.000000 harmony-service-lib-1.0.9/harmony/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     3143 2021-07-07 19:25:15.000000 harmony-service-lib-1.0.9/harmony/earthdata.py
--rw-r--r--   0 runner    (1001) docker     (121)      823 2021-07-07 19:25:15.000000 harmony-service-lib-1.0.9/harmony/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    13070 2021-07-07 19:25:15.000000 harmony-service-lib-1.0.9/harmony/http.py
--rw-r--r--   0 runner    (1001) docker     (121)     2724 2021-07-07 19:25:15.000000 harmony-service-lib-1.0.9/harmony/logging.py
--rw-r--r--   0 runner    (1001) docker     (121)    17835 2021-07-07 19:25:15.000000 harmony-service-lib-1.0.9/harmony/message.py
--rw-r--r--   0 runner    (1001) docker     (121)    20645 2021-07-07 19:25:15.000000 harmony-service-lib-1.0.9/harmony/util.py
--rw-r--r--   0 runner    (1001) docker     (121)      228 2021-07-07 19:25:15.000000 harmony-service-lib-1.0.9/harmony/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-07 19:25:26.704805 harmony-service-lib-1.0.9/harmony_service_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6402 2021-07-07 19:25:26.000000 harmony-service-lib-1.0.9/harmony_service_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      541 2021-07-07 19:25:26.000000 harmony-service-lib-1.0.9/harmony_service_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-07 19:25:26.000000 harmony-service-lib-1.0.9/harmony_service_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       67 2021-07-07 19:25:26.000000 harmony-service-lib-1.0.9/harmony_service_lib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-07 19:25:26.000000 harmony-service-lib-1.0.9/harmony_service_lib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      323 2021-07-07 19:25:26.000000 harmony-service-lib-1.0.9/harmony_service_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2021-07-07 19:25:26.000000 harmony-service-lib-1.0.9/harmony_service_lib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-07-07 19:25:26.704805 harmony-service-lib-1.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2433 2021-07-07 19:25:15.000000 harmony-service-lib-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:20:05.427532 harmony_service_lib-1756b0/
+-rw-r--r--   0 runner    (1001) docker     (127)     9772 2024-05-01 17:19:57.000000 harmony_service_lib-1756b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-01 17:19:57.000000 harmony_service_lib-1756b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-05-01 17:20:05.427532 harmony_service_lib-1756b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-05-01 17:19:57.000000 harmony_service_lib-1756b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:20:05.427532 harmony_service_lib-1756b0/harmony/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-01 17:19:57.000000 harmony_service_lib-1756b0/harmony/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33175 2024-05-01 17:19:57.000000 harmony_service_lib-1756b0/harmony/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8515 2024-05-01 17:19:57.000000 harmony_service_lib-1756b0/harmony/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14174 2024-05-01 17:19:57.000000 harmony_service_lib-1756b0/harmony/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-05-01 17:19:57.000000 harmony_service_lib-1756b0/harmony/earthdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-01 17:19:57.000000 harmony_service_lib-1756b0/harmony/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16033 2024-05-01 17:19:57.000000 harmony_service_lib-1756b0/harmony/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-05-01 17:19:57.000000 harmony_service_lib-1756b0/harmony/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22433 2024-05-01 17:19:57.000000 harmony_service_lib-1756b0/harmony/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6164 2024-05-01 17:19:57.000000 harmony_service_lib-1756b0/harmony/message_utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-01 17:19:57.000000 harmony_service_lib-1756b0/harmony/s3_stac_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21561 2024-05-01 17:19:57.000000 harmony_service_lib-1756b0/harmony/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-01 17:19:57.000000 harmony_service_lib-1756b0/harmony/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:20:05.427532 harmony_service_lib-1756b0/harmony_service_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-05-01 17:20:05.000000 harmony_service_lib-1756b0/harmony_service_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-01 17:20:05.000000 harmony_service_lib-1756b0/harmony_service_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 17:20:05.000000 harmony_service_lib-1756b0/harmony_service_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-01 17:20:05.000000 harmony_service_lib-1756b0/harmony_service_lib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 17:20:05.000000 harmony_service_lib-1756b0/harmony_service_lib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-01 17:20:05.000000 harmony_service_lib-1756b0/harmony_service_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-01 17:20:05.000000 harmony_service_lib-1756b0/harmony_service_lib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 17:20:05.427532 harmony_service_lib-1756b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-05-01 17:19:57.000000 harmony_service_lib-1756b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:20:05.427532 harmony_service_lib-1756b0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    20166 2024-05-01 17:19:57.000000 harmony_service_lib-1756b0/tests/test_adapter_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-05-01 17:19:57.000000 harmony_service_lib-1756b0/tests/test_adapter_stac.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11126 2024-05-01 17:19:57.000000 harmony_service_lib-1756b0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7767 2024-05-01 17:19:57.000000 harmony_service_lib-1756b0/tests/test_cli_stac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3851 2024-05-01 17:19:57.000000 harmony_service_lib-1756b0/tests/test_earthdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15606 2024-05-01 17:19:57.000000 harmony_service_lib-1756b0/tests/test_http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-05-01 17:19:57.000000 harmony_service_lib-1756b0/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10688 2024-05-01 17:19:57.000000 harmony_service_lib-1756b0/tests/test_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19208 2024-05-01 17:19:57.000000 harmony_service_lib-1756b0/tests/test_message_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17755 2024-05-01 17:19:57.000000 harmony_service_lib-1756b0/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-05-01 17:19:57.000000 harmony_service_lib-1756b0/tests/test_util_crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6752 2024-05-01 17:19:57.000000 harmony_service_lib-1756b0/tests/test_util_download.py
```

### Comparing `harmony-service-lib-1.0.9/LICENSE` & `harmony_service_lib-1756b0/LICENSE`

 * *Files identical despite different names*

### Comparing `harmony-service-lib-1.0.9/PKG-INFO` & `harmony_service_lib-1756b0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 Metadata-Version: 2.1
 Name: harmony-service-lib
-Version: 1.0.9
+Version: 1756b0
 Summary: A library for Python-based Harmony services to parse incoming messages, fetch data, stage data, and call back to Harmony
 Home-page: https://github.com/nasa/harmony-service-lib-py
 Author: NASA EOSDIS Harmony Team
 Author-email: patrick@element84.com
 License: License :: OSI Approved :: Apache Software License
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: boto3~=1.14
+Requires-Dist: deprecation~=2.1.0
+Requires-Dist: pynacl~=1.4
+Requires-Dist: pystac~=0.5.3
+Requires-Dist: python-json-logger~=2.0.1
+Requires-Dist: requests~=2.24
+Requires-Dist: urllib3~=1.26.9
 
 # harmony-service-lib
 
 A library for Python-based Harmony services to parse incoming messages, fetch data, stage data, and call back to Harmony
 
 ## Installing
 
@@ -51,15 +56,18 @@
 result to call to one of the adapter's `#completed_with_*` methods. The adapter
 class provides helper methods for retrieving data, staging results, and cleaning
 up temporary files, though these can be overridden or ignored if a service
 needs different behavior, e.g. if it operates on data in situ and does not
 want to download the remote file.
 
 A full example of these two requirements with use of helpers can be found in
-[example/example_service.py](example/example_service.py)
+[example/example_service.py](example/example_service.py). Also see
+[adapting-new-services](https://github.com/nasa/harmony/blob/main/docs/guides/adapting-new-services.md) for in depth
+guidance on service development using this library, especially the
+[info on proper error handling](https://github.com/nasa/harmony/blob/main/docs/guides/adapting-new-services.md#5-error-handling).
 
 ## Environment
 
 The following environment variables can be used to control the behavior of the
 library and allow easier testing:
 
 REQUIRED:
@@ -106,26 +114,27 @@
        messages will be formatted as JSON.
 * `HEALTH_CHECK_PATH`: Set this to the path where the health check file should be stored. This
        file's mtime is set to the current time whenever a successful attempt is made to to read the
        message queue (whether or not a message is retrieved). This file can be used by a container's
        health check command. The container is considered unhealthy if the mtime of the file is old -
        where 'old' is configurable in the service container. If this variable is not set the path
        defaults to '/tmp/health.txt'.
+* `MAX_DOWNLOAD_RETRIES`: Number of times to retry HTTP download calls that fail due to transient errors.
 
 OPTIONAL -- Use with CAUTION:
 
 * `FALLBACK_AUTHN_ENABLED`: Default: False. Enable the fallback authentication that
   uses the EDL application credentials. See CAUTION note above.
 * `EDL_USERNAME`: The Earthdata Login username used for fallback authn.
 * `EDL_PASSWORD`: The Earthdata Login password used for fallback authn.
 
 ## Development Setup
 
 Prerequisites:
-  - Python 3.7+, ideally installed via a virtual environment
+  - Python 3.8+, ideally installed via a virtual environment
   - A local copy of the code
 
 Install dependencies:
 
     $ make install
 
 Run linter against production code:
@@ -142,9 +151,7 @@
 
 ## Releasing
 
 GitHub release notes will automatically be generated based on pull request subjects.
 Pull request subject lines should therefore concisely emphasize library
 user-facing behavior and updates they should appear in the changelog.  If more
 information is needed for release notes, note that in the PR content.
-
-
```

### Comparing `harmony-service-lib-1.0.9/README.md` & `harmony_service_lib-1756b0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -34,15 +34,18 @@
 result to call to one of the adapter's `#completed_with_*` methods. The adapter
 class provides helper methods for retrieving data, staging results, and cleaning
 up temporary files, though these can be overridden or ignored if a service
 needs different behavior, e.g. if it operates on data in situ and does not
 want to download the remote file.
 
 A full example of these two requirements with use of helpers can be found in
-[example/example_service.py](example/example_service.py)
+[example/example_service.py](example/example_service.py). Also see
+[adapting-new-services](https://github.com/nasa/harmony/blob/main/docs/guides/adapting-new-services.md) for in depth
+guidance on service development using this library, especially the
+[info on proper error handling](https://github.com/nasa/harmony/blob/main/docs/guides/adapting-new-services.md#5-error-handling).
 
 ## Environment
 
 The following environment variables can be used to control the behavior of the
 library and allow easier testing:
 
 REQUIRED:
@@ -89,26 +92,27 @@
        messages will be formatted as JSON.
 * `HEALTH_CHECK_PATH`: Set this to the path where the health check file should be stored. This
        file's mtime is set to the current time whenever a successful attempt is made to to read the
        message queue (whether or not a message is retrieved). This file can be used by a container's
        health check command. The container is considered unhealthy if the mtime of the file is old -
        where 'old' is configurable in the service container. If this variable is not set the path
        defaults to '/tmp/health.txt'.
+* `MAX_DOWNLOAD_RETRIES`: Number of times to retry HTTP download calls that fail due to transient errors.
 
 OPTIONAL -- Use with CAUTION:
 
 * `FALLBACK_AUTHN_ENABLED`: Default: False. Enable the fallback authentication that
   uses the EDL application credentials. See CAUTION note above.
 * `EDL_USERNAME`: The Earthdata Login username used for fallback authn.
 * `EDL_PASSWORD`: The Earthdata Login password used for fallback authn.
 
 ## Development Setup
 
 Prerequisites:
-  - Python 3.7+, ideally installed via a virtual environment
+  - Python 3.8+, ideally installed via a virtual environment
   - A local copy of the code
 
 Install dependencies:
 
     $ make install
 
 Run linter against production code:
```

### Comparing `harmony-service-lib-1.0.9/harmony/adapter.py` & `harmony_service_lib-1756b0/harmony/adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,29 +14,29 @@
 import logging
 import uuid
 from abc import ABC
 from tempfile import mkdtemp
 from warnings import warn
 
 from deprecation import deprecated
-from pystac import Item, Asset
+from pystac import Catalog, Item, Asset, read_file
 
 from harmony.exceptions import CanceledException
+from harmony.http import request_context
 from harmony.logging import build_logger
 from harmony.message import Temporal
 from harmony.util import touch_health_check_file
 from . import util
 
 
 class BaseHarmonyAdapter(ABC):
     """
     Abstract base class for Harmony service adapters.  Service implementations
-    should inherit from this class and implement the `#invoke(self)` method to
-    adapt the Harmony message (`self.message`) into a service call and the
-    output of the service call into a response to Harmony (`self.completed_with_*`)
+    should inherit from this class and implement the `#invoke(self)` or `#process_item(self, item, source)`
+    method to adapt the Harmony message (`self.message`) into a service call
 
     Services may choose to override methods that do data downloads and result
     staging as well, if they use a different mechanism
 
     Attributes
     ----------
     message : harmony.Message
@@ -67,14 +67,18 @@
         config : harmony.util.Config
             The configuration values for this runtime environment.
         """
         if catalog is None:
             warn('Invoking adapter.BaseHarmonyAdapter without a STAC catalog is deprecated',
                  DeprecationWarning, stacklevel=2)
 
+        # set the request ID in the global context so we can use it in other places
+        request_id = message.requestId if hasattr(message, 'requestId') else None
+        request_context['request_id'] = request_id
+
         self.message = message
         self.catalog = catalog
         self.config = config
 
         if self.config is not None:
             self.init_logging()
         else:
@@ -103,25 +107,55 @@
     def invoke(self):
         """
         Invokes the service to process `self.message`.  By default, this will call process_item
         on all items in the input catalog
 
         Returns
         -------
-        (harmony.Message, pystac.Catalog)
+        (harmony.Message, pystac.Catalog | list)
             A tuple of the Harmony message, with any processed fields marked as such and
-            a STAC catalog describing the output
+            in this implementation, a single STAC catalog describing the output.
+            (Services overriding this method may return a list of STAC catalogs if desired.)
         """
         # New-style processing using STAC
         if self.catalog:
             return (self.message, self._process_catalog_recursive(self.catalog))
 
-        # Current processing using callbacks
+        # Deprecated, processing using callbacks
         self._process_with_callbacks()
 
+    def get_all_catalog_items(self, catalog: Catalog, follow_page_links=True):
+        """
+        Returns a lazy sequence of all the items (including from child catalogs) in the catalog.
+        Can handle paged catalogs (catalogs with next/prev).
+
+        Parameters
+        ----------
+        catalog : pystac.Catalog
+            The catalog from which to get items
+        follow_page_links : boolean
+            Whether or not to follow 'next' links - defaults to True
+
+        Returns
+        -------
+        A generator that can be iterated to provide a lazy sequence of `pystac.Item`s
+        """
+        # Return immediate items and items from sub-catalogs
+        for item in catalog.get_all_items():
+            yield item
+
+        # process 'next' link if present
+        if follow_page_links:
+            link = catalog.get_single_link(rel='next')
+            if link:
+                next_catalog = read_file(link.get_href())
+                next_items = self.get_all_catalog_items(next_catalog, True)
+                for item in next_items:
+                    yield item
+
     def _process_catalog_recursive(self, catalog):
         """
         Helper method to recursively process a catalog and all of its children, producing a new
         output catalog of the results
 
         Parameters
         ----------
@@ -152,14 +186,21 @@
             output_item = self.process_item(item.clone(), source)
             if output_item:
                 # Ensure the item gets a new ID
                 if output_item.id == item.id:
                     output_item.id = str(uuid.uuid4())
                 result.add_item(output_item)
         self.logger.info(f'Processed {item_count} granule(s)')
+
+        # process 'next' link if present
+        link = catalog.get_single_link(rel='next')
+        if link:
+            next_catalog = read_file(link.get_href())
+            result.add_child(self._process_catalog_recursive(next_catalog))
+
         return result
 
     def _process_with_callbacks(self):
         """
         Method for backward compatibility with non-chaining workflows.  Takes an incoming message
         containing granules, translates the granules into STAC items, and passes them individually
         to process_item
```

### Comparing `harmony-service-lib-1.0.9/harmony/aws.py` & `harmony_service_lib-1756b0/harmony/aws.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 """
 This module includes various AWS-specific functions to stage data in S3 and deal with
 messages in SQS queues.
 
 This module relies on the harmony.util.config and its environment variables to be
 set for correct operation. See that module and the project README for details.
 """
+from urllib.parse import urlparse
+from os import environ
 import boto3
 from botocore.config import Config
+from harmony import util
 
 
 def is_s3(url: str) -> bool:
     """Predicate to determine if a url is an S3 endpoint."""
     return url is not None and url.lower().startswith('s3')
 
 
-def _aws_parameters(use_localstack, localstack_host, region):
+def aws_parameters(use_localstack, localstack_host, region):
     """Constructs a configuration dict that can be used to create an aws client.
 
     Parameters
     ----------
     use_localstack : bool
         Whether to use the localstack in this environment.
     localstack_host : str
@@ -39,14 +42,33 @@
         }
     else:
         return {
             'region_name': region
         }
 
 
+def write_s3(url, txt):
+    """
+    Writes text to the given  s3 url.
+
+    Parameters
+    ----------
+    url: The s3 file url.
+    txt: The file contents.
+    """
+    parsed = urlparse(url)
+    config = util.config(validate=environ.get('ENV') != 'test')
+    service_params = aws_parameters(
+            config.use_localstack, config.localstack_host, config.aws_default_region)
+    bucket = parsed.netloc
+    key = parsed.path[1:]
+    s3 = boto3.resource("s3", **service_params)
+    s3.Object(bucket, key).put(Body=txt)
+
+
 def _get_aws_client(config, service, user_agent=None):
     """
     Returns a boto3 client for accessing the provided service.  Accesses the service in us-west-2
     unless "AWS_DEFAULT_REGION" is set.  If the environment variable "USE_LOCALSTACK" is set to "true",
     it will return a client that will access a LocalStack instance instead of AWS.
 
     Parameters
@@ -61,15 +83,15 @@
 
     Returns
     -------
     s3_client : boto3.*.Client
         A client appropriate for accessing the provided service
     """
     boto_cfg = Config(user_agent_extra=user_agent)
-    service_params = _aws_parameters(config.use_localstack, config.localstack_host, config.aws_default_region)
+    service_params = aws_parameters(config.use_localstack, config.localstack_host, config.aws_default_region)
 
     return boto3.client(service_name=service, config=boto_cfg, **service_params)
 
 
 def download(config, url, destination_file, user_agent=None):
     """Download an S3 object to the specified destination directory.
```

### Comparing `harmony-service-lib-1.0.9/harmony/cli.py` & `harmony_service_lib-1756b0/harmony/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,20 +8,49 @@
 
 import json
 import logging
 from os import path, makedirs
 import datetime
 
 from pystac import Catalog, CatalogType
+from pystac.layout import BestPracticesLayoutStrategy
 
 from harmony.exceptions import CanceledException, HarmonyException
 from harmony.message import Message
 from harmony.logging import setup_stdout_log_formatting, build_logger
 from harmony.util import (receive_messages, delete_message, change_message_visibility,
                           config, create_decrypter)
+from harmony.version import get_version
+from harmony.aws import is_s3, write_s3
+from harmony.s3_stac_io import write
+
+
+class MultiCatalogLayoutStrategy(BestPracticesLayoutStrategy):
+    """
+    Layout that adheres to what the Harmony server expects
+    when multiple catalogs are output by a service.
+    """
+
+    def __init__(self, index):
+        self.index = index
+
+    def get_catalog_href(self, cat, parent_dir, is_root):
+        """
+        Returns the catalog href, using its index number as
+        part of the file name, e.g. s3://outputs/catalog0.json.
+
+        Parameters
+        ----------
+        parent_dir : string
+            The parent directory of the catalog
+        Returns
+        -------
+        The catalog href, postfixed with catalog{idx}.json
+        """
+        return path.join(parent_dir, f'catalog{self.index}.json')
 
 
 def setup_cli(parser):
     """
     Adds Harmony arguments to the CLI being parsed by the provided parser
 
     Parameters
@@ -138,16 +167,21 @@
     metadata_dir : string
         Directory into which the error should be written
     message : string
         The error message to write
     category : string
         The error category to write
     """
-    with open(path.join(metadata_dir, 'error.json'), 'w') as file:
-        json.dump({'error': message, 'category': category}, file)
+    error_data = {'error': message, 'category': category}
+    if is_s3(metadata_dir):
+        json_str = json.dumps(error_data)
+        write_s3(f'{metadata_dir}error.json', json_str)
+    else:
+        with open(path.join(metadata_dir, 'error.json'), 'w') as file:
+            json.dump(error_data, file)
 
 
 def _build_adapter(AdapterClass, message_string, sources_path, data_location, config):
     """
     Creates the adapter to be invoked for the given harmony input
 
     Parameters
@@ -197,20 +231,31 @@
     metadata_dir : string
         The name of the directory where STAC and message output should be written
     Returns
     -------
     True if the operation completed successfully, False otherwise
     """
     try:
-        makedirs(metadata_dir, exist_ok=True)
-        (out_message, out_catalog) = adapter.invoke()
-        out_catalog.normalize_and_save(metadata_dir, CatalogType.SELF_CONTAINED)
-
-        with open(path.join(metadata_dir, 'message.json'), 'w') as file:
-            json.dump(out_message.output_data, file)
+        logging.info(f'Invoking adapter with harmony-service-lib-py version {get_version()}')
+        is_s3_metadata_dir = is_s3(metadata_dir)
+        if not is_s3_metadata_dir:
+            makedirs(metadata_dir, exist_ok=True)
+        (out_message, stac_output) = adapter.invoke()
+        if isinstance(stac_output, list):
+            for idx, catalog in enumerate(stac_output):
+                catalog.normalize_and_save(metadata_dir, CatalogType.SELF_CONTAINED, MultiCatalogLayoutStrategy(idx))
+            json_str = json.dumps([f'catalog{i}.json' for i, c in enumerate(stac_output)])
+            write(path.join(metadata_dir, 'batch-catalogs.json'), json_str)
+            write(path.join(metadata_dir, 'batch-count.txt'), f'{len(stac_output)}')
+        else:  # assume stac_output is a single catalog
+            stac_output.normalize_and_save(metadata_dir, CatalogType.SELF_CONTAINED)
+
+        if not is_s3_metadata_dir:
+            with open(path.join(metadata_dir, 'message.json'), 'w') as file:
+                json.dump(out_message.output_data, file)
     except HarmonyException as err:
         logging.error(err, exc_info=1)
         _write_error(metadata_dir, err.message, err.category)
         raise
     except BaseException as err:
         logging.error(err, exc_info=1)
         _write_error(metadata_dir, 'Service request failed with an unknown error')
```

### Comparing `harmony-service-lib-1.0.9/harmony/earthdata.py` & `harmony_service_lib-1756b0/harmony/earthdata.py`

 * *Files identical despite different names*

### Comparing `harmony-service-lib-1.0.9/harmony/exceptions.py` & `harmony_service_lib-1756b0/harmony/exceptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,7 +22,14 @@
 
 
 class ForbiddenException(HarmonyException):
     """Class for throwing an exception indicating download failed due to not being able to access the data"""
 
     def __init__(self, message=None):
         super().__init__(message, 'Forbidden')
+
+
+class ServerException(HarmonyException):
+    """Class for throwing an exception indicating the download failed due to a generic 500 internal server error """
+
+    def __init__(self, message=None):
+        super().__init__(message, 'Server')
```

### Comparing `harmony-service-lib-1.0.9/harmony/http.py` & `harmony_service_lib-1756b0/harmony/http.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,34 +8,59 @@
 
 This module relies on the harmony.util.config and its environment variables to be
 set for correct operation. See that module and the project README for details.
 """
 
 from functools import lru_cache
 import json
-from urllib.parse import urlparse
+from time import sleep
+from urllib.parse import urlparse, parse_qs, urlencode, urlunparse
 import datetime
 import sys
 import os
 import re
 
 import requests
 
 from harmony.earthdata import EarthdataAuth, EarthdataSession
-from harmony.exceptions import ForbiddenException
+from harmony.exceptions import ServerException, ForbiddenException
 from harmony.logging import build_logger
 
 # Timeout in seconds.  Per requests docs, this is not a time limit on
 # the entire response download; rather, an exception is raised if the
 # server has not issued a response for timeout seconds (more
 # precisely, if no bytes have been received on the underlying socket
 # for timeout seconds).  See:
 # https://2.python-requests.org/en/master/user/quickstart/#timeouts
 TIMEOUT = 60
 
+MAX_RETRY_DELAY_SECS = 90
+
+# `request_context` is used to provide information about the request to functions like `download`
+# without adding extra function arguments
+request_context = {}
+
+
+def get_retry_delay(retry_num: int, max_delay: int = MAX_RETRY_DELAY_SECS) -> int:
+    """The number of seconds to sleep before retrying. Exponential backoff starting
+    from 5 seconds up the max_delay. So with a max delay of 60 the retry periods
+    would be 5, 10, 20, 40, 60, ..., 60.
+
+    Parameters
+        ----------
+        retry_num : int
+            The current number of times this request has been retried
+        max_delay: int
+            The maximum number of seconds to wait before retrying
+        Returns
+        -------
+        int : The number of seconds to wait before retrying
+    """
+    return min(max_delay, 2.5 * (2 ** retry_num))
+
 
 def is_http(url: str) -> bool:
     """Predicate to determine if the url is an http endpoint.
 
     Parameters
     ----------
     url : str
@@ -102,44 +127,58 @@
     """
     json_object = json.loads(body)
     return (f"Request could not be completed because you need to agree to the EULA "
             f"at {json_object['resolution_url']}")
 
 
 @lru_cache(maxsize=128)
-def _valid(oauth_host: str, oauth_client_id: str, access_token: str) -> bool:
-    """
-    Validates the user access token with Earthdata Login.
+def _earthdata_session():
+    """Constructs an EarthdataSession for use to download one or more files."""
+    return EarthdataSession()
 
-    Parameters
-    ----------
-    oauth_host: The Earthdata Login hostname
-    oauth_client_id: The EDL application's client id
-    access_token: The user's access token to validate
 
-    Returns
-    -------
-    Boolean indicating a valid or invalid user access token
-    """
-    url = f'{oauth_host}/oauth/tokens/user?token={access_token}&client_id={oauth_client_id}'
-    response = requests.post(url, timeout=TIMEOUT)
+def _add_api_request_uuid(url):
+    request_id = request_context.get('request_id')
 
-    if response.ok:
-        return True
+    if request_id is None:
+        return url
 
-    raise Exception(response.json())
+    # Parse the URL into components
+    parsed_url = urlparse(url)
 
+    # only add the request_id if this is an http/https url
+    if parsed_url.scheme != 'http' and parsed_url.scheme != 'https':
+        return url
 
-@lru_cache(maxsize=128)
-def _earthdata_session():
-    """Constructs an EarthdataSession for use to download one or more files."""
-    return EarthdataSession()
+    # Extract the current query parameters from the URL
+    query_params = parse_qs(parsed_url.query)
+
+    # Add or update the 'request_id' parameter
+    query_params['A-api-request-uuid'] = request_id
 
+    # Convert the query parameters back to a string
+    query_string = urlencode(query_params, doseq=True)
 
-def _download(config, url: str, access_token: str, data, user_agent=None, **kwargs_download_agent):
+    # Rebuild the URL with the new query string
+    new_url = urlunparse(
+        (parsed_url.scheme, parsed_url.netloc, parsed_url.path,
+         parsed_url.params, query_string, parsed_url.fragment)
+    )
+
+    return new_url
+
+
+def _download(
+    config, url: str,
+    access_token: str,
+    data,
+    total_retries: int,
+    logger, user_agent=None,
+    **kwargs_download_agent
+):
     """Implements the download functionality.
 
     Using the EarthdataSession and EarthdataAuth extensions to the
     `requests` module, this function will download the given url and
     perform any necessary Earthdata Login OAuth handshakes.
 
     Parameters
@@ -153,14 +192,16 @@
         and the app identity.
     data : dict or Tuple[str, str]
         Optional parameter for additional data to send to the server
         when making an HTTP POST request. These data will be URL
         encoded to a query string containing a series of `key=value`
         pairs, separated by ampersands. If None (the default), the
         request will be sent with an HTTP GET request.
+    total_retries: int
+        Upper limit on the number of times to retry the request
     user_agent : str
         The user agent that is requesting the download.
         E.g. harmony/0.0.0 (harmony-sit) harmony-service-lib/4.0 (gdal-subsetter)
     kwargs_download_agent: dict
         kwargs to be passed to the download agent
         E.g. stream=True
 
@@ -169,23 +210,60 @@
     requests.Response with the download result
 
     """
     headers = {}
     if user_agent is not None:
         headers['user-agent'] = user_agent
     auth = EarthdataAuth(config.oauth_uid, config.oauth_password, access_token)
-    with _earthdata_session() as session:
-        session.auth = auth
-        if data is None:
-            return session.get(url, headers=headers, timeout=TIMEOUT, **kwargs_download_agent)
-        else:
-            # Including this header since the stdlib does by default,
-            # but we've switched to `requests` which does not.
-            headers['Content-Type'] = 'application/x-www-form-urlencoded'
-            return session.post(url, headers=headers, data=data, timeout=TIMEOUT)
+    tries = 0
+    retry = True
+    response = None
+    while retry is True:
+        retry = False
+        tries += 1
+        try:
+            session = _earthdata_session()
+            session.auth = auth
+            if data is None:
+                response = session.get(url, headers=headers, timeout=TIMEOUT, **kwargs_download_agent)
+                if response.ok:
+                    return response
+                else:
+                    raise Exception(f'Unable to download due to status code: {response.status_code} \
+                        and content {response.content}')
+            else:
+                # Including this header since the stdlib does by default,
+                # but we've switched to `requests` which does not.
+                headers['Content-Type'] = 'application/x-www-form-urlencoded'
+                response = session.post(url, headers=headers, data=data, timeout=TIMEOUT, **kwargs_download_agent)
+                if response.ok:
+                    return response
+                else:
+                    raise Exception(f'Unable to download due to status code: {response.status_code} \
+                        and content {response.content}')
+
+        except Exception:
+            if response is not None and _is_eula_error(response.content):
+                msg = _eula_error_message(response.content)
+                logger.info(f'{msg} due to: {response.content}')
+                return response
+
+            if response is not None and response.status_code in (401, 403):
+                msg = f'Forbidden: Unable to download {url}. Will not retry.'
+                logger.info(f'{msg} due to: {response.content}')
+                return response
+
+            if tries < total_retries:
+                retry = True
+                delay = get_retry_delay(tries)
+                logger.exception(f'Retrying failed download {url}')
+                sleep(delay)
+            else:
+                logger.error(f'All retries exhaused for downloading {url}')
+                return response
 
 
 def _download_with_fallback_authn(config, url: str, data, user_agent=None, **kwargs_download_agent):
     """Downloads the given url using Basic authentication as a fallback
     mechanism should the normal EDL Oauth handshake fail.
 
     This function requires the `edl_username` and `edl_password`
@@ -200,14 +278,16 @@
         The url for the resource to download
     data : dict or Tuple[str, str]
         Optional parameter for additional data to send to the server
         when making an HTTP POST request. These data will be URL
         encoded to a query string containing a series of `key=value`
         pairs, separated by ampersands. If None (the default), the
         request will be sent with an HTTP GET request.
+    total_retries: int
+        Upper limit on the number of times to retry the request
     user_agent : str
         The user agent that is requesting the download.
         E.g. harmony/0.0.0 (harmony-sit) harmony-service-lib/4.0 (gdal-subsetter)
     kwargs_download_agent: dict
         kwargs to be passed to the download agent
         E.g. stream=True
 
@@ -216,18 +296,20 @@
     requests.Response with the download result
 
     """
     headers = {}
     if user_agent is not None:
         headers['user-agent'] = user_agent
     auth = requests.auth.HTTPBasicAuth(config.edl_username, config.edl_password)
+    session = requests.Session()
+    session.auth = auth
     if data is None:
-        return requests.get(url, headers=headers, timeout=TIMEOUT, auth=auth, **kwargs_download_agent)
+        return session.get(url, headers=headers, timeout=TIMEOUT, **kwargs_download_agent)
     else:
-        return requests.post(url, headers=headers, data=data, timeout=TIMEOUT, auth=auth)
+        return session.post(url, headers=headers, data=data, timeout=TIMEOUT)
 
 
 def _log_download_performance(logger, url, duration_ms, file_size):
     """Logs a message tracking performance information related to a file download.
 
     Parameters
     ----------
@@ -308,33 +390,38 @@
           for optimized speed and memory consumption.
           If you are experiencing some performance decay for high-throughput small-sized granules,
           you may want to set stream=False.
     """
 
     response = None
     logger = build_logger(config)
+    # Add the request ID to the download url so it can be used by Cloud Metrics
+    url = _add_api_request_uuid(url)
     start_time = datetime.datetime.now()
     logger.info(f'timing.download.start {url}')
 
     if (not stream) and buffer_size:
         logger.warn(
             f"In download paramters, buffer_size={buffer_size} will be ignored since stream is set to be {stream}."
         )
     elif stream and not isinstance(buffer_size, int):
         raise Exception(f"In download parameters: buffer_size must be integer when stream={stream}.")
 
-    if access_token is not None and _valid(config.oauth_host, config.oauth_client_id, access_token):
-        response = _download(config, url, access_token, data, user_agent, stream=stream)
+    if access_token is not None:
+        response = _download(
+            config, url, access_token, data, config.max_download_retries, logger, user_agent, stream=stream
+        )
 
     if response is None or not response.ok:
         if config.fallback_authn_enabled:
             msg = ('No valid user access token in request or EDL OAuth authentication failed.'
                    'Fallback authentication enabled: retrying with Basic auth.')
             logger.warning(msg)
-            response = _download_with_fallback_authn(config, url, data, user_agent, stream=stream)
+            response = _download_with_fallback_authn(
+                config, url, data, user_agent, stream=stream)
 
     if response.ok:
         if not stream:
             destination_file.write(response.content)
             file_size = sys.getsizeof(response.content)
         else:
             for chunk in response.iter_content(chunk_size=buffer_size):
@@ -353,13 +440,11 @@
         raise ForbiddenException(msg)
 
     if response.status_code in (401, 403):
         msg = f'Forbidden: Unable to download {url}'
         logger.info(f'{msg} due to: {response.content}')
         raise ForbiddenException(msg)
 
-    if response.status_code == 500:
-        logger.info(f'Unable to download (500) due to: {response.content}')
-        raise Exception('Unable to download.')
-
-    logger.info(f'Unable to download (unknown error) due to: {response.content}')
-    raise Exception('Unable to download: unknown error.')
+    msg = f'Unable to download due to status code: {response.status_code} and content \
+        {response.content} and all retries exhausted.'
+    logger.error(msg)
+    raise ServerException(msg)
```

### Comparing `harmony-service-lib-1.0.9/harmony/message.py` & `harmony_service_lib-1756b0/harmony/message.py`

 * *Files 10% similar despite different names*

```diff
@@ -50,14 +50,30 @@
             setattr(self, prop, data.get(prop))
         for prop in list_properties:
             Class = list_properties[prop]
             items = data.get(prop) or []
             value = [Class(item) for item in items]
             setattr(self, prop, value)
 
+    def __getitem__(self, key):
+        """
+        Retrieve the value corresponding to a key in data
+
+        Parameters
+        ----------
+        key : str
+            The key to retrieve the value for
+
+        Returns
+        -------
+        value : object or None
+            The value corresponding to the key if it exists, otherwise None
+        """
+        return self.data.get(key)
+
     def process(self, *prop):
         """
         Marks the given property as having been processed and returns its value.
         If multiple properties are passed, returns their values an array
 
         Parameters
         ----------
@@ -95,40 +111,50 @@
         finally:
             JsonObject.reprdepth -= 1
         return result
 
 
 class Source(JsonObject):
     """
-    A collection / granule / variable data source as found in the Harmony message
-    "sources" list.
+    A collection / granule / variable / coordinateVariable data source as found in
+    the Harmony message "sources" list.
 
     Attributes
     ----------
     collection : string
         The id of the collection the data source's variables and granules are in
+    shortName : string
+        The unique short name of the collection as returned by the CMR
+    versionId : string
+        The version id of the collection as returned by the CMR
     variables : list
         A list of Variable objects for the variables which should be transformed
+    coordinateVariables: list
+        A list of Variable objects containing the coordinate variables for the
+        collection.
     granules : list
         A list of Granule objects for the granules which should be operated on
     """
 
     def __init__(self, message_data):
         """
         Constructor
 
         Parameters
         ----------
         message_data : dictionary
             The Harmony message "sources" item to deserialize
         """
         super().__init__(message_data,
-                         properties=['collection'],
+                         properties=['collection', 'shortName', 'versionId'],
                          list_properties={
-                             'variables': Variable, 'granules': Granule}
+                             'variables': Variable,
+                             'coordinateVariables': Variable,
+                             'granules': Granule
+                            }
                          )
         for granule in self.granules:
             granule.collection = self.collection
             granule.variables = self.variables
 
 
 class Variable(JsonObject):
@@ -141,26 +167,70 @@
         The UMM-Var ID of the variable.
     name : string
         The UMM-Var short name of the variable, typically identifies layer name found in the
         science data file.
     fullPath : string
          The variable's absolute path within the file, including hierarchy.  Derived from
          UMM-Var group path combined with name.
+    relatedUrls : list
+         A list of RelatedUrl(s) for the variable.
     """
 
     def __init__(self, message_data):
         """
         Constructor
 
         Parameters
         ----------
         message_data : dictionary
-            The Harmony message "variables" item to deserialize
+            The Harmony message "variables" or "coordinateVariables" item to deserialize
         """
-        super().__init__(message_data, properties=['id', 'name', 'fullPath'])
+        super().__init__(
+            message_data,
+            properties=['id', 'name', 'fullPath', 'type', 'subtype'],
+            list_properties={
+                'relatedUrls': RelatedUrl
+            })
+
+
+class RelatedUrl(JsonObject):
+    """
+    A related URL describes an external resource or location on the web
+    (data access location, project home page, relevant software packages, etc.)
+
+    Attributes
+    ----------
+    url : string
+        Points to the location of the resource described by the RelatedUrl.
+    urlContentType : string
+        A keyword which describes the content of a link at a high level.
+    type : string
+        A keyword which specifies the content of a link.
+    subtype : string
+        A keyword which further specifies the content of a link.
+    description : string
+        Explains where the link navigates and the type of information it contains.
+    format : string
+        The format of the data.
+    mimeType : string
+        The mime type of the data.
+    """
+
+    def __init__(self, message_data):
+        """
+        Constructor
+
+        Parameters
+        ----------
+        message_data : dictionary
+            The Harmony message "relatedUrls" item to deserialize
+        """
+        super().__init__(message_data, properties=[
+            'url', 'urlContentType', 'type', 'subtype', 'description', 'format', 'mimeType']
+        )
 
 
 class Granule(JsonObject):
     """
     A science granule as found in a Harmony source's "granules" list
 
     Attributes
@@ -218,14 +288,42 @@
         ----------
         message_data : dictionary
             The Harmony message "format.scaleExtent.[x|y]" object to deserialize
         """
         super().__init__(message_data, properties=['min', 'max'])
 
 
+class Dimension(JsonObject):
+    """
+    Dimension subset parameters as found in a single dimension from the list of the
+    Harmony message's "subset.dimensions" field.
+
+    Attributes
+    ----------
+    name: string
+        The name of the dimension
+    min: float
+        The min value for the dimension
+    max: float
+        The max value for the dimension
+    """
+
+    def __init__(self, message_data):
+        """
+        Constructor
+
+        Parameters
+        ----------
+        message_data : dictionary
+            A single dimension from the list of the Harmony message's "subset.dimensions"
+            field
+        """
+        super().__init__(message_data, properties=['name', 'min', 'max'])
+
+
 class ScaleExtent(JsonObject):
     """
     Scale extent parameters as found in a Harmony message's "format.scaleExtent" object
 
     Attributes
     ----------
     x: message.MinMax
@@ -388,28 +486,38 @@
     Subsetting parameters as found in a Harmony message's "subset" object
 
     Attributes
     ----------
     bbox : list
         A list of 4 floating point values corresponding to [West, South, East, North]
         coordinates
+    point: list containing 2 floating point values corresponding to longitude and latitude
+    shape: RemoteResource
+        A reference to a location containing a shapefile
+    dimensions: list
+        A list of Dimension objects to subset against
     """
 
     def __init__(self, message_data):
         """
         Constructor
 
         Parameters
         ----------
         message_data : dictionary
             The Harmony message "subset" object to deserialize
         """
-        super().__init__(message_data, properties=['bbox', 'shape'])
+        super().__init__(message_data, properties=['bbox', 'point', 'shape', 'dimensions'])
         if self.shape is not None:
             self.shape = RemoteResource(message_data['shape'])
+        if self.dimensions is not None:
+            dimensions = []
+            for dimension in self.dimensions:
+                dimensions.append(Dimension(dimension))
+            self.dimensions = dimensions
 
 
 class Temporal(JsonObject):
     """
     Temporal subsetting parameters as found in a Harmony message's "temporal" object
 
     Attributes
@@ -436,14 +544,33 @@
         super().__init__(message_data or {}, properties=['start', 'end'])
         if start is not None:
             self.start = start
         if end is not None:
             self.end = end
 
 
+class ExtraArgs(JsonObject):
+    """
+    Extra Args parameters as found in a Harmony message's "extraArgs" object
+    The value of extra args parameter can be retrieved via ['<parameter>'],
+    e.g. message.extraArgs['cut'] will return the value of 'cut' parameter in extraArgs.
+    """
+
+    def __init__(self, message_data):
+        """
+        Constructor
+
+        Parameters
+        ----------
+        message_data : dictionary
+            The Harmony message "extraArgs" object to deserialize
+        """
+        super().__init__(message_data)
+
+
 class Message(JsonObject):
     """
     Top-level object corresponding to an incoming Harmony message.  Constructing
     this with a JSON string will deserialize the message into native Python object,
     perform any necessary version interpretation, and add some helpers to make access
     easier.  Generally, this object should be created and allowed to produce its
     child objects rather than directly instantiating Subset, Format, etc objects.
@@ -483,14 +610,22 @@
         service invocations.
     format: message.Format
         The Harmony message's output parameters
     subset: message.Subset
         The Harmony message's subsetting parameters
     temporal: message.Temporal
         The Harmony message's temporal subsetting parameters
+    concatenate: bool
+        True if the service should concatenate multiple input files into a single output
+        file and false otherwise.
+    extendDimensions: list
+        A list of dimensions to extend.
+    extraArgs: object
+        A map of key (string type) and value (any type) pairs indicating the extra arguments
+        that should be passed to the worker command
     """
 
     def __init__(self, json_str_or_dict, decrypter=lambda x: x):
         """
         Builds a Message object and all of its child objects by deserializing the
         provided JSON string and performing any necessary version interpretation.
 
@@ -516,29 +651,34 @@
                 'isSynchronous',
                 'user',
                 'accessToken',
                 'client',
                 'requestId',
                 'format',
                 'subset',
-                'temporal'
+                'temporal',
+                'concatenate',
+                'extendDimensions',
+                'extraArgs'
             ],
             list_properties={'sources': Source}
         )
 
         self.decrypter = decrypter
 
         if self.format is not None:
             self.format = Format(json_obj['format'])
         if self.subset is not None:
             self.subset = Subset(json_obj['subset'])
         if self.temporal is not None:
             self.temporal = Temporal(json_obj['temporal'])
         if self.accessToken is not None:
             self.accessToken = self.decrypter(self.accessToken)
+        if self.extraArgs is not None:
+            self.extraArgs = ExtraArgs(json_obj['extraArgs'])
 
     @property
     def json(self):
         return json.dumps(self.output_data)
 
     def digest(self):
         """
```

### Comparing `harmony-service-lib-1.0.9/harmony/util.py` & `harmony_service_lib-1756b0/harmony/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     AWS_DEFAULT_REGION: The AWS region in which the S3 client is operating (default: "us-west-2")
 
 Required when staging to S3 and not using the Harmony-provided stagingLocation prefix:
     STAGING_BUCKET: The bucket where staged files should be placed
     STAGING_PATH: The base path under which staged files should be placed
 
 Required when using HTTPS, allowing Earthdata Login auth:
-    OAUTH_HOST:     The Earthdata Login (EDL) environment to connect to
+    OAUTH_HOST:         The Earthdata Login (EDL) environment to connect to
     OAUTH_CLIENT_ID:    The EDL application client id used to acquire an EDL shared access token
     OAUTH_UID:          The EDL application UID used to acquire an EDL shared access token
     OAUTH_PASSWORD:     The EDL application password used to acquire an EDL shared access token
     OAUTH_REDIRECT_URI: A valid redirect URI for the EDL application (NOTE: the redirect URI is
                         not followed or used; it does need to be in the app's redirect URI list)
 
 Always provided by newer versions of the Harmony frontend:
@@ -38,29 +38,31 @@
 Optional when reading from or staging to S3:
     USE_LOCALSTACK:  'true' if the S3 client should connect to a LocalStack instance instead of
                      Amazon S3 (for testing)
     LOCALSTACK_HOST: The hostname of the Localstack to connect to if `USE_LOCALSTACK`.
     BACKEND_HOST:    The hostname of the Harmony backend. Deprecated / unused by this package.
 
 Optional:
-    APP_NAME:          A name for the service that will appear in log entries.
-    ENV:               The application environment. One of: dev, test. Used for local development.
-    TEXT_LOGGER:       Whether to log in plaintext or JSON. Default: True (plaintext).
-    HEALTH_CHECK_PATH: The filesystem path that should be `touch`ed to indicate the service is
-                       alive.
+    APP_NAME:             A name for the service that will appear in log entries.
+    ENV:                  The application environment. One of: dev, test. Used for local development.
+    TEXT_LOGGER:          Whether to log in plaintext or JSON. Default: True (plaintext).
+    HEALTH_CHECK_PATH:    The filesystem path that should be `touch`ed to indicate the service is
+                          alive.
+    MAX_DOWNLOAD_RETRIES: Number of times to retry HTTP download calls that fail due to transient errors.
 """
 
 from base64 import b64decode
 from collections import namedtuple
 from functools import lru_cache
 import hashlib
 import logging
 from pathlib import Path, PurePath
 from os import environ, path
 import sys
+import re
 from urllib import parse
 
 from nacl.secret import SecretBox
 
 from harmony import aws
 from harmony import http
 # The following imports are for backwards-compatibility for services
@@ -92,30 +94,32 @@
         'aws_default_region',
         'staging_path',
         'staging_bucket',
         'env',
         'text_logger',
         'health_check_path',
         'shared_secret_key',
-        'user_agent'
+        'user_agent',
+        'max_download_retries'
     ])
 
 
 def _validated_config(config):
     """Validates that the given Config has values for all required
     variables and returns it if so. Raises an Exception if invalid.
     """
     required = [
         'shared_secret_key',
         'oauth_client_id',
         'oauth_uid',
         'oauth_password',
         'oauth_redirect_uri',
         'staging_path',
-        'staging_bucket'
+        'staging_bucket',
+        'max_download_retries'
     ]
 
     unset = [var.upper() for var in required if getattr(config, var) is None]
 
     # Conditionally required
     if config.fallback_authn_enabled and getattr(config, 'edl_username') is None:
         unset.append("EDL_USERNAME")
@@ -157,14 +161,18 @@
         value = environ.get(name, default)
         return value.strip('\"') if value is not None else None
 
     def bool_envvar(name: str, default: bool) -> bool:
         value = environ.get(name)
         return str.lower(value) == 'true' if value is not None else default
 
+    def int_envvar(name: str, default: int) -> int:
+        value = environ.get(name)
+        return int(value) if value is not None else default
+
     oauth_redirect_uri = str_envvar('OAUTH_REDIRECT_URI', None)
     if oauth_redirect_uri is not None:
         oauth_redirect_uri = parse.quote(oauth_redirect_uri)
     backend_host = str_envvar('BACKEND_HOST', 'localhost')
     localstack_host = str_envvar('LOCALSTACK_HOST', backend_host)
 
     config = Config(
@@ -183,15 +191,16 @@
         aws_default_region=str_envvar('AWS_DEFAULT_REGION', 'us-west-2'),
         staging_path=str_envvar('STAGING_PATH', None),
         staging_bucket=str_envvar('STAGING_BUCKET', None),
         env=str_envvar('ENV', ''),
         text_logger=bool_envvar('TEXT_LOGGER', False),
         health_check_path=str_envvar('HEALTH_CHECK_PATH', '/tmp/health.txt'),
         shared_secret_key=str_envvar('SHARED_SECRET_KEY', DEFAULT_SHARED_SECRET_KEY),
-        user_agent=str_envvar('USER_AGENT', 'harmony (unknown version)')
+        user_agent=str_envvar('USER_AGENT', 'harmony (unknown version)'),
+        max_download_retries=int_envvar('MAX_DOWNLOAD_RETRIES', 0)
     )
 
     if validate:
         return _validated_config(config)
     else:
         return config
 
@@ -505,42 +514,57 @@
             The output filename
     """
     url = filename
     # Get everything between the last non-trailing '/' before the query and the first '?'
     # Do this instead of using a URL parser, because our URLs are not complex in practice and
     # it is useful to allow relative file paths to work for local testing.
     original_filename = url.split('?')[0].rstrip('/').split('/')[-1]
-    (original_basename, original_ext) = path.splitext(original_filename)
+    decoded_original_filename = parse.unquote(original_filename)
+    (original_basename, original_ext) = path.splitext(decoded_original_filename)
     if ext is None:
         ext = original_ext
 
     if not ext.startswith('.'):
         ext = '.' + ext
 
     suffixes = []
     if variable_subset and len(variable_subset) == 1:
         var = variable_subset[0]
         if hasattr(var, 'name'):
             var = var.name
-        suffixes.append('_' + var.replace('/', '_'))
+        suffixes.append('_' + var)
     if is_regridded:
         suffixes.append('_regridded')
     if is_subsetted:
         suffixes.append('_subsetted')
     suffixes.append(ext)
 
     result = original_basename
     # Iterate suffixes in reverse, removing them from the result if they're at the end of the string
     # This supports the case of chaining where one service regrids and another subsets but we don't
     # want names to get mangled
     for suffix in suffixes[::-1]:
         if result.endswith(suffix):
             result = result[:-len(suffix)]
 
-    return result + "".join(suffixes)
+    result += "".join(suffixes)
+
+    # replace special chars that may have been encoded or present in variable_subset
+    result = re.sub('\\/|:', '_', result)
+
+    # runs of underscores are replaced with single underscore
+    result = re.sub(r'_{2,}', '_', result)
+
+    # leading or trailing underscores are removed
+    result = re.sub(r'^_+|_+$', '', result)
+
+    # underscores before or after periods are removed
+    result = re.sub(r'_{0,}\._{0,}', '.', result)
+
+    return result
 
 
 def bbox_to_geometry(bbox):
     '''
     Creates a GeoJSON geometry given a GeoJSON BBox, accounting for antimeridian
 
     Parameters
```

### Comparing `harmony-service-lib-1.0.9/harmony_service_lib.egg-info/PKG-INFO` & `harmony_service_lib-1756b0/harmony_service_lib.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 Metadata-Version: 2.1
 Name: harmony-service-lib
-Version: 1.0.9
+Version: 1756b0
 Summary: A library for Python-based Harmony services to parse incoming messages, fetch data, stage data, and call back to Harmony
 Home-page: https://github.com/nasa/harmony-service-lib-py
 Author: NASA EOSDIS Harmony Team
 Author-email: patrick@element84.com
 License: License :: OSI Approved :: Apache Software License
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: boto3~=1.14
+Requires-Dist: deprecation~=2.1.0
+Requires-Dist: pynacl~=1.4
+Requires-Dist: pystac~=0.5.3
+Requires-Dist: python-json-logger~=2.0.1
+Requires-Dist: requests~=2.24
+Requires-Dist: urllib3~=1.26.9
 
 # harmony-service-lib
 
 A library for Python-based Harmony services to parse incoming messages, fetch data, stage data, and call back to Harmony
 
 ## Installing
 
@@ -51,15 +56,18 @@
 result to call to one of the adapter's `#completed_with_*` methods. The adapter
 class provides helper methods for retrieving data, staging results, and cleaning
 up temporary files, though these can be overridden or ignored if a service
 needs different behavior, e.g. if it operates on data in situ and does not
 want to download the remote file.
 
 A full example of these two requirements with use of helpers can be found in
-[example/example_service.py](example/example_service.py)
+[example/example_service.py](example/example_service.py). Also see
+[adapting-new-services](https://github.com/nasa/harmony/blob/main/docs/guides/adapting-new-services.md) for in depth
+guidance on service development using this library, especially the
+[info on proper error handling](https://github.com/nasa/harmony/blob/main/docs/guides/adapting-new-services.md#5-error-handling).
 
 ## Environment
 
 The following environment variables can be used to control the behavior of the
 library and allow easier testing:
 
 REQUIRED:
@@ -106,26 +114,27 @@
        messages will be formatted as JSON.
 * `HEALTH_CHECK_PATH`: Set this to the path where the health check file should be stored. This
        file's mtime is set to the current time whenever a successful attempt is made to to read the
        message queue (whether or not a message is retrieved). This file can be used by a container's
        health check command. The container is considered unhealthy if the mtime of the file is old -
        where 'old' is configurable in the service container. If this variable is not set the path
        defaults to '/tmp/health.txt'.
+* `MAX_DOWNLOAD_RETRIES`: Number of times to retry HTTP download calls that fail due to transient errors.
 
 OPTIONAL -- Use with CAUTION:
 
 * `FALLBACK_AUTHN_ENABLED`: Default: False. Enable the fallback authentication that
   uses the EDL application credentials. See CAUTION note above.
 * `EDL_USERNAME`: The Earthdata Login username used for fallback authn.
 * `EDL_PASSWORD`: The Earthdata Login password used for fallback authn.
 
 ## Development Setup
 
 Prerequisites:
-  - Python 3.7+, ideally installed via a virtual environment
+  - Python 3.8+, ideally installed via a virtual environment
   - A local copy of the code
 
 Install dependencies:
 
     $ make install
 
 Run linter against production code:
@@ -142,9 +151,7 @@
 
 ## Releasing
 
 GitHub release notes will automatically be generated based on pull request subjects.
 Pull request subject lines should therefore concisely emphasize library
 user-facing behavior and updates they should appear in the changelog.  If more
 information is needed for release notes, note that in the PR content.
-
-
```

### Comparing `harmony-service-lib-1.0.9/setup.py` & `harmony_service_lib-1756b0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,19 +53,20 @@
     keywords=[],
     scripts=[],
     entry_points={
         "console_scripts": ["harmony-service-lib=harmony.cli.__main__:main"]
     },
     zip_safe=False,
     install_requires=DEPENDENCIES,
-    extras_require={
-        'dev': DEV_DEPENDENCIES
-    },
+    # HARMONY-1188 - uncomment this
+    # extras_require={
+    #     'dev': DEV_DEPENDENCIES
+    # },
     test_suite="tests",
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     # license and classifier list:
     # https://pypi.org/pypi?%3Aaction=list_classifiers
     license="License :: OSI Approved :: Apache Software License",
     classifiers=[
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent"
```

