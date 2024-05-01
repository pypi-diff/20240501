# Comparing `tmp/quadplots-1.0.0.tar.gz` & `tmp/quadplots-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quadplots-1.0.0.tar", last modified: Wed May  1 14:25:50 2024, max compression
+gzip compressed data, was "quadplots-1.0.2.tar", last modified: Wed May  1 14:37:18 2024, max compression
```

## Comparing `quadplots-1.0.0.tar` & `quadplots-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-05-01 14:25:50.544015 quadplots-1.0.0/
--rw-r--r--   0 chris     (1000) chris     (1000)     1069 2024-04-30 23:29:27.000000 quadplots-1.0.0/LICENSE
--rw-r--r--   0 chris     (1000) chris     (1000)     2743 2024-05-01 14:25:50.544015 quadplots-1.0.0/PKG-INFO
--rw-r--r--   0 chris     (1000) chris     (1000)     1768 2024-05-01 14:24:54.000000 quadplots-1.0.0/README.md
--rw-r--r--   0 chris     (1000) chris     (1000)     1403 2024-05-01 14:22:18.000000 quadplots-1.0.0/pyproject.toml
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-05-01 14:25:50.544015 quadplots-1.0.0/quadplots/
--rw-r--r--   0 chris     (1000) chris     (1000)     5623 2024-04-30 22:42:37.000000 quadplots-1.0.0/quadplots/GraphQuad.py
--rw-r--r--   0 chris     (1000) chris     (1000)     8472 2024-04-30 22:42:37.000000 quadplots-1.0.0/quadplots/Interval.py
--rwxr-xr-x   0 chris     (1000) chris     (1000)     6476 2024-04-30 22:42:37.000000 quadplots-1.0.0/quadplots/Quadrature.py
--rw-r--r--   0 chris     (1000) chris     (1000)      128 2024-05-01 13:33:45.000000 quadplots-1.0.0/quadplots/__init__.py
--rw-r--r--   0 chris     (1000) chris     (1000)     3272 2024-04-30 22:42:37.000000 quadplots-1.0.0/quadplots/__main__.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-05-01 14:25:50.544015 quadplots-1.0.0/quadplots.egg-info/
--rw-r--r--   0 chris     (1000) chris     (1000)     2743 2024-05-01 14:25:50.000000 quadplots-1.0.0/quadplots.egg-info/PKG-INFO
--rw-r--r--   0 chris     (1000) chris     (1000)      345 2024-05-01 14:25:50.000000 quadplots-1.0.0/quadplots.egg-info/SOURCES.txt
--rw-r--r--   0 chris     (1000) chris     (1000)        1 2024-05-01 14:25:50.000000 quadplots-1.0.0/quadplots.egg-info/dependency_links.txt
--rw-r--r--   0 chris     (1000) chris     (1000)       59 2024-05-01 14:25:50.000000 quadplots-1.0.0/quadplots.egg-info/entry_points.txt
--rw-r--r--   0 chris     (1000) chris     (1000)       96 2024-05-01 14:25:50.000000 quadplots-1.0.0/quadplots.egg-info/requires.txt
--rw-r--r--   0 chris     (1000) chris     (1000)       10 2024-05-01 14:25:50.000000 quadplots-1.0.0/quadplots.egg-info/top_level.txt
--rw-r--r--   0 chris     (1000) chris     (1000)       38 2024-05-01 14:25:50.544015 quadplots-1.0.0/setup.cfg
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-05-01 14:37:18.625565 quadplots-1.0.2/
+-rw-r--r--   0 chris     (1000) chris     (1000)     1069 2024-04-30 23:29:27.000000 quadplots-1.0.2/LICENSE
+-rw-r--r--   0 chris     (1000) chris     (1000)     2557 2024-05-01 14:37:18.625565 quadplots-1.0.2/PKG-INFO
+-rw-r--r--   0 chris     (1000) chris     (1000)     1582 2024-05-01 14:35:58.000000 quadplots-1.0.2/README.md
+-rw-r--r--   0 chris     (1000) chris     (1000)     1403 2024-05-01 14:37:05.000000 quadplots-1.0.2/pyproject.toml
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-05-01 14:37:18.622232 quadplots-1.0.2/quadplots/
+-rw-r--r--   0 chris     (1000) chris     (1000)     5623 2024-04-30 22:42:37.000000 quadplots-1.0.2/quadplots/GraphQuad.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     8472 2024-04-30 22:42:37.000000 quadplots-1.0.2/quadplots/Interval.py
+-rwxr-xr-x   0 chris     (1000) chris     (1000)     6476 2024-04-30 22:42:37.000000 quadplots-1.0.2/quadplots/Quadrature.py
+-rw-r--r--   0 chris     (1000) chris     (1000)      128 2024-05-01 14:37:05.000000 quadplots-1.0.2/quadplots/__init__.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     3272 2024-04-30 22:42:37.000000 quadplots-1.0.2/quadplots/__main__.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-05-01 14:37:18.622232 quadplots-1.0.2/quadplots.egg-info/
+-rw-r--r--   0 chris     (1000) chris     (1000)     2557 2024-05-01 14:37:18.000000 quadplots-1.0.2/quadplots.egg-info/PKG-INFO
+-rw-r--r--   0 chris     (1000) chris     (1000)      345 2024-05-01 14:37:18.000000 quadplots-1.0.2/quadplots.egg-info/SOURCES.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)        1 2024-05-01 14:37:18.000000 quadplots-1.0.2/quadplots.egg-info/dependency_links.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)       59 2024-05-01 14:37:18.000000 quadplots-1.0.2/quadplots.egg-info/entry_points.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)       96 2024-05-01 14:37:18.000000 quadplots-1.0.2/quadplots.egg-info/requires.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)       10 2024-05-01 14:37:18.000000 quadplots-1.0.2/quadplots.egg-info/top_level.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)       38 2024-05-01 14:37:18.625565 quadplots-1.0.2/setup.cfg
```

### Comparing `quadplots-1.0.0/LICENSE` & `quadplots-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `quadplots-1.0.0/PKG-INFO` & `quadplots-1.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quadplots
-Version: 1.0.0
+Version: 1.0.2
 Summary: Create animations of simple numerical integration methods.
 Author: Chris Copley
 Project-URL: Repository, https://github.com/CopOnTheRun/quadplots
 Project-URL: Issues, https://github.com/CopOnTheRun/quadplots/issues
 Keywords: Simpson's Rule,Trapezoidal rule,Riemann Sum,Visualization,Graph,Quadrature
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -33,38 +33,38 @@
 
 Basic usage of quadplots only requires an expression you want to graph (must be valid python), and the start and end points.
 
 ```
 quadplots "x**2 - 3*x + 1" -2 3 
 ```
 
-![A riemann sum with n = 10 from -2 to 3](https://github.com/CopOnTheRun/quadplots/blob/main/images/basic_example.svg)
+![](https://github.com/CopOnTheRun/quadplots/raw/main/images/basic_example.svg)
 
 By default quadplots will graph a riemann sum with n=10 and use the midpoint method, but you can easily change these options.
 
 ```
 quadplots "x**2 - 3*x + 1" -2 3 --method min --partitions 5
 ```
 
 
-![A riemann sum with n = 5 from -2 to 3 using the min method](https://github.com/CopOnTheRun/quadplots/blob/main/images/min_example.svg)
+![](https://github.com/CopOnTheRun/quadplots/raw/main/images/min_example.svg)
 
 You can also change the type of quadrature method used
 
 ```
 quadplots "x**3 - 8*x + 7" -2 3 --method min --partitions 4 --quad-type simpson 
 ```
-![A Simpson's method with n = 4 from -2 to 3](https://github.com/CopOnTheRun/quadplots/blob/main/images/simpson_example.svg)
+![](https://github.com/CopOnTheRun/quadplots/raw/main/images/simpson_example.svg)
 
 If you want, instead of python functions, you can write latex by adding the `--latex` flag to the command.
 
 ```
 quadplots "\exp{-x^{2}}" -2 4 --partitions 4 --quad_type simpson --latex
 ```
-![A Simpson's method with n = 4 from -2 to 4](images/latex_example.svg)
+![](https://github.com/CopOnTheRun/quadplots/raw/main/images/latex_example.svg)
 
 Finally, if you wish to animate the plot, you can pass `--animate` with a list of partitions you would like to see at each frame.
 
 ```
 quadplots "\exp{-x^{2}}" -2 4 --partitions 4 --quad_type simpson --latex --animate 2 4 6 10 100
 ```
-![A Simpson's method with n = 4 from -2 to 4, animated](https://github.com/CopOnTheRun/quadplots/blob/main/images/animation_example.gif)
+![](https://github.com/CopOnTheRun/quadplots/raw/main/images/animation_example.gif)
```

