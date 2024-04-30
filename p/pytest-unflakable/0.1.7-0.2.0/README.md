# Comparing `tmp/pytest-unflakable-0.1.7.tar.gz` & `tmp/pytest_unflakable-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-unflakable-0.1.7.tar", last modified: Sun Nov 12 12:04:18 2023, max compression
+gzip compressed data, was "pytest_unflakable-0.2.0.tar", last modified: Tue Apr 30 23:43:46 2024, max compression
```

## Comparing `pytest-unflakable-0.1.7.tar` & `pytest_unflakable-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 12:04:18.888563 pytest-unflakable-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2023-11-12 12:04:05.000000 pytest-unflakable-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-11-12 12:04:05.000000 pytest-unflakable-0.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2023-11-12 12:04:18.888563 pytest-unflakable-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2023-11-12 12:04:05.000000 pytest-unflakable-0.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       85 2023-11-12 12:04:05.000000 pytest-unflakable-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2023-11-12 12:04:18.888563 pytest-unflakable-0.1.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 12:04:18.884564 pytest-unflakable-0.1.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 12:04:18.888563 pytest-unflakable-0.1.7/src/pytest_unflakable/
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2023-11-12 12:04:05.000000 pytest-unflakable-0.1.7/src/pytest_unflakable/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     6952 2023-11-12 12:04:05.000000 pytest-unflakable-0.1.7/src/pytest_unflakable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7545 2023-11-12 12:04:05.000000 pytest-unflakable-0.1.7/src/pytest_unflakable/_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2023-11-12 12:04:05.000000 pytest-unflakable-0.1.7/src/pytest_unflakable/_git.py
--rw-r--r--   0 runner    (1001) docker     (127)    26344 2023-11-12 12:04:05.000000 pytest-unflakable-0.1.7/src/pytest_unflakable/_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 12:04:18.888563 pytest-unflakable-0.1.7/src/pytest_unflakable.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2023-11-12 12:04:18.000000 pytest-unflakable-0.1.7/src/pytest_unflakable.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      510 2023-11-12 12:04:18.000000 pytest-unflakable-0.1.7/src/pytest_unflakable.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-12 12:04:18.000000 pytest-unflakable-0.1.7/src/pytest_unflakable.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2023-11-12 12:04:18.000000 pytest-unflakable-0.1.7/src/pytest_unflakable.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-11-12 12:04:18.000000 pytest-unflakable-0.1.7/src/pytest_unflakable.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-11-12 12:04:18.000000 pytest-unflakable-0.1.7/src/pytest_unflakable.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 12:04:18.888563 pytest-unflakable-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    71558 2023-11-12 12:04:05.000000 pytest-unflakable-0.1.7/tests/test_unflakable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:43:46.311634 pytest_unflakable-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-30 23:43:31.000000 pytest_unflakable-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-30 23:43:31.000000 pytest_unflakable-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-04-30 23:43:46.311634 pytest_unflakable-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-04-30 23:43:31.000000 pytest_unflakable-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-30 23:43:31.000000 pytest_unflakable-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-30 23:43:46.311634 pytest_unflakable-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:43:46.307634 pytest_unflakable-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:43:46.311634 pytest_unflakable-0.2.0/src/pytest_unflakable/
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-30 23:43:31.000000 pytest_unflakable-0.2.0/src/pytest_unflakable/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6952 2024-04-30 23:43:31.000000 pytest_unflakable-0.2.0/src/pytest_unflakable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7501 2024-04-30 23:43:31.000000 pytest_unflakable-0.2.0/src/pytest_unflakable/_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-30 23:43:31.000000 pytest_unflakable-0.2.0/src/pytest_unflakable/_git.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26340 2024-04-30 23:43:31.000000 pytest_unflakable-0.2.0/src/pytest_unflakable/_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:43:46.311634 pytest_unflakable-0.2.0/src/pytest_unflakable.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-04-30 23:43:46.000000 pytest_unflakable-0.2.0/src/pytest_unflakable.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-30 23:43:46.000000 pytest_unflakable-0.2.0/src/pytest_unflakable.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 23:43:46.000000 pytest_unflakable-0.2.0/src/pytest_unflakable.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-30 23:43:46.000000 pytest_unflakable-0.2.0/src/pytest_unflakable.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-30 23:43:46.000000 pytest_unflakable-0.2.0/src/pytest_unflakable.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-30 23:43:46.000000 pytest_unflakable-0.2.0/src/pytest_unflakable.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:43:46.311634 pytest_unflakable-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    73317 2024-04-30 23:43:31.000000 pytest_unflakable-0.2.0/tests/test_unflakable.py
```

### Comparing `pytest-unflakable-0.1.7/LICENSE` & `pytest_unflakable-0.2.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022-2023 Developer Innovations, LLC
+Copyright (c) 2022-2024 Developer Innovations, LLC
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pytest-unflakable-0.1.7/PKG-INFO` & `pytest_unflakable-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-unflakable
-Version: 0.1.7
+Version: 0.2.0
 Summary: Unflakable plugin for PyTest
 Home-page: https://unflakable.com
 Author: Unflakable
 Author-email: support@unflakable.com
 Maintainer: Unflakable
 Maintainer-email: support@unflakable.com
 License: MIT
