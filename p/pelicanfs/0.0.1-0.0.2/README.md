# Comparing `tmp/pelicanfs-0.0.1.tar.gz` & `tmp/pelicanfs-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pelicanfs-0.0.1.tar", last modified: Tue Apr 16 20:35:42 2024, max compression
+gzip compressed data, was "pelicanfs-0.0.2.tar", last modified: Wed May  1 00:21:28 2024, max compression
```

## Comparing `pelicanfs-0.0.1.tar` & `pelicanfs-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,18 @@
-drwxr-xr-x   0 useradmin   (503) staff       (20)        0 2024-04-16 20:35:42.006247 pelicanfs-0.0.1/
--rw-r--r--   0 useradmin   (503) staff       (20)    11357 2024-02-23 17:09:37.000000 pelicanfs-0.0.1/LICENSE
--rw-r--r--   0 useradmin   (503) staff       (20)     1200 2024-04-16 20:35:42.006176 pelicanfs-0.0.1/PKG-INFO
--rw-r--r--   0 useradmin   (503) staff       (20)     1794 2024-04-16 17:37:17.000000 pelicanfs-0.0.1/README.md
--rw-r--r--   0 useradmin   (503) staff       (20)      167 2024-04-16 16:33:12.000000 pelicanfs-0.0.1/pyproject.toml
--rw-r--r--   0 useradmin   (503) staff       (20)      181 2024-04-16 20:35:42.006517 pelicanfs-0.0.1/setup.cfg
--rw-r--r--   0 useradmin   (503) staff       (20)     1543 2024-04-16 20:35:07.000000 pelicanfs-0.0.1/setup.py
-drwxr-xr-x   0 useradmin   (503) staff       (20)        0 2024-04-16 20:35:42.002431 pelicanfs-0.0.1/src/
-drwxr-xr-x   0 useradmin   (503) staff       (20)        0 2024-04-16 20:35:42.004497 pelicanfs-0.0.1/src/pelicanfs/
--rw-r--r--   0 useradmin   (503) staff       (20)        0 2024-04-09 19:50:20.000000 pelicanfs-0.0.1/src/pelicanfs/__init__.py
--rw-r--r--   0 useradmin   (503) staff       (20)    10002 2024-04-16 15:59:20.000000 pelicanfs-0.0.1/src/pelicanfs/core.py
--rw-r--r--   0 useradmin   (503) staff       (20)     1868 2024-04-15 14:56:27.000000 pelicanfs-0.0.1/src/pelicanfs/dir_header_parser.py
-drwxr-xr-x   0 useradmin   (503) staff       (20)        0 2024-04-16 20:35:42.005900 pelicanfs-0.0.1/src/pelicanfs.egg-info/
--rw-r--r--   0 useradmin   (503) staff       (20)     1200 2024-04-16 20:35:41.000000 pelicanfs-0.0.1/src/pelicanfs.egg-info/PKG-INFO
--rw-r--r--   0 useradmin   (503) staff       (20)      339 2024-04-16 20:35:42.000000 pelicanfs-0.0.1/src/pelicanfs.egg-info/SOURCES.txt
--rw-r--r--   0 useradmin   (503) staff       (20)        1 2024-04-16 20:35:41.000000 pelicanfs-0.0.1/src/pelicanfs.egg-info/dependency_links.txt
--rw-r--r--   0 useradmin   (503) staff       (20)      141 2024-04-16 20:35:41.000000 pelicanfs-0.0.1/src/pelicanfs.egg-info/requires.txt
--rw-r--r--   0 useradmin   (503) staff       (20)       10 2024-04-16 20:35:41.000000 pelicanfs-0.0.1/src/pelicanfs.egg-info/top_level.txt
-drwxr-xr-x   0 useradmin   (503) staff       (20)        0 2024-04-16 20:35:42.005606 pelicanfs-0.0.1/tests/
--rw-r--r--   0 useradmin   (503) staff       (20)      838 2024-04-09 21:23:46.000000 pelicanfs-0.0.1/tests/test_fsspec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:21:28.595954 pelicanfs-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-01 00:21:21.000000 pelicanfs-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-05-01 00:21:28.595954 pelicanfs-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-01 00:21:21.000000 pelicanfs-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-01 00:21:21.000000 pelicanfs-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-01 00:21:28.595954 pelicanfs-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-01 00:21:21.000000 pelicanfs-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:21:28.591954 pelicanfs-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:21:28.595954 pelicanfs-0.0.2/src/pelicanfs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 00:21:21.000000 pelicanfs-0.0.2/src/pelicanfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10194 2024-05-01 00:21:21.000000 pelicanfs-0.0.2/src/pelicanfs/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-01 00:21:21.000000 pelicanfs-0.0.2/src/pelicanfs/dir_header_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:21:28.595954 pelicanfs-0.0.2/src/pelicanfs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-05-01 00:21:28.000000 pelicanfs-0.0.2/src/pelicanfs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-01 00:21:28.000000 pelicanfs-0.0.2/src/pelicanfs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 00:21:28.000000 pelicanfs-0.0.2/src/pelicanfs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-01 00:21:28.000000 pelicanfs-0.0.2/src/pelicanfs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-01 00:21:28.000000 pelicanfs-0.0.2/src/pelicanfs.egg-info/top_level.txt
```

### Comparing `pelicanfs-0.0.1/LICENSE` & `pelicanfs-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pelicanfs-0.0.1/README.md` & `pelicanfs-0.0.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,57 @@
 # PelicanFS
 
 ## Overview
 
