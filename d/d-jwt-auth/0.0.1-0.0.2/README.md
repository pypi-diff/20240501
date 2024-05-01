# Comparing `tmp/d_jwt_auth-0.0.1.tar.gz` & `tmp/d_jwt_auth-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "d_jwt_auth-0.0.1.tar", last modified: Sat Apr 20 00:36:51 2024, max compression
+gzip compressed data, was "d_jwt_auth-0.0.2.tar", last modified: Wed May  1 04:48:23 2024, max compression
```

## Comparing `d_jwt_auth-0.0.1.tar` & `d_jwt_auth-0.0.2.tar`

### file list

```diff
@@ -1,45 +1,44 @@
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2024-04-20 00:36:51.345092 d_jwt_auth-0.0.1/
--rw-rw-r--   0 ali       (1000) ali       (1000)     1069 2024-04-19 07:51:05.000000 d_jwt_auth-0.0.1/LICENSE
--rw-rw-r--   0 ali       (1000) ali       (1000)    11462 2024-04-20 00:36:51.345092 d_jwt_auth-0.0.1/PKG-INFO
--rw-rw-r--   0 ali       (1000) ali       (1000)    10126 2024-04-20 00:18:39.000000 d_jwt_auth-0.0.1/README.md
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2024-04-20 00:36:51.149093 d_jwt_auth-0.0.1/config/
--rw-rw-r--   0 ali       (1000) ali       (1000)        0 2024-04-19 18:54:17.000000 d_jwt_auth-0.0.1/config/__init__.py
--rw-rw-r--   0 ali       (1000) ali       (1000)      389 2024-04-19 18:54:17.000000 d_jwt_auth-0.0.1/config/asgi.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     3266 2024-04-20 00:05:58.000000 d_jwt_auth-0.0.1/config/settings.py
--rw-rw-r--   0 ali       (1000) ali       (1000)      762 2024-04-19 18:54:17.000000 d_jwt_auth-0.0.1/config/urls.py
--rw-rw-r--   0 ali       (1000) ali       (1000)      389 2024-04-19 18:54:17.000000 d_jwt_auth-0.0.1/config/wsgi.py
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2024-04-20 00:36:51.313092 d_jwt_auth-0.0.1/d_jwt_auth/
--rw-rw-r--   0 ali       (1000) ali       (1000)        0 2024-04-19 18:34:36.000000 d_jwt_auth-0.0.1/d_jwt_auth/__init__.py
--rw-rw-r--   0 ali       (1000) ali       (1000)      144 2024-04-19 03:20:09.000000 d_jwt_auth-0.0.1/d_jwt_auth/admin.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     1926 2024-04-19 07:41:22.000000 d_jwt_auth-0.0.1/d_jwt_auth/app_settings.py
--rw-rw-r--   0 ali       (1000) ali       (1000)      150 2024-04-19 18:21:44.000000 d_jwt_auth-0.0.1/d_jwt_auth/apps.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     1594 2024-04-19 05:10:17.000000 d_jwt_auth-0.0.1/d_jwt_auth/authenticate.py
--rw-rw-r--   0 ali       (1000) ali       (1000)      560 2024-04-18 01:51:55.000000 d_jwt_auth-0.0.1/d_jwt_auth/cache.py
--rw-rw-r--   0 ali       (1000) ali       (1000)      803 2024-04-18 03:51:03.000000 d_jwt_auth-0.0.1/d_jwt_auth/client.py
--rw-rw-r--   0 ali       (1000) ali       (1000)      183 2024-04-18 03:48:12.000000 d_jwt_auth-0.0.1/d_jwt_auth/constants.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     1225 2024-04-18 15:23:34.000000 d_jwt_auth-0.0.1/d_jwt_auth/encryption.py
--rw-rw-r--   0 ali       (1000) ali       (1000)       84 2024-04-18 03:06:06.000000 d_jwt_auth-0.0.1/d_jwt_auth/exceptions.py
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2024-04-20 00:36:51.329092 d_jwt_auth-0.0.1/d_jwt_auth/migrations/
--rw-rw-r--   0 ali       (1000) ali       (1000)      928 2024-04-19 07:10:03.000000 d_jwt_auth-0.0.1/d_jwt_auth/migrations/0001_initial.py
--rw-rw-r--   0 ali       (1000) ali       (1000)        0 2023-11-27 10:37:30.000000 d_jwt_auth-0.0.1/d_jwt_auth/migrations/__init__.py
--rw-rw-r--   0 ali       (1000) ali       (1000)      863 2024-04-18 03:16:46.000000 d_jwt_auth-0.0.1/d_jwt_auth/models.py
--rw-rw-r--   0 ali       (1000) ali       (1000)      835 2024-04-19 04:51:44.000000 d_jwt_auth-0.0.1/d_jwt_auth/serializers.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     2172 2024-04-20 00:25:32.000000 d_jwt_auth-0.0.1/d_jwt_auth/services.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     4943 2024-04-19 04:48:08.000000 d_jwt_auth-0.0.1/d_jwt_auth/token.py
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2024-04-20 00:36:51.321092 d_jwt_auth-0.0.1/d_jwt_auth.egg-info/
--rw-rw-r--   0 ali       (1000) ali       (1000)    11462 2024-04-20 00:36:50.000000 d_jwt_auth-0.0.1/d_jwt_auth.egg-info/PKG-INFO
--rw-rw-r--   0 ali       (1000) ali       (1000)      861 2024-04-20 00:36:50.000000 d_jwt_auth-0.0.1/d_jwt_auth.egg-info/SOURCES.txt
--rw-rw-r--   0 ali       (1000) ali       (1000)        1 2024-04-20 00:36:50.000000 d_jwt_auth-0.0.1/d_jwt_auth.egg-info/dependency_links.txt
--rw-rw-r--   0 ali       (1000) ali       (1000)        1 2024-04-20 00:36:50.000000 d_jwt_auth-0.0.1/d_jwt_auth.egg-info/not-zip-safe
--rw-rw-r--   0 ali       (1000) ali       (1000)      108 2024-04-20 00:36:50.000000 d_jwt_auth-0.0.1/d_jwt_auth.egg-info/requires.txt
--rw-rw-r--   0 ali       (1000) ali       (1000)       18 2024-04-20 00:36:50.000000 d_jwt_auth-0.0.1/d_jwt_auth.egg-info/top_level.txt
--rw-rw-r--   0 ali       (1000) ali       (1000)       38 2024-04-20 00:36:51.345092 d_jwt_auth-0.0.1/setup.cfg
--rw-rw-r--   0 ali       (1000) ali       (1000)     1854 2024-04-19 18:05:52.000000 d_jwt_auth-0.0.1/setup.py
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2024-04-20 00:36:51.341092 d_jwt_auth-0.0.1/tests/
--rw-rw-r--   0 ali       (1000) ali       (1000)     2650 2024-04-19 18:51:44.000000 d_jwt_auth-0.0.1/tests/test_app_settings.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     1239 2024-04-19 18:51:44.000000 d_jwt_auth-0.0.1/tests/test_cache.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     6909 2024-04-19 18:51:44.000000 d_jwt_auth-0.0.1/tests/test_client.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     1439 2024-04-19 18:51:44.000000 d_jwt_auth-0.0.1/tests/test_encryption.py
--rw-rw-r--   0 ali       (1000) ali       (1000)      811 2024-04-19 18:51:44.000000 d_jwt_auth-0.0.1/tests/test_models.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     5702 2024-04-20 00:05:23.000000 d_jwt_auth-0.0.1/tests/test_services.py
--rw-rw-r--   0 ali       (1000) ali       (1000)    10697 2024-04-19 18:51:44.000000 d_jwt_auth-0.0.1/tests/test_token.py
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2024-05-01 04:48:22.970930 d_jwt_auth-0.0.2/
+-rw-rw-r--   0 ali       (1000) ali       (1000)     1069 2024-04-19 07:51:05.000000 d_jwt_auth-0.0.2/LICENSE
+-rw-rw-r--   0 ali       (1000) ali       (1000)    11696 2024-05-01 04:48:22.970930 d_jwt_auth-0.0.2/PKG-INFO
+-rw-rw-r--   0 ali       (1000) ali       (1000)    10360 2024-05-01 04:36:53.000000 d_jwt_auth-0.0.2/README.md
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2024-05-01 04:48:22.946929 d_jwt_auth-0.0.2/config/
+-rw-rw-r--   0 ali       (1000) ali       (1000)        0 2024-04-19 18:54:17.000000 d_jwt_auth-0.0.2/config/__init__.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)      389 2024-04-19 18:54:17.000000 d_jwt_auth-0.0.2/config/asgi.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     3465 2024-05-01 04:31:50.000000 d_jwt_auth-0.0.2/config/settings.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)      762 2024-04-19 18:54:17.000000 d_jwt_auth-0.0.2/config/urls.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)      389 2024-04-19 18:54:17.000000 d_jwt_auth-0.0.2/config/wsgi.py
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2024-05-01 04:48:22.950929 d_jwt_auth-0.0.2/d_jwt_auth/
+-rw-rw-r--   0 ali       (1000) ali       (1000)        0 2024-04-19 18:34:36.000000 d_jwt_auth-0.0.2/d_jwt_auth/__init__.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)      144 2024-04-19 03:20:09.000000 d_jwt_auth-0.0.2/d_jwt_auth/admin.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     2024 2024-05-01 02:17:28.000000 d_jwt_auth-0.0.2/d_jwt_auth/app_settings.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)      150 2024-04-19 18:21:44.000000 d_jwt_auth-0.0.2/d_jwt_auth/apps.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     1594 2024-04-19 05:10:17.000000 d_jwt_auth-0.0.2/d_jwt_auth/authenticate.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)      560 2024-04-18 01:51:55.000000 d_jwt_auth-0.0.2/d_jwt_auth/cache.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)      803 2024-04-18 03:51:03.000000 d_jwt_auth-0.0.2/d_jwt_auth/client.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)      183 2024-05-01 04:29:12.000000 d_jwt_auth-0.0.2/d_jwt_auth/constants.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     1225 2024-04-18 15:23:34.000000 d_jwt_auth-0.0.2/d_jwt_auth/encryption.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)       84 2024-04-18 03:06:06.000000 d_jwt_auth-0.0.2/d_jwt_auth/exceptions.py
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2024-05-01 04:48:22.950929 d_jwt_auth-0.0.2/d_jwt_auth/migrations/
+-rw-rw-r--   0 ali       (1000) ali       (1000)     1048 2024-05-01 02:45:10.000000 d_jwt_auth-0.0.2/d_jwt_auth/migrations/0001_initial.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)        0 2023-11-27 10:37:30.000000 d_jwt_auth-0.0.2/d_jwt_auth/migrations/__init__.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)      970 2024-05-01 02:29:31.000000 d_jwt_auth-0.0.2/d_jwt_auth/models.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     2919 2024-05-01 04:11:40.000000 d_jwt_auth-0.0.2/d_jwt_auth/services.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     6124 2024-05-01 04:30:10.000000 d_jwt_auth-0.0.2/d_jwt_auth/token.py
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2024-05-01 04:48:22.950929 d_jwt_auth-0.0.2/d_jwt_auth.egg-info/
+-rw-rw-r--   0 ali       (1000) ali       (1000)    11696 2024-05-01 04:48:22.000000 d_jwt_auth-0.0.2/d_jwt_auth.egg-info/PKG-INFO
+-rw-rw-r--   0 ali       (1000) ali       (1000)      835 2024-05-01 04:48:22.000000 d_jwt_auth-0.0.2/d_jwt_auth.egg-info/SOURCES.txt
+-rw-rw-r--   0 ali       (1000) ali       (1000)        1 2024-05-01 04:48:22.000000 d_jwt_auth-0.0.2/d_jwt_auth.egg-info/dependency_links.txt
+-rw-rw-r--   0 ali       (1000) ali       (1000)        1 2024-05-01 04:48:22.000000 d_jwt_auth-0.0.2/d_jwt_auth.egg-info/not-zip-safe
+-rw-rw-r--   0 ali       (1000) ali       (1000)      108 2024-05-01 04:48:22.000000 d_jwt_auth-0.0.2/d_jwt_auth.egg-info/requires.txt
+-rw-rw-r--   0 ali       (1000) ali       (1000)       18 2024-05-01 04:48:22.000000 d_jwt_auth-0.0.2/d_jwt_auth.egg-info/top_level.txt
+-rw-rw-r--   0 ali       (1000) ali       (1000)       38 2024-05-01 04:48:22.970930 d_jwt_auth-0.0.2/setup.cfg
+-rw-rw-r--   0 ali       (1000) ali       (1000)     1854 2024-05-01 04:44:33.000000 d_jwt_auth-0.0.2/setup.py
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2024-05-01 04:48:22.970930 d_jwt_auth-0.0.2/tests/
+-rw-rw-r--   0 ali       (1000) ali       (1000)     2650 2024-04-19 18:51:44.000000 d_jwt_auth-0.0.2/tests/test_app_settings.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     1239 2024-04-19 18:51:44.000000 d_jwt_auth-0.0.2/tests/test_cache.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     6909 2024-04-19 18:51:44.000000 d_jwt_auth-0.0.2/tests/test_client.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     1439 2024-04-19 18:51:44.000000 d_jwt_auth-0.0.2/tests/test_encryption.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)      811 2024-04-19 18:51:44.000000 d_jwt_auth-0.0.2/tests/test_models.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     6823 2024-05-01 02:59:28.000000 d_jwt_auth-0.0.2/tests/test_services.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)    12791 2024-05-01 04:30:31.000000 d_jwt_auth-0.0.2/tests/test_token.py
```

### Comparing `d_jwt_auth-0.0.1/LICENSE` & `d_jwt_auth-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `d_jwt_auth-0.0.1/PKG-INFO` & `d_jwt_auth-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: d_jwt_auth
-Version: 0.0.1
+Version: 0.0.2
 Summary: django-jwt-auth is an application for authenticating users with jwt in Django.
 Home-page: https://github.com/alireza-fa/django-jwt-auth
 Author: Alireza Feizi
 Author-email: alirezafeyze44@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/alireza-fa/django-jwt-auth
 Classifier: Development Status :: 5 - Production/Stable
@@ -47,14 +47,16 @@
 
 3. **Professional and highly efficient token invalidation method**
 
 4. **Ability to use caching, doubling the performance in token validation**
 
 5. **Validation access token with ip address and device && validation refresh token with device name**
 
+6. **Limit the number of devices that use an account 
+
 ## Getting Started with d_jwt_auth
 
 First, install the `d_jwt_auth` package:
 
 ```
 pip install d_jwt_auth
 ```
@@ -268,13 +270,17 @@
 This field allows you to specify whether to use caching for token validation or not. If you want to use caching, set it to `True`. Using caching can improve performance by at least two times, and significantly fewer queries are made to the database to retrieve the `UseAuth` object.
 By default, this field is set to `False`, but it is recommended to use caching.
 
 `JWT_AUTH_GET_USER_BY_ACCESS_TOKEN = False`
 
 Based on the previous explanations, if you set this field to `True`, the user information will be retrieved from the access token. By using this feature, you no longer need to query the database every time to retrieve user information, and the response time for retrieving user information can be at least two times faster.
 
+`JWT_AUTH_DEVICE_LIMIT = True`
+
+Using this field, you can specify how many devices can use the same account at the same time. If you do not specify, no limit will be considered.
+
 ## ----------------------- ----------------------
 For customizations and modifications, you have complete freedom, and you can easily personalize the package according to your project's needs.
 
 I would appreciate it if you could support me by starring this project and contributing to its improvement.
 
 I hope this package proves useful for you.
```