@@ -12,29 +12,30 @@
 Project-URL: Documentation, https://docs.unflakable.com/plugins/pytest
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Testing
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pytest>=6.2.0
 Requires-Dist: requests>=2.19.0
 Provides-Extra: dev
-Requires-Dist: requests-mock[fixture]; extra == "dev"
+Requires-Dist: freezegun>=1.2.2; extra == "dev"
+Requires-Dist: requests-mock[fixture]==1.11.0; extra == "dev"
 
 <p align="center">
   <a href="https://unflakable.com" target="_blank" rel="noopener" align="center">
     <img src="https://github.com/unflakable/unflakable-python/blob/main/images/logo.svg?raw=true" width="350" alt="Unflakable" />
   </a>
 </p>
```

#### html2text {}

```diff
@@ -1,25 +1,25 @@
-Metadata-Version: 2.1 Name: pytest-unflakable Version: 0.1.7 Summary:
+Metadata-Version: 2.1 Name: pytest-unflakable Version: 0.2.0 Summary:
 Unflakable plugin for PyTest Home-page: https://unflakable.com Author:
 Unflakable Author-email: support@unflakable.com Maintainer: Unflakable
 Maintainer-email: support@unflakable.com License: MIT Project-URL: Repository,
 https://github.com/unflakable/unflakable-python Project-URL: Documentation,
 https://docs.unflakable.com/plugins/pytest Classifier: Development Status :: 4
 - Beta Classifier: Framework :: Pytest Classifier: Intended Audience ::
 Developers Classifier: Topic :: Software Development :: Testing Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3 ::
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3.12 Classifier: Programming Language :: Python :: 3 ::
 Only Classifier: Operating System :: OS Independent Classifier: License :: OSI
