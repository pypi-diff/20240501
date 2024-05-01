# Comparing `tmp/FoundationDesign-0.0.6.tar.gz` & `tmp/FoundationDesign-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FoundationDesign-0.0.6.tar", last modified: Fri Dec 29 18:15:06 2023, max compression
+gzip compressed data, was "FoundationDesign-0.0.7.tar", last modified: Wed May  1 20:09:07 2024, max compression
```

## Comparing `FoundationDesign-0.0.6.tar` & `FoundationDesign-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-12-29 18:15:06.336136 FoundationDesign-0.0.6/
-drwxrwxrwx   0        0        0        0 2023-12-29 18:15:06.322320 FoundationDesign-0.0.6/FoundationDesign/
--rw-rw-rw-   0        0        0      604 2023-11-25 12:38:34.000000 FoundationDesign-0.0.6/FoundationDesign/__init__.py
--rw-rw-rw-   0        0        0   158675 2023-11-25 12:38:34.000000 FoundationDesign-0.0.6/FoundationDesign/combinedfootingdesign.py
--rw-rw-rw-   0        0        0     6850 2023-12-29 18:12:48.000000 FoundationDesign-0.0.6/FoundationDesign/concretedesignfunc.py
--rw-rw-rw-   0        0        0     2605 2023-11-25 12:38:34.000000 FoundationDesign-0.0.6/FoundationDesign/datavalidation.py
--rw-rw-rw-   0        0        0    98922 2023-12-28 08:30:25.000000 FoundationDesign-0.0.6/FoundationDesign/foundationdesign.py
-drwxrwxrwx   0        0        0        0 2023-12-29 18:15:06.332292 FoundationDesign-0.0.6/FoundationDesign.egg-info/
--rw-rw-rw-   0        0        0     7073 2023-12-29 18:15:06.000000 FoundationDesign-0.0.6/FoundationDesign.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      407 2023-12-29 18:15:06.000000 FoundationDesign-0.0.6/FoundationDesign.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-29 18:15:06.000000 FoundationDesign-0.0.6/FoundationDesign.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-12-29 18:15:06.000000 FoundationDesign-0.0.6/FoundationDesign.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-12-29 18:15:06.000000 FoundationDesign-0.0.6/FoundationDesign.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1087 2023-11-25 12:38:34.000000 FoundationDesign-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     7073 2023-12-29 18:15:06.335084 FoundationDesign-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     6589 2023-11-26 22:13:13.000000 FoundationDesign-0.0.6/README.md
--rw-rw-rw-   0        0        0       42 2023-12-29 18:15:06.337130 FoundationDesign-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      898 2023-12-29 18:14:08.000000 FoundationDesign-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 20:09:07.287370 FoundationDesign-0.0.7/
+drwxrwxrwx   0        0        0        0 2024-05-01 20:09:07.283381 FoundationDesign-0.0.7/FoundationDesign.egg-info/
+-rw-rw-rw-   0        0        0     7653 2024-05-01 20:09:07.000000 FoundationDesign-0.0.7/FoundationDesign.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      316 2024-05-01 20:09:07.000000 FoundationDesign-0.0.7/FoundationDesign.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 20:09:07.000000 FoundationDesign-0.0.7/FoundationDesign.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-05-01 20:09:07.000000 FoundationDesign-0.0.7/FoundationDesign.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 20:09:07.000000 FoundationDesign-0.0.7/FoundationDesign.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1089 2024-04-29 21:30:46.000000 FoundationDesign-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     7653 2024-05-01 20:09:07.285376 FoundationDesign-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     7010 2024-05-01 18:34:26.000000 FoundationDesign-0.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-01 20:09:07.287370 FoundationDesign-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      981 2024-05-01 19:02:28.000000 FoundationDesign-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 20:09:07.279392 FoundationDesign-0.0.7/tests/
+-rw-rw-rw-   0        0        0     2382 2024-04-29 21:31:05.000000 FoundationDesign-0.0.7/tests/test.py
+-rw-rw-rw-   0        0        0     1187 2024-04-06 14:37:43.000000 FoundationDesign-0.0.7/tests/test2.py
+-rw-rw-rw-   0        0        0     3110 2024-05-01 17:30:05.000000 FoundationDesign-0.0.7/tests/test_PadFoundation.py
+-rw-rw-rw-   0        0        0     5573 2024-05-01 16:08:17.000000 FoundationDesign-0.0.7/tests/test_PadFoundationDesign.py
```

### Comparing `FoundationDesign-0.0.6/FoundationDesign.egg-info/PKG-INFO` & `FoundationDesign-0.0.7/FoundationDesign.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 Metadata-Version: 2.1
 Name: FoundationDesign
-Version: 0.0.6
-Summary:  A python module for structural analysis and design of different foundation type in accordance to the Eurocodes
+Version: 0.0.7
+Summary: A python module for structural analysis and design of different foundation types in accordance to the Eurocodes
+Home-page: https://github.com/kunle009/FoundationDesign
 Author: Kunle Yusuf
 Author-email: kunleyusuf858@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: indeterminatebeam==2.2.1
