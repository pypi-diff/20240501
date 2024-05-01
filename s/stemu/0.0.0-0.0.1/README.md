# Comparing `tmp/stemu-0.0.0.tar.gz` & `tmp/stemu-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stemu-0.0.0.tar", last modified: Thu Apr 18 13:01:01 2024, max compression
+gzip compressed data, was "stemu-0.0.1.tar", last modified: Wed May  1 07:46:45 2024, max compression
```

## Comparing `stemu-0.0.0.tar` & `stemu-0.0.1.tar`

### file list

```diff
@@ -1,17 +1,22 @@
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2024-04-18 13:01:01.313534 stemu-0.0.0/
--rw-r--r--   0 will      (1000) will      (1000)     1084 2024-04-18 12:41:58.000000 stemu-0.0.0/LICENSE
--rw-r--r--   0 will      (1000) will      (1000)     7623 2024-04-18 13:01:01.313534 stemu-0.0.0/PKG-INFO
--rw-r--r--   0 will      (1000) will      (1000)     4725 2024-04-18 12:41:58.000000 stemu-0.0.0/README.rst
--rw-r--r--   0 will      (1000) will      (1000)     1646 2024-04-18 12:41:58.000000 stemu-0.0.0/pyproject.toml
--rw-r--r--   0 will      (1000) will      (1000)       94 2024-04-18 13:01:01.313534 stemu-0.0.0/setup.cfg
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2024-04-18 13:01:01.313534 stemu-0.0.0/stemu/
--rw-r--r--   0 will      (1000) will      (1000)      115 2024-04-18 12:41:58.000000 stemu-0.0.0/stemu/__init__.py
--rw-r--r--   0 will      (1000) will      (1000)       22 2024-04-18 12:41:58.000000 stemu-0.0.0/stemu/_version.py
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2024-04-18 13:01:01.313534 stemu-0.0.0/stemu.egg-info/
--rw-r--r--   0 will      (1000) will      (1000)     7623 2024-04-18 13:01:01.000000 stemu-0.0.0/stemu.egg-info/PKG-INFO
--rw-r--r--   0 will      (1000) will      (1000)      245 2024-04-18 13:01:01.000000 stemu-0.0.0/stemu.egg-info/SOURCES.txt
--rw-r--r--   0 will      (1000) will      (1000)        1 2024-04-18 13:01:01.000000 stemu-0.0.0/stemu.egg-info/dependency_links.txt
--rw-r--r--   0 will      (1000) will      (1000)      129 2024-04-18 13:01:01.000000 stemu-0.0.0/stemu.egg-info/requires.txt
--rw-r--r--   0 will      (1000) will      (1000)        6 2024-04-18 13:01:01.000000 stemu-0.0.0/stemu.egg-info/top_level.txt
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2024-04-18 13:01:01.313534 stemu-0.0.0/tests/
--rw-r--r--   0 will      (1000) will      (1000)       36 2024-04-18 12:41:58.000000 stemu-0.0.0/tests/test_example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 07:46:45.362740 stemu-0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-01 07:46:41.000000 stemu-0.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7699 2024-05-01 07:46:45.362740 stemu-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4725 2024-05-01 07:46:41.000000 stemu-0.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-01 07:46:41.000000 stemu-0.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-01 07:46:45.362740 stemu-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 07:46:45.358740 stemu-0.0.1/stemu/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-01 07:46:41.000000 stemu-0.0.1/stemu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-01 07:46:41.000000 stemu-0.0.1/stemu/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-05-01 07:46:41.000000 stemu-0.0.1/stemu/emu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-05-01 07:46:41.000000 stemu-0.0.1/stemu/skutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-05-01 07:46:41.000000 stemu-0.0.1/stemu/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 07:46:45.362740 stemu-0.0.1/stemu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7699 2024-05-01 07:46:45.000000 stemu-0.0.1/stemu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-01 07:46:45.000000 stemu-0.0.1/stemu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 07:46:45.000000 stemu-0.0.1/stemu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-01 07:46:45.000000 stemu-0.0.1/stemu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-01 07:46:45.000000 stemu-0.0.1/stemu.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 07:46:45.362740 stemu-0.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-01 07:46:41.000000 stemu-0.0.1/tests/test_emu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-01 07:46:41.000000 stemu-0.0.1/tests/test_skutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-01 07:46:41.000000 stemu-0.0.1/tests/test_utils.py
```

### Comparing `stemu-0.0.0/LICENSE` & `stemu-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stemu-0.0.0/PKG-INFO` & `stemu-0.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stemu
-Version: 0.0.0
+Version: 0.0.1
 Summary: s(t) emulation of smooth functions by stacking
 Author-email: Harry Bevins <htjb2@cam.ac.uk>, Will Handley <williamjameshandley@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Will Handley & Harry Bevins
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -43,14 +43,17 @@
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: matplotlib
+Requires-Dist: pandas
+Requires-Dist: tensorflow
+Requires-Dist: scikit-learn
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx_rtd_theme; extra == "docs"
 Requires-Dist: numpydoc; extra == "docs"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
