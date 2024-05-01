# Comparing `tmp/sw_product_lib-0.8.9.tar.gz` & `tmp/sw_product_lib-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sw_product_lib-0.8.9.tar", max compression
+gzip compressed data, was "sw_product_lib-0.9.0.tar", max compression
```

## Comparing `sw_product_lib-0.8.9.tar` & `sw_product_lib-0.9.0.tar`

### file list

```diff
@@ -1,19 +1,24 @@
--rw-r--r--   0        0        0     1010 2024-03-21 02:43:39.472758 sw_product_lib-0.8.9/pyproject.toml
--rw-r--r--   0        0        0       87 2024-03-21 02:43:39.472758 sw_product_lib-0.8.9/sw_product_lib/__init__.py
--rw-r--r--   0        0        0        0 2024-03-21 02:43:39.472758 sw_product_lib-0.8.9/sw_product_lib/apps/__init__.py
--rw-r--r--   0        0        0        0 2024-03-21 02:43:39.476758 sw_product_lib-0.8.9/sw_product_lib/apps/admin/__init__.py
--rw-r--r--   0        0        0     4784 2024-03-21 02:43:39.476758 sw_product_lib-0.8.9/sw_product_lib/apps/admin/backend.py
--rw-r--r--   0        0        0     2504 2024-03-21 02:43:39.476758 sw_product_lib-0.8.9/sw_product_lib/apps/admin/status.py
--rw-r--r--   0        0        0        0 2024-03-21 02:43:39.476758 sw_product_lib-0.8.9/sw_product_lib/client/__init__.py
--rw-r--r--   0        0        0     2953 2024-03-21 02:43:39.476758 sw_product_lib-0.8.9/sw_product_lib/client/backend.py
--rw-r--r--   0        0        0     3885 2024-03-21 02:43:39.476758 sw_product_lib-0.8.9/sw_product_lib/client/billing.py
--rw-r--r--   0        0        0     7097 2024-03-21 02:43:39.476758 sw_product_lib-0.8.9/sw_product_lib/client/job.py
--rw-r--r--   0        0        0     2186 2024-03-21 02:43:39.476758 sw_product_lib-0.8.9/sw_product_lib/client/resource.py
--rw-r--r--   0        0        0        0 2024-03-21 02:43:39.476758 sw_product_lib-0.8.9/sw_product_lib/platform/__init__.py
--rw-r--r--   0        0        0      331 2024-03-21 02:43:39.476758 sw_product_lib-0.8.9/sw_product_lib/platform/gql.py
--rw-r--r--   0        0        0    33154 2024-03-21 02:43:39.476758 sw_product_lib-0.8.9/sw_product_lib/service.py
--rw-r--r--   0        0        0     9932 2024-03-21 02:43:39.476758 sw_product_lib-0.8.9/sw_product_lib/types/backend.py
--rw-r--r--   0        0        0     2416 2024-03-21 02:43:39.476758 sw_product_lib-0.8.9/sw_product_lib/types/batch_job.py
--rw-r--r--   0        0        0    23981 2024-03-21 02:43:39.476758 sw_product_lib-0.8.9/sw_product_lib/types/job.py
--rw-r--r--   0        0        0     8871 2024-03-21 02:43:39.476758 sw_product_lib-0.8.9/sw_product_lib/types/resource.py
--rw-r--r--   0        0        0      759 1970-01-01 00:00:00.000000 sw_product_lib-0.8.9/PKG-INFO
+-rw-r--r--   0        0        0     1035 2024-05-01 18:31:35.035625 sw_product_lib-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      246 2024-05-01 18:31:35.035625 sw_product_lib-0.9.0/sw_product_lib/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-01 18:31:35.035625 sw_product_lib-0.9.0/sw_product_lib/apps/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-01 18:31:35.035625 sw_product_lib-0.9.0/sw_product_lib/apps/admin/__init__.py
+-rw-r--r--   0        0        0     4784 2024-05-01 18:31:35.035625 sw_product_lib-0.9.0/sw_product_lib/apps/admin/backend.py
+-rw-r--r--   0        0        0     2509 2024-05-01 18:31:35.039626 sw_product_lib-0.9.0/sw_product_lib/apps/admin/status.py
+-rw-r--r--   0        0        0       19 2024-05-01 18:31:35.039626 sw_product_lib-0.9.0/sw_product_lib/apps/auth/__init__.py
+-rw-r--r--   0        0        0     1940 2024-05-01 18:31:35.039626 sw_product_lib-0.9.0/sw_product_lib/apps/auth/gcp.py
+-rw-r--r--   0        0        0     1926 2024-05-01 18:31:35.039626 sw_product_lib-0.9.0/sw_product_lib/apps/auth/sw_proxy.py
+-rw-r--r--   0        0        0        0 2024-05-01 18:31:35.039626 sw_product_lib-0.9.0/sw_product_lib/client/__init__.py
+-rw-r--r--   0        0        0     2953 2024-05-01 18:31:35.039626 sw_product_lib-0.9.0/sw_product_lib/client/backend.py
+-rw-r--r--   0        0        0     3885 2024-05-01 18:31:35.039626 sw_product_lib-0.9.0/sw_product_lib/client/billing.py
+-rw-r--r--   0        0        0     7097 2024-05-01 18:31:35.039626 sw_product_lib-0.9.0/sw_product_lib/client/job.py
+-rw-r--r--   0        0        0     2186 2024-05-01 18:31:35.039626 sw_product_lib-0.9.0/sw_product_lib/client/resource.py
+-rw-r--r--   0        0        0        0 2024-05-01 18:31:35.039626 sw_product_lib-0.9.0/sw_product_lib/platform/__init__.py
+-rw-r--r--   0        0        0      331 2024-05-01 18:31:35.039626 sw_product_lib-0.9.0/sw_product_lib/platform/gql.py
+-rw-r--r--   0        0        0    35187 2024-05-01 18:31:35.039626 sw_product_lib-0.9.0/sw_product_lib/service.py
+-rw-r--r--   0        0        0     9932 2024-05-01 18:31:35.039626 sw_product_lib-0.9.0/sw_product_lib/types/backend.py
+-rw-r--r--   0        0        0     2416 2024-05-01 18:31:35.039626 sw_product_lib-0.9.0/sw_product_lib/types/batch_job.py
+-rw-r--r--   0        0        0    23748 2024-05-01 18:31:35.039626 sw_product_lib-0.9.0/sw_product_lib/types/job.py
+-rw-r--r--   0        0        0     8902 2024-05-01 18:31:35.039626 sw_product_lib-0.9.0/sw_product_lib/types/resource.py
+-rw-r--r--   0        0        0        0 2024-05-01 18:31:35.039626 sw_product_lib-0.9.0/sw_product_lib/utils/__init__.py
+-rw-r--r--   0        0        0      636 2024-05-01 18:31:35.039626 sw_product_lib-0.9.0/sw_product_lib/utils/jwt_utils.py
+-rw-r--r--   0        0        0      805 1970-01-01 00:00:00.000000 sw_product_lib-0.9.0/PKG-INFO
```

### Comparing `sw_product_lib-0.8.9/pyproject.toml` & `sw_product_lib-0.9.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -9,26 +9,27 @@
 
 [tool.flake8]
 max-line-length = 88
 per-file-ignores = ["__init__.py:F401", "./docs/*:E402"]
 
 [tool.poetry]
 name = "sw-product-lib"
