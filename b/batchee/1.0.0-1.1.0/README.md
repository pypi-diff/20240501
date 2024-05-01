# Comparing `tmp/batchee-1.0.0.tar.gz` & `tmp/batchee-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batchee-1.0.0.tar", max compression
+gzip compressed data, was "batchee-1.1.0.tar", max compression
```

## Comparing `batchee-1.0.0.tar` & `batchee-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11357 2024-04-23 21:15:08.599802 batchee-1.0.0/LICENSE
--rw-r--r--   0        0        0     2002 2024-04-23 21:15:08.599802 batchee-1.0.0/README.md
--rw-r--r--   0        0        0        0 2024-04-23 21:15:08.599802 batchee-1.0.0/batcher/__init__.py
--rw-r--r--   0        0        0        0 2024-04-23 21:15:08.599802 batchee-1.0.0/batcher/harmony/__init__.py
--rw-r--r--   0        0        0     2229 2024-04-23 21:15:08.599802 batchee-1.0.0/batcher/harmony/cli.py
--rw-r--r--   0        0        0     6347 2024-04-23 21:15:08.599802 batchee-1.0.0/batcher/harmony/service_adapter.py
--rw-r--r--   0        0        0     4811 2024-04-23 21:15:08.599802 batchee-1.0.0/batcher/harmony/util.py
--rw-r--r--   0        0        0     4454 2024-04-23 21:15:08.599802 batchee-1.0.0/batcher/tempo_filename_parser.py
--rw-r--r--   0        0        0     1331 2024-04-23 21:15:30.191808 batchee-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2964 1970-01-01 00:00:00.000000 batchee-1.0.0/setup.py
--rw-r--r--   0        0        0     2556 1970-01-01 00:00:00.000000 batchee-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-01 17:27:41.710010 batchee-1.1.0/LICENSE
+-rw-r--r--   0        0        0     2522 2024-05-01 17:27:41.710010 batchee-1.1.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-01 17:27:41.710010 batchee-1.1.0/batcher/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-01 17:27:41.710010 batchee-1.1.0/batcher/harmony/__init__.py
+-rw-r--r--   0        0        0     2229 2024-05-01 17:27:41.710010 batchee-1.1.0/batcher/harmony/cli.py
+-rw-r--r--   0        0        0     6347 2024-05-01 17:27:41.710010 batchee-1.1.0/batcher/harmony/service_adapter.py
+-rw-r--r--   0        0        0     4811 2024-05-01 17:27:41.710010 batchee-1.1.0/batcher/harmony/util.py
+-rw-r--r--   0        0        0     4454 2024-05-01 17:27:41.710010 batchee-1.1.0/batcher/tempo_filename_parser.py
+-rw-r--r--   0        0        0     1331 2024-05-01 17:27:58.030316 batchee-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3493 1970-01-01 00:00:00.000000 batchee-1.1.0/setup.py
+-rw-r--r--   0        0        0     3076 1970-01-01 00:00:00.000000 batchee-1.1.0/PKG-INFO
```

### Comparing `batchee-1.0.0/LICENSE` & `batchee-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `batchee-1.0.0/README.md` & `batchee-1.1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: batchee
+Version: 1.1.0
+Summary: Determine how to group together input files into batches for subsequent concatenation
+Author: Daniel Kaufman
+Author-email: daniel.kaufman@nasa.gov
+Requires-Python: >=3.10,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: harmony-service-lib (>=1.0.26,<2.0.0)
+Description-Content-Type: text/markdown
+
 <p align="center">
     <img alt="batchee, a python package for grouping together filenames to enable subsequent batched operations (such as concatenation)."
     src="https://github.com/danielfromearth/batchee/assets/114174502/8b1a92a5-eccc-4674-9c00-3698e752077e" width="250"
     />
 </p>
 
 <p align="center">
@@ -10,14 +24,23 @@
     </a>
     <a href="https://github.com/python/black" target="_blank">
         <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Code style">
     </a>
     <a href="http://mypy-lang.org/" target="_blank">
         <img src="http://www.mypy-lang.org/static/mypy_badge.svg" alt="Mypy checked">
     </a>
+    <a href="https://pypi.org/project/batchee/" target="_blank">
+        <img src="https://img.shields.io/pypi/pyversions/batchee.svg" alt="Python Versions">
+    </a>
+    <a href="https://pypi.org/project/batchee" target="_blank">
+        <img src="https://img.shields.io/pypi/v/batchee?color=%2334D058label=pypi%20package" alt="Package version">
+    </a>
+    <a href="https://codecov.io/gh/nasa/batchee">
+     <img src="https://codecov.io/gh/nasa/batchee/graph/badge.svg?token=WDj92iN7c4" alt="Code coverage">
+    </a>
 </p>
 
 [//]: # (Using deprecated `align="center"` for the logo image and badges above, because of https://stackoverflow.com/a/62383408)
 
 
 # Overview
 _____
@@ -55,7 +78,8 @@
 #### Options
 
 - `-h`, `--help`            show this help message and exit
 - `-v`, `--verbose`  Enable verbose output to stdout; useful for debugging
 
 ---
 This package is NASA Software Release Authorization (SRA) # LAR-20440-1
+
```

