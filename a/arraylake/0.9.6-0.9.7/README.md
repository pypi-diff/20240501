# Comparing `tmp/arraylake-0.9.6.tar.gz` & `tmp/arraylake-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arraylake-0.9.6.tar", max compression
+gzip compressed data, was "arraylake-0.9.7.tar", max compression
```

## Comparing `arraylake-0.9.6.tar` & `arraylake-0.9.7.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0      653 2024-04-27 00:28:22.714914 arraylake-0.9.6/README.md
--rw-r--r--   0        0        0      416 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/__init__.py
--rw-r--r--   0        0        0       63 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/__main__.py
--rw-r--r--   0        0        0    22304 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/api_utils.py
--rw-r--r--   0        0        0     9770 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/asyn.py
--rw-r--r--   0        0        0     4001 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/chunkstore/__init__.py
--rw-r--r--   0        0        0     4056 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/chunkstore/abc.py
--rw-r--r--   0        0        0     9973 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/chunkstore/base_chunkstore.py
--rw-r--r--   0        0        0     6664 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/chunkstore/fsspec_chunkstore.py
--rw-r--r--   0        0        0     1862 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/chunkstore/fsspec_compat.py
--rw-r--r--   0        0        0    10893 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/chunkstore/s3chunkstore.py
--rw-r--r--   0        0        0        0 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/cli/__init__.py
--rw-r--r--   0        0        0     4915 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/cli/auth.py
--rw-r--r--   0        0        0     4741 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/cli/config.py
--rw-r--r--   0        0        0     1615 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/cli/main.py
--rw-r--r--   0        0        0     5630 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/cli/repo.py
--rw-r--r--   0        0        0     4860 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/cli/utils.py
--rw-r--r--   0        0        0    21046 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/client.py
--rw-r--r--   0        0        0     8181 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/commits.py
--rw-r--r--   0        0        0     2976 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/config.py
--rw-r--r--   0        0        0      176 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/config.yaml
--rw-r--r--   0        0        0     5221 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/diagnostics.py
--rw-r--r--   0        0        0      345 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/exceptions.py
--rw-r--r--   0        0        0      194 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/experimental.py
--rw-r--r--   0        0        0     1082 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/log_util.py
--rw-r--r--   0        0        0      261 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/metastore/__init__.py
--rw-r--r--   0        0        0    15638 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/metastore/abc.py
--rw-r--r--   0        0        0    23366 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/metastore/http_metastore.py
--rw-r--r--   0        0        0        0 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/py.typed
--rw-r--r--   0        0        0    92130 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/repo.py
--rw-r--r--   0        0        0     7180 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/retrier.py
--rw-r--r--   0        0        0     1526 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/strategies.py
--rw-r--r--   0        0        0     4776 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/token.py
--rw-r--r--   0        0        0    27584 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/types.py
--rw-r--r--   0        0        0    17216 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/virtual.py
--rw-r--r--   0        0        0      851 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/zarr_util.py
--rw-r--r--   0        0        0     5405 2024-04-27 00:28:43.102988 arraylake-0.9.6/pyproject.toml
--rw-r--r--   0        0        0     2515 1970-01-01 00:00:00.000000 arraylake-0.9.6/PKG-INFO
+-rw-r--r--   0        0        0      653 2024-05-01 17:25:24.438752 arraylake-0.9.7/README.md
+-rw-r--r--   0        0        0      416 2024-05-01 17:25:24.438752 arraylake-0.9.7/arraylake/__init__.py
+-rw-r--r--   0        0        0       63 2024-05-01 17:25:24.438752 arraylake-0.9.7/arraylake/__main__.py
+-rw-r--r--   0        0        0    22304 2024-05-01 17:25:24.438752 arraylake-0.9.7/arraylake/api_utils.py
+-rw-r--r--   0        0        0     9770 2024-05-01 17:25:24.438752 arraylake-0.9.7/arraylake/asyn.py
+-rw-r--r--   0        0        0     4001 2024-05-01 17:25:24.438752 arraylake-0.9.7/arraylake/chunkstore/__init__.py
+-rw-r--r--   0        0        0     4056 2024-05-01 17:25:24.438752 arraylake-0.9.7/arraylake/chunkstore/abc.py
+-rw-r--r--   0        0        0     9973 2024-05-01 17:25:24.438752 arraylake-0.9.7/arraylake/chunkstore/base_chunkstore.py
+-rw-r--r--   0        0        0     6664 2024-05-01 17:25:24.438752 arraylake-0.9.7/arraylake/chunkstore/fsspec_chunkstore.py
+-rw-r--r--   0        0        0     1862 2024-05-01 17:25:24.438752 arraylake-0.9.7/arraylake/chunkstore/fsspec_compat.py
+-rw-r--r--   0        0        0    10893 2024-05-01 17:25:24.438752 arraylake-0.9.7/arraylake/chunkstore/s3chunkstore.py
+-rw-r--r--   0        0        0        0 2024-05-01 17:25:24.438752 arraylake-0.9.7/arraylake/cli/__init__.py
+-rw-r--r--   0        0        0     4915 2024-05-01 17:25:24.438752 arraylake-0.9.7/arraylake/cli/auth.py
+-rw-r--r--   0        0        0     4741 2024-05-01 17:25:24.438752 arraylake-0.9.7/arraylake/cli/config.py
+-rw-r--r--   0        0        0     1615 2024-05-01 17:25:24.438752 arraylake-0.9.7/arraylake/cli/main.py
+-rw-r--r--   0        0        0     5653 2024-05-01 17:25:24.442752 arraylake-0.9.7/arraylake/cli/repo.py
+-rw-r--r--   0        0        0     4860 2024-05-01 17:25:24.442752 arraylake-0.9.7/arraylake/cli/utils.py
+-rw-r--r--   0        0        0    21140 2024-05-01 17:25:24.442752 arraylake-0.9.7/arraylake/client.py
+-rw-r--r--   0        0        0     8181 2024-05-01 17:25:24.442752 arraylake-0.9.7/arraylake/commits.py
+-rw-r--r--   0        0        0     2976 2024-05-01 17:25:24.442752 arraylake-0.9.7/arraylake/config.py
+-rw-r--r--   0        0        0      176 2024-05-01 17:25:24.442752 arraylake-0.9.7/arraylake/config.yaml
+-rw-r--r--   0        0        0     5221 2024-05-01 17:25:24.442752 arraylake-0.9.7/arraylake/diagnostics.py
+-rw-r--r--   0        0        0      345 2024-05-01 17:25:24.442752 arraylake-0.9.7/arraylake/exceptions.py
+-rw-r--r--   0        0        0      194 2024-05-01 17:25:24.442752 arraylake-0.9.7/arraylake/experimental.py
+-rw-r--r--   0        0        0     1082 2024-05-01 17:25:24.442752 arraylake-0.9.7/arraylake/log_util.py
+-rw-r--r--   0        0        0      261 2024-05-01 17:25:24.442752 arraylake-0.9.7/arraylake/metastore/__init__.py
+-rw-r--r--   0        0        0    15638 2024-05-01 17:25:24.442752 arraylake-0.9.7/arraylake/metastore/abc.py
+-rw-r--r--   0        0        0    23366 2024-05-01 17:25:24.442752 arraylake-0.9.7/arraylake/metastore/http_metastore.py
+-rw-r--r--   0        0        0        0 2024-05-01 17:25:24.442752 arraylake-0.9.7/arraylake/py.typed
+-rw-r--r--   0        0        0    92130 2024-05-01 17:25:24.442752 arraylake-0.9.7/arraylake/repo.py
+-rw-r--r--   0        0        0     7180 2024-05-01 17:25:24.442752 arraylake-0.9.7/arraylake/retrier.py
+-rw-r--r--   0        0        0     1526 2024-05-01 17:25:24.442752 arraylake-0.9.7/arraylake/strategies.py
+-rw-r--r--   0        0        0     4776 2024-05-01 17:25:24.442752 arraylake-0.9.7/arraylake/token.py
+-rw-r--r--   0        0        0    28691 2024-05-01 17:25:24.442752 arraylake-0.9.7/arraylake/types.py
+-rw-r--r--   0        0        0    17216 2024-05-01 17:25:24.442752 arraylake-0.9.7/arraylake/virtual.py
+-rw-r--r--   0        0        0      851 2024-05-01 17:25:24.442752 arraylake-0.9.7/arraylake/zarr_util.py
+-rw-r--r--   0        0        0     5405 2024-05-01 17:25:42.270750 arraylake-0.9.7/pyproject.toml
+-rw-r--r--   0        0        0     2515 1970-01-01 00:00:00.000000 arraylake-0.9.7/PKG-INFO
```

### Comparing `arraylake-0.9.6/README.md` & `arraylake-0.9.7/README.md`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.6/arraylake/api_utils.py` & `arraylake-0.9.7/arraylake/api_utils.py`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.6/arraylake/asyn.py` & `arraylake-0.9.7/arraylake/asyn.py`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.6/arraylake/chunkstore/__init__.py` & `arraylake-0.9.7/arraylake/chunkstore/__init__.py`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.6/arraylake/chunkstore/abc.py` & `arraylake-0.9.7/arraylake/chunkstore/abc.py`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.6/arraylake/chunkstore/base_chunkstore.py` & `arraylake-0.9.7/arraylake/chunkstore/base_chunkstore.py`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.6/arraylake/chunkstore/fsspec_chunkstore.py` & `arraylake-0.9.7/arraylake/chunkstore/fsspec_chunkstore.py`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.6/arraylake/chunkstore/fsspec_compat.py` & `arraylake-0.9.7/arraylake/chunkstore/fsspec_compat.py`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.6/arraylake/chunkstore/s3chunkstore.py` & `arraylake-0.9.7/arraylake/chunkstore/s3chunkstore.py`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.6/arraylake/cli/auth.py` & `arraylake-0.9.7/arraylake/cli/auth.py`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.6/arraylake/cli/config.py` & `arraylake-0.9.7/arraylake/cli/config.py`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.6/arraylake/cli/main.py` & `arraylake-0.9.7/arraylake/cli/main.py`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.6/arraylake/cli/repo.py` & `arraylake-0.9.7/arraylake/cli/repo.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,35 +135,35 @@
 
     if output == "json":
         print_json(_tree.model_dump_json())
     else:
         rich_console.print(_tree._as_rich_tree(name=repo_name))
 
 