-version = "0.8.9"
+version = "0.9.0"
 description = "Python library for Strangeworks products to interact with the Strangeworks Platform"
 authors = ["Strangeworks Devs <hello@strangeworks.com>"]
 license = "Apache-2.0"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 gql = "^3.4.1"
 fastapi = "^0.104.0"
 python-jose = { extras = ["cryptography"], version = "^3.3.0" }
-strangeworks-core = "^0.3.8"
+strangeworks-core = "^0.3.10"
 deprecated = "^1.2.13"
+google-auth = "^2.29.0"
 
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^5.0.4"
 pre-commit = "^2.20.0"
 types-requests = "^2.28.10"
 Flake8-pyproject = "^1.1.0"
```

### Comparing `sw_product_lib-0.8.9/sw_product_lib/apps/admin/backend.py` & `sw_product_lib-0.9.0/sw_product_lib/apps/admin/backend.py`

 * *Files identical despite different names*

### Comparing `sw_product_lib-0.8.9/sw_product_lib/apps/admin/status.py` & `sw_product_lib-0.9.0/sw_product_lib/apps/admin/status.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Status Update objects and function types."""
 from abc import ABC, abstractmethod
-from typing import Callable
+from typing import Any, Callable
 
 from pydantic import BaseModel
 from strangeworks_core.types.backend import Status as BackendStatus
 
 
 """Status Converter.
 
