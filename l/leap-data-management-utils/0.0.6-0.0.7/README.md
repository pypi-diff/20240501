# Comparing `tmp/leap_data_management_utils-0.0.6.tar.gz` & `tmp/leap_data_management_utils-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leap_data_management_utils-0.0.6.tar", last modified: Tue Apr 30 19:54:19 2024, max compression
+gzip compressed data, was "leap_data_management_utils-0.0.7.tar", last modified: Wed May  1 03:03:23 2024, max compression
```

## Comparing `leap_data_management_utils-0.0.6.tar` & `leap_data_management_utils-0.0.7.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:54:19.219972 leap_data_management_utils-0.0.6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:54:19.215972 leap_data_management_utils-0.0.6/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-30 19:54:07.000000 leap_data_management_utils-0.0.6/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:54:19.215972 leap_data_management_utils-0.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-30 19:54:07.000000 leap_data_management_utils-0.0.6/.github/workflows/catalog-ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-30 19:54:07.000000 leap_data_management_utils-0.0.6/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-30 19:54:07.000000 leap_data_management_utils-0.0.6/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-04-30 19:54:07.000000 leap_data_management_utils-0.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-30 19:54:07.000000 leap_data_management_utils-0.0.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-30 19:54:07.000000 leap_data_management_utils-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-30 19:54:19.219972 leap_data_management_utils-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-30 19:54:07.000000 leap_data_management_utils-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:54:19.215972 leap_data_management_utils-0.0.6/ci/
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-30 19:54:07.000000 leap_data_management_utils-0.0.6/ci/environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:54:19.219972 leap_data_management_utils-0.0.6/leap_data_management_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-30 19:54:07.000000 leap_data_management_utils-0.0.6/leap_data_management_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-30 19:54:19.000000 leap_data_management_utils-0.0.6/leap_data_management_utils/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     8944 2024-04-30 19:54:07.000000 leap_data_management_utils-0.0.6/leap_data_management_utils/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-04-30 19:54:07.000000 leap_data_management_utils-0.0.6/leap_data_management_utils/cmip_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-04-30 19:54:07.000000 leap_data_management_utils-0.0.6/leap_data_management_utils/cmip_testing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9115 2024-04-30 19:54:07.000000 leap_data_management_utils-0.0.6/leap_data_management_utils/cmip_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     7799 2024-04-30 19:54:07.000000 leap_data_management_utils-0.0.6/leap_data_management_utils/data_management_transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:54:19.219972 leap_data_management_utils-0.0.6/leap_data_management_utils/testing_notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)    25238 2024-04-30 19:54:07.000000 leap_data_management_utils-0.0.6/leap_data_management_utils/testing_notebooks/testing_cmip_bigquery.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:54:19.219972 leap_data_management_utils-0.0.6/leap_data_management_utils/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-30 19:54:07.000000 leap_data_management_utils-0.0.6/leap_data_management_utils/tests/test_cmip_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-30 19:54:07.000000 leap_data_management_utils-0.0.6/leap_data_management_utils/tests/test_data_management_transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:54:19.219972 leap_data_management_utils-0.0.6/leap_data_management_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-30 19:54:19.000000 leap_data_management_utils-0.0.6/leap_data_management_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-30 19:54:19.000000 leap_data_management_utils-0.0.6/leap_data_management_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 19:54:19.000000 leap_data_management_utils-0.0.6/leap_data_management_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-30 19:54:19.000000 leap_data_management_utils-0.0.6/leap_data_management_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-30 19:54:19.000000 leap_data_management_utils-0.0.6/leap_data_management_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-30 19:54:19.000000 leap_data_management_utils-0.0.6/leap_data_management_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-04-30 19:54:07.000000 leap_data_management_utils-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 19:54:19.219972 leap_data_management_utils-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 03:03:23.258377 leap_data_management_utils-0.0.7/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 03:03:23.254377 leap_data_management_utils-0.0.7/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-01 03:03:09.000000 leap_data_management_utils-0.0.7/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 03:03:23.254377 leap_data_management_utils-0.0.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-01 03:03:09.000000 leap_data_management_utils-0.0.7/.github/workflows/catalog-ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-01 03:03:09.000000 leap_data_management_utils-0.0.7/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-01 03:03:09.000000 leap_data_management_utils-0.0.7/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-05-01 03:03:09.000000 leap_data_management_utils-0.0.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-01 03:03:09.000000 leap_data_management_utils-0.0.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-01 03:03:09.000000 leap_data_management_utils-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-01 03:03:23.258377 leap_data_management_utils-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-01 03:03:09.000000 leap_data_management_utils-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 03:03:23.254377 leap_data_management_utils-0.0.7/ci/
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-01 03:03:09.000000 leap_data_management_utils-0.0.7/ci/environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 03:03:23.258377 leap_data_management_utils-0.0.7/leap_data_management_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-01 03:03:09.000000 leap_data_management_utils-0.0.7/leap_data_management_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-01 03:03:23.000000 leap_data_management_utils-0.0.7/leap_data_management_utils/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8944 2024-05-01 03:03:09.000000 leap_data_management_utils-0.0.7/leap_data_management_utils/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-05-01 03:03:09.000000 leap_data_management_utils-0.0.7/leap_data_management_utils/cmip_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-05-01 03:03:09.000000 leap_data_management_utils-0.0.7/leap_data_management_utils/cmip_testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9115 2024-05-01 03:03:09.000000 leap_data_management_utils-0.0.7/leap_data_management_utils/cmip_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9450 2024-05-01 03:03:09.000000 leap_data_management_utils-0.0.7/leap_data_management_utils/data_management_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 03:03:23.258377 leap_data_management_utils-0.0.7/leap_data_management_utils/testing_notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)    25238 2024-05-01 03:03:09.000000 leap_data_management_utils-0.0.7/leap_data_management_utils/testing_notebooks/testing_cmip_bigquery.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 03:03:23.258377 leap_data_management_utils-0.0.7/leap_data_management_utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-01 03:03:09.000000 leap_data_management_utils-0.0.7/leap_data_management_utils/tests/test_cmip_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-01 03:03:09.000000 leap_data_management_utils-0.0.7/leap_data_management_utils/tests/test_data_management_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 03:03:23.258377 leap_data_management_utils-0.0.7/leap_data_management_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-01 03:03:23.000000 leap_data_management_utils-0.0.7/leap_data_management_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-01 03:03:23.000000 leap_data_management_utils-0.0.7/leap_data_management_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 03:03:23.000000 leap_data_management_utils-0.0.7/leap_data_management_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-01 03:03:23.000000 leap_data_management_utils-0.0.7/leap_data_management_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-01 03:03:23.000000 leap_data_management_utils-0.0.7/leap_data_management_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-01 03:03:23.000000 leap_data_management_utils-0.0.7/leap_data_management_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-05-01 03:03:09.000000 leap_data_management_utils-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 03:03:23.258377 leap_data_management_utils-0.0.7/setup.cfg
```

### Comparing `leap_data_management_utils-0.0.6/.github/workflows/catalog-ci.yaml` & `leap_data_management_utils-0.0.7/.github/workflows/catalog-ci.yaml`

 * *Files identical despite different names*

### Comparing `leap_data_management_utils-0.0.6/.github/workflows/ci.yaml` & `leap_data_management_utils-0.0.7/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `leap_data_management_utils-0.0.6/.github/workflows/release.yaml` & `leap_data_management_utils-0.0.7/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `leap_data_management_utils-0.0.6/.gitignore` & `leap_data_management_utils-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `leap_data_management_utils-0.0.6/.pre-commit-config.yaml` & `leap_data_management_utils-0.0.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `leap_data_management_utils-0.0.6/LICENSE` & `leap_data_management_utils-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `leap_data_management_utils-0.0.6/PKG-INFO` & `leap_data_management_utils-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leap-data-management-utils
-Version: 0.0.6
+Version: 0.0.7
 Summary: LEAP / pangeo-forge-recipes extension library for logging data in Google Big Query
 Author-email: LEAP <leap@columbia.edu>
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
```

