# Comparing `tmp/prelude_cli-1.7.4.tar.gz` & `tmp/prelude_cli-1.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prelude_cli-1.7.4.tar", last modified: Wed Apr 17 18:50:45 2024, max compression
+gzip compressed data, was "prelude_cli-1.7.5.tar", last modified: Wed May  1 21:28:17 2024, max compression
```

## Comparing `prelude_cli-1.7.4.tar` & `prelude_cli-1.7.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-17 18:50:45.430266 prelude_cli-1.7.4/
--rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude_cli-1.7.4/LICENSE
--rw-r--r--   0 pack       (501) staff       (20)       31 2023-01-24 13:01:01.000000 prelude_cli-1.7.4/MANIFEST.in
--rw-r--r--   0 pack       (501) staff       (20)      940 2024-04-17 18:50:45.430079 prelude_cli-1.7.4/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      391 2023-03-01 15:58:44.000000 prelude_cli-1.7.4/README.md
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-17 18:50:45.423944 prelude_cli-1.7.4/prelude_cli/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude_cli-1.7.4/prelude_cli/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     1014 2024-04-03 22:19:39.000000 prelude_cli-1.7.4/prelude_cli/cli.py
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-12-08 16:31:30.000000 prelude_cli-1.7.4/prelude_cli/spinner.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-17 18:50:45.426344 prelude_cli-1.7.4/prelude_cli/templates/
--rw-r--r--   0 pack       (501) staff       (20)     1120 2024-01-05 14:14:44.000000 prelude_cli-1.7.4/prelude_cli/templates/README.md
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude_cli-1.7.4/prelude_cli/templates/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)      261 2024-01-05 14:14:44.000000 prelude_cli-1.7.4/prelude_cli/templates/template.go
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-17 18:50:45.429006 prelude_cli-1.7.4/prelude_cli/views/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude_cli-1.7.4/prelude_cli/views/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)    10043 2024-04-03 22:19:39.000000 prelude_cli-1.7.4/prelude_cli/views/build.py
--rw-r--r--   0 pack       (501) staff       (20)      552 2023-02-08 14:42:44.000000 prelude_cli-1.7.4/prelude_cli/views/configure.py
--rw-r--r--   0 pack       (501) staff       (20)    10255 2024-04-17 18:29:22.000000 prelude_cli-1.7.4/prelude_cli/views/detect.py
--rw-r--r--   0 pack       (501) staff       (20)     2543 2024-04-11 19:46:08.000000 prelude_cli-1.7.4/prelude_cli/views/generate.py
--rw-r--r--   0 pack       (501) staff       (20)     8568 2024-04-17 18:29:22.000000 prelude_cli-1.7.4/prelude_cli/views/iam.py
--rw-r--r--   0 pack       (501) staff       (20)     4771 2024-04-17 18:29:22.000000 prelude_cli-1.7.4/prelude_cli/views/partner.py
--rw-r--r--   0 pack       (501) staff       (20)      662 2024-04-03 22:19:39.000000 prelude_cli-1.7.4/prelude_cli/views/shared.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-17 18:50:45.429602 prelude_cli-1.7.4/prelude_cli.egg-info/
--rw-r--r--   0 pack       (501) staff       (20)      940 2024-04-17 18:50:45.000000 prelude_cli-1.7.4/prelude_cli.egg-info/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      660 2024-04-17 18:50:45.000000 prelude_cli-1.7.4/prelude_cli.egg-info/SOURCES.txt
--rw-r--r--   0 pack       (501) staff       (20)        1 2024-04-17 18:50:45.000000 prelude_cli-1.7.4/prelude_cli.egg-info/dependency_links.txt
--rw-r--r--   0 pack       (501) staff       (20)       48 2024-04-17 18:50:45.000000 prelude_cli-1.7.4/prelude_cli.egg-info/entry_points.txt
--rw-r--r--   0 pack       (501) staff       (20)       48 2024-04-17 18:50:45.000000 prelude_cli-1.7.4/prelude_cli.egg-info/requires.txt
--rw-r--r--   0 pack       (501) staff       (20)       12 2024-04-17 18:50:45.000000 prelude_cli-1.7.4/prelude_cli.egg-info/top_level.txt
--rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude_cli-1.7.4/pyproject.toml
--rw-r--r--   0 pack       (501) staff       (20)      680 2024-04-17 18:50:45.430658 prelude_cli-1.7.4/setup.cfg
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-05-01 21:28:17.317145 prelude_cli-1.7.5/
+-rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude_cli-1.7.5/LICENSE
+-rw-r--r--   0 pack       (501) staff       (20)       31 2023-01-24 13:01:01.000000 prelude_cli-1.7.5/MANIFEST.in
+-rw-r--r--   0 pack       (501) staff       (20)      940 2024-05-01 21:28:17.317036 prelude_cli-1.7.5/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      391 2023-03-01 15:58:44.000000 prelude_cli-1.7.5/README.md
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-05-01 21:28:17.311130 prelude_cli-1.7.5/prelude_cli/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude_cli-1.7.5/prelude_cli/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     1014 2024-04-03 22:19:39.000000 prelude_cli-1.7.5/prelude_cli/cli.py
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-12-08 16:31:30.000000 prelude_cli-1.7.5/prelude_cli/spinner.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-05-01 21:28:17.313032 prelude_cli-1.7.5/prelude_cli/templates/
+-rw-r--r--   0 pack       (501) staff       (20)     1120 2024-01-05 14:14:44.000000 prelude_cli-1.7.5/prelude_cli/templates/README.md
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude_cli-1.7.5/prelude_cli/templates/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)      261 2024-01-05 14:14:44.000000 prelude_cli-1.7.5/prelude_cli/templates/template.go
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-05-01 21:28:17.315969 prelude_cli-1.7.5/prelude_cli/views/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude_cli-1.7.5/prelude_cli/views/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)    10043 2024-04-03 22:19:39.000000 prelude_cli-1.7.5/prelude_cli/views/build.py
+-rw-r--r--   0 pack       (501) staff       (20)      552 2023-02-08 14:42:44.000000 prelude_cli-1.7.5/prelude_cli/views/configure.py
+-rw-r--r--   0 pack       (501) staff       (20)    10400 2024-04-25 18:56:47.000000 prelude_cli-1.7.5/prelude_cli/views/detect.py
+-rw-r--r--   0 pack       (501) staff       (20)     2543 2024-04-11 19:46:08.000000 prelude_cli-1.7.5/prelude_cli/views/generate.py
+-rw-r--r--   0 pack       (501) staff       (20)     8568 2024-04-17 18:29:22.000000 prelude_cli-1.7.5/prelude_cli/views/iam.py
+-rw-r--r--   0 pack       (501) staff       (20)     4771 2024-04-17 18:29:22.000000 prelude_cli-1.7.5/prelude_cli/views/partner.py
+-rw-r--r--   0 pack       (501) staff       (20)      662 2024-04-03 22:19:39.000000 prelude_cli-1.7.5/prelude_cli/views/shared.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-05-01 21:28:17.316699 prelude_cli-1.7.5/prelude_cli.egg-info/
+-rw-r--r--   0 pack       (501) staff       (20)      940 2024-05-01 21:28:17.000000 prelude_cli-1.7.5/prelude_cli.egg-info/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      660 2024-05-01 21:28:17.000000 prelude_cli-1.7.5/prelude_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 pack       (501) staff       (20)        1 2024-05-01 21:28:17.000000 prelude_cli-1.7.5/prelude_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 pack       (501) staff       (20)       48 2024-05-01 21:28:17.000000 prelude_cli-1.7.5/prelude_cli.egg-info/entry_points.txt
+-rw-r--r--   0 pack       (501) staff       (20)       48 2024-05-01 21:28:17.000000 prelude_cli-1.7.5/prelude_cli.egg-info/requires.txt
+-rw-r--r--   0 pack       (501) staff       (20)       12 2024-05-01 21:28:17.000000 prelude_cli-1.7.5/prelude_cli.egg-info/top_level.txt
+-rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude_cli-1.7.5/pyproject.toml
+-rw-r--r--   0 pack       (501) staff       (20)      680 2024-05-01 21:28:17.317487 prelude_cli-1.7.5/setup.cfg
```

### Comparing `prelude_cli-1.7.4/LICENSE` & `prelude_cli-1.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `prelude_cli-1.7.4/PKG-INFO` & `prelude_cli-1.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-cli
-Version: 1.7.4
+Version: 1.7.5
 Summary: For interacting with the Prelude SDK
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prelude_cli-1.7.4/prelude_cli/cli.py` & `prelude_cli-1.7.5/prelude_cli/cli.py`

 * *Files identical despite different names*

