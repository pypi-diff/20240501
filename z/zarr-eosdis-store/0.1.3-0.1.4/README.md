# Comparing `tmp/zarr-eosdis-store-0.1.3.tar.gz` & `tmp/zarr-eosdis-store-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zarr-eosdis-store-0.1.3.tar", last modified: Wed Aug 11 20:07:51 2021, max compression
+gzip compressed data, was "zarr-eosdis-store-0.1.4.tar", last modified: Fri Feb  2 17:30:06 2024, max compression
```

## Comparing `zarr-eosdis-store-0.1.3.tar` & `zarr-eosdis-store-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-11 20:07:51.731186 zarr-eosdis-store-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (121)     9772 2021-08-11 20:07:24.000000 zarr-eosdis-store-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       25 2021-08-11 20:07:24.000000 zarr-eosdis-store-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6090 2021-08-11 20:07:51.731186 zarr-eosdis-store-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5340 2021-08-11 20:07:24.000000 zarr-eosdis-store-0.1.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-11 20:07:51.727186 zarr-eosdis-store-0.1.3/eosdis_store/
--rw-r--r--   0 runner    (1001) docker     (121)      163 2021-08-11 20:07:24.000000 zarr-eosdis-store-0.1.3/eosdis_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9510 2021-08-11 20:07:24.000000 zarr-eosdis-store-0.1.3/eosdis_store/dmrpp.py
--rw-r--r--   0 runner    (1001) docker     (121)     9757 2021-08-11 20:07:24.000000 zarr-eosdis-store-0.1.3/eosdis_store/stores.py
--rw-r--r--   0 runner    (1001) docker     (121)       23 2021-08-11 20:07:49.000000 zarr-eosdis-store-0.1.3/eosdis_store/version.py
--rw-r--r--   0 runner    (1001) docker     (121)      114 2021-08-11 20:07:24.000000 zarr-eosdis-store-0.1.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-08-11 20:07:51.731186 zarr-eosdis-store-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1895 2021-08-11 20:07:24.000000 zarr-eosdis-store-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-11 20:07:51.731186 zarr-eosdis-store-0.1.3/zarr_eosdis_store.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6090 2021-08-11 20:07:51.000000 zarr-eosdis-store-0.1.3/zarr_eosdis_store.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      354 2021-08-11 20:07:51.000000 zarr-eosdis-store-0.1.3/zarr_eosdis_store.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-11 20:07:51.000000 zarr-eosdis-store-0.1.3/zarr_eosdis_store.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      267 2021-08-11 20:07:51.000000 zarr-eosdis-store-0.1.3/zarr_eosdis_store.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2021-08-11 20:07:51.000000 zarr-eosdis-store-0.1.3/zarr_eosdis_store.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 17:30:06.578964 zarr-eosdis-store-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     9772 2024-02-02 17:29:36.000000 zarr-eosdis-store-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-02 17:29:36.000000 zarr-eosdis-store-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6697 2024-02-02 17:30:06.578964 zarr-eosdis-store-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-02-02 17:29:36.000000 zarr-eosdis-store-0.1.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 17:30:06.578964 zarr-eosdis-store-0.1.4/eosdis_store/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-02-02 17:29:36.000000 zarr-eosdis-store-0.1.4/eosdis_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9510 2024-02-02 17:29:36.000000 zarr-eosdis-store-0.1.4/eosdis_store/dmrpp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9757 2024-02-02 17:29:36.000000 zarr-eosdis-store-0.1.4/eosdis_store/stores.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-02 17:30:04.000000 zarr-eosdis-store-0.1.4/eosdis_store/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-02-02 17:29:36.000000 zarr-eosdis-store-0.1.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-02 17:30:06.578964 zarr-eosdis-store-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-02-02 17:29:36.000000 zarr-eosdis-store-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 17:30:06.578964 zarr-eosdis-store-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5610 2024-02-02 17:29:36.000000 zarr-eosdis-store-0.1.4/tests/test_dmrpp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6274 2024-02-02 17:29:36.000000 zarr-eosdis-store-0.1.4/tests/test_stores.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 17:30:06.578964 zarr-eosdis-store-0.1.4/zarr_eosdis_store.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6697 2024-02-02 17:30:06.000000 zarr-eosdis-store-0.1.4/zarr_eosdis_store.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-02-02 17:30:06.000000 zarr-eosdis-store-0.1.4/zarr_eosdis_store.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-02 17:30:06.000000 zarr-eosdis-store-0.1.4/zarr_eosdis_store.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-02-02 17:30:06.000000 zarr-eosdis-store-0.1.4/zarr_eosdis_store.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-02 17:30:06.000000 zarr-eosdis-store-0.1.4/zarr_eosdis_store.egg-info/top_level.txt
```

### Comparing `zarr-eosdis-store-0.1.3/LICENSE` & `zarr-eosdis-store-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `zarr-eosdis-store-0.1.3/PKG-INFO` & `zarr-eosdis-store-0.1.4/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: zarr-eosdis-store
-Version: 0.1.3
-Summary: Zarr Store class for working with EOSDIS cloud data
-Home-page: https://github.com/nasa/zarr-eosdis-store
-Author: Patrick Quinn, Matthew Hanson
-Author-email: patrick@patrickquinn.net
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 zarr-eosdis-store
 =================
 
 The zarr-eosdis-store library allows NASA EOSDIS Collections to be accessed efficiently
 by the `Zarr Python library <https://zarr.readthedocs.io/en/stable/index.html>`_, provided they
 have a sidecar DMR++ metadata file generated.
 