-@app.command()
+@app.command(hidden=True)
 @coro  # type: ignore
 async def get_status(
     repo_name: str = typer.Argument(..., help="Name of repository {ORG}/{REPO_NAME}"),
     output: ListOutputType = typer.Option("rich", help="Output formatting"),
 ):
     repo = await AsyncClient().get_repo_object(repo_name)
     if output == "json":
         print_json(data=repo.status.model_dump())
     else:
         print(repo.status.mode.value)
 
 
-@app.command()
+@app.command(hidden=True)
 @coro  # type: ignore
 async def set_status(
     repo_name: str = typer.Argument(..., help="Name of repository {ORG}/{REPO_NAME}"),
     mode: RepoOperationMode = typer.Argument(..., help="An option"),
     message: str = typer.Option(None, help="Optional message to bind to state"),
     output: ListOutputType = typer.Option("rich", help="Output formatting"),
 ):
     c = AsyncClient()
-    await c.set_repo_status(repo_name, mode, message)
+    await c._set_repo_status(repo_name, mode, message)
     repo = await c.get_repo_object(repo_name)
     if output == "json":
         print_json(data=repo.status.model_dump())
     else:
         print(repo.status.mode.value)
```

### Comparing `arraylake-0.9.6/arraylake/cli/utils.py` & `arraylake-0.9.7/arraylake/cli/utils.py`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.6/arraylake/client.py` & `arraylake-0.9.7/arraylake/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,15 @@
 
         author: Author = user.as_author()
         arepo = AsyncRepo(db, cstore, name, author)
         if checkout:
             await arepo.checkout()
         return arepo
 
-    async def set_repo_status(
+    async def _set_repo_status(
         self, qualified_repo_name: str, mode: RepoOperationMode, message: str | None = None
     ) -> RepoOperationStatusResponse:
         org, repo_name = _parse_org_and_repo(qualified_repo_name)
         mstore = self._metastore_for_org(org)
         return await mstore.set_repo_status(repo_name, mode, message)
 
     async def get_or_create_repo(
@@ -171,15 +171,15 @@
         Args:
             name: Full name of the repo (of the form [ORG]/[REPO])
             bucket_config_nickname: the created repo will use this bucket for its chunks.
                If the repo exists, bucket_config_nickname is ignored.
             checkout: Automatically checkout the repo after instantiation.
                If the repo does not exist, checkout is ignored.
         """
-        if bucket_nickname:
+        if bucket_config_nickname is None and bucket_nickname:
             bucket_config_nickname = bucket_nickname
             warnings.warn("bucket_nickname has been renamed to bucket_config_nickname and will be removed in Arraylake 0.10", FutureWarning)
         org, repo_name = _parse_org_and_repo(name)
         repos = [r for r in await self.list_repos(org) if r.name == repo_name]
         if repos:
             (repo,) = repos
             if bucket_config_nickname:
@@ -193,30 +193,30 @@
                     raise ValueError(
                         "This repo exists, but does not have a bucket config attached. Please remove the bucket_config_nickname argument."
                     )
                 else:
                     return await self.get_repo(name, checkout=checkout)
             return await self.get_repo(name, checkout=checkout)
         else:
-            return await self.create_repo(name, bucket_config_nickname)
+            return await self.create_repo(name, bucket_config_nickname=bucket_config_nickname)
 
     async def create_repo(
         self,
         name: str,
         bucket_nickname: Optional[str] = None,
         *,
         bucket_config_nickname: Optional[str] = None,
     ) -> AsyncRepo:
         """Create a new repo
 
         Args:
             name: Full name of the repo to create (of the form [ORG]/[REPO])
             bucket_config_nickname: An optional bucket to use for the chunkstore
         """
-        if bucket_nickname:
+        if bucket_config_nickname is None and bucket_nickname:
             bucket_config_nickname = bucket_nickname
             warnings.warn("bucket_nickname has been renamed to bucket_config_nickname and will be removed in Arraylake 0.10", FutureWarning)
 
         org, repo_name = _parse_org_and_repo(name)
         mstore = self._metastore_for_org(org)
         db = await mstore.create_database(repo_name, bucket_config_nickname)
```