### Comparing `d_jwt_auth-0.0.1/README.md` & `d_jwt_auth-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 
 3. **Professional and highly efficient token invalidation method**
 
 4. **Ability to use caching, doubling the performance in token validation**
 
 5. **Validation access token with ip address and device && validation refresh token with device name**
 
+6. **Limit the number of devices that use an account 
+
 ## Getting Started with d_jwt_auth
 
 First, install the `d_jwt_auth` package:
 
 ```
 pip install d_jwt_auth
 ```
@@ -235,13 +237,17 @@
 This field allows you to specify whether to use caching for token validation or not. If you want to use caching, set it to `True`. Using caching can improve performance by at least two times, and significantly fewer queries are made to the database to retrieve the `UseAuth` object.
 By default, this field is set to `False`, but it is recommended to use caching.
 
 `JWT_AUTH_GET_USER_BY_ACCESS_TOKEN = False`
 
 Based on the previous explanations, if you set this field to `True`, the user information will be retrieved from the access token. By using this feature, you no longer need to query the database every time to retrieve user information, and the response time for retrieving user information can be at least two times faster.
 
+`JWT_AUTH_DEVICE_LIMIT = True`
+
+Using this field, you can specify how many devices can use the same account at the same time. If you do not specify, no limit will be considered.
+
 ## ----------------------- ----------------------
 For customizations and modifications, you have complete freedom, and you can easily personalize the package according to your project's needs.
 
 I would appreciate it if you could support me by starring this project and contributing to its improvement.
 
 I hope this package proves useful for you.
