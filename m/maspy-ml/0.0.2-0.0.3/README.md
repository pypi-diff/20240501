# Comparing `tmp/maspy-ml-0.0.2.tar.gz` & `tmp/maspy-ml-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maspy-ml-0.0.2.tar", last modified: Tue Apr 30 17:04:28 2024, max compression
+gzip compressed data, was "maspy-ml-0.0.3.tar", last modified: Tue Apr 30 17:12:40 2024, max compression
```

## Comparing `maspy-ml-0.0.2.tar` & `maspy-ml-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 17:04:28.485208 maspy-ml-0.0.2/
--rw-rw-rw-   0        0        0      631 2024-04-30 17:04:28.484210 maspy-ml-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     5540 2024-04-29 17:06:13.000000 maspy-ml-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-30 17:04:28.434136 maspy-ml-0.0.2/maspy/
--rw-rw-rw-   0        0        0      407 2024-04-29 16:16:10.000000 maspy-ml-0.0.2/maspy/__init__.py
--rw-rw-rw-   0        0        0     4926 2024-04-30 16:55:36.000000 maspy-ml-0.0.2/maspy/admin.py
--rw-rw-rw-   0        0        0    26278 2024-04-30 16:57:27.000000 maspy-ml-0.0.2/maspy/agent.py
--rw-rw-rw-   0        0        0     4305 2024-04-29 16:50:14.000000 maspy-ml-0.0.2/maspy/communication.py
--rw-rw-rw-   0        0        0     4984 2024-04-30 15:23:34.000000 maspy-ml-0.0.2/maspy/environment.py
--rw-rw-rw-   0        0        0      249 2024-04-08 01:20:57.000000 maspy-ml-0.0.2/maspy/error.py
--rw-rw-rw-   0        0        0    28882 2024-03-06 19:42:41.000000 maspy-ml-0.0.2/maspy/learning.py
--rw-rw-rw-   0        0        0      792 2024-04-29 12:28:21.000000 maspy-ml-0.0.2/maspy/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-30 17:04:28.447092 maspy-ml-0.0.2/maspy_ml.egg-info/
--rw-rw-rw-   0        0        0      631 2024-04-30 17:04:28.000000 maspy-ml-0.0.2/maspy_ml.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      378 2024-04-30 17:04:28.000000 maspy-ml-0.0.2/maspy_ml.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 17:04:28.000000 maspy-ml-0.0.2/maspy_ml.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-04-30 17:04:28.000000 maspy-ml-0.0.2/maspy_ml.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-30 17:04:28.485208 maspy-ml-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      925 2024-04-30 16:58:10.000000 maspy-ml-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-30 17:04:28.483213 maspy-ml-0.0.2/tests/
--rw-rw-rw-   0        0        0        0 2024-04-09 03:42:49.000000 maspy-ml-0.0.2/tests/__init__.py
--rw-rw-rw-   0        0        0      154 2024-04-25 19:34:48.000000 maspy-ml-0.0.2/tests/test_agent.py
--rw-rw-rw-   0        0        0     1016 2024-04-24 20:26:45.000000 maspy-ml-0.0.2/tests/test_communication.py
--rw-rw-rw-   0        0        0     3256 2024-04-24 20:26:45.000000 maspy-ml-0.0.2/tests/test_environment.py
+drwxrwxrwx   0        0        0        0 2024-04-30 17:12:40.252163 maspy-ml-0.0.3/
+-rw-rw-rw-   0        0        0      631 2024-04-30 17:12:40.251165 maspy-ml-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5540 2024-04-29 17:06:13.000000 maspy-ml-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-30 17:12:40.241192 maspy-ml-0.0.3/maspy/
+-rw-rw-rw-   0        0        0      407 2024-04-29 16:16:10.000000 maspy-ml-0.0.3/maspy/__init__.py
+-rw-rw-rw-   0        0        0     4926 2024-04-30 16:55:36.000000 maspy-ml-0.0.3/maspy/admin.py
+-rw-rw-rw-   0        0        0    26304 2024-04-30 17:09:07.000000 maspy-ml-0.0.3/maspy/agent.py
+-rw-rw-rw-   0        0        0     4305 2024-04-29 16:50:14.000000 maspy-ml-0.0.3/maspy/communication.py
+-rw-rw-rw-   0        0        0     4984 2024-04-30 15:23:34.000000 maspy-ml-0.0.3/maspy/environment.py
+-rw-rw-rw-   0        0        0      249 2024-04-08 01:20:57.000000 maspy-ml-0.0.3/maspy/error.py
+-rw-rw-rw-   0        0        0    28882 2024-03-06 19:42:41.000000 maspy-ml-0.0.3/maspy/learning.py
+-rw-rw-rw-   0        0        0      792 2024-04-29 12:28:21.000000 maspy-ml-0.0.3/maspy/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-30 17:12:40.247176 maspy-ml-0.0.3/maspy_ml.egg-info/
+-rw-rw-rw-   0        0        0      631 2024-04-30 17:12:40.000000 maspy-ml-0.0.3/maspy_ml.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      378 2024-04-30 17:12:40.000000 maspy-ml-0.0.3/maspy_ml.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 17:12:40.000000 maspy-ml-0.0.3/maspy_ml.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-04-30 17:12:40.000000 maspy-ml-0.0.3/maspy_ml.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-30 17:12:40.252163 maspy-ml-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      925 2024-04-30 17:12:26.000000 maspy-ml-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 17:12:40.250168 maspy-ml-0.0.3/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-09 03:42:49.000000 maspy-ml-0.0.3/tests/__init__.py
+-rw-rw-rw-   0        0        0      154 2024-04-25 19:34:48.000000 maspy-ml-0.0.3/tests/test_agent.py
+-rw-rw-rw-   0        0        0     1016 2024-04-24 20:26:45.000000 maspy-ml-0.0.3/tests/test_communication.py
+-rw-rw-rw-   0        0        0     3256 2024-04-24 20:26:45.000000 maspy-ml-0.0.3/tests/test_environment.py
```

### Comparing `maspy-ml-0.0.2/PKG-INFO` & `maspy-ml-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maspy-ml
-Version: 0.0.2
+Version: 0.0.3
 Summary: Multi-Agent Systems in Python with Machine Learning
 Author: Alexandre Mellado
 Author-email: <melladoallm@gamil.com>
 Keywords: python,autonomous agents,multi-agent system,machine learning
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `maspy-ml-0.0.2/README.md` & `maspy-ml-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `maspy-ml-0.0.2/maspy/admin.py` & `maspy-ml-0.0.3/maspy/admin.py`

 * *Files identical despite different names*

### Comparing `maspy-ml-0.0.2/maspy/agent.py` & `maspy-ml-0.0.3/maspy/agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -641,15 +641,15 @@
                 ctxt = self.get(context,ck_src=False)
                 if not ctxt:
                     break
                 for x in ctxt[0]._args:
                     args += (x,)
             else:    
                 return plan, args
