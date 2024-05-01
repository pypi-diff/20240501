# Comparing `tmp/forwardkinematics-1.2.1.tar.gz` & `tmp/forwardkinematics-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forwardkinematics-1.2.1.tar", max compression
+gzip compressed data, was "forwardkinematics-1.2.2.tar", max compression
```

## Comparing `forwardkinematics-1.2.1.tar` & `forwardkinematics-1.2.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0      582 2024-04-15 13:03:46.485598 forwardkinematics-1.2.1/README.md
--rw-r--r--   0        0        0      205 2024-04-15 13:04:03.309632 forwardkinematics-1.2.1/forwardkinematics/__init__.py
--rw-r--r--   0        0        0      330 2024-04-15 13:03:46.485598 forwardkinematics-1.2.1/forwardkinematics/fksCommon/fk.py
--rw-r--r--   0        0        0     2344 2024-04-15 13:03:46.485598 forwardkinematics-1.2.1/forwardkinematics/planarFks/planarArmFk.py
--rw-r--r--   0        0        0      677 2024-04-15 13:03:46.485598 forwardkinematics-1.2.1/forwardkinematics/planarFks/planar_fk.py
--rw-r--r--   0        0        0        0 2024-04-15 13:03:46.485598 forwardkinematics-1.2.1/forwardkinematics/urdfFks/casadiConversion/__init__.py
--rw-r--r--   0        0        0        0 2024-04-15 13:03:46.485598 forwardkinematics-1.2.1/forwardkinematics/urdfFks/casadiConversion/geometry/__init__.py
--rw-r--r--   0        0        0     3442 2024-04-15 13:03:46.485598 forwardkinematics-1.2.1/forwardkinematics/urdfFks/casadiConversion/geometry/transformation_matrix.py
--rw-r--r--   0        0        0     6240 2024-04-15 13:03:46.485598 forwardkinematics-1.2.1/forwardkinematics/urdfFks/casadiConversion/urdfparser.py
--rw-r--r--   0        0        0      122 2024-04-15 13:03:46.485598 forwardkinematics-1.2.1/forwardkinematics/urdfFks/generic_urdf_fk.py
--rw-r--r--   0        0        0     4151 2024-04-15 13:03:46.485598 forwardkinematics-1.2.1/forwardkinematics/urdfFks/urdfFk.py
--rw-r--r--   0        0        0     7616 2024-04-15 13:04:03.309632 forwardkinematics-1.2.1/forwardkinematics/xmlFks/generic_xml_fk.py
--rw-r--r--   0        0        0      762 2024-04-15 13:04:03.309632 forwardkinematics-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     1486 1970-01-01 00:00:00.000000 forwardkinematics-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0      582 2024-05-01 00:35:45.524049 forwardkinematics-1.2.2/README.md
+-rw-r--r--   0        0        0      205 2024-05-01 00:35:45.524049 forwardkinematics-1.2.2/forwardkinematics/__init__.py
+-rw-r--r--   0        0        0      940 2024-05-01 00:36:05.380183 forwardkinematics-1.2.2/forwardkinematics/fksCommon/fk.py
+-rw-r--r--   0        0        0     2565 2024-05-01 00:36:05.380183 forwardkinematics-1.2.2/forwardkinematics/planarFks/planarArmFk.py
+-rw-r--r--   0        0        0     1269 2024-05-01 00:36:05.380183 forwardkinematics-1.2.2/forwardkinematics/planarFks/planar_fk.py
+-rw-r--r--   0        0        0     1617 2024-05-01 00:36:05.380183 forwardkinematics-1.2.2/forwardkinematics/planarFks/point_fk.py
+-rw-r--r--   0        0        0        0 2024-05-01 00:35:45.524049 forwardkinematics-1.2.2/forwardkinematics/urdfFks/casadiConversion/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-01 00:35:45.524049 forwardkinematics-1.2.2/forwardkinematics/urdfFks/casadiConversion/geometry/__init__.py
+-rw-r--r--   0        0        0     3442 2024-05-01 00:35:45.524049 forwardkinematics-1.2.2/forwardkinematics/urdfFks/casadiConversion/geometry/transformation_matrix.py
+-rw-r--r--   0        0        0     6240 2024-05-01 00:35:45.524049 forwardkinematics-1.2.2/forwardkinematics/urdfFks/casadiConversion/urdfparser.py
+-rw-r--r--   0        0        0      122 2024-05-01 00:35:45.524049 forwardkinematics-1.2.2/forwardkinematics/urdfFks/generic_urdf_fk.py
+-rw-r--r--   0        0        0     4151 2024-05-01 00:35:45.524049 forwardkinematics-1.2.2/forwardkinematics/urdfFks/urdfFk.py
+-rw-r--r--   0        0        0     7616 2024-05-01 00:35:45.524049 forwardkinematics-1.2.2/forwardkinematics/xmlFks/generic_xml_fk.py
+-rw-r--r--   0        0        0      762 2024-05-01 00:36:05.380183 forwardkinematics-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1486 1970-01-01 00:00:00.000000 forwardkinematics-1.2.2/PKG-INFO
```

### Comparing `forwardkinematics-1.2.1/README.md` & `forwardkinematics-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `forwardkinematics-1.2.1/forwardkinematics/urdfFks/casadiConversion/geometry/transformation_matrix.py` & `forwardkinematics-1.2.2/forwardkinematics/urdfFks/casadiConversion/geometry/transformation_matrix.py`

 * *Files identical despite different names*

### Comparing `forwardkinematics-1.2.1/forwardkinematics/urdfFks/casadiConversion/urdfparser.py` & `forwardkinematics-1.2.2/forwardkinematics/urdfFks/casadiConversion/urdfparser.py`

 * *Files identical despite different names*

### Comparing `forwardkinematics-1.2.1/forwardkinematics/urdfFks/urdfFk.py` & `forwardkinematics-1.2.2/forwardkinematics/urdfFks/urdfFk.py`

 * *Files identical despite different names*

### Comparing `forwardkinematics-1.2.1/forwardkinematics/xmlFks/generic_xml_fk.py` & `forwardkinematics-1.2.2/forwardkinematics/xmlFks/generic_xml_fk.py`

 * *Files identical despite different names*

### Comparing `forwardkinematics-1.2.1/pyproject.toml` & `forwardkinematics-1.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "forwardkinematics"
-version = "1.2.1"
+version = "1.2.2"
 description = "\"Light-weight implementation of forward kinematics using casadi.\""
 authors = ["Max Spahn <m.spahn@tudelft.nl>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/maxspahn/forwardKinematics.git"
 repository = "https://github.com/maxspahn/forwardKinematics.git"
```

### Comparing `forwardkinematics-1.2.1/PKG-INFO` & `forwardkinematics-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forwardkinematics
-Version: 1.2.1
+Version: 1.2.2
 Summary: "Light-weight implementation of forward kinematics using casadi."
 Home-page: https://github.com/maxspahn/forwardKinematics.git
 License: MIT
 Author: Max Spahn
 Author-email: m.spahn@tudelft.nl
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