```

### Comparing `d_jwt_auth-0.0.1/config/settings.py` & `d_jwt_auth-0.0.2/config/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -119,8 +119,16 @@
 STATIC_URL = 'static/'
 
 # Default primary key field type
 # https://docs.djangoproject.com/en/4.2/ref/settings/#default-auto-field
 
 DEFAULT_AUTO_FIELD = 'django.db.models.BigAutoField'
 
-JWT_AUTH_CACHE_USING = True
+JWT_AUTH_CACHE_USING = False
+
+if JWT_AUTH_CACHE_USING:
+    CACHES = {
+        "default": {
+            "BACKEND": "django.core.cache.backends.redis.RedisCache",
+            "LOCATION": "redis://127.0.0.1:6379",
+        }
+    }
```

### Comparing `d_jwt_auth-0.0.1/config/urls.py` & `d_jwt_auth-0.0.2/config/urls.py`

 * *Files identical despite different names*

### Comparing `d_jwt_auth-0.0.1/d_jwt_auth/app_settings.py` & `d_jwt_auth-0.0.2/d_jwt_auth/app_settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,14 +59,18 @@
     def cache_using(self):
         return self._setting("CACHE_USING", False)
 
     @property
     def get_user_by_access_token(self):
         return self._setting("GET_USER_BY_ACCESS_TOKEN", False)
 
