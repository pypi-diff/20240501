# Comparing `tmp/galgebra-0.5.1.tar.gz` & `tmp/galgebra-0.5.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galgebra-0.5.1.tar", last modified: Mon Apr  1 07:21:35 2024, max compression
+gzip compressed data, was "galgebra-0.5.2rc1.tar", last modified: Wed May  1 09:46:56 2024, max compression
```

## Comparing `galgebra-0.5.1.tar` & `galgebra-0.5.2rc1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 07:21:35.321779 galgebra-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-01 07:21:33.000000 galgebra-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10899 2024-04-01 07:21:35.321779 galgebra-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9779 2024-04-01 07:21:33.000000 galgebra-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 07:21:35.317779 galgebra-0.5.1/galgebra/
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-01 07:21:33.000000 galgebra-0.5.1/galgebra/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 07:21:35.317779 galgebra-0.5.1/galgebra/_backports/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-01 07:21:33.000000 galgebra-0.5.1/galgebra/_backports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-01 07:21:33.000000 galgebra-0.5.1/galgebra/_backports/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 07:21:35.321779 galgebra-0.5.1/galgebra/_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-01 07:21:33.000000 galgebra-0.5.1/galgebra/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-01 07:21:33.000000 galgebra-0.5.1/galgebra/_utils/cached_property.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-01 07:21:33.000000 galgebra-0.5.1/galgebra/_utils/kwarg_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-04-01 07:21:33.000000 galgebra-0.5.1/galgebra/_utils/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-01 07:21:33.000000 galgebra-0.5.1/galgebra/_utils/printable.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-01 07:21:33.000000 galgebra-0.5.1/galgebra/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-04-01 07:21:33.000000 galgebra-0.5.1/galgebra/atoms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-04-01 07:21:33.000000 galgebra-0.5.1/galgebra/deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)    12225 2024-04-01 07:21:33.000000 galgebra-0.5.1/galgebra/dop.py
--rw-r--r--   0 runner    (1001) docker     (127)    86234 2024-04-01 07:21:33.000000 galgebra-0.5.1/galgebra/ga.py
--rw-r--r--   0 runner    (1001) docker     (127)    33789 2024-04-01 07:21:33.000000 galgebra-0.5.1/galgebra/lt.py
--rw-r--r--   0 runner    (1001) docker     (127)    27006 2024-04-01 07:21:33.000000 galgebra-0.5.1/galgebra/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    69857 2024-04-01 07:21:33.000000 galgebra-0.5.1/galgebra/mv.py
--rw-r--r--   0 runner    (1001) docker     (127)    42443 2024-04-01 07:21:33.000000 galgebra-0.5.1/galgebra/printer.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-01 07:21:33.000000 galgebra-0.5.1/galgebra/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 07:21:35.317779 galgebra-0.5.1/galgebra.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10899 2024-04-01 07:21:35.000000 galgebra-0.5.1/galgebra.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-01 07:21:35.000000 galgebra-0.5.1/galgebra.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 07:21:35.000000 galgebra-0.5.1/galgebra.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-01 07:21:35.000000 galgebra-0.5.1/galgebra.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-01 07:21:35.000000 galgebra-0.5.1/galgebra.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-01 07:21:35.321779 galgebra-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-01 07:21:33.000000 galgebra-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 07:21:35.321779 galgebra-0.5.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-01 07:21:33.000000 galgebra-0.5.1/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11452 2024-04-01 07:21:33.000000 galgebra-0.5.1/test/test_differential_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     4570 2024-04-01 07:21:33.000000 galgebra-0.5.1/test/test_lt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-04-01 07:21:33.000000 galgebra-0.5.1/test/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7608 2024-04-01 07:21:33.000000 galgebra-0.5.1/test/test_mv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3567 2024-04-01 07:21:33.000000 galgebra-0.5.1/test/test_printer.py
--rw-r--r--   0 runner    (1001) docker     (127)    25852 2024-04-01 07:21:33.000000 galgebra-0.5.1/test/test_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:46:56.563029 galgebra-0.5.2rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-01 09:46:50.000000 galgebra-0.5.2rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11765 2024-05-01 09:46:56.563029 galgebra-0.5.2rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10642 2024-05-01 09:46:50.000000 galgebra-0.5.2rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:46:56.559029 galgebra-0.5.2rc1/galgebra/
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-01 09:46:50.000000 galgebra-0.5.2rc1/galgebra/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:46:56.563029 galgebra-0.5.2rc1/galgebra/_backports/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-01 09:46:50.000000 galgebra-0.5.2rc1/galgebra/_backports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-01 09:46:50.000000 galgebra-0.5.2rc1/galgebra/_backports/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:46:56.563029 galgebra-0.5.2rc1/galgebra/_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-01 09:46:50.000000 galgebra-0.5.2rc1/galgebra/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-01 09:46:50.000000 galgebra-0.5.2rc1/galgebra/_utils/cached_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-01 09:46:50.000000 galgebra-0.5.2rc1/galgebra/_utils/kwarg_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-05-01 09:46:50.000000 galgebra-0.5.2rc1/galgebra/_utils/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-01 09:46:50.000000 galgebra-0.5.2rc1/galgebra/_utils/printable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-01 09:46:50.000000 galgebra-0.5.2rc1/galgebra/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-05-01 09:46:50.000000 galgebra-0.5.2rc1/galgebra/atoms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-05-01 09:46:50.000000 galgebra-0.5.2rc1/galgebra/deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12225 2024-05-01 09:46:50.000000 galgebra-0.5.2rc1/galgebra/dop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86234 2024-05-01 09:46:50.000000 galgebra-0.5.2rc1/galgebra/ga.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33789 2024-05-01 09:46:50.000000 galgebra-0.5.2rc1/galgebra/lt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27006 2024-05-01 09:46:50.000000 galgebra-0.5.2rc1/galgebra/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69857 2024-05-01 09:46:50.000000 galgebra-0.5.2rc1/galgebra/mv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42443 2024-05-01 09:46:50.000000 galgebra-0.5.2rc1/galgebra/printer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-01 09:46:50.000000 galgebra-0.5.2rc1/galgebra/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:46:56.559029 galgebra-0.5.2rc1/galgebra.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11765 2024-05-01 09:46:56.000000 galgebra-0.5.2rc1/galgebra.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-01 09:46:56.000000 galgebra-0.5.2rc1/galgebra.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 09:46:56.000000 galgebra-0.5.2rc1/galgebra.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-01 09:46:56.000000 galgebra-0.5.2rc1/galgebra.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-01 09:46:56.000000 galgebra-0.5.2rc1/galgebra.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-01 09:46:56.563029 galgebra-0.5.2rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-01 09:46:50.000000 galgebra-0.5.2rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:46:56.563029 galgebra-0.5.2rc1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-01 09:46:50.000000 galgebra-0.5.2rc1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11452 2024-05-01 09:46:50.000000 galgebra-0.5.2rc1/test/test_differential_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4570 2024-05-01 09:46:50.000000 galgebra-0.5.2rc1/test/test_lt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-05-01 09:46:50.000000 galgebra-0.5.2rc1/test/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7608 2024-05-01 09:46:50.000000 galgebra-0.5.2rc1/test/test_mv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3567 2024-05-01 09:46:50.000000 galgebra-0.5.2rc1/test/test_printer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25852 2024-05-01 09:46:50.000000 galgebra-0.5.2rc1/test/test_test.py
```

### Comparing `galgebra-0.5.1/LICENSE` & `galgebra-0.5.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `galgebra-0.5.1/PKG-INFO` & `galgebra-0.5.2rc1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galgebra
-Version: 0.5.1
+Version: 0.5.2rc1
 Summary: Symbolic Geometric Algebra/Calculus package for SymPy.
 Home-page: https://github.com/pygae/galgebra
 Author: Alan Bromborsky
 Maintainer: Hugo Hadfield
 Maintainer-email: hadfield.hugo@gmail.com
 License: BSD
 Project-URL: Documentation, http://galgebra.readthedocs.io
@@ -275,7 +275,32 @@
 Note that in the [doc/books](https://github.com/pygae/galgebra/blob/master/doc/books/) directory there are:
 
 - `BookGA.pdf` which is a collection of notes on Geometric Algebra and Calculus based of "Geometric Algebra for Physicists" by Doran and Lasenby and on some papers by Lasenby and Hestenes.
 - `galgebra.pdf` which is the original main doc of GAlgebra in PDF format, while the math part is still valid, the part describing the installation and usage of GAlgebra is outdated, please read with caution or visit https://galgebra.readthedocs.io/ instead.
 - `Macdonald` which contains bundled supplementary materials for [Linear and Geometric Algebra](http://www.faculty.luther.edu/~macdonal/laga/index.html) and [Vector and Geometric Calculus](http://www.faculty.luther.edu/~macdonal/vagc/index.html) by Alan Macdonald, see [here](https://github.com/pygae/galgebra/blob/master/doc/books/Macdonald/) and [here](https://github.com/pygae/galgebra/blob/master/examples/Macdonald/) for more information.
 
 <!-- end: bundled-resources -->
+
+Star History
+-------------------
+
+<a href="https://star-history.com/#pygae/galgebra&Date">
+ <picture>
+   <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=pygae/galgebra&type=Date&theme=dark" />
+   <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=pygae/galgebra&type=Date" />
+   <img alt="Star History Chart" src="https://api.star-history.com/svg?repos=pygae/galgebra&type=Date" />
+ </picture>
+</a>
+
+Contributors
+-------------------
+
+<a href="https://github.com/pygae/galgebra/graphs/contributors">
+  <img src="https://contrib.rocks/image?repo=pygae/galgebra" />
+</a>
+
+Made with [contrib.rocks](https://contrib.rocks).
+
+Citing This Library
+-------------------
+
+For citation information, see [our `CITATION.md` file](https://github.com/pygae/galgebra/blob/master/CITATION.md).
```

