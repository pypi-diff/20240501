# Comparing `tmp/ocp_tessellate-2.3.2.tar.gz` & `tmp/ocp_tessellate-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocp_tessellate-2.3.2.tar", last modified: Mon Apr 22 06:39:28 2024, max compression
+gzip compressed data, was "ocp_tessellate-2.3.3.tar", last modified: Wed May  1 16:38:49 2024, max compression
```

## Comparing `ocp_tessellate-2.3.2.tar` & `ocp_tessellate-2.3.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2024-04-22 06:39:28.569401 ocp_tessellate-2.3.2/
--rw-r--r--   0 bernhard   (501) staff       (20)     1109 2024-04-22 06:39:28.569320 ocp_tessellate-2.3.2/PKG-INFO
--rw-r--r--   0 bernhard   (501) staff       (20)       17 2023-01-23 07:09:46.000000 ocp_tessellate-2.3.2/README.md
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2024-04-22 06:39:28.566524 ocp_tessellate-2.3.2/ocp_tessellate/
--rw-r--r--   0 bernhard   (501) staff       (20)     2942 2024-04-14 10:24:20.000000 ocp_tessellate-2.3.2/ocp_tessellate/__init__.py
--rw-r--r--   0 bernhard   (501) staff       (20)     1123 2024-04-20 11:53:24.000000 ocp_tessellate-2.3.2/ocp_tessellate/_version.py
--rw-r--r--   0 bernhard   (501) staff       (20)     4452 2024-04-20 12:24:45.000000 ocp_tessellate-2.3.2/ocp_tessellate/b123d_assembly.py
--rw-r--r--   0 bernhard   (501) staff       (20)    15298 2024-04-22 06:38:46.000000 ocp_tessellate-2.3.2/ocp_tessellate/cad_objects.py
--rw-r--r--   0 bernhard   (501) staff       (20)    34183 2024-04-22 06:38:46.000000 ocp_tessellate-2.3.2/ocp_tessellate/convert.py
--rw-r--r--   0 bernhard   (501) staff       (20)    10324 2024-04-20 16:35:57.000000 ocp_tessellate-2.3.2/ocp_tessellate/defaults.py
--rw-r--r--   0 bernhard   (501) staff       (20)    25136 2024-03-14 07:11:29.000000 ocp_tessellate-2.3.2/ocp_tessellate/ocp_utils.py
--rw-r--r--   0 bernhard   (501) staff       (20)    13711 2024-04-20 12:25:36.000000 ocp_tessellate-2.3.2/ocp_tessellate/stepreader.py
--rw-r--r--   0 bernhard   (501) staff       (20)    18104 2024-04-22 06:38:46.000000 ocp_tessellate-2.3.2/ocp_tessellate/tessellator.py
--rw-r--r--   0 bernhard   (501) staff       (20)     1065 2023-11-24 07:13:16.000000 ocp_tessellate-2.3.2/ocp_tessellate/trace.py
--rw-r--r--   0 bernhard   (501) staff       (20)     6177 2024-04-14 10:38:44.000000 ocp_tessellate-2.3.2/ocp_tessellate/utils.py
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2024-04-22 06:39:28.568910 ocp_tessellate-2.3.2/ocp_tessellate.egg-info/
--rw-r--r--   0 bernhard   (501) staff       (20)     1109 2024-04-22 06:39:28.000000 ocp_tessellate-2.3.2/ocp_tessellate.egg-info/PKG-INFO
--rw-r--r--   0 bernhard   (501) staff       (20)      949 2024-04-22 06:39:28.000000 ocp_tessellate-2.3.2/ocp_tessellate.egg-info/SOURCES.txt
--rw-r--r--   0 bernhard   (501) staff       (20)        1 2024-04-22 06:39:28.000000 ocp_tessellate-2.3.2/ocp_tessellate.egg-info/dependency_links.txt
--rw-r--r--   0 bernhard   (501) staff       (20)        1 2024-04-22 06:39:28.000000 ocp_tessellate-2.3.2/ocp_tessellate.egg-info/not-zip-safe
--rw-r--r--   0 bernhard   (501) staff       (20)      112 2024-04-22 06:39:28.000000 ocp_tessellate-2.3.2/ocp_tessellate.egg-info/requires.txt
--rw-r--r--   0 bernhard   (501) staff       (20)       15 2024-04-22 06:39:28.000000 ocp_tessellate-2.3.2/ocp_tessellate.egg-info/top_level.txt
--rw-r--r--   0 bernhard   (501) staff       (20)      671 2024-04-22 06:39:28.569654 ocp_tessellate-2.3.2/setup.cfg
--rw-r--r--   0 bernhard   (501) staff       (20)     1627 2024-04-21 12:51:04.000000 ocp_tessellate-2.3.2/setup.py
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2024-04-22 06:39:28.568755 ocp_tessellate-2.3.2/tests/
--rw-r--r--   0 bernhard   (501) staff       (20)     1419 2024-03-21 20:20:19.000000 ocp_tessellate-2.3.2/tests/test_cache.py
--rw-r--r--   0 bernhard   (501) staff       (20)     1100 2024-04-18 07:02:00.000000 ocp_tessellate-2.3.2/tests/test_cadquery_sketch.py
--rw-r--r--   0 bernhard   (501) staff       (20)      895 2024-04-18 06:37:27.000000 ocp_tessellate-2.3.2/tests/test_color.py
--rw-r--r--   0 bernhard   (501) staff       (20)     1200 2023-06-19 17:26:20.000000 ocp_tessellate-2.3.2/tests/test_coordsystem.py
--rw-r--r--   0 bernhard   (501) staff       (20)     1999 2024-04-18 06:38:50.000000 ocp_tessellate-2.3.2/tests/test_instances.py
--rw-r--r--   0 bernhard   (501) staff       (20)      486 2024-04-20 16:35:15.000000 ocp_tessellate-2.3.2/tests/test_parallel.py
--rw-r--r--   0 bernhard   (501) staff       (20)      870 2023-11-24 07:13:16.000000 ocp_tessellate-2.3.2/tests/test_partgroup.py
--rw-r--r--   0 bernhard   (501) staff       (20)      766 2024-04-20 11:45:07.000000 ocp_tessellate-2.3.2/tests/test_stl.py
--rw-r--r--   0 bernhard   (501) staff       (20)      811 2024-04-18 06:53:11.000000 ocp_tessellate-2.3.2/tests/tests_build123d assembly.py
--rw-r--r--   0 bernhard   (501) staff       (20)     8564 2024-04-22 06:37:55.000000 ocp_tessellate-2.3.2/tests/tests_build123d hinge.py
--rw-r--r--   0 bernhard   (501) staff       (20)     3328 2023-11-28 20:16:07.000000 ocp_tessellate-2.3.2/tests/tests_build123d.py
--rw-r--r--   0 bernhard   (501) staff       (20)     1879 2023-07-21 16:20:28.000000 ocp_tessellate-2.3.2/tests/tests_cadquery.py
--rw-r--r--   0 bernhard   (501) staff       (20)     3022 2023-06-19 17:42:50.000000 ocp_tessellate-2.3.2/tests/tests_cadquery_boxes.py
--rw-r--r--   0 bernhard   (501) staff       (20)     3697 2023-07-21 16:20:28.000000 ocp_tessellate-2.3.2/tests/tests_cadquery_door.py
--rw-r--r--   0 bernhard   (501) staff       (20)     8496 2023-11-21 06:59:53.000000 ocp_tessellate-2.3.2/tests/tests_cadquery_hexapod.py
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2024-05-01 16:38:49.795728 ocp_tessellate-2.3.3/
+-rw-r--r--   0 bernhard   (501) staff       (20)     1109 2024-05-01 16:38:49.795665 ocp_tessellate-2.3.3/PKG-INFO
+-rw-r--r--   0 bernhard   (501) staff       (20)       17 2023-01-23 07:09:46.000000 ocp_tessellate-2.3.3/README.md
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2024-05-01 16:38:49.792729 ocp_tessellate-2.3.3/ocp_tessellate/
+-rw-r--r--   0 bernhard   (501) staff       (20)     2942 2024-04-14 10:24:20.000000 ocp_tessellate-2.3.3/ocp_tessellate/__init__.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     1123 2024-05-01 15:00:59.000000 ocp_tessellate-2.3.3/ocp_tessellate/_version.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     4452 2024-04-20 12:24:45.000000 ocp_tessellate-2.3.3/ocp_tessellate/b123d_assembly.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    15298 2024-05-01 14:59:35.000000 ocp_tessellate-2.3.3/ocp_tessellate/cad_objects.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    34018 2024-05-01 15:00:44.000000 ocp_tessellate-2.3.3/ocp_tessellate/convert.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    10324 2024-04-20 16:35:57.000000 ocp_tessellate-2.3.3/ocp_tessellate/defaults.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    25136 2024-05-01 14:59:35.000000 ocp_tessellate-2.3.3/ocp_tessellate/ocp_utils.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    13711 2024-04-20 12:25:36.000000 ocp_tessellate-2.3.3/ocp_tessellate/stepreader.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    18104 2024-05-01 14:59:35.000000 ocp_tessellate-2.3.3/ocp_tessellate/tessellator.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     1065 2023-11-24 07:13:16.000000 ocp_tessellate-2.3.3/ocp_tessellate/trace.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     6177 2024-04-14 10:38:44.000000 ocp_tessellate-2.3.3/ocp_tessellate/utils.py
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2024-05-01 16:38:49.795248 ocp_tessellate-2.3.3/ocp_tessellate.egg-info/
+-rw-r--r--   0 bernhard   (501) staff       (20)     1109 2024-05-01 16:38:49.000000 ocp_tessellate-2.3.3/ocp_tessellate.egg-info/PKG-INFO
+-rw-r--r--   0 bernhard   (501) staff       (20)      949 2024-05-01 16:38:49.000000 ocp_tessellate-2.3.3/ocp_tessellate.egg-info/SOURCES.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)        1 2024-05-01 16:38:49.000000 ocp_tessellate-2.3.3/ocp_tessellate.egg-info/dependency_links.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)        1 2024-05-01 16:38:49.000000 ocp_tessellate-2.3.3/ocp_tessellate.egg-info/not-zip-safe
+-rw-r--r--   0 bernhard   (501) staff       (20)      112 2024-05-01 16:38:49.000000 ocp_tessellate-2.3.3/ocp_tessellate.egg-info/requires.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)       15 2024-05-01 16:38:49.000000 ocp_tessellate-2.3.3/ocp_tessellate.egg-info/top_level.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)      671 2024-05-01 16:38:49.795976 ocp_tessellate-2.3.3/setup.cfg
+-rw-r--r--   0 bernhard   (501) staff       (20)     1627 2024-05-01 15:00:59.000000 ocp_tessellate-2.3.3/setup.py
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2024-05-01 16:38:49.795081 ocp_tessellate-2.3.3/tests/
+-rw-r--r--   0 bernhard   (501) staff       (20)     1419 2024-03-21 20:20:19.000000 ocp_tessellate-2.3.3/tests/test_cache.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     1100 2024-04-22 06:56:06.000000 ocp_tessellate-2.3.3/tests/test_cadquery_sketch.py
+-rw-r--r--   0 bernhard   (501) staff       (20)      895 2024-04-18 06:37:27.000000 ocp_tessellate-2.3.3/tests/test_color.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     1200 2023-06-19 17:26:20.000000 ocp_tessellate-2.3.3/tests/test_coordsystem.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     1999 2024-04-18 06:38:50.000000 ocp_tessellate-2.3.3/tests/test_instances.py
+-rw-r--r--   0 bernhard   (501) staff       (20)      486 2024-04-20 16:35:15.000000 ocp_tessellate-2.3.3/tests/test_parallel.py
+-rw-r--r--   0 bernhard   (501) staff       (20)      870 2023-11-24 07:13:16.000000 ocp_tessellate-2.3.3/tests/test_partgroup.py
+-rw-r--r--   0 bernhard   (501) staff       (20)      766 2024-04-20 11:45:07.000000 ocp_tessellate-2.3.3/tests/test_stl.py
+-rw-r--r--   0 bernhard   (501) staff       (20)      811 2024-04-18 06:53:11.000000 ocp_tessellate-2.3.3/tests/tests_build123d assembly.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     8564 2024-04-22 06:37:55.000000 ocp_tessellate-2.3.3/tests/tests_build123d hinge.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     3328 2023-11-28 20:16:07.000000 ocp_tessellate-2.3.3/tests/tests_build123d.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     1879 2023-07-21 16:20:28.000000 ocp_tessellate-2.3.3/tests/tests_cadquery.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     3022 2023-06-19 17:42:50.000000 ocp_tessellate-2.3.3/tests/tests_cadquery_boxes.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     3697 2023-07-21 16:20:28.000000 ocp_tessellate-2.3.3/tests/tests_cadquery_door.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     8496 2023-11-21 06:59:53.000000 ocp_tessellate-2.3.3/tests/tests_cadquery_hexapod.py
```

### Comparing `ocp_tessellate-2.3.2/PKG-INFO` & `ocp_tessellate-2.3.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocp_tessellate
-Version: 2.3.2
+Version: 2.3.3
 Summary: Tessellate OCP objects
 Home-page: https://github.com/bernhard-42/ocp-tessellate
 Author: Bernhard Walter
 Author-email: b_walter@arcor.de
 Keywords: CAD,cadquery
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: IPython
@@ -18,14 +18,14 @@
 Requires-Python: >=3.9
 Requires-Dist: webcolors~=1.12
 Requires-Dist: numpy
 Requires-Dist: numpy-quaternion
 Requires-Dist: cachetools~=5.2.0
 Requires-Dist: imagesize
 Provides-Extra: dev