+    @property
+    def get_device_limit(self):
+        return self._setting("DEVICE_LIMIT", None)
+
 
 @functools.lru_cache
 def jwt_auth_app_settings() -> AppSettings:
     return AppSettings("JWT_AUTH_", get_random_bytes(32))
 
 
 app_setting = jwt_auth_app_settings()
```

### Comparing `d_jwt_auth-0.0.1/d_jwt_auth/authenticate.py` & `d_jwt_auth-0.0.2/d_jwt_auth/authenticate.py`

 * *Files identical despite different names*

### Comparing `d_jwt_auth-0.0.1/d_jwt_auth/cache.py` & `d_jwt_auth-0.0.2/d_jwt_auth/cache.py`

 * *Files identical despite different names*

### Comparing `d_jwt_auth-0.0.1/d_jwt_auth/client.py` & `d_jwt_auth-0.0.2/d_jwt_auth/client.py`

 * *Files identical despite different names*

### Comparing `d_jwt_auth-0.0.1/d_jwt_auth/encryption.py` & `d_jwt_auth-0.0.2/d_jwt_auth/encryption.py`

 * *Files identical despite different names*

### Comparing `d_jwt_auth-0.0.1/d_jwt_auth/migrations/0001_initial.py` & `d_jwt_auth-0.0.2/d_jwt_auth/migrations/0001_initial.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by Django 4.2 on 2024-04-19 07:10
+# Generated by Django 4.2 on 2024-05-01 02:45
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
 
     initial = True