### Comparing `arraylake-0.9.6/arraylake/commits.py` & `arraylake-0.9.7/arraylake/commits.py`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.6/arraylake/config.py` & `arraylake-0.9.7/arraylake/config.py`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.6/arraylake/diagnostics.py` & `arraylake-0.9.7/arraylake/diagnostics.py`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.6/arraylake/log_util.py` & `arraylake-0.9.7/arraylake/log_util.py`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.6/arraylake/metastore/abc.py` & `arraylake-0.9.7/arraylake/metastore/abc.py`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.6/arraylake/metastore/http_metastore.py` & `arraylake-0.9.7/arraylake/metastore/http_metastore.py`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.6/arraylake/repo.py` & `arraylake-0.9.7/arraylake/repo.py`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.6/arraylake/retrier.py` & `arraylake-0.9.7/arraylake/retrier.py`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.6/arraylake/strategies.py` & `arraylake-0.9.7/arraylake/strategies.py`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.6/arraylake/token.py` & `arraylake-0.9.7/arraylake/token.py`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.6/arraylake/types.py` & `arraylake-0.9.7/arraylake/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -268,23 +268,48 @@
     nickname: str
     platform: Platform
     name: str
     prefix: str = ""  # default for compatibility with older data
     extra_config: Mapping[str, Union[str, bool]]
     auth_config: AuthConfig = Field(discriminator="method")
 