### Comparing `galgebra-0.5.1/README.md` & `galgebra-0.5.2rc1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -247,7 +247,32 @@
 Note that in the [doc/books](https://github.com/pygae/galgebra/blob/master/doc/books/) directory there are:
 
 - `BookGA.pdf` which is a collection of notes on Geometric Algebra and Calculus based of "Geometric Algebra for Physicists" by Doran and Lasenby and on some papers by Lasenby and Hestenes.
 - `galgebra.pdf` which is the original main doc of GAlgebra in PDF format, while the math part is still valid, the part describing the installation and usage of GAlgebra is outdated, please read with caution or visit https://galgebra.readthedocs.io/ instead.
 - `Macdonald` which contains bundled supplementary materials for [Linear and Geometric Algebra](http://www.faculty.luther.edu/~macdonal/laga/index.html) and [Vector and Geometric Calculus](http://www.faculty.luther.edu/~macdonal/vagc/index.html) by Alan Macdonald, see [here](https://github.com/pygae/galgebra/blob/master/doc/books/Macdonald/) and [here](https://github.com/pygae/galgebra/blob/master/examples/Macdonald/) for more information.
 
 <!-- end: bundled-resources -->
+
+Star History
+-------------------
+
+<a href="https://star-history.com/#pygae/galgebra&Date">
+ <picture>
+   <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=pygae/galgebra&type=Date&theme=dark" />
+   <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=pygae/galgebra&type=Date" />
+   <img alt="Star History Chart" src="https://api.star-history.com/svg?repos=pygae/galgebra&type=Date" />
+ </picture>
+</a>
+
+Contributors
+-------------------
+
+<a href="https://github.com/pygae/galgebra/graphs/contributors">
+  <img src="https://contrib.rocks/image?repo=pygae/galgebra" />
+</a>
+
+Made with [contrib.rocks](https://contrib.rocks).
+
+Citing This Library
+-------------------
+
+For citation information, see [our `CITATION.md` file](https://github.com/pygae/galgebra/blob/master/CITATION.md).
```

### Comparing `galgebra-0.5.1/galgebra/__init__.py` & `galgebra-0.5.2rc1/galgebra/__init__.py`

 * *Files identical despite different names*

### Comparing `galgebra-0.5.1/galgebra/_utils/cached_property.py` & `galgebra-0.5.2rc1/galgebra/_utils/cached_property.py`

 * *Files identical despite different names*

### Comparing `galgebra-0.5.1/galgebra/_utils/kwarg_parser.py` & `galgebra-0.5.2rc1/galgebra/_utils/kwarg_parser.py`

 * *Files identical despite different names*

### Comparing `galgebra-0.5.1/galgebra/_utils/parser.py` & `galgebra-0.5.2rc1/galgebra/_utils/parser.py`

 * *Files identical despite different names*

### Comparing `galgebra-0.5.1/galgebra/_utils/printable.py` & `galgebra-0.5.2rc1/galgebra/_utils/printable.py`

 * *Files identical despite different names*

### Comparing `galgebra-0.5.1/galgebra/atoms.py` & `galgebra-0.5.2rc1/galgebra/atoms.py`

 * *Files identical despite different names*

### Comparing `galgebra-0.5.1/galgebra/deprecated.py` & `galgebra-0.5.2rc1/galgebra/deprecated.py`

 * *Files identical despite different names*

### Comparing `galgebra-0.5.1/galgebra/dop.py` & `galgebra-0.5.2rc1/galgebra/dop.py`

 * *Files identical despite different names*

### Comparing `galgebra-0.5.1/galgebra/ga.py` & `galgebra-0.5.2rc1/galgebra/ga.py`

 * *Files identical despite different names*

### Comparing `galgebra-0.5.1/galgebra/lt.py` & `galgebra-0.5.2rc1/galgebra/lt.py`

 * *Files identical despite different names*

### Comparing `galgebra-0.5.1/galgebra/metric.py` & `galgebra-0.5.2rc1/galgebra/metric.py`

 * *Files identical despite different names*

### Comparing `galgebra-0.5.1/galgebra/mv.py` & `galgebra-0.5.2rc1/galgebra/mv.py`

 * *Files identical despite different names*

### Comparing `galgebra-0.5.1/galgebra/printer.py` & `galgebra-0.5.2rc1/galgebra/printer.py`

 * *Files identical despite different names*

### Comparing `galgebra-0.5.1/galgebra/utils.py` & `galgebra-0.5.2rc1/galgebra/utils.py`

 * *Files identical despite different names*

### Comparing `galgebra-0.5.1/galgebra.egg-info/PKG-INFO` & `galgebra-0.5.2rc1/galgebra.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galgebra
-Version: 0.5.1
+Version: 0.5.2rc1
 Summary: Symbolic Geometric Algebra/Calculus package for SymPy.
 Home-page: https://github.com/pygae/galgebra
 Author: Alan Bromborsky
 Maintainer: Hugo Hadfield
 Maintainer-email: hadfield.hugo@gmail.com
 License: BSD
 Project-URL: Documentation, http://galgebra.readthedocs.io
@@ -275,7 +275,32 @@
 Note that in the [doc/books](https://github.com/pygae/galgebra/blob/master/doc/books/) directory there are:
 
 - `BookGA.pdf` which is a collection of notes on Geometric Algebra and Calculus based of "Geometric Algebra for Physicists" by Doran and Lasenby and on some papers by Lasenby and Hestenes.
 - `galgebra.pdf` which is the original main doc of GAlgebra in PDF format, while the math part is still valid, the part describing the installation and usage of GAlgebra is outdated, please read with caution or visit https://galgebra.readthedocs.io/ instead.
 - `Macdonald` which contains bundled supplementary materials for [Linear and Geometric Algebra](http://www.faculty.luther.edu/~macdonal/laga/index.html) and [Vector and Geometric Calculus](http://www.faculty.luther.edu/~macdonal/vagc/index.html) by Alan Macdonald, see [here](https://github.com/pygae/galgebra/blob/master/doc/books/Macdonald/) and [here](https://github.com/pygae/galgebra/blob/master/examples/Macdonald/) for more information.
 
 <!-- end: bundled-resources -->
+
+Star History
+-------------------
+
+<a href="https://star-history.com/#pygae/galgebra&Date">
+ <picture>
+   <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=pygae/galgebra&type=Date&theme=dark" />
+   <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=pygae/galgebra&type=Date" />
+   <img alt="Star History Chart" src="https://api.star-history.com/svg?repos=pygae/galgebra&type=Date" />
+ </picture>
+</a>
+
+Contributors
+-------------------
+
+<a href="https://github.com/pygae/galgebra/graphs/contributors">
+  <img src="https://contrib.rocks/image?repo=pygae/galgebra" />
+</a>
+
+Made with [contrib.rocks](https://contrib.rocks).
+
+Citing This Library
+-------------------
+
+For citation information, see [our `CITATION.md` file](https://github.com/pygae/galgebra/blob/master/CITATION.md).
```

### Comparing `galgebra-0.5.1/galgebra.egg-info/SOURCES.txt` & `galgebra-0.5.2rc1/galgebra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `galgebra-0.5.1/setup.py` & `galgebra-0.5.2rc1/setup.py`

 * *Files identical despite different names*

### Comparing `galgebra-0.5.1/test/test_differential_ops.py` & `galgebra-0.5.2rc1/test/test_differential_ops.py`

 * *Files identical despite different names*

### Comparing `galgebra-0.5.1/test/test_lt.py` & `galgebra-0.5.2rc1/test/test_lt.py`

 * *Files identical despite different names*

### Comparing `galgebra-0.5.1/test/test_misc.py` & `galgebra-0.5.2rc1/test/test_misc.py`

 * *Files identical despite different names*

### Comparing `galgebra-0.5.1/test/test_mv.py` & `galgebra-0.5.2rc1/test/test_mv.py`

 * *Files identical despite different names*

### Comparing `galgebra-0.5.1/test/test_printer.py` & `galgebra-0.5.2rc1/test/test_printer.py`

 * *Files identical despite different names*

### Comparing `galgebra-0.5.1/test/test_test.py` & `galgebra-0.5.2rc1/test/test_test.py`

 * *Files identical despite different names*