@@ -14,14 +14,15 @@
         migrations.CreateModel(
             name='UserAuth',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('user_id', models.IntegerField(db_index=True, verbose_name='user id')),
                 ('token_type', models.PositiveSmallIntegerField(choices=[(1, 'access token'), (2, 'refresh token')], verbose_name='token type')),
                 ('uuid', models.UUIDField(db_index=True, unique=True, verbose_name='uuid')),
+                ('device_login_count', models.PositiveSmallIntegerField(default=0, verbose_name='device login count')),
             ],
             options={
                 'verbose_name': 'UserAuth',
                 'verbose_name_plural': 'UserAuths',
                 'ordering': ('-id',),
             },
         ),
```

### Comparing `d_jwt_auth-0.0.1/d_jwt_auth/models.py` & `d_jwt_auth-0.0.2/d_jwt_auth/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     TOKEN_TYPE_CHOICES = (
         (ACCESS_TOKEN, "access token"),
         (REFRESH_TOKEN, "refresh token")
     )
     user_id = models.IntegerField(verbose_name=_("user id"), db_index=True)
     token_type = models.PositiveSmallIntegerField(choices=TOKEN_TYPE_CHOICES, verbose_name=_("token type"))
     uuid = models.UUIDField(verbose_name=_("uuid"), unique=True, db_index=True)
+    device_login_count = models.PositiveSmallIntegerField(default=0, verbose_name=_("device login count"))
 
     class Meta:
         verbose_name = _("UserAuth")
         verbose_name_plural = _("UserAuths")
         ordering = ("-id",)
 
     def __str__(self):
```

### Comparing `d_jwt_auth-0.0.1/d_jwt_auth/services.py` & `d_jwt_auth-0.0.2/d_jwt_auth/services.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,14 +50,29 @@
 
     if app_setting.cache_using:
         set_cache(key=TOKEN_TYPE_KEY[token_type].format(user_id=user_id), value=str(user_auth.uuid), timeout=60*60*24*30)
 
     return str(user_auth.uuid)
 
 
+def get_user_auth(user_id: int, token_type: int) -> UserAuth:
+    user_auths = UserAuth.objects.filter(user_id=user_id, token_type=token_type)
+    if user_auths.exists():
+        user_auth = user_auths.first()
+        if app_setting.cache_using and not get_cache(key=TOKEN_TYPE_KEY[token_type].format(user_id=user_id)):
+            set_cache(key=TOKEN_TYPE_KEY[token_type].format(user_id=user_id), value=str(user_auth.uuid),
+                      timeout=60 * 60 * 24 * 30)
+    else:
+        user_auth = create_user_auth(user_id=user_id, token_type=token_type)
+        if app_setting.cache_using:
+            set_cache(key=TOKEN_TYPE_KEY[token_type].format(user_id=user_id), value=str(user_auth.uuid), timeout=60*60*24*30)
+
+    return user_auth
+
+
 def update_user_auth_uuid(user_id: int, token_type: int) -> str:
     user_auths = UserAuth.objects.filter(user_id=user_id, token_type=token_type)
     if user_auths.exists():
         user_auth = user_auths.first()
         user_auth = save_user_auth_uuid(user_auth=user_auth)
     else:
         user_auth = create_user_auth(user_id=user_id, token_type=token_type)