@@ -60,15 +63,15 @@
 Requires-Dist: pre-commit; extra == "test"
 
 =====================================================
 stemu: s(t) emulation of smooth functions by stacking
 =====================================================
 :stemu: s(t) emulation of smooth functions by stacking 
 :Author: Harry Bevins & Will Handley
-:Version: 0.0.0
+:Version: 0.0.1
 :Homepage: https://github.com/handley-lab/stemu
 :Documentation: http://stemu.readthedocs.io/
 
 .. image:: https://github.com/handley-lab/stemu/actions/workflows/unittests.yaml/badge.svg?branch=master
    :target: https://github.com/handley-lab/stemu/actions/workflows/unittests.yaml?query=branch%3Amaster
    :alt: Unit test status
 .. image:: https://github.com/handley-lab/stemu/actions/workflows/build.yaml/badge.svg?branch=master
```

### Comparing `stemu-0.0.0/README.rst` & `stemu-0.0.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 =====================================================
 stemu: s(t) emulation of smooth functions by stacking
 =====================================================
 :stemu: s(t) emulation of smooth functions by stacking 
 :Author: Harry Bevins & Will Handley
-:Version: 0.0.0
+:Version: 0.0.1
 :Homepage: https://github.com/handley-lab/stemu
 :Documentation: http://stemu.readthedocs.io/
 
 .. image:: https://github.com/handley-lab/stemu/actions/workflows/unittests.yaml/badge.svg?branch=master
    :target: https://github.com/handley-lab/stemu/actions/workflows/unittests.yaml?query=branch%3Amaster
    :alt: Unit test status
 .. image:: https://github.com/handley-lab/stemu/actions/workflows/build.yaml/badge.svg?branch=master
```

### Comparing `stemu-0.0.0/pyproject.toml` & `stemu-0.0.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -13,14 +13,17 @@
 readme = "README.rst"
 license = {file = "LICENSE"}
 requires-python = ">=3.8"
 dependencies = [
     'numpy',
     'scipy',
     'matplotlib',
+    'pandas',
+    'tensorflow',
+    'scikit-learn',
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Development Status :: 1 - Planning",
     "Intended Audience :: Developers",
```

### Comparing `stemu-0.0.0/stemu.egg-info/PKG-INFO` & `stemu-0.0.1/stemu.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stemu
-Version: 0.0.0
+Version: 0.0.1
 Summary: s(t) emulation of smooth functions by stacking
 Author-email: Harry Bevins <htjb2@cam.ac.uk>, Will Handley <williamjameshandley@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Will Handley & Harry Bevins
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -43,14 +43,17 @@
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: matplotlib
+Requires-Dist: pandas
+Requires-Dist: tensorflow
+Requires-Dist: scikit-learn
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx_rtd_theme; extra == "docs"
 Requires-Dist: numpydoc; extra == "docs"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
@@ -60,15 +63,15 @@
 Requires-Dist: pre-commit; extra == "test"
 
 =====================================================
 stemu: s(t) emulation of smooth functions by stacking
 =====================================================
 :stemu: s(t) emulation of smooth functions by stacking 
 :Author: Harry Bevins & Will Handley
-:Version: 0.0.0
+:Version: 0.0.1
 :Homepage: https://github.com/handley-lab/stemu
 :Documentation: http://stemu.readthedocs.io/
 
 .. image:: https://github.com/handley-lab/stemu/actions/workflows/unittests.yaml/badge.svg?branch=master
    :target: https://github.com/handley-lab/stemu/actions/workflows/unittests.yaml?query=branch%3Amaster
    :alt: Unit test status
 .. image:: https://github.com/handley-lab/stemu/actions/workflows/build.yaml/badge.svg?branch=master
```

