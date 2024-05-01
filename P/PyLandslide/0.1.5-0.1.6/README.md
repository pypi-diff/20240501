# Comparing `tmp/PyLandslide-0.1.5.tar.gz` & `tmp/PyLandslide-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyLandslide-0.1.5.tar", last modified: Thu Apr 25 12:29:03 2024, max compression
+gzip compressed data, was "PyLandslide-0.1.6.tar", last modified: Wed May  1 20:40:42 2024, max compression
```

## Comparing `PyLandslide-0.1.5.tar` & `PyLandslide-0.1.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 12:29:03.980742 PyLandslide-0.1.5/
--rw-rw-rw-   0        0        0    35823 2023-12-01 01:14:16.000000 PyLandslide-0.1.5/LICENSE
--rw-rw-rw-   0        0        0     3939 2024-04-25 12:29:03.979745 PyLandslide-0.1.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-25 12:29:03.957819 PyLandslide-0.1.5/PyLandslide/
--rw-rw-rw-   0        0        0       54 2023-12-01 01:14:16.000000 PyLandslide-0.1.5/PyLandslide/__init__.py
--rw-rw-rw-   0        0        0     3980 2023-12-01 01:52:39.000000 PyLandslide-0.1.5/PyLandslide/cli.py
--rw-rw-rw-   0        0        0    12096 2024-04-25 12:21:45.000000 PyLandslide-0.1.5/PyLandslide/data_preparation.py
--rw-rw-rw-   0        0        0    14905 2023-12-01 01:14:16.000000 PyLandslide-0.1.5/PyLandslide/sensitivity.py
--rw-rw-rw-   0        0        0    10112 2023-12-01 01:14:16.000000 PyLandslide-0.1.5/PyLandslide/weightrange.py
-drwxrwxrwx   0        0        0        0 2024-04-25 12:29:03.970775 PyLandslide-0.1.5/PyLandslide.egg-info/
--rw-rw-rw-   0        0        0     3939 2024-04-25 12:29:03.000000 PyLandslide-0.1.5/PyLandslide.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      420 2024-04-25 12:29:03.000000 PyLandslide-0.1.5/PyLandslide.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 12:29:03.000000 PyLandslide-0.1.5/PyLandslide.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2024-04-25 12:29:03.000000 PyLandslide-0.1.5/PyLandslide.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       51 2024-04-25 12:29:03.000000 PyLandslide-0.1.5/PyLandslide.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-25 12:29:03.000000 PyLandslide-0.1.5/PyLandslide.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3082 2024-04-25 12:28:07.000000 PyLandslide-0.1.5/README.rst
--rw-rw-rw-   0        0        0       42 2024-04-25 12:29:03.982120 PyLandslide-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1183 2024-04-25 12:28:28.000000 PyLandslide-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-25 12:29:03.978749 PyLandslide-0.1.5/tests/
--rw-rw-rw-   0        0        0      101 2023-12-01 01:14:17.000000 PyLandslide-0.1.5/tests/test_sensitivity.py
--rw-rw-rw-   0        0        0     3572 2023-12-01 01:14:17.000000 PyLandslide-0.1.5/tests/test_weightrange.py
+drwxrwxrwx   0        0        0        0 2024-05-01 20:40:42.981228 PyLandslide-0.1.6/
+-rw-rw-rw-   0        0        0    35823 2023-12-01 01:14:16.000000 PyLandslide-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0     3648 2024-05-01 20:40:42.980231 PyLandslide-0.1.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-01 20:40:42.970669 PyLandslide-0.1.6/PyLandslide/
+-rw-rw-rw-   0        0        0       54 2023-12-01 01:14:16.000000 PyLandslide-0.1.6/PyLandslide/__init__.py
+-rw-rw-rw-   0        0        0     3980 2023-12-01 01:52:39.000000 PyLandslide-0.1.6/PyLandslide/cli.py
+-rw-rw-rw-   0        0        0    12096 2024-04-25 12:21:45.000000 PyLandslide-0.1.6/PyLandslide/data_preparation.py
+-rw-rw-rw-   0        0        0    14905 2023-12-01 01:14:16.000000 PyLandslide-0.1.6/PyLandslide/sensitivity.py
+-rw-rw-rw-   0        0        0    10112 2023-12-01 01:14:16.000000 PyLandslide-0.1.6/PyLandslide/weightrange.py
+drwxrwxrwx   0        0        0        0 2024-05-01 20:40:42.976244 PyLandslide-0.1.6/PyLandslide.egg-info/
+-rw-rw-rw-   0        0        0     3648 2024-05-01 20:40:42.000000 PyLandslide-0.1.6/PyLandslide.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      420 2024-05-01 20:40:42.000000 PyLandslide-0.1.6/PyLandslide.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 20:40:42.000000 PyLandslide-0.1.6/PyLandslide.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2024-05-01 20:40:42.000000 PyLandslide-0.1.6/PyLandslide.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       51 2024-05-01 20:40:42.000000 PyLandslide-0.1.6/PyLandslide.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-01 20:40:42.000000 PyLandslide-0.1.6/PyLandslide.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2791 2024-05-01 20:37:47.000000 PyLandslide-0.1.6/README.rst
+-rw-rw-rw-   0        0        0       42 2024-05-01 20:40:42.981228 PyLandslide-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1183 2024-05-01 20:39:36.000000 PyLandslide-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 20:40:42.979235 PyLandslide-0.1.6/tests/
+-rw-rw-rw-   0        0        0      101 2023-12-01 01:14:17.000000 PyLandslide-0.1.6/tests/test_sensitivity.py
+-rw-rw-rw-   0        0        0     3572 2023-12-01 01:14:17.000000 PyLandslide-0.1.6/tests/test_weightrange.py
```

### Comparing `PyLandslide-0.1.5/LICENSE` & `PyLandslide-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `PyLandslide-0.1.5/PKG-INFO` & `PyLandslide-0.1.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyLandslide
-Version: 0.1.5
+Version: 0.1.6
 Summary: Tool for landslide susceptibility mapping and uncertainty analysis.
 Home-page: https://github.com/WRHGroup/PyLandslide
 Author: Mohammed Basheer
 Author-email: mohammedadamabbaker@gmail.com
 License: GNU
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation :: PyPy
@@ -70,20 +70,18 @@
 .. code-block:: console
 
     python setup.py develop
 
 Citation
 ========
 
-Please cite the following papers when using PyLandslide:
+Please cite the following paper when using PyLandslide:
 
 
-    1. Basheer, M., Oommen, T., 2024. PyLandslide: A Python tool for landslide susceptibility mapping and uncertainty analysis. Environmental Modelling and Software. 106055. https://doi.org/10.1016/j.envsoft.2024.106055.
-    2. Basheer, M., Oommen, T., Takamatsu, M., Suzuki, S., 2022. Machine learning and sensitivity analysis approach to quantify uncertainty in landslide susceptibility mapping. Policy Research Working Paper, World Bank Group, Washington, D.C. https://doi.org/10.1596/1813-9450-10264.
-
+    Basheer, M., Oommen, T., 2024. PyLandslide: A Python tool for landslide susceptibility mapping and uncertainty analysis. Environmental Modelling and Software. 106055. https://doi.org/10.1016/j.envsoft.2024.106055.
 
 License
 =======
 
 Copyright (C) 2023, `Mohammed Basheer <https://scholar.google.com/citations?user=KM_oVpkAAAAJ&hl=en>`__ and `Thomas Oommen <https://scholar.google.com/citations?user=EP89cqIAAAAJ&hl=en>`__.
