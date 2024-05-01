# Comparing `tmp/velosaurus_sum-1.0.3.tar.gz` & `tmp/velosaurus_sum-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "velosaurus_sum-1.0.3.tar", last modified: Wed May  1 14:46:04 2024, max compression
+gzip compressed data, was "velosaurus_sum-1.0.4.tar", last modified: Wed May  1 14:50:39 2024, max compression
```

## Comparing `velosaurus_sum-1.0.3.tar` & `velosaurus_sum-1.0.4.tar`

### file list

```diff
@@ -1,13 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:46:04.257981 velosaurus_sum-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-01 14:46:04.257981 velosaurus_sum-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-01 14:45:55.000000 velosaurus_sum-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-01 14:45:55.000000 velosaurus_sum-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 14:46:04.257981 velosaurus_sum-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-01 14:45:55.000000 velosaurus_sum-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:46:04.257981 velosaurus_sum-1.0.3/test/
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-01 14:45:55.000000 velosaurus_sum-1.0.3/test/test_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:46:04.257981 velosaurus_sum-1.0.3/velosaurus_sum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-01 14:46:04.000000 velosaurus_sum-1.0.3/velosaurus_sum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-01 14:46:04.000000 velosaurus_sum-1.0.3/velosaurus_sum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 14:46:04.000000 velosaurus_sum-1.0.3/velosaurus_sum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 14:46:04.000000 velosaurus_sum-1.0.3/velosaurus_sum.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:50:39.642553 velosaurus_sum-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-01 14:50:39.642553 velosaurus_sum-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-01 14:50:34.000000 velosaurus_sum-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-01 14:50:34.000000 velosaurus_sum-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 14:50:39.642553 velosaurus_sum-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-01 14:50:34.000000 velosaurus_sum-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:50:39.642553 velosaurus_sum-1.0.4/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:50:34.000000 velosaurus_sum-1.0.4/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-01 14:50:34.000000 velosaurus_sum-1.0.4/test/test_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:50:39.642553 velosaurus_sum-1.0.4/velosaurus_sum/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:50:34.000000 velosaurus_sum-1.0.4/velosaurus_sum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-01 14:50:34.000000 velosaurus_sum-1.0.4/velosaurus_sum/calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:50:39.642553 velosaurus_sum-1.0.4/velosaurus_sum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-01 14:50:39.000000 velosaurus_sum-1.0.4/velosaurus_sum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-01 14:50:39.000000 velosaurus_sum-1.0.4/velosaurus_sum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 14:50:39.000000 velosaurus_sum-1.0.4/velosaurus_sum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-01 14:50:39.000000 velosaurus_sum-1.0.4/velosaurus_sum.egg-info/top_level.txt
```

### Comparing `velosaurus_sum-1.0.3/PKG-INFO` & `velosaurus_sum-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: velosaurus_sum
-Version: 1.0.3
+Version: 1.0.4
 Summary: Just a dummy project for some pipeline and package deployment testing
 Home-page: https://github.com/OliverZott/python-devops-example
 Author: Oliver Zott
 Author-email: zott_oliver@web.de
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `velosaurus_sum-1.0.3/README.md` & `velosaurus_sum-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `velosaurus_sum-1.0.3/pyproject.toml` & `velosaurus_sum-1.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `velosaurus_sum-1.0.3/setup.py` & `velosaurus_sum-1.0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name="velosaurus_sum",
-    version="1.0.3",
+    version="1.0.4",
     description="Just a dummy project for some pipeline and package deployment testing",
     long_description="Just a dummy project for some pipeline and package deployment testing",
     author="Oliver Zott",
     author_email="zott_oliver@web.de",
     url="https://github.com/OliverZott/python-devops-example",
-    packages=find_packages(where="src"),
+    packages=find_packages(),
     install_requires=[
         # Add any dependencies your project requires
     ],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
```

### Comparing `velosaurus_sum-1.0.3/velosaurus_sum.egg-info/PKG-INFO` & `velosaurus_sum-1.0.4/velosaurus_sum.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: velosaurus_sum
-Version: 1.0.3
+Version: 1.0.4
 Summary: Just a dummy project for some pipeline and package deployment testing
 Home-page: https://github.com/OliverZott/python-devops-example
 Author: Oliver Zott
 Author-email: zott_oliver@web.de
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

