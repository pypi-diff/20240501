# Comparing `tmp/join_eos_exif-1.1.2.tar.gz` & `tmp/join_eos_exif-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "join_eos_exif-1.1.2.tar", max compression
+gzip compressed data, was "join_eos_exif-1.2.0.tar", max compression
```

## Comparing `join_eos_exif-1.1.2.tar` & `join_eos_exif-1.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      447 2023-05-11 17:48:25.898827 join_eos_exif-1.1.2/README.md
--rw-r--r--   0        0        0     7315 2023-05-11 17:48:25.898827 join_eos_exif-1.1.2/join_eos_exif/OrthoRenamer.py
--rw-r--r--   0        0        0      136 2023-05-11 17:48:25.898827 join_eos_exif-1.1.2/join_eos_exif/__init__.py
--rw-r--r--   0        0        0      577 2023-05-11 17:51:10.846030 join_eos_exif-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     1175 1970-01-01 00:00:00.000000 join_eos_exif-1.1.2/setup.py
--rw-r--r--   0        0        0     1020 1970-01-01 00:00:00.000000 join_eos_exif-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0      434 2024-05-01 18:57:34.123518 join_eos_exif-1.2.0/README.md
+-rw-r--r--   0        0        0     7390 2024-05-01 18:57:34.127518 join_eos_exif-1.2.0/join_eos_exif/OrthoRenamer.py
+-rw-r--r--   0        0        0      136 2024-05-01 18:57:34.127518 join_eos_exif-1.2.0/join_eos_exif/__init__.py
+-rw-r--r--   0        0        0      582 2024-05-01 19:08:15.612523 join_eos_exif-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1159 1970-01-01 00:00:00.000000 join_eos_exif-1.2.0/setup.py
+-rw-r--r--   0        0        0     1007 1970-01-01 00:00:00.000000 join_eos_exif-1.2.0/PKG-INFO
```

### Comparing `join_eos_exif-1.1.2/join_eos_exif/OrthoRenamer.py` & `join_eos_exif-1.2.0/join_eos_exif/OrthoRenamer.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 import numpy as np
 import pandas as pd
 
 logger = logging.getLogger(__name__)
 
 
 class OrthoRenamer(ABC):
-    def __init__(self, verbose=True):
+    def __init__(self, out_suffix="_rgbi.tif", verbose=True):
         super().__init__()
+        self.out_suffix = out_suffix
         self.verbose = verbose
         self.errors = []  # list of filenames that can not be matched.
 
     @staticmethod
     def _get_eos_header_offset(filename: str) -> int:
         with open(filename) as f:
             lines = [line.strip() for line in f.readlines()]
@@ -87,15 +88,15 @@
             exif["GPS Event"], errors="coerce", downcast="integer"
         ).dropna()
 
         # Inner join on event #s
         joined = pd.merge(eos, exif, left_on="# EVENT", right_on="GPS Event")
 
         # Create updated filename column
-        joined["CIR_Filename"] = joined["Filename"].str[:-4] + "_rgbi.tif"
+        joined["CIR_Filename"] = joined["Filename"].str.replace(".IIQ", self.out_suffix)
 
         # Populate the errors list
         unmatched_exif = exif[(~exif["Filename"].isin(joined["Filename"]))]
         self.errors = list(unmatched_exif["Filename"])
 
         # Print some info
         num_matched = len(joined)
```

### Comparing `join_eos_exif-1.1.2/pyproject.toml` & `join_eos_exif-1.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "join-eos-exif"
-version = "v1.1.2"
+version = "v1.2.0"
 description = "Join EOS files to images using EXIF data"
 authors = ["Taylor Denouden <taylor.denouden@hakai.org>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "join_eos_exif"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.11"
 PyQt6 = "^6.4.0"
 numpy = "^1.23.5"
 pandas = "^2.0.1"
 
 [tool.poetry.group.dev.dependencies]
-black = "^23.3.0"
+black = ">=23.3,<25.0"
 pre-commit = "^3.3.1"
 pyinstaller = "^5.6.2"
 pytest = "^7.2.0"
 ruff = "^0.0.265"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `join_eos_exif-1.1.2/setup.py` & `join_eos_exif-1.2.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['PyQt6>=6.4.0,<7.0.0', 'numpy>=1.23.5,<2.0.0', 'pandas>=2.0.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'join-eos-exif',
-    'version': '1.1.2',
+    'version': '1.2.0',
     'description': 'Join EOS files to images using EXIF data',
-    'long_description': '# joinEOStoEXIF\n\nApplication to join EOS and EXIF data files for image processing\n\nUI made with PyQt5 v5.14.1\nexe generated using Pyinstaller 3.4\n\n## Installation\n\n```sh\npip install -r requirements.txt\n```\n\n## Running\n\nUse join_data.exe or\n\n```sh\npython join_data.py\n```\n\n## Tests\n\nThe test.py file runs tests on sample input files stored in the sample_files folder.\n\nIt looks for one CSV and one txt file in each folder\n\n```sh\npython test.py\n```\n',
+    'long_description': '# EOS-EXIF-Join\n\nApplication to join EOS and EXIF data files for image processing\n\nUI made with PyQt6\nexe generated using Pyinstaller\n\n## Installation\n\nInstall the poetry package manager then:\n\n```sh\npoetry install\n```\n\n## Running\n\nUse join_data.exe or\n\n```sh\npoetry run python -m gui\n```\n\n## Building\n\nBuilds are done automatically with GitHub Actions when pushing a tag with a semantic\nversion formats like `vN.N.N` or `vN.N.N-rcN`\n',
     'author': 'Taylor Denouden',
     'author_email': 'taylor.denouden@hakai.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `join_eos_exif-1.1.2/PKG-INFO` & `join_eos_exif-1.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,48 +1,45 @@
 Metadata-Version: 2.1
 Name: join-eos-exif
-Version: 1.1.2
+Version: 1.2.0
 Summary: Join EOS files to images using EXIF data
 License: MIT
 Author: Taylor Denouden
 Author-email: taylor.denouden@hakai.org
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: PyQt6 (>=6.4.0,<7.0.0)
 Requires-Dist: numpy (>=1.23.5,<2.0.0)
 Requires-Dist: pandas (>=2.0.1,<3.0.0)
 Description-Content-Type: text/markdown
 
-# joinEOStoEXIF
+# EOS-EXIF-Join
 
 Application to join EOS and EXIF data files for image processing
 
-UI made with PyQt5 v5.14.1
-exe generated using Pyinstaller 3.4
+UI made with PyQt6
+exe generated using Pyinstaller
 
 ## Installation
 
+Install the poetry package manager then:
+
 ```sh
-pip install -r requirements.txt
+poetry install
 ```
 
 ## Running
 
 Use join_data.exe or
 
 ```sh
-python join_data.py
+poetry run python -m gui
 ```
 
-## Tests
-
-The test.py file runs tests on sample input files stored in the sample_files folder.
-
-It looks for one CSV and one txt file in each folder
+## Building
 
-```sh
-python test.py
-```
+Builds are done automatically with GitHub Actions when pushing a tag with a semantic
+version formats like `vN.N.N` or `vN.N.N-rcN`
```

