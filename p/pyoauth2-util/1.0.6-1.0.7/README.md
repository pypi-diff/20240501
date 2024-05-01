# Comparing `tmp/pyoauth2_util-1.0.6.tar.gz` & `tmp/pyoauth2_util-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyoauth2_util-1.0.6.tar", last modified: Mon Mar 25 13:21:20 2024, max compression
+gzip compressed data, was "pyoauth2_util-1.0.7.tar", last modified: Wed May  1 13:50:17 2024, max compression
```

## Comparing `pyoauth2_util-1.0.6.tar` & `pyoauth2_util-1.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:21:20.383617 pyoauth2_util-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-03-25 13:21:12.000000 pyoauth2_util-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-03-25 13:21:20.383617 pyoauth2_util-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-25 13:21:12.000000 pyoauth2_util-1.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:21:20.383617 pyoauth2_util-1.0.6/pyoauth2_util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 13:21:12.000000 pyoauth2_util-1.0.6/pyoauth2_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-03-25 13:21:12.000000 pyoauth2_util-1.0.6/pyoauth2_util/oauth2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:21:20.383617 pyoauth2_util-1.0.6/pyoauth2_util.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-03-25 13:21:20.000000 pyoauth2_util-1.0.6/pyoauth2_util.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-03-25 13:21:20.000000 pyoauth2_util-1.0.6/pyoauth2_util.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 13:21:20.000000 pyoauth2_util-1.0.6/pyoauth2_util.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-25 13:21:20.000000 pyoauth2_util-1.0.6/pyoauth2_util.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-25 13:21:20.000000 pyoauth2_util-1.0.6/pyoauth2_util.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 13:21:20.000000 pyoauth2_util-1.0.6/pyoauth2_util.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 13:21:20.383617 pyoauth2_util-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-03-25 13:21:12.000000 pyoauth2_util-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:50:17.460578 pyoauth2_util-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-01 13:50:02.000000 pyoauth2_util-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-01 13:50:17.460578 pyoauth2_util-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-01 13:50:02.000000 pyoauth2_util-1.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:50:17.460578 pyoauth2_util-1.0.7/pyoauth2_util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 13:50:02.000000 pyoauth2_util-1.0.7/pyoauth2_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-05-01 13:50:02.000000 pyoauth2_util-1.0.7/pyoauth2_util/oauth2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:50:17.460578 pyoauth2_util-1.0.7/pyoauth2_util.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-01 13:50:17.000000 pyoauth2_util-1.0.7/pyoauth2_util.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-01 13:50:17.000000 pyoauth2_util-1.0.7/pyoauth2_util.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 13:50:17.000000 pyoauth2_util-1.0.7/pyoauth2_util.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-01 13:50:17.000000 pyoauth2_util-1.0.7/pyoauth2_util.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-01 13:50:17.000000 pyoauth2_util-1.0.7/pyoauth2_util.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 13:50:17.000000 pyoauth2_util-1.0.7/pyoauth2_util.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 13:50:17.460578 pyoauth2_util-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-01 13:50:02.000000 pyoauth2_util-1.0.7/setup.py
```

### Comparing `pyoauth2_util-1.0.6/LICENSE` & `pyoauth2_util-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyoauth2_util-1.0.6/pyoauth2_util/oauth2.py` & `pyoauth2_util-1.0.7/pyoauth2_util/oauth2.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,15 @@
 import logging
 
 import jwt
 from jwt import exceptions
 import datetime
 from fastapi import Header, HTTPException
 from starlette import status
-from pyconfig_util.config_util import Setting
-
-setting = Setting()
+from pyconfig_util.config_util import setting
 
 
 # 创建 JWT token
 def create_token(user_id: int, is_admin: bool = True, day: int = 99999):
     """
     :param user_id: 用户id
     :param day:  日期。单位天 ，默认99999天
```

### Comparing `pyoauth2_util-1.0.6/setup.py` & `pyoauth2_util-1.0.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 with io.open("requirements.txt", 'r') as f:
     install_requires = f.read().split(os.sep)
 
 
 setup(
     name='pyoauth2_util',
-    version='1.0.6',
+    version='1.0.7',
     description='oauth2助手',
     author='buyfakett',
     author_email='buyfakett@vip.qq.com',
     license='MIT',
     url="https://github.com/buyfakett",
     packages=find_packages(),  # packages=["pytest"],
     long_description=long_description,
```