```

### Comparing `d_jwt_auth-0.0.1/d_jwt_auth/token.py` & `d_jwt_auth-0.0.2/d_jwt_auth/token.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from django.contrib.auth import get_user_model
 
 from .app_settings import app_setting
 from .constants import ACCESS_TOKEN, REFRESH_TOKEN, UUID_FIELD, USER_ID, TOKEN_TYPE, DEVICE_NAME, IP_ADDRESS
 from .encryption import encrypt, decrypt
 from .exceptions import TokenError
 from .client import get_client_info
-from .services import get_user_auth_uuid
+from .services import get_user_auth_uuid, update_user_auth_uuid, get_user_auth
 from .models import UserAuth
 
 User = get_user_model()
 
 
 class AccessToken(Token):
     lifetime = app_setting.access_token_lifetime
@@ -39,26 +39,52 @@
     for key in claims:
         claims[key] = token.get(key)
 
 
 def generate_refresh_token_with_claims(**kwargs) -> str:
     refresh_token = RefreshToken()
 
-    kwargs[UUID_FIELD] = get_user_auth_uuid(user_id=kwargs[USER_ID], token_type=UserAuth.REFRESH_TOKEN)
+    if app_setting.get_device_limit:
+        user_auth = get_user_auth(user_id=kwargs[USER_ID], token_type=UserAuth.REFRESH_TOKEN)
+        if user_auth.device_login_count >= app_setting.get_device_limit:
+            user_auth.device_login_count = 0
+            uuid = update_user_auth_uuid(user_id=kwargs[USER_ID], token_type=UserAuth.REFRESH_TOKEN)
+            kwargs[UUID_FIELD] = uuid
+            user_auth.uuid = uuid
+        else:
+            kwargs[UUID_FIELD] = str(user_auth.uuid)
+        user_auth.device_login_count += 1
+        user_auth.save()
+    else:
+        kwargs[UUID_FIELD] = get_user_auth_uuid(user_id=kwargs[USER_ID], token_type=UserAuth.REFRESH_TOKEN)
+
     set_token_claims(token=refresh_token, claims=app_setting.refresh_token_claims, **kwargs)
 
     refresh_token = encrypt_token(refresh_token)
 
     return refresh_token
 
 
 def generate_access_token_with_claims(**kwargs) -> str:
     access_token = AccessToken()
 
-    kwargs[UUID_FIELD] = get_user_auth_uuid(user_id=kwargs[USER_ID], token_type=UserAuth.ACCESS_TOKEN)
+    if app_setting.get_device_limit:
+        user_auth = get_user_auth(user_id=kwargs[USER_ID], token_type=UserAuth.ACCESS_TOKEN)
+        if user_auth.device_login_count >= app_setting.get_device_limit:
+            user_auth.device_login_count = 0
+            uuid = update_user_auth_uuid(user_id=kwargs[USER_ID], token_type=UserAuth.ACCESS_TOKEN)
+            kwargs[UUID_FIELD] = uuid
+            user_auth.uuid = uuid
+        else:
+            kwargs[UUID_FIELD] = str(user_auth.uuid)
+        user_auth.device_login_count += 1
+        user_auth.save()
+    else:
+        kwargs[UUID_FIELD] = get_user_auth_uuid(user_id=kwargs[USER_ID], token_type=UserAuth.ACCESS_TOKEN)
+
     set_token_claims(token=access_token, claims=app_setting.access_token_claims, **kwargs)
 
     access_token = encrypt_token(access_token)
 
     return access_token
 
 
@@ -140,15 +166,15 @@
     token = validate_token(request=request, raw_token=raw_refresh_token)
 
     client_info = get_client_info(request=request)
 
     validate_refresh_token(token=token, client_info=client_info)
 
     try:
-        user = User.objects.get(id=token["id"])
+        user = User.objects.get(id=token[USER_ID])
     except User.DoesNotExist as err:
         raise TokenError(err)
 
     user.last_login = now()
     user.save()
 
     return generate_access_token_with_claims(**user.__dict__, **client_info)
```

### Comparing `d_jwt_auth-0.0.1/d_jwt_auth.egg-info/PKG-INFO` & `d_jwt_auth-0.0.2/d_jwt_auth.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: d-jwt-auth
-Version: 0.0.1
+Version: 0.0.2
 Summary: django-jwt-auth is an application for authenticating users with jwt in Django.
 Home-page: https://github.com/alireza-fa/django-jwt-auth
 Author: Alireza Feizi
 Author-email: alirezafeyze44@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/alireza-fa/django-jwt-auth
 Classifier: Development Status :: 5 - Production/Stable
@@ -47,14 +47,16 @@
 
 3. **Professional and highly efficient token invalidation method**
 
 4. **Ability to use caching, doubling the performance in token validation**
 
 5. **Validation access token with ip address and device && validation refresh token with device name**
 
+6. **Limit the number of devices that use an account 
+
 ## Getting Started with d_jwt_auth
 
 First, install the `d_jwt_auth` package:
 
 ```
 pip install d_jwt_auth
 ```