-PelicanFS is a file system interface (fsspec) for the Pelican Platform.  For more information about the Pelican Platform, please visit the [Pelican Platform](https://pelicanplatform.org) and the [Pelican Platform Github](https://github.com/PelicanPlatform/pelican) pages. For more information about fsspec, visit the [filesystem-spec](https://filesystem-spec.readthedocs.io/en/latest/index.html) page.
+PelicanFS is a file system interface (fsspec) for the Pelican Platform.  For more information about pelican, see our [main website](https://pelicanplatform.org) or [Github page](https://github.com/PelicanPlatform/pelican). For more information about fsspec, visit the [filesystem-spec](https://filesystem-spec.readthedocs.io/en/latest/index.html) page.
 
 
 ## Limitations
 
 PelicanFS is built on top of the http fsspec implementation. As such, any functionality that isn’t available in the http implementation is also *not* available in PelicanFS.
 
 ### Installation
 
-To install pelican, run:```pip install pelicanfs```### Using PelicanFS
+To install pelican, run:
+
+```
+pip install pelicanfs
+```
+
+To install from source, run:
+
+```
+git clone https://github.com/PelicanPlatform/pelicanfs.git
+cd pelicanfs
+pip install -e .
+```
+
+
+### Using PelicanFS
 
 To use pelicanfs, first create a `PelicanFileSystem` and provide it with the url for the director of your data federation. As an example using the OSDF director
 
 ```python
 from pelicanfs.core import PelicanFileSystem
 
 pelfs = PelicanFileSystem("https://osdf-director.osg-htc.org/")
 ```
 
-From there, use `pelfs` as you would an http fsspec using a namespace path as the url path. For example:
+Once `pelfs` is pointed at your federation's director, fsspec commands can be applied to Pelican namespaces. For example:
 
 ```python
 hello_world = pelfs.cat('/ospool/uc-shared/public/OSG-Staff/validation/test.txt')
 print(hello_world)
 ```
 
 ### Getting an FSMap
 
 Sometimes various systems that interact with an fsspec want a key-value mapper rather than a url. To do that, call the `PelicanMap` function with the namespace path and a `PelicanFileSystem` object rather than using the fsspec `get_mapper` call. For example
 
 ```python
 from pelicanfs.core import PelicanFileSystem, PelicanMap
 
 pelfs = PelicanFileSystem(“some-director-url”)
-file1 = PelicanMap(“namespace/file/1”, pelfs=pelfs)
-file2 = PelicanMap(“namespace/file/2”, pelfs=pelfs)
+file1 = PelicanMap(“/namespace/file/1”, pelfs=pelfs)
+file2 = PelicanMap(“/namespace/file/2”, pelfs=pelfs)
 ds = xarray.open_mfdataset([file1,file2], engine='zarr')
 ```
```

### Comparing `pelicanfs-0.0.1/setup.py` & `pelicanfs-0.0.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 packages = find_packages()
 print(packages)
 
 setup(
     name="pelicanfs",
-    version="0.0.1",
+    version="0.0.2",
     description="An FSSpec Implementation using the Pelican System",
     url = "https://github.com/PelicanPlatform/pelicanfs",
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Science/Research",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
@@ -20,14 +20,16 @@
         "License :: OSI Approved :: Apache Software License",
     ],
     keywords="pelican, fsspec",
         packages=find_packages(
         where='src',
         include=['pelicanfs*'],
     ),
+    long_description=open('README.md').read(),
+    long_description_content_type='text/markdown',
     package_dir={"": "src"},
     python_requires=">=3.7, <4",
     install_requires=["aiohttp==3.9.4", 
                       "aiosignal==1.3.1",
                       "async-timeout==4.0.3",
                       "attrs==23.2.0",
                       "frozenlist==1.4.1",
@@ -36,8 +38,8 @@
                       "multidict==6.0.5",
                       "yarl==1.9.4"],
     project_urls={
         "Source": "https://github.com/PelicanPlatform/pelicanfs",
         "Pelican Source": "https://github.com/PelicanPlatform/pelican",
         "Bug Reports":"https://github.com/PelicanPlatform/pelicanfs/issues"
     },
-)
+)
```

### Comparing `pelicanfs-0.0.1/src/pelicanfs/core.py` & `pelicanfs-0.0.2/src/pelicanfs/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,20 +94,20 @@
         metalist = parse_metalink(headers)[1:]
         while len(metalist) > 0:
             updatedUrl = metalist[0][0]
             metalist = metalist[1:]
             # Timeout response in seconds - the default response is 5 minutes
             timeout = aiohttp.ClientTimeout(total=2)
             async with aiohttp.ClientSession() as session:
-                async with session.get(updatedUrl, timeout=timeout) as resp:
-                    try:
+                try:
+                    async with session.get(updatedUrl, timeout=timeout) as resp:
                         resp.status
-                    except (aiohttp.client_exceptions.ClientConnectorError, FileNotFoundError, asyncio.TimeoutError):
-                        continue
-                    break
+                except (aiohttp.client_exceptions.ClientConnectorError, FileNotFoundError, asyncio.TimeoutError, asyncio.exceptions.TimeoutError):
+                    continue
+                break
         if len(metalist) == 0:
             # No working cache was found
             raise RuntimeError
         
         return updatedUrl
 
     
@@ -220,14 +220,18 @@
                         cUrl = cacheUrl = await self.get_working_cache(parsedUrl.path)
                     cacheUrl.append(cUrl)
             result = await func(self, cacheUrl, *args[1:], **kwargs)
             return result
         return wrapper
 
     @_cache_dec
+    async def open_async(self, path, mode="rb", size=None, **kwargs):
+        return await self.httpFileSystem.open_async(path, mode, size, **kwargs)
+    
+    @_cache_dec
     async def _cat_file(self, path, start=None, end=None, **kwargs):
         return await self.httpFileSystem._cat_file(path, start, end, **kwargs)
 
     @_cache_dec
     async def _exists(self, path, **kwargs):
         return await self.httpFileSystem._exists(path, **kwargs)
```

### Comparing `pelicanfs-0.0.1/src/pelicanfs/dir_header_parser.py` & `pelicanfs-0.0.2/src/pelicanfs/dir_header_parser.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,8 @@
-"""
-Copyright (C) 2024, Pelican Project, Morgridge Institute for Research
- 
-Licensed under the Apache License, Version 2.0 (the "License"); you
-may not use this file except in compliance with the License.  You may
-obtain a copy of the License at
- 
-    http://www.apache.org/licenses/LICENSE-2.0
- 
-Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-See the License for the specific language governing permissions and
-limitations under the License. 
-"""
 
-
-"""
-Code to parse the headers returned by a GET call to the director
-"""
 def parse_metalink(headers={}):
     """
     Parse the metalink headers to get a list of caches to attempt to try in priority orider
     """
     linkPrio = []
 
     if "Link" in headers:
```

