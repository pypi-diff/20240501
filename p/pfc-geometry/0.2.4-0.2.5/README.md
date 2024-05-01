# Comparing `tmp/pfc_geometry-0.2.4.tar.gz` & `tmp/pfc_geometry-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pfc_geometry-0.2.4.tar", last modified: Thu Apr 18 11:54:31 2024, max compression
+gzip compressed data, was "pfc_geometry-0.2.5.tar", last modified: Wed May  1 08:46:13 2024, max compression
```

## Comparing `pfc_geometry-0.2.4.tar` & `pfc_geometry-0.2.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:54:31.663937 pfc_geometry-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)     7632 2024-04-18 11:54:11.000000 pfc_geometry-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-18 11:54:31.663937 pfc_geometry-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-18 11:54:11.000000 pfc_geometry-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:54:31.663937 pfc_geometry-0.2.4/geometry/
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-18 11:54:11.000000 pfc_geometry-0.2.4/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11277 2024-04-18 11:54:11.000000 pfc_geometry-0.2.4/geometry/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-04-18 11:54:11.000000 pfc_geometry-0.2.4/geometry/coordinate_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-04-18 11:54:11.000000 pfc_geometry-0.2.4/geometry/gps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-18 11:54:11.000000 pfc_geometry-0.2.4/geometry/mass.py
--rw-r--r--   0 runner    (1001) docker     (127)     5025 2024-04-18 11:54:11.000000 pfc_geometry-0.2.4/geometry/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     9367 2024-04-18 11:54:11.000000 pfc_geometry-0.2.4/geometry/quaternion.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-18 11:54:11.000000 pfc_geometry-0.2.4/geometry/testing.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-18 11:54:11.000000 pfc_geometry-0.2.4/geometry/time.py
--rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-04-18 11:54:11.000000 pfc_geometry-0.2.4/geometry/transformation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:54:31.663937 pfc_geometry-0.2.4/pfc_geometry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-18 11:54:31.000000 pfc_geometry-0.2.4/pfc_geometry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-18 11:54:31.000000 pfc_geometry-0.2.4/pfc_geometry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 11:54:31.000000 pfc_geometry-0.2.4/pfc_geometry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-18 11:54:31.000000 pfc_geometry-0.2.4/pfc_geometry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-18 11:54:31.000000 pfc_geometry-0.2.4/pfc_geometry.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-18 11:54:31.663937 pfc_geometry-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-18 11:54:11.000000 pfc_geometry-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:54:31.663937 pfc_geometry-0.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-04-18 11:54:11.000000 pfc_geometry-0.2.4/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-18 11:54:11.000000 pfc_geometry-0.2.4/tests/test_coord.py
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-18 11:54:11.000000 pfc_geometry-0.2.4/tests/test_gps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-18 11:54:11.000000 pfc_geometry-0.2.4/tests/test_mass.py
--rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-04-18 11:54:11.000000 pfc_geometry-0.2.4/tests/test_point.py
--rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-04-18 11:54:11.000000 pfc_geometry-0.2.4/tests/test_quaternion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-18 11:54:11.000000 pfc_geometry-0.2.4/tests/test_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:46:13.280727 pfc_geometry-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     7632 2024-05-01 08:45:58.000000 pfc_geometry-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-01 08:46:13.280727 pfc_geometry-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-01 08:45:58.000000 pfc_geometry-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:46:13.276727 pfc_geometry-0.2.5/geometry/
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-01 08:45:58.000000 pfc_geometry-0.2.5/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11277 2024-05-01 08:45:58.000000 pfc_geometry-0.2.5/geometry/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-05-01 08:45:58.000000 pfc_geometry-0.2.5/geometry/coordinate_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-05-01 08:45:58.000000 pfc_geometry-0.2.5/geometry/gps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-05-01 08:45:58.000000 pfc_geometry-0.2.5/geometry/mass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5031 2024-05-01 08:45:58.000000 pfc_geometry-0.2.5/geometry/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9367 2024-05-01 08:45:58.000000 pfc_geometry-0.2.5/geometry/quaternion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-01 08:45:58.000000 pfc_geometry-0.2.5/geometry/testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-01 08:45:58.000000 pfc_geometry-0.2.5/geometry/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-05-01 08:45:58.000000 pfc_geometry-0.2.5/geometry/transformation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:46:13.280727 pfc_geometry-0.2.5/pfc_geometry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-01 08:46:13.000000 pfc_geometry-0.2.5/pfc_geometry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-01 08:46:13.000000 pfc_geometry-0.2.5/pfc_geometry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 08:46:13.000000 pfc_geometry-0.2.5/pfc_geometry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-01 08:46:13.000000 pfc_geometry-0.2.5/pfc_geometry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-01 08:46:13.000000 pfc_geometry-0.2.5/pfc_geometry.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-01 08:46:13.280727 pfc_geometry-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-01 08:45:58.000000 pfc_geometry-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:46:13.280727 pfc_geometry-0.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-05-01 08:45:58.000000 pfc_geometry-0.2.5/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-01 08:45:58.000000 pfc_geometry-0.2.5/tests/test_coord.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-01 08:45:58.000000 pfc_geometry-0.2.5/tests/test_gps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-01 08:45:58.000000 pfc_geometry-0.2.5/tests/test_mass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-05-01 08:45:58.000000 pfc_geometry-0.2.5/tests/test_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-01 08:45:58.000000 pfc_geometry-0.2.5/tests/test_quaternion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-01 08:45:58.000000 pfc_geometry-0.2.5/tests/test_transform.py
```

### Comparing `pfc_geometry-0.2.4/LICENSE` & `pfc_geometry-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.2.4/PKG-INFO` & `pfc_geometry-0.2.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: pfc_geometry
-Version: 0.2.4
+Version: 0.2.5
 Summary: A package for handling 3D geometry with a nice interface
 Home-page: https://github.com/PyFlightCoach/geometry
 Author: Thomas David
 Author-email: thomasdavid0@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: setuptools
 Requires-Dist: numpy
 Requires-Dist: pandas
 
 # geometry #
 
 Tools for handling 3D geometry, mostly just adds a nice interface to various geometric enterties. Each geometric entity can also be a vector of geometric entities. Each entity wraps a numpy array with the relevant number of columns labelled according to the cols class property and rows equal to the number of elements in the vector. Attribute access to each column is available and returns a numpy array.