@@ -17,15 +17,15 @@
     remote status of object.
 
 Return
 ------
 : Any
     A Strangeworks platform status type.
 """
-StatusConverter = Callable[[str | dict], any]
+StatusConverter = Callable[[str | dict], Any]
 
 
 class BaseStatusUpdate(BaseModel, ABC):
     """Base class represending a status update for a remote object."""
 
     remote_id: str
     remote_status: str | dict
```

### Comparing `sw_product_lib-0.8.9/sw_product_lib/client/backend.py` & `sw_product_lib-0.9.0/sw_product_lib/client/backend.py`

 * *Files identical despite different names*

### Comparing `sw_product_lib-0.8.9/sw_product_lib/client/billing.py` & `sw_product_lib-0.9.0/sw_product_lib/client/billing.py`

 * *Files identical despite different names*

### Comparing `sw_product_lib-0.8.9/sw_product_lib/client/job.py` & `sw_product_lib-0.9.0/sw_product_lib/client/job.py`

 * *Files identical despite different names*

### Comparing `sw_product_lib-0.8.9/sw_product_lib/client/resource.py` & `sw_product_lib-0.9.0/sw_product_lib/client/resource.py`

 * *Files identical despite different names*

### Comparing `sw_product_lib-0.8.9/sw_product_lib/service.py` & `sw_product_lib-0.9.0/sw_product_lib/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 """product.py."""
-
 import json
 import tempfile
 from dataclasses import dataclass
 from functools import singledispatch
 from pathlib import Path
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
 import requests
 from deprecated import deprecated
 from fastapi import Request
-from jose import jwt
 from strangeworks_core.config.config import Config
 from strangeworks_core.errors.error import StrangeworksError
 from strangeworks_core.platform import auth
 from strangeworks_core.platform.gql import API, APIInfo
 from strangeworks_core.types.batch import Options
 from strangeworks_core.types.func import Func
 from strangeworks_core.types.job import Status as JobStatus
 from strangeworks_core.types.machine import Accelerator, Machine
 
+from sw_product_lib.apps.auth import sw_proxy
 from sw_product_lib.client import billing
 from sw_product_lib.client.billing import BillingTransaction
 from sw_product_lib.platform.gql import ProductAPI
 from sw_product_lib.types import backend, batch_job, job, resource
 from sw_product_lib.types.job import AppliedJobTag, File, Job
 from sw_product_lib.types.resource import Resource
 
+from . import in_dev_mode
+
 
 DEFAULT_PLATFORM_BASE_URL = "https://api.strangeworks.com"
 
 
 _cfg = Config(use_namespace=False)
 
 
@@ -42,31 +43,46 @@
         if _api_key and _base_url
         else None
     )
 
 
 @dataclass
 class ServiceContext:
-    """Base Context for Product Lib Requests."""
+    """Base Context for Product Lib Requests.
+
+    The Context object encapsulates items needed to make calls to the Product API. The
+    attributes of the class are typically extracted from the JWT token sent as a part
+    of the request from the platform. For system-level requests (requests whose URL
+    does not have a resource slug and only has a product slug), the service request has
+    the product slug as well as an API connection. For user requests (requests whose URL
+    includes a resource slug), the RequestContext object should be used.
+    """
 
     product_slug: str
     product_api_key: str | None = None
     api: ProductAPI | None = None
 
     def __init__(
         self,
         product_slug: str,
         product_api_key: str | None = None,
         api: ProductAPI | None = None,
+        base_url: str | None = None,
     ):
         self.product_slug = product_slug
         self.product_api_key = product_api_key or _cfg.get("PRODUCT_LIB_API_KEY")
-        self.api = api or _api(
-            api_key=self.product_api_key,
+        self.api = api or _api(api_key=self.product_api_key, url=base_url)
+
+    @classmethod
+    def from_request(cls, request: Request):
+        """Generate Service Context from request."""
+        claims, _ = sw_proxy.verify_token(
+            request=request, verify_signature=False if in_dev_mode() else True
         )
+        return cls(product_slug=claims.get("ProductSlug"))
 
 
 @dataclass
 class RequestContext(ServiceContext):
     workspace_member_slug: str | None = None
     resource_slug: str | None = None
     resource_token_id: Optional[str] = None
@@ -103,44 +119,33 @@
             parent_job_slug=parent_job_slug,
             product_api_key=product_api_key or _cfg.get("PRODUCT_LIB_API_KEY"),
             workspace_slug=workspace_slug,
         )
 
     @staticmethod
     def from_request(request: Request):
-        token = request.headers.get("x-strangeworks-access-token")
-        if not token:
-            raise StrangeworksError.forbidden_error(
-                message="request missing access token"
-            )
-        return RequestContext.from_jwt(
-            token=token,
+        # wrote out verify_signature value to make it easier to read.
+        claims, token = sw_proxy.verify_token(
+            request=request, verify_signature=False if in_dev_mode() else True
+        )
+        return RequestContext(
+            resource_token_id=claims.get("ResourceTokenID"),
+            workspace_member_slug=claims["WorkspaceMemberSlug"],
+            product_slug=claims.get("ProductSlug"),
+            resource_slug=claims["ResourceSlug"],
+            resource_entitlements=claims.get("ResourceEntitlements"),
+            workspace_slug=claims.get("WorkspaceSlug"),
             parent_job_slug=request.headers.get("x-strangeworks-parent-job-slug"),
             _auth_token=token,
             product_api_key=_cfg.get("PRODUCT_LIB_API_KEY"),
             experiment_trial_id=request.headers.get(
                 "x-strangeworks-experiment-trial-id"
             ),
         )
 
-    @staticmethod
-    def from_jwt(token: str, **kwargs):
-        # the key to verify each token will be available as API_SIGNING_KEY
-        message = jwt.decode(token=token, key=None, options={"verify_signature": False})
-        # throw ex if resource slug or workspace member slug is missing.
-        return RequestContext(
-            resource_token_id=message.get("ResourceTokenID"),
-            workspace_member_slug=message["WorkspaceMemberSlug"],
-            product_slug=message.get("ProductSlug"),
-            resource_slug=message["ResourceSlug"],
-            resource_entitlements=message.get("ResourceEntitlements"),
-            workspace_slug=message.get("WorkspaceSlug"),
-            **kwargs,
-        )
-
 
 def create_job(
     ctx: RequestContext,
     external_identifier: Optional[str] = None,
     status: str = "CREATED",
     remote_status: Optional[str] = None,
     job_data_schema: Optional[str] = None,
@@ -180,15 +185,15 @@
         job_data_schema=job_data_schema,
         job_data=job_data,
         experiment_trial_id=ctx.experiment_trial_id,
     )
 
 
 def update_job(
-    ctx: RequestContext,
+    ctx: ServiceContext,
     job_slug: str,
     parent_job_slug: Optional[str] = None,
     external_identifier: Optional[str] = None,
     status: Optional[str] = None,
     remote_status: Optional[str] = None,
     job_data_schema: Optional[str] = None,
     job_data: Optional[str] = None,
@@ -214,15 +219,14 @@
     job_data_schema: Optional[str]
         link to the json schema describing job output.
     job_data: Optional[str]
         job output.
     """
     return job.update(
         api=ctx.api or _api(),
-        resource_slug=ctx.resource_slug,
         job_slug=job_slug,
         parent_job_slug=parent_job_slug,
         external_identifier=external_identifier,
         status=status,
         remote_status=remote_status,
         job_data_schema=job_data_schema,
         job_data=job_data,
@@ -516,15 +520,15 @@
 
 
 def get_jobs(
     ctx: ServiceContext,
     resource_slug: str | None = None,
     parent_job_slug: str | None = None,
     tags: List[str] | None = None,
-    statuses: List[str] | None = None,
+    statuses: List[JobStatus] | None = None,
     cursor: str | None = None,
     batch_size: int = 50,
 ) -> Tuple[List[Job], str, bool]:
     """Get Jobs (pagination)
 
     Uses pagination to retrieve list of jobs which match given filters.
     Example of how to paginate over jobs:
@@ -570,15 +574,15 @@
         tags=tags,
         statuses=statuses,
         start_cursor=cursor,
         batch_size=50 if batch_size > 50 else batch_size,
     )
 
 
-def get_job(ctx: RequestContext, job_slug: str) -> Job:
+def get_job(ctx: ServiceContext, job_slug: str) -> Job:
     """Get the job identified by job_slug.
 
 
     Parameters
     ----------
     ctx: RequestContext
         contains key-values specific to the current request.
@@ -586,15 +590,15 @@
         job_slug identifies the job which is fetched.
 
     Returns
     -------
     Job
         A Job object identified by the slug.
     """
-    return job.get(api=ctx.api or _api(), resource_slug=ctx.resource_slug, id=job_slug)
+    return job.get(api=ctx.api or _api(), id=job_slug)
 
 
 def get_job_by_external_identifier(
     ctx: RequestContext, external_identifier: str
 ) -> Optional[Job]:
     """Get the job identified by external_identifier.
     Parameters
@@ -881,24 +885,30 @@
     -------
     Job
         A job object denoting the sub-job.
     """
     parent_slug = parent_job.slug if isinstance(parent_job, Job) else parent_job
     if not parent_slug:
         raise ValueError("parent_job (slug or Job object) must be provided.")
-    retval = job.execute_subjob(
-        parent_job_slug=parent_slug,
-        api_key=ctx.product_api_key,
-        proxy_auth_token=ctx._auth_token,
-        resource=subjob_resource,
-        path=subjob_path,
-        json=subjob_json,
-        data=subjob_data,
-        base_url=_cfg.get("PRODUCT_LIB_BASE_URL") or DEFAULT_PLATFORM_BASE_URL,
-    )
+
+    try:
+        retval = job.execute_subjob(
+            parent_job_slug=parent_slug,
+            api_key=ctx.product_api_key,
+            proxy_auth_token=ctx._auth_token,
+            resource=subjob_resource,
+            path=subjob_path,
+            json=subjob_json,
+            data=subjob_data,
+            base_url=_cfg.get("PRODUCT_LIB_BASE_URL") or DEFAULT_PLATFORM_BASE_URL,
+        )
+        retval.raise_for_status()
+    except requests.exceptions.HTTPError as e:
+        raise StrangeworksError(message=e) from e
+
     as_json = retval.json()
 
     if raw_result is True:
         return as_json
 
     return result_parser(as_json)
 
@@ -1037,7 +1047,45 @@
         _url, headers={"Authorization": f"bearer {authtoken}"}, stream=True
     ) as resp:
         resp.raise_for_status()
         with open(_fpath.as_posix(), "wb") as fp:
             for chunk in resp.iter_content(chunk_size=chunk_size):
                 fp.write(chunk)
     return _fpath
+
+
+def get_jobs_to_update(
+    ctx: RequestContext,
+    cursor: str | None = None,
+    batch_size: int = 50,
+) -> Tuple[List[Job], str, bool]:
+    """Retrieve paginated list of jobs to update.
+
+    Platform will only return jobs which were created by the application. In more
+    detailed terms, the jobs whose resource is for the same product as the product
+    whose api key is used to request the list will be returned.
+
+    Along with matching the current product, jobs must be in a non-terminal state (see
+    NON_TERMINAL_STATUSES in jobs)
+
+    If the resource associated with the job has a api_url specified, this function
+    will only retrieve jobs whose resource api url matches the one specified by the
+    environment variable STRANGEWORKS_CONFIG_DEFAULT_PRODUCT_CUSTOM_URL.
+
+    Returns
+    -------
+    : List[Jobs], str, bool
+        a tuple consisting of a list of jobs, a string to indicate the cursor, and a
+        boolean indicating whether there are any more records to be fetched.
+    """
+    api_url = _cfg.get("product_custom_url") or None
+
+    jobs, cursor, has_next = job.get_list(
+        api=ctx.api or _api(),
+        statuses=job.NON_TERMINAL_STATUSES,
+        start_cursor=cursor,
+        batch_size=50 if batch_size > 50 else batch_size,
+    )
+    result_list = (
+        [j for j in jobs if j.resource.api_url == api_url] if len(jobs) > 0 else []
+    )
+    return result_list, cursor, has_next
```

### Comparing `sw_product_lib-0.8.9/sw_product_lib/types/backend.py` & `sw_product_lib-0.9.0/sw_product_lib/types/backend.py`

 * *Files identical despite different names*

### Comparing `sw_product_lib-0.8.9/sw_product_lib/types/batch_job.py` & `sw_product_lib-0.9.0/sw_product_lib/types/batch_job.py`

 * *Files identical despite different names*

### Comparing `sw_product_lib-0.8.9/sw_product_lib/types/job.py` & `sw_product_lib-0.9.0/sw_product_lib/types/job.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,20 @@
 from strangeworks_core.types.job import Job as JobBase
 from strangeworks_core.types.job import Status as JobStatus
 from strangeworks_core.utils import str_to_datetime
 
 from .resource import Resource
 
 
+NON_TERMINAL_STATUSES = [JobStatus.CREATED, JobStatus.QUEUED, JobStatus.RUNNING]
+
+
 class Job(JobBase):
     parent_job_slug: str | None = None
+    resource: Resource | None = None
 
     def __init__(
         self,
         parentJob: Optional[Dict[str, Any]] = None,
         **kwargs,
     ):
         super().__init__(**kwargs)
@@ -179,26 +183,24 @@
 
     return Job.from_dict(platform_result["jobCreate"]["job"])
 
 
 update_request = Operation(
     query="""
             mutation jobUpdate(
-                $resource_slug: String!
                 $job_slug: String!
                 $parent_job_slug: String
                 $external_identifier: String
                 $status: JobStatus
                 $remote_status: String
                 $job_data_schema: String
                 $job_data: JSON
             ) {
                 jobUpdate(
                     input: {
-                        resourceSlug: $resource_slug
                         jobSlug: $job_slug
                         parentJobSlug: $parent_job_slug
                         externalIdentifier: $external_identifier
                         status: $status
                         remoteStatus: $remote_status
                         jobDataSchema: $job_data_schema
                         jobData: $job_data
@@ -232,31 +234,29 @@
             }
         """,
 )
 
 
 def update(
     api: API,
-    resource_slug: str,
     job_slug: str,
     parent_job_slug: Optional[str] = None,
     external_identifier: Optional[str] = None,
     status: Optional[str] = None,
     remote_status: Optional[str] = None,
     job_data_schema: Optional[str] = None,
     job_data: Optional[str] = None,
+    **kwargs,
 ) -> Job:
     """Make an update to a job entry.
 
     Parameters
     ----------
     api: API
         provides access to the platform API.
-    resource_slug: str
-        used as identifier for the resource.
     job_slug: str
         identifier used to retrieve the job.
     parent_job_slug: Optional[str]
         slug of the job which created this job.
     external_identifier: Optional[str]
         id typically generated as a result of making a request to an external system.
     status: {Optionapstr
@@ -278,16 +278,16 @@
         **locals(),
     )
     return Job.from_dict(platform_result["jobUpdate"]["job"])
 
 
 get_job_request = Operation(
     query="""
-    query job($resource_slug: String!, $job_slug: String!) {
-        job(resourceSlug: $resource_slug, jobSlug: $job_slug) {
+    query job($job_slug: String!) {
+        job(jobSlug: $job_slug) {
             id
             childJobs {
                 id
                 slug
                 status
                 isTerminalState
                 remoteStatus
@@ -330,36 +330,33 @@
     }
     """
 )
 
 
 def get(
     api: API,
-    resource_slug: str,
     id: str,
+    **kwargs,
 ) -> Job:
     """Retrieve job info
 
     Parameters
     ----------
     api: API
         provides access to the platform API.
-    resource_slug: str
-        identifier for the resource.
     id: str
         the job_slug identifier used to retrieve the job.
 
     Returns
     -------
     Job
         The ``Job`` object identified by the slug.
     """
     platform_result = api.execute(
         op=get_job_request,
-        resource_slug=resource_slug,
         job_slug=id,
     )
     return Job.from_dict(platform_result["job"])
 
 
 get_jobs_request = Operation(
     query="""
@@ -397,14 +394,15 @@
                         slug
                         status
                         parentJob {
                             slug
                         }
                         resource {
                             slug
+                            apiRoute
                         }
                         externalIdentifier
                         isTerminalState
                         remoteStatus
                         dateCreated
                         dateUpdated
                     }
@@ -412,20 +410,20 @@
             }
         }
 """,
 )
 
 
 def get_list(
-    api: API, start_cursor: str = None, batch_size: int = 50, **kwargs
+    api: API,
+    start_cursor: str = None,
+    batch_size: int = 50,
+    **kwargs,
 ) -> Tuple[List[Job], str, bool]:
     """Return list of jobs."""
-    # has_next_page = True
-    # jobs = []
-    # while has_next_page:
     platform_result = api.execute(
         op=get_jobs_request, first=batch_size, after=start_cursor, **kwargs
     )
     if "jobs" not in platform_result:
         raise StrangeworksError(
             message="Missing field ('jobs') in response to jobs query",
             status_code=500,
```

### Comparing `sw_product_lib-0.8.9/sw_product_lib/types/resource.py` & `sw_product_lib-0.9.0/sw_product_lib/types/resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,15 @@
             "isInternal": self.is_internal,
             valueKey: self.value,
         }
 
 
 class Resource(ResourceBase):
     configurations: list[ResourceConfiguration] | None = None
+    api_url: str | None = None
 
     def __init__(
         self,
         configurations: Optional[list[dict[str, Any]]] = None,
         **kwargs,
     ) -> None:
         super().__init__(**kwargs)
```

### Comparing `sw_product_lib-0.8.9/PKG-INFO` & `sw_product_lib-0.9.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: sw-product-lib
-Version: 0.8.9
+Version: 0.9.0
 Summary: Python library for Strangeworks products to interact with the Strangeworks Platform
 License: Apache-2.0
 Author: Strangeworks Devs
 Author-email: hello@strangeworks.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: deprecated (>=1.2.13,<2.0.0)
 Requires-Dist: fastapi (>=0.104.0,<0.105.0)
+Requires-Dist: google-auth (>=2.29.0,<3.0.0)
 Requires-Dist: gql (>=3.4.1,<4.0.0)
 Requires-Dist: python-jose[cryptography] (>=3.3.0,<4.0.0)
-Requires-Dist: strangeworks-core (>=0.3.8,<0.4.0)
+Requires-Dist: strangeworks-core (>=0.3.10,<0.4.0)
```

