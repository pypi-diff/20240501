# Comparing `tmp/randomnwn-0.3.1.tar.gz` & `tmp/randomnwn-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "randomnwn-0.3.1.tar", last modified: Tue Jun 13 21:32:41 2023, max compression
+gzip compressed data, was "randomnwn-0.4.0.tar", last modified: Wed May  1 21:34:02 2024, max compression
```

## Comparing `randomnwn-0.3.1.tar` & `randomnwn-0.4.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 21:32:41.965087 randomnwn-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (122)     1071 2023-06-13 21:32:31.000000 randomnwn-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     2359 2023-06-13 21:32:41.965087 randomnwn-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2015 2023-06-13 21:32:31.000000 randomnwn-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 21:32:41.961087 randomnwn-0.3.1/randomnwn/
--rw-r--r--   0 runner    (1001) docker     (122)      851 2023-06-13 21:32:31.000000 randomnwn-0.3.1/randomnwn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5077 2023-06-13 21:32:31.000000 randomnwn-0.3.1/randomnwn/_models.py
--rw-r--r--   0 runner    (1001) docker     (122)    13216 2023-06-13 21:32:31.000000 randomnwn-0.3.1/randomnwn/calculations.py
--rw-r--r--   0 runner    (1001) docker     (122)    11299 2023-06-13 21:32:31.000000 randomnwn-0.3.1/randomnwn/dynamics.py
--rw-r--r--   0 runner    (1001) docker     (122)     3569 2023-06-13 21:32:31.000000 randomnwn-0.3.1/randomnwn/fromtext.py
--rw-r--r--   0 runner    (1001) docker     (122)     4165 2023-06-13 21:32:31.000000 randomnwn-0.3.1/randomnwn/line_functions.py
--rw-r--r--   0 runner    (1001) docker     (122)    15555 2023-06-13 21:32:31.000000 randomnwn-0.3.1/randomnwn/nanowires.py
--rw-r--r--   0 runner    (1001) docker     (122)     6141 2023-06-13 21:32:31.000000 randomnwn-0.3.1/randomnwn/plotting.py
--rw-r--r--   0 runner    (1001) docker     (122)     1374 2023-06-13 21:32:31.000000 randomnwn-0.3.1/randomnwn/units.py
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-06-13 21:32:31.000000 randomnwn-0.3.1/randomnwn/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 21:32:41.965087 randomnwn-0.3.1/randomnwn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2359 2023-06-13 21:32:41.000000 randomnwn-0.3.1/randomnwn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      408 2023-06-13 21:32:41.000000 randomnwn-0.3.1/randomnwn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-13 21:32:41.000000 randomnwn-0.3.1/randomnwn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-06-13 21:32:41.000000 randomnwn-0.3.1/randomnwn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-13 21:32:41.965087 randomnwn-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      657 2023-06-13 21:32:31.000000 randomnwn-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 21:32:41.965087 randomnwn-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     2111 2023-06-13 21:32:31.000000 randomnwn-0.3.1/tests/test_nanowires.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:34:02.647827 randomnwn-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-01 21:33:57.000000 randomnwn-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-05-01 21:34:02.647827 randomnwn-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-01 21:33:57.000000 randomnwn-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:34:02.643827 randomnwn-0.4.0/randomnwn/
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-01 21:33:57.000000 randomnwn-0.4.0/randomnwn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-05-01 21:33:57.000000 randomnwn-0.4.0/randomnwn/_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13216 2024-05-01 21:33:57.000000 randomnwn-0.4.0/randomnwn/calculations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11299 2024-05-01 21:33:57.000000 randomnwn-0.4.0/randomnwn/dynamics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-05-01 21:33:57.000000 randomnwn-0.4.0/randomnwn/fromtext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-05-01 21:33:57.000000 randomnwn-0.4.0/randomnwn/line_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15555 2024-05-01 21:33:57.000000 randomnwn-0.4.0/randomnwn/nanowires.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6168 2024-05-01 21:33:57.000000 randomnwn-0.4.0/randomnwn/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-01 21:33:57.000000 randomnwn-0.4.0/randomnwn/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-01 21:33:57.000000 randomnwn-0.4.0/randomnwn/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:34:02.647827 randomnwn-0.4.0/randomnwn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-05-01 21:34:02.000000 randomnwn-0.4.0/randomnwn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-01 21:34:02.000000 randomnwn-0.4.0/randomnwn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 21:34:02.000000 randomnwn-0.4.0/randomnwn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-01 21:34:02.000000 randomnwn-0.4.0/randomnwn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 21:34:02.647827 randomnwn-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-01 21:33:57.000000 randomnwn-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:34:02.647827 randomnwn-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-01 21:33:57.000000 randomnwn-0.4.0/tests/test_nanowires.py
```

### Comparing `randomnwn-0.3.1/LICENSE` & `randomnwn-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `randomnwn-0.3.1/PKG-INFO` & `randomnwn-0.4.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,14 @@
-Metadata-Version: 2.1
-Name: randomnwn
-Version: 0.3.1
-Summary: Modelling and analyzing random nanowire networks in Python.
-Home-page: https://github.com/marcus-k/Random-NWNs
-Author: Marcus Kasdorf
-Author-email: marcus.kasdorf@ucalgary.ca
-License: MIT License
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Random NWNs [![Tests](https://github.com/marcus-k/Random-NWNs/actions/workflows/python-package.yml/badge.svg)](https://github.com/marcus-k/Random-NWNs/actions/workflows/python-package.yml)
 
-Python package for modelling and analyzing random nanowire networks. This package was a summer research project lasting from May 2021 to August 2021 under the supervision of Dr. Claudia Gomes da Rocha.
+Python package for modelling and analyzing random nanowire networks. This package was a summer research project lasting from May 2021 to August 2021 under the supervision of Dr. Claudia Gomes da Rocha. 
+
+**Update:** This project will now be continuing as of May 2024. If you are using this project, please note there will be **active development** on it and the functionality may change.
 
-For future additions, feel free to fork the repository, but please give credit where it's due, either here or to Marcus Kasdorf.
+For future additions, feel free to fork the repository. Please cite Marcus Kasdorf if you wish to extend the project.
 
 # Table of Contents
 * [Installation](#installation)
 * [Usage](#usage)
 * [Uninstallation](#uninstallation)
 
 # Installation
```

