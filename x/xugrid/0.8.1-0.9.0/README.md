# Comparing `tmp/xugrid-0.8.1.tar.gz` & `tmp/xugrid-0.9.0.tar.gz`

## Comparing `xugrid-0.8.1.tar` & `xugrid-0.9.0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 xugrid-0.8.1/tests/__init__.py
--rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 xugrid-0.8.1/tests/conftest.py
--rw-r--r--   0        0        0     8417 2020-02-02 00:00:00.000000 xugrid-0.8.1/tests/test_burn.py
--rw-r--r--   0        0        0    21941 2020-02-02 00:00:00.000000 xugrid-0.8.1/tests/test_connectivity.py
--rw-r--r--   0        0        0    11185 2020-02-02 00:00:00.000000 xugrid-0.8.1/tests/test_conventions.py
--rw-r--r--   0        0        0     9032 2020-02-02 00:00:00.000000 xugrid-0.8.1/tests/test_conversion.py
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 xugrid-0.8.1/tests/test_core_utils.py
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 xugrid-0.8.1/tests/test_data.py
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 xugrid-0.8.1/tests/test_interpolate.py
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 xugrid-0.8.1/tests/test_meshkernel_utils.py
--rw-r--r--   0        0        0     8494 2020-02-02 00:00:00.000000 xugrid-0.8.1/tests/test_partitioning.py
--rw-r--r--   0        0        0     9084 2020-02-02 00:00:00.000000 xugrid-0.8.1/tests/test_plot.py
--rw-r--r--   0        0        0    14583 2020-02-02 00:00:00.000000 xugrid-0.8.1/tests/test_plot_utils.py
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 xugrid-0.8.1/tests/test_polygonize.py
--rw-r--r--   0        0        0     5362 2020-02-02 00:00:00.000000 xugrid-0.8.1/tests/test_snap.py
--rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 xugrid-0.8.1/tests/test_sparse.py
--rw-r--r--   0        0        0    13398 2020-02-02 00:00:00.000000 xugrid-0.8.1/tests/test_ugrid1d.py
--rw-r--r--   0        0        0    42413 2020-02-02 00:00:00.000000 xugrid-0.8.1/tests/test_ugrid2d.py
--rw-r--r--   0        0        0    43391 2020-02-02 00:00:00.000000 xugrid-0.8.1/tests/test_ugrid_dataset.py
--rw-r--r--   0        0        0    10444 2020-02-02 00:00:00.000000 xugrid-0.8.1/tests/test_voronoi.py
--rw-r--r--   0        0        0    11748 2020-02-02 00:00:00.000000 xugrid-0.8.1/tests/fixtures/fixture_regridder.py
--rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 xugrid-0.8.1/tests/test_regrid/test_overlap_1d.py
--rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 xugrid-0.8.1/tests/test_regrid/test_reduce.py
--rw-r--r--   0        0        0     7629 2020-02-02 00:00:00.000000 xugrid-0.8.1/tests/test_regrid/test_regridder.py
--rw-r--r--   0        0        0    12952 2020-02-02 00:00:00.000000 xugrid-0.8.1/tests/test_regrid/test_structured.py
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 xugrid-0.8.1/tests/test_regrid/test_unstructured.py
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 xugrid-0.8.1/tests/test_regrid/test_utils.py
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 xugrid-0.8.1/xugrid/__init__.py
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 xugrid-0.8.1/xugrid/constants.py
--rw-r--r--   0        0        0     8411 2020-02-02 00:00:00.000000 xugrid-0.8.1/xugrid/conversion.py
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 xugrid-0.8.1/xugrid/meshkernel_utils.py
--rw-r--r--   0        0        0     4317 2020-02-02 00:00:00.000000 xugrid-0.8.1/xugrid/core/accessorbase.py
--rw-r--r--   0        0        0     3550 2020-02-02 00:00:00.000000 xugrid-0.8.1/xugrid/core/common.py
--rw-r--r--   0        0        0    22948 2020-02-02 00:00:00.000000 xugrid-0.8.1/xugrid/core/dataarray_accessor.py
--rw-r--r--   0        0        0    21552 2020-02-02 00:00:00.000000 xugrid-0.8.1/xugrid/core/dataset_accessor.py
--rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 xugrid-0.8.1/xugrid/core/sparse.py
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 xugrid-0.8.1/xugrid/core/utils.py
--rw-r--r--   0        0        0    11809 2020-02-02 00:00:00.000000 xugrid-0.8.1/xugrid/core/wrap.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 xugrid-0.8.1/xugrid/data/__init__.py
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 xugrid-0.8.1/xugrid/data/registry.txt
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 xugrid-0.8.1/xugrid/data/sample_data.py
--rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 xugrid-0.8.1/xugrid/data/synthetic.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 xugrid-0.8.1/xugrid/plot/__init__.py
--rw-r--r--   0        0        0    24118 2020-02-02 00:00:00.000000 xugrid-0.8.1/xugrid/plot/plot.py
--rw-r--r--   0        0        0    22098 2020-02-02 00:00:00.000000 xugrid-0.8.1/xugrid/plot/utils.py
--rw-r--r--   0        0        0     7738 2020-02-02 00:00:00.000000 xugrid-0.8.1/xugrid/regrid/overlap_1d.py
--rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 xugrid-0.8.1/xugrid/regrid/reduce.py
--rw-r--r--   0        0        0    19466 2020-02-02 00:00:00.000000 xugrid-0.8.1/xugrid/regrid/regridder.py
--rw-r--r--   0        0        0    24782 2020-02-02 00:00:00.000000 xugrid-0.8.1/xugrid/regrid/structured.py
--rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 xugrid-0.8.1/xugrid/regrid/unstructured.py
--rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 xugrid-0.8.1/xugrid/regrid/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xugrid-0.8.1/xugrid/ugrid/__init__.py
--rw-r--r--   0        0        0    10283 2020-02-02 00:00:00.000000 xugrid-0.8.1/xugrid/ugrid/burn.py
--rw-r--r--   0        0        0    28379 2020-02-02 00:00:00.000000 xugrid-0.8.1/xugrid/ugrid/connectivity.py
--rw-r--r--   0        0        0    15249 2020-02-02 00:00:00.000000 xugrid-0.8.1/xugrid/ugrid/conventions.py
--rw-r--r--   0        0        0     9917 2020-02-02 00:00:00.000000 xugrid-0.8.1/xugrid/ugrid/interpolate.py
--rw-r--r--   0        0        0    11073 2020-02-02 00:00:00.000000 xugrid-0.8.1/xugrid/ugrid/partitioning.py
--rw-r--r--   0        0        0     4960 2020-02-02 00:00:00.000000 xugrid-0.8.1/xugrid/ugrid/polygonize.py
--rw-r--r--   0        0        0    15482 2020-02-02 00:00:00.000000 xugrid-0.8.1/xugrid/ugrid/snapping.py
--rw-r--r--   0        0        0    23182 2020-02-02 00:00:00.000000 xugrid-0.8.1/xugrid/ugrid/ugrid1d.py
--rw-r--r--   0        0        0    73125 2020-02-02 00:00:00.000000 xugrid-0.8.1/xugrid/ugrid/ugrid2d.py
--rw-r--r--   0        0        0    24273 2020-02-02 00:00:00.000000 xugrid-0.8.1/xugrid/ugrid/ugridbase.py
--rw-r--r--   0        0        0    14185 2020-02-02 00:00:00.000000 xugrid-0.8.1/xugrid/ugrid/voronoi.py
--rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 xugrid-0.8.1/.gitignore
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 xugrid-0.8.1/LICENSE
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 xugrid-0.8.1/README.rst
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 xugrid-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 xugrid-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 xugrid-0.9.0/tests/__init__.py
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 xugrid-0.9.0/tests/conftest.py
+-rw-r--r--   0        0        0     8417 2020-02-02 00:00:00.000000 xugrid-0.9.0/tests/test_burn.py
+-rw-r--r--   0        0        0    21941 2020-02-02 00:00:00.000000 xugrid-0.9.0/tests/test_connectivity.py
+-rw-r--r--   0        0        0    11185 2020-02-02 00:00:00.000000 xugrid-0.9.0/tests/test_conventions.py
+-rw-r--r--   0        0        0    10733 2020-02-02 00:00:00.000000 xugrid-0.9.0/tests/test_conversion.py
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 xugrid-0.9.0/tests/test_core_utils.py
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 xugrid-0.9.0/tests/test_data.py
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 xugrid-0.9.0/tests/test_interpolate.py
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 xugrid-0.9.0/tests/test_meshkernel_utils.py
+-rw-r--r--   0        0        0    14091 2020-02-02 00:00:00.000000 xugrid-0.9.0/tests/test_partitioning.py
+-rw-r--r--   0        0        0     9084 2020-02-02 00:00:00.000000 xugrid-0.9.0/tests/test_plot.py
+-rw-r--r--   0        0        0    14583 2020-02-02 00:00:00.000000 xugrid-0.9.0/tests/test_plot_utils.py
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 xugrid-0.9.0/tests/test_polygonize.py
+-rw-r--r--   0        0        0     5362 2020-02-02 00:00:00.000000 xugrid-0.9.0/tests/test_snap.py
+-rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 xugrid-0.9.0/tests/test_sparse.py
+-rw-r--r--   0        0        0    13743 2020-02-02 00:00:00.000000 xugrid-0.9.0/tests/test_ugrid1d.py
+-rw-r--r--   0        0        0    45700 2020-02-02 00:00:00.000000 xugrid-0.9.0/tests/test_ugrid2d.py
+-rw-r--r--   0        0        0    45189 2020-02-02 00:00:00.000000 xugrid-0.9.0/tests/test_ugrid_dataset.py
+-rw-r--r--   0        0        0    10444 2020-02-02 00:00:00.000000 xugrid-0.9.0/tests/test_voronoi.py
+-rw-r--r--   0        0        0    11748 2020-02-02 00:00:00.000000 xugrid-0.9.0/tests/fixtures/fixture_regridder.py
+-rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 xugrid-0.9.0/tests/test_regrid/test_overlap_1d.py
+-rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 xugrid-0.9.0/tests/test_regrid/test_reduce.py
+-rw-r--r--   0        0        0     7629 2020-02-02 00:00:00.000000 xugrid-0.9.0/tests/test_regrid/test_regridder.py
+-rw-r--r--   0        0        0    12952 2020-02-02 00:00:00.000000 xugrid-0.9.0/tests/test_regrid/test_structured.py
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 xugrid-0.9.0/tests/test_regrid/test_unstructured.py
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 xugrid-0.9.0/tests/test_regrid/test_utils.py
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 xugrid-0.9.0/xugrid/__init__.py
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 xugrid-0.9.0/xugrid/constants.py
+-rw-r--r--   0        0        0    10492 2020-02-02 00:00:00.000000 xugrid-0.9.0/xugrid/conversion.py
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 xugrid-0.9.0/xugrid/meshkernel_utils.py
+-rw-r--r--   0        0        0     4317 2020-02-02 00:00:00.000000 xugrid-0.9.0/xugrid/core/accessorbase.py
+-rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 xugrid-0.9.0/xugrid/core/common.py
+-rw-r--r--   0        0        0    22948 2020-02-02 00:00:00.000000 xugrid-0.9.0/xugrid/core/dataarray_accessor.py
+-rw-r--r--   0        0        0    21552 2020-02-02 00:00:00.000000 xugrid-0.9.0/xugrid/core/dataset_accessor.py
+-rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 xugrid-0.9.0/xugrid/core/sparse.py
+-rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 xugrid-0.9.0/xugrid/core/utils.py
+-rw-r--r--   0        0        0    12927 2020-02-02 00:00:00.000000 xugrid-0.9.0/xugrid/core/wrap.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 xugrid-0.9.0/xugrid/data/__init__.py
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 xugrid-0.9.0/xugrid/data/registry.txt
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 xugrid-0.9.0/xugrid/data/sample_data.py
+-rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 xugrid-0.9.0/xugrid/data/synthetic.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 xugrid-0.9.0/xugrid/plot/__init__.py
+-rw-r--r--   0        0        0    24105 2020-02-02 00:00:00.000000 xugrid-0.9.0/xugrid/plot/plot.py
+-rw-r--r--   0        0        0    22098 2020-02-02 00:00:00.000000 xugrid-0.9.0/xugrid/plot/utils.py
+-rw-r--r--   0        0        0     7738 2020-02-02 00:00:00.000000 xugrid-0.9.0/xugrid/regrid/overlap_1d.py
+-rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 xugrid-0.9.0/xugrid/regrid/reduce.py
+-rw-r--r--   0        0        0    19466 2020-02-02 00:00:00.000000 xugrid-0.9.0/xugrid/regrid/regridder.py
+-rw-r--r--   0        0        0    24782 2020-02-02 00:00:00.000000 xugrid-0.9.0/xugrid/regrid/structured.py
+-rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 xugrid-0.9.0/xugrid/regrid/unstructured.py
+-rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 xugrid-0.9.0/xugrid/regrid/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xugrid-0.9.0/xugrid/ugrid/__init__.py
+-rw-r--r--   0        0        0    10358 2020-02-02 00:00:00.000000 xugrid-0.9.0/xugrid/ugrid/burn.py
+-rw-r--r--   0        0        0    28379 2020-02-02 00:00:00.000000 xugrid-0.9.0/xugrid/ugrid/connectivity.py
+-rw-r--r--   0        0        0    15250 2020-02-02 00:00:00.000000 xugrid-0.9.0/xugrid/ugrid/conventions.py
+-rw-r--r--   0        0        0     9917 2020-02-02 00:00:00.000000 xugrid-0.9.0/xugrid/ugrid/interpolate.py
+-rw-r--r--   0        0        0    13382 2020-02-02 00:00:00.000000 xugrid-0.9.0/xugrid/ugrid/partitioning.py
+-rw-r--r--   0        0        0     4960 2020-02-02 00:00:00.000000 xugrid-0.9.0/xugrid/ugrid/polygonize.py
+-rw-r--r--   0        0        0    15482 2020-02-02 00:00:00.000000 xugrid-0.9.0/xugrid/ugrid/snapping.py
+-rw-r--r--   0        0        0    23262 2020-02-02 00:00:00.000000 xugrid-0.9.0/xugrid/ugrid/ugrid1d.py
+-rw-r--r--   0        0        0    78071 2020-02-02 00:00:00.000000 xugrid-0.9.0/xugrid/ugrid/ugrid2d.py
+-rw-r--r--   0        0        0    24778 2020-02-02 00:00:00.000000 xugrid-0.9.0/xugrid/ugrid/ugridbase.py
+-rw-r--r--   0        0        0    14185 2020-02-02 00:00:00.000000 xugrid-0.9.0/xugrid/ugrid/voronoi.py
+-rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 xugrid-0.9.0/.gitignore
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 xugrid-0.9.0/LICENSE
+-rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 xugrid-0.9.0/README.rst
+-rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 xugrid-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     3535 2020-02-02 00:00:00.000000 xugrid-0.9.0/PKG-INFO
```

### Comparing `xugrid-0.8.1/tests/__init__.py` & `xugrid-0.9.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.8.1/tests/conftest.py` & `xugrid-0.9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.8.1/tests/test_burn.py` & `xugrid-0.9.0/tests/test_burn.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.8.1/tests/test_connectivity.py` & `xugrid-0.9.0/tests/test_connectivity.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.8.1/tests/test_conventions.py` & `xugrid-0.9.0/tests/test_conventions.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.8.1/tests/test_conversion.py` & `xugrid-0.9.0/tests/test_conversion.py`

 * *Files 9% similar despite different names*

```diff
@@ -126,14 +126,64 @@
     _faces_geos_roundtrip(triangle_mesh)
 
 
 def test_faces_geos_roundtrip__mixed(mixed_mesh):
     _faces_geos_roundtrip(mixed_mesh)
 
 