#### html2text {}

```diff
@@ -1,11 +1,20 @@
+Metadata-Version: 2.1 Name: batchee Version: 1.1.0 Summary: Determine how to
+group together input files into batches for subsequent concatenation Author:
+Daniel Kaufman Author-email: daniel.kaufman@nasa.gov Requires-Python:
+>=3.10,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Topic :: Software Development :: Libraries :: Python
+Modules Requires-Dist: harmony-service-lib (>=1.0.26,<2.0.0) Description-
+Content-Type: text/markdown
 [batchee, a python package for grouping together filenames to enable subsequent
                  batched operations (such as concatenation).]
 _[_P_r_o_j_e_c_t_ _S_t_a_t_u_s_:_ _A_c_t_i_v_e_ _â___ _T_h_e_ _p_r_o_j_e_c_t_ _h_a_s_ _r_e_a_c_h_e_d_ _a_ _s_t_a_b_l_e_,_ _u_s_a_b_l_e_ _s_t_a_t_e_ _a_n_d
-            _i_s_ _b_e_i_n_g_ _a_c_t_i_v_e_l_y_ _d_e_v_e_l_o_p_e_d_]_[_C_o_d_e_ _s_t_y_l_e_]_[_M_y_p_y_ _c_h_e_c_k_e_d_]
+_i_s_ _b_e_i_n_g_ _a_c_t_i_v_e_l_y_ _d_e_v_e_l_o_p_e_d_]_[_C_o_d_e_ _s_t_y_l_e_]_[_M_y_p_y_ _c_h_e_c_k_e_d_]_[_P_y_t_h_o_n_ _V_e_r_s_i_o_n_s_]_[_P_a_c_k_a_g_e
+                            _v_e_r_s_i_o_n_]_[_C_o_d_e_ _c_o_v_e_r_a_g_e_]
 [//]: # (Using deprecated `align="center"` for the logo image and badges above,
 because of https://stackoverflow.com/a/62383408) # Overview _____ _Batchee_
 groups together filenames so that further operations (such as concatenation)
 can be performed separately on each group of files. ## Installing _____ For
 local development, one can clone the repository and then use poetry or pip from
 the local directory: ```shell git clone ``` ###### (Option A) using poetry: i)
 Follow the instructions for installing `poetry` [here](https://python-
```

### Comparing `batchee-1.0.0/batcher/harmony/cli.py` & `batchee-1.1.0/batcher/harmony/cli.py`

 * *Files identical despite different names*

### Comparing `batchee-1.0.0/batcher/harmony/service_adapter.py` & `batchee-1.1.0/batcher/harmony/service_adapter.py`

 * *Files identical despite different names*

### Comparing `batchee-1.0.0/batcher/harmony/util.py` & `batchee-1.1.0/batcher/harmony/util.py`

 * *Files identical despite different names*

### Comparing `batchee-1.0.0/batcher/tempo_filename_parser.py` & `batchee-1.1.0/batcher/tempo_filename_parser.py`

 * *Files identical despite different names*

