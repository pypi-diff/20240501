# Comparing `tmp/django_dynaform-0.1.0.tar.gz` & `tmp/django_dynaform-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_dynaform-0.1.0.tar", last modified: Thu Apr 18 09:37:50 2024, max compression
+gzip compressed data, was "django_dynaform-0.1.1.tar", last modified: Wed May  1 09:57:37 2024, max compression
```

## Comparing `django_dynaform-0.1.0.tar` & `django_dynaform-0.1.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:37:50.916034 django_dynaform-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-04-18 09:37:50.916034 django_dynaform-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-18 09:37:38.000000 django_dynaform-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:37:50.916034 django_dynaform-0.1.0/django_dynaform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-04-18 09:37:50.000000 django_dynaform-0.1.0/django_dynaform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-18 09:37:50.000000 django_dynaform-0.1.0/django_dynaform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 09:37:50.000000 django_dynaform-0.1.0/django_dynaform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 09:37:50.000000 django_dynaform-0.1.0/django_dynaform.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-18 09:37:50.000000 django_dynaform-0.1.0/django_dynaform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-18 09:37:50.000000 django_dynaform-0.1.0/django_dynaform.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:37:50.912034 django_dynaform-0.1.0/dynaform/
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-18 09:37:38.000000 django_dynaform-0.1.0/dynaform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-18 09:37:38.000000 django_dynaform-0.1.0/dynaform/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-18 09:37:38.000000 django_dynaform-0.1.0/dynaform/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-18 09:37:38.000000 django_dynaform-0.1.0/dynaform/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-04-18 09:37:38.000000 django_dynaform-0.1.0/dynaform/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:37:50.912034 django_dynaform-0.1.0/dynaform/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-18 09:37:38.000000 django_dynaform-0.1.0/dynaform/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:37:38.000000 django_dynaform-0.1.0/dynaform/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-18 09:37:38.000000 django_dynaform-0.1.0/dynaform/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-04-18 09:37:38.000000 django_dynaform-0.1.0/dynaform/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:37:50.908034 django_dynaform-0.1.0/dynaform/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:37:50.916034 django_dynaform-0.1.0/dynaform/templates/dynaform/
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-18 09:37:38.000000 django_dynaform-0.1.0/dynaform/templates/dynaform/base.html
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-18 09:37:38.000000 django_dynaform-0.1.0/dynaform/templates/dynaform/dynaform-data-edit.html
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-18 09:37:38.000000 django_dynaform-0.1.0/dynaform/templates/dynaform/dynaform-data-list.html
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-18 09:37:38.000000 django_dynaform-0.1.0/dynaform/templates/dynaform/link-to-dynaform-data-delete.html
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-18 09:37:38.000000 django_dynaform-0.1.0/dynaform/templates/dynaform/link-to-dynaform-data-edit.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:37:50.916034 django_dynaform-0.1.0/dynaform/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:37:38.000000 django_dynaform-0.1.0/dynaform/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-18 09:37:38.000000 django_dynaform-0.1.0/dynaform/templatetags/dynaform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-18 09:37:38.000000 django_dynaform-0.1.0/dynaform/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-18 09:37:38.000000 django_dynaform-0.1.0/dynaform/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:37:50.916034 django_dynaform-0.1.0/settings/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:37:38.000000 django_dynaform-0.1.0/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-18 09:37:38.000000 django_dynaform-0.1.0/settings/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-18 09:37:38.000000 django_dynaform-0.1.0/settings/dummy.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-18 09:37:38.000000 django_dynaform-0.1.0/settings/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-18 09:37:50.916034 django_dynaform-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-04-18 09:37:38.000000 django_dynaform-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:37:50.916034 django_dynaform-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-04-18 09:37:38.000000 django_dynaform-0.1.0/tests/test_forms.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:37:38.000000 django_dynaform-0.1.0/tests/test_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:57:37.604625 django_dynaform-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-05-01 09:57:37.604625 django_dynaform-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-01 09:57:29.000000 django_dynaform-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:57:37.600625 django_dynaform-0.1.1/django_dynaform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-05-01 09:57:37.000000 django_dynaform-0.1.1/django_dynaform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-01 09:57:37.000000 django_dynaform-0.1.1/django_dynaform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 09:57:37.000000 django_dynaform-0.1.1/django_dynaform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 09:57:37.000000 django_dynaform-0.1.1/django_dynaform.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-01 09:57:37.000000 django_dynaform-0.1.1/django_dynaform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-01 09:57:37.000000 django_dynaform-0.1.1/django_dynaform.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:57:37.600625 django_dynaform-0.1.1/dynaform/
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-01 09:57:29.000000 django_dynaform-0.1.1/dynaform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-01 09:57:29.000000 django_dynaform-0.1.1/dynaform/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-01 09:57:29.000000 django_dynaform-0.1.1/dynaform/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-01 09:57:29.000000 django_dynaform-0.1.1/dynaform/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-01 09:57:29.000000 django_dynaform-0.1.1/dynaform/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:57:37.600625 django_dynaform-0.1.1/dynaform/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-05-01 09:57:29.000000 django_dynaform-0.1.1/dynaform/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 09:57:29.000000 django_dynaform-0.1.1/dynaform/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-05-01 09:57:29.000000 django_dynaform-0.1.1/dynaform/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-05-01 09:57:29.000000 django_dynaform-0.1.1/dynaform/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:57:37.596625 django_dynaform-0.1.1/dynaform/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:57:37.600625 django_dynaform-0.1.1/dynaform/templates/dynaform/
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-01 09:57:29.000000 django_dynaform-0.1.1/dynaform/templates/dynaform/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-01 09:57:29.000000 django_dynaform-0.1.1/dynaform/templates/dynaform/dynaform-data-edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-01 09:57:29.000000 django_dynaform-0.1.1/dynaform/templates/dynaform/dynaform-data-list.html
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-01 09:57:29.000000 django_dynaform-0.1.1/dynaform/templates/dynaform/link-to-dynaform-data-delete.html
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-01 09:57:29.000000 django_dynaform-0.1.1/dynaform/templates/dynaform/link-to-dynaform-data-edit.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:57:37.600625 django_dynaform-0.1.1/dynaform/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 09:57:29.000000 django_dynaform-0.1.1/dynaform/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-05-01 09:57:29.000000 django_dynaform-0.1.1/dynaform/templatetags/dynaform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-01 09:57:29.000000 django_dynaform-0.1.1/dynaform/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-05-01 09:57:29.000000 django_dynaform-0.1.1/dynaform/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:57:37.600625 django_dynaform-0.1.1/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 09:57:29.000000 django_dynaform-0.1.1/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-01 09:57:29.000000 django_dynaform-0.1.1/settings/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-01 09:57:29.000000 django_dynaform-0.1.1/settings/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-01 09:57:29.000000 django_dynaform-0.1.1/settings/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-01 09:57:37.604625 django_dynaform-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-05-01 09:57:29.000000 django_dynaform-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:57:37.600625 django_dynaform-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-01 09:57:29.000000 django_dynaform-0.1.1/tests/test_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 09:57:29.000000 django_dynaform-0.1.1/tests/test_service.py
```

### Comparing `django_dynaform-0.1.0/PKG-INFO` & `django_dynaform-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-dynaform
-Version: 0.1.0
+Version: 0.1.1
 Summary: Dynamic form for Django
 Home-page: https://github.com/loghmanb/django-dynaform
 Author: Loghman Barari
 Author-email: loghmanb@gmail.com
 License: BSD
 Project-URL: Source, https://github.com/loghmanb/django-dynaform
 Classifier: Development Status :: 5 - Production/Stable