+def test_is_monotonic_and_increasing():
+    with pytest.raises(ValueError):
+        cv._is_monotonic_and_increasing([0.0, -1.0, 2.0])
+    with pytest.raises(ValueError):
+        cv._is_monotonic_and_increasing([2.0, 0.0, 1.0])
+
+    assert cv._is_monotonic_and_increasing([0.0, 1.0, 2.0])
+    assert not cv._is_monotonic_and_increasing([2.0, 1.0, 0.0])
+
+    ascending = np.array(
+        [
+            [0.0, 1.0, 2.0],
+            [3.0, 4.0, 5.0],
+            [6.0, 7.0, 8.0],
+        ]
+    )
+    descending = np.array(
+        [
+            [8.0, 7.0, 6.0],
+            [5.0, 4.0, 3.0],
+            [2.0, 1.0, 0.0],
+        ]
+    )
+    assert cv._is_monotonic_and_increasing(ascending, axis=0)
+    assert cv._is_monotonic_and_increasing(ascending, axis=1)
+    assert not cv._is_monotonic_and_increasing(descending, axis=1)
+    assert not cv._is_monotonic_and_increasing(descending, axis=1)
+
+
+def test_infer_interval_breaks():
+    assert np.allclose([-0.5, 0.5, 1.5], cv.infer_interval_breaks([0, 1]))
+    assert np.allclose(
+        [-0.5, 0.5, 5.0, 9.5, 10.5], cv.infer_interval_breaks([0, 1, 9, 10])
+    )
+
+    xref, yref = np.meshgrid(np.arange(6), np.arange(5))
+    cx = (xref[1:, 1:] + xref[:-1, :-1]) / 2
+    cy = (yref[1:, 1:] + yref[:-1, :-1]) / 2
+    x = cv.infer_interval_breaks(cx, axis=1)
+    x = cv.infer_interval_breaks(x, axis=0)
+    y = cv.infer_interval_breaks(cy, axis=1)
+    y = cv.infer_interval_breaks(y, axis=0)
+    np.testing.assert_allclose(xref, x)
+    np.testing.assert_allclose(yref, y)
+
+    # test that ValueError is raised for non-monotonic 1D inputs
+    with pytest.raises(ValueError):
+        cv.infer_interval_breaks(np.array([0, 2, 1]), check_monotonic=True)
+
+
 def test_scalar_spacing(structured_mesh_ascending, structured_mesh_descending):
     upcoords = structured_mesh_ascending.coords["x"]
     downcoords = structured_mesh_descending.coords["x"]
     spacing = xr.DataArray(0.1, name="dx")
     with pytest.raises(ValueError, match="spacing of x does not match value of dx"):
         cv._scalar_spacing(upcoords, spacing)
 
@@ -159,87 +209,78 @@
 def test_implicit_spacing(structured_mesh_ascending, structured_mesh_descending):
     da = xr.DataArray(
         [[0.0, 0.0]],
         {"y": [0.0], "x": [1.0, 2.0]},
         ["y", "x"],
     )
     with pytest.raises(ValueError, match="Cannot derive spacing of 1-sized coordinate"):
-        cv._implicit_spacing(da.coords["y"])
+        cv.infer_interval_breaks1d(da, "y")
 
-    upcoords = structured_mesh_ascending.coords["x"]
-    downcoords = structured_mesh_descending.coords["x"]
-    assert np.allclose(cv._implicit_spacing(upcoords), 1.0)
-    assert np.allclose(cv._implicit_spacing(downcoords), 1.0)
+    actual = cv.infer_interval_breaks1d(structured_mesh_ascending, "x")
+    assert np.allclose(actual, [1.0, 3.0, 5.0, 7.0, 9.0])
+    actual = cv.infer_interval_breaks1d(structured_mesh_descending, "x")
+    assert np.allclose(actual, [9.0, 7.0, 5.0, 3.0, 1.0])
 
 
 @pytest.mark.parametrize("spacing_type", ["implicit", "scalar", "array"])
