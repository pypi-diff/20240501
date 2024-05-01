# Comparing `tmp/drf-secure-token-1.1.0.tar.gz` & `tmp/drf-secure-token-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/drf-secure-token-1.1.0.tar", last modified: Tue Jan 12 08:05:13 2021, max compression
+gzip compressed data, was "drf-secure-token-1.2.0.tar", last modified: Wed May  1 05:20:57 2024, max compression
```

## Comparing `drf-secure-token-1.1.0.tar` & `drf-secure-token-1.2.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 th13f     (1000) th13f     (1000)        0 2021-01-12 08:05:13.000000 drf-secure-token-1.1.0/
-drwxrwxr-x   0 th13f     (1000) th13f     (1000)        0 2021-01-12 08:05:13.000000 drf-secure-token-1.1.0/drf_secure_token/
--rw-r--r--   0 th13f     (1000) th13f     (1000)      202 2017-10-11 14:32:45.000000 drf-secure-token-1.1.0/drf_secure_token/apps.py
--rw-rw-r--   0 th13f     (1000) th13f     (1000)      973 2019-09-20 13:38:04.000000 drf-secure-token-1.1.0/drf_secure_token/middleware.py
--rw-rw-r--   0 th13f     (1000) th13f     (1000)     1589 2021-01-11 13:34:50.000000 drf-secure-token-1.1.0/drf_secure_token/abstract_models.py
--rw-r--r--   0 th13f     (1000) th13f     (1000)       66 2017-10-11 14:32:45.000000 drf-secure-token-1.1.0/drf_secure_token/__init__.py
--rw-r--r--   0 th13f     (1000) th13f     (1000)      264 2017-10-11 14:32:45.000000 drf-secure-token-1.1.0/drf_secure_token/models.py
-drwxrwxr-x   0 th13f     (1000) th13f     (1000)        0 2021-01-12 08:05:13.000000 drf-secure-token-1.1.0/drf_secure_token/migrations/
--rw-rw-r--   0 th13f     (1000) th13f     (1000)      666 2020-07-23 13:40:56.000000 drf-secure-token-1.1.0/drf_secure_token/migrations/0004_auto_20160422_0837.py
--rw-rw-r--   0 th13f     (1000) th13f     (1000)      480 2020-07-23 13:40:56.000000 drf-secure-token-1.1.0/drf_secure_token/migrations/0002_token_expire_in.py
--rw-rw-r--   0 th13f     (1000) th13f     (1000)      454 2020-07-23 13:40:56.000000 drf-secure-token-1.1.0/drf_secure_token/migrations/0003_auto_20151223_0921.py
--rw-rw-r--   0 th13f     (1000) th13f     (1000)      655 2020-07-23 13:40:56.000000 drf-secure-token-1.1.0/drf_secure_token/migrations/0006_auto_20170227_1945.py
--rw-rw-r--   0 th13f     (1000) th13f     (1000)      966 2020-07-23 13:40:56.000000 drf-secure-token-1.1.0/drf_secure_token/migrations/0001_initial.py
--rw-r--r--   0 th13f     (1000) th13f     (1000)        0 2017-10-11 14:32:45.000000 drf-secure-token-1.1.0/drf_secure_token/migrations/__init__.py
--rw-rw-r--   0 th13f     (1000) th13f     (1000)      524 2020-07-23 13:40:56.000000 drf-secure-token-1.1.0/drf_secure_token/migrations/0005_auto_20170227_1038.py
--rw-rw-r--   0 th13f     (1000) th13f     (1000)      963 2020-07-23 13:40:56.000000 drf-secure-token-1.1.0/drf_secure_token/migrations/0007_auto_20190920_1044.py
--rw-rw-r--   0 th13f     (1000) th13f     (1000)      844 2021-01-11 13:34:50.000000 drf-secure-token-1.1.0/drf_secure_token/settings.py
--rw-rw-r--   0 th13f     (1000) th13f     (1000)      582 2020-07-23 13:40:56.000000 drf-secure-token-1.1.0/drf_secure_token/authentication.py
--rw-rw-r--   0 th13f     (1000) th13f     (1000)     1045 2021-01-11 13:34:50.000000 drf-secure-token-1.1.0/drf_secure_token/tasks.py
--rw-rw-r--   0 th13f     (1000) th13f     (1000)      264 2020-07-23 13:40:56.000000 drf-secure-token-1.1.0/drf_secure_token/admin.py
--rw-rw-r--   0 th13f     (1000) th13f     (1000)     1142 2019-09-20 13:38:04.000000 drf-secure-token-1.1.0/drf_secure_token/checkers.py
-drwxrwxr-x   0 th13f     (1000) th13f     (1000)        0 2021-01-12 08:05:13.000000 drf-secure-token-1.1.0/drf_secure_token.egg-info/
--rw-r--r--   0 th13f     (1000) th13f     (1000)     2556 2021-01-12 08:05:13.000000 drf-secure-token-1.1.0/drf_secure_token.egg-info/PKG-INFO
--rw-r--r--   0 th13f     (1000) th13f     (1000)       20 2021-01-12 08:05:13.000000 drf-secure-token-1.1.0/drf_secure_token.egg-info/requires.txt
--rw-r--r--   0 th13f     (1000) th13f     (1000)      922 2021-01-12 08:05:13.000000 drf-secure-token-1.1.0/drf_secure_token.egg-info/SOURCES.txt
--rw-r--r--   0 th13f     (1000) th13f     (1000)       45 2021-01-12 08:05:13.000000 drf-secure-token-1.1.0/drf_secure_token.egg-info/top_level.txt
--rw-r--r--   0 th13f     (1000) th13f     (1000)        1 2021-01-12 08:05:13.000000 drf-secure-token-1.1.0/drf_secure_token.egg-info/dependency_links.txt
--rw-rw-r--   0 th13f     (1000) th13f     (1000)     2556 2021-01-12 08:05:13.000000 drf-secure-token-1.1.0/PKG-INFO
--rw-rw-r--   0 th13f     (1000) th13f     (1000)     1456 2021-01-11 13:34:50.000000 drf-secure-token-1.1.0/README.rst
--rw-rw-r--   0 th13f     (1000) th13f     (1000)     1113 2021-01-11 13:34:50.000000 drf-secure-token-1.1.0/setup.py
--rw-rw-r--   0 th13f     (1000) th13f     (1000)       38 2021-01-12 08:05:13.000000 drf-secure-token-1.1.0/setup.cfg
+drwxr-xr-x   0 th13f      (501) staff       (20)        0 2024-05-01 05:20:57.588209 drf-secure-token-1.2.0/
+-rw-r--r--   0 th13f      (501) staff       (20)     2070 2024-05-01 05:20:57.588078 drf-secure-token-1.2.0/PKG-INFO
+-rw-r--r--   0 th13f      (501) staff       (20)     1456 2024-05-01 05:18:20.000000 drf-secure-token-1.2.0/README.rst
+drwxr-xr-x   0 th13f      (501) staff       (20)        0 2024-05-01 05:20:57.586712 drf-secure-token-1.2.0/drf_secure_token/
+-rw-r--r--   0 th13f      (501) staff       (20)      113 2024-05-01 05:18:20.000000 drf-secure-token-1.2.0/drf_secure_token/__init__.py
+-rw-r--r--   0 th13f      (501) staff       (20)     1589 2024-05-01 05:18:20.000000 drf-secure-token-1.2.0/drf_secure_token/abstract_models.py
+-rw-r--r--   0 th13f      (501) staff       (20)      264 2024-05-01 05:18:20.000000 drf-secure-token-1.2.0/drf_secure_token/admin.py
+-rw-r--r--   0 th13f      (501) staff       (20)      201 2024-05-01 05:18:20.000000 drf-secure-token-1.2.0/drf_secure_token/apps.py
+-rw-r--r--   0 th13f      (501) staff       (20)      581 2024-05-01 05:18:20.000000 drf-secure-token-1.2.0/drf_secure_token/authentication.py
+-rw-r--r--   0 th13f      (501) staff       (20)     1141 2024-05-01 05:18:20.000000 drf-secure-token-1.2.0/drf_secure_token/checkers.py
+-rw-r--r--   0 th13f      (501) staff       (20)      794 2024-05-01 05:18:20.000000 drf-secure-token-1.2.0/drf_secure_token/middleware.py
+drwxr-xr-x   0 th13f      (501) staff       (20)        0 2024-05-01 05:20:57.587952 drf-secure-token-1.2.0/drf_secure_token/migrations/
+-rw-r--r--   0 th13f      (501) staff       (20)      966 2024-05-01 05:18:20.000000 drf-secure-token-1.2.0/drf_secure_token/migrations/0001_initial.py
+-rw-r--r--   0 th13f      (501) staff       (20)      480 2024-05-01 05:18:20.000000 drf-secure-token-1.2.0/drf_secure_token/migrations/0002_token_expire_in.py
+-rw-r--r--   0 th13f      (501) staff       (20)      454 2024-05-01 05:18:20.000000 drf-secure-token-1.2.0/drf_secure_token/migrations/0003_auto_20151223_0921.py
+-rw-r--r--   0 th13f      (501) staff       (20)      666 2024-05-01 05:18:20.000000 drf-secure-token-1.2.0/drf_secure_token/migrations/0004_auto_20160422_0837.py
+-rw-r--r--   0 th13f      (501) staff       (20)      524 2024-05-01 05:18:20.000000 drf-secure-token-1.2.0/drf_secure_token/migrations/0005_auto_20170227_1038.py
+-rw-r--r--   0 th13f      (501) staff       (20)      655 2024-05-01 05:18:20.000000 drf-secure-token-1.2.0/drf_secure_token/migrations/0006_auto_20170227_1945.py
+-rw-r--r--   0 th13f      (501) staff       (20)      963 2024-05-01 05:18:20.000000 drf-secure-token-1.2.0/drf_secure_token/migrations/0007_auto_20190920_1044.py
+-rw-r--r--   0 th13f      (501) staff       (20)        0 2024-05-01 05:18:20.000000 drf-secure-token-1.2.0/drf_secure_token/migrations/__init__.py
+-rw-r--r--   0 th13f      (501) staff       (20)      263 2024-05-01 05:18:20.000000 drf-secure-token-1.2.0/drf_secure_token/models.py
+-rw-r--r--   0 th13f      (501) staff       (20)      844 2024-05-01 05:18:20.000000 drf-secure-token-1.2.0/drf_secure_token/settings.py
+-rw-r--r--   0 th13f      (501) staff       (20)     1045 2024-05-01 05:18:20.000000 drf-secure-token-1.2.0/drf_secure_token/tasks.py
+drwxr-xr-x   0 th13f      (501) staff       (20)        0 2024-05-01 05:20:57.587181 drf-secure-token-1.2.0/drf_secure_token.egg-info/
+-rw-r--r--   0 th13f      (501) staff       (20)     2070 2024-05-01 05:20:57.000000 drf-secure-token-1.2.0/drf_secure_token.egg-info/PKG-INFO
+-rw-r--r--   0 th13f      (501) staff       (20)      922 2024-05-01 05:20:57.000000 drf-secure-token-1.2.0/drf_secure_token.egg-info/SOURCES.txt
+-rw-r--r--   0 th13f      (501) staff       (20)        1 2024-05-01 05:20:57.000000 drf-secure-token-1.2.0/drf_secure_token.egg-info/dependency_links.txt
+-rw-r--r--   0 th13f      (501) staff       (20)       20 2024-05-01 05:20:57.000000 drf-secure-token-1.2.0/drf_secure_token.egg-info/requires.txt
+-rw-r--r--   0 th13f      (501) staff       (20)       45 2024-05-01 05:20:57.000000 drf-secure-token-1.2.0/drf_secure_token.egg-info/top_level.txt
+-rw-r--r--   0 th13f      (501) staff       (20)       38 2024-05-01 05:20:57.588251 drf-secure-token-1.2.0/setup.cfg
+-rw-r--r--   0 th13f      (501) staff       (20)     1113 2024-05-01 05:18:20.000000 drf-secure-token-1.2.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `drf-secure-token-1.1.0/drf_secure_token/middleware.py` & `drf-secure-token-1.2.0/drf_secure_token/middleware.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,15 @@
 from django.utils import timezone
+from django.utils.deprecation import MiddlewareMixin
 
 from drf_secure_token.models import Token
 from drf_secure_token.settings import settings as token_settings
 
-try:
-    # Using MiddlewareMixin to add compatibility level between the new and old middleware styles.
-    from django.utils.deprecation import MiddlewareMixin as MiddlewareParent
-except ImportError:
-    MiddlewareParent = object
 
-
-class UpdateTokenMiddleware(MiddlewareParent):
+class UpdateTokenMiddleware(MiddlewareMixin):
     def process_response(self, request, response):
         token = getattr(request, 'auth', None)
         if not isinstance(token, Token):
             return response
 
         if token_settings.UPDATE_TOKEN:
             now = timezone.now()
```

