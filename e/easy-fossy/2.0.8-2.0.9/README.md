# Comparing `tmp/easy_fossy-2.0.8.tar.gz` & `tmp/easy_fossy-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_fossy-2.0.8.tar", max compression
+gzip compressed data, was "easy_fossy-2.0.9.tar", max compression
```

## Comparing `easy_fossy-2.0.8.tar` & `easy_fossy-2.0.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0     1089 2024-02-13 20:02:56.662156 easy_fossy-2.0.8/LICENSE
--rwxr-xr-x   0        0        0     7135 2024-02-13 20:23:00.389925 easy_fossy-2.0.8/README.md
--rwxr-xr-x   0        0        0    52256 2024-02-13 20:20:15.634316 easy_fossy-2.0.8/easy_fossy/__init__.py
--rwxr-xr-x   0        0        0    19105 2024-02-13 21:32:48.577321 easy_fossy-2.0.8/easy_fossy/models.py
--rwxr-xr-x   0        0        0      612 2024-02-13 21:33:21.695690 easy_fossy-2.0.8/pyproject.toml
--rw-r--r--   0        0        0     7735 1970-01-01 00:00:00.000000 easy_fossy-2.0.8/PKG-INFO
+-rwxr-xr-x   0        0        0     1089 2024-02-13 20:02:56.662156 easy_fossy-2.0.9/LICENSE
+-rwxr-xr-x   0        0        0     7135 2024-02-13 20:23:00.389925 easy_fossy-2.0.9/README.md
+-rwxr-xr-x   0        0        0    52272 2024-02-13 21:42:14.060276 easy_fossy-2.0.9/easy_fossy/__init__.py
+-rwxr-xr-x   0        0        0    19105 2024-02-13 21:37:08.139628 easy_fossy-2.0.9/easy_fossy/models.py
+-rwxr-xr-x   0        0        0      612 2024-02-13 21:42:32.847998 easy_fossy-2.0.9/pyproject.toml
+-rw-r--r--   0        0        0     7735 1970-01-01 00:00:00.000000 easy_fossy-2.0.9/PKG-INFO
```

### Comparing `easy_fossy-2.0.8/LICENSE` & `easy_fossy-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `easy_fossy-2.0.8/README.md` & `easy_fossy-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `easy_fossy-2.0.8/easy_fossy/__init__.py` & `easy_fossy-2.0.9/easy_fossy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,15 +148,15 @@
 
         response = requests.request(
             "GET", self.url + str("users"), data=payload, headers=headers
         )
 
         match response.json():
             case [*args]:
-                users = [User(**user) for user in args]
+                users = [print(user) and User(**user) for user in args]
                 # for j in jobs:
                 #     print(jobs)
                 return users
             case _:
                 print(response.text)
 
     # get_all_users()
```

### Comparing `easy_fossy-2.0.8/easy_fossy/models.py` & `easy_fossy-2.0.9/easy_fossy/models.py`

 * *Files identical despite different names*

### Comparing `easy_fossy-2.0.8/pyproject.toml` & `easy_fossy-2.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "easy_fossy"
-version = "2.0.8"
+version = "2.0.9"
 description = "fossology API wrapper in python 3.10"
 authors = ["dinesh_ravi"]
 license = "MIT License"
 readme = "README.md"
 
 [tool.poetry.scripts]
 easy_fossy = 'easy_fossy:easy_fossy'
```

### Comparing `easy_fossy-2.0.8/PKG-INFO` & `easy_fossy-2.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy_fossy
-Version: 2.0.8
+Version: 2.0.9
 Summary: fossology API wrapper in python 3.10
 License: MIT
 Author: dinesh_ravi
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