+Requires-Dist: numpy==1.24.4
+Requires-Dist: plotly==5.15.0
 
 
 # FoundationDesign
 
 [![PyPi](https://img.shields.io/pypi/v/FoundationDesign.svg)](https://pypi.org/project/FoundationDesign/)
 ![PyPI - License](https://img.shields.io/pypi/l/FoundationDesign)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/FoundationDesign)
+[![Downloads](https://static.pepy.tech/badge/foundationdesign)](https://pepy.tech/project/foundationdesign)
+[![Downloads](https://static.pepy.tech/badge/foundationdesign/month)](https://pepy.tech/project/foundationdesign)
+[![build & test](https://github.com/kunle009/FoundationDesign/actions/workflows/build-and-test.yml/badge.svg?branch=main)](https://github.com/kunle009/FoundationDesign/actions/workflows/build-and-test.yml)
 
 
 FoundationDesign is a python module to be used for the design and analysis
 of different foundation types in accordance to the Eurocode 2.
 This project is an attempt to have a free standalone python package that can
 be used to analyse and design foundations with results as good as paid softwares.
 This module will be useful in determining:
@@ -118,17 +124,17 @@
 Lots of checks can be done on the Foundation which can be found in the notebooks contained in the examples folder
 To show the bending moment of the Foundation. The ```plot_bending_moment_X()``` can be called this figure will show the
 bending moment values at the critical location along the Foundation length or width. Plotting methods takes a show_plot argument which can either be True or False. which by default is True
 
     fdn_design.plot_bending_moment_X()
     fdn_design.plot_shear_force_X()
 This outputs the bending moment plot with the design bending moment shown at the face of the column
-![Image](https://github.com/CodedKunz/FoundationDesign/blob/main/examples/bending_moment1.png?raw=true)
+![Image](https://github.com/kunle009/FoundationDesign/blob/main/assets/bending_moment1.png?raw=true)
 The shear force plot is also displayed with critical shearforce showing at 1d from column the face
-![Image](https://github.com/CodedKunz/FoundationDesign/blob/main/examples/shear_force.jpg?raw=true)
+![Image](https://github.com/kunle009/FoundationDesign/blob/main/assets/shear_force.jpg?raw=true)
 
 ## Installing the package
 
 If you want to install the `FoundationDesign` package, you run this one-liner:
 
     pip install FoundationDesign
 
@@ -140,7 +146,8 @@
 ## Future Works
 
 The following are areas that will be implemented in future:
 
 - Adding a method to calculate crack width
 - PDF report generation
 - User documentation
+- A comprehensive web app for analysis and design of foundations
```

### Comparing `FoundationDesign-0.0.6/LICENSE` & `FoundationDesign-0.0.7/LICENSE`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 CodedKunz
+Copyright (c) 2022 Kunle Yusuf
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `FoundationDesign-0.0.6/PKG-INFO` & `FoundationDesign-0.0.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 Metadata-Version: 2.1
 Name: FoundationDesign
-Version: 0.0.6
-Summary:  A python module for structural analysis and design of different foundation type in accordance to the Eurocodes
+Version: 0.0.7
+Summary: A python module for structural analysis and design of different foundation types in accordance to the Eurocodes
+Home-page: https://github.com/kunle009/FoundationDesign
 Author: Kunle Yusuf
 Author-email: kunleyusuf858@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: indeterminatebeam==2.2.1
+Requires-Dist: numpy==1.24.4
+Requires-Dist: plotly==5.15.0
 
 
 # FoundationDesign
 
 [![PyPi](https://img.shields.io/pypi/v/FoundationDesign.svg)](https://pypi.org/project/FoundationDesign/)
 ![PyPI - License](https://img.shields.io/pypi/l/FoundationDesign)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/FoundationDesign)
+[![Downloads](https://static.pepy.tech/badge/foundationdesign)](https://pepy.tech/project/foundationdesign)
+[![Downloads](https://static.pepy.tech/badge/foundationdesign/month)](https://pepy.tech/project/foundationdesign)
+[![build & test](https://github.com/kunle009/FoundationDesign/actions/workflows/build-and-test.yml/badge.svg?branch=main)](https://github.com/kunle009/FoundationDesign/actions/workflows/build-and-test.yml)
 
 
 FoundationDesign is a python module to be used for the design and analysis
 of different foundation types in accordance to the Eurocode 2.
 This project is an attempt to have a free standalone python package that can
 be used to analyse and design foundations with results as good as paid softwares.
 This module will be useful in determining:
@@ -118,17 +124,17 @@
 Lots of checks can be done on the Foundation which can be found in the notebooks contained in the examples folder
 To show the bending moment of the Foundation. The ```plot_bending_moment_X()``` can be called this figure will show the
 bending moment values at the critical location along the Foundation length or width. Plotting methods takes a show_plot argument which can either be True or False. which by default is True
 
     fdn_design.plot_bending_moment_X()
     fdn_design.plot_shear_force_X()
 This outputs the bending moment plot with the design bending moment shown at the face of the column
-![Image](https://github.com/CodedKunz/FoundationDesign/blob/main/examples/bending_moment1.png?raw=true)
+![Image](https://github.com/kunle009/FoundationDesign/blob/main/assets/bending_moment1.png?raw=true)
 The shear force plot is also displayed with critical shearforce showing at 1d from column the face
-![Image](https://github.com/CodedKunz/FoundationDesign/blob/main/examples/shear_force.jpg?raw=true)
+![Image](https://github.com/kunle009/FoundationDesign/blob/main/assets/shear_force.jpg?raw=true)
 
 ## Installing the package
 
 If you want to install the `FoundationDesign` package, you run this one-liner:
 
     pip install FoundationDesign
 
@@ -140,7 +146,8 @@
 ## Future Works
 
 The following are areas that will be implemented in future:
 
 - Adding a method to calculate crack width
 - PDF report generation
 - User documentation
+- A comprehensive web app for analysis and design of foundations
```

### Comparing `FoundationDesign-0.0.6/README.md` & `FoundationDesign-0.0.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 
 # FoundationDesign
 
 [![PyPi](https://img.shields.io/pypi/v/FoundationDesign.svg)](https://pypi.org/project/FoundationDesign/)
 ![PyPI - License](https://img.shields.io/pypi/l/FoundationDesign)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/FoundationDesign)
+[![Downloads](https://static.pepy.tech/badge/foundationdesign)](https://pepy.tech/project/foundationdesign)
+[![Downloads](https://static.pepy.tech/badge/foundationdesign/month)](https://pepy.tech/project/foundationdesign)
+[![build & test](https://github.com/kunle009/FoundationDesign/actions/workflows/build-and-test.yml/badge.svg?branch=main)](https://github.com/kunle009/FoundationDesign/actions/workflows/build-and-test.yml)
 
 
 FoundationDesign is a python module to be used for the design and analysis
 of different foundation types in accordance to the Eurocode 2.
 This project is an attempt to have a free standalone python package that can
 be used to analyse and design foundations with results as good as paid softwares.
 This module will be useful in determining:
@@ -105,17 +107,17 @@
 Lots of checks can be done on the Foundation which can be found in the notebooks contained in the examples folder
 To show the bending moment of the Foundation. The ```plot_bending_moment_X()``` can be called this figure will show the
 bending moment values at the critical location along the Foundation length or width. Plotting methods takes a show_plot argument which can either be True or False. which by default is True
 
     fdn_design.plot_bending_moment_X()
     fdn_design.plot_shear_force_X()
 This outputs the bending moment plot with the design bending moment shown at the face of the column
-![Image](https://github.com/CodedKunz/FoundationDesign/blob/main/examples/bending_moment1.png?raw=true)
+![Image](https://github.com/kunle009/FoundationDesign/blob/main/assets/bending_moment1.png?raw=true)
 The shear force plot is also displayed with critical shearforce showing at 1d from column the face
-![Image](https://github.com/CodedKunz/FoundationDesign/blob/main/examples/shear_force.jpg?raw=true)
+![Image](https://github.com/kunle009/FoundationDesign/blob/main/assets/shear_force.jpg?raw=true)
 
 ## Installing the package
 
 If you want to install the `FoundationDesign` package, you run this one-liner:
 
     pip install FoundationDesign
 
@@ -127,7 +129,8 @@
 ## Future Works
 
 The following are areas that will be implemented in future:
 
 - Adding a method to calculate crack width
 - PDF report generation
 - User documentation
+- A comprehensive web app for analysis and design of foundations
```

### Comparing `FoundationDesign-0.0.6/setup.py` & `FoundationDesign-0.0.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,29 @@
-import setuptools
+from setuptools import setup, find_packages
 import os
 
 
-#store readme.md files
+# store readme.md files
 with open("README.md", "r") as fh:
     long_description = fh.read()
-#read the requirements
+# read the requirements
 with open("requirements.txt", "r") as fh:
     requirements = [line.strip() for line in fh]
 
-setuptools.setup(
+setup(
     name="FoundationDesign",
-    version="0.0.6",
+    packages=find_packages("FoundationDesign"),
+    version="0.0.7",
     author="Kunle Yusuf",
     author_email="kunleyusuf858@gmail.com",
-    description=" A python module for structural analysis and design of different foundation type in accordance to the Eurocodes",
+    description="A python module for structural analysis and design of different foundation types in accordance to the Eurocodes",
+    url = 'https://github.com/kunle009/FoundationDesign',
     long_description=long_description,
     long_description_content_type="text/markdown",
-    packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3.6',
+    python_requires=">=3.8",
     install_requires=requirements,
 )
```