### Comparing `drf-secure-token-1.1.0/drf_secure_token/abstract_models.py` & `drf-secure-token-1.2.0/drf_secure_token/abstract_models.py`

 * *Files identical despite different names*

### Comparing `drf-secure-token-1.1.0/drf_secure_token/migrations/0004_auto_20160422_0837.py` & `drf-secure-token-1.2.0/drf_secure_token/migrations/0004_auto_20160422_0837.py`

 * *Files identical despite different names*

### Comparing `drf-secure-token-1.1.0/drf_secure_token/migrations/0006_auto_20170227_1945.py` & `drf-secure-token-1.2.0/drf_secure_token/migrations/0006_auto_20170227_1945.py`

 * *Files identical despite different names*

### Comparing `drf-secure-token-1.1.0/drf_secure_token/migrations/0001_initial.py` & `drf-secure-token-1.2.0/drf_secure_token/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `drf-secure-token-1.1.0/drf_secure_token/migrations/0005_auto_20170227_1038.py` & `drf-secure-token-1.2.0/drf_secure_token/migrations/0005_auto_20170227_1038.py`

 * *Files identical despite different names*

### Comparing `drf-secure-token-1.1.0/drf_secure_token/migrations/0007_auto_20190920_1044.py` & `drf-secure-token-1.2.0/drf_secure_token/migrations/0007_auto_20190920_1044.py`

 * *Files identical despite different names*

