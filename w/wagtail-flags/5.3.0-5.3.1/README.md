# Comparing `tmp/wagtail-flags-5.3.0.tar.gz` & `tmp/wagtail_flags-5.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-flags-5.3.0.tar", last modified: Fri Mar 10 13:06:23 2023, max compression
+gzip compressed data, was "wagtail_flags-5.3.1.tar", last modified: Wed May  1 15:37:39 2024, max compression
```

## Comparing `wagtail-flags-5.3.0.tar` & `wagtail_flags-5.3.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 13:06:23.686351 wagtail-flags-5.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-03-10 13:06:05.000000 wagtail-flags-5.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-03-10 13:06:05.000000 wagtail-flags-5.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-03-10 13:06:23.686351 wagtail-flags-5.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-03-10 13:06:05.000000 wagtail-flags-5.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-03-10 13:06:05.000000 wagtail-flags-5.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-10 13:06:23.686351 wagtail-flags-5.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-10 13:06:05.000000 wagtail-flags-5.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 13:06:23.682351 wagtail-flags-5.3.0/wagtail_flags.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-03-10 13:06:23.000000 wagtail-flags-5.3.0/wagtail_flags.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-03-10 13:06:23.000000 wagtail-flags-5.3.0/wagtail_flags.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 13:06:23.000000 wagtail-flags-5.3.0/wagtail_flags.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-10 13:06:23.000000 wagtail-flags-5.3.0/wagtail_flags.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-10 13:06:23.000000 wagtail-flags-5.3.0/wagtail_flags.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 13:06:23.686351 wagtail-flags-5.3.0/wagtailflags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 13:06:05.000000 wagtail-flags-5.3.0/wagtailflags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-03-10 13:06:05.000000 wagtail-flags-5.3.0/wagtailflags/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-03-10 13:06:05.000000 wagtail-flags-5.3.0/wagtailflags/conditions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-10 13:06:05.000000 wagtail-flags-5.3.0/wagtailflags/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-10 13:06:05.000000 wagtail-flags-5.3.0/wagtailflags/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 13:06:23.682351 wagtail-flags-5.3.0/wagtailflags/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 13:06:23.682351 wagtail-flags-5.3.0/wagtailflags/static/wagtailflags/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 13:06:23.686351 wagtail-flags-5.3.0/wagtailflags/static/wagtailflags/css/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-10 13:06:05.000000 wagtail-flags-5.3.0/wagtailflags/static/wagtailflags/css/wagtailflags.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 13:06:23.682351 wagtail-flags-5.3.0/wagtailflags/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 13:06:23.686351 wagtail-flags-5.3.0/wagtailflags/templates/wagtailflags/
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-03-10 13:06:05.000000 wagtail-flags-5.3.0/wagtailflags/templates/wagtailflags/flag.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 13:06:23.686351 wagtail-flags-5.3.0/wagtailflags/templates/wagtailflags/flags/
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-03-10 13:06:05.000000 wagtail-flags-5.3.0/wagtailflags/templates/wagtailflags/flags/create_flag.html
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-03-10 13:06:05.000000 wagtail-flags-5.3.0/wagtailflags/templates/wagtailflags/flags/delete_condition.html
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-03-10 13:06:05.000000 wagtail-flags-5.3.0/wagtailflags/templates/wagtailflags/flags/delete_flag.html
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-03-10 13:06:05.000000 wagtail-flags-5.3.0/wagtailflags/templates/wagtailflags/flags/edit_condition.html
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-03-10 13:06:05.000000 wagtail-flags-5.3.0/wagtailflags/templates/wagtailflags/flags/flag_index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 13:06:23.686351 wagtail-flags-5.3.0/wagtailflags/templates/wagtailflags/includes/
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-03-10 13:06:05.000000 wagtail-flags-5.3.0/wagtailflags/templates/wagtailflags/includes/flag_breadcrumbs.html
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-03-10 13:06:05.000000 wagtail-flags-5.3.0/wagtailflags/templates/wagtailflags/includes/flag_header.html
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-03-10 13:06:05.000000 wagtail-flags-5.3.0/wagtailflags/templates/wagtailflags/includes/flag_index.html
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-03-10 13:06:05.000000 wagtail-flags-5.3.0/wagtailflags/templates/wagtailflags/includes/header.html
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-03-10 13:06:05.000000 wagtail-flags-5.3.0/wagtailflags/templates/wagtailflags/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 13:06:23.686351 wagtail-flags-5.3.0/wagtailflags/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 13:06:05.000000 wagtail-flags-5.3.0/wagtailflags/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-03-10 13:06:05.000000 wagtail-flags-5.3.0/wagtailflags/templatetags/wagtailflags_admin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 13:06:23.686351 wagtail-flags-5.3.0/wagtailflags/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 13:06:05.000000 wagtail-flags-5.3.0/wagtailflags/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-03-10 13:06:05.000000 wagtail-flags-5.3.0/wagtailflags/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-03-10 13:06:05.000000 wagtail-flags-5.3.0/wagtailflags/tests/test_apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-03-10 13:06:05.000000 wagtail-flags-5.3.0/wagtailflags/tests/test_conditions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-03-10 13:06:05.000000 wagtail-flags-5.3.0/wagtailflags/tests/test_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-03-10 13:06:05.000000 wagtail-flags-5.3.0/wagtailflags/tests/test_templatetags_wagtailflags_admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-03-10 13:06:05.000000 wagtail-flags-5.3.0/wagtailflags/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-03-10 13:06:05.000000 wagtail-flags-5.3.0/wagtailflags/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 13:06:05.000000 wagtail-flags-5.3.0/wagtailflags/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-03-10 13:06:05.000000 wagtail-flags-5.3.0/wagtailflags/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-03-10 13:06:05.000000 wagtail-flags-5.3.0/wagtailflags/wagtail_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:37:39.817324 wagtail_flags-5.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-05-01 15:37:36.000000 wagtail_flags-5.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-01 15:37:36.000000 wagtail_flags-5.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-05-01 15:37:39.813324 wagtail_flags-5.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4218 2024-05-01 15:37:36.000000 wagtail_flags-5.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-01 15:37:36.000000 wagtail_flags-5.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 15:37:39.817324 wagtail_flags-5.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-01 15:37:36.000000 wagtail_flags-5.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:37:39.813324 wagtail_flags-5.3.1/wagtail_flags.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-05-01 15:37:39.000000 wagtail_flags-5.3.1/wagtail_flags.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-01 15:37:39.000000 wagtail_flags-5.3.1/wagtail_flags.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 15:37:39.000000 wagtail_flags-5.3.1/wagtail_flags.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-01 15:37:39.000000 wagtail_flags-5.3.1/wagtail_flags.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-01 15:37:39.000000 wagtail_flags-5.3.1/wagtail_flags.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:37:39.809324 wagtail_flags-5.3.1/wagtailflags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 15:37:36.000000 wagtail_flags-5.3.1/wagtailflags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-01 15:37:36.000000 wagtail_flags-5.3.1/wagtailflags/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-01 15:37:36.000000 wagtail_flags-5.3.1/wagtailflags/conditions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-01 15:37:36.000000 wagtail_flags-5.3.1/wagtailflags/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-01 15:37:36.000000 wagtail_flags-5.3.1/wagtailflags/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:37:39.805324 wagtail_flags-5.3.1/wagtailflags/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:37:39.805324 wagtail_flags-5.3.1/wagtailflags/static/wagtailflags/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:37:39.809324 wagtail_flags-5.3.1/wagtailflags/static/wagtailflags/css/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 15:37:36.000000 wagtail_flags-5.3.1/wagtailflags/static/wagtailflags/css/wagtailflags.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:37:39.805324 wagtail_flags-5.3.1/wagtailflags/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:37:39.809324 wagtail_flags-5.3.1/wagtailflags/templates/wagtailflags/
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-01 15:37:36.000000 wagtail_flags-5.3.1/wagtailflags/templates/wagtailflags/flag.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:37:39.813324 wagtail_flags-5.3.1/wagtailflags/templates/wagtailflags/flags/
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-01 15:37:36.000000 wagtail_flags-5.3.1/wagtailflags/templates/wagtailflags/flags/create_flag.html
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-01 15:37:36.000000 wagtail_flags-5.3.1/wagtailflags/templates/wagtailflags/flags/delete_condition.html
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-01 15:37:36.000000 wagtail_flags-5.3.1/wagtailflags/templates/wagtailflags/flags/delete_flag.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-01 15:37:36.000000 wagtail_flags-5.3.1/wagtailflags/templates/wagtailflags/flags/edit_condition.html
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-01 15:37:36.000000 wagtail_flags-5.3.1/wagtailflags/templates/wagtailflags/flags/flag_index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:37:39.813324 wagtail_flags-5.3.1/wagtailflags/templates/wagtailflags/includes/
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-01 15:37:36.000000 wagtail_flags-5.3.1/wagtailflags/templates/wagtailflags/includes/flag_breadcrumbs.html
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-01 15:37:36.000000 wagtail_flags-5.3.1/wagtailflags/templates/wagtailflags/includes/flag_header.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-01 15:37:36.000000 wagtail_flags-5.3.1/wagtailflags/templates/wagtailflags/includes/flag_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-01 15:37:36.000000 wagtail_flags-5.3.1/wagtailflags/templates/wagtailflags/includes/header.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-01 15:37:36.000000 wagtail_flags-5.3.1/wagtailflags/templates/wagtailflags/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:37:39.813324 wagtail_flags-5.3.1/wagtailflags/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 15:37:36.000000 wagtail_flags-5.3.1/wagtailflags/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-01 15:37:36.000000 wagtail_flags-5.3.1/wagtailflags/templatetags/wagtailflags_admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:37:39.813324 wagtail_flags-5.3.1/wagtailflags/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 15:37:36.000000 wagtail_flags-5.3.1/wagtailflags/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-05-01 15:37:36.000000 wagtail_flags-5.3.1/wagtailflags/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-01 15:37:36.000000 wagtail_flags-5.3.1/wagtailflags/tests/test_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-01 15:37:36.000000 wagtail_flags-5.3.1/wagtailflags/tests/test_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-01 15:37:36.000000 wagtail_flags-5.3.1/wagtailflags/tests/test_signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-01 15:37:36.000000 wagtail_flags-5.3.1/wagtailflags/tests/test_templatetags_wagtailflags_admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8156 2024-05-01 15:37:36.000000 wagtail_flags-5.3.1/wagtailflags/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-01 15:37:36.000000 wagtail_flags-5.3.1/wagtailflags/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 15:37:36.000000 wagtail_flags-5.3.1/wagtailflags/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-05-01 15:37:36.000000 wagtail_flags-5.3.1/wagtailflags/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-05-01 15:37:36.000000 wagtail_flags-5.3.1/wagtailflags/wagtail_hooks.py
```

### Comparing `wagtail-flags-5.3.0/LICENSE` & `wagtail_flags-5.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail-flags-5.3.0/PKG-INFO` & `wagtail_flags-5.3.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-flags
-Version: 5.3.0
+Version: 5.3.1
 Summary: Feature flags for Wagtail sites
 Author-email: CFPB <tech@cfpb.gov>
 License: CC0
 Project-URL: Homepage, https://github.com/cfpb/wagtail-flags
 Project-URL: Bug Reports, https://github.com/cfpb/wagtail-flags/issues
 Project-URL: Source, https://github.com/cfpb/wagtail-flags
 Classifier: Framework :: Django
