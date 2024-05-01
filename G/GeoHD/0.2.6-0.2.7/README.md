# Comparing `tmp/geohd-0.2.6.tar.gz` & `tmp/geohd-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geohd-0.2.6.tar", last modified: Thu Apr 18 19:20:01 2024, max compression
+gzip compressed data, was "geohd-0.2.7.tar", last modified: Wed May  1 13:43:11 2024, max compression
```

## Comparing `geohd-0.2.6.tar` & `geohd-0.2.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 19:20:01.832762 geohd-0.2.6/
-drwxrwxrwx   0        0        0        0 2024-04-18 19:20:01.823757 geohd-0.2.6/GeoHD/
--rw-rw-rw-   0        0        0    14398 2024-04-11 18:22:13.000000 geohd-0.2.6/GeoHD/AKDE.py
--rw-rw-rw-   0        0        0      161 2024-04-05 18:06:35.000000 geohd-0.2.6/GeoHD/__init__.py
--rw-rw-rw-   0        0        0     5330 2024-04-12 08:52:23.000000 geohd-0.2.6/GeoHD/analyze.py
--rw-rw-rw-   0        0        0     5860 2024-04-10 14:39:39.000000 geohd-0.2.6/GeoHD/process.py
--rw-rw-rw-   0        0        0    39256 2024-04-12 08:52:35.000000 geohd-0.2.6/GeoHD/utils.py
--rw-rw-rw-   0        0        0     2912 2024-04-05 18:31:26.000000 geohd-0.2.6/GeoHD/visualize.py
--rw-rw-rw-   0        0        0    10016 2024-04-12 08:52:35.000000 geohd-0.2.6/GeoHD/zone.py
-drwxrwxrwx   0        0        0        0 2024-04-18 19:20:01.830739 geohd-0.2.6/GeoHD.egg-info/
--rw-rw-rw-   0        0        0     5567 2024-04-18 19:20:01.000000 geohd-0.2.6/GeoHD.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      331 2024-04-18 19:20:01.000000 geohd-0.2.6/GeoHD.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 19:20:01.000000 geohd-0.2.6/GeoHD.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-04-18 19:20:01.000000 geohd-0.2.6/GeoHD.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-18 19:20:01.000000 geohd-0.2.6/GeoHD.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35182 2024-04-01 18:46:45.000000 geohd-0.2.6/LICENSE
--rw-rw-rw-   0        0        0     5567 2024-04-18 19:20:01.831760 geohd-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0     5071 2024-04-18 19:19:37.000000 geohd-0.2.6/README.md
--rw-rw-rw-   0        0        0       42 2024-04-18 19:20:01.832762 geohd-0.2.6/setup.cfg
--rw-rw-rw-   0        0        0      718 2024-04-18 19:19:37.000000 geohd-0.2.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-18 19:20:01.828747 geohd-0.2.6/test/
--rw-rw-rw-   0        0        0     2273 2024-04-12 09:42:46.000000 geohd-0.2.6/test/test_automation.py
-drwxrwxrwx   0        0        0        0 2024-04-18 19:20:01.829745 geohd-0.2.6/test_local/
--rw-rw-rw-   0        0        0        0 2024-04-01 18:50:35.000000 geohd-0.2.6/test_local/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 13:43:11.201589 geohd-0.2.7/
+drwxrwxrwx   0        0        0        0 2024-05-01 13:43:11.191918 geohd-0.2.7/GeoHD/
+-rw-rw-rw-   0        0        0    14398 2024-04-11 18:22:13.000000 geohd-0.2.7/GeoHD/AKDE.py
+-rw-rw-rw-   0        0        0      161 2024-04-05 18:06:35.000000 geohd-0.2.7/GeoHD/__init__.py
+-rw-rw-rw-   0        0        0     5330 2024-04-12 08:52:23.000000 geohd-0.2.7/GeoHD/analyze.py
+-rw-rw-rw-   0        0        0     5860 2024-04-10 14:39:39.000000 geohd-0.2.7/GeoHD/process.py
+-rw-rw-rw-   0        0        0    39256 2024-04-12 08:52:35.000000 geohd-0.2.7/GeoHD/utils.py
+-rw-rw-rw-   0        0        0     2912 2024-04-05 18:31:26.000000 geohd-0.2.7/GeoHD/visualize.py
+-rw-rw-rw-   0        0        0    10016 2024-04-12 08:52:35.000000 geohd-0.2.7/GeoHD/zone.py
+drwxrwxrwx   0        0        0        0 2024-05-01 13:43:11.196532 geohd-0.2.7/GeoHD.egg-info/
+-rw-rw-rw-   0        0        0     5903 2024-05-01 13:43:11.000000 geohd-0.2.7/GeoHD.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      331 2024-05-01 13:43:11.000000 geohd-0.2.7/GeoHD.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 13:43:11.000000 geohd-0.2.7/GeoHD.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-05-01 13:43:11.000000 geohd-0.2.7/GeoHD.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-01 13:43:11.000000 geohd-0.2.7/GeoHD.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35182 2024-04-01 18:46:45.000000 geohd-0.2.7/LICENSE
+-rw-rw-rw-   0        0        0     5903 2024-05-01 13:43:11.200509 geohd-0.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0     5407 2024-05-01 13:42:24.000000 geohd-0.2.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-01 13:43:11.201589 geohd-0.2.7/setup.cfg
+-rw-rw-rw-   0        0        0      718 2024-05-01 13:42:24.000000 geohd-0.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 13:43:11.196532 geohd-0.2.7/test/
+-rw-rw-rw-   0        0        0     2273 2024-04-12 09:42:46.000000 geohd-0.2.7/test/test_automation.py
+drwxrwxrwx   0        0        0        0 2024-05-01 13:43:11.196532 geohd-0.2.7/test_local/
+-rw-rw-rw-   0        0        0        0 2024-04-01 18:50:35.000000 geohd-0.2.7/test_local/__init__.py
```

### Comparing `geohd-0.2.6/GeoHD/AKDE.py` & `geohd-0.2.7/GeoHD/AKDE.py`

 * *Files identical despite different names*

### Comparing `geohd-0.2.6/GeoHD/analyze.py` & `geohd-0.2.7/GeoHD/analyze.py`

 * *Files identical despite different names*

### Comparing `geohd-0.2.6/GeoHD/process.py` & `geohd-0.2.7/GeoHD/process.py`

 * *Files identical despite different names*

### Comparing `geohd-0.2.6/GeoHD/utils.py` & `geohd-0.2.7/GeoHD/utils.py`

 * *Files identical despite different names*

### Comparing `geohd-0.2.6/GeoHD/visualize.py` & `geohd-0.2.7/GeoHD/visualize.py`

 * *Files identical despite different names*

### Comparing `geohd-0.2.6/GeoHD/zone.py` & `geohd-0.2.7/GeoHD/zone.py`

 * *Files identical despite different names*

### Comparing `geohd-0.2.6/GeoHD.egg-info/PKG-INFO` & `geohd-0.2.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,11 @@
-Metadata-Version: 2.1
-Name: GeoHD
-Version: 0.2.6
-Summary: A Python toolkit for geospatial hotspot detection, Avisualization, and analysis using urban data
-Home-page: https://github.com/yan-yuchen/GeoHD
-Author: Yuchen Yan
-Author-email: ycyan001@gmail.com
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy
-Requires-Dist: scipy
-Requires-Dist: matplotlib
-Requires-Dist: contextily
-Requires-Dist: geopandas
-Requires-Dist: pointpats
-Requires-Dist: h3
-
 # GeoHD
 
 ![python](https://img.shields.io/badge/python-3.11-black)
-![GitHub release](https://img.shields.io/badge/release-v0.2.6-blue)
+![GitHub release](https://img.shields.io/badge/release-v0.2.7-blue)
 ![pypi](https://img.shields.io/badge/pypi-v0.2.6-orange)
 ![license](https://img.shields.io/badge/license-GNU%20AGPLv3-green)
 
 [**Getting Started**](#getting-started)
 | [**Issues**](#issues)
 | [**Contribute**](#contribute)
 | [**Citation**](#citation)
@@ -145,12 +128,16 @@
 * Open an issue on the package [issue tracker](https://github.com/yan-yuchen/GeoHD/issues) clearly describing your intentions on code modifications or additions
 * Ensure your modifications or additions adhere to the existing standard of the GeoHD package, specifically detailed documentation for new methods (see existing methods for example documentation)
 * Test your modifications to ensure that the core functionality of the package has not been altered by running the unit tests 
 * Once the issue has been discussed with a package author, you may open a pull request containing your modifications
 
 ## Citation
 
+Yan, Y., 2024. GeoHD: A Python Toolkit for Geospatial Hotspot Detection, Visualization, and Analysis. SSRN Electron. J. https://doi.org/10.2139/ssrn.4799686
+
+Yan, Y., Quan, W., Wang, H., 2024. A data‐driven adaptive geospatial hotspot detection approach in smart cities. Trans. GIS tgis.13137. https://doi.org/10.1111/tgis.13137
+
 
 ## Authors
 
 * Yuchen Yan
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `geohd-0.2.6/LICENSE` & `geohd-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `geohd-0.2.6/PKG-INFO` & `geohd-0.2.7/GeoHD.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GeoHD
-Version: 0.2.6
+Version: 0.2.7
 Summary: A Python toolkit for geospatial hotspot detection, Avisualization, and analysis using urban data
 Home-page: https://github.com/yan-yuchen/GeoHD
 Author: Yuchen Yan
 Author-email: ycyan001@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
@@ -14,15 +14,15 @@
 Requires-Dist: geopandas
 Requires-Dist: pointpats
 Requires-Dist: h3
 
 # GeoHD
 
 ![python](https://img.shields.io/badge/python-3.11-black)
-![GitHub release](https://img.shields.io/badge/release-v0.2.6-blue)
+![GitHub release](https://img.shields.io/badge/release-v0.2.7-blue)
 ![pypi](https://img.shields.io/badge/pypi-v0.2.6-orange)
 ![license](https://img.shields.io/badge/license-GNU%20AGPLv3-green)
 
 [**Getting Started**](#getting-started)
 | [**Issues**](#issues)
 | [**Contribute**](#contribute)
 | [**Citation**](#citation)
@@ -145,12 +145,16 @@
 * Open an issue on the package [issue tracker](https://github.com/yan-yuchen/GeoHD/issues) clearly describing your intentions on code modifications or additions
 * Ensure your modifications or additions adhere to the existing standard of the GeoHD package, specifically detailed documentation for new methods (see existing methods for example documentation)
 * Test your modifications to ensure that the core functionality of the package has not been altered by running the unit tests 
 * Once the issue has been discussed with a package author, you may open a pull request containing your modifications
 
 ## Citation
 
+Yan, Y., 2024. GeoHD: A Python Toolkit for Geospatial Hotspot Detection, Visualization, and Analysis. SSRN Electron. J. https://doi.org/10.2139/ssrn.4799686
+
+Yan, Y., Quan, W., Wang, H., 2024. A data‐driven adaptive geospatial hotspot detection approach in smart cities. Trans. GIS tgis.13137. https://doi.org/10.1111/tgis.13137
+
 
 ## Authors
 
 * Yuchen Yan
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `geohd-0.2.6/README.md` & `geohd-0.2.7/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,28 @@
+Metadata-Version: 2.1
+Name: GeoHD
+Version: 0.2.7
+Summary: A Python toolkit for geospatial hotspot detection, Avisualization, and analysis using urban data
+Home-page: https://github.com/yan-yuchen/GeoHD
+Author: Yuchen Yan
+Author-email: ycyan001@gmail.com
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: matplotlib
+Requires-Dist: contextily
+Requires-Dist: geopandas
+Requires-Dist: pointpats
+Requires-Dist: h3
+
 # GeoHD
 
 ![python](https://img.shields.io/badge/python-3.11-black)
-![GitHub release](https://img.shields.io/badge/release-v0.2.6-blue)
+![GitHub release](https://img.shields.io/badge/release-v0.2.7-blue)
 ![pypi](https://img.shields.io/badge/pypi-v0.2.6-orange)
 ![license](https://img.shields.io/badge/license-GNU%20AGPLv3-green)
 
 [**Getting Started**](#getting-started)
 | [**Issues**](#issues)
 | [**Contribute**](#contribute)
 | [**Citation**](#citation)
@@ -128,12 +145,16 @@
 * Open an issue on the package [issue tracker](https://github.com/yan-yuchen/GeoHD/issues) clearly describing your intentions on code modifications or additions
 * Ensure your modifications or additions adhere to the existing standard of the GeoHD package, specifically detailed documentation for new methods (see existing methods for example documentation)
 * Test your modifications to ensure that the core functionality of the package has not been altered by running the unit tests 
 * Once the issue has been discussed with a package author, you may open a pull request containing your modifications
 
 ## Citation
 
+Yan, Y., 2024. GeoHD: A Python Toolkit for Geospatial Hotspot Detection, Visualization, and Analysis. SSRN Electron. J. https://doi.org/10.2139/ssrn.4799686
+
+Yan, Y., Quan, W., Wang, H., 2024. A data‐driven adaptive geospatial hotspot detection approach in smart cities. Trans. GIS tgis.13137. https://doi.org/10.1111/tgis.13137
+
 
 ## Authors
 
 * Yuchen Yan
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `geohd-0.2.6/setup.py` & `geohd-0.2.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='GeoHD',
-    version='0.2.6',
+    version='0.2.7',
     description='A Python toolkit for geospatial hotspot detection, Avisualization, and analysis using urban data',
     author='Yuchen Yan',
     author_email='ycyan001@gmail.com',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/yan-yuchen/GeoHD",    
     packages=find_packages(),
```

### Comparing `geohd-0.2.6/test/test_automation.py` & `geohd-0.2.7/test/test_automation.py`

 * *Files identical despite different names*