### Comparing `drf-secure-token-1.1.0/drf_secure_token/settings.py` & `drf-secure-token-1.2.0/drf_secure_token/settings.py`

 * *Files identical despite different names*

### Comparing `drf-secure-token-1.1.0/drf_secure_token/authentication.py` & `drf-secure-token-1.2.0/drf_secure_token/authentication.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 from rest_framework import exceptions
 from rest_framework.authentication import TokenAuthentication
 
 from drf_secure_token.models import Token
```

### Comparing `drf-secure-token-1.1.0/drf_secure_token/tasks.py` & `drf-secure-token-1.2.0/drf_secure_token/tasks.py`

 * *Files identical despite different names*

### Comparing `drf-secure-token-1.1.0/drf_secure_token/checkers.py` & `drf-secure-token-1.2.0/drf_secure_token/checkers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from django.utils import timezone
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 from rest_framework.settings import perform_import
 
 from drf_secure_token.settings import settings as token_settings
 
 
 class BaseChecker(object):
```

### Comparing `drf-secure-token-1.1.0/drf_secure_token.egg-info/PKG-INFO` & `drf-secure-token-1.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,75 +1,74 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: drf-secure-token
-Version: 1.1.0
-Summary: Add secure token to djnago-rest-framework
-Home-page: UNKNOWN
+Version: 1.2.0
+Summary: Add secure token to django-rest-framework
+Home-page: 
 Author: Tima Akulich
 Author-email: tima.akulich@gmail.com
 License: BSD License