```

### Comparing `PyLandslide-0.1.5/PyLandslide/cli.py` & `PyLandslide-0.1.6/PyLandslide/cli.py`

 * *Files identical despite different names*

### Comparing `PyLandslide-0.1.5/PyLandslide/data_preparation.py` & `PyLandslide-0.1.6/PyLandslide/data_preparation.py`

 * *Files identical despite different names*

### Comparing `PyLandslide-0.1.5/PyLandslide/sensitivity.py` & `PyLandslide-0.1.6/PyLandslide/sensitivity.py`

 * *Files identical despite different names*

### Comparing `PyLandslide-0.1.5/PyLandslide/weightrange.py` & `PyLandslide-0.1.6/PyLandslide/weightrange.py`

 * *Files identical despite different names*

### Comparing `PyLandslide-0.1.5/PyLandslide.egg-info/PKG-INFO` & `PyLandslide-0.1.6/PyLandslide.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyLandslide
-Version: 0.1.5
+Version: 0.1.6
 Summary: Tool for landslide susceptibility mapping and uncertainty analysis.
 Home-page: https://github.com/WRHGroup/PyLandslide
 Author: Mohammed Basheer
 Author-email: mohammedadamabbaker@gmail.com
 License: GNU
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation :: PyPy
@@ -70,20 +70,18 @@
 .. code-block:: console
 
     python setup.py develop
 
 Citation
 ========
 