-def test_infer_bounds(
+def test_infer_breaks_intervals1d(
     structured_mesh_ascending, structured_mesh_descending, spacing_type
 ):
     up = structured_mesh_ascending
     down = structured_mesh_descending
     x_expected = np.array(
-        [
-            [1.0, 3.0],
-            [3.0, 5.0],
-            [5.0, 7.0],
-            [7.0, 9.0],
-        ]
+        [1.0, 3.0, 5.0, 7.0, 9.0],
     )
     y_expected = np.array(
-        [
-            [2.5, 7.5],
-            [7.5, 12.5],
-            [12.5, 17.5],
-        ]
+        [2.5, 7.5, 12.5, 17.5],
     )
 
     if spacing_type == "scalar":
         up = up.assign_coords({"dx": 2.0, "dy": 5.0})
         down = down.assign_coords({"dx": 2.0, "dy": 5.0})
     elif spacing_type == "array":
         up = up.assign_coords({"dx": ("x", [2.0] * 4), "dy": ("y", [5.0] * 3)})
         down = down.assign_coords({"dx": ("x", [2.0] * 4), "dy": ("y", [5.0] * 3)})
 
-    assert np.allclose(cv.infer_bounds(up, "x"), x_expected)
-    assert np.allclose(cv.infer_bounds(up, "y"), y_expected)
-    assert np.allclose(cv.infer_bounds(down, "x"), x_expected[::-1])
-    assert np.allclose(cv.infer_bounds(down, "y"), y_expected[::-1])
+    assert np.allclose(cv.infer_interval_breaks1d(up, "x"), x_expected)
+    assert np.allclose(cv.infer_interval_breaks1d(up, "y"), y_expected)
+    assert np.allclose(cv.infer_interval_breaks1d(down, "x"), x_expected[::-1])
+    assert np.allclose(cv.infer_interval_breaks1d(down, "y"), y_expected[::-1])
 
 
-def test_infer_bounds_errors(structured_mesh_ascending):
+def test_infer_breaks_intervals1d_errors(structured_mesh_ascending):
     up = structured_mesh_ascending
     up = up.assign_coords(x=[2.0, 4.0, 3.0, 8.0])
 
-    with pytest.raises(ValueError, match="x is not monotonic"):
-        cv.infer_bounds(up, "x")
+    with pytest.raises(ValueError, match="The input coordinate is not monotonic."):
+        cv.infer_interval_breaks1d(up, "x")
 
 
-def test_bounds_to_vertices(structured_mesh_ascending, structured_mesh_descending):
+def test_bounds_to_vertices():
     with pytest.raises(ValueError, match="Bounds are not monotonic"):
         cv.bounds_to_vertices(
             xr.DataArray(
                 data=[[0.0, 1.0], [2.0, 3.0], [1.0, 2.0]], dims=["x", "nbound"]
             )
         )
 
-    up = structured_mesh_ascending
-    down = structured_mesh_descending
     x_vertices = np.array([1.0, 3.0, 5.0, 7.0, 9.0])
     y_vertices = np.array([2.5, 7.5, 12.5, 17.5])
     # Ascending
-    x_bounds = cv.infer_bounds(up, "x")
-    y_bounds = cv.infer_bounds(up, "y")
+    x_bounds = np.column_stack((x_vertices[:-1], x_vertices[1:]))
+    y_bounds = np.column_stack((y_vertices[:-1], y_vertices[1:]))
     assert np.allclose(cv.bounds_to_vertices(x_bounds), x_vertices)
     assert np.allclose(cv.bounds_to_vertices(y_bounds), y_vertices)
     # Descending
-    x_bounds = cv.infer_bounds(down, "x")
-    y_bounds = cv.infer_bounds(down, "y")
-    assert np.allclose(cv.bounds_to_vertices(x_bounds), x_vertices[::-1])
-    assert np.allclose(cv.bounds_to_vertices(y_bounds), y_vertices[::-1])
+    xrev = x_vertices[::-1]
+    yrev = y_vertices[::-1]
+    x_bounds = np.column_stack((xrev[1:], xrev[:-1]))
+    y_bounds = np.column_stack((yrev[1:], yrev[:-1]))
+    assert np.allclose(cv.bounds_to_vertices(x_bounds), xrev)
+    assert np.allclose(cv.bounds_to_vertices(y_bounds), yrev)
 
 
 def test_infer_xy_coords():
     da = xr.DataArray(
         data=[[1]],
         coords={"y": [1], "x": [1]},
         dims=["y", "x"],
```

### Comparing `xugrid-0.8.1/tests/test_data.py` & `xugrid-0.9.0/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.8.1/tests/test_interpolate.py` & `xugrid-0.9.0/tests/test_interpolate.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.8.1/tests/test_meshkernel_utils.py` & `xugrid-0.9.0/tests/test_meshkernel_utils.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.8.1/tests/test_plot.py` & `xugrid-0.9.0/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.8.1/tests/test_plot_utils.py` & `xugrid-0.9.0/tests/test_plot_utils.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.8.1/tests/test_polygonize.py` & `xugrid-0.9.0/tests/test_polygonize.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.8.1/tests/test_snap.py` & `xugrid-0.9.0/tests/test_snap.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.8.1/tests/test_sparse.py` & `xugrid-0.9.0/tests/test_sparse.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.8.1/tests/test_ugrid1d.py` & `xugrid-0.9.0/tests/test_ugrid1d.py`

 * *Files 1% similar despite different names*

```diff
@@ -439,7 +439,19 @@
     with pytest.raises(ValueError, match="Expected network1d_nNodes; got: abc"):
         grid.connectivity_matrix(dim="abc", xy_weights=True)
 
     connectivity = grid.connectivity_matrix(grid.node_dimension, True)
     assert isinstance(connectivity, sparse.csr_matrix)
     assert np.allclose(connectivity.data, [1.5, 1.5, 0.75, 0.75])
     assert np.array_equal(connectivity.indices, [1, 0, 2, 1])
+
+
+def test_equals():
+    grid = grid1d()
+    grid_copy = grid1d()
+    assert grid.equals(grid)
+    assert grid.equals(grid_copy)
+    xr_grid = grid.to_dataset()
+    assert not grid.equals(xr_grid)
+    grid_copy.attrs["attr"] = "something_else"
+    # Dataset.identical is called so returns False
+    assert not grid.equals(grid_copy)
```

### Comparing `xugrid-0.8.1/tests/test_ugrid2d.py` & `xugrid-0.9.0/tests/test_ugrid2d.py`

 * *Files 6% similar despite different names*

```diff
@@ -287,14 +287,27 @@
     grid = grid2d()
     ds = grid.to_dataset()
     grid2 = xugrid.Ugrid2d.from_dataset(ds)
     assert isinstance(grid2._dataset, xr.Dataset)
     assert grid2._dataset == ds
 
 
+def test_ugrid2d_dataset_no_mutation():
+    grid = grid2d()
+    ds = grid.to_dataset()
+    # Test a non-default fill value
+    face_nodes = ds["mesh2d_face_nodes"]
+    face_nodes = face_nodes.where(face_nodes != -1, other=-999)
+    face_nodes.attrs["_FillValue"] = -999
+    ds["mesh2d_face_nodes"] = face_nodes
+    reference = ds.copy(deep=True)
+    xugrid.Ugrid2d.from_dataset(ds)
+    assert ds.identical(reference)
+
+
 def test_ugrid2d_from_meshkernel():
     # Setup a meshkernel Mesh2d mimick
     class Mesh2d(NamedTuple):
         node_x: np.ndarray
         node_y: np.ndarray
         face_nodes: np.ndarray
         nodes_per_face: np.ndarray
@@ -975,14 +988,92 @@
 
 @requires_meshkernel
 def test_meshkernel():
     grid = grid2d()
     assert isinstance(grid.meshkernel, mk.MeshKernel)
 
 
+def test_from_structured_intervals1d():
+    grid = xugrid.Ugrid2d.from_structured_intervals1d(
+        x_intervals=[0.0, 1.0, 2.0],
+        y_intervals=[2.0, 1.0, 0.0],
+    )
+    assert isinstance(grid, xugrid.Ugrid2d)
+    assert grid.n_face == 4
+
+
+def test_from_structured_intervals2d():
+    with pytest.raises(ValueError, match="Dimensions of intervals must be 2D."):
+        xugrid.Ugrid2d.from_structured_intervals2d(
+            x_intervals=[0.0, 1.0, 2.0],
+            y_intervals=[2.0, 1.0, 0.0],
+        )
+    with pytest.raises(ValueError, match="Interval shapes must match."):
+        xugrid.Ugrid2d.from_structured_intervals2d(
+            x_intervals=[[0.0, 1.0, 2.0]],
+            y_intervals=[[2.0, 1.0, 0.0, 4.0]],
+        )
+
+    grid = xugrid.Ugrid2d.from_structured_intervals2d(
+        x_intervals=[[0.0, 1.0, 2.0], [0.0, 1.0, 2.0], [0.0, 1.0, 2.0]],
+        y_intervals=[
+            [2.0, 1.0, 0.0],
+            [2.0, 1.0, 0.0],
+            [2.0, 1.0, 0.0],
+        ],
+    )
+    assert isinstance(grid, xugrid.Ugrid2d)
+    assert grid.n_face == 4
+
+
+def test_from_structured_bounds():
+    x_vertices = np.array([1.0, 3.0, 5.0, 7.0, 9.0])
+    y_vertices = np.array([2.5, 7.5, 12.5, 17.5])
+    # Ascending
+    x_bounds = np.column_stack((x_vertices[:-1], x_vertices[1:]))
+    y_bounds = np.column_stack((y_vertices[:-1], y_vertices[1:]))
+    grid = xugrid.Ugrid2d.from_structured_bounds(x_bounds, y_bounds)
+    assert isinstance(grid, xugrid.Ugrid2d)
+    assert grid.n_face == 12
+
+
+def test_from_structured():
+    da = xr.DataArray(
+        data=np.ones((2, 2)),
+        coords={"y": [12.0, 11.0], "x": [1.0, 2.0]},
+        dims=("y", "x"),
+    )
+    grid = xugrid.Ugrid2d.from_structured(da)
+    assert isinstance(grid, xugrid.Ugrid2d)
+    assert grid.n_face == 4
+
+    da = xr.DataArray(
+        data=np.ones((2, 2)),
+        coords={"lat": [12.0, 11.0], "lon": [1.0, 2.0]},
+        dims=("lat", "lon"),
+    )
+    grid = xugrid.Ugrid2d.from_structured(da, x="lon", y="lat")
+    assert isinstance(grid, xugrid.Ugrid2d)
+    assert grid.n_face == 4
+
+
+def test_form_structured_multicoord():
+    da = xr.DataArray(
+        data=np.ones((2, 2)),
+        coords={
+            "yc": (("y", "x"), [[12.0, 11.0], [13.0, 12.0]]),
+            "xc": (("y", "x"), [[1.0, 2.0], [2.0, 3.0]]),
+        },
+        dims=("y", "x"),
+    )
+    grid = xugrid.Ugrid2d.from_structured_multicoord(da, x="xc", y="yc")
+    assert isinstance(grid, xugrid.Ugrid2d)
+    assert grid.n_face == 4
+
+
 def test_from_shapely():
     with pytest.raises(TypeError):
         x = np.array([0.0, 1.0, 2.0])
         y = np.array([0.0, 0.0, 0.0])
         xugrid.Ugrid2d.from_shapely(geometry=shapely.linestrings(x, y))
 
     xy = np.array(
@@ -1271,7 +1362,18 @@
         )
         assert np.array_equal(back_ds["c"], [0, 1, 2, 3, 4, 5])
 
         back = periodic_grid.to_nonperiodic(xmax=3.0)
         assert np.allclose(back.node_coordinates, expected_vertices)
         assert np.array_equal(back.face_node_connectivity, expected_faces)
         assert back.edge_node_connectivity.shape == (17, 2)
+
+
+def test_equals():
+    grid = grid2d()
+    grid_copy = grid2d()
+    assert grid.equals(grid)
+    assert grid.equals(grid_copy)
+    xr_grid = grid.to_dataset()
+    assert not grid.equals(xr_grid)
+    grid_copy.attrs["attr"] = "something_else"
+    assert not grid.equals(grid_copy)
```

### Comparing `xugrid-0.8.1/tests/test_ugrid_dataset.py` & `xugrid-0.9.0/tests/test_ugrid_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,14 +173,33 @@
         assert uda.shape == (2, 12)
         assert np.allclose(uda.ugrid.sel(x=2.0, y=5.0), [[0], [12]])
         # Check whether flipping the y-axis doesn't cause any problems
         flipped = da.isel(y=slice(None, None, -1))
         uda = xugrid.UgridDataArray.from_structured(flipped)
         assert np.allclose(uda.ugrid.sel(x=2.0, y=5.0), [[0], [12]])
 
+    def test_from_structured_multicoord(self):
+        da = xr.DataArray(
+            data=[[0, 1], [2, 3]],
+            coords={
+                "yc": (("y", "x"), [[12.0, 11.0], [12.0, 11.0]]),
+                "xc": (("y", "x"), [[10.0, 12.0], [10.0, 12.0]]),
+            },
+            dims=("y", "x"),
+        )
+        uda = xugrid.UgridDataArray.from_structured(da)
+        assert isinstance(uda, xugrid.UgridDataArray)
+        assert np.array_equal(np.unique(uda.ugrid.grid.node_x), [-0.5, 0.5, 1.5])
+        assert np.array_equal(uda.data, [0, 1, 2, 3])
+
+        uda = xugrid.UgridDataArray.from_structured(da, x="xc", y="yc")
+        assert isinstance(uda, xugrid.UgridDataArray)
+        assert np.array_equal(np.unique(uda.ugrid.grid.node_x), [9.0, 11.0, 13.0])
+        assert np.array_equal(uda.data, [0, 1, 2, 3])
+
     def test_unary_op(self):
         alltrue = self.uda.astype(bool)
         allfalse = alltrue.copy()
         allfalse[:] = False
         assert (~allfalse).all()
         assert isinstance(~allfalse, xugrid.UgridDataArray)
 
@@ -924,14 +943,19 @@
     assert np.array_equal(result["layer"], [1, 2])
 
     uds1d = ugrid1d_ds()
     uda3 = uds1d["a1d"].assign_coords(layer=2)
     with pytest.raises(ValueError, match="All UgridDataArrays must have the same grid"):
         xugrid.concat([uda1, uda3], dim="layer")
 
+    # test issue 206 resolved
+    # https://github.com/Deltares/xugrid/issues/206
+    result = xugrid.concat([uda1, uda2.copy()], dim="foo")
+    assert len(result.grids) == 1
+
 
 def test_multiple_topology_errors():
     # Create a dataset with two UGRID topologies:
     uds = ugrid1d_ds()
     uds["a"] = xugrid.UgridDataset(UGRID_DS())["a"]
 
     with pytest.raises(TypeError, match="Can only access grid topology"):
@@ -948,15 +972,15 @@
     uds2d = xugrid.UgridDataset(UGRID_DS())
     uds1d = ugrid1d_ds()
     merged = xugrid.merge([uds2d, uds1d])
     assert isinstance(merged, xugrid.UgridDataset)
     assert len(merged.grids) == 2
 
 
-def get_ugrid_fillvaluem999_startindex1():
+def get_ugrid_fillvaluem999_startindex1_ds():
     """
     Return a minimal dataset with a specific fill value.
 
     This is a very minimal but comparable dataset to Grevelingen_0002_map.nc
     (FM output).
 
     * It contains both triangles and squares.
@@ -1105,52 +1129,54 @@
         "_FillValue": -999,
     }
     ds2["mesh2d_edge_nodes"] = xr.DataArray(
         enc, dims=(mesh2d_attrs["edge_dimension"], "two"), attrs=enc_attrs
     )
 
     # add dummy face variable in order to have a face dimension in the uds
-    facevar = np.ones(shape=(ds2.dims[mesh2d_attrs["face_dimension"]]))
+    facevar = np.ones(shape=(ds2.sizes[mesh2d_attrs["face_dimension"]]))
     ds2["mesh2d_facevar"] = xr.DataArray(facevar, dims=(mesh2d_attrs["face_dimension"]))
 
     # add dummy nodevar to plot and trigger triangulation procedure
-    nodevar = np.ones(shape=(ds2.dims[mesh2d_attrs["node_dimension"]]))
+    nodevar = np.ones(shape=(ds2.sizes[mesh2d_attrs["node_dimension"]]))
     ds2["mesh2d_nodevar"] = xr.DataArray(nodevar, dims=(mesh2d_attrs["node_dimension"]))
+    return ds2
 
+
+def get_ugrid_fillvaluem999_startindex1_uds():
     # upon loading a dataset from a file, xarray decodes it, so we also do it here
+    ds2 = get_ugrid_fillvaluem999_startindex1_ds()
     ds2_enc = xr.decode_cf(ds2)
-
     uds = xugrid.UgridDataset(ds2_enc)
-
     return uds
 
 
 def test_fm_fillvalue_startindex_isel():
     """
     FM data has 1-based starting index and _FillValue -999, this raises several
     issues. Since it is not possible to generate a Ugrid2d with these
     attributes, we are testing with raw data
     """
 
     # xugrid 0.5.0 warns "RuntimeWarning: invalid value encountered in cast: cast = data.astype(dtype, copy=True)"
-    uds = get_ugrid_fillvaluem999_startindex1()
+    uds = get_ugrid_fillvaluem999_startindex1_uds()
 
     # xugrid 0.6.0 raises "ValueError: Invalid edge_node_connectivity"
     uds.isel({uds.grid.face_dimension: [1]})
 
 
 def test_fm_facenodeconnectivity_fillvalue():
     """
     FM data has 1-based starting index and _FillValue -999, this raises several
     issues. Since it is not possible to generate a Ugrid2d with these
     attributes, we are testing with raw data
     """
 
     # xugrid 0.5.0 warns "RuntimeWarning: invalid value encountered in cast: cast = data.astype(dtype, copy=True)"
-    uds = get_ugrid_fillvaluem999_startindex1()
+    uds = get_ugrid_fillvaluem999_startindex1_uds()
 
     # xugrid 0.6.0 has -2 values in the array
     assert (uds.grid.face_node_connectivity != -2).all()
 
 
 def test_periodic_conversion():
     vertices = np.array(
@@ -1235,7 +1261,23 @@
 def test_laplace_interpolate_1d():
     uda = ugrid1d_ds()["a1d"]
     uda[:] = 1.0
     uda[1] = np.nan
     actual = uda.ugrid.laplace_interpolate(direct_solve=True)
     assert isinstance(actual, xugrid.UgridDataArray)
     assert np.allclose(actual, 1.0)
+
+
+def test_ugriddataset_wrap_twice(tmp_path):
+    """
+    in issue https://github.com/Deltares/xugrid/issues/208 wrapping a ds
+    twice with UgridDataset resulted in "ValueError: connectivity contains negative values",
+    because the original connectivity array in the xarray dataset was altered.
+    This tests ensures that future changes will not cause this issue again.
+    """
+    ds_raw = get_ugrid_fillvaluem999_startindex1_ds()
+    file_nc = tmp_path / "ugrid_fillvaluem999_startindex1.nc"
+    ds_raw.to_netcdf(file_nc)
+    ds = xr.open_dataset(file_nc)
+
+    _ = xugrid.UgridDataset(ds)
+    _ = xugrid.UgridDataset(ds)
```

### Comparing `xugrid-0.8.1/tests/test_voronoi.py` & `xugrid-0.9.0/tests/test_voronoi.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.8.1/tests/fixtures/fixture_regridder.py` & `xugrid-0.9.0/tests/fixtures/fixture_regridder.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.8.1/tests/test_regrid/test_overlap_1d.py` & `xugrid-0.9.0/tests/test_regrid/test_overlap_1d.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.8.1/tests/test_regrid/test_reduce.py` & `xugrid-0.9.0/tests/test_regrid/test_reduce.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.8.1/tests/test_regrid/test_regridder.py` & `xugrid-0.9.0/tests/test_regrid/test_regridder.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.8.1/tests/test_regrid/test_structured.py` & `xugrid-0.9.0/tests/test_regrid/test_structured.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.8.1/tests/test_regrid/test_unstructured.py` & `xugrid-0.9.0/tests/test_regrid/test_unstructured.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.8.1/tests/test_regrid/test_utils.py` & `xugrid-0.9.0/tests/test_regrid/test_utils.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.8.1/xugrid/__init__.py` & `xugrid-0.9.0/xugrid/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from xugrid.ugrid.conventions import UgridRolesAccessor
 from xugrid.ugrid.partitioning import merge_partitions
 from xugrid.ugrid.polygonize import polygonize
 from xugrid.ugrid.snapping import snap_to_grid
 from xugrid.ugrid.ugrid1d import Ugrid1d
 from xugrid.ugrid.ugrid2d import Ugrid2d
 
-__version__ = "0.8.1"
+__version__ = "0.9.0"
 
 __all__ = (
     "data",
     "concat",
     "full_like",
     "merge",
     "ones_like",
```

### Comparing `xugrid-0.8.1/xugrid/constants.py` & `xugrid-0.9.0/xugrid/constants.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.8.1/xugrid/conversion.py` & `xugrid-0.9.0/xugrid/conversion.py`

 * *Files 18% similar despite different names*

```diff
@@ -129,56 +129,118 @@
 def _array_spacing(coords, spacing):
     if coords.size != spacing.size:
         raise ValueError(f"size of {coords.name} does not match size of {spacing.name}")
     halfdiff = 0.5 * abs(spacing)
     return halfdiff
 
 
-def _implicit_spacing(coords):
-    dim = coords.dims[0]
-    if coords.size == 1:
-        raise ValueError(
-            f"Cannot derive spacing of 1-sized coordinate: {coords.name} \n"
-            f"Set bounds yourself or assign a d{coords.name} variable with spacing"
-        )
-    halfdiff = 0.5 * abs(coords.diff(dim)).to_numpy()
-    return np.insert(halfdiff, 0, halfdiff[0])
+def _is_monotonic_and_increasing(coord, axis=0) -> bool:
+    """
+    Test if monotonic and retun whether increasing along axis.
+    Raises error if not monotonic.
+
+    Copied and slightly adapted from xarray.utils.
+
+    >>> _is_monotonic(np.array([0, 1, 2]))
+    True
+    >>> _is_monotonic(np.array([2, 1, 0]))
+    True
+    >>> _is_monotonic(np.array([0, 2, 1]))
+    False
+    """
+    coord = np.asarray(coord)
+    n = coord.shape[axis]
+    delta_pos = coord.take(np.arange(1, n), axis=axis) >= coord.take(
+        np.arange(0, n - 1), axis=axis
+    )
+    delta_neg = coord.take(np.arange(1, n), axis=axis) <= coord.take(
+        np.arange(0, n - 1), axis=axis
+    )
+    if np.all(delta_pos):
+        return True
+    elif np.all(delta_neg):
+        return False
+    else:
+        raise ValueError("The input coordinate is not monotonic.")
+
 
+def infer_interval_breaks(coord, axis: int = 0, check_monotonic: bool = False):
+    """
+    Infer intervals from cell center coordinates.
+
+    Copied and adapted from xarray.utils.
+
+    >>> _infer_interval_breaks(np.arange(5))
+    array([-0.5,  0.5,  1.5,  2.5,  3.5,  4.5])
+    >>> _infer_interval_breaks([[0, 1], [3, 4]], axis=1)
+    array([[-0.5,  0.5,  1.5],
+           [ 2.5,  3.5,  4.5]])
+    """
+    coord = np.asarray(coord)
+    if check_monotonic:
+        _is_monotonic_and_increasing(coord, axis=axis)
+
+    deltas = 0.5 * np.diff(coord, axis=axis)
+    if deltas.size == 0:
+        deltas = np.array(0.0)
+
+    first = np.take(coord, [0], axis=axis) - np.take(deltas, [0], axis=axis)
+    last = np.take(coord, [-1], axis=axis) + np.take(deltas, [-1], axis=axis)
+    trim_last = tuple(
+        slice(None, -1) if n == axis else slice(None) for n in range(coord.ndim)
+    )
+    interval_breaks = np.concatenate(
+        [first, coord[trim_last] + deltas, last], axis=axis
+    )
+    return interval_breaks
 
-def infer_bounds(
+
+def infer_interval_breaks1d(
     obj: Union[xr.DataArray, xr.Dataset],
     var: str,
-):
-    coords = obj[var]
-    index = obj.indexes[var]
-    if not (index.is_monotonic_increasing or index.is_monotonic_decreasing):
-        raise ValueError(f"{var} is not monotonic")
-
-    # e.g. rioxarray will set dx, dy as (scalar) values.
+) -> np.ndarray:
+    """
+    Infer the breaks for 1D coordinates.
+
+        * For non-equidistant grids, taking half of each cell size result in
+          wrong answers.
+        * Cell size may be provided by a dx or dy attribute instead.
+        * We also want to take 1-row or 1 column topologies into account.
+    """
+    coord = obj[var]
     spacing_name = f"d{var}"
+
+    # Spacing name is provided:
     if spacing_name in obj.coords:
         spacing = obj[spacing_name]
-        spacing_shape = spacing.shape
-        if len(spacing_shape) > 1:
+        if spacing.ndim > 1:
             raise NotImplementedError(
                 f"More than one dimension in spacing variable: {spacing_name}"
             )
+        if spacing.shape in ((), (1,)):
+            halfdiff = _scalar_spacing(coord, spacing)
+        else:
+            halfdiff = _array_spacing(coord, spacing)
 
-        if spacing_shape in ((), (1,)):
-            halfdiff = _scalar_spacing(coords, spacing)
+        # Now check if monotonic and take orientation into account.
+        if _is_monotonic_and_increasing(coord):
+            intervals = np.insert(coord + halfdiff, 0, coord[0] - halfdiff[0])
         else:
-            halfdiff = _array_spacing(coords, spacing)
-    # Implicit spacing
+            intervals = np.insert(coord - halfdiff, 0, coord[0] + halfdiff[0])
+
+    # Implicit spacing, infer from coordinates instead:
     else:
-        halfdiff = _implicit_spacing(coords)
+        if coord.size == 1:
+            raise ValueError(
+                f"Cannot derive spacing of 1-sized coordinate: {var} \n"
+                f"Assign a d{var} variable with spacing instead."
+            )
+        intervals = infer_interval_breaks(coord.to_numpy(), check_monotonic=True)
 
-    lower = coords - halfdiff
-    upper = coords + halfdiff
-    bounds = xr.concat([lower, upper], dim="bounds").transpose()
-    return bounds
+    return intervals
 
 
 def infer_xy_coords(obj):
     # First check names, then check whether CF roles are specified.
     x = None
     y = None
     if "x" in obj.dims and "y" in obj.dims:
```

### Comparing `xugrid-0.8.1/xugrid/meshkernel_utils.py` & `xugrid-0.9.0/xugrid/meshkernel_utils.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.8.1/xugrid/core/accessorbase.py` & `xugrid-0.9.0/xugrid/core/accessorbase.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.8.1/xugrid/core/common.py` & `xugrid-0.9.0/xugrid/core/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from functools import wraps
 
 import xarray as xr
 
+from xugrid.core.utils import unique_grids
 from xugrid.core.wrap import UgridDataArray, UgridDataset
 
 DATAARRAY_NAME = "__xarray_dataarray_name__"
 DATAARRAY_VARIABLE = "__xarray_dataarray_variable__"
 
 
 def open_dataset(*args, **kwargs):
@@ -94,15 +95,15 @@
                 raise TypeError(
                     "Can only concatenate xugrid UgridDataset and UgridDataArray "
                     f"objects, got {type(obj).__name__}"
                 )
 
             bare_objs.append(obj.obj)
 
-        grids = set(grids)
+        grids = unique_grids(grids)
         result = func(bare_objs, *args, **kwargs)
         if isinstance(result, xr.DataArray):
             if len(grids) > 1:
                 raise ValueError("All UgridDataArrays must have the same grid")
             return UgridDataArray(result, next(iter(grids)))
         else:
             return UgridDataset(result, grids)
```

### Comparing `xugrid-0.8.1/xugrid/core/dataarray_accessor.py` & `xugrid-0.9.0/xugrid/core/dataarray_accessor.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.8.1/xugrid/core/dataset_accessor.py` & `xugrid-0.9.0/xugrid/core/dataset_accessor.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.8.1/xugrid/core/sparse.py` & `xugrid-0.9.0/xugrid/core/sparse.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.8.1/xugrid/core/utils.py` & `xugrid-0.9.0/xugrid/core/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 https://github.com/pydata/xarray/blob/main/LICENSE
 """
 from __future__ import annotations
 
 from collections.abc import Hashable, Mapping
 from typing import Any, TypeVar, cast
 
+from xugrid.ugrid.ugridbase import UgridType
+
 T = TypeVar("T")
 
 
 def is_dict_like(value: Any) -> Any:
     return hasattr(value, "keys") and hasattr(value, "__getitem__")
 
 
@@ -51,7 +53,18 @@
         self._accessor = accessor
 
     def __get__(self, obj: None | object, cls) -> Any:
         if obj is None:
             return self._accessor
 
         return self._accessor(obj)  # type: ignore  # assume it is a valid accessor!
+
+
+def unique_grids(grids: list[UgridType]) -> list[UgridType]:
+    uniques: list[UgridType] = []
+    for grid in grids:
+        for unique in uniques:
+            if grid.equals(unique):
+                break
+        else:
+            uniques.append(grid)
+    return uniques
```

### Comparing `xugrid-0.8.1/xugrid/core/wrap.py` & `xugrid-0.9.0/xugrid/core/wrap.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 """
 Wrap in advance instead of overloading __getattr__.
 
 This allows for tab completion and documentation.
 """
+from __future__ import annotations
 
 import types
 from collections import ChainMap
 from functools import wraps
 from itertools import chain
 from typing import List, Sequence, Union
 
 import xarray as xr
 from pandas import RangeIndex
 
 import xugrid
 from xugrid.conversion import grid_from_dataset, grid_from_geodataframe
+from xugrid.core.utils import unique_grids
 from xugrid.ugrid.ugrid2d import Ugrid2d
 from xugrid.ugrid.ugridbase import AbstractUgrid, UgridType, align
 
 # Import entire module here for circular import of UgridDatasetAccessor and
 # UgridDataArrayAccessor. Note: can only be used in functions (since that code
 # is run at runtime).
 
@@ -29,15 +31,15 @@
 
     # Topology can either be a sequence of grids or a grid.
     if isinstance(topology, (list, set, tuple)):
         grids = {dim: grid for grid in topology for dim in grid.dimensions}
     else:
         grids = {dim: topology for dim in topology.dimensions}
 
-    item_grids = list({grids[dim] for dim in obj.dims if dim in grids})
+    item_grids = unique_grids([grids[dim] for dim in obj.dims if dim in grids])
 
     if len(item_grids) == 0:
         return obj
     else:
         result, aligned = align(obj, item_grids, old_indexes)
 
         if isinstance(result, xr.DataArray):
@@ -226,32 +228,57 @@
         topology available.
         """
         return xugrid.core.dataarray_accessor.UgridDataArrayAccessor(
             self.obj, self.grid
         )
 
     @staticmethod
-    def from_structured(da: xr.DataArray):
+    def from_structured(
+        da: xr.DataArray,
+        x: str | None = None,
+        y: str | None = None,
+    ) -> "UgridDataArray":
         """
         Create a UgridDataArray from a (structured) xarray DataArray.
 
         The spatial dimensions are flattened into a single UGRID face dimension.
 
+        By default, this method looks for the "x" and "y" coordinates and assumes
+        they are one-dimensional. To convert rotated or curvilinear coordinates,
+        provide the names of the x and y coordinates.
+
         Parameters
         ----------
         da: xr.DataArray
             Last two dimensions must be ``("y", "x")``.
+        x: str, default: None
+            Which coordinate to use as the UGRID x-coordinate.
+        y: str, default: None
+            Which coordinate to use as the UGRID y-coordinate.
 
         Returns
         -------
         unstructured: UgridDataArray
         """
         if da.dims[-2:] != ("y", "x"):
             raise ValueError('Last two dimensions of da must be ("y", "x")')
-        grid = Ugrid2d.from_structured(da)
+        if (x is None) ^ (y is None):
+            raise ValueError("Provide both x and y, or neither.")
+        if x is None:
+            grid = Ugrid2d.from_structured(da)
+        else:
+            # Find out if it's multi-dimensional
+            xdim = da[x].ndim
+            if xdim == 1:
+                grid = Ugrid2d.from_structured(da, x=x, y=y)
+            elif xdim == 2:
+                grid = Ugrid2d.from_structured_multicoord(da, x=x, y=y)
+            else:
+                raise ValueError(f"x and y must be 1D or 2D. Found: {xdim}")
+
         dims = da.dims[:-2]
         coords = {k: da.coords[k] for k in dims}
         face_da = xr.DataArray(
             da.data.reshape(*da.shape[:-2], -1),
             coords=coords,
             dims=[*dims, grid.face_dimension],
             name=da.name,
```

### Comparing `xugrid-0.8.1/xugrid/data/sample_data.py` & `xugrid-0.9.0/xugrid/data/sample_data.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.8.1/xugrid/data/synthetic.py` & `xugrid-0.9.0/xugrid/data/synthetic.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.8.1/xugrid/plot/plot.py` & `xugrid-0.9.0/xugrid/plot/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -446,15 +446,15 @@
     # cells otherwise for the smallest axis.
     resolution = kwargs.pop("resolution", None)
     if resolution is None:
         resolution = min(dx, dy) / 500
 
     _, _, index = grid.rasterize(resolution)
     img = da.to_numpy()[index].astype(float)
-    img[index == grid.fill_value] = np.nan
+    img[index == -1] = np.nan
     primitive = ax.imshow(img, **kwargs)
     return primitive
 
 
 @_plot2d
 def contour(grid, da, ax, **kwargs):
     """
```

### Comparing `xugrid-0.8.1/xugrid/plot/utils.py` & `xugrid-0.9.0/xugrid/plot/utils.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.8.1/xugrid/regrid/overlap_1d.py` & `xugrid-0.9.0/xugrid/regrid/overlap_1d.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.8.1/xugrid/regrid/reduce.py` & `xugrid-0.9.0/xugrid/regrid/reduce.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.8.1/xugrid/regrid/regridder.py` & `xugrid-0.9.0/xugrid/regrid/regridder.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.8.1/xugrid/regrid/structured.py` & `xugrid-0.9.0/xugrid/regrid/structured.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.8.1/xugrid/regrid/unstructured.py` & `xugrid-0.9.0/xugrid/regrid/unstructured.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.8.1/xugrid/regrid/utils.py` & `xugrid-0.9.0/xugrid/regrid/utils.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.8.1/xugrid/ugrid/burn.py` & `xugrid-0.9.0/xugrid/ugrid/burn.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from typing import List, Union
 
 import numba as nb
 import numpy as np
 import xarray as xr
 from numba_celltree.constants import TOLERANCE_ON_EDGE, Point, Triangle
 from numba_celltree.geometry_utils import (
@@ -12,25 +14,19 @@
 )
 
 import xugrid
 from xugrid.constants import FloatArray, IntArray, MissingOptionalModule
 
 try:
     import shapely
+
 except ImportError:
     shapely = MissingOptionalModule("shapely")
 
 
-POINT = shapely.GeometryType.POINT
-LINESTRING = shapely.GeometryType.LINESTRING
-LINEARRING = shapely.GeometryType.LINEARRING
-POLYGON = shapely.GeometryType.POLYGON
-GEOM_NAMES = {v: k for k, v in shapely.GeometryType.__members__.items()}
-
-
 @nb.njit(inline="always")
 def in_bounds(p: Point, a: Point, b: Point) -> bool:
     """
     Check whether point p falls within the bounding box created by a and b
     (after we've checked the size of the cross product).
 
     However, we must take into account that a line may be either vertical
@@ -224,15 +220,15 @@
     output[face_index] = values[value_index]
     return
 
 
 def burn_vector_geometry(
     gdf: "geopandas.GeoDataframe",  # type: ignore # noqa
     like: Union["xugrid.Ugrid2d", "xugrid.UgridDataArray", "xugrid.UgridDataset"],
-    column: str = None,
+    column: str | None = None,
     fill: Union[int, float] = np.nan,
     all_touched: bool = False,
 ) -> None:
     """
     Burn vector geometries (points, lines, polygons) into a Ugrid2d mesh.
 
     If no ``column`` argument is provided, a value of 1.0 will be burned in to
@@ -240,29 +236,35 @@
 
     Parameters
     ----------
     gdf: geopandas.GeoDataFrame
         Polygons, points, and/or lines to be burned into the grid.
     like: UgridDataArray, UgridDataset, or Ugrid2d
         Grid to burn the vector data into.
-    column: str
+    column: str, optional
         Name of the geodataframe column of which to the values to burn into
         grid.
     fill: int, float, optional, default value ``np.nan``.
         Fill value for nodata areas.
     all_touched: bool, optional, default value ``False``.
         All mesh faces (cells) touched by polygons will be updated, not just
         those whose center point is within the polygon.
 
     Returns
     -------
     burned: UgridDataArray
     """
     import geopandas as gpd
 
+    POINT = shapely.GeometryType.POINT
+    LINESTRING = shapely.GeometryType.LINESTRING
+    LINEARRING = shapely.GeometryType.LINEARRING
+    POLYGON = shapely.GeometryType.POLYGON
+    GEOM_NAMES = {v: k for k, v in shapely.GeometryType.__members__.items()}
+
     if not isinstance(gdf, gpd.GeoDataFrame):
         raise TypeError(f"gdf must be GeoDataFrame, received: {type(like).__name__}")
     if isinstance(like, (xugrid.UgridDataArray, xugrid.UgridDataset)):
         like = like.ugrid.grid
     if not isinstance(like, xugrid.Ugrid2d):
         raise TypeError(
             "Like must be Ugrid2d, UgridDataArray, or UgridDataset;"
```

### Comparing `xugrid-0.8.1/xugrid/ugrid/connectivity.py` & `xugrid-0.9.0/xugrid/ugrid/connectivity.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.8.1/xugrid/ugrid/conventions.py` & `xugrid-0.9.0/xugrid/ugrid/conventions.py`

 * *Files 0% similar despite different names*

```diff
@@ -267,15 +267,15 @@
                 else:
                     if prev_dim not in var_dims:
                         raise UgridDimensionError(
                             f"{key}: {prev_dim} not in {role}: {varname}"
                             f" with dimensions: {var_dims}"
                         )
             elif isinstance(key, int):
-                dim_size = ds.dims[dim]
+                dim_size = ds.sizes[dim]
                 if not dim_size == key:
                     raise UgridDimensionError(
                         f"Expected size {key} for dimension {dim} in variable "
                         f"{varname} with role {role}, found instead: "
                         f"{dim_size}"
                     )
```

### Comparing `xugrid-0.8.1/xugrid/ugrid/interpolate.py` & `xugrid-0.9.0/xugrid/ugrid/interpolate.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.8.1/xugrid/ugrid/partitioning.py` & `xugrid-0.9.0/xugrid/ugrid/partitioning.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """Create and merge partitioned UGRID topologies."""
 from collections import defaultdict
-from itertools import accumulate
+from itertools import accumulate, chain
 from typing import List
 
 import numpy as np
 import xarray as xr
 
 from xugrid.constants import IntArray, IntDType
 from xugrid.core.wrap import UgridDataArray, UgridDataset
 from xugrid.ugrid.connectivity import renumber
+from xugrid.ugrid.ugridbase import UgridType
 
 
 def labels_to_indices(labels: IntArray) -> List[IntArray]:
     """
     Convert a 1D array of N labels into a N arrays of indices.
 
     E.g. [0, 1, 0, 2, 2] -> [[0, 2], [1], [3, 4]]
@@ -141,21 +142,15 @@
         edges = grid.edge_node_connectivity
         n_edge = len(edges)
         all_edges[edge_offset : edge_offset + n_edge] = node_inverse[edges + offset]
 
     return _merge_connectivity(all_edges, slices)
 
 
-def validate_partition_topology(grouped, n_partition: int):
-    n = n_partition
-    if not all(len(v) == n for v in grouped.values()):
-        raise ValueError(
-            f"Expected {n} UGRID topologies for {n} partitions, received: " f"{grouped}"
-        )
-
+def validate_partition_topology(grouped: defaultdict[str, UgridType]) -> None:
     for name, grids in grouped.items():
         types = {type(grid) for grid in grids}
         if len(types) > 1:
             raise TypeError(
                 f"All partition topologies with name {name} should be of the "
                 f"same type, received: {types}"
             )
@@ -166,45 +161,68 @@
                 f"Dimension names on UGRID topology {name} do not match "
                 f"across partitions: {griddims[0]} versus {griddims[1]}"
             )
 
     return None
 
 
-def group_grids_by_name(partitions):
+def group_grids_by_name(partitions: list[UgridDataset]) -> defaultdict[str, UgridType]:
     grouped = defaultdict(list)
     for partition in partitions:
         for grid in partition.grids:
             grouped[grid.name].append(grid)
 
-    validate_partition_topology(grouped, len(partitions))
+    validate_partition_topology(grouped)
     return grouped
 
 
-def validate_partition_objects(data_objects):
-    # Check presence of variables.
-    allvars = list({tuple(sorted(ds.data_vars)) for ds in data_objects})
-    if len(allvars) > 1:
-        raise ValueError(
-            "These variables are present in some partitions, but not in "
-            f"others: {set(allvars[0]).symmetric_difference(allvars[1])}"
-        )
-    # Check dimensions
-    for var in allvars.pop():
-        vardims = list({ds[var].dims for ds in data_objects})
-        if len(vardims) > 1:
-            raise ValueError(
-                f"Dimensions for {var} do not match across partitions: "
-                f"{vardims[0]} versus {vardims[1]}"
-            )
+def group_data_objects_by_gridname(
+    partitions: list[UgridDataset]
+) -> defaultdict[str, xr.Dataset]:
+    # Convert to dataset for convenience
+    data_objects = [partition.obj for partition in partitions]
+    data_objects = [
+        obj.to_dataset() if isinstance(obj, xr.DataArray) else obj
+        for obj in data_objects
+    ]
+
+    grouped = defaultdict(list)
+    for partition, obj in zip(partitions, data_objects):
+        for grid in partition.grids:
+            grouped[grid.name].append(obj)
+
+    return grouped
+
+
+def validate_partition_objects(
+    objects_by_gridname: defaultdict[str, xr.Dataset]
+) -> None:
+    for data_objects in objects_by_gridname.values():
+        allvars = list({tuple(sorted(ds.data_vars)) for ds in data_objects})
+        unique_vars = set(chain(*allvars))
+        # Check dimensions
+        dims_per_var = [
+            {ds[var].dims for ds in data_objects if var in ds.data_vars}
+            for var in unique_vars
+        ]
+        for var, vardims in zip(unique_vars, dims_per_var):
+            if len(vardims) > 1:
+                vardims_ls = list(vardims)
+                raise ValueError(
+                    f"Dimensions for '{var}' do not match across partitions: "
+                    f"{vardims_ls[0]} versus {vardims_ls[1]}"
+                )
+    return None
 
 
-def separate_variables(data_objects, ugrid_dims):
+def separate_variables(
+    objects_by_gridname: defaultdict[str, xr.Dataset], ugrid_dims: set[str]
+):
     """Separate into UGRID variables grouped by dimension, and other variables."""
-    validate_partition_objects(data_objects)
+    validate_partition_objects(objects_by_gridname)
 
     def assert_single_dim(intersection):
         if len(intersection) > 1:
             raise ValueError(
                 f"{var} contains more than one UGRID dimension: {intersection}"
             )
 
@@ -212,39 +230,85 @@
         return tuple[:index] + tuple[index + 1 :]
 
     def all_equal(iterator):
         first = next(iter(iterator))
         return all(element == first for element in iterator)
 
     # Group variables by UGRID dimension.
-    first = data_objects[0]
-    variables = first.variables
-    vardims = {var: tuple(first[var].dims) for var in variables}
-    grouped = defaultdict(list)  # UGRID associated vars
-    other = []  # other vars
-    for var, da in variables.items():
-        shapes = (obj[var].shape for obj in data_objects)
-
-        # Check if variable depends on UGRID dimension.
-        intersection = ugrid_dims.intersection(da.dims)
-        if intersection:
-            assert_single_dim(intersection)
-            # Now check whether the non-UGRID dimensions match.
-            dim = intersection.pop()  # Get the single element in the set.
-            axis = vardims[var].index(dim)
-            shapes = [remove_item(shape, axis) for shape in shapes]
-            if all_equal(shapes):
-                grouped[dim].append(var)
+    grouped = defaultdict(set)  # UGRID associated vars
+    other = defaultdict(set)  # other vars
+
+    for gridname, data_objects in objects_by_gridname.items():
+        variables = {
+            varname: data
+            for obj in data_objects
+            for varname, data in obj.variables.items()
+        }
+        vardims = {varname: data.dims for varname, data in variables.items()}
+        for var, dims in vardims.items():
+            shapes = [obj[var].shape for obj in data_objects if var in obj]
+
+            # Check if variable depends on UGRID dimension.
+            intersection = ugrid_dims.intersection(dims)
+            if intersection:
+                assert_single_dim(intersection)
+                # Now check whether the non-UGRID dimensions match.
+                dim = intersection.pop()  # Get the single element in the set.
+                axis = dims.index(dim)
+                shapes = [remove_item(shape, axis) for shape in shapes]
+                if all_equal(shapes):
+                    grouped[dim].add(var)
 
-        elif all_equal(shapes):
-            other.append(var)
+            elif all_equal(shapes):
+                other[gridname].add(var)
 
     return grouped, other
 
 
+def merge_data_along_dim(
+    data_objects: list[xr.Dataset],
+    vars: list[str],
+    merge_dim: str,
+    indexes: list[np.array],
+    merged_grid: UgridType,
+) -> xr.Dataset:
+    """
+    Select variables from the data objects.
+    Pad connectivity dims if needed.
+    Concatenate along dim.
+    """
+    max_sizes = merged_grid.max_connectivity_sizes
+    ugrid_connectivity_dims = set(max_sizes)
+
+    to_merge = []
+    for obj, index in zip(data_objects, indexes):
+        # Check for presence of vars
+        missing_vars = set(vars).difference(set(obj.variables.keys()))
+        if missing_vars:
+            raise ValueError(f"Missing variables: {missing_vars} in partition {obj}")
+
+        selection = obj[vars].isel({merge_dim: index}, missing_dims="ignore")
+
+        # Pad the ugrid connectivity dims (e.g. n_max_face_node_connectivity) if
+        # needed.
+        present_dims = ugrid_connectivity_dims.intersection(selection.dims)
+        pad_width = {}
+        for dim in present_dims:
+            nmax = max_sizes[dim]
+            size = selection.sizes[dim]
+            if size != nmax:
+                pad_width[dim] = (0, nmax - size)
+        if pad_width:
+            selection = selection.pad(pad_width=pad_width)
+
+        to_merge.append(selection)
+
+    return xr.concat(to_merge, dim=merge_dim)
+
+
 def merge_partitions(partitions):
     """
     Merge topology and data, partitioned along UGRID dimensions, into a single
     UgridDataset.
 
     UGRID topologies and variables are merged if they share a name. Topologies
     and variables must be present in *all* partitions. Dimension names must
@@ -266,42 +330,47 @@
     if len(types) > 1:
         type_names = [t.__name__ for t in types]
         raise TypeError(msg.format(type_names))
     obj_type = types.pop()
     if obj_type not in (UgridDataArray, UgridDataset):
         raise TypeError(msg.format(obj_type.__name__))
 
-    # Convert to dataset for convenience
-    data_objects = [partition.obj for partition in partitions]
-    data_objects = [
-        obj.to_dataset() if isinstance(obj, xr.DataArray) else obj
-        for obj in data_objects
-    ]
     # Collect grids
     grids = [grid for p in partitions for grid in p.grids]
     ugrid_dims = {dim for grid in grids for dim in grid.dimensions}
     grids_by_name = group_grids_by_name(partitions)
-    vars_by_dim, other_vars = separate_variables(data_objects, ugrid_dims)
+
+    data_objects_by_name = group_data_objects_by_gridname(partitions)
+    vars_by_dim, other_vars_by_name = separate_variables(
+        data_objects_by_name, ugrid_dims
+    )
 
     # First, take identical non-UGRID variables from the first partition:
-    merged = data_objects[0][other_vars]
+    merged = xr.Dataset()
 
     # Merge the UGRID topologies into one, and find the indexes to index into
     # the data to avoid duplicates.
     merged_grids = []
-    for grids in grids_by_name.values():
+    for gridname, grids in grids_by_name.items():
+        data_objects = data_objects_by_name[gridname]
+        other_vars = other_vars_by_name[gridname]
+
         # First, merge the grid topology.
         grid = grids[0]
         merged_grid, indexes = grid.merge_partitions(grids)
         merged_grids.append(merged_grid)
 
-        # Now remove duplicates, then concatenate along the UGRID dimension.
+        # Add other vars, unassociated with UGRID dimensions, to dataset.
+        for obj in data_objects:
+            other_vars_obj = set(other_vars).intersection(set(obj.data_vars))
+            merged.update(obj[other_vars_obj])
+
         for dim, dim_indexes in indexes.items():
             vars = vars_by_dim[dim]
-            selection = [
-                obj[vars].isel({dim: index}, missing_dims="ignore")
-                for obj, index in zip(data_objects, dim_indexes)
-            ]
-            merged_selection = xr.concat(selection, dim=dim)
+            if len(vars) == 0:
+                continue
+            merged_selection = merge_data_along_dim(
+                data_objects, vars, dim, dim_indexes, merged_grid
+            )
             merged.update(merged_selection)
 
     return UgridDataset(merged, merged_grids)
```

### Comparing `xugrid-0.8.1/xugrid/ugrid/polygonize.py` & `xugrid-0.9.0/xugrid/ugrid/polygonize.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.8.1/xugrid/ugrid/snapping.py` & `xugrid-0.9.0/xugrid/ugrid/snapping.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.8.1/xugrid/ugrid/ugrid1d.py` & `xugrid-0.9.0/xugrid/ugrid/ugrid1d.py`

 * *Files 1% similar despite different names*

```diff
@@ -626,15 +626,17 @@
             indexes=self._indexes,
             projected=self.projected,
             crs=self.crs,
             attrs=self._attrs,
         )
 
     @staticmethod
-    def merge_partitions(grids: Sequence["Ugrid1d"]) -> "Ugrid1d":
+    def merge_partitions(
+        grids: Sequence["Ugrid1d"]
+    ) -> tuple["Ugrid1d", dict[str, np.array]]:
         """
         Merge grid partitions into a single whole.
 
         Duplicate edges are included only once, and removed from subsequent
         partitions before merging.
 
         Parameters
@@ -658,14 +660,15 @@
         }
 
         merged_grid = Ugrid1d(
             *node_coordinates.T,
             fill_value,
             new_edges,
             name=grid.name,
+            indexes=grid._indexes,
             projected=grid.projected,
             crs=grid.crs,
             attrs=grid._attrs,
         )
         return merged_grid, indexes
 
     def reindex_like(
```

### Comparing `xugrid-0.8.1/xugrid/ugrid/ugrid2d.py` & `xugrid-0.9.0/xugrid/ugrid/ugrid2d.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from itertools import chain
 from typing import Any, Dict, Optional, Sequence, Tuple, Union
 
 import numpy as np
 import pandas as pd
 import xarray as xr
 from numba_celltree import CellTree2d
@@ -412,14 +414,28 @@
         return {
             self.node_dimension: self.n_node,
             self.edge_dimension: self.n_edge,
             self.face_dimension: self.n_face,
         }
 
     @property
+    def max_face_node_dimension(self) -> str:
+        return self._attrs["max_face_nodes_dimension"]
+
+    @property
+    def max_connectivity_sizes(self) -> dict[str, int]:
+        return {
+            self.max_face_node_dimension: self.n_max_node_per_face,
+        }
+
+    @property
+    def max_connectivity_dimensions(self) -> tuple[str]:
+        return (self.max_face_node_dimension,)
+
+    @property
     def topology_dimension(self):
         """Highest dimensionality of the geometric elements: 2"""
         return 2
 
     @property
     def face_dimension(self):
         """Return the name of the face dimension."""
@@ -1485,15 +1501,17 @@
         from xugrid.ugrid.partitioning import labels_to_indices
 
         labels = self.label_partitions(n_part)
         indices = labels_to_indices(labels.values)
         return [self.topology_subset(index) for index in indices]
 
     @staticmethod
-    def merge_partitions(grids: Sequence["Ugrid2d"]) -> "Ugrid2d":
+    def merge_partitions(
+        grids: Sequence["Ugrid2d"]
+    ) -> tuple["Ugrid2d", dict[str, np.array]]:
         """
         Merge grid partitions into a single whole.
 
         Duplicate faces are included only once, and removed from subsequent
         partitions before merging.
 
         Parameters
@@ -1966,58 +1984,182 @@
 
         x, y, face_node_connectivity, fill_value = conversion.polygons_to_faces(
             geometry
         )
         return Ugrid2d(x, y, fill_value, face_node_connectivity, crs=crs)
 
     @staticmethod
-    def from_structured_bounds(
-        x_bounds: np.ndarray,
-        y_bounds: np.ndarray,
+    def _from_intervals_helper(
+        node_x: np.ndarray,
+        node_y: np.ndarray,
+        nx: int,
+        ny: int,
     ) -> "Ugrid2d":
-        nx, _ = x_bounds.shape
-        ny, _ = y_bounds.shape
-        nfaces = ny * nx
-        x = conversion.bounds_to_vertices(x_bounds)
-        y = conversion.bounds_to_vertices(y_bounds)
-
-        # Compute all vertices, these are the ugrid nodes
-        node_y, node_x = (a.ravel() for a in np.meshgrid(y, x, indexing="ij"))
         linear_index = np.arange(node_x.size, dtype=IntDType).reshape((ny + 1, nx + 1))
         # Allocate face_node_connectivity
-        face_nodes = np.empty((nfaces, 4), dtype=IntDType)
+        face_nodes = np.empty((ny * nx, 4), dtype=IntDType)
         # Set connectivity in counterclockwise manner
         face_nodes[:, 0] = linear_index[:-1, 1:].ravel()  # upper right
         face_nodes[:, 1] = linear_index[:-1, :-1].ravel()  # upper left
         face_nodes[:, 2] = linear_index[1:, :-1].ravel()  # lower left
         face_nodes[:, 3] = linear_index[1:, 1:].ravel()  # lower right
         return Ugrid2d(node_x, node_y, -1, face_nodes)
 
     @staticmethod
+    def from_structured_intervals1d(
+        x_intervals: np.ndarray,
+        y_intervals: np.ndarray,
+    ) -> "Ugrid2d":
+        """
+        Create a Ugrid2d topology from a structured topology based on 1D intervals.
+
+        Parameters
+        ----------
+        x_intervals: np.ndarray of shape (M + 1,)
+            x-coordinate interval values for N row and M columns.
+        y_intervals: np.ndarray of shape (N + 1,)
+            y-coordinate interval values for N row and M columns.
+        """
+        x_intervals = np.asarray(x_intervals)
+        y_intervals = np.asarray(y_intervals)
+        nx = x_intervals.shape[0] - 1
+        ny = y_intervals.shape[0] - 1
+        node_y, node_x = (
+            a.ravel() for a in np.meshgrid(y_intervals, x_intervals, indexing="ij")
+        )
+        return Ugrid2d._from_intervals_helper(node_x, node_y, nx, ny)
+
+    @staticmethod
+    def from_structured_intervals2d(
+        x_intervals: np.ndarray,
+        y_intervals: np.ndarray,
+    ) -> "Ugrid2d":
+        """
+        Create a Ugrid2d topology from a structured topology based on 2D intervals.
+
+        Parameters
+        ----------
+        x_intervals: np.ndarray of shape shape (N + 1, M + 1)
+            x-coordinate interval values for N row and M columns.
+        y_intervals: np.ndarray of shape shape (N + 1, M + 1)
+            y-coordinate interval values for N row and M columns.
+        """
+        x_intervals = np.asarray(x_intervals)
+        y_intervals = np.asarray(y_intervals)
+        shape = x_intervals.shape
+        if (x_intervals.ndim != 2) or (y_intervals.ndim != 2):
+            raise ValueError("Dimensions of intervals must be 2D.")
+        if shape != y_intervals.shape:
+            raise ValueError(
+                "Interval shapes must match. Found: "
+                f"x_intervals: {shape}, versus y_intervals: {y_intervals.shape}"
+            )
+        nx = shape[1] - 1
+        ny = shape[0] - 1
+        node_x = x_intervals.ravel()
+        node_y = y_intervals.ravel()
+        return Ugrid2d._from_intervals_helper(node_x, node_y, nx, ny)
+
+    @staticmethod
+    def from_structured_bounds(
+        x_bounds: np.ndarray,
+        y_bounds: np.ndarray,
+    ) -> "Ugrid2d":
+        """
+        Create a Ugrid2d topology from a structured topology based on 1D bounds.
+
+        The bounds contain the lower and upper cell boundary for each cell.
+
+        Parameters
+        ----------
+        x_bounds: np.ndarray of shape (M, 2)
+            x-coordinate bounds for N row and M columns.
+        y_bounds: np.ndarray of shape (N, 2)
+            y-coordinate bounds for N row and M columns.
+
+        Returns
+        -------
+        grid: Ugrid2d
+        """
+        nx, _ = x_bounds.shape
+        ny, _ = y_bounds.shape
+        x = conversion.bounds_to_vertices(x_bounds)
+        y = conversion.bounds_to_vertices(y_bounds)
+        node_y, node_x = (a.ravel() for a in np.meshgrid(y, x, indexing="ij"))
+        return Ugrid2d._from_intervals_helper(node_x, node_y, nx, ny)
+
+    @staticmethod
     def from_structured(
         data: Union[xr.DataArray, xr.Dataset],
-        x_bounds: str = None,
-        y_bounds: str = None,
+        x: str | None = None,
+        y: str | None = None,
     ) -> "Ugrid2d":
-        if x_bounds is not None and y_bounds is not None:
-            x_bounds = data[x_bounds]
-            y_bounds = data[y_bounds]
-        else:
-            x_coord, y_coord = conversion.infer_xy_coords(data)
-            x_bounds = conversion.infer_bounds(data, x_coord)
-            y_bounds = conversion.infer_bounds(data, y_coord)
-            if x_bounds is None or y_bounds is None:
+        """
+        Create a Ugrid2d topology from an axis-aligned rectilinear structured topology.
+
+        This method assumes the coordinates are 1D.
+
+        Use ``from_structured_multicoord`` for 2D x and y coordinates, e.g. for
+        (approximated) curvilinear and rotated structured topologies.
+
+        Parameters
+        ----------
+        data: xr.DataArray or xr.Dataset
+        x: str, optional
+            Name of the 1D coordinate to use as the UGRID x-coordinate.
+        y: str, optional
+            Name of the 1D coordinate to use as the UGRID y-coordinate.
+
+        Returns
+        -------
+        grid: Ugrid2d
+        """
+        if x is None or y is None:
+            x, y = conversion.infer_xy_coords(data)
+            if x is None or y is None:
                 raise ValueError(
-                    "Could not infer bounds. Please provide x_bounds and"
-                    " y_bounds explicitly."
+                    "Could not infer bounds. Please provide x and y explicitly."
                 )
-        return Ugrid2d.from_structured_bounds(
-            x_bounds.to_numpy(),
-            y_bounds.to_numpy(),
-        )
+
+        x_intervals = conversion.infer_interval_breaks1d(data, x)
+        y_intervals = conversion.infer_interval_breaks1d(data, y)
+        return Ugrid2d.from_structured_intervals1d(x_intervals, y_intervals)
+
+    @staticmethod
+    def from_structured_multicoord(
+        data: Union[xr.DataArray, xr.Dataset],
+        x: str,
+        y: str,
+    ) -> "Ugrid2d":
+        """
+        Create a Ugrid2d topology from a structured topology, including rotated
+        and (approximated) curvilinear topologies.
+
+        This method assumes the coordinates are 2D.
+
+        Use ``from_structured`` for 1D x and y coordinates, which is generally
+        the case for axis-aligned rectilinear topologies (most rasters).
+
+        Parameters
+        ----------
+        data: xr.DataArray or xr.Dataset
+        x: str
+            Name of the 2D coordinate to use as the UGRID x-coordinate.
+        y: str
+            Name of the 2D coordinate to use as the UGRID y-coordinate.
+
+        Returns
+        -------
+        grid: Ugrid2d
+        """
+        xv = conversion.infer_interval_breaks(data[x], axis=1, check_monotonic=True)
+        xv = conversion.infer_interval_breaks(xv, axis=0)
+        yv = conversion.infer_interval_breaks(data[y], axis=1)
+        yv = conversion.infer_interval_breaks(yv, axis=0, check_monotonic=True)
+        return Ugrid2d.from_structured_intervals2d(xv, yv)
 
     def to_shapely(self, dim):
         """
         Convert UGRID topology to shapely objects.
 
         * nodes: points
         * edges: linestrings
```

### Comparing `xugrid-0.8.1/xugrid/ugrid/ugridbase.py` & `xugrid-0.9.0/xugrid/ugrid/ugridbase.py`

 * *Files 3% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         pass
 
     @abc.abstractstaticmethod
     def from_dataset():
         pass
 
     @abc.abstractmethod
-    def to_dataset():
+    def to_dataset() -> xr.Dataset:
         pass
 
     @abc.abstractmethod
     def topology_subset():
         pass
 
     @abc.abstractmethod
@@ -268,19 +268,22 @@
 
     def __repr__(self):
         if self._dataset:
             return self._dataset.__repr__()
         else:
             return self.to_dataset().__repr__()
 
-    def equals(self, other):
-        if not isinstance(other, type(self)):
-            return False
-        # TODO: check values, etc.
-        return True
+    def equals(self, other) -> bool:
+        if other is self:
+            return True
+        elif isinstance(other, type(self)):
+            xr_self = self.to_dataset()
+            xr_other = other.to_dataset()
+            return xr_self.identical(xr_other)
+        return False
 
     def copy(self):
         """Create a deepcopy."""
         return copy.deepcopy(self)
 
     @property
     def attrs(self):
@@ -293,14 +296,26 @@
 
     @property
     def edge_dimension(self):
         """Name of edge dimension"""
         return self._attrs["edge_dimension"]
 
     @property
+    def max_connectivity_dimensions(self) -> tuple[str]:
+        return ()
+
+    @property
+    def max_connectivity_sizes(self) -> dict[str, int]:
+        return {}
+
+    @property
+    def sizes(self) -> dict[str, int]:
+        return self.dimensions
+
+    @property
     def node_coordinates(self) -> FloatArray:
         """Coordinates (x, y) of the nodes (vertices)"""
         return np.column_stack([self.node_x, self.node_y])
 
     @property
     def n_node(self) -> int:
         """Number of nodes (vertices) in the UGRID topology"""
@@ -382,29 +397,30 @@
     def _prepare_connectivity(
         da: xr.DataArray, fill_value: Union[float, int], dtype: type
     ) -> xr.DataArray:
         start_index = da.attrs.get("start_index", 0)
         if start_index not in (0, 1):
             raise ValueError(f"start_index should be 0 or 1, received: {start_index}")
 
-        data = da.to_numpy()
+        data = da.to_numpy().copy()
         # If xarray detects a _FillValue, it converts the array to floats and
         # replaces the fill value by NaN, and moves the _FillValue to
         # da.encoding.
         if "_FillValue" in da.attrs:
             is_fill = data == da.attrs["_FillValue"]
         else:
             is_fill = np.isnan(data)
+        # Set the fill_value before casting: otherwise the cast may fail.
         data[is_fill] = fill_value
+        cast = data.astype(dtype, copy=False)
 
-        cast = data.astype(dtype, copy=True)
+        not_fill = ~is_fill
         if start_index:
-            cast -= start_index
-        cast[is_fill] = fill_value
-        if (cast[~is_fill] < 0).any():
+            cast[not_fill] -= start_index
+        if (cast[not_fill] < 0).any():
             raise ValueError("connectivity contains negative values")
         return da.copy(data=cast)
 
     def _precheck(self, multi_index):
         dim, index = multi_index.popitem()
         for check_dim, check_index in multi_index.items():
             if not index.equals(check_index):
```

### Comparing `xugrid-0.8.1/xugrid/ugrid/voronoi.py` & `xugrid-0.9.0/xugrid/ugrid/voronoi.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.8.1/.gitignore` & `xugrid-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `xugrid-0.8.1/LICENSE` & `xugrid-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xugrid-0.8.1/README.rst` & `xugrid-0.9.0/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Xugrid
 ======
 
-.. image:: https://img.shields.io/github/actions/workflow/status/deltares/xugrid/ci.yml?style=flat-square
+.. image:: https://img.shields.io/github/actions/workflow/status/deltares/xugrid/ci.yml
    :target: https://github.com/deltares/xugrid/actions?query=workflows%3Aci
-.. image:: https://img.shields.io/codecov/c/github/deltares/xugrid.svg?style=flat-square
+.. image:: https://img.shields.io/codecov/c/github/deltares/xugrid.svg
    :target: https://app.codecov.io/gh/deltares/xugrid
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
+.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.10534099.svg
+  :target: https://doi.org/10.5281/zenodo.10534099
 
 **This is a work in progress.** `See documentation <https://deltares.github.io/xugrid/>`_.
 
 Xarray extension to work with 2D unstructured grids, for data and topology
 stored according to `UGRID conventions
 <https://ugrid-conventions.github.io/ugrid-conventions>`_.
```

### Comparing `xugrid-0.8.1/pyproject.toml` & `xugrid-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xugrid-0.8.1/PKG-INFO` & `xugrid-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xugrid
-Version: 0.8.1
+Version: 0.9.0
 Summary: Xarray extension for unstructured grids
 Project-URL: Home, https://github.com/deltares/xugrid
 Project-URL: Code, https://github.com/deltares/xugrid
 Project-URL: Issues, https://github.com/deltares/xugrid/issues
 Maintainer-email: Huite Bootsma <huite.bootsma@deltares.nl>
 License: MIT
 License-File: LICENSE
@@ -39,20 +39,22 @@
 Requires-Dist: shapely>=2.0; extra == 'all'
 Requires-Dist: zarr; extra == 'all'
 Description-Content-Type: text/x-rst
 
 Xugrid
 ======
 
-.. image:: https://img.shields.io/github/actions/workflow/status/deltares/xugrid/ci.yml?style=flat-square
+.. image:: https://img.shields.io/github/actions/workflow/status/deltares/xugrid/ci.yml
    :target: https://github.com/deltares/xugrid/actions?query=workflows%3Aci
-.. image:: https://img.shields.io/codecov/c/github/deltares/xugrid.svg?style=flat-square
+.. image:: https://img.shields.io/codecov/c/github/deltares/xugrid.svg
    :target: https://app.codecov.io/gh/deltares/xugrid
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
+.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.10534099.svg
+  :target: https://doi.org/10.5281/zenodo.10534099
 
 **This is a work in progress.** `See documentation <https://deltares.github.io/xugrid/>`_.
 
 Xarray extension to work with 2D unstructured grids, for data and topology
 stored according to `UGRID conventions
 <https://ugrid-conventions.github.io/ugrid-conventions>`_.
```