-    # NOTE: Validation on name is not necessary, as S3 has fairly strict naming
-    # rules. If name doesn't exactly match the S3 bucket name, then we have a
-    # bigger problem than simple naming rules.
+    @model_validator(mode="after")
+    def _validate_bucket_options(self):
+        if self.platform in ["s3"]:  # TODO: decide if the same is needed for gs buckets
+            if "region_name" not in self.extra_config:
+                raise ValueError("S3 buckets require a region_name.")
+        if self.platform == "s3-compatible":
+            if "endpoint_url" not in self.extra_config:
+                raise ValueError("S3-compatible buckets require an endpoint_url.")
+        return self
+
+    @field_validator("name")
+    @classmethod
+    def validate_name(cls, name: str) -> str:
+        # NOTE: S3 and GCS have fairly strict naming rules so we can mostly rely on them here.
+        # Our checks are meant to make sure the data we receive is valid.
+        if " " in name:
+            raise ValueError("Bucket name must not contain spaces.")
+        if "://" in name:
+            raise ValueError("Bucket name must not contain schemes.")
+        if "/" in name:
+            raise ValueError("Bucket name must not contain slashes.")
+        if len(name) < 3:
+            raise ValueError("Bucket name must be at least 3 characters long.")
+        return name
 
     @field_validator("prefix")
     @classmethod
     def validate_prefix(cls, prefix: str) -> str:
+        if prefix == "":
+            return prefix
         # Remove leading and trailing whitespace.
         prefix = prefix.strip()
+        if " " in prefix:
+            raise ValueError("Bucket prefix must not contain spaces.")
         if len(prefix) > 900:  # S3 max key size minus some buffer for key
             raise ValueError("Bucket prefix must be at most 900 characters long.")
         if prefix.startswith("/") or prefix.endswith("/"):
             raise ValueError("Bucket prefix must not start or end with a slash.")
         return prefix
 
     @field_validator("nickname")
```

### Comparing `arraylake-0.9.6/arraylake/virtual.py` & `arraylake-0.9.7/arraylake/virtual.py`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.6/arraylake/zarr_util.py` & `arraylake-0.9.7/arraylake/zarr_util.py`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.6/pyproject.toml` & `arraylake-0.9.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "arraylake"
-version = "0.9.6"  # placeholder
+version = "0.9.7"  # placeholder
 description = "Python client for ArrayLake"
 authors = ["Joe Hamman <joe@earthmover.io>"]
 readme = "README.md"
 packages = [{include = "arraylake"}]
 
 [[tool.poetry.source]]
 name = "pytorch-cpu-src"
```

### Comparing `arraylake-0.9.6/PKG-INFO` & `arraylake-0.9.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arraylake
-Version: 0.9.6
+Version: 0.9.7
 Summary: Python client for ArrayLake
 Author: Joe Hamman
 Author-email: joe@earthmover.io
 Requires-Python: >=3.10,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: arraylake Version: 0.9.6 Summary: Python client for
+Metadata-Version: 2.1 Name: arraylake Version: 0.9.7 Summary: Python client for
 ArrayLake Author: Joe Hamman Author-email: joe@earthmover.io Requires-Python:
 >=3.10,<3.13 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Provides-
 Extra: grib Provides-Extra: virtual Provides-Extra: widgets Provides-Extra:
 xarray Requires-Dist: aiobotocore[boto3] (>=2.4.0,<3.0.0) Requires-Dist:
 aioitertools (>=0.11.0,<0.12.0) Requires-Dist: boto3 (>=1.24,<2.0) Requires-
```