### Comparing `randomnwn-0.3.1/README.md` & `randomnwn-0.4.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,26 @@
+Metadata-Version: 2.1
+Name: randomnwn
+Version: 0.4.0
+Summary: Modelling and analyzing random nanowire networks in Python.
+Home-page: https://github.com/marcus-k/Random-NWNs
+Author: Marcus Kasdorf
+Author-email: marcus.kasdorf@ucalgary.ca
+License: MIT License
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Random NWNs [![Tests](https://github.com/marcus-k/Random-NWNs/actions/workflows/python-package.yml/badge.svg)](https://github.com/marcus-k/Random-NWNs/actions/workflows/python-package.yml)
 
-Python package for modelling and analyzing random nanowire networks. This package was a summer research project lasting from May 2021 to August 2021 under the supervision of Dr. Claudia Gomes da Rocha.
+Python package for modelling and analyzing random nanowire networks. This package was a summer research project lasting from May 2021 to August 2021 under the supervision of Dr. Claudia Gomes da Rocha. 
+
+**Update:** This project will now be continuing as of May 2024. If you are using this project, please note there will be **active development** on it and the functionality may change.
 
-For future additions, feel free to fork the repository, but please give credit where it's due, either here or to Marcus Kasdorf.
+For future additions, feel free to fork the repository. Please cite Marcus Kasdorf if you wish to extend the project.
 
 # Table of Contents
 * [Installation](#installation)
 * [Usage](#usage)
 * [Uninstallation](#uninstallation)
 
 # Installation
```

### Comparing `randomnwn-0.3.1/randomnwn/__init__.py` & `randomnwn-0.4.0/randomnwn/__init__.py`

 * *Files identical despite different names*

### Comparing `randomnwn-0.3.1/randomnwn/_models.py` & `randomnwn-0.4.0/randomnwn/_models.py`

 * *Files identical despite different names*

### Comparing `randomnwn-0.3.1/randomnwn/calculations.py` & `randomnwn-0.4.0/randomnwn/calculations.py`

 * *Files identical despite different names*

### Comparing `randomnwn-0.3.1/randomnwn/dynamics.py` & `randomnwn-0.4.0/randomnwn/dynamics.py`

 * *Files identical despite different names*

### Comparing `randomnwn-0.3.1/randomnwn/fromtext.py` & `randomnwn-0.4.0/randomnwn/fromtext.py`

 * *Files identical despite different names*

### Comparing `randomnwn-0.3.1/randomnwn/line_functions.py` & `randomnwn-0.4.0/randomnwn/line_functions.py`

 * *Files identical despite different names*

### Comparing `randomnwn-0.3.1/randomnwn/nanowires.py` & `randomnwn-0.4.0/randomnwn/nanowires.py`

 * *Files identical despite different names*

### Comparing `randomnwn-0.3.1/randomnwn/plotting.py` & `randomnwn-0.4.0/randomnwn/plotting.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,21 +73,21 @@
             *np.array([(point.x, point.y) for point in NWN.graph["loc"].values()]).T, 
             zorder=10, s=5, c="blue"
         )
 
     # Defaults to blue and pink lines, else random colors are used.
     if rnd_color:
         for i in range(NWN.graph["wire_num"]):
-            ax.plot(*np.array(NWN.graph["lines"][i]).T)
+            ax.plot(*np.asarray(NWN.graph["lines"][i].coords).T)
     else:
         for i in range(NWN.graph["wire_num"]):
             if (i,) in NWN.graph["electrode_list"]:
-                ax.plot(*np.array(NWN.graph["lines"][i]).T, c="xkcd:light blue")
+                ax.plot(*np.asarray(NWN.graph["lines"][i].coords).T, c="xkcd:light blue")
             else:
-                ax.plot(*np.array(NWN.graph["lines"][i]).T, c="pink")
+                ax.plot(*np.asarray(NWN.graph["lines"][i].coords).T, c="pink")
 
     # Scale axes according to the characteristic values
     if scaled:
         ax.xaxis.set_major_formatter(
             ticker.FuncFormatter(lambda x, pos: f"{x * l0:.3g}")
         )
         ax.yaxis.set_major_formatter(
```

### Comparing `randomnwn-0.3.1/randomnwn/units.py` & `randomnwn-0.4.0/randomnwn/units.py`

 * *Files identical despite different names*

### Comparing `randomnwn-0.3.1/randomnwn.egg-info/PKG-INFO` & `randomnwn-0.4.0/randomnwn.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: randomnwn
-Version: 0.3.1
+Version: 0.4.0
 Summary: Modelling and analyzing random nanowire networks in Python.
 Home-page: https://github.com/marcus-k/Random-NWNs
 Author: Marcus Kasdorf
 Author-email: marcus.kasdorf@ucalgary.ca
 License: MIT License
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Random NWNs [![Tests](https://github.com/marcus-k/Random-NWNs/actions/workflows/python-package.yml/badge.svg)](https://github.com/marcus-k/Random-NWNs/actions/workflows/python-package.yml)
 
-Python package for modelling and analyzing random nanowire networks. This package was a summer research project lasting from May 2021 to August 2021 under the supervision of Dr. Claudia Gomes da Rocha.
+Python package for modelling and analyzing random nanowire networks. This package was a summer research project lasting from May 2021 to August 2021 under the supervision of Dr. Claudia Gomes da Rocha. 
 
-For future additions, feel free to fork the repository, but please give credit where it's due, either here or to Marcus Kasdorf.
+**Update:** This project will now be continuing as of May 2024. If you are using this project, please note there will be **active development** on it and the functionality may change.
+
+For future additions, feel free to fork the repository. Please cite Marcus Kasdorf if you wish to extend the project.
 
 # Table of Contents
 * [Installation](#installation)
 * [Usage](#usage)
 * [Uninstallation](#uninstallation)
 
 # Installation
```

### Comparing `randomnwn-0.3.1/setup.py` & `randomnwn-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,9 +14,9 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/marcus-k/Random-NWNs',
     author='Marcus Kasdorf',
     author_email='marcus.kasdorf@ucalgary.ca',
     license='MIT License',
     packages=['randomnwn'],
-    python_requires='>=3.8'
+    python_requires='>=3.10'
 )
```

### Comparing `randomnwn-0.3.1/tests/test_nanowires.py` & `randomnwn-0.4.0/tests/test_nanowires.py`

 * *Files identical despite different names*

