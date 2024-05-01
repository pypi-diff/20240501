# Comparing `tmp/acslib-0.1.7.tar.gz` & `tmp/acslib-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acslib-0.1.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "acslib-0.1.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `acslib-0.1.7.tar` & `acslib-0.1.8.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0      163 2024-04-25 17:42:34.491990 acslib-0.1.7/.coveragerc
--rw-r--r--   0        0        0      104 2024-04-25 17:42:34.491990 acslib-0.1.7/.dockerignore
--rw-r--r--   0        0        0      292 2024-04-25 17:42:34.491990 acslib-0.1.7/.editorconfig
--rw-r--r--   0        0        0      296 2024-04-25 17:42:34.491990 acslib-0.1.7/.github/pr_template.md
--rw-r--r--   0        0        0     9382 2024-04-25 17:42:34.491990 acslib-0.1.7/.github/workflows/test_publish_release..yml
--rw-r--r--   0        0        0     1388 2024-04-25 17:42:34.491990 acslib-0.1.7/.gitignore
--rw-r--r--   0        0        0       81 2024-04-25 17:42:34.491990 acslib-0.1.7/.isort.cfg
--rw-r--r--   0        0        0      875 2024-04-25 17:42:34.491990 acslib-0.1.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0      118 2024-04-25 17:42:34.491990 acslib-0.1.7/AUTHORS.md
--rw-r--r--   0        0        0      212 2024-04-25 17:42:34.491990 acslib-0.1.7/CONTRIBUTING.md
--rw-r--r--   0        0        0      473 2024-04-25 17:42:34.491990 acslib-0.1.7/Dockerfile
--rw-r--r--   0        0        0       59 2024-04-25 17:42:34.491990 acslib-0.1.7/HISTORY.md
--rw-r--r--   0        0        0     1089 2024-04-25 17:42:34.491990 acslib-0.1.7/LICENSE
--rw-r--r--   0        0        0      589 2024-04-25 17:42:34.491990 acslib-0.1.7/Makefile
--rw-r--r--   0        0        0     5171 2024-04-25 17:42:34.491990 acslib-0.1.7/README.md
--rw-r--r--   0        0        0      188 2024-04-25 17:42:34.491990 acslib-0.1.7/acslib/__init__.py
--rw-r--r--   0        0        0      218 2024-04-25 17:42:34.491990 acslib-0.1.7/acslib/base/__init__.py
--rw-r--r--   0        0        0      259 2024-04-25 17:42:34.491990 acslib-0.1.7/acslib/base/acs.py
--rw-r--r--   0        0        0      172 2024-04-25 17:42:34.491990 acslib-0.1.7/acslib/base/config.py
--rw-r--r--   0        0        0     6294 2024-04-25 17:42:34.491990 acslib-0.1.7/acslib/base/connection.py
--rw-r--r--   0        0        0      272 2024-04-25 17:42:34.491990 acslib-0.1.7/acslib/base/search.py
--rw-r--r--   0        0        0     6113 2024-04-25 17:42:34.491990 acslib-0.1.7/acslib/base/status.py
--rw-r--r--   0        0        0      322 2024-04-25 17:42:34.491990 acslib-0.1.7/acslib/ccure/__init__.py
--rw-r--r--   0        0        0      595 2024-04-25 17:42:34.491990 acslib-0.1.7/acslib/ccure/base.py
--rw-r--r--   0        0        0     2923 2024-04-25 17:42:34.491990 acslib-0.1.7/acslib/ccure/config.py
--rw-r--r--   0        0        0     7444 2024-04-25 17:42:34.491990 acslib-0.1.7/acslib/ccure/connection.py
--rw-r--r--   0        0        0    17568 2024-04-25 17:42:34.491990 acslib-0.1.7/acslib/ccure/crud.py
--rw-r--r--   0        0        0     1070 2024-04-25 17:42:34.491990 acslib-0.1.7/acslib/ccure/data_models.py
--rw-r--r--   0        0        0     1141 2024-04-25 17:42:34.491990 acslib-0.1.7/acslib/ccure/endpoints.py
--rw-r--r--   0        0        0     7674 2024-04-25 17:42:34.491990 acslib-0.1.7/acslib/ccure/filters.py
--rw-r--r--   0        0        0       36 2024-04-25 17:42:34.491990 acslib-0.1.7/acslib/ccure/tests/__init__.py
--rw-r--r--   0        0        0     1839 2024-04-25 17:42:34.491990 acslib-0.1.7/acslib/ccure/tests/conftest.py
--rw-r--r--   0        0        0     2037 2024-04-25 17:42:34.491990 acslib-0.1.7/acslib/ccure/tests/test_base.py
--rw-r--r--   0        0        0     2801 2024-04-25 17:42:34.491990 acslib-0.1.7/acslib/ccure/tests/test_config.py
--rw-r--r--   0        0        0     2111 2024-04-25 17:42:34.491990 acslib-0.1.7/acslib/ccure/tests/test_connection.py
--rw-r--r--   0        0        0     2588 2024-04-25 17:42:34.491990 acslib-0.1.7/acslib/ccure/tests/test_search.py
--rw-r--r--   0        0        0      348 2024-04-25 17:42:34.491990 acslib-0.1.7/acslib/ccure/types.py
--rw-r--r--   0        0        0       11 2024-04-25 17:42:34.491990 acslib-0.1.7/docs/api.md
--rw-r--r--   0        0        0       41 2024-04-25 17:42:34.491990 acslib-0.1.7/docs/authors.md
--rw-r--r--   0        0        0       46 2024-04-25 17:42:34.491990 acslib-0.1.7/docs/contributing.md
--rw-r--r--   0        0        0       41 2024-04-25 17:42:34.491990 acslib-0.1.7/docs/history.md
--rw-r--r--   0        0        0       42 2024-04-25 17:42:34.491990 acslib-0.1.7/docs/index.md
--rw-r--r--   0        0        0     1188 2024-04-25 17:42:34.491990 acslib-0.1.7/docs/installation.md
--rw-r--r--   0        0        0       87 2024-04-25 17:42:34.491990 acslib-0.1.7/docs/usage.md
--rw-r--r--   0        0        0       20 2024-04-25 17:42:34.491990 acslib-0.1.7/envrc_sample
--rw-r--r--   0        0        0     1949 2024-04-25 17:42:34.491990 acslib-0.1.7/mkdocs.yml
--rw-r--r--   0        0        0     1918 2024-04-25 17:42:34.491990 acslib-0.1.7/notebooks/.ipynb_checkpoints/encode_investigation-checkpoint
--rw-r--r--   0        0        0     2314 2024-04-25 17:42:34.491990 acslib-0.1.7/notebooks/.ipynb_checkpoints/encode_investigation-checkpoint.ipynb
--rw-r--r--   0        0        0    12624 2024-04-25 17:42:34.491990 acslib-0.1.7/notebooks/encode_investigation.ipynb
--rw-r--r--   0        0        0     2699 2024-04-25 17:42:34.491990 acslib-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      219 2024-04-25 17:42:34.491990 acslib-0.1.7/pytest.ini
--rw-r--r--   0        0        0      926 2024-04-25 17:42:34.491990 acslib-0.1.7/requirements/base/base.txt
--rw-r--r--   0        0        0     4618 2024-04-25 17:42:34.491990 acslib-0.1.7/requirements/dev/dev.txt
--rw-r--r--   0        0        0     6756 1970-01-01 00:00:00.000000 acslib-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      163 2024-05-01 13:37:48.327647 acslib-0.1.8/.coveragerc
+-rw-r--r--   0        0        0      104 2024-05-01 13:37:48.327647 acslib-0.1.8/.dockerignore
+-rw-r--r--   0        0        0      292 2024-05-01 13:37:48.327647 acslib-0.1.8/.editorconfig
+-rw-r--r--   0        0        0      296 2024-05-01 13:37:48.327647 acslib-0.1.8/.github/pr_template.md
+-rw-r--r--   0        0        0     9382 2024-05-01 13:37:48.327647 acslib-0.1.8/.github/workflows/test_publish_release..yml
+-rw-r--r--   0        0        0     1388 2024-05-01 13:37:48.327647 acslib-0.1.8/.gitignore
+-rw-r--r--   0        0        0       81 2024-05-01 13:37:48.327647 acslib-0.1.8/.isort.cfg
+-rw-r--r--   0        0        0      875 2024-05-01 13:37:48.327647 acslib-0.1.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      118 2024-05-01 13:37:48.327647 acslib-0.1.8/AUTHORS.md
+-rw-r--r--   0        0        0      212 2024-05-01 13:37:48.327647 acslib-0.1.8/CONTRIBUTING.md
+-rw-r--r--   0        0        0      473 2024-05-01 13:37:48.327647 acslib-0.1.8/Dockerfile
+-rw-r--r--   0        0        0       59 2024-05-01 13:37:48.327647 acslib-0.1.8/HISTORY.md
+-rw-r--r--   0        0        0     1089 2024-05-01 13:37:48.327647 acslib-0.1.8/LICENSE
+-rw-r--r--   0        0        0      589 2024-05-01 13:37:48.327647 acslib-0.1.8/Makefile
+-rw-r--r--   0        0        0     5171 2024-05-01 13:37:48.327647 acslib-0.1.8/README.md
+-rw-r--r--   0        0        0      188 2024-05-01 13:37:48.327647 acslib-0.1.8/acslib/__init__.py
+-rw-r--r--   0        0        0      218 2024-05-01 13:37:48.327647 acslib-0.1.8/acslib/base/__init__.py
+-rw-r--r--   0        0        0      259 2024-05-01 13:37:48.327647 acslib-0.1.8/acslib/base/acs.py
+-rw-r--r--   0        0        0      172 2024-05-01 13:37:48.327647 acslib-0.1.8/acslib/base/config.py
+-rw-r--r--   0        0        0     6294 2024-05-01 13:37:48.327647 acslib-0.1.8/acslib/base/connection.py
+-rw-r--r--   0        0        0      272 2024-05-01 13:37:48.327647 acslib-0.1.8/acslib/base/search.py
+-rw-r--r--   0        0        0     6113 2024-05-01 13:37:48.327647 acslib-0.1.8/acslib/base/status.py
+-rw-r--r--   0        0        0      322 2024-05-01 13:37:48.327647 acslib-0.1.8/acslib/ccure/__init__.py
+-rw-r--r--   0        0        0      595 2024-05-01 13:37:48.327647 acslib-0.1.8/acslib/ccure/base.py
+-rw-r--r--   0        0        0     2923 2024-05-01 13:37:48.327647 acslib-0.1.8/acslib/ccure/config.py
+-rw-r--r--   0        0        0     7460 2024-05-01 13:37:48.327647 acslib-0.1.8/acslib/ccure/connection.py
+-rw-r--r--   0        0        0    20500 2024-05-01 13:37:48.327647 acslib-0.1.8/acslib/ccure/crud.py
+-rw-r--r--   0        0        0     1070 2024-05-01 13:37:48.327647 acslib-0.1.8/acslib/ccure/data_models.py
+-rw-r--r--   0        0        0     1141 2024-05-01 13:37:48.327647 acslib-0.1.8/acslib/ccure/endpoints.py
+-rw-r--r--   0        0        0     7674 2024-05-01 13:37:48.327647 acslib-0.1.8/acslib/ccure/filters.py
+-rw-r--r--   0        0        0       36 2024-05-01 13:37:48.327647 acslib-0.1.8/acslib/ccure/tests/__init__.py
+-rw-r--r--   0        0        0     1839 2024-05-01 13:37:48.327647 acslib-0.1.8/acslib/ccure/tests/conftest.py
+-rw-r--r--   0        0        0     2037 2024-05-01 13:37:48.327647 acslib-0.1.8/acslib/ccure/tests/test_base.py
+-rw-r--r--   0        0        0     2801 2024-05-01 13:37:48.327647 acslib-0.1.8/acslib/ccure/tests/test_config.py
+-rw-r--r--   0        0        0     2111 2024-05-01 13:37:48.327647 acslib-0.1.8/acslib/ccure/tests/test_connection.py
+-rw-r--r--   0        0        0     2588 2024-05-01 13:37:48.327647 acslib-0.1.8/acslib/ccure/tests/test_search.py
+-rw-r--r--   0        0        0      837 2024-05-01 13:37:48.327647 acslib-0.1.8/acslib/ccure/types.py
+-rw-r--r--   0        0        0       11 2024-05-01 13:37:48.327647 acslib-0.1.8/docs/api.md
+-rw-r--r--   0        0        0       41 2024-05-01 13:37:48.327647 acslib-0.1.8/docs/authors.md
+-rw-r--r--   0        0        0       46 2024-05-01 13:37:48.327647 acslib-0.1.8/docs/contributing.md
+-rw-r--r--   0        0        0       41 2024-05-01 13:37:48.327647 acslib-0.1.8/docs/history.md
+-rw-r--r--   0        0        0       42 2024-05-01 13:37:48.327647 acslib-0.1.8/docs/index.md
+-rw-r--r--   0        0        0     1188 2024-05-01 13:37:48.327647 acslib-0.1.8/docs/installation.md
+-rw-r--r--   0        0        0       87 2024-05-01 13:37:48.327647 acslib-0.1.8/docs/usage.md
+-rw-r--r--   0        0        0       20 2024-05-01 13:37:48.327647 acslib-0.1.8/envrc_sample
+-rw-r--r--   0        0        0     1949 2024-05-01 13:37:48.327647 acslib-0.1.8/mkdocs.yml
+-rw-r--r--   0        0        0     1918 2024-05-01 13:37:48.327647 acslib-0.1.8/notebooks/.ipynb_checkpoints/encode_investigation-checkpoint
+-rw-r--r--   0        0        0     2314 2024-05-01 13:37:48.327647 acslib-0.1.8/notebooks/.ipynb_checkpoints/encode_investigation-checkpoint.ipynb
+-rw-r--r--   0        0        0    12624 2024-05-01 13:37:48.327647 acslib-0.1.8/notebooks/encode_investigation.ipynb
+-rw-r--r--   0        0        0     2699 2024-05-01 13:37:48.327647 acslib-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      219 2024-05-01 13:37:48.331647 acslib-0.1.8/pytest.ini
+-rw-r--r--   0        0        0      926 2024-05-01 13:37:48.331647 acslib-0.1.8/requirements/base/base.txt
+-rw-r--r--   0        0        0     4618 2024-05-01 13:37:48.331647 acslib-0.1.8/requirements/dev/dev.txt
+-rw-r--r--   0        0        0     6756 1970-01-01 00:00:00.000000 acslib-0.1.8/PKG-INFO
```

### Comparing `acslib-0.1.7/.github/workflows/test_publish_release..yml` & `acslib-0.1.8/.github/workflows/test_publish_release..yml`

 * *Files identical despite different names*

### Comparing `acslib-0.1.7/.gitignore` & `acslib-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `acslib-0.1.7/.pre-commit-config.yaml` & `acslib-0.1.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `acslib-0.1.7/LICENSE` & `acslib-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `acslib-0.1.7/Makefile` & `acslib-0.1.8/Makefile`

 * *Files identical despite different names*