### Comparing `quadplots-1.0.0/README.md` & `quadplots-1.0.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -6,38 +6,38 @@
 
 Basic usage of quadplots only requires an expression you want to graph (must be valid python), and the start and end points.
 
 ```
 quadplots "x**2 - 3*x + 1" -2 3 
 ```
 
-![A riemann sum with n = 10 from -2 to 3](https://github.com/CopOnTheRun/quadplots/blob/main/images/basic_example.svg)
+![](https://github.com/CopOnTheRun/quadplots/raw/main/images/basic_example.svg)
 
 By default quadplots will graph a riemann sum with n=10 and use the midpoint method, but you can easily change these options.
 
 ```
 quadplots "x**2 - 3*x + 1" -2 3 --method min --partitions 5
 ```
 
 
-![A riemann sum with n = 5 from -2 to 3 using the min method](https://github.com/CopOnTheRun/quadplots/blob/main/images/min_example.svg)
+![](https://github.com/CopOnTheRun/quadplots/raw/main/images/min_example.svg)
 
 You can also change the type of quadrature method used
 
 ```
 quadplots "x**3 - 8*x + 7" -2 3 --method min --partitions 4 --quad-type simpson 
 ```
-![A Simpson's method with n = 4 from -2 to 3](https://github.com/CopOnTheRun/quadplots/blob/main/images/simpson_example.svg)
+![](https://github.com/CopOnTheRun/quadplots/raw/main/images/simpson_example.svg)
 
 If you want, instead of python functions, you can write latex by adding the `--latex` flag to the command.
 
 ```
 quadplots "\exp{-x^{2}}" -2 4 --partitions 4 --quad_type simpson --latex
 ```
-![A Simpson's method with n = 4 from -2 to 4](images/latex_example.svg)
+![](https://github.com/CopOnTheRun/quadplots/raw/main/images/latex_example.svg)
 
 Finally, if you wish to animate the plot, you can pass `--animate` with a list of partitions you would like to see at each frame.
 
 ```
 quadplots "\exp{-x^{2}}" -2 4 --partitions 4 --quad_type simpson --latex --animate 2 4 6 10 100
 ```
-![A Simpson's method with n = 4 from -2 to 4, animated](https://github.com/CopOnTheRun/quadplots/blob/main/images/animation_example.gif)
+![](https://github.com/CopOnTheRun/quadplots/raw/main/images/animation_example.gif)
```

### Comparing `quadplots-1.0.0/pyproject.toml` & `quadplots-1.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires      = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "quadplots"
 description = "Create animations of simple numerical integration methods."
 readme = "README.md"
-version = "1.0.0"
+version = "1.0.2"
 authors = [{name = "Chris Copley"}]
 license = {file = "LICENSE.md"}
 keywords = ["Simpson's Rule", "Trapezoidal rule", "Riemann Sum", "Visualization", "Graph", "Quadrature"]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
@@ -35,15 +35,15 @@
 [project.scripts]
 quadplots = "btrview.scripts.btrview:main"
 
 [tool.setuptools]
 packages = ["quadplots"]
 
 [tool.bumpver]
-current_version = "1.0.0"
+current_version = "1.0.2"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 commit = true
 tag = true
 push = false
```

### Comparing `quadplots-1.0.0/quadplots/GraphQuad.py` & `quadplots-1.0.2/quadplots/GraphQuad.py`

 * *Files identical despite different names*

### Comparing `quadplots-1.0.0/quadplots/Interval.py` & `quadplots-1.0.2/quadplots/Interval.py`

 * *Files identical despite different names*

### Comparing `quadplots-1.0.0/quadplots/Quadrature.py` & `quadplots-1.0.2/quadplots/Quadrature.py`

 * *Files identical despite different names*

### Comparing `quadplots-1.0.0/quadplots/__main__.py` & `quadplots-1.0.2/quadplots/__main__.py`

 * *Files identical despite different names*

### Comparing `quadplots-1.0.0/quadplots.egg-info/PKG-INFO` & `quadplots-1.0.2/quadplots.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quadplots
-Version: 1.0.0
+Version: 1.0.2
 Summary: Create animations of simple numerical integration methods.
 Author: Chris Copley
 Project-URL: Repository, https://github.com/CopOnTheRun/quadplots
 Project-URL: Issues, https://github.com/CopOnTheRun/quadplots/issues
 Keywords: Simpson's Rule,Trapezoidal rule,Riemann Sum,Visualization,Graph,Quadrature
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -33,38 +33,38 @@
 
 Basic usage of quadplots only requires an expression you want to graph (must be valid python), and the start and end points.
 
 ```
 quadplots "x**2 - 3*x + 1" -2 3 
 ```
 
-![A riemann sum with n = 10 from -2 to 3](https://github.com/CopOnTheRun/quadplots/blob/main/images/basic_example.svg)
+![](https://github.com/CopOnTheRun/quadplots/raw/main/images/basic_example.svg)
 
 By default quadplots will graph a riemann sum with n=10 and use the midpoint method, but you can easily change these options.
 
 ```
 quadplots "x**2 - 3*x + 1" -2 3 --method min --partitions 5
 ```
 
 
-![A riemann sum with n = 5 from -2 to 3 using the min method](https://github.com/CopOnTheRun/quadplots/blob/main/images/min_example.svg)
+![](https://github.com/CopOnTheRun/quadplots/raw/main/images/min_example.svg)
 
 You can also change the type of quadrature method used
 
 ```
 quadplots "x**3 - 8*x + 7" -2 3 --method min --partitions 4 --quad-type simpson 
 ```
-![A Simpson's method with n = 4 from -2 to 3](https://github.com/CopOnTheRun/quadplots/blob/main/images/simpson_example.svg)
+![](https://github.com/CopOnTheRun/quadplots/raw/main/images/simpson_example.svg)
 
 If you want, instead of python functions, you can write latex by adding the `--latex` flag to the command.
 
 ```
 quadplots "\exp{-x^{2}}" -2 4 --partitions 4 --quad_type simpson --latex
 ```
-![A Simpson's method with n = 4 from -2 to 4](images/latex_example.svg)
+![](https://github.com/CopOnTheRun/quadplots/raw/main/images/latex_example.svg)
 
 Finally, if you wish to animate the plot, you can pass `--animate` with a list of partitions you would like to see at each frame.
 
 ```
 quadplots "\exp{-x^{2}}" -2 4 --partitions 4 --quad_type simpson --latex --animate 2 4 6 10 100
 ```
-![A Simpson's method with n = 4 from -2 to 4, animated](https://github.com/CopOnTheRun/quadplots/blob/main/images/animation_example.gif)
+![](https://github.com/CopOnTheRun/quadplots/raw/main/images/animation_example.gif)
```