```

### Comparing `pfc_geometry-0.2.4/README.md` & `pfc_geometry-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.2.4/geometry/__init__.py` & `pfc_geometry-0.2.5/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.2.4/geometry/base.py` & `pfc_geometry-0.2.5/geometry/base.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.2.4/geometry/coordinate_frame.py` & `pfc_geometry-0.2.5/geometry/coordinate_frame.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.2.4/geometry/gps.py` & `pfc_geometry-0.2.5/geometry/gps.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.2.4/geometry/mass.py` & `pfc_geometry-0.2.5/geometry/mass.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.2.4/geometry/point.py` & `pfc_geometry-0.2.5/geometry/point.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 You should have received a copy of the GNU General Public License along with
 this program. If not, see <http://www.gnu.org/licenses/>.
 """
 from __future__ import annotations
 from .base import Base
 import numpy as np
 import pandas as pd
-from typing import List 
 from warnings import warn
 
 
 class Point(Base):
     cols=["x", "y", "z"]
     from_np = [
         "sin","cos","tan",
@@ -52,14 +51,17 @@
     
     def min(self):
         return Point(np.min(self.data, axis=0))
 
     def angles(self, p2):
         return (self.cross(p2) / (abs(self) * abs(p2))).arcsin
     
+    def planar_angles(self):
+        return Point(np.arctan2(self.y, self.z), np.arctan2(self.z, self.x), np.arctan2(self.x, self.y))
+
     def angle(self, p2):
         return abs(Point.angles(self, p2))
     
     @staticmethod
     def X(value=1, count=1):
         return Point(np.tile([value,0,0], (count, 1)))
 
@@ -168,18 +170,14 @@
     return abs(a.dot(b)) < tolerance
 
 @ppmeth
 def min_angle_between(p1: Point, p2: Point):
     angle = angle_between(p1, p2) % np.pi
     return min(angle, np.pi - angle)
 
-@ppmeth
-def angle_between(a: Point, b: Point) -> float: 
-    return np.arccos(cos_angle_between(a, b))
-
 def arbitrary_perpendicular(v: Point) -> Point:
     return Point(-v.y, v.x, 0).unit()
 
 def vector_norm(point: Point):
     return abs(point)
 
 def normalize_vector(point: Point):
```

### Comparing `pfc_geometry-0.2.4/geometry/quaternion.py` & `pfc_geometry-0.2.5/geometry/quaternion.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.2.4/geometry/time.py` & `pfc_geometry-0.2.5/geometry/time.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.2.4/geometry/transformation.py` & `pfc_geometry-0.2.5/geometry/transformation.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.2.4/pfc_geometry.egg-info/PKG-INFO` & `pfc_geometry-0.2.5/pfc_geometry.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: pfc_geometry
-Version: 0.2.4
+Version: 0.2.5
 Summary: A package for handling 3D geometry with a nice interface
 Home-page: https://github.com/PyFlightCoach/geometry
 Author: Thomas David
 Author-email: thomasdavid0@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: setuptools
 Requires-Dist: numpy
 Requires-Dist: pandas
 
 # geometry #
 
 Tools for handling 3D geometry, mostly just adds a nice interface to various geometric enterties. Each geometric entity can also be a vector of geometric entities. Each entity wraps a numpy array with the relevant number of columns labelled according to the cols class property and rows equal to the number of elements in the vector. Attribute access to each column is available and returns a numpy array.
```

### Comparing `pfc_geometry-0.2.4/pfc_geometry.egg-info/SOURCES.txt` & `pfc_geometry-0.2.5/pfc_geometry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.2.4/setup.py` & `pfc_geometry-0.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.2.4/tests/test_base.py` & `pfc_geometry-0.2.5/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.2.4/tests/test_coord.py` & `pfc_geometry-0.2.5/tests/test_coord.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.2.4/tests/test_gps.py` & `pfc_geometry-0.2.5/tests/test_gps.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.2.4/tests/test_mass.py` & `pfc_geometry-0.2.5/tests/test_mass.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.2.4/tests/test_point.py` & `pfc_geometry-0.2.5/tests/test_point.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.2.4/tests/test_quaternion.py` & `pfc_geometry-0.2.5/tests/test_quaternion.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.2.4/tests/test_transform.py` & `pfc_geometry-0.2.5/tests/test_transform.py`

 * *Files identical despite different names*

