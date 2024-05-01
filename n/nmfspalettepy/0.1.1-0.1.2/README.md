# Comparing `tmp/nmfspalettepy-0.1.1.tar.gz` & `tmp/nmfspalettepy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nmfspalettepy-0.1.1.tar", last modified: Wed May  1 20:25:54 2024, max compression
+gzip compressed data, was "nmfspalettepy-0.1.2.tar", last modified: Wed May  1 20:28:54 2024, max compression
```

## Comparing `nmfspalettepy-0.1.1.tar` & `nmfspalettepy-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 20:25:54.184908 nmfspalettepy-0.1.1/
--rw-rw-rw-   0        0        0      523 2023-12-06 21:45:16.000000 nmfspalettepy-0.1.1/LICENSE.md
--rw-rw-rw-   0        0        0     3366 2024-05-01 20:25:54.169282 nmfspalettepy-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     3116 2024-05-01 20:12:45.000000 nmfspalettepy-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-01 20:25:54.160234 nmfspalettepy-0.1.1/nmfspalettepy/
--rw-rw-rw-   0        0        0      141 2024-05-01 19:42:52.000000 nmfspalettepy-0.1.1/nmfspalettepy/__init__.py
--rw-rw-rw-   0        0        0     1924 2024-05-01 19:34:30.000000 nmfspalettepy-0.1.1/nmfspalettepy/palettes.py
-drwxrwxrwx   0        0        0        0 2024-05-01 20:25:54.169282 nmfspalettepy-0.1.1/nmfspalettepy.egg-info/
--rw-rw-rw-   0        0        0     3366 2024-05-01 20:25:53.000000 nmfspalettepy-0.1.1/nmfspalettepy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2024-05-01 20:25:54.000000 nmfspalettepy-0.1.1/nmfspalettepy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 20:25:53.000000 nmfspalettepy-0.1.1/nmfspalettepy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-01 20:25:53.000000 nmfspalettepy-0.1.1/nmfspalettepy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-01 20:25:53.000000 nmfspalettepy-0.1.1/nmfspalettepy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-01 20:25:54.184908 nmfspalettepy-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      538 2024-05-01 20:25:50.000000 nmfspalettepy-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 20:28:54.132250 nmfspalettepy-0.1.2/
+-rw-rw-rw-   0        0        0      523 2023-12-06 21:45:16.000000 nmfspalettepy-0.1.2/LICENSE.md
+-rw-rw-rw-   0        0        0     3560 2024-05-01 20:28:54.132250 nmfspalettepy-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3310 2024-05-01 20:28:45.000000 nmfspalettepy-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-01 20:28:54.116624 nmfspalettepy-0.1.2/nmfspalettepy/
+-rw-rw-rw-   0        0        0      141 2024-05-01 19:42:52.000000 nmfspalettepy-0.1.2/nmfspalettepy/__init__.py
+-rw-rw-rw-   0        0        0     1924 2024-05-01 19:34:30.000000 nmfspalettepy-0.1.2/nmfspalettepy/palettes.py
+drwxrwxrwx   0        0        0        0 2024-05-01 20:28:54.132250 nmfspalettepy-0.1.2/nmfspalettepy.egg-info/
+-rw-rw-rw-   0        0        0     3560 2024-05-01 20:28:54.000000 nmfspalettepy-0.1.2/nmfspalettepy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2024-05-01 20:28:54.000000 nmfspalettepy-0.1.2/nmfspalettepy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 20:28:54.000000 nmfspalettepy-0.1.2/nmfspalettepy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-01 20:28:54.000000 nmfspalettepy-0.1.2/nmfspalettepy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-01 20:28:54.000000 nmfspalettepy-0.1.2/nmfspalettepy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-01 20:28:54.132250 nmfspalettepy-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      538 2024-05-01 20:27:32.000000 nmfspalettepy-0.1.2/setup.py
```

### Comparing `nmfspalettepy-0.1.1/LICENSE.md` & `nmfspalettepy-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nmfspalettepy-0.1.1/PKG-INFO` & `nmfspalettepy-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: nmfspalettepy
-Version: 0.1.1
+Version: 0.1.2
 Summary: NMFS color palettes handling library
 Author: Michael Akridge
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: numpy
 Requires-Dist: matplotlib
 
 # nmfspalettepy
 
-`nmfspalettepy` is a Python library designed to facilitate the use of National Marine Fisheries Service (NMFS) color palettes for data visualization projects. It provides easy access to a series of color schemes.
+`nmfspalettepy` is a Python library designed to facilitate the use of National Marine Fisheries Service (NMFS) color palettes for data visualization. It provides easy access to a series of NMFS color schemes.
+
+##Source:
+- view on Github: https://github.com/MichaelAkridge-NOAA/NOAA-NMFS-Brand-Resources/tree/nmfspalettepy
 
 ## Features
 
 - Provides a set of predefined color palettes using the NMFS color palettes.
 - Functions to display and utilize these palettes in visualizations.
 - Easy integration with matplotlib for creating custom color maps.
 
@@ -80,13 +83,13 @@
 
 ```
 ----------
 #### Disclaimer
 This repository is a scientific product and is not official communication of the National Oceanic and Atmospheric Administration, or the United States Department of Commerce. All NOAA GitHub project content is provided on an ‘as is’ basis and the user assumes responsibility for its use. Any claims against the Department of Commerce or Department of Commerce bureaus stemming from the use of this GitHub project will be governed by all applicable Federal law. Any reference to specific commercial products, processes, or services by service mark, trademark, manufacturer, or otherwise, does not constitute or imply their endorsement, recommendation or favoring by the Department of Commerce. The Department of Commerce seal and logo, or the seal and logo of a DOC bureau, shall not be used in any manner to imply endorsement of any commercial product or activity by DOC or the United States Government.
 
 ##### License
-See the [LICENSE.md](./LICENSE.md) for details
+See the [LICENSE.md](https://github.com/MichaelAkridge-NOAA/NOAA-NMFS-Brand-Resources/tree/nmfspalettepy/LICENSE.md) for details
 
 ##### Credits
 - Inspired by: 
    - https://github.com/nmfs-fish-tools/nmfspalette/
    - https://connect.fisheries.noaa.gov/colors/
```