### Comparing `leap_data_management_utils-0.0.6/leap_data_management_utils/catalog.py` & `leap_data_management_utils-0.0.7/leap_data_management_utils/catalog.py`

 * *Files identical despite different names*

### Comparing `leap_data_management_utils-0.0.6/leap_data_management_utils/cmip_catalog.py` & `leap_data_management_utils-0.0.7/leap_data_management_utils/cmip_catalog.py`

 * *Files identical despite different names*

### Comparing `leap_data_management_utils-0.0.6/leap_data_management_utils/cmip_testing.py` & `leap_data_management_utils-0.0.7/leap_data_management_utils/cmip_testing.py`

 * *Files identical despite different names*

### Comparing `leap_data_management_utils-0.0.6/leap_data_management_utils/cmip_transforms.py` & `leap_data_management_utils-0.0.7/leap_data_management_utils/cmip_transforms.py`

 * *Files identical despite different names*

### Comparing `leap_data_management_utils-0.0.6/leap_data_management_utils/data_management_transforms.py` & `leap_data_management_utils-0.0.7/leap_data_management_utils/data_management_transforms.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,86 @@
 # Note: All of this code was written by Julius Busecke and copied from this feedstock:
 # https://github.com/leap-stc/cmip6-leap-feedstock/blob/main/feedstock/recipe.py#L262
 
