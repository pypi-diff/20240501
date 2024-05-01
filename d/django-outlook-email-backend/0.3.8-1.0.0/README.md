# Comparing `tmp/django_outlook_email_backend-0.3.8.tar.gz` & `tmp/django_outlook_email_backend-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_outlook_email_backend-0.3.8.tar", last modified: Tue Apr 30 20:15:27 2024, max compression
+gzip compressed data, was "django_outlook_email_backend-1.0.0.tar", last modified: Wed May  1 11:47:16 2024, max compression
```

## Comparing `django_outlook_email_backend-0.3.8.tar` & `django_outlook_email_backend-1.0.0.tar`

### file list

```diff
@@ -1,12 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:15:27.447795 django_outlook_email_backend-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-30 20:15:27.447795 django_outlook_email_backend-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-30 20:15:17.000000 django_outlook_email_backend-0.3.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-04-30 20:15:17.000000 django_outlook_email_backend-0.3.8/django_oauth2_email.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:15:27.447795 django_outlook_email_backend-0.3.8/django_outlook_email_backend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-30 20:15:27.000000 django_outlook_email_backend-0.3.8/django_outlook_email_backend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-30 20:15:27.000000 django_outlook_email_backend-0.3.8/django_outlook_email_backend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 20:15:27.000000 django_outlook_email_backend-0.3.8/django_outlook_email_backend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-30 20:15:27.000000 django_outlook_email_backend-0.3.8/django_outlook_email_backend.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 20:15:27.000000 django_outlook_email_backend-0.3.8/django_outlook_email_backend.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 20:15:27.447795 django_outlook_email_backend-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-30 20:15:17.000000 django_outlook_email_backend-0.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:47:16.729891 django_outlook_email_backend-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-01 11:47:16.729891 django_outlook_email_backend-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-01 11:47:13.000000 django_outlook_email_backend-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:47:16.725891 django_outlook_email_backend-1.0.0/django_outlook_email/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 11:47:13.000000 django_outlook_email_backend-1.0.0/django_outlook_email/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-01 11:47:13.000000 django_outlook_email_backend-1.0.0/django_outlook_email/django_outlook_email_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:47:16.725891 django_outlook_email_backend-1.0.0/django_outlook_email/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 11:47:13.000000 django_outlook_email_backend-1.0.0/django_outlook_email/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-01 11:47:13.000000 django_outlook_email_backend-1.0.0/django_outlook_email/exceptions/microsoft_graph_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:47:16.729891 django_outlook_email_backend-1.0.0/django_outlook_email_backend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-01 11:47:16.000000 django_outlook_email_backend-1.0.0/django_outlook_email_backend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-01 11:47:16.000000 django_outlook_email_backend-1.0.0/django_outlook_email_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 11:47:16.000000 django_outlook_email_backend-1.0.0/django_outlook_email_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-01 11:47:16.000000 django_outlook_email_backend-1.0.0/django_outlook_email_backend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-01 11:47:16.000000 django_outlook_email_backend-1.0.0/django_outlook_email_backend.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 11:47:16.000000 django_outlook_email_backend-1.0.0/django_outlook_email_backend.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 11:47:16.729891 django_outlook_email_backend-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-01 11:47:13.000000 django_outlook_email_backend-1.0.0/setup.py
```

### Comparing `django_outlook_email_backend-0.3.8/setup.py` & `django_outlook_email_backend-1.0.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 
 setup(
-    name='django-outlook-email-backend',
-    version='0.3.8',
+    name='django_outlook_email-backend',
+    version='1.0.0',
     description='Ouauth2 outlook email backend for Django',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Marc Claramunt',
     author_email='mclaramunt@enley.com',
     license='MIT',
     zip_safe=True,
@@ -16,8 +16,10 @@
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
     url='https://github.com/enley-es/django-outlook-email-backend',
+    packages=["django_outlook_email","django_outlook_email.exceptions"],
+    install_requires = ['requests~=2.25', 'msal==1.*']
 )
```

