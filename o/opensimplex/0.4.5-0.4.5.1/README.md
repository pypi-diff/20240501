# Comparing `tmp/opensimplex-0.4.5.tar.gz` & `tmp/opensimplex-0.4.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opensimplex-0.4.5.tar", last modified: Sun Jul  9 13:37:15 2023, max compression
+gzip compressed data, was "opensimplex-0.4.5.1.tar", last modified: Wed May  1 13:53:31 2024, max compression
```

## Comparing `opensimplex-0.4.5.tar` & `opensimplex-0.4.5.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 lmas      (1001) lmas      (1001)        0 2023-07-09 13:37:15.344821 opensimplex-0.4.5/
--rw-r--r--   0 lmas      (1001) lmas      (1001)     1074 2022-06-08 13:33:35.000000 opensimplex-0.4.5/LICENSE
--rw-r--r--   0 lmas      (1001) lmas      (1001)       16 2023-04-02 17:34:20.000000 opensimplex-0.4.5/MANIFEST.in
--rw-r--r--   0 lmas      (1001) lmas      (1001)    10793 2023-07-09 13:37:15.344512 opensimplex-0.4.5/PKG-INFO
--rw-r--r--   0 lmas      (1001) lmas      (1001)    10141 2023-06-13 12:14:46.000000 opensimplex-0.4.5/README.md
-drwxr-xr-x   0 lmas      (1001) lmas      (1001)        0 2023-07-09 13:37:15.342371 opensimplex-0.4.5/opensimplex/
--rw-r--r--   0 lmas      (1001) lmas      (1001)       62 2023-04-02 17:37:23.000000 opensimplex-0.4.5/opensimplex/__init__.py
--rw-r--r--   0 lmas      (1001) lmas      (1001)     5878 2023-02-18 14:27:39.000000 opensimplex-0.4.5/opensimplex/api.py
--rw-r--r--   0 lmas      (1001) lmas      (1001)     2651 2022-08-05 16:56:16.000000 opensimplex-0.4.5/opensimplex/constants.py
--rw-r--r--   0 lmas      (1001) lmas      (1001)    71171 2022-08-05 16:56:16.000000 opensimplex-0.4.5/opensimplex/internals.py
-drwxr-xr-x   0 lmas      (1001) lmas      (1001)        0 2023-07-09 13:37:15.343320 opensimplex-0.4.5/opensimplex.egg-info/
--rw-r--r--   0 lmas      (1001) lmas      (1001)    10793 2023-07-09 13:37:14.000000 opensimplex-0.4.5/opensimplex.egg-info/PKG-INFO
--rw-r--r--   0 lmas      (1001) lmas      (1001)      459 2023-07-09 13:37:15.000000 opensimplex-0.4.5/opensimplex.egg-info/SOURCES.txt
--rw-r--r--   0 lmas      (1001) lmas      (1001)        1 2023-07-09 13:37:14.000000 opensimplex-0.4.5/opensimplex.egg-info/dependency_links.txt
--rw-r--r--   0 lmas      (1001) lmas      (1001)        1 2023-07-09 13:25:36.000000 opensimplex-0.4.5/opensimplex.egg-info/not-zip-safe
--rw-r--r--   0 lmas      (1001) lmas      (1001)       12 2023-07-09 13:37:15.000000 opensimplex-0.4.5/opensimplex.egg-info/requires.txt
--rw-r--r--   0 lmas      (1001) lmas      (1001)       18 2023-07-09 13:37:15.000000 opensimplex-0.4.5/opensimplex.egg-info/top_level.txt
--rw-r--r--   0 lmas      (1001) lmas      (1001)       38 2023-07-09 13:37:15.344891 opensimplex-0.4.5/setup.cfg
--rw-r--r--   0 lmas      (1001) lmas      (1001)     1051 2022-08-07 14:30:42.000000 opensimplex-0.4.5/setup.py
-drwxr-xr-x   0 lmas      (1001) lmas      (1001)        0 2023-07-09 13:37:15.344235 opensimplex-0.4.5/tests/
--rw-r--r--   0 lmas      (1001) lmas      (1001)        0 2022-06-08 13:33:35.000000 opensimplex-0.4.5/tests/__init__.py
--rw-r--r--   0 lmas      (1001) lmas      (1001)     1420 2022-08-05 16:56:16.000000 opensimplex-0.4.5/tests/benchmark_opensimplex.py
--rw-r--r--   0 lmas      (1001) lmas      (1001)    12976 2022-08-05 16:56:16.000000 opensimplex-0.4.5/tests/numpy_shapes.npz
--rw-r--r--   0 lmas      (1001) lmas      (1001)   235060 2022-06-08 13:33:35.000000 opensimplex-0.4.5/tests/samples.json.gz
--rw-r--r--   0 lmas      (1001) lmas      (1001)     3401 2023-02-18 14:27:39.000000 opensimplex-0.4.5/tests/test_opensimplex.py
+drwxr-xr-x   0 lmas      (1001) lmas      (1001)        0 2024-05-01 13:53:31.456239 opensimplex-0.4.5.1/
+-rw-r--r--   0 lmas      (1001) lmas      (1001)     1074 2023-11-22 20:46:40.000000 opensimplex-0.4.5.1/LICENSE
+-rw-r--r--   0 lmas      (1001) lmas      (1001)       16 2023-11-22 20:46:40.000000 opensimplex-0.4.5.1/MANIFEST.in
+-rw-r--r--   0 lmas      (1001) lmas      (1001)    10587 2024-05-01 13:53:31.456046 opensimplex-0.4.5.1/PKG-INFO
+-rw-r--r--   0 lmas      (1001) lmas      (1001)     9927 2024-05-01 13:47:13.000000 opensimplex-0.4.5.1/README.md
+drwxr-xr-x   0 lmas      (1001) lmas      (1001)        0 2024-05-01 13:53:31.454669 opensimplex-0.4.5.1/opensimplex/
+-rw-r--r--   0 lmas      (1001) lmas      (1001)       64 2024-05-01 13:39:54.000000 opensimplex-0.4.5.1/opensimplex/__init__.py
+-rw-r--r--   0 lmas      (1001) lmas      (1001)     5880 2024-05-01 13:00:20.000000 opensimplex-0.4.5.1/opensimplex/api.py
+-rw-r--r--   0 lmas      (1001) lmas      (1001)     2651 2023-11-22 20:46:40.000000 opensimplex-0.4.5.1/opensimplex/constants.py
+-rw-r--r--   0 lmas      (1001) lmas      (1001)    71171 2023-11-22 20:46:40.000000 opensimplex-0.4.5.1/opensimplex/internals.py
+drwxr-xr-x   0 lmas      (1001) lmas      (1001)        0 2024-05-01 13:53:31.455276 opensimplex-0.4.5.1/opensimplex.egg-info/
+-rw-r--r--   0 lmas      (1001) lmas      (1001)    10587 2024-05-01 13:53:31.000000 opensimplex-0.4.5.1/opensimplex.egg-info/PKG-INFO
+-rw-r--r--   0 lmas      (1001) lmas      (1001)      459 2024-05-01 13:53:31.000000 opensimplex-0.4.5.1/opensimplex.egg-info/SOURCES.txt
+-rw-r--r--   0 lmas      (1001) lmas      (1001)        1 2024-05-01 13:53:31.000000 opensimplex-0.4.5.1/opensimplex.egg-info/dependency_links.txt
+-rw-r--r--   0 lmas      (1001) lmas      (1001)        1 2024-05-01 13:51:21.000000 opensimplex-0.4.5.1/opensimplex.egg-info/not-zip-safe
+-rw-r--r--   0 lmas      (1001) lmas      (1001)       12 2024-05-01 13:53:31.000000 opensimplex-0.4.5.1/opensimplex.egg-info/requires.txt
+-rw-r--r--   0 lmas      (1001) lmas      (1001)       18 2024-05-01 13:53:31.000000 opensimplex-0.4.5.1/opensimplex.egg-info/top_level.txt
+-rw-r--r--   0 lmas      (1001) lmas      (1001)       38 2024-05-01 13:53:31.456284 opensimplex-0.4.5.1/setup.cfg
+-rw-r--r--   0 lmas      (1001) lmas      (1001)     1057 2024-05-01 12:06:16.000000 opensimplex-0.4.5.1/setup.py
+drwxr-xr-x   0 lmas      (1001) lmas      (1001)        0 2024-05-01 13:53:31.455843 opensimplex-0.4.5.1/tests/
+-rw-r--r--   0 lmas      (1001) lmas      (1001)        0 2023-11-22 20:46:40.000000 opensimplex-0.4.5.1/tests/__init__.py
+-rw-r--r--   0 lmas      (1001) lmas      (1001)     1420 2023-11-22 20:46:40.000000 opensimplex-0.4.5.1/tests/benchmark_opensimplex.py
+-rw-r--r--   0 lmas      (1001) lmas      (1001)    12976 2023-11-22 20:46:40.000000 opensimplex-0.4.5.1/tests/numpy_shapes.npz
+-rw-r--r--   0 lmas      (1001) lmas      (1001)   235060 2023-11-22 20:46:40.000000 opensimplex-0.4.5.1/tests/samples.json.gz
+-rw-r--r--   0 lmas      (1001) lmas      (1001)     3401 2023-11-22 20:46:40.000000 opensimplex-0.4.5.1/tests/test_opensimplex.py
```

### Comparing `opensimplex-0.4.5/LICENSE` & `opensimplex-0.4.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `opensimplex-0.4.5/PKG-INFO` & `opensimplex-0.4.5.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: opensimplex
-Version: 0.4.5
+Version: 0.4.5.1
 Summary: OpenSimplex is a noise generation function like Perlin or Simplex noise, but better.
-Home-page: https://github.com/lmas/opensimplex
-Download-URL: https://github.com/lmas/opensimplex/releases
+Home-page: https://code.larus.se/lmas/opensimplex
+Download-URL: https://code.larus.se/lmas/opensimplex/releases
 Author: Alex
 Author-email: opensimplex@larus.se
 License: MIT
 Keywords: opensimplex simplex noise 2D 3D 4D
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,15 +15,14 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # OpenSimplex Noise
 
-[![build-status](https://github.com/lmas/opensimplex/workflows/Tests/badge.svg?branch=master)](https://github.com/lmas/opensimplex/actions)
 [![pypi-version](https://img.shields.io/pypi/v/opensimplex?label=Version)](https://pypi.org/project/opensimplex/)
 [![pypi-downloads](https://img.shields.io/pypi/dm/opensimplex?label=Downloads)](https://pypistats.org/packages/opensimplex)
 
 [OpenSimplex] is a noise generation function like [Perlin] or [Simplex] noise, but better.
 
     OpenSimplex noise is an n-dimensional gradient noise function that was
     developed in order to overcome the patent-related issues surrounding
@@ -38,24 +37,22 @@
 [Perlin]: https://en.wikipedia.org/wiki/Perlin_noise
 [Simplex]: https://en.wikipedia.org/wiki/Simplex_noise
 [original code]: https://gist.github.com/KdotJPG/b1270127455a94ac5d19
 
 ## Status
 
 The `master` branch contains the latest code (possibly unstable),
-with automatic tests running for **Python 3.8, 3.9, 3.10 on Linux, MacOS and Windows**.
-**FreeBSD** is also supported, though it's only locally tested as Github Actions
-don't offer FreeBSD support.
+please refer to the [version tags] for the latest stable version.
+An old, archived copy can be found at [Github].
 
-Please refer to the [version tags] for the latest stable version.
+[version tags]: https://code.larus.se/lmas/opensimplex/tags
+[Github]: https://github.com/lmas/opensimplex
 
-[version tags]: https://github.com/lmas/opensimplex/tags
 
-
-Updates for **v0.4+**:
+Updates for **v0.4.***:
 
 - Adds a hard dependency on 'Numpy', for array optimizations aimed at heavier workloads.
 - Adds optional dependency on 'Numba', for further speed optimizations using caching
   (currently untested due to issues with llvmlite).
 - Adds typing support.
 - General refactor and cleanup of the library, tests and docs.
 - **Breaking changes: API functions uses new names.**
@@ -211,15 +208,15 @@
             [[0.36930335, 0.36046537],
              [0.36360679, 0.35500328]]]])
 
 ## FAQ
 
 - What does the distribution of the noise values look like?
 
-![Noise Distribution](https://github.com/lmas/opensimplex/raw/master/images/distribution.png)
+![Noise Distribution](images/distribution.png)
 
 - Is this relevantly different enough to avoid any real trouble with the
 original patent?
 
     > If you read the [patent
     > claims](http://www.google.com/patents/US6867776):
     >
@@ -264,39 +261,32 @@
 
 ## Credits
 
 - Kurt Spencer - Original work
 - Owen Raccuglia - Test cases, [Go Module]
 - /u/redblobgames - Fixed conversion for Java's long type, see [Reddit]
 
-And all the other Github [Contributors] and [Bug Hunters]. Thanks!
+And all the other [Contributors] and [Bug Hunters]. Thanks!
 
 [Go Module]: https://github.com/ojrac/opensimplex-go
 [Reddit]: https://old.reddit.com/r/proceduralgeneration/comments/327zkm/repeated_patterns_in_opensimplex_python_port/cq8tth7/
-[Contributors]: https://github.com/lmas/opensimplex/graphs/contributors
-[Bug Hunters]: https://github.com/lmas/opensimplex/issues?q=is%3Aclosed
+[Contributors]: https://code.larus.se/lmas/opensimplex/activity/contributors
+[Bug Hunters]: https://code.larus.se/lmas/opensimplex/issues?state=closed
 
 ## License
 
 While the original work was released to the public domain by Kurt, this package is using the MIT license.
 
 Please see the file LICENSE for details.
 
 ## Example Output
 
 More example code and trinkets can be found in the [examples] directory.
 
-[examples]: https://github.com/lmas/opensimplex/tree/master/examples
+[examples]: https://code.larus.se/lmas/opensimplex/src/branch/master/examples
 
 Example images visualising 2D, 3D and 4D noise on a 2D plane, using the default seed:
 
-**2D noise**
-
-![Noise 2D](https://github.com/lmas/opensimplex/raw/master/images/noise2d.png)
-
-**3D noise**
-
-![Noise 3D](https://github.com/lmas/opensimplex/raw/master/images/noise3d.png)
-
-**4D noise**
+<img alt="Abstract black and white blobs visualizing 2D opensimplex noise on a 2D plane" src="images/noise2d.png">
+<img alt="Abstract black and white blobs visualizing 3D opensimplex noise on a 2D plane" src="images/noise3d.png">
+<img alt="Abstract black and white blobs visualizing 4D opensimplex noise on a 2D plane" src="images/noise4d.png">
 
-![Noise 4D](https://github.com/lmas/opensimplex/raw/master/images/noise4d.png)
```