-Requires-Dist: bumpversion; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 Requires-Dist: black; extra == "dev"
+Requires-Dist: bumpversion; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: pyYaml; extra == "dev"
 
 Tessellate OCP (https://github.com/cadquery/OCP) objects to use with threejs
```

### Comparing `ocp_tessellate-2.3.2/ocp_tessellate/__init__.py` & `ocp_tessellate-2.3.3/ocp_tessellate/__init__.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-2.3.2/ocp_tessellate/_version.py` & `ocp_tessellate-2.3.3/ocp_tessellate/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,9 +24,9 @@
     r = re.compile(
         r"(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)\-{0,1}(?P<release>\D*)(?P<build>\d*)"
     )
     major, minor, patch, release, build = r.match(version).groups()
     return VersionInfo(major, minor, patch, release, build)
 
 
-__version__ = "2.3.2"  # DO NOT EDIT THIS DIRECTLY!  It is managed by bumpversion
+__version__ = "2.3.3"  # DO NOT EDIT THIS DIRECTLY!  It is managed by bumpversion
 __version_info__ = get_version(__version__)
```

### Comparing `ocp_tessellate-2.3.2/ocp_tessellate/b123d_assembly.py` & `ocp_tessellate-2.3.3/ocp_tessellate/b123d_assembly.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-2.3.2/ocp_tessellate/cad_objects.py` & `ocp_tessellate-2.3.3/ocp_tessellate/cad_objects.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-2.3.2/ocp_tessellate/convert.py` & `ocp_tessellate-2.3.3/ocp_tessellate/convert.py`

 * *Files 1% similar despite different names*

```diff
@@ -549,18 +549,14 @@
             len(cad_obj.objects) == 0
             or (len(cad_obj.objects) == 1 and is_vector(cad_obj.objects[0]))
         ):  # Workplane:
             cad_obj = cad_obj.plane.location
             if obj_name is None:
                 obj_name = "workplane"
 
