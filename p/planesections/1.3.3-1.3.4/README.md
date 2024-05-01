# Comparing `tmp/planesections-1.3.3.tar.gz` & `tmp/planesections-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "planesections-1.3.3.tar", last modified: Sun Feb 18 23:20:46 2024, max compression
+gzip compressed data, was "planesections-1.3.4.tar", last modified: Wed May  1 07:50:08 2024, max compression
```

## Comparing `planesections-1.3.3.tar` & `planesections-1.3.4.tar`

### file list

```diff
@@ -1,39 +1,57 @@
-drwxrwxrwx   0        0        0        0 2024-02-18 23:20:46.351383 planesections-1.3.3/
--rw-rw-rw-   0        0        0     3817 2024-02-18 23:20:46.350874 planesections-1.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     3317 2022-07-04 01:05:38.000000 planesections-1.3.3/README.md
--rw-rw-rw-   0        0        0     1096 2022-06-22 08:25:47.000000 planesections-1.3.3/license.txt
-drwxrwxrwx   0        0        0        0 2024-02-18 23:20:46.271312 planesections-1.3.3/planesections/
--rw-rw-rw-   0        0        0     1052 2024-02-10 23:48:48.000000 planesections-1.3.3/planesections/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-18 23:20:46.301312 planesections-1.3.3/planesections/analysis/
--rw-rw-rw-   0        0        0      244 2024-02-10 23:48:48.000000 planesections-1.3.3/planesections/analysis/__init__.py
--rw-rw-rw-   0        0        0    15560 2024-02-10 23:48:48.000000 planesections-1.3.3/planesections/analysis/openSees.py
--rw-rw-rw-   0        0        0    10359 2024-02-10 23:48:48.000000 planesections-1.3.3/planesections/analysis/pynite.py
--rw-rw-rw-   0        0        0      225 2024-02-10 23:48:48.000000 planesections-1.3.3/planesections/analysis/recorder.py
--rw-rw-rw-   0        0        0    50457 2024-02-18 22:54:37.000000 planesections-1.3.3/planesections/builder.py
-drwxrwxrwx   0        0        0        0 2024-02-18 23:20:46.310312 planesections-1.3.3/planesections/diagram/
--rw-rw-rw-   0        0        0      188 2024-02-10 23:48:48.000000 planesections-1.3.3/planesections/diagram/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-18 23:20:46.327310 planesections-1.3.3/planesections/diagram/components/
--rw-rw-rw-   0        0        0        0 2024-02-10 23:48:48.000000 planesections-1.3.3/planesections/diagram/components/__init__.py
--rw-rw-rw-   0        0        0     3121 2024-02-10 23:48:48.000000 planesections-1.3.3/planesections/diagram/components/abstract.py
--rw-rw-rw-   0        0        0    22746 2024-02-18 23:17:12.000000 planesections-1.3.3/planesections/diagram/components/basic.py
--rw-rw-rw-   0        0        0    14760 2024-02-10 23:48:48.000000 planesections-1.3.3/planesections/diagram/components/basic_old.py
--rw-rw-rw-   0        0        0    29815 2024-02-10 23:48:48.000000 planesections-1.3.3/planesections/diagram/diagram.py
--rw-rw-rw-   0        0        0     4855 2024-02-10 23:48:48.000000 planesections-1.3.3/planesections/environment.py
-drwxrwxrwx   0        0        0        0 2024-02-18 23:20:46.345311 planesections-1.3.3/planesections/postprocess/
--rw-rw-rw-   0        0        0      240 2024-02-10 23:48:48.000000 planesections-1.3.3/planesections/postprocess/__init__.py
--rw-rw-rw-   0        0        0     2367 2024-02-10 23:48:48.000000 planesections-1.3.3/planesections/postprocess/parse.py
--rw-rw-rw-   0        0        0    16291 2024-02-18 23:11:56.000000 planesections-1.3.3/planesections/postprocess/plot.py
--rw-rw-rw-   0        0        0     8914 2024-02-10 23:48:48.000000 planesections-1.3.3/planesections/postprocess/poi.py
--rw-rw-rw-   0        0        0     1902 2024-02-10 23:48:48.000000 planesections-1.3.3/planesections/section.py
-drwxrwxrwx   0        0        0        0 2024-02-18 23:20:46.349383 planesections-1.3.3/planesections/units/
--rw-rw-rw-   0        0        0        0 2024-02-10 23:48:48.000000 planesections-1.3.3/planesections/units/__init__.py
--rw-rw-rw-   0        0        0     1490 2024-02-10 23:48:48.000000 planesections-1.3.3/planesections/units/diagramUnits.py
--rw-rw-rw-   0        0        0      113 2024-02-10 23:48:48.000000 planesections-1.3.3/planesections/units/metric.py
-drwxrwxrwx   0        0        0        0 2024-02-18 23:20:46.284311 planesections-1.3.3/planesections.egg-info/
--rw-rw-rw-   0        0        0     3817 2024-02-18 23:20:45.000000 planesections-1.3.3/planesections.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      940 2024-02-18 23:20:46.000000 planesections-1.3.3/planesections.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-18 23:20:45.000000 planesections-1.3.3/planesections.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2024-02-18 23:20:45.000000 planesections-1.3.3/planesections.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-02-18 23:20:45.000000 planesections-1.3.3/planesections.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-18 23:20:46.351383 planesections-1.3.3/setup.cfg
--rw-rw-rw-   0        0        0      872 2024-02-18 23:20:00.000000 planesections-1.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 07:50:08.727409 planesections-1.3.4/
+-rw-rw-rw-   0        0        0    11558 2021-07-09 06:59:36.000000 planesections-1.3.4/LICENSE
+-rw-rw-rw-   0        0        0    18849 2024-05-01 07:50:08.726399 planesections-1.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4278 2024-02-18 23:44:40.000000 planesections-1.3.4/README.md
+-rw-rw-rw-   0        0        0     1529 2024-05-01 07:49:19.000000 planesections-1.3.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-01 07:50:08.727999 planesections-1.3.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-01 07:50:08.447170 planesections-1.3.4/src/
+drwxrwxrwx   0        0        0        0 2024-05-01 07:50:08.484456 planesections-1.3.4/src/planesections/
+-rw-rw-rw-   0        0        0     1052 2024-04-27 22:14:07.000000 planesections-1.3.4/src/planesections/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 07:50:08.533294 planesections-1.3.4/src/planesections/analysis/
+-rw-rw-rw-   0        0        0      244 2024-04-27 22:14:07.000000 planesections-1.3.4/src/planesections/analysis/__init__.py
+-rw-rw-rw-   0        0        0    15560 2024-04-27 22:14:07.000000 planesections-1.3.4/src/planesections/analysis/openSees.py
+-rw-rw-rw-   0        0        0    10359 2024-04-27 22:14:07.000000 planesections-1.3.4/src/planesections/analysis/pynite.py
+-rw-rw-rw-   0        0        0      225 2024-04-27 22:14:07.000000 planesections-1.3.4/src/planesections/analysis/recorder.py
+-rw-rw-rw-   0        0        0    50457 2024-04-27 22:14:07.000000 planesections-1.3.4/src/planesections/builder.py
+drwxrwxrwx   0        0        0        0 2024-05-01 07:50:08.546408 planesections-1.3.4/src/planesections/diagram/
+-rw-rw-rw-   0        0        0      188 2024-04-27 22:14:07.000000 planesections-1.3.4/src/planesections/diagram/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 07:50:08.570080 planesections-1.3.4/src/planesections/diagram/components/
+-rw-rw-rw-   0        0        0        0 2024-04-27 22:14:07.000000 planesections-1.3.4/src/planesections/diagram/components/__init__.py
+-rw-rw-rw-   0        0        0     3121 2024-04-27 22:14:07.000000 planesections-1.3.4/src/planesections/diagram/components/abstract.py
+-rw-rw-rw-   0        0        0    22746 2024-04-27 22:14:07.000000 planesections-1.3.4/src/planesections/diagram/components/basic.py
+-rw-rw-rw-   0        0        0    14760 2024-04-27 22:14:07.000000 planesections-1.3.4/src/planesections/diagram/components/basic_old.py
+-rw-rw-rw-   0        0        0    29815 2024-04-27 22:14:07.000000 planesections-1.3.4/src/planesections/diagram/diagram.py
+-rw-rw-rw-   0        0        0     4855 2024-04-27 22:14:07.000000 planesections-1.3.4/src/planesections/environment.py
+drwxrwxrwx   0        0        0        0 2024-05-01 07:50:08.599382 planesections-1.3.4/src/planesections/postprocess/
+-rw-rw-rw-   0        0        0      240 2024-04-27 22:14:07.000000 planesections-1.3.4/src/planesections/postprocess/__init__.py
+-rw-rw-rw-   0        0        0     2367 2024-04-27 22:14:07.000000 planesections-1.3.4/src/planesections/postprocess/parse.py
+-rw-rw-rw-   0        0        0    16291 2024-04-27 22:14:07.000000 planesections-1.3.4/src/planesections/postprocess/plot.py
+-rw-rw-rw-   0        0        0     8914 2024-04-27 22:14:07.000000 planesections-1.3.4/src/planesections/postprocess/poi.py
+-rw-rw-rw-   0        0        0     1902 2024-04-27 22:14:07.000000 planesections-1.3.4/src/planesections/section.py
+drwxrwxrwx   0        0        0        0 2024-05-01 07:50:08.614813 planesections-1.3.4/src/planesections/units/
+-rw-rw-rw-   0        0        0        0 2024-04-27 22:14:07.000000 planesections-1.3.4/src/planesections/units/__init__.py
+-rw-rw-rw-   0        0        0     1490 2024-04-27 22:14:07.000000 planesections-1.3.4/src/planesections/units/diagramUnits.py
+-rw-rw-rw-   0        0        0      113 2024-04-27 22:14:07.000000 planesections-1.3.4/src/planesections/units/metric.py
+drwxrwxrwx   0        0        0        0 2024-05-01 07:50:08.724399 planesections-1.3.4/src/planesections.egg-info/
+-rw-rw-rw-   0        0        0    18849 2024-05-01 07:50:08.000000 planesections-1.3.4/src/planesections.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1472 2024-05-01 07:50:08.000000 planesections-1.3.4/src/planesections.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 07:50:08.000000 planesections-1.3.4/src/planesections.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2024-05-01 07:50:08.000000 planesections-1.3.4/src/planesections.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       49 2024-05-01 07:50:08.000000 planesections-1.3.4/src/planesections.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-01 07:50:08.723400 planesections-1.3.4/test/
+-rw-rw-rw-   0        0        0     1169 2023-07-16 02:20:31.000000 planesections-1.3.4/test/test_Beam_3D.py
+-rw-rw-rw-   0        0        0     1240 2023-07-16 02:15:58.000000 planesections-1.3.4/test/test_Beam_PointLoad_IDs.py
+-rw-rw-rw-   0        0        0      717 2023-09-02 23:05:55.000000 planesections-1.3.4/test/test_Node.py
+-rw-rw-rw-   0        0        0     4842 2023-07-16 02:21:50.000000 planesections-1.3.4/test/test_builder.py
+-rw-rw-rw-   0        0        0      669 2023-12-28 00:40:25.000000 planesections-1.3.4/test/test_builder_loads_linear.py
+-rw-rw-rw-   0        0        0     5808 2023-12-28 00:40:25.000000 planesections-1.3.4/test/test_diagram_box_normalization.py
+-rw-rw-rw-   0        0        0      965 2023-12-28 00:40:25.000000 planesections-1.3.4/test/test_diagram_box_overlap.py
+-rw-rw-rw-   0        0        0     3575 2023-12-28 00:40:25.000000 planesections-1.3.4/test/test_diagram_box_stacking.py
+-rw-rw-rw-   0        0        0     2620 2023-12-28 00:40:25.000000 planesections-1.3.4/test/test_diagram_boxes.py
+-rw-rw-rw-   0        0        0      976 2022-08-08 05:23:52.000000 planesections-1.3.4/test/test_diagram_labels.py
+-rw-rw-rw-   0        0        0     1318 2022-08-08 05:23:52.000000 planesections-1.3.4/test/test_diagram_units.py
+-rw-rw-rw-   0        0        0     1303 2023-07-16 01:31:42.000000 planesections-1.3.4/test/test_fixities.py
+-rw-rw-rw-   0        0        0      968 2024-01-04 06:06:14.000000 planesections-1.3.4/test/test_imports.py
+-rw-rw-rw-   0        0        0     2479 2022-08-08 05:23:52.000000 planesections-1.3.4/test/test_labeling.py
+-rw-rw-rw-   0        0        0     1833 2024-02-10 23:08:06.000000 planesections-1.3.4/test/test_poi.py
+-rw-rw-rw-   0        0        0     3001 2022-07-17 02:38:06.000000 planesections-1.3.4/test/test_units_diagramEnv.py
```

### Comparing `planesections-1.3.3/PKG-INFO` & `planesections-1.3.4/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,61 +1,66 @@
-Metadata-Version: 2.1
-Name: planesections
-Version: 1.3.3
-Summary: A light-weight FEM beam analyzer.
-Home-page: https://github.com/cslotboom/planesections
-Author: Christian Slotboom
-Author-email: christian.slotboom@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: opensees
-License-File: license.txt
-
 # PlaneSections