@@ -39,23 +39,23 @@
 
 ![PyPI](https://img.shields.io/pypi/v/django-dynaform?label=django-dynaform)
 
 ## Overview
 
 Dynamic Django forms allow users to define, edit, and populate their own entities and apply runtime schema changes to them. `django-dynaform` is a unique tools to empower your project with more dynamicity with minimum database changes. It is ideal and unique tools for frequently changing and/or temporary data structures. It is the goal of this project to provide a bring dynamicity with maximum benefit to a project with less effort.
 
-This package provides models to help admin users quickly add/change/drop dynamic models for their specific use case, and use them in dynamic templates. The schema changes are applied in the runtime, *without* database metadata changes, so it could use in dynamic templates with zero downtime and any side effects of changing in data structure.
+[This package](https://pypi.org/project/django-dynaform/) provides models to help admin users quickly add/change/drop dynamic models for their specific use case, and use them in dynamic templates. The schema changes are applied in the runtime, *without* database metadata changes, so it could use in dynamic templates with zero downtime and any side effects of changing in data structure.
 
 > **Disclaimer**:
 > 
 > It is not recommended to use this project for business critical data due to the high potential for data loss. Tables can be dropped very easily, and without backups, even a small user error could be catastrophic.
 
 ## Example project
 
-You can download an example project from https://github.com/loghmanb/django-dynaform/example
+You can download an example project from https://github.com/loghmanb/django-dynaform/tree/main/example
 go to the folder and run below commands
 
 ```shell
 $ pip install -r requirements.txt
 $ python manage.py loaddata sample-data.json.gz
 $ python manage.py runserver 0:8000
 ```
```

### Comparing `django_dynaform-0.1.0/README.md` & `django_dynaform-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 
 ![PyPI](https://img.shields.io/pypi/v/django-dynaform?label=django-dynaform)
 
 ## Overview
 
 Dynamic Django forms allow users to define, edit, and populate their own entities and apply runtime schema changes to them. `django-dynaform` is a unique tools to empower your project with more dynamicity with minimum database changes. It is ideal and unique tools for frequently changing and/or temporary data structures. It is the goal of this project to provide a bring dynamicity with maximum benefit to a project with less effort.
 
-This package provides models to help admin users quickly add/change/drop dynamic models for their specific use case, and use them in dynamic templates. The schema changes are applied in the runtime, *without* database metadata changes, so it could use in dynamic templates with zero downtime and any side effects of changing in data structure.
+[This package](https://pypi.org/project/django-dynaform/) provides models to help admin users quickly add/change/drop dynamic models for their specific use case, and use them in dynamic templates. The schema changes are applied in the runtime, *without* database metadata changes, so it could use in dynamic templates with zero downtime and any side effects of changing in data structure.
 
 > **Disclaimer**:
 > 
 > It is not recommended to use this project for business critical data due to the high potential for data loss. Tables can be dropped very easily, and without backups, even a small user error could be catastrophic.
 
 ## Example project
 
-You can download an example project from https://github.com/loghmanb/django-dynaform/example
+You can download an example project from https://github.com/loghmanb/django-dynaform/tree/main/example
 go to the folder and run below commands
 
 ```shell
 $ pip install -r requirements.txt
 $ python manage.py loaddata sample-data.json.gz
 $ python manage.py runserver 0:8000
 ```
```

### Comparing `django_dynaform-0.1.0/django_dynaform.egg-info/PKG-INFO` & `django_dynaform-0.1.1/django_dynaform.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-dynaform
-Version: 0.1.0
+Version: 0.1.1
 Summary: Dynamic form for Django
 Home-page: https://github.com/loghmanb/django-dynaform
 Author: Loghman Barari
 Author-email: loghmanb@gmail.com
 License: BSD
 Project-URL: Source, https://github.com/loghmanb/django-dynaform
 Classifier: Development Status :: 5 - Production/Stable
@@ -39,23 +39,23 @@
 
 ![PyPI](https://img.shields.io/pypi/v/django-dynaform?label=django-dynaform)
 
 ## Overview
 
 Dynamic Django forms allow users to define, edit, and populate their own entities and apply runtime schema changes to them. `django-dynaform` is a unique tools to empower your project with more dynamicity with minimum database changes. It is ideal and unique tools for frequently changing and/or temporary data structures. It is the goal of this project to provide a bring dynamicity with maximum benefit to a project with less effort.
 
-This package provides models to help admin users quickly add/change/drop dynamic models for their specific use case, and use them in dynamic templates. The schema changes are applied in the runtime, *without* database metadata changes, so it could use in dynamic templates with zero downtime and any side effects of changing in data structure.
+[This package](https://pypi.org/project/django-dynaform/) provides models to help admin users quickly add/change/drop dynamic models for their specific use case, and use them in dynamic templates. The schema changes are applied in the runtime, *without* database metadata changes, so it could use in dynamic templates with zero downtime and any side effects of changing in data structure.
 
 > **Disclaimer**:
 > 
 > It is not recommended to use this project for business critical data due to the high potential for data loss. Tables can be dropped very easily, and without backups, even a small user error could be catastrophic.
 
 ## Example project
 
-You can download an example project from https://github.com/loghmanb/django-dynaform/example
+You can download an example project from https://github.com/loghmanb/django-dynaform/tree/main/example
 go to the folder and run below commands
 
 ```shell
 $ pip install -r requirements.txt
 $ python manage.py loaddata sample-data.json.gz
 $ python manage.py runserver 0:8000
 ```
```

### Comparing `django_dynaform-0.1.0/django_dynaform.egg-info/SOURCES.txt` & `django_dynaform-0.1.1/django_dynaform.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_dynaform-0.1.0/dynaform/__init__.py` & `django_dynaform-0.1.1/dynaform/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,18 +8,18 @@
           __/ |
          |___/
 """
 
 import django
 
 __title__ = "DynaForm"
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 __author__ = "Loghman Barari"
 __license__ = "BSD 3-Clause"
-__copyright__ = "Copyright 2022-Present Loghman Barari"
+__copyright__ = "Copyright 2023-Present Loghman Barari"
 
 # Version synonym
 VERSION = __version__
 
 # Header encoding (see RFC5987)
 HTTP_HEADER_ENCODING = "iso-8859-1"
```

### Comparing `django_dynaform-0.1.0/dynaform/admin.py` & `django_dynaform-0.1.1/dynaform/admin.py`

 * *Files identical despite different names*

### Comparing `django_dynaform-0.1.0/dynaform/apps.py` & `django_dynaform-0.1.1/dynaform/apps.py`

 * *Files identical despite different names*

### Comparing `django_dynaform-0.1.0/dynaform/const.py` & `django_dynaform-0.1.1/dynaform/const.py`

 * *Files identical despite different names*

### Comparing `django_dynaform-0.1.0/dynaform/forms.py` & `django_dynaform-0.1.1/dynaform/forms.py`

 * *Files identical despite different names*

### Comparing `django_dynaform-0.1.0/dynaform/migrations/0001_initial.py` & `django_dynaform-0.1.1/dynaform/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_dynaform-0.1.0/dynaform/models.py` & `django_dynaform-0.1.1/dynaform/models.py`

 * *Files identical despite different names*

### Comparing `django_dynaform-0.1.0/dynaform/service.py` & `django_dynaform-0.1.1/dynaform/service.py`

 * *Files identical despite different names*

### Comparing `django_dynaform-0.1.0/dynaform/templates/dynaform/base.html` & `django_dynaform-0.1.1/dynaform/templates/dynaform/base.html`

 * *Files identical despite different names*

### Comparing `django_dynaform-0.1.0/dynaform/templates/dynaform/dynaform-data-edit.html` & `django_dynaform-0.1.1/dynaform/templates/dynaform/dynaform-data-edit.html`

 * *Files identical despite different names*

### Comparing `django_dynaform-0.1.0/dynaform/templates/dynaform/dynaform-data-list.html` & `django_dynaform-0.1.1/dynaform/templates/dynaform/dynaform-data-list.html`

 * *Files identical despite different names*

### Comparing `django_dynaform-0.1.0/dynaform/templatetags/dynaform.py` & `django_dynaform-0.1.1/dynaform/templatetags/dynaform.py`

 * *Files identical despite different names*

### Comparing `django_dynaform-0.1.0/dynaform/urls.py` & `django_dynaform-0.1.1/dynaform/urls.py`

 * *Files identical despite different names*

### Comparing `django_dynaform-0.1.0/dynaform/views.py` & `django_dynaform-0.1.1/dynaform/views.py`

 * *Files identical despite different names*

### Comparing `django_dynaform-0.1.0/setup.cfg` & `django_dynaform-0.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `django_dynaform-0.1.0/setup.py` & `django_dynaform-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `django_dynaform-0.1.0/tests/test_forms.py` & `django_dynaform-0.1.1/tests/test_forms.py`

 * *Files identical despite different names*