### Comparing `prelude_cli-1.7.4/prelude_cli/templates/README.md` & `prelude_cli-1.7.5/prelude_cli/templates/README.md`

 * *Files identical despite different names*

### Comparing `prelude_cli-1.7.4/prelude_cli/views/build.py` & `prelude_cli-1.7.5/prelude_cli/views/build.py`

 * *Files identical despite different names*

### Comparing `prelude_cli-1.7.4/prelude_cli/views/configure.py` & `prelude_cli-1.7.5/prelude_cli/views/configure.py`

 * *Files identical despite different names*

### Comparing `prelude_cli-1.7.4/prelude_cli/views/detect.py` & `prelude_cli-1.7.5/prelude_cli/views/detect.py`

 * *Files 2% similar despite different names*

```diff
@@ -237,20 +237,21 @@
 @click.option('--dos', help='comma-separated list of DOS', type=str)
 @click.option('--endpoints', help='comma-separated list of endpoint IDs', type=str)
 @click.option('--finish', help='end date of activity (end of day)', type=str)
 @click.option('--os', help='comma-separated list of OS', type=str)
 @click.option('--policy', help='comma-separated list of policies', type=str)
 @click.option('--social', help='whether to fetch account-specific or social stats. Applicable to the following views: protected', is_flag=True)
 @click.option('--start', help='start date of activity (beginning of day)', type=str)
+@click.option('--statuses', help='comma-separated list of statuses', type=str)
 @click.option('--techniques', help='comma-separated list of techniques', type=str)
 @click.option('--tests', help='comma-separated list of test IDs', type=str)
 @click.option('--threats', help='comma-separated list of threat IDs', type=str)
 @click.pass_obj
 @handle_api_error
-def describe_activity(controller, control, dos, endpoints, finish, os, policy, social, start, techniques, tests, threats, view):
+def describe_activity(controller, control, dos, endpoints, finish, os, policy, social, start, statuses, techniques, tests, threats, view):
     """ View my Detect results """
     start = parse(start) if start else datetime.now(timezone.utc) - timedelta(days=29)
     finish = parse(finish) if finish else datetime.now(timezone.utc)
     filters = dict(
         start=datetime.combine(start, time.min),
         finish=datetime.combine(finish, time.max)
     )
@@ -262,14 +263,16 @@
         filters['endpoints'] = endpoints
     if os:
         filters['os'] = os
     if policy:
         filters['policy'] = policy
     if social:
         filters['impersonate'] = 'social'
+    if statuses:
+        filters['statuses'] = statuses
     if techniques:
         filters['techniques'] = techniques
     if tests:
         filters['tests'] = tests
     if threats:
         filters['threats'] = threats
```