### Comparing `opensimplex-0.4.5/README.md` & `opensimplex-0.4.5.1/opensimplex.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,28 @@
+Metadata-Version: 2.1
+Name: opensimplex
+Version: 0.4.5.1
+Summary: OpenSimplex is a noise generation function like Perlin or Simplex noise, but better.
+Home-page: https://code.larus.se/lmas/opensimplex
+Download-URL: https://code.larus.se/lmas/opensimplex/releases
+Author: Alex
+Author-email: opensimplex@larus.se
+License: MIT
+Keywords: opensimplex simplex noise 2D 3D 4D
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 
 # OpenSimplex Noise
 
-[![build-status](https://github.com/lmas/opensimplex/workflows/Tests/badge.svg?branch=master)](https://github.com/lmas/opensimplex/actions)
 [![pypi-version](https://img.shields.io/pypi/v/opensimplex?label=Version)](https://pypi.org/project/opensimplex/)
 [![pypi-downloads](https://img.shields.io/pypi/dm/opensimplex?label=Downloads)](https://pypistats.org/packages/opensimplex)
 
 [OpenSimplex] is a noise generation function like [Perlin] or [Simplex] noise, but better.
 
     OpenSimplex noise is an n-dimensional gradient noise function that was
     developed in order to overcome the patent-related issues surrounding
@@ -20,24 +37,22 @@
 [Perlin]: https://en.wikipedia.org/wiki/Perlin_noise
 [Simplex]: https://en.wikipedia.org/wiki/Simplex_noise
 [original code]: https://gist.github.com/KdotJPG/b1270127455a94ac5d19
 
 ## Status
 
 The `master` branch contains the latest code (possibly unstable),
-with automatic tests running for **Python 3.8, 3.9, 3.10 on Linux, MacOS and Windows**.
-**FreeBSD** is also supported, though it's only locally tested as Github Actions
-don't offer FreeBSD support.
-
-Please refer to the [version tags] for the latest stable version.
+please refer to the [version tags] for the latest stable version.
+An old, archived copy can be found at [Github].
 
-[version tags]: https://github.com/lmas/opensimplex/tags
+[version tags]: https://code.larus.se/lmas/opensimplex/tags
+[Github]: https://github.com/lmas/opensimplex
 
 
-Updates for **v0.4+**:
+Updates for **v0.4.***:
 
 - Adds a hard dependency on 'Numpy', for array optimizations aimed at heavier workloads.
 - Adds optional dependency on 'Numba', for further speed optimizations using caching
   (currently untested due to issues with llvmlite).
 - Adds typing support.
 - General refactor and cleanup of the library, tests and docs.
 - **Breaking changes: API functions uses new names.**
@@ -193,15 +208,15 @@
             [[0.36930335, 0.36046537],
              [0.36360679, 0.35500328]]]])
 
 ## FAQ
 
 - What does the distribution of the noise values look like?
 
-![Noise Distribution](https://github.com/lmas/opensimplex/raw/master/images/distribution.png)
+![Noise Distribution](images/distribution.png)
 
 - Is this relevantly different enough to avoid any real trouble with the
 original patent?
 
     > If you read the [patent
     > claims](http://www.google.com/patents/US6867776):
     >
@@ -246,39 +261,32 @@
 
 ## Credits
 
 - Kurt Spencer - Original work
 - Owen Raccuglia - Test cases, [Go Module]
 - /u/redblobgames - Fixed conversion for Java's long type, see [Reddit]
 
-And all the other Github [Contributors] and [Bug Hunters]. Thanks!
+And all the other [Contributors] and [Bug Hunters]. Thanks!
 
 [Go Module]: https://github.com/ojrac/opensimplex-go
 [Reddit]: https://old.reddit.com/r/proceduralgeneration/comments/327zkm/repeated_patterns_in_opensimplex_python_port/cq8tth7/
-[Contributors]: https://github.com/lmas/opensimplex/graphs/contributors
-[Bug Hunters]: https://github.com/lmas/opensimplex/issues?q=is%3Aclosed
+[Contributors]: https://code.larus.se/lmas/opensimplex/activity/contributors
+[Bug Hunters]: https://code.larus.se/lmas/opensimplex/issues?state=closed
 
 ## License
 
 While the original work was released to the public domain by Kurt, this package is using the MIT license.
 
 Please see the file LICENSE for details.
 
 ## Example Output
 
 More example code and trinkets can be found in the [examples] directory.
 
-[examples]: https://github.com/lmas/opensimplex/tree/master/examples
+[examples]: https://code.larus.se/lmas/opensimplex/src/branch/master/examples
 
 Example images visualising 2D, 3D and 4D noise on a 2D plane, using the default seed:
 
-**2D noise**
-
-![Noise 2D](https://github.com/lmas/opensimplex/raw/master/images/noise2d.png)
-
-**3D noise**
-
-![Noise 3D](https://github.com/lmas/opensimplex/raw/master/images/noise3d.png)
-
-**4D noise**
+<img alt="Abstract black and white blobs visualizing 2D opensimplex noise on a 2D plane" src="images/noise2d.png">
+<img alt="Abstract black and white blobs visualizing 3D opensimplex noise on a 2D plane" src="images/noise3d.png">
+<img alt="Abstract black and white blobs visualizing 4D opensimplex noise on a 2D plane" src="images/noise4d.png">
 
-![Noise 4D](https://github.com/lmas/opensimplex/raw/master/images/noise4d.png)
```

### Comparing `opensimplex-0.4.5/opensimplex/api.py` & `opensimplex-0.4.5.1/opensimplex/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     :return: seed as integer
 
     >>> get_seed()
     3
     """
     return _default.get_seed()
 
+
 def noise2(x: float, y: float) -> float:
     """
     Generate 2D OpenSimplex noise from X,Y coordinates.
     :param x: x coordinate as float
     :param y: y coordinate as float
     :return:  generated 2D noise as float, between -1.0 and 1.0
 
@@ -145,14 +146,15 @@
              [0.36360679, 0.35500328]]]])
     """
     return _default.noise4array(x, y, z, w)
 
 
 ################################################################################
 
+
 # This class is provided for backwards compatibility and might disappear in the future. Use at your own risk.
 class OpenSimplex(object):
     def __init__(self, seed: int) -> None:
         self._perm, self._perm_grad_index3 = _init(seed)
         self._seed = seed
 
     def get_seed(self) -> int:
```

### Comparing `opensimplex-0.4.5/opensimplex/constants.py` & `opensimplex-0.4.5.1/opensimplex/constants.py`

 * *Files identical despite different names*

### Comparing `opensimplex-0.4.5/opensimplex/internals.py` & `opensimplex-0.4.5.1/opensimplex/internals.py`

 * *Files identical despite different names*

### Comparing `opensimplex-0.4.5/opensimplex.egg-info/PKG-INFO` & `opensimplex-0.4.5.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,10 @@
-Metadata-Version: 2.1
-Name: opensimplex
-Version: 0.4.5
-Summary: OpenSimplex is a noise generation function like Perlin or Simplex noise, but better.
-Home-page: https://github.com/lmas/opensimplex
-Download-URL: https://github.com/lmas/opensimplex/releases
-Author: Alex
-Author-email: opensimplex@larus.se
-License: MIT
-Keywords: opensimplex simplex noise 2D 3D 4D
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 
 # OpenSimplex Noise
 
-[![build-status](https://github.com/lmas/opensimplex/workflows/Tests/badge.svg?branch=master)](https://github.com/lmas/opensimplex/actions)
 [![pypi-version](https://img.shields.io/pypi/v/opensimplex?label=Version)](https://pypi.org/project/opensimplex/)
 [![pypi-downloads](https://img.shields.io/pypi/dm/opensimplex?label=Downloads)](https://pypistats.org/packages/opensimplex)
 
 [OpenSimplex] is a noise generation function like [Perlin] or [Simplex] noise, but better.
 
     OpenSimplex noise is an n-dimensional gradient noise function that was
     developed in order to overcome the patent-related issues surrounding
@@ -38,24 +19,22 @@
 [Perlin]: https://en.wikipedia.org/wiki/Perlin_noise
 [Simplex]: https://en.wikipedia.org/wiki/Simplex_noise
 [original code]: https://gist.github.com/KdotJPG/b1270127455a94ac5d19
 
 ## Status
 
 The `master` branch contains the latest code (possibly unstable),
-with automatic tests running for **Python 3.8, 3.9, 3.10 on Linux, MacOS and Windows**.
-**FreeBSD** is also supported, though it's only locally tested as Github Actions
-don't offer FreeBSD support.
-
-Please refer to the [version tags] for the latest stable version.
+please refer to the [version tags] for the latest stable version.
+An old, archived copy can be found at [Github].
 
-[version tags]: https://github.com/lmas/opensimplex/tags
+[version tags]: https://code.larus.se/lmas/opensimplex/tags
+[Github]: https://github.com/lmas/opensimplex
 
 
-Updates for **v0.4+**:
+Updates for **v0.4.***:
 
 - Adds a hard dependency on 'Numpy', for array optimizations aimed at heavier workloads.
 - Adds optional dependency on 'Numba', for further speed optimizations using caching
   (currently untested due to issues with llvmlite).
 - Adds typing support.
 - General refactor and cleanup of the library, tests and docs.
 - **Breaking changes: API functions uses new names.**
@@ -211,15 +190,15 @@
             [[0.36930335, 0.36046537],
              [0.36360679, 0.35500328]]]])
 
 ## FAQ
 
 - What does the distribution of the noise values look like?
 
-![Noise Distribution](https://github.com/lmas/opensimplex/raw/master/images/distribution.png)
+![Noise Distribution](images/distribution.png)
 
 - Is this relevantly different enough to avoid any real trouble with the
 original patent?
 
     > If you read the [patent
     > claims](http://www.google.com/patents/US6867776):
     >
@@ -264,39 +243,32 @@
 
 ## Credits
 
 - Kurt Spencer - Original work
 - Owen Raccuglia - Test cases, [Go Module]
 - /u/redblobgames - Fixed conversion for Java's long type, see [Reddit]
 
-And all the other Github [Contributors] and [Bug Hunters]. Thanks!
+And all the other [Contributors] and [Bug Hunters]. Thanks!
 
 [Go Module]: https://github.com/ojrac/opensimplex-go
 [Reddit]: https://old.reddit.com/r/proceduralgeneration/comments/327zkm/repeated_patterns_in_opensimplex_python_port/cq8tth7/
-[Contributors]: https://github.com/lmas/opensimplex/graphs/contributors
-[Bug Hunters]: https://github.com/lmas/opensimplex/issues?q=is%3Aclosed
+[Contributors]: https://code.larus.se/lmas/opensimplex/activity/contributors
+[Bug Hunters]: https://code.larus.se/lmas/opensimplex/issues?state=closed
 
 ## License
 
 While the original work was released to the public domain by Kurt, this package is using the MIT license.
 
 Please see the file LICENSE for details.
 
 ## Example Output
 
 More example code and trinkets can be found in the [examples] directory.
 
-[examples]: https://github.com/lmas/opensimplex/tree/master/examples
+[examples]: https://code.larus.se/lmas/opensimplex/src/branch/master/examples
 
 Example images visualising 2D, 3D and 4D noise on a 2D plane, using the default seed:
 
-**2D noise**
-
-![Noise 2D](https://github.com/lmas/opensimplex/raw/master/images/noise2d.png)
-
-**3D noise**
-
-![Noise 3D](https://github.com/lmas/opensimplex/raw/master/images/noise3d.png)
-
-**4D noise**
+<img alt="Abstract black and white blobs visualizing 2D opensimplex noise on a 2D plane" src="images/noise2d.png">
+<img alt="Abstract black and white blobs visualizing 3D opensimplex noise on a 2D plane" src="images/noise3d.png">
+<img alt="Abstract black and white blobs visualizing 4D opensimplex noise on a 2D plane" src="images/noise4d.png">
 
-![Noise 4D](https://github.com/lmas/opensimplex/raw/master/images/noise4d.png)
```

### Comparing `opensimplex-0.4.5/setup.py` & `opensimplex-0.4.5.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,16 +11,16 @@
     version=__version__,
     author=__author__,
     author_email='opensimplex@larus.se',
     description='OpenSimplex is a noise generation function like Perlin or Simplex noise, but better.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords='opensimplex simplex noise 2D 3D 4D',
-    url='https://github.com/lmas/opensimplex',
-    download_url='https://github.com/lmas/opensimplex/releases',
+    url='https://code.larus.se/lmas/opensimplex',
+    download_url='https://code.larus.se/lmas/opensimplex/releases',
     license='MIT',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'numpy>=1.22',
     ],
     zip_safe=False,
```

### Comparing `opensimplex-0.4.5/tests/benchmark_opensimplex.py` & `opensimplex-0.4.5.1/tests/benchmark_opensimplex.py`

 * *Files identical despite different names*

### Comparing `opensimplex-0.4.5/tests/numpy_shapes.npz` & `opensimplex-0.4.5.1/tests/numpy_shapes.npz`

 * *Files identical despite different names*

### Comparing `opensimplex-0.4.5/tests/samples.json.gz` & `opensimplex-0.4.5.1/tests/samples.json.gz`

 * *Files identical despite different names*

### Comparing `opensimplex-0.4.5/tests/test_opensimplex.py` & `opensimplex-0.4.5.1/tests/test_opensimplex.py`

 * *Files identical despite different names*