### Comparing `batchee-1.0.0/pyproject.toml` & `batchee-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "batchee"
-version = "1.0.0"
+version = "1.1.0"
 description = "Determine how to group together input files into batches for subsequent concatenation"
 authors = ["Daniel Kaufman <daniel.kaufman@nasa.gov>"]
 readme = "README.md"
 classifiers = [
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
 packages = [
```

### Comparing `batchee-1.0.0/setup.py` & `batchee-1.1.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 
 entry_points = \
 {'console_scripts': ['batchee = batcher.tempo_filename_parser:main',
                      'batchee_harmony = batcher.harmony.cli:main']}
 
 setup_kwargs = {
     'name': 'batchee',
-    'version': '1.0.0',
+    'version': '1.1.0',
     'description': 'Determine how to group together input files into batches for subsequent concatenation',
-    'long_description': '<p align="center">\n    <img alt="batchee, a python package for grouping together filenames to enable subsequent batched operations (such as concatenation)."\n    src="https://github.com/danielfromearth/batchee/assets/114174502/8b1a92a5-eccc-4674-9c00-3698e752077e" width="250"\n    />\n</p>\n\n<p align="center">\n    <a href="https://www.repostatus.org/#active" target="_blank">\n        <img src="https://www.repostatus.org/badges/latest/active.svg" alt="Project Status: Active – The project has reached a stable, usable state and is being actively developed">\n    </a>\n    <a href="https://github.com/python/black" target="_blank">\n        <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Code style">\n    </a>\n    <a href="http://mypy-lang.org/" target="_blank">\n        <img src="http://www.mypy-lang.org/static/mypy_badge.svg" alt="Mypy checked">\n    </a>\n</p>\n\n[//]: # (Using deprecated `align="center"` for the logo image and badges above, because of https://stackoverflow.com/a/62383408)\n\n\n# Overview\n_____\n\n_Batchee_ groups together filenames so that further operations (such as concatenation) can be performed separately on each group of files.\n\n## Installing\n_____\n\nFor local development, one can clone the repository and then use poetry or pip from the local directory:\n\n```shell\ngit clone <Repository URL>\n```\n\n###### (Option A) using poetry:\ni) Follow the instructions for installing `poetry` [here](https://python-poetry.org/docs/).\n\nii) Run ```poetry install``` from the repository directory.\n\n###### (Option B) using pip: Run ```pip install .``` from the repository directory.\n\n## Usage\n_____\n\n```shell\nbatchee [file_names ...]\n```\n\n###### Or, If installed using a `poetry` environment:\n```shell\npoetry run batchee [file_names ...]\n```\n\n#### Options\n\n- `-h`, `--help`            show this help message and exit\n- `-v`, `--verbose`  Enable verbose output to stdout; useful for debugging\n\n---\nThis package is NASA Software Release Authorization (SRA) # LAR-20440-1\n',
+    'long_description': '<p align="center">\n    <img alt="batchee, a python package for grouping together filenames to enable subsequent batched operations (such as concatenation)."\n    src="https://github.com/danielfromearth/batchee/assets/114174502/8b1a92a5-eccc-4674-9c00-3698e752077e" width="250"\n    />\n</p>\n\n<p align="center">\n    <a href="https://www.repostatus.org/#active" target="_blank">\n        <img src="https://www.repostatus.org/badges/latest/active.svg" alt="Project Status: Active – The project has reached a stable, usable state and is being actively developed">\n    </a>\n    <a href="https://github.com/python/black" target="_blank">\n        <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Code style">\n    </a>\n    <a href="http://mypy-lang.org/" target="_blank">\n        <img src="http://www.mypy-lang.org/static/mypy_badge.svg" alt="Mypy checked">\n    </a>\n    <a href="https://pypi.org/project/batchee/" target="_blank">\n        <img src="https://img.shields.io/pypi/pyversions/batchee.svg" alt="Python Versions">\n    </a>\n    <a href="https://pypi.org/project/batchee" target="_blank">\n        <img src="https://img.shields.io/pypi/v/batchee?color=%2334D058label=pypi%20package" alt="Package version">\n    </a>\n    <a href="https://codecov.io/gh/nasa/batchee">\n     <img src="https://codecov.io/gh/nasa/batchee/graph/badge.svg?token=WDj92iN7c4" alt="Code coverage">\n    </a>\n</p>\n\n[//]: # (Using deprecated `align="center"` for the logo image and badges above, because of https://stackoverflow.com/a/62383408)\n\n\n# Overview\n_____\n\n_Batchee_ groups together filenames so that further operations (such as concatenation) can be performed separately on each group of files.\n\n## Installing\n_____\n\nFor local development, one can clone the repository and then use poetry or pip from the local directory:\n\n```shell\ngit clone <Repository URL>\n```\n\n###### (Option A) using poetry:\ni) Follow the instructions for installing `poetry` [here](https://python-poetry.org/docs/).\n\nii) Run ```poetry install``` from the repository directory.\n\n###### (Option B) using pip: Run ```pip install .``` from the repository directory.\n\n## Usage\n_____\n\n```shell\nbatchee [file_names ...]\n```\n\n###### Or, If installed using a `poetry` environment:\n```shell\npoetry run batchee [file_names ...]\n```\n\n#### Options\n\n- `-h`, `--help`            show this help message and exit\n- `-v`, `--verbose`  Enable verbose output to stdout; useful for debugging\n\n---\nThis package is NASA Software Release Authorization (SRA) # LAR-20440-1\n',
     'author': 'Daniel Kaufman',
     'author_email': 'daniel.kaufman@nasa.gov',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,20 +1,21 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['batcher',
 'batcher.harmony'] package_data = \ {'': ['*']} install_requires = \ ['harmony-
 service-lib>=1.0.26,<2.0.0'] entry_points = \ {'console_scripts': ['batchee =
 batcher.tempo_filename_parser:main', 'batchee_harmony = batcher.harmony.cli:
-main']} setup_kwargs = { 'name': 'batchee', 'version': '1.0.0', 'description':
+main']} setup_kwargs = { 'name': 'batchee', 'version': '1.1.0', 'description':
 'Determine how to group together input files into batches for subsequent
 concatenation', 'long_description': '
 \n n src="https://github.com/danielfromearth/batchee/assets/114174502/8b1a92a5-
                 eccc-4674-9c00-3698e752077e" width="250"\n />\n
 \n\n
   \n _\_n_ _[_P_r_o_j_e_c_t_ _S_t_a_t_u_s_:_ _A_c_t_i_v_e_ _â___ _T_h_e_ _p_r_o_j_e_c_t_ _h_a_s_ _r_e_a_c_h_e_d_ _a_ _s_t_a_b_l_e_,_ _u_s_a_b_l_e
    _s_t_a_t_e_ _a_n_d_ _i_s_ _b_e_i_n_g_ _a_c_t_i_v_e_l_y_ _d_e_v_e_l_o_p_e_d_]_\_n_ \n _\_n_ _[_C_o_d_e_ _s_t_y_l_e_]_\_n_ \n _\_n_ _[_M_y_p_y
-                                 _c_h_e_c_k_e_d_]_\_n_ \n
+  _c_h_e_c_k_e_d_]_\_n_ \n _\_n_ _[_P_y_t_h_o_n_ _V_e_r_s_i_o_n_s_]_\_n_ \n _\_n_ _[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_\_n_ \n _\_n_ _[_C_o_d_e
+                                _c_o_v_e_r_a_g_e_]_\_n_ \n
 \n\n[//]: # (Using deprecated `align="center"` for the logo image and badges
 above, because of https://stackoverflow.com/a/62383408)\n\n\n#
 Overview\n_____\n\n_Batchee_ groups together filenames so that further
 operations (such as concatenation) can be performed separately on each group of
 files.\n\n## Installing\n_____\n\nFor local development, one can clone the
 repository and then use poetry or pip from the local directory:
 \n\n```shell\ngit clone \n```\n\n###### (Option A) using poetry:\ni) Follow the
```

