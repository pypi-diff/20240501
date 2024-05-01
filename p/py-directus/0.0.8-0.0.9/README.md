# Comparing `tmp/py_directus-0.0.8.tar.gz` & `tmp/py_directus-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_directus-0.0.8.tar", last modified: Mon Nov 13 19:20:53 2023, max compression
+gzip compressed data, was "py_directus-0.0.9.tar", last modified: Mon Nov 13 19:22:18 2023, max compression
```

## Comparing `py_directus-0.0.8.tar` & `py_directus-0.0.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 19:20:53.477808 py_directus-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)    10533 2023-11-13 19:20:53.477808 py_directus-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10130 2023-11-13 19:20:50.000000 py_directus-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 19:20:53.473808 py_directus-0.0.8/py_directus/
--rw-r--r--   0 runner    (1001) docker     (127)      257 2023-11-13 19:20:50.000000 py_directus-0.0.8/py_directus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3825 2023-11-13 19:20:50.000000 py_directus-0.0.8/py_directus/aggregator.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7890 2023-11-13 19:20:50.000000 py_directus-0.0.8/py_directus/directus.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8171 2023-11-13 19:20:50.000000 py_directus-0.0.8/py_directus/directus_request.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5232 2023-11-13 19:20:50.000000 py_directus-0.0.8/py_directus/directus_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2023-11-13 19:20:50.000000 py_directus-0.0.8/py_directus/expression.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 19:20:53.477808 py_directus-0.0.8/py_directus/fast_api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-13 19:20:50.000000 py_directus-0.0.8/py_directus/fast_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3475 2023-11-13 19:20:50.000000 py_directus-0.0.8/py_directus/fast_api/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      329 2023-11-13 19:20:50.000000 py_directus-0.0.8/py_directus/fast_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2023-11-13 19:20:50.000000 py_directus-0.0.8/py_directus/fast_api/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2023-11-13 19:20:50.000000 py_directus-0.0.8/py_directus/fast_api/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3989 2023-11-13 19:20:50.000000 py_directus-0.0.8/py_directus/filter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      634 2023-11-13 19:20:50.000000 py_directus-0.0.8/py_directus/models.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1870 2023-11-13 19:20:50.000000 py_directus-0.0.8/py_directus/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2023-11-13 19:20:50.000000 py_directus-0.0.8/py_directus/transformation.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2023-11-13 19:20:50.000000 py_directus-0.0.8/py_directus/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 19:20:53.477808 py_directus-0.0.8/py_directus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10533 2023-11-13 19:20:53.000000 py_directus-0.0.8/py_directus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      670 2023-11-13 19:20:53.000000 py_directus-0.0.8/py_directus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-13 19:20:53.000000 py_directus-0.0.8/py_directus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-13 19:20:53.000000 py_directus-0.0.8/py_directus.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      183 2023-11-13 19:20:53.000000 py_directus-0.0.8/py_directus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-11-13 19:20:53.000000 py_directus-0.0.8/py_directus.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-13 19:20:53.477808 py_directus-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2023-11-13 19:20:51.000000 py_directus-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 19:22:18.365889 py_directus-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    10533 2023-11-13 19:22:18.365889 py_directus-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10130 2023-11-13 19:22:12.000000 py_directus-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 19:22:18.361889 py_directus-0.0.9/py_directus/
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2023-11-13 19:22:12.000000 py_directus-0.0.9/py_directus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3825 2023-11-13 19:22:12.000000 py_directus-0.0.9/py_directus/aggregator.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7890 2023-11-13 19:22:12.000000 py_directus-0.0.9/py_directus/directus.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8171 2023-11-13 19:22:12.000000 py_directus-0.0.9/py_directus/directus_request.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5232 2023-11-13 19:22:12.000000 py_directus-0.0.9/py_directus/directus_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2023-11-13 19:22:12.000000 py_directus-0.0.9/py_directus/expression.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 19:22:18.365889 py_directus-0.0.9/py_directus/fast_api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-13 19:22:12.000000 py_directus-0.0.9/py_directus/fast_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3475 2023-11-13 19:22:12.000000 py_directus-0.0.9/py_directus/fast_api/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2023-11-13 19:22:12.000000 py_directus-0.0.9/py_directus/fast_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2023-11-13 19:22:12.000000 py_directus-0.0.9/py_directus/fast_api/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2023-11-13 19:22:12.000000 py_directus-0.0.9/py_directus/fast_api/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3989 2023-11-13 19:22:12.000000 py_directus-0.0.9/py_directus/filter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      634 2023-11-13 19:22:12.000000 py_directus-0.0.9/py_directus/models.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1870 2023-11-13 19:22:12.000000 py_directus-0.0.9/py_directus/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2023-11-13 19:22:12.000000 py_directus-0.0.9/py_directus/transformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2023-11-13 19:22:12.000000 py_directus-0.0.9/py_directus/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 19:22:18.361889 py_directus-0.0.9/py_directus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10533 2023-11-13 19:22:18.000000 py_directus-0.0.9/py_directus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2023-11-13 19:22:18.000000 py_directus-0.0.9/py_directus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-13 19:22:18.000000 py_directus-0.0.9/py_directus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-13 19:22:18.000000 py_directus-0.0.9/py_directus.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2023-11-13 19:22:18.000000 py_directus-0.0.9/py_directus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2023-11-13 19:22:18.000000 py_directus-0.0.9/py_directus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-13 19:22:18.365889 py_directus-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2023-11-13 19:22:14.000000 py_directus-0.0.9/setup.py
```

### Comparing `py_directus-0.0.8/PKG-INFO` & `py_directus-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_directus
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python wrapper for asynchronous interaction with Directus
 Home-page: https://github.com/panos-stavrianos/py-directus
 Author: Panos Stavrianos
 Author-email: panos@orbitsystems.gr
 License: MIT license
 Keywords: directus,async,wrapper,api,python,asyncio
 Requires-Python: >=3.6
