# Comparing `tmp/django-cache-helper-1.0.4.tar.gz` & `tmp/django_cache_helper-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-cache-helper-1.0.4.tar", last modified: Fri Jun 23 18:00:30 2023, max compression
+gzip compressed data, was "django_cache_helper-1.0.5.tar", last modified: Wed May  1 13:41:10 2024, max compression
```

## Comparing `django-cache-helper-1.0.4.tar` & `django_cache_helper-1.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 kevinfox   (501) wheel        (0)        0 2023-06-23 18:00:30.662915 django-cache-helper-1.0.4/
--rw-r--r--   0 kevinfox   (501) wheel        (0)     3466 2023-06-23 18:00:30.662485 django-cache-helper-1.0.4/PKG-INFO
--rw-r--r--   0 kevinfox   (501) wheel        (0)     2884 2022-11-10 14:29:26.000000 django-cache-helper-1.0.4/README.md
-drwxr-xr-x   0 kevinfox   (501) wheel        (0)        0 2023-06-23 18:00:30.657465 django-cache-helper-1.0.4/cache_helper/
--rw-r--r--   0 kevinfox   (501) wheel        (0)       20 2023-06-23 18:00:09.000000 django-cache-helper-1.0.4/cache_helper/__init__.py
--rw-r--r--   0 kevinfox   (501) wheel        (0)     7482 2023-06-23 18:00:09.000000 django-cache-helper-1.0.4/cache_helper/decorators.py
--rw-r--r--   0 kevinfox   (501) wheel        (0)      110 2022-11-10 14:16:47.000000 django-cache-helper-1.0.4/cache_helper/exceptions.py
--rw-r--r--   0 kevinfox   (501) wheel        (0)      470 2020-01-15 18:19:24.000000 django-cache-helper-1.0.4/cache_helper/interfaces.py
--rw-r--r--   0 kevinfox   (501) wheel        (0)       94 2022-11-10 14:16:47.000000 django-cache-helper-1.0.4/cache_helper/settings.py
--rw-r--r--   0 kevinfox   (501) wheel        (0)     4323 2022-11-10 14:16:47.000000 django-cache-helper-1.0.4/cache_helper/utils.py
-drwxr-xr-x   0 kevinfox   (501) wheel        (0)        0 2023-06-23 18:00:30.661822 django-cache-helper-1.0.4/django_cache_helper.egg-info/
--rw-r--r--   0 kevinfox   (501) wheel        (0)     3466 2023-06-23 18:00:30.000000 django-cache-helper-1.0.4/django_cache_helper.egg-info/PKG-INFO
--rw-r--r--   0 kevinfox   (501) wheel        (0)      349 2023-06-23 18:00:30.000000 django-cache-helper-1.0.4/django_cache_helper.egg-info/SOURCES.txt
--rw-r--r--   0 kevinfox   (501) wheel        (0)        1 2023-06-23 18:00:30.000000 django-cache-helper-1.0.4/django_cache_helper.egg-info/dependency_links.txt
--rw-r--r--   0 kevinfox   (501) wheel        (0)       13 2023-06-23 18:00:30.000000 django-cache-helper-1.0.4/django_cache_helper.egg-info/top_level.txt
--rw-r--r--   0 kevinfox   (501) wheel        (0)      841 2022-11-10 14:26:01.000000 django-cache-helper-1.0.4/pyproject.toml
--rw-r--r--   0 kevinfox   (501) wheel        (0)       38 2023-06-23 18:00:30.663080 django-cache-helper-1.0.4/setup.cfg
+drwxr-xr-x   0 anthonypanat   (502) staff       (20)        0 2024-05-01 13:41:10.404427 django_cache_helper-1.0.5/
+-rw-r--r--   0 anthonypanat   (502) staff       (20)     3466 2024-05-01 13:41:10.404036 django_cache_helper-1.0.5/PKG-INFO
+-rw-r--r--   0 anthonypanat   (502) staff       (20)     2884 2024-05-01 13:39:56.000000 django_cache_helper-1.0.5/README.md
+drwxr-xr-x   0 anthonypanat   (502) staff       (20)        0 2024-05-01 13:41:10.398648 django_cache_helper-1.0.5/cache_helper/
+-rw-r--r--   0 anthonypanat   (502) staff       (20)       20 2024-05-01 13:39:56.000000 django_cache_helper-1.0.5/cache_helper/__init__.py
+-rw-r--r--   0 anthonypanat   (502) staff       (20)     8207 2024-05-01 13:39:56.000000 django_cache_helper-1.0.5/cache_helper/decorators.py
+-rw-r--r--   0 anthonypanat   (502) staff       (20)      110 2024-05-01 13:39:56.000000 django_cache_helper-1.0.5/cache_helper/exceptions.py
+-rw-r--r--   0 anthonypanat   (502) staff       (20)      470 2024-05-01 13:39:56.000000 django_cache_helper-1.0.5/cache_helper/interfaces.py
+-rw-r--r--   0 anthonypanat   (502) staff       (20)       94 2024-05-01 13:39:56.000000 django_cache_helper-1.0.5/cache_helper/settings.py
+-rw-r--r--   0 anthonypanat   (502) staff       (20)     4323 2024-05-01 13:39:56.000000 django_cache_helper-1.0.5/cache_helper/utils.py
+drwxr-xr-x   0 anthonypanat   (502) staff       (20)        0 2024-05-01 13:41:10.403448 django_cache_helper-1.0.5/django_cache_helper.egg-info/
+-rw-r--r--   0 anthonypanat   (502) staff       (20)     3466 2024-05-01 13:41:10.000000 django_cache_helper-1.0.5/django_cache_helper.egg-info/PKG-INFO
+-rw-r--r--   0 anthonypanat   (502) staff       (20)      349 2024-05-01 13:41:10.000000 django_cache_helper-1.0.5/django_cache_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 anthonypanat   (502) staff       (20)        1 2024-05-01 13:41:10.000000 django_cache_helper-1.0.5/django_cache_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 anthonypanat   (502) staff       (20)       13 2024-05-01 13:41:10.000000 django_cache_helper-1.0.5/django_cache_helper.egg-info/top_level.txt
+-rw-r--r--   0 anthonypanat   (502) staff       (20)      841 2024-05-01 13:39:56.000000 django_cache_helper-1.0.5/pyproject.toml
+-rw-r--r--   0 anthonypanat   (502) staff       (20)       38 2024-05-01 13:41:10.404787 django_cache_helper-1.0.5/setup.cfg
```

### Comparing `django-cache-helper-1.0.4/PKG-INFO` & `django_cache_helper-1.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: django-cache-helper
-Version: 1.0.4
+Version: 1.0.5
 Summary: a simple tool for making caching functions, methods, and class methods a little bit easier.
 Author-email: YCharts <developers@ycharts.com>
 Project-URL: Homepage, https://github.com/ycharts/django_cache_helper
 Keywords: cache,django
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Django
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 django-cache-helper
 ===================
 
 &nbsp;
 [![PyPI](https://img.shields.io/pypi/v/django-cache-helper?color=green)](https://pypi.org/project/django-cache-helper/)
```

### Comparing `django-cache-helper-1.0.4/README.md` & `django_cache_helper-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `django-cache-helper-1.0.4/cache_helper/decorators.py` & `django_cache_helper-1.0.5/cache_helper/decorators.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,41 +9,44 @@
 
 from django.core.cache import cache
 from django.utils.functional import wraps
 
 from cache_helper import utils
 
 logger = logging.getLogger(__name__)
+CACHE_KEY_NOT_FOUND = 'cache_key_not_found'
+
 
 def cached(timeout):
     def _cached(func):
         func_name = utils.get_function_name(func)
 
         @wraps(func)
         def wrapper(*args, **kwargs):
             function_cache_key = utils.get_function_cache_key(func_name, args, kwargs)
             cache_key = utils.get_hashed_cache_key(function_cache_key)
 
             try:
-                value = cache.get(cache_key)
+                # Attempts to get cache key and defaults to a string constant which will be returned if the cache
+                # key does not exist due to expiry or never being set.
+                value = cache.get(cache_key, CACHE_KEY_NOT_FOUND)
             except Exception:
                 logger.warning(
                     f'Error retrieving value from Cache for Key: {function_cache_key}',
                     exc_info=True,
                 )
-                value = None
+                value = CACHE_KEY_NOT_FOUND
 
-            if value is None:
+            if value == CACHE_KEY_NOT_FOUND:
                 value = func(*args, **kwargs)
                 # Try and set the key, value pair in the cache.
                 # But if it fails on an error from the underlying
                 # cache system, handle it.
                 try:
                     cache.set(cache_key, value, timeout)
-
                 except CacheSetError:
                     logger.warning(
                         f'Error saving value to Cache for Key: {function_cache_key}',
                         exc_info=True,
                     )
 
             return value
@@ -69,29 +72,29 @@
 def cached_class_method(timeout):
     def _cached(func):
         func_name = utils.get_function_name(func)
 
         @wraps(func)
         def wrapper(*args, **kwargs):
             # skip the first arg because it will be the class itself
-            function_cache_key = utils.get_function_cache_key(
-                func_name, args[1:], kwargs
-            )
+            function_cache_key = utils.get_function_cache_key(func_name, args[1:], kwargs)
             cache_key = utils.get_hashed_cache_key(function_cache_key)
 
             try:
-                value = cache.get(cache_key)
+                # Attempts to get cache key and defaults to a string constant which will be returned if the cache
+                # key does not exist due to expiry or never being set.
+                value = cache.get(cache_key, CACHE_KEY_NOT_FOUND)
             except Exception:
                 logger.warning(
                     f'Error retrieving value from Cache for Key: {function_cache_key}',
                     exc_info=True,
                 )
-                value = None
+                value = CACHE_KEY_NOT_FOUND
 
-            if value is None:
+            if value == CACHE_KEY_NOT_FOUND:
                 value = func(*args, **kwargs)
                 # Try and set the key, value pair in the cache.
                 # But if it fails on an error from the underlying
                 # cache system, handle it.
                 try:
                     cache.set(cache_key, value, timeout)
                 except CacheSetError:
@@ -146,34 +149,39 @@
             # It behaves exactly like `_invalidate` with `obj` automatically included as the first argument.
             fn.invalidate = functools.partial(self._invalidate, obj)
 
             return fn
 
         def __call__(self, *args, **kwargs):
             cache_key, function_cache_key = self.create_cache_key(*args, **kwargs)
+
             try:
-                value = cache.get(cache_key)
+                # Attempts to get cache key and defaults to a string constant which will be returned if the cache
+                # key does not exist due to expiry or never being set.
+                value = cache.get(cache_key, CACHE_KEY_NOT_FOUND)
             except Exception:
                 logger.warning(
                     f'Error retrieving value from Cache for Key: {function_cache_key}',
                     exc_info=True,
                 )
-                value = None
-            if value is None:
+                value = CACHE_KEY_NOT_FOUND
+
+            if value == CACHE_KEY_NOT_FOUND:
                 value = self.func(*args, **kwargs)
                 # Try and set the key, value pair in the cache.
                 # But if it fails on an error from the underlying
                 # cache system, handle it.
                 try:
                     cache.set(cache_key, value, timeout)
                 except CacheSetError:
                     logger.warning(
                         f'Error saving value to Cache for Key: {function_cache_key}',
                         exc_info=True,
                     )
+
             return value
 
         def _invalidate(self, *args, **kwargs):
             """
             A method to invalidate a result from the cache.
             :param args: The args passed into the original function. This includes `self` for instance methods, and
             `cls` for class methods.
```

### Comparing `django-cache-helper-1.0.4/cache_helper/utils.py` & `django_cache_helper-1.0.5/cache_helper/utils.py`

 * *Files identical despite different names*

### Comparing `django-cache-helper-1.0.4/django_cache_helper.egg-info/PKG-INFO` & `django_cache_helper-1.0.5/django_cache_helper.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: django-cache-helper
-Version: 1.0.4
+Version: 1.0.5
 Summary: a simple tool for making caching functions, methods, and class methods a little bit easier.
 Author-email: YCharts <developers@ycharts.com>
 Project-URL: Homepage, https://github.com/ycharts/django_cache_helper
 Keywords: cache,django
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Django
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 django-cache-helper
 ===================
 
 &nbsp;
 [![PyPI](https://img.shields.io/pypi/v/django-cache-helper?color=green)](https://pypi.org/project/django-cache-helper/)
```

### Comparing `django-cache-helper-1.0.4/pyproject.toml` & `django_cache_helper-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [project]
 name = "django-cache-helper"
 authors = [
     { name="YCharts", email="developers@ycharts.com" },
 ]
 description = "a simple tool for making caching functions, methods, and class methods a little bit easier."
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 keywords = [
     "cache",
     "django"
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "Environment :: Web Environment",
```