-Please cite the following papers when using PyLandslide:
+Please cite the following paper when using PyLandslide:
 
 
-    1. Basheer, M., Oommen, T., 2024. PyLandslide: A Python tool for landslide susceptibility mapping and uncertainty analysis. Environmental Modelling and Software. 106055. https://doi.org/10.1016/j.envsoft.2024.106055.
-    2. Basheer, M., Oommen, T., Takamatsu, M., Suzuki, S., 2022. Machine learning and sensitivity analysis approach to quantify uncertainty in landslide susceptibility mapping. Policy Research Working Paper, World Bank Group, Washington, D.C. https://doi.org/10.1596/1813-9450-10264.
-
+    Basheer, M., Oommen, T., 2024. PyLandslide: A Python tool for landslide susceptibility mapping and uncertainty analysis. Environmental Modelling and Software. 106055. https://doi.org/10.1016/j.envsoft.2024.106055.
 
 License
 =======
 
 Copyright (C) 2023, `Mohammed Basheer <https://scholar.google.com/citations?user=KM_oVpkAAAAJ&hl=en>`__ and `Thomas Oommen <https://scholar.google.com/citations?user=EP89cqIAAAAJ&hl=en>`__.
```

### Comparing `PyLandslide-0.1.5/README.rst` & `PyLandslide-0.1.6/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -46,20 +46,18 @@
 .. code-block:: console
 
     python setup.py develop
 
 Citation
 ========
 
-Please cite the following papers when using PyLandslide:
+Please cite the following paper when using PyLandslide:
 
 
-    1. Basheer, M., Oommen, T., 2024. PyLandslide: A Python tool for landslide susceptibility mapping and uncertainty analysis. Environmental Modelling and Software. 106055. https://doi.org/10.1016/j.envsoft.2024.106055.
-    2. Basheer, M., Oommen, T., Takamatsu, M., Suzuki, S., 2022. Machine learning and sensitivity analysis approach to quantify uncertainty in landslide susceptibility mapping. Policy Research Working Paper, World Bank Group, Washington, D.C. https://doi.org/10.1596/1813-9450-10264.
-
+    Basheer, M., Oommen, T., 2024. PyLandslide: A Python tool for landslide susceptibility mapping and uncertainty analysis. Environmental Modelling and Software. 106055. https://doi.org/10.1016/j.envsoft.2024.106055.
 
 License
 =======
 
 Copyright (C) 2023, `Mohammed Basheer <https://scholar.google.com/citations?user=KM_oVpkAAAAJ&hl=en>`__ and `Thomas Oommen <https://scholar.google.com/citations?user=EP89cqIAAAAJ&hl=en>`__.
```

### Comparing `PyLandslide-0.1.5/setup.py` & `PyLandslide-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.rst') as f:
     long_description = f.read()
 
 setup(
     name='PyLandslide',
-    version='0.1.5',
+    version='0.1.6',
     long_description=long_description,
     long_description_content_type="text/x-rst",
     description='Tool for landslide susceptibility mapping and uncertainty analysis.',
     url='https://github.com/WRHGroup/PyLandslide',
     author='Mohammed Basheer',
     author_email='mohammedadamabbaker@gmail.com',
     license='GNU',
```

### Comparing `PyLandslide-0.1.5/tests/test_weightrange.py` & `PyLandslide-0.1.6/tests/test_weightrange.py`

 * *Files identical despite different names*