-        # ensure builder objects participate in finding instances
-        if is_build123d(cad_obj) and hasattr(cad_obj, "_obj"):
-            cad_obj = cad_obj._obj
-
         if is_cadquery_assembly(cad_obj):
             _debug("to_assembly: cadquery assembly", obj_name)
 
             add_to_ass = False
             if is_assembly:
                 ass = pg
                 ass.name = cad_obj.name
```

### Comparing `ocp_tessellate-2.3.2/ocp_tessellate/defaults.py` & `ocp_tessellate-2.3.3/ocp_tessellate/defaults.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-2.3.2/ocp_tessellate/ocp_utils.py` & `ocp_tessellate-2.3.3/ocp_tessellate/ocp_utils.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-2.3.2/ocp_tessellate/stepreader.py` & `ocp_tessellate-2.3.3/ocp_tessellate/stepreader.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-2.3.2/ocp_tessellate/tessellator.py` & `ocp_tessellate-2.3.3/ocp_tessellate/tessellator.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-2.3.2/ocp_tessellate/trace.py` & `ocp_tessellate-2.3.3/ocp_tessellate/trace.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-2.3.2/ocp_tessellate/utils.py` & `ocp_tessellate-2.3.3/ocp_tessellate/utils.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-2.3.2/ocp_tessellate.egg-info/PKG-INFO` & `ocp_tessellate-2.3.3/ocp_tessellate.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocp_tessellate
-Version: 2.3.2
+Version: 2.3.3
 Summary: Tessellate OCP objects
 Home-page: https://github.com/bernhard-42/ocp-tessellate
 Author: Bernhard Walter
 Author-email: b_walter@arcor.de
 Keywords: CAD,cadquery
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: IPython
@@ -18,14 +18,14 @@
 Requires-Python: >=3.9
 Requires-Dist: webcolors~=1.12
 Requires-Dist: numpy
 Requires-Dist: numpy-quaternion
 Requires-Dist: cachetools~=5.2.0
 Requires-Dist: imagesize
 Provides-Extra: dev