### Comparing `acslib-0.1.7/README.md` & `acslib-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `acslib-0.1.7/acslib/base/connection.py` & `acslib-0.1.8/acslib/base/connection.py`

 * *Files identical despite different names*

### Comparing `acslib-0.1.7/acslib/base/status.py` & `acslib-0.1.8/acslib/base/status.py`

 * *Files identical despite different names*

### Comparing `acslib-0.1.7/acslib/ccure/base.py` & `acslib-0.1.8/acslib/ccure/base.py`

 * *Files identical despite different names*

### Comparing `acslib-0.1.7/acslib/ccure/config.py` & `acslib-0.1.8/acslib/ccure/config.py`

 * *Files identical despite different names*

### Comparing `acslib-0.1.7/acslib/ccure/connection.py` & `acslib-0.1.8/acslib/ccure/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,20 +171,20 @@
             Parameters:
                 data: data about the new clearance assignment
 
             Returns: list of strings representing key/value pairs
             """
             entries = []
             for key, val in data.items():
-                if isinstance(val, (int, str)):
+                if isinstance(val, (int, float, str)):
                     if prefix:
                         entries.append(f"{prefix}[{key}]={val}")
                     else:
                         entries.append(f"{key}={val}")
-                elif isinstance(val, list):
+                elif isinstance(val, (list, tuple)):
                     for i, list_item in enumerate(val):
                         if isinstance(list_item, dict):
                             entries.extend(
                                 get_form_entries(data=list_item, prefix=prefix + f"{key}[{i}]")
                             )
                         elif prefix:
                             entries.append(f"{prefix}[{key}][]={list_item}")
```

### Comparing `acslib-0.1.7/acslib/ccure/crud.py` & `acslib-0.1.8/acslib/ccure/crud.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from datetime import datetime, timezone
 import json
 from typing import Optional
 
 from acslib.base import ACSRequestData, ACSRequestResponse, status, ACSRequestException
 from acslib.base.connection import ACSRequestMethod
 from acslib.ccure.base import CcureACS
 from acslib.ccure.connection import CcureConnection
@@ -12,15 +13,15 @@
     PersonnelFilter,
 )
 from acslib.ccure.data_models import (
     ClearanceItemCreateData,
     CredentialCreateData,
     PersonnelCreateData,
 )
-from acslib.ccure.types import ClearanceItemType
+from acslib.ccure.types import ObjectType, ImageType
 
 
 class CcureAPI:
     def __init__(self, connection: Optional[CcureConnection] = None):
         self.personnel = CcurePersonnel(connection)
         self.clearance = CcureClearance(connection)
         self.credential = CcureCredential(connection)
@@ -126,14 +127,87 @@
             request_data=ACSRequestData(
                 url=self.config.base_url
                 + self.config.endpoints.DELETE_PERSONNEL.format(_id=personnel_id),
                 headers=self.connection.base_headers,
             ),
         )
 
+    def add_image(
+        self, personnel_id: int, image: str, image_name: str = "", partition_id: int = 1
+    ) -> ACSRequestResponse:
+        """
+        Set an image to a personnel object's PrimaryPortrait property
+        - `image` is base-64 encoded.
+        - `image_name` must be unique.
+        - `partition_id` refers to the partition where the personnel object is stored.
+        """
+        if not image_name:
+            timestamp = int(datetime.now(timezone.utc).timestamp())
+            image_name = f"{personnel_id}_{timestamp}"
+        request_data = {
+            "type": ObjectType.PERSONNEL.complete,
+            "ID": personnel_id,
+            "Children": [
+                {
+                    "Type": ObjectType.IMAGE.complete,
+                    "PropertyNames": [
+                        "Name",
+                        "ParentId",  # required but doesn't do anything
+                        "ImageType",
+                        "PartitionID",
+                        "Primary",
+                        "Image",
+                    ],
+                    "Propertyvalues": [
+                        image_name,
+                        personnel_id,
+                        ImageType.PORTRAIT.value,
+                        partition_id,
+                        True,  # we're only adding primary portraits
+                        image,
+                    ],
+                }
+            ],
+        }
+        return self.connection.request(
+            ACSRequestMethod.POST,
+            request_data=ACSRequestData(
+                url=self.config.base_url + self.config.endpoints.PERSIST_TO_CONTAINER,
+                data=self.connection.encode_data(request_data),
+                headers=self.connection.base_headers | self.connection.header_for_form_data,
+            ),
+        )
+
+    def get_image(self, personnel_id: int) -> Optional[str]:
+        """
+        Get the `PrimaryPortrait` property for the person with the given personnel ID.
+        The returned image is a base-64 encoded string.
+        """
+        self.logger.info(f"Getting personnel image for personnel {personnel_id}")
+        request_json = {
+            "TypeFullName": "Personnel",
+            "pageSize": self.connection.config.page_size,
+            "pageNumber": 1,
+            "DisplayProperties": ["PrimaryPortrait"],
+            "WhereClause": f"ObjectID = {personnel_id}",
+        }
+        response = self.connection.request(
+            ACSRequestMethod.POST,
+            request_data=ACSRequestData(
+                url=self.config.base_url + self.config.endpoints.FIND_OBJS_W_CRITERIA,
+                request_json=request_json,
+                headers=self.connection.base_headers,
+            ),
+        ).json
+        if response:
+            return response[0]["PrimaryPortrait"]
+        raise ACSRequestException(
+            status.HTTP_400_BAD_REQUEST, f"No personnel found with ID {personnel_id}"
+        )
+
 
 class CcureClearance(CcureACS):
     def __init__(self, connection: Optional[CcureConnection] = None):
         super().__init__(connection)
         self.search_filter = ClearanceFilter()
 
     def search(self, terms: list, search_filter: Optional[ClearanceFilter] = None) -> list:
@@ -327,15 +401,15 @@
 class CcureClearanceItem(CcureACS):
     def __init__(self, connection: Optional[CcureConnection] = None):
         super().__init__(connection)
         self.search_filter = ClearanceItemFilter()
 
     def search(
         self,
-        item_type: ClearanceItemType,
+        item_type: ObjectType,
         terms: Optional[list] = None,
         search_filter: Optional[ClearanceItemFilter] = None,
     ) -> list:
         """
         Get a list of ClearanceItem objects matching given search terms
 
         :param terms: list of search terms