+import os
 import subprocess
 from dataclasses import dataclass
 from datetime import datetime, timezone
 from typing import Optional
 
 import apache_beam as beam
 import zarr
 from google.api_core.exceptions import NotFound
 from google.cloud import bigquery
 from ruamel.yaml import YAML
 
 yaml = YAML(typ='safe')
 
 
-def get_github_commit_url() -> Optional[str]:
-    """Get the GitHub commit URL for the current commit"""
-    # Get GitHub Server URL
-    github_server_url = 'https://github.com'
+def get_github_actions_url() -> str:
+    """Return the url of the gh action run"""
+    if os.getenv('GITHUB_ACTIONS') == 'true':
+        print('Running from within GH actions')
+        server_url = os.getenv('GITHUB_SERVER_URL')
+        repository = os.getenv('GITHUB_REPOSITORY')
+        run_id = os.getenv('GITHUB_RUN_ID')
+        commit_hash = os.getenv('GITHUB_SHA')
 
-    # Get the repository's remote origin URL
-    try:
-        repo_origin_url = subprocess.check_output(
-            ['git', 'config', '--get', 'remote.origin.url'], text=True
-        ).strip()
-
-        # Extract the repository path from the remote URL
-        repository_path = repo_origin_url.split('github.com/')[-1].replace('.git', '')
+        if server_url and repository and run_id and commit_hash:
+            return f'{server_url}/{repository}/actions/runs/{run_id}'
+        else:
+            print('One or more environment variables are missing.')
+            return 'none'
+    else:
+        return 'none'
 
-        # Get the current commit SHA
-        commit_sha = subprocess.check_output(['git', 'rev-parse', 'HEAD'], text=True).strip()
 
-        # Construct the GitHub commit URL
-        git_url_hash = f'{github_server_url}/{repository_path}/commit/{commit_sha}'
+def get_github_commit_url() -> str:
+    """Get the GitHub commit URL for the current commit"""
+    # Get GitHub Server URL
 
-        # Output the GitHub commit URL
-        return git_url_hash
+    # check if this is running from within a github action
+    if os.getenv('GITHUB_ACTIONS') == 'true':
+        print('Running from within GH actions')
+        server_url = os.getenv('GITHUB_SERVER_URL')
+        repository = os.getenv('GITHUB_REPOSITORY')
+        run_id = os.getenv('GITHUB_RUN_ID')
+        commit_hash = os.getenv('GITHUB_SHA')
 