-Description: ================
-        DRF Secure Token
-        ================
-        
-        Quick start
-        -----------
-        
-        1. Add "drf_secure_token" to your INSTALLED_APPS setting like this::
-        
-            INSTALLED_APPS = [
-                ...
-                'rest_framework',
-                'drf_secure_token',
-            ]
-        
-        2. Add following lines to your settings.py::
-        
-            REST_FRAMEWORK = {
-                'DEFAULT_AUTHENTICATION_CLASSES': [
-                    'rest_framework.authentication.BasicAuthentication',
-                    'drf_secure_token.authentication.SecureTokenAuthentication',
-                 ]
-            }
-        
-        3. For updating token add this middleware to your MIDDLEWARE_CLASSES::
-        
-            MIDDLEWARE_CLASSES = (
-                ...
-                'drf_secure_token.middleware.UpdateTokenMiddleware',
-            )
-        
-        4. Add UPDATE_TOKEN to your 'dev' settings if you don't want to update token in DEBUG mode::
-        
-            UPDATE_TOKEN = False
-        
-        5. Add TOKEN_AGE to your settings::
-        
-            TOKEN_AGE = 60*10 # 10 min
-        
-        6. (Optional) To cleanup dead tokens celery can be used. Way to enable depends from celery version
-        
-        6.1 Celery 4, just enable it with settings::
-        
-            REMOVE_TOKENS_THROUGH_CELERY = True
-        
-        6.2 Celery 5, add periodic task manually::
-        
-            @app.on_after_finalize.connect
-            def setup_periodic_tasks(sender, **kwargs):
-                from drf_secure_token.tasks import DELETE_OLD_TOKENS
-        
-                app.conf.beat_schedule.update({
-                    'drf_secure_token.tasks.delete_old_tokens': DELETE_OLD_TOKENS,
-                })
-        
-        7. Run `python manage.py migrate` to create the drf_secure_token models.
-        
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+
+================
+DRF Secure Token
+================
+
+Quick start
+-----------
+
+1. Add "drf_secure_token" to your INSTALLED_APPS setting like this::
+
+    INSTALLED_APPS = [
+        ...
+        'rest_framework',
+        'drf_secure_token',
+    ]
+
+2. Add following lines to your settings.py::
+
+    REST_FRAMEWORK = {
+        'DEFAULT_AUTHENTICATION_CLASSES': [
+            'rest_framework.authentication.BasicAuthentication',
+            'drf_secure_token.authentication.SecureTokenAuthentication',
+         ]
+    }
+
+3. For updating token add this middleware to your MIDDLEWARE_CLASSES::
+
+    MIDDLEWARE_CLASSES = (
+        ...
+        'drf_secure_token.middleware.UpdateTokenMiddleware',
+    )
+
+4. Add UPDATE_TOKEN to your 'dev' settings if you don't want to update token in DEBUG mode::
+
+    UPDATE_TOKEN = False
+
+5. Add TOKEN_AGE to your settings::
+
+    TOKEN_AGE = 60*10 # 10 min
+
+6. (Optional) To cleanup dead tokens celery can be used. Way to enable depends from celery version
+
+6.1 Celery 4, just enable it with settings::
+
+    REMOVE_TOKENS_THROUGH_CELERY = True
+
+6.2 Celery 5, add periodic task manually::
+
+    @app.on_after_finalize.connect
+    def setup_periodic_tasks(sender, **kwargs):
+        from drf_secure_token.tasks import DELETE_OLD_TOKENS
+
+        app.conf.beat_schedule.update({
+            'drf_secure_token.tasks.delete_old_tokens': DELETE_OLD_TOKENS,
+        })
+
+7. Run `python manage.py migrate` to create the drf_secure_token models.
```

### Comparing `drf-secure-token-1.1.0/drf_secure_token.egg-info/SOURCES.txt` & `drf-secure-token-1.2.0/drf_secure_token.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drf-secure-token-1.1.0/PKG-INFO` & `drf-secure-token-1.2.0/drf_secure_token.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,75 +1,74 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: drf-secure-token
-Version: 1.1.0
-Summary: Add secure token to djnago-rest-framework
-Home-page: UNKNOWN
+Version: 1.2.0
+Summary: Add secure token to django-rest-framework
+Home-page: 
 Author: Tima Akulich
 Author-email: tima.akulich@gmail.com
 License: BSD License