### Comparing `prelude_cli-1.7.4/prelude_cli/views/generate.py` & `prelude_cli-1.7.5/prelude_cli/views/generate.py`

 * *Files identical despite different names*

### Comparing `prelude_cli-1.7.4/prelude_cli/views/iam.py` & `prelude_cli-1.7.5/prelude_cli/views/iam.py`

 * *Files identical despite different names*

### Comparing `prelude_cli-1.7.4/prelude_cli/views/partner.py` & `prelude_cli-1.7.5/prelude_cli/views/partner.py`

 * *Files identical despite different names*

### Comparing `prelude_cli-1.7.4/prelude_cli/views/shared.py` & `prelude_cli-1.7.5/prelude_cli/views/shared.py`

 * *Files identical despite different names*

### Comparing `prelude_cli-1.7.4/prelude_cli.egg-info/PKG-INFO` & `prelude_cli-1.7.5/prelude_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-cli
-Version: 1.7.4
+Version: 1.7.5
 Summary: For interacting with the Prelude SDK
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prelude_cli-1.7.4/prelude_cli.egg-info/SOURCES.txt` & `prelude_cli-1.7.5/prelude_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prelude_cli-1.7.4/setup.cfg` & `prelude_cli-1.7.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = prelude-cli
-version = 1.7.4
+version = 1.7.5
 author = Prelude Research
 author_email = support@preludesecurity.com
 description = For interacting with the Prelude SDK
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/preludeorg
 classifiers =
```

