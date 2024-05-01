# Comparing `tmp/pymoxel-0.0.0.tar.gz` & `tmp/pymoxel-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymoxel-0.0.0.tar", last modified: Sun Sep 10 22:53:14 2023, max compression
+gzip compressed data, was "pymoxel-0.1.0.tar", last modified: Wed May  1 15:41:42 2024, max compression
```

## Comparing `pymoxel-0.0.0.tar` & `pymoxel-0.1.0.tar`

### file list

```diff
@@ -1,23 +1,60 @@
-drwxr-xr-x   0 asar      (1000) asar      (1000)        0 2023-09-10 22:53:14.973086 pymoxel-0.0.0/
--rw-r--r--   0 asar      (1000) asar      (1000)    35149 2023-09-09 08:55:21.000000 pymoxel-0.0.0/LICENSE
--rw-r--r--   0 asar      (1000) asar      (1000)       33 2023-09-09 10:01:04.000000 pymoxel-0.0.0/MANIFEST.in
--rw-r--r--   0 asar      (1000) asar      (1000)     2833 2023-09-10 22:53:14.972086 pymoxel-0.0.0/PKG-INFO
--rw-r--r--   0 asar      (1000) asar      (1000)     2139 2023-09-10 22:19:01.000000 pymoxel-0.0.0/README.md
--rw-r--r--   0 asar      (1000) asar      (1000)      861 2023-09-10 22:43:01.000000 pymoxel-0.0.0/pyproject.toml
--rw-r--r--   0 asar      (1000) asar      (1000)       38 2023-09-10 22:53:14.973086 pymoxel-0.0.0/setup.cfg
-drwxr-xr-x   0 asar      (1000) asar      (1000)        0 2023-09-10 22:53:14.969086 pymoxel-0.0.0/src/
-drwxr-xr-x   0 asar      (1000) asar      (1000)        0 2023-09-10 22:53:14.970086 pymoxel-0.0.0/src/moxel/
--rw-r--r--   0 asar      (1000) asar      (1000)     1215 2023-09-10 21:53:59.000000 pymoxel-0.0.0/src/moxel/__init__.py
--rw-r--r--   0 asar      (1000) asar      (1000)     1257 2023-09-09 10:18:46.000000 pymoxel-0.0.0/src/moxel/__main__.py
--rw-r--r--   0 asar      (1000) asar      (1000)     3696 2023-09-09 10:19:05.000000 pymoxel-0.0.0/src/moxel/cli.py
--rw-r--r--   0 asar      (1000) asar      (1000)     4338 2023-08-05 18:09:49.000000 pymoxel-0.0.0/src/moxel/lj_params.json
--rw-r--r--   0 asar      (1000) asar      (1000)    21415 2023-09-09 19:45:18.000000 pymoxel-0.0.0/src/moxel/utils.py
-drwxr-xr-x   0 asar      (1000) asar      (1000)        0 2023-09-10 22:53:14.972086 pymoxel-0.0.0/src/pymoxel.egg-info/
--rw-r--r--   0 asar      (1000) asar      (1000)     2833 2023-09-10 22:53:14.000000 pymoxel-0.0.0/src/pymoxel.egg-info/PKG-INFO
--rw-r--r--   0 asar      (1000) asar      (1000)      361 2023-09-10 22:53:14.000000 pymoxel-0.0.0/src/pymoxel.egg-info/SOURCES.txt
--rw-r--r--   0 asar      (1000) asar      (1000)        1 2023-09-10 22:53:14.000000 pymoxel-0.0.0/src/pymoxel.egg-info/dependency_links.txt
--rw-r--r--   0 asar      (1000) asar      (1000)       65 2023-09-10 22:53:14.000000 pymoxel-0.0.0/src/pymoxel.egg-info/requires.txt
--rw-r--r--   0 asar      (1000) asar      (1000)        6 2023-09-10 22:53:14.000000 pymoxel-0.0.0/src/pymoxel.egg-info/top_level.txt
-drwxr-xr-x   0 asar      (1000) asar      (1000)        0 2023-09-10 22:53:14.972086 pymoxel-0.0.0/tests/
--rw-r--r--   0 asar      (1000) asar      (1000)     1381 2023-09-09 10:19:34.000000 pymoxel-0.0.0/tests/test_cli.py
--rw-r--r--   0 asar      (1000) asar      (1000)     9633 2023-09-09 10:19:41.000000 pymoxel-0.0.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:41:42.903982 pymoxel-0.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:41:42.887982 pymoxel-0.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:41:42.891982 pymoxel-0.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-01 15:41:38.000000 pymoxel-0.1.0/.github/workflows/python-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-01 15:41:38.000000 pymoxel-0.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-01 15:41:38.000000 pymoxel-0.1.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-01 15:41:38.000000 pymoxel-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-05-01 15:41:42.903982 pymoxel-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-05-01 15:41:38.000000 pymoxel-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:41:42.891982 pymoxel-0.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-01 15:41:38.000000 pymoxel-0.1.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-01 15:41:38.000000 pymoxel-0.1.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-01 15:41:38.000000 pymoxel-0.1.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:41:42.891982 pymoxel-0.1.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-01 15:41:38.000000 pymoxel-0.1.0/docs/source/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-01 15:41:38.000000 pymoxel-0.1.0/docs/source/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-01 15:41:38.000000 pymoxel-0.1.0/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:41:42.891982 pymoxel-0.1.0/docs/source/down/
+-rw-r--r--   0 runner    (1001) docker     (127)     4067 2024-05-01 15:41:38.000000 pymoxel-0.1.0/docs/source/down/CIFs.zip
+-rw-r--r--   0 runner    (1001) docker     (127)    13638 2024-05-01 15:41:38.000000 pymoxel-0.1.0/docs/source/down/IRMOF-1.cif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:41:42.895982 pymoxel-0.1.0/docs/source/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   101913 2024-05-01 15:41:38.000000 pymoxel-0.1.0/docs/source/images/moxel_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)  1955651 2024-05-01 15:41:38.000000 pymoxel-0.1.0/docs/source/images/moxel_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   423802 2024-05-01 15:41:38.000000 pymoxel-0.1.0/docs/source/images/plot_voxels.png
+-rw-r--r--   0 runner    (1001) docker     (127)   347027 2024-05-01 15:41:38.000000 pymoxel-0.1.0/docs/source/images/voxels.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-01 15:41:38.000000 pymoxel-0.1.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-01 15:41:38.000000 pymoxel-0.1.0/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-01 15:41:38.000000 pymoxel-0.1.0/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-01 15:41:38.000000 pymoxel-0.1.0/docs/source/moxel.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-05-01 15:41:38.000000 pymoxel-0.1.0/docs/source/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-01 15:41:38.000000 pymoxel-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 15:41:42.903982 pymoxel-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:41:42.891982 pymoxel-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:41:42.899982 pymoxel-0.1.0/src/moxel/
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-01 15:41:38.000000 pymoxel-0.1.0/src/moxel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-05-01 15:41:38.000000 pymoxel-0.1.0/src/moxel/_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-01 15:41:38.000000 pymoxel-0.1.0/src/moxel/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15346 2024-05-01 15:41:38.000000 pymoxel-0.1.0/src/moxel/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-05-01 15:41:38.000000 pymoxel-0.1.0/src/moxel/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:41:42.903982 pymoxel-0.1.0/src/pymoxel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-05-01 15:41:42.000000 pymoxel-0.1.0/src/pymoxel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-01 15:41:42.000000 pymoxel-0.1.0/src/pymoxel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 15:41:42.000000 pymoxel-0.1.0/src/pymoxel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-01 15:41:42.000000 pymoxel-0.1.0/src/pymoxel.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-01 15:41:42.000000 pymoxel-0.1.0/src/pymoxel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-01 15:41:42.000000 pymoxel-0.1.0/src/pymoxel.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:41:42.899982 pymoxel-0.1.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:41:42.903982 pymoxel-0.1.0/tests/CIFs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-01 15:41:38.000000 pymoxel-0.1.0/tests/CIFs/COF-5.cif
+-rw-r--r--   0 runner    (1001) docker     (127)    13638 2024-05-01 15:41:38.000000 pymoxel-0.1.0/tests/CIFs/IRMOF-1.cif
+-rw-r--r--   0 runner    (1001) docker     (127)    32325 2024-05-01 15:41:38.000000 pymoxel-0.1.0/tests/CIFs/ZIF-69.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-05-01 15:41:38.000000 pymoxel-0.1.0/tests/CIFs/ZnHBDC.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-01 15:41:38.000000 pymoxel-0.1.0/tests/CIFs/ZnMOF-74.cif
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 15:41:38.000000 pymoxel-0.1.0/tests/CIFs/corrupted_1.cif
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 15:41:38.000000 pymoxel-0.1.0/tests/CIFs/corrupted_2.cif
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 15:41:38.000000 pymoxel-0.1.0/tests/CIFs/corrupted_3.cif
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 15:41:38.000000 pymoxel-0.1.0/tests/CIFs/corrupted_4.cif
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 15:41:38.000000 pymoxel-0.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-01 15:41:38.000000 pymoxel-0.1.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-05-01 15:41:38.000000 pymoxel-0.1.0/tests/test_utils.py
```

### Comparing `pymoxel-0.0.0/LICENSE` & `pymoxel-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymoxel-0.0.0/PKG-INFO` & `pymoxel-0.1.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,19 @@
-Metadata-Version: 2.1
-Name: pymoxel
-Version: 0.0.0
-Summary: Package for parallel calculation of energy voxels.
-Author-email: "Antonios P. Sarikas" <antonios.sarikas@gmail.com>
-License: GPL-3.0-only
-Project-URL: Homepage, https://github.com/adosar/moxel
-Project-URL: Documentation, https://moxel.readthedocs.io
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: matplotlib>=3.7.1
-Requires-Dist: numpy>=1.24.1
-Requires-Dist: pymatgen>=2023.5.10
-Requires-Dist: rich>=13.4.1
-
 <h1 align="center">
   <img alt="Logo" src="https://raw.githubusercontent.com/adosar/moxel/master/docs/source/images/moxel_logo.svg"/>
 </h1>
 
 <h4 align="center">
   
 [![Requires Python 3.10+](https://img.shields.io/badge/Python-3.10%2B-blue?logo=python&logoColor=yellow&label=Python&labelColor=black&color=blue)](https://www.python.org/downloads/)
 [![Licensed under GPL-3.0-only](https://img.shields.io/badge/GPL--3.0--only-gold?label=License&labelColor=black)](https://spdx.org/licenses/GPL-3.0-only.html)
-[![Read The Docs](https://img.shields.io/badge/stable-green?logo=readthedocs&logoColor=blue&label=Read%20The%20Docs&labelColor=black)](https://moxel.readthedocs.io)
+[![Read the Docs](https://img.shields.io/badge/stable-green?logo=readthedocs&logoColor=blue&label=Read%20the%20Docs&labelColor=black)](https://moxel.readthedocs.io)
+[![pip install pymoxel](https://img.shields.io/badge/install-blue?logo=pypi&logoColor=yellow&label=PyPI&labelColor=black)](https://pypi.org/project/pymoxel/)
 [![Documentation Status](https://readthedocs.org/projects/moxel/badge/?version=stable)](https://moxel.readthedocs.io/en/stable/?badge=stable)
+[![PyPI version](https://badge.fury.io/py/pymoxel.svg)](https://badge.fury.io/py/pymoxel)
 
 </h4>
 
 MOXελ is a Python package for **parallel calculation of energy voxels**, with
 emphasis on reticular chemistry.
 
 The majority of time in a ML workflow goes into constructing the inputs and
@@ -38,15 +21,16 @@
 
 MOXελ aims to provide a **simple and fast interface to generate energy voxels in
 a ML-ready format**, minimizing as much as possible the time spent on these
 preprocessing steps.
 
 ## ⚙️  Installation
 It is strongly recommended to **perform the installation inside a virtual environment**.
-Check the [installations steps](https://moxel.readthedocs.io/en/stable/installation.html).
+
+Check the [installation steps](https://moxel.readthedocs.io/en/stable/installation.html).
 
 Assuming an activated virtual environment:
 ```sh
 pip install pymoxel
 ```
 
 ## 📖 Usage
@@ -54,15 +38,28 @@
 
 <p align="center">
   <img alt="Voxels" src="https://raw.githubusercontent.com/adosar/moxel/master/docs/source/images/voxels.gif" width="25%"/>
 </p>
 
 ## 📰 Citing MOXελ
 If you use ΜΟΧελ in your research, please consider citing the following work:
-> Currently N/A.
+
+    @article{Sarikas2024,
+    title = {Gas adsorption meets deep learning: voxelizing the potential energy surface of metal-organic frameworks},
+    volume = {14},
+    ISSN = {2045-2322},
+    url = {http://dx.doi.org/10.1038/s41598-023-50309-8},
+    DOI = {10.1038/s41598-023-50309-8},
+    number = {1},
+    journal = {Scientific Reports},
+    publisher = {Springer Science and Business Media LLC},
+    author = {Sarikas,  Antonios P. and Gkagkas,  Konstantinos and Froudakis,  George E.},
+    year = {2024},
+    month = jan 
+    }
 
 ## 📇 TODO
 * Improve modeling of interactions
 * Improve voxelization scheme
 * Improve performance
 
 ## 📑 License
```

### Comparing `pymoxel-0.0.0/pyproject.toml` & `pymoxel-0.1.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
-requires = ["setuptools"]
+requires = ["setuptools>=64", "setuptools_scm>=8"]
 build-backend = "setuptools.build_meta"
 
+[tool.setuptools_scm]
+# can be empty if no extra settings are needed, presence enables setuptools_scm
+
 [tool.setuptools.packages.find]
 where = ["src"]
 
-[tool.setuptools.dynamic]
-version = {attr = "moxel.__version__"}
-
 [project]
 name = "pymoxel"
 dynamic = ["version"]
 
 authors = [
   {name="Antonios P. Sarikas", email="antonios.sarikas@gmail.com"},
 ]
@@ -24,16 +24,22 @@
 classifiers = [
     "Programming Language :: Python :: 3",
 	"License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: POSIX :: Linux",
 ]
 
 dependencies = [
-	"matplotlib>=3.7.1",
-	"numpy>=1.24.1",
-	"pymatgen>=2023.5.10",
-	"rich>=13.4.1",
+	"numpy",
+	"fire",
+	"pymatgen",
+	"tqdm",
+	"matplotlib",
+	"pyvista",
 ]
 
 [project.urls]
 Homepage = "https://github.com/adosar/moxel"
 Documentation = "https://moxel.readthedocs.io"
+Changelog = "https://moxel.readthedocs.io/en/stable/changes.html"
+
+[project.scripts]
+moxel = "moxel.cli:moxel_fire"
```

### Comparing `pymoxel-0.0.0/src/moxel/__init__.py` & `pymoxel-0.1.0/src/moxel/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # This file is part of MOXελ.
-# Copyright (C) 2023 Antonios P. Sarikas
+# Copyright (C) 2023-2024 Antonios P. Sarikas
 
 # MOXελ is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 # This program is distributed in the hope that it will be useful,
@@ -13,21 +13,12 @@
 
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 """
 MOXελ is a Python package for parallel calculation of energy voxels, with
 emphasis on reticular chemistry.
-
-.. note::
-    Currently, interactions are modelled with the Lennard-Jones (LJ) potential.
 """
 
 __author__ = 'Antonios P. Sarikas'
-__version__ = '0.0.0'
-__copyright__ = "Copyright (c) 2023 Antonios P. Sarikas"
+__copyright__ = "Copyright (C) 2023-2024 Antonios P. Sarikas"
 __license__ = 'GPL-3.0-only'
-
-from . utils import (
-        Grid, voxels_from_file, voxels_from_files, voxels_from_dir,
-        mic_scale_factors, batch_clean_and_merge, plot_voxels
-        )
```

### Comparing `pymoxel-0.0.0/src/moxel/utils.py` & `pymoxel-0.1.0/src/moxel/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,66 @@
 # This file is part of MOXελ.
-# Copyright (C) 2023 Antonios P. Sarikas
+# Copyright (C) 2023-2024 Antonios P. Sarikas
 
 # MOXελ is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
+r"""
+This module provides helper functions for creating voxels.
+
+.. note::
+    Currently, interactions are modelled with the Lennard-Jones (LJ) potential.
+"""
+
 import os
 import json
 import itertools
-import numpy as np
 from pathlib import Path
-import matplotlib as mpl
-from itertools import repeat
-from rich.progress import track
-import matplotlib.pyplot as plt
 from multiprocessing import Pool
-from dataclasses import dataclass
+from itertools import repeat
+import warnings
+import numpy as np
+from tqdm import tqdm
 from pymatgen.core import Structure
+from . _params import lj_params
+warnings.filterwarnings('ignore')
+
+
+def get_names(fname):
+    r"""
+    Load a list of material names saved in ``.json`` format.
+
+    Parameters
+    ----------
+    fname : str
+        Pathname to the ``.json`` file.
+
+    Returns
+    -------
+    names : list
+    """
+    with open(fname, 'r') as fhand:
+        names = json.load(fhand)
+
+    return names
 
 
 def mic_scale_factors(r, lattice_vectors):
     r"""
-    Return scale factors to satisfy minimum image convention (MIC) [1]_ .
+    Return scale factors to satisfy minimum image convention [MIC]_.
 
     Parameters
     ----------
     r : float
         The cutoff radius used in MIC convetion.
     lattice_vectors : array of shape (3, 3)
         The lattice vectors of the unit cell.
@@ -43,58 +69,26 @@
     Returns
     -------
     scale_factors : array of shape (3,)
         ``scale_factors[i]`` scales ``lattice_vectors[i]``.
 
     References
     ----------
-    .. [1] W. Smith, "The Minimum Image Convention in Non-Cubic MD Cells", 1989.
+    .. [MIC] W. Smith, "The Minimum Image Convention in Non-Cubic MD Cells", 1989.
     """
     a, b, c = lattice_vectors
     volume = np.linalg.norm(np.dot(a, np.cross(b, c)))
 
     w_a = volume/np.linalg.norm(np.cross(b, c))
     w_b = volume/np.linalg.norm(np.cross(a, c))
     w_c = volume/np.linalg.norm(np.cross(a, b))
 
     return np.ceil(2*r/np.array([w_a, w_b, w_c]))
 
 
-#def mic_scale_factors(r, lattice_vectors):
-#    r"""
-#    Return scale factors to satisfy minimum image convention (MIC).
-#
-#    Parameters
-#    ----------
-#    r : float
-#        The cutoff radius used in MIC convetion.
-#    lattice_vectors : array of shape (3, 3)
-#        The lattice vectors of the unit cell.
-#        Each row corresponds to a lattice vector.
-#
-#    Returns
-#    -------
-#    scale_factors : array of shape (3,)
-#        ``scale_factors[i]`` scales ``lattice_vectors[i]``.
-#    """
-#    a, b, c = lattice_vectors
-#
-#    a_hat = a/np.linalg.norm(a)
-#    b_a = b - np.dot(b, a_hat)*a_hat # Rejection of b from a.
-#
-#    ab_cross = np.cross(a, b)
-#    ab_cross_hat = ab_cross/np.linalg.norm(ab_cross)
-#    c_ab = np.dot(c, ab_cross_hat)
-#
-#    norms = [np.linalg.norm(i) for i in [a, b_a, c_ab]]
-#
-#    return np.ceil(2*r/np.array(norms))
-
-
-@dataclass
 class Grid:
     r"""
     A 3D energy grid over a crystal structure.
 
     Parameters
     ----------
     grid_size : int, default=25
@@ -104,21 +98,21 @@
     epsilon : float, default=50
         Epsilon value (ε/K) of the probe atom.
     sigma : float, default=2.5
         Sigma value (σ/Å) of the probe atom.
 
     Attributes
     ----------
-    structure : `pymatgen.core.structure.Structure <https://pymatgen.org/pymatgen.core.structure.html#pymatgen.core.structure.Structure>`_
+    structure : :class:`pymatgen.core.structure.Structure`
         Available only after :meth:`Grid.load_structure` has been called.
     structure_name : str
         Available only after :meth:`Grid.load_structure` has been called.
     cubic_box : bool
         Available only after :meth:`Grid.calculate` has been called.
-    voxels : array of shape (grid_size, grid_size, grid_size)
+    voxels : array of shape (grid_size,)*3
        Available only after :meth:`Grid.calculate` has been called.
     """
     def __init__(self, grid_size=25, cutoff=10, epsilon=50, sigma=2.5):
         self.grid_size = grid_size
         self.cutoff = cutoff
         self.epsilon = epsilon
         self.sigma = sigma
@@ -129,18 +123,17 @@
 
         Parameters
         ----------
         cif_pathname : str
            Pathname to the ``.cif`` file.
         """
         self.structure = Structure.from_file(cif_pathname)
-        #self.structure_name = cif_pathname.split('/')[-1].split('.')[0]
-        self.structure_name = cif_pathname.split('/')[-1].removesuffix('.cif')
+        self.structure_name = Path(cif_pathname).stem
 
-    def calculate(self, cubic_box=False, length=30, potential='lj'):
+    def calculate(self, cubic_box=False, length=30, potential='lj', n_jobs=None):
         r"""
         Iterate over the grid and return voxels.
 
         For computational efficiency and to assure (approximately) the same
         spatial resolution, the grid is overlayed over a supercell scaled
         according to MIC, see :func:`mic_scale_factors`.
 
@@ -153,67 +146,70 @@
         ----------
         potential : str, default='lj'
             The potential used to calculate voxels. Currently, only the
             LJ potential is supported.
         cubic_box : bool, default=False
             If ``True``, the simulation box is cubic.
         length : float, default=30
-            The size of the cubic box in Å. Takes effect only if ``cubic_box=True``.
+            The size of the cubic box in Å. Takes effect only
+            if ``cubic_box == True``.
+        n_jobs : int, optional
+            Number of jobs to run in parallel. If ``None``, all processors are
+            used.
 
         Returns
         -------
-        voxels : array of shape (grid_size, grid_size, grid_size)
+        voxels : array of shape (grid_size,)*3
             The energy voxels as :math:`e^{-\beta \mathcal{V}}`, to ensure
             numerical stability.
         Notes
         -----
         For structures that can not be processsed, their voxels are filled with
         zeros.
         """
         self.cubic_box = cubic_box
 
         if cubic_box:
             d = length / 2
-            probe_coords = np.linspace(0-d, 0+d, self.grid_size) # Cartesian
+            probe_coords = np.linspace(0-d, 0+d, self.grid_size)  # Cartesian.
             self._simulation_box = self.structure
         else:
-            probe_coords = np.linspace(0, 1, self.grid_size) # Fractional
+            probe_coords = np.linspace(0, 1, self.grid_size)  # Fractional.
             scale = mic_scale_factors(self.cutoff, self.structure.lattice.matrix)
             self._simulation_box = self.structure * scale
         
         if potential == 'lj':
             # Embarrassingly parallel.
-            with Pool(processes=None) as p:
-                energies = list(
-                        p.map(
-                            self.lj_potential, itertools.product(*(probe_coords,)*3)
-                            )
+            with Pool(processes=n_jobs) as p:
+                energies = p.map(
+                        self.lj_potential, itertools.product(*(probe_coords,)*3)
                         )
+
         self.voxels = np.array(energies, dtype=np.float32).reshape((self.grid_size,)*3)
 
         return self.voxels
 
     def lj_potential(self, coords):
         r"""
         Calculate LJ potential at cartesian or fractional
         coordinates.
 
         Parameters
         ----------
         coordinates : array_like of shape (3,)
-            If ``cubic_box=True`` cartesian. Else, fractional.
+            If ``cubic_box == True`` cartesian. Else, fractional.
 
         Returns
         -------
         energy : float
             Energy as :math:`e^{-\beta \mathcal{V}}`, to ensure numerical stability.
         """
         if self.cubic_box:
             cartesian_coords = coords
-            neighbors = self._simulation_box.get_sites_in_sphere(coords, self.cutoff)
+            neighbors = self._simulation_box.get_sites_in_sphere(cartesian_coords, self.cutoff)
         else:
             cartesian_coords = self._simulation_box.lattice.get_cartesian_coords(coords)
             neighbors = self._simulation_box.get_sites_in_sphere(cartesian_coords, self.cutoff)
 
         energy = 0
         if len(neighbors) != 0:
             for atom in neighbors:
@@ -221,23 +217,24 @@
                 if r_ij <= 1e-3:
                     energy += 1000
                 else:
                     e_j, s_j = lj_params[atom.species_string]
                     x = (0.5 * (s_j + self.sigma)) / r_ij
                     energy += 4 * np.sqrt(e_j * self.epsilon) * (x**12 - x**6)
 
-        return np.exp(-(1 / 298) * energy) # For numerical stability.
+        # This should be changed with clipping in future versions.
+        return np.exp(-(1 / 298) * energy)  # For numerical stability.
 
 
 def voxels_from_file(
         cif_pathname, grid_size=25, cutoff=10,
         epsilon=50, sigma=2.5, cubic_box=False, length=30, 
-        only_voxels=True,
+        n_jobs=None, only_voxels=True,
         ):
-    """
+    r"""
     Return voxels from ``.cif`` file.
 
     Parameters
     ----------
     cif_pathname : str
        Pathname to the ``.cif`` file.
     grid_size : int, default=25
@@ -247,388 +244,231 @@
     epsilon : float, default=50
         Epsilon value (ε/K) of the probe atom.
     sigma : float, default=25
         Sigma value (σ/Å) of the probe atom.
     cubic_box : bool, default=False
         If ``True``, the simulation box is cubic.
     length : float, default=30
-        The size of the cubic box in Å. Takes effect only if ``cubic_box=True``.
+        The size of the cubic box in Å. Takes effect only if ``cubic_box == True``.
+    n_jobs : int, optional
+        Number of jobs to run in parallel. If ``None``, all processors are used.
     only_voxels : bool, default=True
         Determines ``out`` type.
         
     Returns
     -------
-    out : ``array`` or :class:`.Grid`
-        If ``only_voxels=True``, array of shape ``(grid_size, grid_size,
-        grid_size)``. Otherwise, :class:`.Grid`.
+    out : ``array`` or :class:`Grid`
+        If ``only_voxels == True``, array of shape ``(grid_size,)*3``.
+        Otherwise, :class:`Grid`.
 
     Notes
     -----
-
-    * For structures that can not be processsed, their voxels are filled with zeros.
+    For structures that can not be processsed, their voxels are filled with zeros.
     """
     grid = Grid(grid_size, cutoff, epsilon, sigma)
     try:
         grid.load_structure(cif_pathname)
-        grid.calculate(cubic_box=cubic_box, length=length)
-    except ValueError:
+        grid.calculate(cubic_box=cubic_box, length=length, n_jobs=n_jobs)
+    except:
         grid.voxels = np.full(shape=(grid_size,)*3, fill_value=0, dtype=np.float32)
 
     if only_voxels:
         return grid.voxels
     else:
         return grid
 
 
 def voxels_from_files(
-        cif_pathnames, grid_size=25, cutoff=10,
-        epsilon=50, sigma=2.5,
-        cubic_box=False, length=30,
-        out_pathname=None,
+        cif_pathnames, out_pathname, grid_size=25, cutoff=10,
+        epsilon=50, sigma=2.5, cubic_box=False, length=30,
+        n_jobs=None,
         ):
-    """
-    Calculate voxels from a list of ``.cif`` files and save them in ``out_pathname`` as
-    ``array`` of shape ``(n_samples, grid_size, grid_size, grid_size)``, where
-    ``n_samples`` is the number of is the number of ``.cif`` files in
-    ``cif_pathnames``.
+    r"""
+    Calculate voxels from a list of ``.cif`` files and store them under
+    ``out_pathname`` as :class:`numpy.array` of shape
+    ``(n_samples, grid_size, grid_size, grid_size)``,
+    where ``n_samples == len(cif_pathnames)``.
+
+    After processing the following files are created::
 
+        out_pathname
+            ├──voxels.npy
+            └──names.json
+
+    The file ``names.json`` stores the names of the materials, which might be
+    useful for later indexing.
 
     Parameters
     ----------
-    cif_pathanmes : list
+    cif_pathnames : list
        List of pathnames to the ``.cif`` files.
+    out_pathname : str
+        Pathname to the directory under which voxels are stored.
     grid_size : int, default=25
         Number of grid points along each dimension.
     cutoff : float, default=10
         Cutoff radius (Å) for the LJ potential.
     epsilon : float, default=50
         Epsilon value (ε/K) of the probe atom.
     sigma : float, default=25
         Sigma value (σ/Å) of the probe atom.
     cubic_box : bool, default=False
         If ``True``, the simulation box is cubic.
     length : float, default=30
-        The size of the cubic box in Å. Takes effect only if ``cubic_box=True``.
-    out_pathname : str, optional
-        Pathname to the file holding the voxels. If not specified, voxels are stored in
-        ``./voxels.npy``.
+        The size of the cubic box in Å. Takes effect only if ``cubic_box == True``.
+    n_jobs : int, optional
+        Number of jobs to run in parallel. If ``None``, all processors are used.
     
     Notes
     -----
-
     * Samples in output array follow the order in ``cif_pathnames``.
-
     * For structures that can not be processsed, their voxels are filled with zeros.
     """
-    n = len(cif_pathnames)
-    cif_files = [i for i in cif_pathnames if i.endswith('.cif')]
-    out_pathname = './voxels.npy' if not out_pathname else out_pathname
+    n_samples = len(cif_pathnames)
+    names = [Path(i).stem for i in cif_pathnames]
+
+    # Store the names.
+    with open(f'{out_pathname}/names.json', mode='w') as fhand:
+        json.dump(names, fhand, indent=4)
 
     fp = np.lib.format.open_memmap(
-        out_pathname, mode='w+',
-        shape=(n, *(grid_size,)*3),
+        f'{out_pathname}/voxels.npy', mode='w+',
+        shape=(n_samples, *(grid_size,)*3),
         dtype=np.float32
         )
 
     grids = map(
-            voxels_from_file, cif_files,
+            voxels_from_file, cif_pathnames,
             repeat(grid_size), repeat(cutoff),
             repeat(epsilon), repeat(sigma),
-            repeat(cubic_box), repeat(length)
+            repeat(cubic_box), repeat(length),
+            repeat(n_jobs)
             )
 
-    for i in track(range(n), description='Processing...'):
+    for i in tqdm(range(n_samples), desc='Creating voxels'):
         fp[i] = next(grids)
 
     fp.flush()
 
 
 def voxels_from_dir(
-        cif_dirname, grid_size=25, cutoff=10,
-        epsilon=50, sigma=2.5,
-        cubic_box=False, length=30,
-        out_pathname=None,
+        cif_dirname, out_pathname, grid_size=25, cutoff=10,
+        epsilon=50, sigma=2.5, cubic_box=False, length=30,
+        n_jobs=None,
         ):
-    """
-    Calculate voxels from ``.cif`` files in ``cif_dirname`` and save them in
-    ``out_pathname`` as ``array`` of shape ``(n_samples, grid_size, grid_size,
-    grid_size)``, where ``n_samples`` is the number of ``.cif`` files in
-    ``cif_dirname``.
+    r"""
+    Calculate voxels from a directory of ``.cif`` files and save them under
+    ``out_pathname`` as :class:`numpy.array` of shape
+    ``(n_samples, grid_size, grid_size, grid_size)``,
+    where ``n_samples == len(cif_pathnames)``.
+
+    After processing the following files are created::
+
+        out_pathname
+            ├──voxels.npy
+            └──names.json
+
+    The file ``names.json`` stores the names of the materials, which might be
+    useful for later indexing.
 
     Parameters
     ----------
     cif_dirname : str
        Pathname to the directory containing the ``.cif`` files.
+    out_pathname : str
+        Pathname to the directory under which voxels are stored.
     grid_size : int, default=25
-       Number of grid points along each dimension.
+        Number of grid points along each dimension.
     cutoff : float, default=10
         Cutoff radius (Å) for the LJ potential.
     epsilon : float, default=50
         Epsilon value (ε/K) of the probe atom.
+    sigma : float, default=25
+        Sigma value (σ/Å) of the probe atom.
     cubic_box : bool, default=False
         If ``True``, the simulation box is cubic.
     length : float, default=30
-        The size of the cubic box in Å. Takes effect only if ``cubic_box=True``.
-    sigma : float, default=25
-        Sigma value (σ/Å) of the probe atom.
-    out_pathname : str, optional
-        Pathname to the file holding the voxels. If not specified, voxels are stored
-        in ``./voxels.npy``.
-    
+        The size of the cubic box in Å. Takes effect only if ``cubic_box == True``.
+    n_jobs : int, optional
+        Number of jobs to run in parallel. If ``None``, all processors are used.
+
     Notes
     -----
-
     * Samples in output array follow the order in ``sorted(os.listdir(cif_dirname))``.
-
     * For structures that can not be processsed, their voxels are filled with zeros.
     """
-    files = sorted(os.listdir(cif_dirname))
-    cif_files = [f'{cif_dirname}/{file}' for file in files if file.endswith('.cif')]
-    n = len(cif_files)
-    out_pathname = './voxels.npy' if not out_pathname else out_pathname
-
-    fp = np.lib.format.open_memmap(
-            out_pathname, mode='w+',
-            shape=(n, *(grid_size,)*3),
-            dtype=np.float32
-            )
+    files = [os.path.join(cif_dirname, f) for f in sorted(os.listdir(cif_dirname))]
 
-    grids = map(
-            voxels_from_file, cif_files,
-            repeat(grid_size), repeat(cutoff),
-            repeat(epsilon), repeat(sigma),
-            repeat(cubic_box), repeat(length)
+    voxels_from_files(
+            files, out_pathname,
+            grid_size=grid_size, cutoff=cutoff,
+            epsilon=epsilon, sigma=sigma,
+            cubic_box=cubic_box, length=length,
+            n_jobs=n_jobs,
             )
 
-    for i in track(range(n), description='Processing...'):
-        fp[i] = next(grids)
-
-    fp.flush()
 
-
-#def batch_create(cif_pathnames, n_batches, batches_dirname=None):
-#    """
-#    Split a number of structures into ``n_batches`` of approximately equal size.
-#
-#    The batches are created under the ``batches_dirname`` directory.
-#
-#    For example, the i-th batch corresponds to ``batches_dirname/batch_i``.
-#
-#    Note that the **structures are randomly shuffled** prior to splitting.  The
-#    new ordering for the i-th batch is stored in
-#    ``batches_dirname/batch_i/names.json``
-#
-#    Parameters
-#    ----------
-#    cif_filenames : list
-#        List of pathnames to the ``.cif`` files.
-#    n_batches : int
-#        Number of batches that will be created.
-#    batches_dirname : str, optional
-#        Pathname to the directory where batches will be created. If ``None``, the
-#        batches are created under ``./``.
-#   """
-#    cif_pathnames = np.array([i for i in cif_pathnames if i.endswith('.cif')])
-#    np.random.shuffle(cif_pathnames)
-#
-#    batches = np.array_split(cif_pathnames, n_batches)
-#
-#    if batches_dirname == None:
-#        batches_dirname = '.'
-#
-#    for i, batch in enumerate(batches):
-#        os.mkdir(f'{batches_dirname}/batch_{i}')
-#        info_dict = {'names': list(batch), 'size': len(batch)}
-#
-#        with open(f'{batches_dirname}/batch_{i}/names.json', 'w') as fhand:
-#            json.dump(info_dict, fhand, indent=4)
-#
-
-#def batch_calculate(batch_dirname, cif_dirname, **kwargs):
-#    """
-#    Calculate voxels for the structures in ``batch_dirname/names.json``.
-#
-#    The voxels are saved in ``batch_dirname/voxels.npy``.
-#
-#    Parameters
-#    ----------
-#    batch_dirname : str
-#        Pathname to the batch directory.
-#    cif_dirname : str
-#        Pathname to the directory holding the ``.cif`` files.
-#    **kwargs :
-#        Valid keyword arguments for :func:`voxels_from_files`.
-#
-#        .. warning::
-#            Do not pass the arguments ``cif_pathnames`` and ``out_pathname`` of
-#            :func:`voxels_from_files`.
-#
-#    Notes
-#    -----
-#    For structures that can not be processsed, their voxels are filled with
-#    zeros.
-#    """
-#    with open(f'{batch_dirname}/names.json', 'r') as fhand:
-#        info = json.load(fhand)
-#
-#    names, size = info['names'], info['size']
-#    cif_names = [f'{cif_dirname}/{name}.cif' for name in names]
-#
-#    voxels_from_files(
-#        cif_names,
-#        out_pathname=f'{batch_dirname}/voxels.npy',
-#        **kwargs
-#        )
-#
-
-def batch_clean_and_merge(batch_dirnames, out_pathname=None):
+def batch_clean(batch_dirname):
     """
-    Clean a single batch, or *first clean and then merge* multiple batches.
-    All batches must have the form::
+    Clean a single batch.
+
+    The batch must have the form::
 
         batch
         ├──voxels.npy
         └──names.json
 
     Cleaning is required since the voxels for some structures might be zero,
-    see :func:`Grid.calculate`.
+    see :func:`Grid.calculate`. After cleaning, the directory has the form::
 
-    If ``len(batch_dirnames) == 1`` the cleaned voxels for are stored under
-    ``batch_dirnames[0]/clean_voxels.npy`` and the names of their corresponding
-    structures under ``batch_dirnames[0]/clean_names.json``.
-
-    If ``len(batch_dirnames) > 1`` the voxels (*cleaned and merged*) are stored
-    under ``out_pathname/clean_voxels.npy`` and the names of their corresponding
-    structures under ``out_pathname/clean_names.json``. That is::
-
-        out_pathname
+        batch
+        ├──voxels.npy
+        ├──names.json
         ├──clean_voxels.npy
         └──clean_names.json
 
     Parameters
     ----------
-    batch_dirnames : list
-        List of pathnames to the directories of the batches.
-    out_pathname : str, optional
-        Pathname to the directory holding the clean voxels and names.  The
-        directory is created if it doesn't exist. Takes effect only if
-        ``len(batch_dirnames) > 1``. If ``None`` voxels and names are
-        stored under ``./clean_voxels.npy`` and ``./clean_names.json``.
+    batch_dirname : str
+        Pathname to the directory which requires cleaning.
 
     Returns
     -------
     exit_status : int
         If no voxels are missing ``0`` else ``1``.
     """
-    batch_dict = dict()
-
-    for i, batch_dir in enumerate(batch_dirnames):
-        with open(f'{batch_dir}/names.json', 'r') as fhand:
-            info = json.load(fhand)
-
-        names = np.array(info['names'])
-
-        fp = np.load(f'{batch_dir}/voxels.npy', mmap_mode='r')
-
-        missing_idx = [i for i, j in enumerate(fp) if np.all(j == 0)]
+    # Case 1: no missing voxels.
+    names = get_names(f'{batch_dirname}/names.json')
+    voxels = np.load(f'{batch_dirname}/voxels.npy', mmap_mode='r')
 
-        batch_dict[f'batch_{i}'] = (fp, names, missing_idx)
+    missing_idx = [i for i, x in enumerate(voxels) if np.all(x == 0)]
 
-    missing = sum([len(batch_dict[i][2]) != 0 for i in batch_dict])
-    if missing == 0:
-        os.rename(f'{batch_dirnames[0]}/names.json', f'{batch_dirnames[0]}/clean_names.json') 
-        os.rename(f'{batch_dirnames[0]}/voxels.npy', f'{batch_dirnames[0]}/clean_voxels.npy') 
-        print('No missing voxels found!!')
+    if len(missing_idx) == 0:
+        print('No missing voxels found!')
         return 0
 
+    # Case 2: missing voxels.
     print('Missing voxels found! Cleaning...')
-    if len(batch_dirnames) == 1:
-        clean_dir = batch_dirnames[0]
-    elif out_pathname == None:
-        clean_dir = '.'
-    else:
-        clean_dir = out_pathname
-        try:
-            os.mkdir(clean_dir)
-        except:
-            pass
 
-    clean_size = np.sum([len(batch_dict[b][0]) - len(batch_dict[b][2]) for b in batch_dict.keys()])
+    clean_size = len(voxels) - len(missing_idx)
+
+    # Create a new array to store the clean voxels.
     clean_fp = np.lib.format.open_memmap(
-        f'{clean_dir}/clean_voxels.npy',
-        shape=(clean_size, *fp.shape[1:]),
+        f'{batch_dirname}/clean_voxels.npy',
+        shape=(clean_size, *voxels.shape[1:]),  # Shape (N, grid, grid, grid).
         mode='w+', dtype='float32',
         )
 
     clean_idx = 0
-    for b in batch_dict.keys():
-        for idx, x in enumerate(batch_dict[b][0]):
-            if idx in batch_dict[b][2]:
-                pass
-            else:
-                clean_fp[clean_idx] = x
-                clean_idx += 1
+    for idx, x in enumerate(voxels):
+        if idx in missing_idx:
+            pass
+        else:
+            clean_fp[clean_idx] = x
+            clean_idx += 1
 
-    clean_names = np.concatenate([np.delete(batch_dict[b][1], batch_dict[b][2]) for b in batch_dict.keys()])
-    clean_dict = {'names': list(clean_names)}
+    clean_names = np.delete(names, missing_idx)
 
-    with open(f'{clean_dir}/clean_names.json', 'w') as fhand:
-        json.dump(clean_dict, fhand, indent=4)
+    with open(f'{batch_dirname}/clean_names.json', 'w') as fhand:
+        json.dump(list(clean_names), fhand, indent=4)
 
     return 1
-
-
-def plot_voxels(voxels, *, fill_pattern=None, colorbar=True, cmap='viridis', **kwargs):
-    r"""
-    Visualizing voxels with `Axes3d.voxels`_.
-
-    .. _Axes3d.voxels: https://matplotlib.org/stable/api/_as_gen/mpl_toolkits.mplot3d.axes3d.Axes3D.voxels.html#mpl_toolkits.mplot3d.axes3d.Axes3D.voxels
-
-    Parameters
-    ----------
-    voxels : 3D array
-    fill_pattern : 3D array of bool, optional
-        A 3D array of truthy values, indicating which voxels to fill. If not
-        specified, all voxels are filled.
-    colorbar : bool, default=True
-        Whether to include a colorbar.
-    cmap : str, default='viridis'
-        `Colormap
-        <https://matplotlib.org/stable/tutorials/colors/colormaps.html>`_ that
-        colorizes the voxels based on their value.
-    **kwargs :
-        Valid keyword arguments for `Axes3d.voxels`_.
-
-        .. warning::
-            Do not pass the argument ``facecolors`` of `Axes3d.voxels`_.
-            This argument is used under the hood by :func:`plot_voxels_mpl` to
-            generate the colors of the voxels based on the specified ``cmap``.
-
-    Returns
-    -------
-    fig : `Figure <https://matplotlib.org/stable/api/figure_api.html#matplotlib.figure.Figure>`_
-    """
-
-    if np.all(fill_pattern) == None:
-        fill_pattern = np.full(voxels.shape, True)
-
-    cmap = plt.get_cmap(cmap)
-    norm = mpl.colors.Normalize()
-    colors = cmap((voxels - voxels.min()) / (voxels.max() - voxels.min()))
-
-    fig, ax = plt.subplots(subplot_kw={'projection': '3d'})
-    _ = ax.voxels(filled=fill_pattern, facecolors=colors, **kwargs)
-
-    if colorbar:
-        mappable = mpl.cm.ScalarMappable(norm=mpl.colors.Normalize(), cmap=cmap) 
-        cbar = fig.colorbar(
-            mappable, ax=ax, ticks=[], extend='max',
-            shrink=0.7, pad=0.1,
-            )
-        cbar.ax.set_ylabel(r'$e^{-\beta \mathcal{V}}$', fontsize=12)
-    
-    return fig
-
-
-# Loading LJ parameters.
-with open(f'{Path(__file__).parents[0]}/lj_params.json', 'r') as fhand:
-    lj_params = json.load(fhand)
```

### Comparing `pymoxel-0.0.0/src/pymoxel.egg-info/PKG-INFO` & `pymoxel-0.1.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,41 @@
 Metadata-Version: 2.1
 Name: pymoxel
-Version: 0.0.0
+Version: 0.1.0
 Summary: Package for parallel calculation of energy voxels.
 Author-email: "Antonios P. Sarikas" <antonios.sarikas@gmail.com>
 License: GPL-3.0-only
 Project-URL: Homepage, https://github.com/adosar/moxel
 Project-URL: Documentation, https://moxel.readthedocs.io
+Project-URL: Changelog, https://moxel.readthedocs.io/en/stable/changes.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: matplotlib>=3.7.1
-Requires-Dist: numpy>=1.24.1
-Requires-Dist: pymatgen>=2023.5.10
-Requires-Dist: rich>=13.4.1
+Requires-Dist: numpy
+Requires-Dist: fire
+Requires-Dist: pymatgen
+Requires-Dist: tqdm
+Requires-Dist: matplotlib
+Requires-Dist: pyvista
 
 <h1 align="center">
   <img alt="Logo" src="https://raw.githubusercontent.com/adosar/moxel/master/docs/source/images/moxel_logo.svg"/>
 </h1>
 
 <h4 align="center">
   
 [![Requires Python 3.10+](https://img.shields.io/badge/Python-3.10%2B-blue?logo=python&logoColor=yellow&label=Python&labelColor=black&color=blue)](https://www.python.org/downloads/)
 [![Licensed under GPL-3.0-only](https://img.shields.io/badge/GPL--3.0--only-gold?label=License&labelColor=black)](https://spdx.org/licenses/GPL-3.0-only.html)
-[![Read The Docs](https://img.shields.io/badge/stable-green?logo=readthedocs&logoColor=blue&label=Read%20The%20Docs&labelColor=black)](https://moxel.readthedocs.io)
+[![Read the Docs](https://img.shields.io/badge/stable-green?logo=readthedocs&logoColor=blue&label=Read%20the%20Docs&labelColor=black)](https://moxel.readthedocs.io)
+[![pip install pymoxel](https://img.shields.io/badge/install-blue?logo=pypi&logoColor=yellow&label=PyPI&labelColor=black)](https://pypi.org/project/pymoxel/)
 [![Documentation Status](https://readthedocs.org/projects/moxel/badge/?version=stable)](https://moxel.readthedocs.io/en/stable/?badge=stable)
+[![PyPI version](https://badge.fury.io/py/pymoxel.svg)](https://badge.fury.io/py/pymoxel)
 
 </h4>
 
 MOXελ is a Python package for **parallel calculation of energy voxels**, with
 emphasis on reticular chemistry.
 
 The majority of time in a ML workflow goes into constructing the inputs and
@@ -38,15 +43,16 @@
 
 MOXελ aims to provide a **simple and fast interface to generate energy voxels in
 a ML-ready format**, minimizing as much as possible the time spent on these
 preprocessing steps.
 
 ## ⚙️  Installation
 It is strongly recommended to **perform the installation inside a virtual environment**.
-Check the [installations steps](https://moxel.readthedocs.io/en/stable/installation.html).
+
+Check the [installation steps](https://moxel.readthedocs.io/en/stable/installation.html).
 
 Assuming an activated virtual environment:
 ```sh
 pip install pymoxel
 ```
 
 ## 📖 Usage
@@ -54,15 +60,28 @@
 
 <p align="center">
   <img alt="Voxels" src="https://raw.githubusercontent.com/adosar/moxel/master/docs/source/images/voxels.gif" width="25%"/>
 </p>
 
 ## 📰 Citing MOXελ
 If you use ΜΟΧελ in your research, please consider citing the following work:
-> Currently N/A.
+
+    @article{Sarikas2024,
+    title = {Gas adsorption meets deep learning: voxelizing the potential energy surface of metal-organic frameworks},
+    volume = {14},
+    ISSN = {2045-2322},
+    url = {http://dx.doi.org/10.1038/s41598-023-50309-8},
+    DOI = {10.1038/s41598-023-50309-8},
+    number = {1},
+    journal = {Scientific Reports},
+    publisher = {Springer Science and Business Media LLC},
+    author = {Sarikas,  Antonios P. and Gkagkas,  Konstantinos and Froudakis,  George E.},
+    year = {2024},
+    month = jan 
+    }
 
 ## 📇 TODO
 * Improve modeling of interactions
 * Improve voxelization scheme
 * Improve performance
 
 ## 📑 License
```

### Comparing `pymoxel-0.0.0/tests/test_cli.py` & `pymoxel-0.1.0/tests/test_cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 """
 
 import os
 import unittest
 import tempfile
 
 
+@unittest.skip
 class TestMoxelCLI(unittest.TestCase):
 
     def test_help(self):
         exit_status = os.system('python -m src.moxel -h')
         self.assertEqual(exit_status, 0)
 
     def test_run(self):
```