```

### Comparing `py_directus-0.0.8/README.md` & `py_directus-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `py_directus-0.0.8/py_directus/aggregator.py` & `py_directus-0.0.9/py_directus/aggregator.py`

 * *Files identical despite different names*

### Comparing `py_directus-0.0.8/py_directus/directus.py` & `py_directus-0.0.9/py_directus/directus.py`

 * *Files identical despite different names*

### Comparing `py_directus-0.0.8/py_directus/directus_request.py` & `py_directus-0.0.9/py_directus/directus_request.py`

 * *Files identical despite different names*

### Comparing `py_directus-0.0.8/py_directus/directus_response.py` & `py_directus-0.0.9/py_directus/directus_response.py`

 * *Files identical despite different names*

### Comparing `py_directus-0.0.8/py_directus/fast_api/auth.py` & `py_directus-0.0.9/py_directus/fast_api/auth.py`

 * *Files identical despite different names*

### Comparing `py_directus-0.0.8/py_directus/fast_api/globals.py` & `py_directus-0.0.9/py_directus/fast_api/globals.py`

 * *Files identical despite different names*

### Comparing `py_directus-0.0.8/py_directus/fast_api/utils.py` & `py_directus-0.0.9/py_directus/fast_api/utils.py`

 * *Files identical despite different names*

### Comparing `py_directus-0.0.8/py_directus/filter.py` & `py_directus-0.0.9/py_directus/filter.py`

 * *Files identical despite different names*

### Comparing `py_directus-0.0.8/py_directus/models.py` & `py_directus-0.0.9/py_directus/models.py`

 * *Files identical despite different names*

### Comparing `py_directus-0.0.8/py_directus/operators.py` & `py_directus-0.0.9/py_directus/operators.py`

 * *Files identical despite different names*

### Comparing `py_directus-0.0.8/py_directus/transformation.py` & `py_directus-0.0.9/py_directus/transformation.py`

 * *Files identical despite different names*

### Comparing `py_directus-0.0.8/py_directus.egg-info/PKG-INFO` & `py_directus-0.0.9/py_directus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-directus
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python wrapper for asynchronous interaction with Directus
 Home-page: https://github.com/panos-stavrianos/py-directus
 Author: Panos Stavrianos
 Author-email: panos@orbitsystems.gr
 License: MIT license
 Keywords: directus,async,wrapper,api,python,asyncio
 Requires-Python: >=3.6
```

### Comparing `py_directus-0.0.8/py_directus.egg-info/SOURCES.txt` & `py_directus-0.0.9/py_directus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py_directus-0.0.8/setup.py` & `py_directus-0.0.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with open('requirements.txt') as requirements_file:
     requirements = requirements_file.readlines()
 
 with open('fastapi_requirements.txt') as fastapi_requirements_file:
     fastapi_requirements = fastapi_requirements_file.readlines()
 
 readme = Path('README.md').read_text()
-version = '0.0.8'
+version = '0.0.9'
 if "VERSION_PLACEHOLDER" in version:
     version = '0.0.8'
 setup(
     author="Panos Stavrianos",
     author_email='panos@orbitsystems.gr',
     python_requires='>=3.6',
     description="Python wrapper for asynchronous interaction with Directus",
@@ -29,10 +29,8 @@
     include_package_data=True,
     keywords=['directus', 'async', 'wrapper', 'api', 'python', 'asyncio'],
     name='py_directus',
     packages=find_packages(include=['py_directus', 'py_directus.*']),
     url='https://github.com/panos-stavrianos/py-directus',
     version=version,
     zip_safe=False
-)
-
-#     version='0.0.8',
+)
```

