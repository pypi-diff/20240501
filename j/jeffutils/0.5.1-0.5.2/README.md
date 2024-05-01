# Comparing `tmp/jeffutils-0.5.1.tar.gz` & `tmp/jeffutils-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jeffutils-0.5.1.tar", last modified: Tue Apr 30 20:42:19 2024, max compression
+gzip compressed data, was "jeffutils-0.5.2.tar", last modified: Wed May  1 21:06:04 2024, max compression
```

## Comparing `jeffutils-0.5.1.tar` & `jeffutils-0.5.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-04-30 20:42:19.202553 jeffutils-0.5.1/
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)     1070 2024-03-16 21:55:37.000000 jeffutils-0.5.1/LICENSE.txt
--rw-r--r--   0 jeffx     (1000) jeffx     (1000)      420 2024-04-30 20:42:19.202553 jeffutils-0.5.1/PKG-INFO
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       12 2024-03-16 21:29:21.000000 jeffutils-0.5.1/README.md
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       84 2024-03-16 21:54:38.000000 jeffutils-0.5.1/pyproject.toml
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       38 2024-04-30 20:42:19.202553 jeffutils-0.5.1/setup.cfg
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      559 2024-04-30 20:42:13.000000 jeffutils-0.5.1/setup.py
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-04-30 20:42:19.202553 jeffutils-0.5.1/src/
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-04-30 20:42:19.202553 jeffutils-0.5.1/src/jeffutils/
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        0 2024-03-16 21:50:41.000000 jeffutils-0.5.1/src/jeffutils/__init__.py
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)    16258 2024-04-30 20:41:26.000000 jeffutils-0.5.1/src/jeffutils/utils.py
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-04-30 20:42:19.202553 jeffutils-0.5.1/src/jeffutils.egg-info/
--rw-r--r--   0 jeffx     (1000) jeffx     (1000)      420 2024-04-30 20:42:19.000000 jeffutils-0.5.1/src/jeffutils.egg-info/PKG-INFO
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      242 2024-04-30 20:42:19.000000 jeffutils-0.5.1/src/jeffutils.egg-info/SOURCES.txt
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        1 2024-04-30 20:42:19.000000 jeffutils-0.5.1/src/jeffutils.egg-info/dependency_links.txt
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       10 2024-04-30 20:42:19.000000 jeffutils-0.5.1/src/jeffutils.egg-info/top_level.txt
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-01 21:06:04.766961 jeffutils-0.5.2/
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)     1070 2024-03-16 21:55:37.000000 jeffutils-0.5.2/LICENSE.txt
+-rw-r--r--   0 jeffx     (1000) jeffx     (1000)      420 2024-05-01 21:06:04.766961 jeffutils-0.5.2/PKG-INFO
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       12 2024-03-16 21:29:21.000000 jeffutils-0.5.2/README.md
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       84 2024-03-16 21:54:38.000000 jeffutils-0.5.2/pyproject.toml
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       38 2024-05-01 21:06:04.766961 jeffutils-0.5.2/setup.cfg
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      559 2024-05-01 21:05:59.000000 jeffutils-0.5.2/setup.py
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-01 21:06:04.766961 jeffutils-0.5.2/src/
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-01 21:06:04.766961 jeffutils-0.5.2/src/jeffutils/
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        0 2024-03-16 21:50:41.000000 jeffutils-0.5.2/src/jeffutils/__init__.py
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)    16271 2024-05-01 21:05:36.000000 jeffutils-0.5.2/src/jeffutils/utils.py
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-01 21:06:04.766961 jeffutils-0.5.2/src/jeffutils.egg-info/
+-rw-r--r--   0 jeffx     (1000) jeffx     (1000)      420 2024-05-01 21:06:04.000000 jeffutils-0.5.2/src/jeffutils.egg-info/PKG-INFO
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      242 2024-05-01 21:06:04.000000 jeffutils-0.5.2/src/jeffutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        1 2024-05-01 21:06:04.000000 jeffutils-0.5.2/src/jeffutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       10 2024-05-01 21:06:04.000000 jeffutils-0.5.2/src/jeffutils.egg-info/top_level.txt
```

### Comparing `jeffutils-0.5.1/LICENSE.txt` & `jeffutils-0.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jeffutils-0.5.1/setup.py` & `jeffutils-0.5.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name='jeffutils',
-    version='0.5.1',
+    version='0.5.2',
     author='Jeff Hansen',
     author_email='jeffxhansen@gmail.com',
     description='A series of useful functions and decorators I use in most of my projects. Feel free to use them as well :)',
     package_dir={"": "src"},
     packages = find_packages(where="src"),
     classifiers=[
         'Programming Language :: Python :: 3',
```

### Comparing `jeffutils-0.5.1/src/jeffutils/utils.py` & `jeffutils-0.5.2/src/jeffutils/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,18 +27,18 @@
 
 def stack_trace(e):
     """returns a string representation of the stack trace to
     help with debugging and error messages
     """
     return "".join(traceback.TracebackException.from_exception(e).format())
 
-def curr_time_str():
+def curr_time_str(format="%m-%d-%Y"):
     """returns the current time as a string YYYY-MM-DD"""
     now = datetime.now(timezone.utc)
-    now_str = now.strftime("%m-%d-%Y")
+    now_str = now.strftime(format)
     return now_str
 
 def current_time(utc=True, string=True, timestamp=False, hour_24=False):
     """prints the current time in YYYY-MM-DD HH:MM pm/am format
     can specify current utc time or current local time
     default local
     """
```