@@ -268,13 +270,17 @@
 This field allows you to specify whether to use caching for token validation or not. If you want to use caching, set it to `True`. Using caching can improve performance by at least two times, and significantly fewer queries are made to the database to retrieve the `UseAuth` object.
 By default, this field is set to `False`, but it is recommended to use caching.
 
 `JWT_AUTH_GET_USER_BY_ACCESS_TOKEN = False`
 
 Based on the previous explanations, if you set this field to `True`, the user information will be retrieved from the access token. By using this feature, you no longer need to query the database every time to retrieve user information, and the response time for retrieving user information can be at least two times faster.
 
+`JWT_AUTH_DEVICE_LIMIT = True`
+
+Using this field, you can specify how many devices can use the same account at the same time. If you do not specify, no limit will be considered.
+
 ## ----------------------- ----------------------
 For customizations and modifications, you have complete freedom, and you can easily personalize the package according to your project's needs.
 
 I would appreciate it if you could support me by starring this project and contributing to its improvement.
 
 I hope this package proves useful for you.
```

### Comparing `d_jwt_auth-0.0.1/d_jwt_auth.egg-info/SOURCES.txt` & `d_jwt_auth-0.0.2/d_jwt_auth.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 d_jwt_auth/authenticate.py
 d_jwt_auth/cache.py
 d_jwt_auth/client.py
 d_jwt_auth/constants.py
 d_jwt_auth/encryption.py
 d_jwt_auth/exceptions.py
 d_jwt_auth/models.py
-d_jwt_auth/serializers.py
 d_jwt_auth/services.py
 d_jwt_auth/token.py
 d_jwt_auth.egg-info/PKG-INFO
 d_jwt_auth.egg-info/SOURCES.txt
 d_jwt_auth.egg-info/dependency_links.txt
 d_jwt_auth.egg-info/not-zip-safe
 d_jwt_auth.egg-info/requires.txt