-        self.print(f"Found no applicable plan for {event.change}:{event.data}")
+        self.print(f"Found no applicable plan for {event.change}:{event.data}") if self.full_log else ...
         return None, None
     
     def _execute_plan(self, chosen_plan:Plan, event: Event, args):
         if not chosen_plan:
             return None
         try:
             return self._run_plan(chosen_plan,event.data,args)
```

### Comparing `maspy-ml-0.0.2/maspy/communication.py` & `maspy-ml-0.0.3/maspy/communication.py`

 * *Files identical despite different names*

### Comparing `maspy-ml-0.0.2/maspy/environment.py` & `maspy-ml-0.0.3/maspy/environment.py`

 * *Files identical despite different names*

### Comparing `maspy-ml-0.0.2/maspy/learning.py` & `maspy-ml-0.0.3/maspy/learning.py`

 * *Files identical despite different names*

### Comparing `maspy-ml-0.0.2/maspy/utils.py` & `maspy-ml-0.0.3/maspy/utils.py`

 * *Files identical despite different names*

### Comparing `maspy-ml-0.0.2/maspy_ml.egg-info/PKG-INFO` & `maspy-ml-0.0.3/maspy_ml.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maspy-ml
-Version: 0.0.2
+Version: 0.0.3
 Summary: Multi-Agent Systems in Python with Machine Learning
 Author: Alexandre Mellado
 Author-email: <melladoallm@gamil.com>
 Keywords: python,autonomous agents,multi-agent system,machine learning
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `maspy-ml-0.0.2/setup.py` & `maspy-ml-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'Multi-Agent Systems in Python with Machine Learning'
 LONG_DESCRIPTION = 'A library for the devolopment of multi-agent systems with components of machine learning'
 
 # Setting up
 setup(
     name="maspy-ml",
     version=VERSION,
```

### Comparing `maspy-ml-0.0.2/tests/test_communication.py` & `maspy-ml-0.0.3/tests/test_communication.py`

 * *Files identical despite different names*

### Comparing `maspy-ml-0.0.2/tests/test_environment.py` & `maspy-ml-0.0.3/tests/test_environment.py`

 * *Files identical despite different names*