@@ -14,16 +14,19 @@
 Classifier: Framework :: Wagtail :: 4
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: License :: Public Domain
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: testing
 License-File: LICENSE
+Requires-Dist: wagtail>=4
+Requires-Dist: django-flags>4.2
+Provides-Extra: testing
+Requires-Dist: coverage[toml]; extra == "testing"
 
 # Wagtail-Flags
 
 [![Build Status](https://github.com/cfpb/wagtail-flags/workflows/test/badge.svg)](https://github.com/cfpb/wagtail-flags/actions?query=workflow%3Atest)
 [![Ethical open source](https://img.shields.io/badge/open-ethical-%234baaaa)](https://ethicalsource.dev/definition/)
 
 Feature flags allow you to toggle functionality based on configurable conditions.
```

### Comparing `wagtail-flags-5.3.0/README.md` & `wagtail_flags-5.3.1/README.md`

 * *Files identical despite different names*

### Comparing `wagtail-flags-5.3.0/pyproject.toml` & `wagtail_flags-5.3.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "wagtail-flags"
-version = "5.3.0"
+version = "5.3.1"
 description = "Feature flags for Wagtail sites"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "CC0"}
 authors = [
     {name = "CFPB", email = "tech@cfpb.gov" }
 ]
```

### Comparing `wagtail-flags-5.3.0/wagtail_flags.egg-info/PKG-INFO` & `wagtail_flags-5.3.1/wagtail_flags.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-flags
-Version: 5.3.0
+Version: 5.3.1
 Summary: Feature flags for Wagtail sites
 Author-email: CFPB <tech@cfpb.gov>
 License: CC0
 Project-URL: Homepage, https://github.com/cfpb/wagtail-flags
 Project-URL: Bug Reports, https://github.com/cfpb/wagtail-flags/issues
 Project-URL: Source, https://github.com/cfpb/wagtail-flags
 Classifier: Framework :: Django
@@ -14,16 +14,19 @@
 Classifier: Framework :: Wagtail :: 4
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: License :: Public Domain
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: testing
 License-File: LICENSE
+Requires-Dist: wagtail>=4
+Requires-Dist: django-flags>4.2
+Provides-Extra: testing
+Requires-Dist: coverage[toml]; extra == "testing"
 
 # Wagtail-Flags
 
 [![Build Status](https://github.com/cfpb/wagtail-flags/workflows/test/badge.svg)](https://github.com/cfpb/wagtail-flags/actions?query=workflow%3Atest)
 [![Ethical open source](https://img.shields.io/badge/open-ethical-%234baaaa)](https://ethicalsource.dev/definition/)
 
 Feature flags allow you to toggle functionality based on configurable conditions.
```

### Comparing `wagtail-flags-5.3.0/wagtail_flags.egg-info/SOURCES.txt` & `wagtail_flags-5.3.1/wagtail_flags.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wagtail-flags-5.3.0/wagtailflags/conditions.py` & `wagtail_flags-5.3.1/wagtailflags/conditions.py`

 * *Files identical despite different names*

### Comparing `wagtail-flags-5.3.0/wagtailflags/forms.py` & `wagtail_flags-5.3.1/wagtailflags/forms.py`

 * *Files identical despite different names*

### Comparing `wagtail-flags-5.3.0/wagtailflags/templates/wagtailflags/flag.svg` & `wagtail_flags-5.3.1/wagtailflags/templates/wagtailflags/flag.svg`

 * *Files identical despite different names*

### Comparing `wagtail-flags-5.3.0/wagtailflags/templates/wagtailflags/flags/create_flag.html` & `wagtail_flags-5.3.1/wagtailflags/templates/wagtailflags/flags/create_flag.html`

 * *Files identical despite different names*

### Comparing `wagtail-flags-5.3.0/wagtailflags/templates/wagtailflags/flags/delete_condition.html` & `wagtail_flags-5.3.1/wagtailflags/templates/wagtailflags/flags/delete_condition.html`

 * *Files identical despite different names*

### Comparing `wagtail-flags-5.3.0/wagtailflags/templates/wagtailflags/flags/delete_flag.html` & `wagtail_flags-5.3.1/wagtailflags/templates/wagtailflags/flags/delete_flag.html`

 * *Files identical despite different names*

### Comparing `wagtail-flags-5.3.0/wagtailflags/templates/wagtailflags/flags/edit_condition.html` & `wagtail_flags-5.3.1/wagtailflags/templates/wagtailflags/flags/edit_condition.html`

 * *Files identical despite different names*

### Comparing `wagtail-flags-5.3.0/wagtailflags/templates/wagtailflags/includes/flag_breadcrumbs.html` & `wagtail_flags-5.3.1/wagtailflags/templates/wagtailflags/includes/flag_breadcrumbs.html`

 * *Files 1% similar despite different names*

```diff
@@ -13,26 +13,26 @@
             <button
                 type="button"
                 data-toggle-breadcrumbs
                 class="w-flex w-items-center w-justify-center w-box-border w-ml-0 w-p-4 w-w-slim-header w-h-full w-bg-transparent w-text-grey-400 w-transition hover:w-scale-110 hover:w-text-primary w-outline-offset-inside"
                 aria-label="{% trans 'Toggle breadcrumbs' %}"
                 aria-expanded="false"
             >
-                {% icon name="breadcrumb-expand" class_name="w-w-4 w-h-4" %}
+                {% icon name="breadcrumb-expand" classname="w-w-4 w-h-4" %}
             </button>
 
             <div class="w-relative w-h-slim-header w-mr-4 w-top-0 w-z-20 w-flex w-items-center w-flex-row w-flex-1 sm:w-flex-none w-transition w-duration-300">
                 <nav class="w-flex w-items-center w-flex-row w-h-full" aria-label="{% trans 'Breadcrumb' %}">
                     <ol class="w-flex w-flex-row w-justify-start w-items-center w-h-full w-pl-0 w-my-0 w-gap-2 sm:w-gap-0 sm:w-space-x-2">
                         {% block breadcrumb_items %}
                             <li class="{{ breadcrumb_item_classes }}">
                                 <a class="{{ breadcrumb_link_classes }}" href="{% url 'wagtailflags:list' %}">
                                     {% trans 'Flags' %}
                                 </a>
-                                {% icon name="arrow-right" class_name=icon_classes %}
+                                {% icon name="arrow-right" classname=icon_classes %}
                             </li>
                             {% if flag %}
                             <li class="{{ breadcrumb_item_classes }}">
                                 <a class="{{ breadcrumb_link_classes }}" href="{% url 'wagtailflags:flag_index' flag.name %}">
                                     {{ title }}
                                 </a>
                             </li>
```

### Comparing `wagtail-flags-5.3.0/wagtailflags/templates/wagtailflags/includes/flag_index.html` & `wagtail_flags-5.3.1/wagtailflags/templates/wagtailflags/includes/flag_index.html`

 * *Files identical despite different names*

### Comparing `wagtail-flags-5.3.0/wagtailflags/templates/wagtailflags/index.html` & `wagtail_flags-5.3.1/wagtailflags/templates/wagtailflags/index.html`

 * *Files identical despite different names*

### Comparing `wagtail-flags-5.3.0/wagtailflags/templatetags/wagtailflags_admin.py` & `wagtail_flags-5.3.1/wagtailflags/templatetags/wagtailflags_admin.py`

 * *Files identical despite different names*

### Comparing `wagtail-flags-5.3.0/wagtailflags/tests/settings.py` & `wagtail_flags-5.3.1/wagtailflags/tests/settings.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,68 +20,45 @@
         "USER": os.environ.get("DATABASE_USER", None),
         "PASSWORD": os.environ.get("DATABASE_PASS", None),
         "HOST": os.environ.get("DATABASE_HOST", None),
         "TEST": {"NAME": os.environ.get("DATABASE_NAME", None)},
     },
 }
 
-WAGTAIL_APPS = (
-    "wagtail.contrib.forms",
-    "wagtail.contrib.modeladmin",
-    "wagtail.contrib.settings",
-    "wagtail.admin",
-    "wagtail.documents",
-    "wagtail.images",
-    "wagtail.snippets",
-    "wagtail.sites",
-    "wagtail.users",
-)
-
-WAGTAIL_APPS += (
-    "wagtail",
-    "wagtail.test.testapp",
-)
-WAGTAILADMIN_RICH_TEXT_EDITORS = {
-    "default": {"WIDGET": "wagtail.admin.rich_text.DraftailRichTextArea"},
-    "custom": {"WIDGET": "wagtail.test.testapp.rich_text.CustomRichTextArea"},
-}
-
 WAGTAILADMIN_BASE_URL = "http://localhost:8000"
 
 MIDDLEWARE = (
     "django.middleware.common.CommonMiddleware",
     "django.contrib.sessions.middleware.SessionMiddleware",
     "django.middleware.csrf.CsrfViewMiddleware",
     "django.contrib.auth.middleware.AuthenticationMiddleware",
     "django.contrib.messages.middleware.MessageMiddleware",
     "django.middleware.clickjacking.XFrameOptionsMiddleware",
 )
 
 INSTALLED_APPS = (
+    "django.contrib.admin",
     "django.contrib.auth",
     "django.contrib.contenttypes",
+    "django.contrib.messages",
     "django.contrib.sessions",
-)
-
-
-INSTALLED_APPS = (
-    (
-        "django.contrib.admin",
-        "django.contrib.auth",
-        "django.contrib.contenttypes",
-        "django.contrib.messages",
-        "django.contrib.sessions",
-        "django.contrib.staticfiles",
-        "taggit",
-    )
-    + WAGTAIL_APPS
-    + (
-        "flags",
-        "wagtailflags",
-    )
+    "django.contrib.staticfiles",
+    "taggit",
+    "wagtail",
+    "wagtail.contrib.forms",
+    "wagtail.contrib.modeladmin",
+    "wagtail.contrib.settings",
+    "wagtail.admin",
+    "wagtail.documents",
+    "wagtail.images",
+    "wagtail.snippets",
+    "wagtail.sites",
+    "wagtail.users",
+    "flags",
+    "wagtailflags",
 )
 
 STATIC_URL = "/static/"
 
 TEMPLATES = [
     {
         "BACKEND": "django.template.backends.django.DjangoTemplates",
```

### Comparing `wagtail-flags-5.3.0/wagtailflags/tests/test_conditions.py` & `wagtail_flags-5.3.1/wagtailflags/tests/test_conditions.py`

 * *Files identical despite different names*

### Comparing `wagtail-flags-5.3.0/wagtailflags/tests/test_signals.py` & `wagtail_flags-5.3.1/wagtailflags/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `wagtail-flags-5.3.0/wagtailflags/tests/test_templatetags_wagtailflags_admin.py` & `wagtail_flags-5.3.1/wagtailflags/tests/test_templatetags_wagtailflags_admin.py`

 * *Files identical despite different names*

### Comparing `wagtail-flags-5.3.0/wagtailflags/tests/test_views.py` & `wagtail_flags-5.3.1/wagtailflags/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `wagtail-flags-5.3.0/wagtailflags/views.py` & `wagtail_flags-5.3.1/wagtailflags/views.py`

 * *Files identical despite different names*

### Comparing `wagtail-flags-5.3.0/wagtailflags/wagtail_hooks.py` & `wagtail_flags-5.3.1/wagtailflags/wagtail_hooks.py`

 * *Files identical despite different names*