@@ -164,9 +143,7 @@
 To check coding style::
 
     flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics
 
 To build documentation, generated at ``docs/_build/html/index.html``::
 
     cd docs && make html
-
-
```

### Comparing `zarr-eosdis-store-0.1.3/eosdis_store/dmrpp.py` & `zarr-eosdis-store-0.1.4/eosdis_store/dmrpp.py`

 * *Files identical despite different names*

### Comparing `zarr-eosdis-store-0.1.3/eosdis_store/stores.py` & `zarr-eosdis-store-0.1.4/eosdis_store/stores.py`

 * *Files identical despite different names*

### Comparing `zarr-eosdis-store-0.1.3/setup.py` & `zarr-eosdis-store-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `zarr-eosdis-store-0.1.3/zarr_eosdis_store.egg-info/PKG-INFO` & `zarr-eosdis-store-0.1.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,41 @@
 Metadata-Version: 2.1
 Name: zarr-eosdis-store
-Version: 0.1.3
+Version: 0.1.4
 Summary: Zarr Store class for working with EOSDIS cloud data
 Home-page: https://github.com/nasa/zarr-eosdis-store
 Author: Patrick Quinn, Matthew Hanson
 Author-email: patrick@patrickquinn.net
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: CacheControl>=0.12.6
+Requires-Dist: requests>=2.23.0
+Requires-Dist: requests-futures>=1.0.0
+Requires-Dist: zarr>=2.7.1
+Requires-Dist: ipypb~=0.5
+Requires-Dist: xarray>=0.16
+Requires-Dist: numcodecs>=0.8.1
+Provides-Extra: dev
+Requires-Dist: setuptools>=21.0.0; extra == "dev"
+Requires-Dist: pytest~=5.4; extra == "dev"
+Requires-Dist: flake8~=3.8; extra == "dev"
+Requires-Dist: safety>=1.8.5; extra == "dev"
+Requires-Dist: coverage>=4.5.4; extra == "dev"
+Requires-Dist: pygments~=2.9; extra == "dev"
+Requires-Dist: sphinx>=3.2.1; extra == "dev"
+Requires-Dist: sphinx-rtd-theme>=0.5.0; extra == "dev"
+Requires-Dist: recommonmark>=0.7.1; extra == "dev"
 
 zarr-eosdis-store
 =================
 
 The zarr-eosdis-store library allows NASA EOSDIS Collections to be accessed efficiently
 by the `Zarr Python library <https://zarr.readthedocs.io/en/stable/index.html>`_, provided they
 have a sidecar DMR++ metadata file generated.
@@ -164,9 +178,7 @@
 To check coding style::
 
     flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics
 
 To build documentation, generated at ``docs/_build/html/index.html``::
 
     cd docs && make html
-
-
```