-Approved :: MIT License Requires-Python: >=3.7 Description-Content-Type: text/
+Approved :: MIT License Requires-Python: >=3.8 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: pytest>=6.2.0 Requires-Dist:
-requests>=2.19.0 Provides-Extra: dev Requires-Dist: requests-mock[fixture];
-extra == "dev"
+requests>=2.19.0 Provides-Extra: dev Requires-Dist: freezegun>=1.2.2; extra ==
+"dev" Requires-Dist: requests-mock[fixture]==1.11.0; extra == "dev"
                                  _[_U_n_f_l_a_k_a_b_l_e_]
 [![PyPI version](https://img.shields.io/pypi/v/pytest-unflakable.svg)](https://
 pypi.org/project/pytest-unflakable) # Unflakable Plugin for PyTest This
 Unflakable plugin enables users of the [PyTest](https://pytest.org) Python test
 framework to quarantine flaky tests and track test results. Refer to the
 [PyTest Plugin](https://docs.unflakable.com/plugins/pytest) documentation for
 complete usage instructions. Users of the Python [`unittest` unit testing
```

### Comparing `pytest-unflakable-0.1.7/README.md` & `pytest_unflakable-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,14 @@
 for running `unittest` tests.
 
 ### Compatibility
 
 This plugin maintains compatibility with the PyTest and Python versions listed below:
 
 ![Python versions](https://img.shields.io/pypi/pyversions/pytest-unflakable)
-![PyTest versions](https://img.shields.io/badge/pytest-6.2%20%7C%207.0%20%7C%207.1%20%7C%207.2%20%7C%207.3%20%7C%207.4-blue)
+![PyTest versions](https://img.shields.io/badge/pytest-6.2%20%7C%207.0%20%7C%207.1%20%7C%207.2%20%7C%207.3%20%7C%207.4%20%7C%208.0%20%7C%208.1%20%7C%208.2-blue)
 
 ## Contributing
 
 To report a bug or request a new feature, please
 [file a GitHub issue](https://github.com/unflakable/unflakable-python/issues).
 We also welcome pull requests!
```

#### html2text {}

```diff
@@ -11,11 +11,11 @@
 instructions. Users of the Python [`unittest` unit testing framework](https://
 docs.python.org/3/library/unittest.html) may use this plugin by leveraging
 PyTest's [out-of-the-box support](https://docs.pytest.org/how-to/unittest.html)
 for running `unittest` tests. ### Compatibility This plugin maintains
 compatibility with the PyTest and Python versions listed below: ![Python
 versions](https://img.shields.io/pypi/pyversions/pytest-unflakable) ![PyTest
 versions](https://img.shields.io/badge/pytest-
-6.2%20%7C%207.0%20%7C%207.1%20%7C%207.2%20%7C%207.3%20%7C%207.4-blue) ##
-Contributing To report a bug or request a new feature, please [file a GitHub
-issue](https://github.com/unflakable/unflakable-python/issues). We also welcome
-pull requests!
+6.2%20%7C%207.0%20%7C%207.1%20%7C%207.2%20%7C%207.3%20%7C%207.4%20%7C%208.0%20%7C%208.1%20%7C%208.2-
+blue) ## Contributing To report a bug or request a new feature, please [file a
+GitHub issue](https://github.com/unflakable/unflakable-python/issues). We also
+welcome pull requests!
```

### Comparing `pytest-unflakable-0.1.7/setup.cfg` & `pytest_unflakable-0.2.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pytest-unflakable
-version = 0.1.7
+version = 0.2.0
 author = Unflakable
 author_email = support@unflakable.com
 maintainer = Unflakable
 maintainer_email = support@unflakable.com
 license = MIT
 license_files = 
 	LICENSE
@@ -18,36 +18,37 @@
 classifiers = 
 	Development Status :: 4 - Beta
 	Framework :: Pytest
 	Intended Audience :: Developers
 	Topic :: Software Development :: Testing
 	Programming Language :: Python
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Programming Language :: Python :: 3 :: Only
 	Operating System :: OS Independent
 	License :: OSI Approved :: MIT License
 
 [options]
 package_dir = 
 	=src
 packages = 
 	pytest_unflakable
-python_requires = >=3.7
+python_requires = >=3.8
 install_requires = 
 	pytest>=6.2.0
 	requests>=2.19.0
 
 [options.extras_require]
 dev = 
-	requests-mock[fixture]
+	freezegun>=1.2.2
+	requests-mock[fixture]==1.11.0
 
 [options.entry_points]
 pytest11 = 
 	unflakable = pytest_unflakable
 
 [egg_info]
 tag_build =
```

### Comparing `pytest-unflakable-0.1.7/src/pytest_unflakable/README.md` & `pytest_unflakable-0.2.0/src/pytest_unflakable/README.md`

 * *Files identical despite different names*

### Comparing `pytest-unflakable-0.1.7/src/pytest_unflakable/__init__.py` & `pytest_unflakable-0.2.0/src/pytest_unflakable/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Unflakable plugin for PyTest."""
 
-#  Copyright (c) 2022-2023 Developer Innovations, LLC
+#  Copyright (c) 2022-2024 Developer Innovations, LLC
 
 import argparse
 import logging
 import os
 import pprint
 import sys
 from typing import TYPE_CHECKING
```

### Comparing `pytest-unflakable-0.1.7/src/pytest_unflakable/_api.py` & `pytest_unflakable-0.2.0/src/pytest_unflakable/_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 """Unflakable API."""
 
-#  Copyright (c) 2022-2023 Developer Innovations, LLC
+#  Copyright (c) 2022-2024 Developer Innovations, LLC
 
 from __future__ import annotations
 
 import gzip
 import json
 import logging
 import platform
 import pprint
 import sys
 import time
+from importlib.metadata import version
 from typing import TYPE_CHECKING, List, Mapping, Optional
 
-import pkg_resources
 import requests
 from requests import HTTPError, Response, Session
 
 if TYPE_CHECKING:
     from typing_extensions import NotRequired, TypedDict
 else:
     from typing import Dict
 
     NotRequired = Optional
     TypedDict = Dict
 
 BASE_URL = 'https://app.unflakable.com'
 TEST_NAME_ENTRY_MAX_LENGTH = 4096
-PACKAGE_VERSION = pkg_resources.get_distribution('pytest_unflakable').version
+PACKAGE_VERSION = version('pytest_unflakable')
 PLATFORM_VERSION = platform.platform()
-PYTEST_VERSION = pkg_resources.get_distribution('pytest').version
+PYTEST_VERSION = version('pytest')
 PYTHON_VERSION = f'{sys.version_info.major}.{sys.version_info.minor}.{sys.version_info.micro}'
 USER_AGENT = (
     f'unflakable-pytest-plugin/{PACKAGE_VERSION} (PyTest {PYTEST_VERSION}; '
     f'Python {PYTHON_VERSION}; Platform {PLATFORM_VERSION})'
 )
 NUM_REQUEST_TRIES = 3
```

### Comparing `pytest-unflakable-0.1.7/src/pytest_unflakable/_git.py` & `pytest_unflakable-0.2.0/src/pytest_unflakable/_git.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright (c) 2022-2023 Developer Innovations, LLC
+#  Copyright (c) 2022-2024 Developer Innovations, LLC
 
 import logging
 import sys
 from subprocess import run
 from typing import List, Optional
 
 GIT_ERROR_STR = 'WARNING: Unflakable failed to auto-detect current git branch and commit'
```

### Comparing `pytest-unflakable-0.1.7/src/pytest_unflakable/_plugin.py` & `pytest_unflakable-0.2.0/src/pytest_unflakable/_plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Plugin implementation."""
 
-#  Copyright (c) 2022-2023 Developer Innovations, LLC
+#  Copyright (c) 2022-2024 Developer Innovations, LLC
 
 import logging
 from datetime import datetime, timezone
 from enum import Enum
 from pathlib import Path
 from time import time
 from typing import (TYPE_CHECKING, Any, Dict, Generator, List, Mapping,
@@ -582,15 +582,15 @@
         request.update(**({'commit': self.commit} if self.commit is not None else {}))
 
         return cast(CreateTestSuiteRunInlineRequest, request)
 
     # Allows us to override the exit code if all the failures are quarantined. We need this to be a
     # wrapper so that the default hook still gets invoked and prints the summary line with the test
     # category counts.
-    @pytest.hookimpl(hookwrapper=True, tryfirst=True)
+    @pytest.hookimpl(wrapper=True, tryfirst=True)
     def pytest_sessionfinish(
             self,
             session: pytest.Session,
             exitstatus: int,
     ) -> Generator[None, None, None]:
         self.end_time = time()
         self.logger.debug('called hook pytest_sessionfinish')
```

### Comparing `pytest-unflakable-0.1.7/src/pytest_unflakable.egg-info/PKG-INFO` & `pytest_unflakable-0.2.0/src/pytest_unflakable.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-unflakable
-Version: 0.1.7
+Version: 0.2.0
 Summary: Unflakable plugin for PyTest
 Home-page: https://unflakable.com
 Author: Unflakable
 Author-email: support@unflakable.com
 Maintainer: Unflakable
 Maintainer-email: support@unflakable.com
 License: MIT
@@ -12,29 +12,30 @@
 Project-URL: Documentation, https://docs.unflakable.com/plugins/pytest
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Testing
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pytest>=6.2.0
 Requires-Dist: requests>=2.19.0
 Provides-Extra: dev
-Requires-Dist: requests-mock[fixture]; extra == "dev"
+Requires-Dist: freezegun>=1.2.2; extra == "dev"
+Requires-Dist: requests-mock[fixture]==1.11.0; extra == "dev"
 
 <p align="center">
   <a href="https://unflakable.com" target="_blank" rel="noopener" align="center">
     <img src="https://github.com/unflakable/unflakable-python/blob/main/images/logo.svg?raw=true" width="350" alt="Unflakable" />
   </a>
 </p>
```

#### html2text {}

```diff
@@ -1,25 +1,25 @@
-Metadata-Version: 2.1 Name: pytest-unflakable Version: 0.1.7 Summary:
+Metadata-Version: 2.1 Name: pytest-unflakable Version: 0.2.0 Summary:
 Unflakable plugin for PyTest Home-page: https://unflakable.com Author:
 Unflakable Author-email: support@unflakable.com Maintainer: Unflakable
 Maintainer-email: support@unflakable.com License: MIT Project-URL: Repository,
 https://github.com/unflakable/unflakable-python Project-URL: Documentation,
 https://docs.unflakable.com/plugins/pytest Classifier: Development Status :: 4
 - Beta Classifier: Framework :: Pytest Classifier: Intended Audience ::
 Developers Classifier: Topic :: Software Development :: Testing Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3 ::
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3.12 Classifier: Programming Language :: Python :: 3 ::
 Only Classifier: Operating System :: OS Independent Classifier: License :: OSI
-Approved :: MIT License Requires-Python: >=3.7 Description-Content-Type: text/
+Approved :: MIT License Requires-Python: >=3.8 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: pytest>=6.2.0 Requires-Dist:
-requests>=2.19.0 Provides-Extra: dev Requires-Dist: requests-mock[fixture];
-extra == "dev"
+requests>=2.19.0 Provides-Extra: dev Requires-Dist: freezegun>=1.2.2; extra ==
+"dev" Requires-Dist: requests-mock[fixture]==1.11.0; extra == "dev"
                                  _[_U_n_f_l_a_k_a_b_l_e_]
 [![PyPI version](https://img.shields.io/pypi/v/pytest-unflakable.svg)](https://
 pypi.org/project/pytest-unflakable) # Unflakable Plugin for PyTest This
 Unflakable plugin enables users of the [PyTest](https://pytest.org) Python test
 framework to quarantine flaky tests and track test results. Refer to the
 [PyTest Plugin](https://docs.unflakable.com/plugins/pytest) documentation for
 complete usage instructions. Users of the Python [`unittest` unit testing
```

### Comparing `pytest-unflakable-0.1.7/tests/test_unflakable.py` & `pytest_unflakable-0.2.0/tests/test_unflakable.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Tests for pytest_unflakable plugin."""
 
-#  Copyright (c) 2022-2023 Developer Innovations, LLC
+#  Copyright (c) 2022-2024 Developer Innovations, LLC
 
 import os
 import platform
 import re
 import sys
+from importlib.metadata import version
 
-import pkg_resources
 import pytest
 from _pytest.config import ExitCode
 
 from pytest_unflakable import _api
 
 from .common import (GitMock, MonkeyPatch, _TestAttemptOutcome,
                      _TestResultCounts, run_test_case)
@@ -26,15 +26,15 @@
 @pytest.fixture(params=[f'py{sys.version_info.major}.{sys.version_info.minor}'], autouse=True)
 def _1python_version() -> None:
     pass
 
 
 __PYTEST_MINOR_VERSION_MATCH = re.match(
     r'^([0-9]+\.[0-9]+)\..*$',
-    pkg_resources.get_distribution('pytest').version,
+    version('pytest'),
 )
 assert __PYTEST_MINOR_VERSION_MATCH is not None
 __PYTEST_MINOR_VERSION = __PYTEST_MINOR_VERSION_MATCH.group(1)
 
 
 @pytest.fixture(params=[f'pytest{__PYTEST_MINOR_VERSION}'], autouse=True)
 def _2pytest_version() -> None:
@@ -2251,7 +2251,61 @@
         expected_exit_code=ExitCode.OK,
         expected_branch=None,
         expected_commit=None,
         expect_xdist=xdist,
         extra_args=XDIST_ARGS if xdist else [],
         failed_upload_requests=1,
     )
+
+
+@pytest.mark.parametrize(TEST_PARAMS_VERBOSE_XDIST_ARG_NAMES,
+                         TEST_PARAMS_VERBOSE_XDIST_ARG_VALUES)
+def test_freeze_time(
+    pytester: pytest.Pytester,
+    subprocess_mock: GitMock,
+    verbose: bool,
+    xdist: bool,
+) -> None:
+    pytester.makepyfile(test_input="""
+        from freezegun import freeze_time
+        import unittest
+
+        @freeze_time("2023-02-04")
+        class FrozenTimeTests(unittest.TestCase):
+            @freeze_time("2024-01-01")
+            def test_pass(self):
+                pass
+
+            @freeze_time("2024-01-02")
+            def test_pass2(self):
+                pass
+
+            @freeze_time("2024-01-03")
+            def test_pass3(self):
+                pass
+    """)
+
+    subprocess_mock.update(branch=None, commit=None)
+
+    run_test_case(
+        pytester,
+        manifest={'quarantined_tests': []},
+        expected_test_file_outcomes=[
+            ('test_input.py', [
+                (('FrozenTimeTests', 'test_pass'), [_TestAttemptOutcome.PASSED]),
+                (('FrozenTimeTests', 'test_pass2'), [_TestAttemptOutcome.PASSED]),
+                (('FrozenTimeTests', 'test_pass3'), [_TestAttemptOutcome.PASSED]),
+            ])
+        ],
+        expected_test_result_counts=_TestResultCounts(num_passed=3),
+        expected_uploaded_test_runs={
+            ('test_input.py', ('FrozenTimeTests', 'test_pass')): ['pass'],
+            ('test_input.py', ('FrozenTimeTests', 'test_pass2')): ['pass'],
+            ('test_input.py', ('FrozenTimeTests', 'test_pass3')): ['pass'],
+        },
+        expected_exit_code=ExitCode.OK,
+        expected_branch=None,
+        expected_commit=None,
+        expect_xdist=xdist,
+        extra_args=XDIST_ARGS if xdist else [],
+        verbose=verbose,
+    )
```