-A lightweight beam bending library built on [OpenSeesPy](https://github.com/zhuminjie/OpenSeesPy).
+<p align="center">
+  <img src="doc/img/Beam Image.png" width="500">
+</p>
+
+A lightweight finite element beam bending library built on libraries like [PyNite](https://github.com/JWock82/PyNite) and [OpenSeesPy](https://github.com/zhuminjie/OpenSeesPy).
 The goal of PlaneSections is to make easy-to-use beam anayses, which can be used to quickly document structural calculations.
-Being built on OpenSees, the structural results are reliable, and there is lots of room to build more complex models.
 
-The core classes and API are complete, but development is still in progress. Expect some sytax changes before final release, however deprication warnings
-will be given for breaking changes.
 
 **NOTE:**
 Units for force and length must be applied to the beam in a [consistent unit base for FEM](https://femci.gsfc.nasa.gov/units/index.html).
 PlaneSections has been design with Metric units in mind in terms of scaling diagrams. For those using imperial units, results will work with a consitent unit basis, but the scale of the digrams may be off.
 
+PlaneSections is a FEM solver! Results are only stored at nodes specified by the user - all intermediate values in plots are linearly interpolated.
+
 ## Contents
 * [Installation](https://github.com/cslotboom/planesections#Installation)
+* [Features](https://github.com/cslotboom/planesections#Features)
 * [Documentation](https://github.com/cslotboom/planesections#Documentation)
 * [Demo](https://github.com/cslotboom/planesections#Demo)
+* [Coordinates](https://github.com/cslotboom/planesections#Coordinates)
+* [Solvers](https://github.com/cslotboom/planesections#Solvers)
 * [Work Status](https://github.com/cslotboom/planesections#Status)
 
 
 ## Installation
-Package is installable through pip
+The default package is installable through pip.
 ```
-pip install planesections
+pip -m install planesections
+
+```
+The package with the optional OpenSeesPy dependancy is installable with 
+```
+pip -m install planesections[opensees]
+
 ```
 
+## Features:
+2D and 3D beams can be anayzed under the following force types:
+- Point loads
+- Point Moments
+- Line Element loads
+- Linearly varying element loads (2D only).
+
+Diagrams can also be made of 2D beams, but the support types that can be plotted are limited.
+
 ## Documentation
 All major functions and classes are documented on read-the-docs: https://planesections.readthedocs.io/en/latest/
 
 ## Demo
-The PlaneSections can plot representations that can be used in documentation.
-It's also possible to get the output bening moment, shear force, rotation, and deflection diagrams.
+The PlaneSections can analyze and document beam plots for calcualtions. Below we make a beam, create a diagram of it, then get the output bending moment and shear force diagrams. It's also possible to get rotation, and deflection diagrams but these are not shown here.
 
 ``` Python
 
 import planesections as ps
 
 # Define node locations, and support conditions
 L = 5
-beam = ps.newEulerBeam2D(L)
+beam = ps.newEulerBeam(L)
 
 # Define beam and fixities
 pinned = [1,1,0]
 beam.setFixity(L*0.1, pinned, label = '1')
 beam.setFixity(L*0.9, pinned)
 
 # Define loads
@@ -66,57 +71,49 @@
 beam.addDistLoadVertical(0, L, Pz)
 beam.addDistLoadVertical(1, L*0.3, 5*Pz)
 
 # Plot the beam diagram
 ps.plotBeamDiagram(beam)
 
 # Run the analysis
-analysis = ps.OpenSeesAnalyzer2D(beam)
+analysis = ps.PyNiteAnalyzer2D(beam)
 analysis.runAnalysis()
 
 # Plot the SFD and BMD
-ps.plotShear2D(beam)
-ps.plotMoment2D(beam)
+ps.plotShear(beam)
+ps.plotMoment(beam)
 ```
 
+<p align="center">
+  <img src="doc/img/Beam-Image-2.png" width="500">
+</p>
+<p align="center">
+  <img src="doc/img/Beam-Image-2-SFD.png" width="500">
+</p>  
+<p align="center">
+  <img src="doc/img/Beam-Image-2-BMD.png" width="500">
+</p>  
+
+## Coordinates
+The coordinant system used for beams is as follows:
+<p align="center">
+  <img src="doc/img/coords/forces.JPG" width="700">
+</p>
 
-## Further Examples
-See the examples folder for
 
+## Further Examples
+See the examples folder for more examples!
 
-## Status
-Before the first beta release, the following will be completed.
+## Solvers
+The opensees solver is included as an optional dependancy. It is significantly faster than the PyNite solver (~100x), but the license is more limited in use. OpenSees allows commercial use of the package, but does not allow resale without permission, so use at your own risk! [OpenSees License.](https://opensees.github.io/OpenSeesDocumentation/developer/license.html)
 
-*Analysis and API*:
-- [x] fancy plots (distributed Load)
-- [x] Better deflection plots (distributed Load)
-
-*Infacstructure*:
-- [x] pip package
-  - [x] setup on pypi: complete, package is installable with "pip install planesections"
-  - [x] Add requirements
-- [x] Document code
-  - [x] Finish all class docstrings.
-  - [x] Add Sphinx docs.
-  - [x] Add read the docs website.
-- [ ] Examples
-  - [ ] Finish landing page with code examples and figures.
-  - [ ] Compare simple cases with analytic equations.
-  - [ ] Compare complex cases with sap/rfem/etc.
-
-
-# Post 1.0 release
-*Analysis and API*:
-- [ ] plot labels
+Some restrictions exist for OpenSees license, so this library has been added as an optional dependancy
 
 
+## Status
+PlaneSections is almost "feature complete" in terms of it's analysis functionality. The only additional analysis features I might include are:
+- Spring supports
+- Internal hinges
+- Better cross section support
+These are not slated to be in the next release.
 
-Future work:
- - 3D beams
- - Timoshenko beams
- - Nonlinear beams analysis
- - One-way Slabs?
- - Two-way Slabs?
- - Orthtropic Slabs?
- - Basic simple frame analysis?
- - Basic Nonlinear frame analysis?
```

### Comparing `planesections-1.3.3/planesections/__init__.py` & `planesections-1.3.4/src/planesections/__init__.py`

 * *Files identical despite different names*

### Comparing `planesections-1.3.3/planesections/analysis/openSees.py` & `planesections-1.3.4/src/planesections/analysis/openSees.py`

 * *Files identical despite different names*

### Comparing `planesections-1.3.3/planesections/analysis/pynite.py` & `planesections-1.3.4/src/planesections/analysis/pynite.py`

 * *Files identical despite different names*

### Comparing `planesections-1.3.3/planesections/builder.py` & `planesections-1.3.4/src/planesections/builder.py`

 * *Files identical despite different names*

### Comparing `planesections-1.3.3/planesections/diagram/components/abstract.py` & `planesections-1.3.4/src/planesections/diagram/components/abstract.py`

 * *Files identical despite different names*

### Comparing `planesections-1.3.3/planesections/diagram/components/basic.py` & `planesections-1.3.4/src/planesections/diagram/components/basic.py`

 * *Files identical despite different names*

### Comparing `planesections-1.3.3/planesections/diagram/components/basic_old.py` & `planesections-1.3.4/src/planesections/diagram/components/basic_old.py`

 * *Files identical despite different names*

### Comparing `planesections-1.3.3/planesections/diagram/diagram.py` & `planesections-1.3.4/src/planesections/diagram/diagram.py`

 * *Files identical despite different names*

### Comparing `planesections-1.3.3/planesections/environment.py` & `planesections-1.3.4/src/planesections/environment.py`

 * *Files identical despite different names*

### Comparing `planesections-1.3.3/planesections/postprocess/parse.py` & `planesections-1.3.4/src/planesections/postprocess/parse.py`

 * *Files identical despite different names*

### Comparing `planesections-1.3.3/planesections/postprocess/plot.py` & `planesections-1.3.4/src/planesections/postprocess/plot.py`

 * *Files identical despite different names*

### Comparing `planesections-1.3.3/planesections/postprocess/poi.py` & `planesections-1.3.4/src/planesections/postprocess/poi.py`

 * *Files identical despite different names*

### Comparing `planesections-1.3.3/planesections/section.py` & `planesections-1.3.4/src/planesections/section.py`

 * *Files identical despite different names*

### Comparing `planesections-1.3.3/planesections/units/diagramUnits.py` & `planesections-1.3.4/src/planesections/units/diagramUnits.py`

 * *Files identical despite different names*