### Comparing `nmfspalettepy-0.1.1/README.md` & `nmfspalettepy-0.1.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 # nmfspalettepy
 
-`nmfspalettepy` is a Python library designed to facilitate the use of National Marine Fisheries Service (NMFS) color palettes for data visualization projects. It provides easy access to a series of color schemes.
+`nmfspalettepy` is a Python library designed to facilitate the use of National Marine Fisheries Service (NMFS) color palettes for data visualization. It provides easy access to a series of NMFS color schemes.
+
+##Source:
+- view on Github: https://github.com/MichaelAkridge-NOAA/NOAA-NMFS-Brand-Resources/tree/nmfspalettepy
 
 ## Features
 
 - Provides a set of predefined color palettes using the NMFS color palettes.
 - Functions to display and utilize these palettes in visualizations.
 - Easy integration with matplotlib for creating custom color maps.
 
@@ -70,13 +73,13 @@
 
 ```
 ----------
 #### Disclaimer
 This repository is a scientific product and is not official communication of the National Oceanic and Atmospheric Administration, or the United States Department of Commerce. All NOAA GitHub project content is provided on an ‘as is’ basis and the user assumes responsibility for its use. Any claims against the Department of Commerce or Department of Commerce bureaus stemming from the use of this GitHub project will be governed by all applicable Federal law. Any reference to specific commercial products, processes, or services by service mark, trademark, manufacturer, or otherwise, does not constitute or imply their endorsement, recommendation or favoring by the Department of Commerce. The Department of Commerce seal and logo, or the seal and logo of a DOC bureau, shall not be used in any manner to imply endorsement of any commercial product or activity by DOC or the United States Government.
 
 ##### License
-See the [LICENSE.md](./LICENSE.md) for details
+See the [LICENSE.md](https://github.com/MichaelAkridge-NOAA/NOAA-NMFS-Brand-Resources/tree/nmfspalettepy/LICENSE.md) for details
 
 ##### Credits
 - Inspired by: 
    - https://github.com/nmfs-fish-tools/nmfspalette/
    - https://connect.fisheries.noaa.gov/colors/
```

### Comparing `nmfspalettepy-0.1.1/nmfspalettepy/palettes.py` & `nmfspalettepy-0.1.2/nmfspalettepy/palettes.py`

 * *Files identical despite different names*

### Comparing `nmfspalettepy-0.1.1/nmfspalettepy.egg-info/PKG-INFO` & `nmfspalettepy-0.1.2/nmfspalettepy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: nmfspalettepy
-Version: 0.1.1
+Version: 0.1.2
 Summary: NMFS color palettes handling library
 Author: Michael Akridge
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: numpy
 Requires-Dist: matplotlib
 
 # nmfspalettepy
 
-`nmfspalettepy` is a Python library designed to facilitate the use of National Marine Fisheries Service (NMFS) color palettes for data visualization projects. It provides easy access to a series of color schemes.
+`nmfspalettepy` is a Python library designed to facilitate the use of National Marine Fisheries Service (NMFS) color palettes for data visualization. It provides easy access to a series of NMFS color schemes.
+
+##Source:
+- view on Github: https://github.com/MichaelAkridge-NOAA/NOAA-NMFS-Brand-Resources/tree/nmfspalettepy
 
 ## Features
 
 - Provides a set of predefined color palettes using the NMFS color palettes.
 - Functions to display and utilize these palettes in visualizations.
 - Easy integration with matplotlib for creating custom color maps.
 
@@ -80,13 +83,13 @@
 
 ```
 ----------
 #### Disclaimer
 This repository is a scientific product and is not official communication of the National Oceanic and Atmospheric Administration, or the United States Department of Commerce. All NOAA GitHub project content is provided on an ‘as is’ basis and the user assumes responsibility for its use. Any claims against the Department of Commerce or Department of Commerce bureaus stemming from the use of this GitHub project will be governed by all applicable Federal law. Any reference to specific commercial products, processes, or services by service mark, trademark, manufacturer, or otherwise, does not constitute or imply their endorsement, recommendation or favoring by the Department of Commerce. The Department of Commerce seal and logo, or the seal and logo of a DOC bureau, shall not be used in any manner to imply endorsement of any commercial product or activity by DOC or the United States Government.
 
 ##### License
-See the [LICENSE.md](./LICENSE.md) for details
+See the [LICENSE.md](https://github.com/MichaelAkridge-NOAA/NOAA-NMFS-Brand-Resources/tree/nmfspalettepy/LICENSE.md) for details
 
 ##### Credits
 - Inspired by: 
    - https://github.com/nmfs-fish-tools/nmfspalette/
    - https://connect.fisheries.noaa.gov/colors/
```

### Comparing `nmfspalettepy-0.1.1/setup.py` & `nmfspalettepy-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of your README file
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='nmfspalettepy',
-    version='0.1.1',
+    version='0.1.2',
     description='NMFS color palettes handling library',
     long_description=long_description,
     long_description_content_type='text/markdown',  # This is important
     packages=['nmfspalettepy'],
     install_requires=[
         'numpy',
         'matplotlib'
```