@@ -357,15 +431,15 @@
                 + self.connection.config.endpoints.GET_ALL_WITH_CRITERIA,
                 request_json=request_json,
                 headers=self.connection.base_headers,
             ),
         )
         return response.json
 
-    def count(self, item_type: ClearanceItemType) -> int:
+    def count(self, item_type: ObjectType) -> int:
         """Get the total number of ClearanceItem objects"""
         request_json = {
             "TypeFullName": item_type.complete,
             "pageSize": 0,
             "CountOnly": True,
             "WhereClause": "",
         }
@@ -376,17 +450,15 @@
                 + self.connection.config.endpoints.GET_ALL_WITH_CRITERIA,
                 request_json=request_json,
                 headers=self.connection.base_headers,
             ),
         )
         return response.json
 
-    def update(
-        self, item_type: ClearanceItemType, item_id: int, update_data: dict
-    ) -> ACSRequestResponse:
+    def update(self, item_type: ObjectType, item_id: int, update_data: dict) -> ACSRequestResponse:
         """
         Edit properties of a ClearanceItem object
 
         :param item_type: specifies an item type. eg ClearanceItemType.DOOR
         :param item_id: the ClearanceItem object's CCure ID
         :param update_data: maps ClearanceItem properties to their new values
         """
@@ -403,15 +475,15 @@
                 ),
                 headers=self.connection.base_headers | self.connection.header_for_form_data,
             ),
         )
 
     def create(
         self,
-        item_type: ClearanceItemType,
+        item_type: ObjectType,
         controller_id: int,
         create_data: ClearanceItemCreateData,
     ) -> ACSRequestResponse:
         """
         Create a new clearance item object
 
         :param item_type: eg ClearanceItemType.DOOR, ClearanceItemType.ELEVATOR
@@ -435,15 +507,15 @@
             request_data=ACSRequestData(
                 url=self.config.base_url + self.config.endpoints.PERSIST_TO_CONTAINER,
                 data=self.connection.encode_data(request_data),
                 headers=self.connection.base_headers | self.connection.header_for_form_data,
             ),
         )
 
-    def delete(self, item_type: ClearanceItemType, item_id: int) -> ACSRequestResponse:
+    def delete(self, item_type: ObjectType, item_id: int) -> ACSRequestResponse:
         """Delete a ClearanceItem object by its CCure ID"""
         return self.connection.request(
             ACSRequestMethod.DELETE,
             request_data=ACSRequestData(
                 url=self.config.base_url + self.config.endpoints.DELETE_OBJECT,
                 params={"type": item_type.complete, "id": item_id},
                 headers=self.connection.base_headers,
```

### Comparing `acslib-0.1.7/acslib/ccure/data_models.py` & `acslib-0.1.8/acslib/ccure/data_models.py`

 * *Files identical despite different names*

### Comparing `acslib-0.1.7/acslib/ccure/endpoints.py` & `acslib-0.1.8/acslib/ccure/endpoints.py`

 * *Files identical despite different names*

### Comparing `acslib-0.1.7/acslib/ccure/filters.py` & `acslib-0.1.8/acslib/ccure/filters.py`

 * *Files identical despite different names*

### Comparing `acslib-0.1.7/acslib/ccure/tests/conftest.py` & `acslib-0.1.8/acslib/ccure/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `acslib-0.1.7/acslib/ccure/tests/test_base.py` & `acslib-0.1.8/acslib/ccure/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `acslib-0.1.7/acslib/ccure/tests/test_config.py` & `acslib-0.1.8/acslib/ccure/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `acslib-0.1.7/acslib/ccure/tests/test_connection.py` & `acslib-0.1.8/acslib/ccure/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `acslib-0.1.7/acslib/ccure/tests/test_search.py` & `acslib-0.1.8/acslib/ccure/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `acslib-0.1.7/docs/installation.md` & `acslib-0.1.8/docs/installation.md`

 * *Files identical despite different names*

### Comparing `acslib-0.1.7/mkdocs.yml` & `acslib-0.1.8/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `acslib-0.1.7/notebooks/.ipynb_checkpoints/encode_investigation-checkpoint` & `acslib-0.1.8/notebooks/.ipynb_checkpoints/encode_investigation-checkpoint`

 * *Files identical despite different names*

### Comparing `acslib-0.1.7/notebooks/.ipynb_checkpoints/encode_investigation-checkpoint.ipynb` & `acslib-0.1.8/notebooks/.ipynb_checkpoints/encode_investigation-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `acslib-0.1.7/notebooks/encode_investigation.ipynb` & `acslib-0.1.8/notebooks/encode_investigation.ipynb`

 * *Files identical despite different names*

### Comparing `acslib-0.1.7/pyproject.toml` & `acslib-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core>=3.2, <4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "acslib"
-version = "0.1.7"
+version = "0.1.8"
 authors = [
     { name="Jeremy Gibson", email="jmgibso3@ncsu.edu" },
     { name="Luc Sanchez", email="lgsanche@ncsu.edu" },
     { name="Ryan Semmler", email="rsemmle@ncsu.edu" },
 ]
 description = "A library for interacting with Access Control Systems like Genetec or Ccure9k"
 readme = "README.md"
```

### Comparing `acslib-0.1.7/requirements/base/base.txt` & `acslib-0.1.8/requirements/base/base.txt`

 * *Files 1% similar despite different names*

```diff
@@ -22,17 +22,17 @@
     # via sat-utils
 oracledb==1.4.1
     # via sat-utils
 pyasn1==0.5.0
     # via ldap3
 pycparser==2.21
     # via cffi
-pydantic==2.5.0
+pydantic==2.7.1
     # via acslib (pyproject.toml)
-pydantic-core==2.14.1
+pydantic-core==2.18.2
     # via pydantic
 pyodbc==4.0.39
     # via sat-utils
 requests==2.31.0
     # via sat-utils
 sat-utils==1.1.12
     # via acslib (pyproject.toml)
```

### Comparing `acslib-0.1.7/requirements/dev/dev.txt` & `acslib-0.1.8/requirements/dev/dev.txt`

 * *Files 0% similar despite different names*

```diff
@@ -143,17 +143,17 @@
     # via acslib (pyproject.toml)
 py==1.11.0
     # via pytest
 pyasn1==0.5.0
     # via ldap3
 pycparser==2.21
     # via cffi
-pydantic==2.5.0
+pydantic==2.7.1
     # via acslib (pyproject.toml)
-pydantic-core==2.14.1
+pydantic-core==2.18.2
     # via pydantic
 pygments==2.16.1
     # via
     #   acslib (pyproject.toml)
     #   mkdocs-material
     #   rich
 pymdown-extensions==10.4
```

### Comparing `acslib-0.1.7/PKG-INFO` & `acslib-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acslib
-Version: 0.1.7
+Version: 0.1.8
 Summary: A library for interacting with Access Control Systems like Genetec or Ccure9k
 Author-email: Jeremy Gibson <jmgibso3@ncsu.edu>, Luc Sanchez <lgsanche@ncsu.edu>, Ryan Semmler <rsemmle@ncsu.edu>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: pydantic>=2.5.3, <3.0.0
 Requires-Dist: sat-utils>=1.1.12, <2.0.0
 Requires-Dist: pytest>=6.2.5, <7.0.0 ; extra == "dev"
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: acslib Version: 0.1.7 Summary: A library for
+Metadata-Version: 2.1 Name: acslib Version: 0.1.8 Summary: A library for
 interacting with Access Control Systems like Genetec or Ccure9k Author-email:
 Jeremy Gibson
 ncsu.edu>, Luc Sanchez
 ncsu.edu>, Ryan Semmler
 ncsu.edu> Requires-Python: >=3.10 Description-Content-Type: text/markdown
 Requires-Dist: pydantic>=2.5.3, <3.0.0 Requires-Dist: sat-utils>=1.1.12, <2.0.0
 Requires-Dist: pytest>=6.2.5, <7.0.0 ; extra == "dev" Requires-Dist: pytest-
```