-Requires-Dist: bumpversion; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 Requires-Dist: black; extra == "dev"
+Requires-Dist: bumpversion; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: pyYaml; extra == "dev"
 
 Tessellate OCP (https://github.com/cadquery/OCP) objects to use with threejs
```

### Comparing `ocp_tessellate-2.3.2/ocp_tessellate.egg-info/SOURCES.txt` & `ocp_tessellate-2.3.3/ocp_tessellate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-2.3.2/setup.cfg` & `ocp_tessellate-2.3.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 2.3.2
+current_version = 2.3.3
 commit = False
 tag = False
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(?P<release>\D*)(?P<build>\d*)
 serialize = 
 	{major}.{minor}.{patch}{release}{build}
 	{major}.{minor}.{patch}
```

### Comparing `ocp_tessellate-2.3.2/setup.py` & `ocp_tessellate-2.3.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 LONG_DESCRIPTION = (
     "Tessellate OCP (https://github.com/cadquery/OCP) objects to use with threejs"
 )
 
 setup_args = {
     "name": "ocp_tessellate",
-    "version": "2.3.2",
+    "version": "2.3.3",
     "description": "Tessellate OCP objects",
     "long_description": LONG_DESCRIPTION,
     "include_package_data": True,
     "python_requires": ">=3.9",
     "install_requires": [
         "webcolors~=1.12",
         "numpy",
```

### Comparing `ocp_tessellate-2.3.2/tests/test_cache.py` & `ocp_tessellate-2.3.3/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-2.3.2/tests/test_cadquery_sketch.py` & `ocp_tessellate-2.3.3/tests/test_cadquery_sketch.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-2.3.2/tests/test_color.py` & `ocp_tessellate-2.3.3/tests/test_color.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-2.3.2/tests/test_coordsystem.py` & `ocp_tessellate-2.3.3/tests/test_coordsystem.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-2.3.2/tests/test_instances.py` & `ocp_tessellate-2.3.3/tests/test_instances.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-2.3.2/tests/test_partgroup.py` & `ocp_tessellate-2.3.3/tests/test_partgroup.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-2.3.2/tests/test_stl.py` & `ocp_tessellate-2.3.3/tests/test_stl.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-2.3.2/tests/tests_build123d assembly.py` & `ocp_tessellate-2.3.3/tests/tests_build123d assembly.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-2.3.2/tests/tests_build123d hinge.py` & `ocp_tessellate-2.3.3/tests/tests_build123d hinge.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-2.3.2/tests/tests_build123d.py` & `ocp_tessellate-2.3.3/tests/tests_build123d.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-2.3.2/tests/tests_cadquery.py` & `ocp_tessellate-2.3.3/tests/tests_cadquery.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-2.3.2/tests/tests_cadquery_boxes.py` & `ocp_tessellate-2.3.3/tests/tests_cadquery_boxes.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-2.3.2/tests/tests_cadquery_door.py` & `ocp_tessellate-2.3.3/tests/tests_cadquery_door.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-2.3.2/tests/tests_cadquery_hexapod.py` & `ocp_tessellate-2.3.3/tests/tests_cadquery_hexapod.py`

 * *Files identical despite different names*