-    except subprocess.CalledProcessError as e:
-        print('Error executing Git command:', e)
-        return None
+        if server_url and repository and run_id and commit_hash:
+            git_url_hash = f'{server_url}/{repository}/commit/{commit_hash}'
+        else:
+            print(
+                'Could not construct git_url_hash. One or more environment variables are missing.'
+            )
+            git_url_hash = 'none'
+
+    else:
+        # TODO: If the above fails, maybe still try this? Even though that would be a really rare case?
+        print('Fallback: Calling git via subprocess')
+        github_server_url = 'https://github.com'
+        # Get the repository's remote origin URL
+        try:
+            repo_origin_url = subprocess.check_output(
+                ['git', 'config', '--get', 'remote.origin.url'], text=True
+            ).strip()
+
+            # Extract the repository path from the remote URL
+            repository_path = repo_origin_url.split('github.com/')[-1].replace('.git', '')
+
+            # Get the current commit SHA
+            commit_sha = subprocess.check_output(['git', 'rev-parse', 'HEAD'], text=True).strip()
+
+            # Construct the GitHub commit URL
+            git_url_hash = f'{github_server_url}/{repository_path}/commit/{commit_sha}'
+        except Exception as e:
+            print(f'Getting git_url_hash failed with {e}')
+            git_url_hash = 'none'
+    # Output the GitHub commit URL
+    return git_url_hash
 
 
 def get_catalog_store_urls(catalog_yaml_path: str) -> dict[str, str]:
     with open(catalog_yaml_path) as f:
         catalog_meta = yaml.load(f)
     return {d['id']: d['url'] for d in catalog_meta['stores']}
 
@@ -193,17 +229,19 @@
     # add a post_init method to add the provenance attributes
     def __post_init__(self):
         if self.inject_attrs is None:
             self.inject_attrs = {}
 
         if self.add_provenance:
             git_url_hash = get_github_commit_url()
+            gh_actions_url = get_github_actions_url()
             timestamp = datetime.now(timezone.utc).isoformat()
             provenance_dict = {
                 'pangeo_forge_build_git_hash': git_url_hash,
+                'pangeo_forge_gh_actions_url': gh_actions_url,
                 'pangeo_forge_build_timestamp': timestamp,
             }
             self.inject_attrs.update(provenance_dict)
 
     def _update_zarr_attrs(self, store: zarr.storage.FSStore) -> zarr.storage.FSStore:
         # TODO: Can we get a warning here if the store does not exist?
         attrs = zarr.open(store, mode='a').attrs
```

### Comparing `leap_data_management_utils-0.0.6/leap_data_management_utils/testing_notebooks/testing_cmip_bigquery.ipynb` & `leap_data_management_utils-0.0.7/leap_data_management_utils/testing_notebooks/testing_cmip_bigquery.ipynb`

 * *Files identical despite different names*

### Comparing `leap_data_management_utils-0.0.6/leap_data_management_utils/tests/test_cmip_transforms.py` & `leap_data_management_utils-0.0.7/leap_data_management_utils/tests/test_cmip_transforms.py`

 * *Files identical despite different names*

### Comparing `leap_data_management_utils-0.0.6/leap_data_management_utils/tests/test_data_management_transforms.py` & `leap_data_management_utils-0.0.7/leap_data_management_utils/tests/test_data_management_transforms.py`

 * *Files identical despite different names*

### Comparing `leap_data_management_utils-0.0.6/leap_data_management_utils.egg-info/PKG-INFO` & `leap_data_management_utils-0.0.7/leap_data_management_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leap-data-management-utils
-Version: 0.0.6
+Version: 0.0.7
 Summary: LEAP / pangeo-forge-recipes extension library for logging data in Google Big Query
 Author-email: LEAP <leap@columbia.edu>
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
```

### Comparing `leap_data_management_utils-0.0.6/leap_data_management_utils.egg-info/SOURCES.txt` & `leap_data_management_utils-0.0.7/leap_data_management_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `leap_data_management_utils-0.0.6/pyproject.toml` & `leap_data_management_utils-0.0.7/pyproject.toml`

 * *Files identical despite different names*