```

### Comparing `d_jwt_auth-0.0.1/setup.py` & `d_jwt_auth-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def read(f):
     with open(f, 'r', encoding='utf-8') as file:
         return file.read()
 
 
 setup(
     name='d_jwt_auth',
-    version="0.0.1",
+    version="0.0.2",
     url='https://github.com/alireza-fa/django-jwt-auth',
     license='MIT',
     description='django-jwt-auth is an application for authenticating users with jwt in Django.',
     long_description=read('README.md'),
     long_description_content_type='text/markdown',
     author='Alireza Feizi',
     author_email='alirezafeyze44@gmail.com',
```

### Comparing `d_jwt_auth-0.0.1/tests/test_app_settings.py` & `d_jwt_auth-0.0.2/tests/test_app_settings.py`

 * *Files identical despite different names*

### Comparing `d_jwt_auth-0.0.1/tests/test_cache.py` & `d_jwt_auth-0.0.2/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `d_jwt_auth-0.0.1/tests/test_client.py` & `d_jwt_auth-0.0.2/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `d_jwt_auth-0.0.1/tests/test_encryption.py` & `d_jwt_auth-0.0.2/tests/test_encryption.py`

 * *Files identical despite different names*

### Comparing `d_jwt_auth-0.0.1/tests/test_models.py` & `d_jwt_auth-0.0.2/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `d_jwt_auth-0.0.1/tests/test_services.py` & `d_jwt_auth-0.0.2/tests/test_services.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import uuid
 
 from django.test import TestCase
 from django.contrib.auth import get_user_model
+from django.test import override_settings
 
 from d_jwt_auth.services import create_user_auth, get_user_auth_uuid, ACCESS_UUID_CACHE_KEY, \
-    REFRESH_UUID_CACHE_KEY, update_user_auth_uuid
+    REFRESH_UUID_CACHE_KEY, update_user_auth_uuid, get_user_auth
 from d_jwt_auth.models import UserAuth
 from d_jwt_auth.cache import get_cache, clear_all_cache
 from d_jwt_auth.app_settings import app_setting
 
 User = get_user_model()
 
 
@@ -112,7 +113,27 @@
 
     def test_get_uuid_from_database_once(self):
         clear_all_cache()
         get_user_auth_uuid(user_id=self.user.id, token_type=UserAuth.REFRESH_TOKEN)
         UserAuth.objects.all().delete()
         uuid_field_from_cache = get_user_auth_uuid(user_id=self.user.id, token_type=UserAuth.REFRESH_TOKEN)
         self.assertIsNotNone(uuid_field_from_cache)
+
+    def test_get_user_auth_access_token(self):
+        user_auth = get_user_auth(user_id=self.user.id, token_type=UserAuth.ACCESS_TOKEN)
+        self.assertEqual(user_auth.token_type, UserAuth.ACCESS_TOKEN)
+
+    def test_get_user_auth_refresh_token(self):
+        user_auth = get_user_auth(user_id=self.user.id, token_type=UserAuth.REFRESH_TOKEN)
+        self.assertEqual(user_auth.token_type, UserAuth.REFRESH_TOKEN)
+
+    def test_get_user_auth_create_once(self):
+        user_auth = get_user_auth(user_id=self.user.id, token_type=UserAuth.REFRESH_TOKEN)
+        user_auth2 = get_user_auth(user_id=self.user.id, token_type=UserAuth.REFRESH_TOKEN)
+        self.assertEqual(user_auth2.uuid, user_auth.uuid)
+
+    @override_settings(JWY_AUTH_USING_CACHE=True)
+    def tset_get_user_auth_cache_uuid(self):
+        clear_all_cache()
+        user_auth = get_user_auth(user_id=self.user.id, token_type=UserAuth.ACCESS_TOKEN)
+        uuid_cache = get_cache(key=ACCESS_UUID_CACHE_KEY.format(user_id=self.user.id))
+        self.assertEqual(str(user_auth.uuid), uuid_cache)
```

### Comparing `d_jwt_auth-0.0.1/tests/test_token.py` & `d_jwt_auth-0.0.2/tests/test_token.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from django.test import TestCase
 from django.contrib.auth import get_user_model
+from django.test import override_settings
 
 from rest_framework.test import APIRequestFactory
 from model_bakery import baker
 
 from d_jwt_auth.token import AccessToken, RefreshToken, set_token_claims, get_token_claims, generate_refresh_token_with_claims, \
     generate_access_token_with_claims, encrypt_token, decrypt_token, validate_refresh_token, validate_access_token, \
     validate_token, get_user_by_access_token, generate_token, refresh_access_token
@@ -176,14 +177,46 @@
         request.META["REMOTE_ADDR"] = self.ip_address
         request.META["HTTP_USER_AGENT"] = self.device_name
         token = validate_token(request=request, raw_token=token)
         self.assertEqual(token["token_type"], REFRESH_TOKEN)
         uuid_field = get_user_auth_uuid(user_id=self.user_id, token_type=UserAuth.REFRESH_TOKEN)
         self.assertEqual(uuid_field, token[UUID_FIELD])
 
+    @override_settings(JWT_AUTH_DEVICE_LIMIT=2)
+    def test_generate_refresh_token_with_claims_device_limit(self):
+        request = APIRequestFactory().get(path="/")
+        request.META["REMOTE_ADDR"] = self.ip_address
+        request.META["HTTP_USER_AGENT"] = self.device_name
+        token1 = generate_refresh_token_with_claims(**{**self.user.__dict__, **self.client_info})
+        self.assertIsNotNone(validate_token(request=request, raw_token=token1))
+        token2 = generate_refresh_token_with_claims(**{**self.user.__dict__, **self.client_info})
+        self.assertIsNotNone(validate_token(request=request, raw_token=token2))
+        token3 = generate_refresh_token_with_claims(**{**self.user.__dict__, **self.client_info})
+        self.assertIsNotNone(validate_token(request=request, raw_token=token3))
+        with self.assertRaises(TokenError):
+            validate_token(request=request, raw_token=token1)
+        with self.assertRaises(TokenError):
+            validate_token(request=request, raw_token=token2)
+
+    @override_settings(JWT_AUTH_DEVICE_LIMIT=2)
+    def test_generate_access_token_with_claims_device_limit(self):
+        request = APIRequestFactory().get(path="/")
+        request.META["REMOTE_ADDR"] = self.ip_address
+        request.META["HTTP_USER_AGENT"] = self.device_name
+        token1 = generate_access_token_with_claims(**{**self.user.__dict__, **self.client_info})
+        self.assertIsNotNone(validate_token(request=request, raw_token=token1))
+        token2 = generate_access_token_with_claims(**{**self.user.__dict__, **self.client_info})
+        self.assertIsNotNone(validate_token(request=request, raw_token=token2))
+        token3 = generate_access_token_with_claims(**{**self.user.__dict__, **self.client_info})
+        self.assertIsNotNone(validate_token(request=request, raw_token=token3))
+        with self.assertRaises(TokenError):
+            validate_token(request=request, raw_token=token1)
+        with self.assertRaises(TokenError):
+            validate_token(request=request, raw_token=token2)
+
     def test_generate_access_token_with_claims(self):
         token = generate_access_token_with_claims(**{**self.user.__dict__, **self.client_info})
         request = APIRequestFactory().get(path="/")
         request.META["REMOTE_ADDR"] = self.ip_address
         request.META["HTTP_USER_AGENT"] = self.device_name
         token = validate_token(request=request, raw_token=token)
         self.assertEqual(token["token_type"], ACCESS_TOKEN)
```