-Description: ================
-        DRF Secure Token
-        ================
-        
-        Quick start
-        -----------
-        
-        1. Add "drf_secure_token" to your INSTALLED_APPS setting like this::
-        
-            INSTALLED_APPS = [
-                ...
-                'rest_framework',
-                'drf_secure_token',
-            ]
-        
-        2. Add following lines to your settings.py::
-        
-            REST_FRAMEWORK = {
-                'DEFAULT_AUTHENTICATION_CLASSES': [
-                    'rest_framework.authentication.BasicAuthentication',
-                    'drf_secure_token.authentication.SecureTokenAuthentication',
-                 ]
-            }
-        
-        3. For updating token add this middleware to your MIDDLEWARE_CLASSES::
-        
-            MIDDLEWARE_CLASSES = (
-                ...
-                'drf_secure_token.middleware.UpdateTokenMiddleware',
-            )
-        
-        4. Add UPDATE_TOKEN to your 'dev' settings if you don't want to update token in DEBUG mode::
-        
-            UPDATE_TOKEN = False
-        
-        5. Add TOKEN_AGE to your settings::
-        
-            TOKEN_AGE = 60*10 # 10 min
-        
-        6. (Optional) To cleanup dead tokens celery can be used. Way to enable depends from celery version
-        
-        6.1 Celery 4, just enable it with settings::
-        
-            REMOVE_TOKENS_THROUGH_CELERY = True
-        
-        6.2 Celery 5, add periodic task manually::
-        
-            @app.on_after_finalize.connect
-            def setup_periodic_tasks(sender, **kwargs):
-                from drf_secure_token.tasks import DELETE_OLD_TOKENS
-        
-                app.conf.beat_schedule.update({
-                    'drf_secure_token.tasks.delete_old_tokens': DELETE_OLD_TOKENS,
-                })
-        
-        7. Run `python manage.py migrate` to create the drf_secure_token models.
-        
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+
+================
+DRF Secure Token
+================
+
+Quick start
+-----------
+
+1. Add "drf_secure_token" to your INSTALLED_APPS setting like this::
+
+    INSTALLED_APPS = [
+        ...
+        'rest_framework',
+        'drf_secure_token',
+    ]
+
+2. Add following lines to your settings.py::
+
+    REST_FRAMEWORK = {
+        'DEFAULT_AUTHENTICATION_CLASSES': [
+            'rest_framework.authentication.BasicAuthentication',
+            'drf_secure_token.authentication.SecureTokenAuthentication',
+         ]
+    }
+
+3. For updating token add this middleware to your MIDDLEWARE_CLASSES::
+
+    MIDDLEWARE_CLASSES = (
+        ...
+        'drf_secure_token.middleware.UpdateTokenMiddleware',
+    )
+
+4. Add UPDATE_TOKEN to your 'dev' settings if you don't want to update token in DEBUG mode::
+
+    UPDATE_TOKEN = False
+
+5. Add TOKEN_AGE to your settings::
+
+    TOKEN_AGE = 60*10 # 10 min
+
+6. (Optional) To cleanup dead tokens celery can be used. Way to enable depends from celery version
+
+6.1 Celery 4, just enable it with settings::
+
+    REMOVE_TOKENS_THROUGH_CELERY = True
+
+6.2 Celery 5, add periodic task manually::
+
+    @app.on_after_finalize.connect
+    def setup_periodic_tasks(sender, **kwargs):
+        from drf_secure_token.tasks import DELETE_OLD_TOKENS
+
+        app.conf.beat_schedule.update({
+            'drf_secure_token.tasks.delete_old_tokens': DELETE_OLD_TOKENS,
+        })
+
+7. Run `python manage.py migrate` to create the drf_secure_token models.
```

### Comparing `drf-secure-token-1.1.0/README.rst` & `drf-secure-token-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `drf-secure-token-1.1.0/setup.py` & `drf-secure-token-1.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,19 +6,19 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='drf-secure-token',
-    version='1.1.0',
+    version='1.2.0',
     packages=['drf_secure_token', 'drf_secure_token/migrations'],
     include_package_data=True,
     license='BSD License',
-    description='Add secure token to djnago-rest-framework',
+    description='Add secure token to django-rest-framework',
     long_description=README,
     url='',
     author='Tima Akulich',
     author_email='tima.akulich@gmail.com',
     install_requires=['djangorestframework'],
     classifiers=[
         'Environment :: Web Environment',
```

