# Comparing `tmp/lsst-utils-26.2024.900.tar.gz` & `tmp/lsst_utils-27.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsst-utils-26.2024.900.tar", last modified: Thu Feb 29 10:20:57 2024, max compression
+gzip compressed data, was "lsst_utils-27.0.0rc1.tar", last modified: Wed May  1 21:16:16 2024, max compression
```

## Comparing `lsst-utils-26.2024.900.tar` & `lsst_utils-27.0.0rc1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:57.863523 lsst-utils-26.2024.900/
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-02-29 10:20:57.863523 lsst-utils-26.2024.900/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:57.851523 lsst-utils-26.2024.900/doc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:57.855523 lsst-utils-26.2024.900/doc/lsst.utils/
--rw-r--r--   0 runner    (1001) docker     (127)     9333 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/doc/lsst.utils/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/doc/lsst.utils/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:57.851523 lsst-utils-26.2024.900/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:57.855523 lsst-utils-26.2024.900/python/lsst/
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/python/lsst/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:57.859523 lsst-utils-26.2024.900/python/lsst/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/python/lsst/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/python/lsst/utils/_packaging.py
--rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/python/lsst/utils/classes.py
--rw-r--r--   0 runner    (1001) docker     (127)    11378 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/python/lsst/utils/db_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/python/lsst/utils/deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     4241 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/python/lsst/utils/doImport.py
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/python/lsst/utils/ellipsis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/python/lsst/utils/inheritDoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     9666 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/python/lsst/utils/introspection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/python/lsst/utils/iteration.py
--rw-r--r--   0 runner    (1001) docker     (127)    14795 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/python/lsst/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)    24665 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/python/lsst/utils/packages.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:57.859523 lsst-utils-26.2024.900/python/lsst/utils/plotting/
--rw-r--r--   0 runner    (1001) docker     (127)     5754 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/python/lsst/utils/plotting/limits.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/python/lsst/utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    39013 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/python/lsst/utils/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/python/lsst/utils/threads.py
--rw-r--r--   0 runner    (1001) docker     (127)    16662 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/python/lsst/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4598 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/python/lsst/utils/usage.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-29 10:20:57.000000 lsst-utils-26.2024.900/python/lsst/utils/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    19205 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/python/lsst/utils/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:57.863523 lsst-utils-26.2024.900/python/lsst_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-02-29 10:20:57.000000 lsst-utils-26.2024.900/python/lsst_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-02-29 10:20:57.000000 lsst-utils-26.2024.900/python/lsst_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 10:20:57.000000 lsst-utils-26.2024.900/python/lsst_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-02-29 10:20:57.000000 lsst-utils-26.2024.900/python/lsst_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-29 10:20:57.000000 lsst-utils-26.2024.900/python/lsst_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 10:20:57.000000 lsst-utils-26.2024.900/python/lsst_utils.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-02-29 10:20:57.863523 lsst-utils-26.2024.900/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:57.863523 lsst-utils-26.2024.900/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/tests/test_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)    18137 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/tests/test_db_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/tests/test_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/tests/test_doImport.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/tests/test_ellipsis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/tests/test_executables.py
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/tests/test_getPackageDir.py
--rw-r--r--   0 runner    (1001) docker     (127)     6342 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/tests/test_getTempFilePath.py
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/tests/test_inheritDoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5959 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/tests/test_introspection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/tests/test_iteration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5958 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/tests/test_ordering.py
--rw-r--r--   0 runner    (1001) docker     (127)     8375 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/tests/test_packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     9049 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/tests/test_plotting_limits.py
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/tests/test_threads.py
--rw-r--r--   0 runner    (1001) docker     (127)    13555 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/tests/test_timer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/tests/test_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)    13774 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17166 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/tests/test_wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:16.293961 lsst_utils-27.0.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-05-01 21:16:16.293961 lsst_utils-27.0.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:16.277961 lsst_utils-27.0.0rc1/doc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:16.281961 lsst_utils-27.0.0rc1/doc/lsst.utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     9333 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/doc/lsst.utils/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/doc/lsst.utils/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:16.281961 lsst_utils-27.0.0rc1/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:16.281961 lsst_utils-27.0.0rc1/python/lsst/
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/python/lsst/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:16.285961 lsst_utils-27.0.0rc1/python/lsst/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/python/lsst/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/python/lsst/utils/_packaging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/python/lsst/utils/classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11378 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/python/lsst/utils/db_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/python/lsst/utils/deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4241 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/python/lsst/utils/doImport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/python/lsst/utils/ellipsis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/python/lsst/utils/inheritDoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9666 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/python/lsst/utils/introspection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/python/lsst/utils/iteration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14836 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/python/lsst/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24665 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/python/lsst/utils/packages.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:16.285961 lsst_utils-27.0.0rc1/python/lsst/utils/plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)     5754 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/python/lsst/utils/plotting/limits.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/python/lsst/utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    39013 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/python/lsst/utils/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/python/lsst/utils/threads.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16806 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/python/lsst/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4598 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/python/lsst/utils/usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-01 21:16:16.000000 lsst_utils-27.0.0rc1/python/lsst/utils/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19205 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/python/lsst/utils/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:16.293961 lsst_utils-27.0.0rc1/python/lsst_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-05-01 21:16:16.000000 lsst_utils-27.0.0rc1/python/lsst_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-01 21:16:16.000000 lsst_utils-27.0.0rc1/python/lsst_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 21:16:16.000000 lsst_utils-27.0.0rc1/python/lsst_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-01 21:16:16.000000 lsst_utils-27.0.0rc1/python/lsst_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-01 21:16:16.000000 lsst_utils-27.0.0rc1/python/lsst_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 21:16:15.000000 lsst_utils-27.0.0rc1/python/lsst_utils.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-01 21:16:16.293961 lsst_utils-27.0.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:16.293961 lsst_utils-27.0.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/tests/test_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18133 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/tests/test_db_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/tests/test_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/tests/test_doImport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/tests/test_ellipsis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/tests/test_executables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/tests/test_getPackageDir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6342 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/tests/test_getTempFilePath.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/tests/test_inheritDoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5959 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/tests/test_introspection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/tests/test_iteration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5958 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/tests/test_ordering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8375 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/tests/test_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9049 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/tests/test_plotting_limits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/tests/test_threads.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13555 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/tests/test_timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/tests/test_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13774 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17166 2024-05-01 21:16:08.000000 lsst_utils-27.0.0rc1/tests/test_wrappers.py
```

### Comparing `lsst-utils-26.2024.900/LICENSE` & `lsst_utils-27.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.900/PKG-INFO` & `lsst_utils-27.0.0rc1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-utils
-Version: 26.2024.900
+Version: 27.0.0rc1
 Summary: Utility functions from Rubin Observatory Data Management for the Legacy Survey of Space and Time (LSST).
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/lsst/utils
 Keywords: lsst
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst-utils-26.2024.900/README.rst` & `lsst_utils-27.0.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.900/doc/lsst.utils/CHANGES.rst` & `lsst_utils-27.0.0rc1/doc/lsst.utils/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.900/doc/lsst.utils/index.rst` & `lsst_utils-27.0.0rc1/doc/lsst.utils/index.rst`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.900/pyproject.toml` & `lsst_utils-27.0.0rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -122,17 +122,21 @@
     "raise AssertionError",
     "raise NotImplementedError",
     "if __name__ == .__main__.:",
     "if TYPE_CHECKING:",
 ]
 
 [tool.ruff]
+line-length = 110
+target-version = "py311"
 exclude = [
     "__init__.py",
 ]
+
+[tool.ruff.lint]
 ignore = [
     "N802",
     "N803",
     "N806",
     "N812",
     "N815",
     "N816",
@@ -142,31 +146,29 @@
     "D102",
     "D104",
     "D100",
     "D200",
     "D205",
     "D400",
 ]
-line-length = 110
 select = [
     "E",  # pycodestyle
     "F",  # pyflakes
     "N",  # pep8-naming
     "W",  # pycodestyle
     "D",  # pydocstyle
 ]
-target-version = "py311"
 extend-select = [
     "RUF100", # Warn about unused noqa
 ]
 
-[tool.ruff.pycodestyle]
+[tool.ruff.lint.pycodestyle]
 max-doc-length = 79
 
-[tool.ruff.pydocstyle]
+[tool.ruff.lint.pydocstyle]
 convention = "numpy"
 
 [tool.numpydoc_validation]
 checks = [
     "all",  # All except the rules listed below.
     "SA01",  # See Also section.
     "EX01",  # Example section.
```

### Comparing `lsst-utils-26.2024.900/python/lsst/utils/__init__.py` & `lsst_utils-27.0.0rc1/python/lsst/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.900/python/lsst/utils/_packaging.py` & `lsst_utils-27.0.0rc1/python/lsst/utils/_packaging.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.900/python/lsst/utils/classes.py` & `lsst_utils-27.0.0rc1/python/lsst/utils/classes.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.900/python/lsst/utils/db_auth.py` & `lsst_utils-27.0.0rc1/python/lsst/utils/db_auth.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.900/python/lsst/utils/deprecated.py` & `lsst_utils-27.0.0rc1/python/lsst/utils/deprecated.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.900/python/lsst/utils/doImport.py` & `lsst_utils-27.0.0rc1/python/lsst/utils/doImport.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.900/python/lsst/utils/ellipsis.py` & `lsst_utils-27.0.0rc1/python/lsst/utils/ellipsis.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.900/python/lsst/utils/inheritDoc.py` & `lsst_utils-27.0.0rc1/python/lsst/utils/inheritDoc.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.900/python/lsst/utils/introspection.py` & `lsst_utils-27.0.0rc1/python/lsst/utils/introspection.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.900/python/lsst/utils/iteration.py` & `lsst_utils-27.0.0rc1/python/lsst/utils/iteration.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.900/python/lsst/utils/logging.py` & `lsst_utils-27.0.0rc1/python/lsst/utils/logging.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,25 +13,26 @@
 
 __all__ = (
     "TRACE",
     "VERBOSE",
     "getLogger",
     "getTraceLogger",
     "LsstLogAdapter",
+    "LsstLoggers",
     "PeriodicLogger",
     "trace_set_at",
 )
 
 import logging
 import sys
 import time
 from collections.abc import Generator
 from contextlib import contextmanager
 from logging import LoggerAdapter
-from typing import Any, Union
+from typing import Any, TypeAlias, Union
 
 try:
     import lsst.log.utils as logUtils
 except ImportError:
     logUtils = None
 
 
@@ -344,15 +345,15 @@
     if not logger:
         logger = logging.getLogger(name)
     elif name:
         logger = logger.getChild(name)
     return LsstLogAdapter(logger, {})
 
 
-LsstLoggers = Union[logging.Logger, LsstLogAdapter]
+LsstLoggers: TypeAlias = Union[logging.Logger, LsstLogAdapter]
 
 
 def getTraceLogger(logger: str | LsstLoggers, trace_level: int) -> LsstLogAdapter:
     """Get a logger with the appropriate TRACE name.
 
     Parameters
     ----------
```

### Comparing `lsst-utils-26.2024.900/python/lsst/utils/packages.py` & `lsst_utils-27.0.0rc1/python/lsst/utils/packages.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.900/python/lsst/utils/plotting/limits.py` & `lsst_utils-27.0.0rc1/python/lsst/utils/plotting/limits.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.900/python/lsst/utils/tests.py` & `lsst_utils-27.0.0rc1/python/lsst/utils/tests.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.900/python/lsst/utils/threads.py` & `lsst_utils-27.0.0rc1/python/lsst/utils/threads.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.900/python/lsst/utils/timer.py` & `lsst_utils-27.0.0rc1/python/lsst/utils/timer.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
 
 def logPairs(
     obj: Any,
     pairs: Collection[tuple[str, Any]],
     logLevel: int = logging.DEBUG,
     metadata: MutableMapping | None = None,
-    logger: logging.Logger | None = None,
+    logger: LsstLoggers | None = None,
     stacklevel: int | None = None,
 ) -> None:
     """Log ``(name, value)`` pairs to ``obj.metadata`` and ``obj.log``.
 
     Parameters
     ----------
     obj : `object`
@@ -95,15 +95,15 @@
         or this function will do nothing.
     pairs : sequence
         A sequence of ``(name, value)`` pairs, with value typically numeric.
     logLevel : `int, optional
         Log level (an `logging` level constant, such as `logging.DEBUG`).
     metadata : `collections.abc.MutableMapping`, optional
         Metadata object to write entries to.  Ignored if `None`.
-    logger : `logging.Logger`
+    logger : `logging.Logger` or `lsst.utils.logging.LsstLogAdapter`
         Log object to write entries to.  Ignored if `None`.
     stacklevel : `int`, optional
         The stack level to pass to the logger to adjust which stack frame
         is used to report the file information. If `None` the stack level
         is computed such that it is reported as the first package outside
         of the utils package. If a value is given here it is adjusted by
         1 to account for this caller.
@@ -137,15 +137,15 @@
 
 
 def logInfo(
     obj: Any,
     prefix: str,
     logLevel: int = logging.DEBUG,
     metadata: MutableMapping | None = None,
-    logger: logging.Logger | None = None,
+    logger: LsstLoggers | None = None,
     stacklevel: int | None = None,
 ) -> None:
     """Log timer information to ``obj.metadata`` and ``obj.log``.
 
     Parameters
     ----------
     obj : `object`
@@ -162,15 +162,15 @@
         Name prefix, the resulting entries are ``CpuTime``, etc.. For example
         `timeMethod` uses ``prefix = Start`` when the method begins and
         ``prefix = End`` when the method ends.
     logLevel : optional
         Log level (a `logging` level constant, such as `logging.DEBUG`).
     metadata : `collections.abc.MutableMapping`, optional
         Metadata object to write entries to, overriding ``obj.metadata``.
-    logger : `logging.Logger`
+    logger : `logging.Logger` or `lsst.utils.logging.LsstLogAdapter`
         Log object to write entries to, overriding ``obj.log``.
     stacklevel : `int`, optional
         The stack level to pass to the logger to adjust which stack frame
         is used to report the file information. If `None` the stack level
         is computed such that it is reported as the first package outside
         of the utils package. If a value is given here it is adjusted by
         1 to account for this caller.
@@ -227,27 +227,27 @@
     )
 
 
 def timeMethod(
     _func: Any | None = None,
     *,
     metadata: MutableMapping | None = None,
-    logger: logging.Logger | None = None,
+    logger: LsstLoggers | None = None,
     logLevel: int = logging.DEBUG,
 ) -> Callable:
     """Measure duration of a method.
 
     Parameters
     ----------
     _func : `~collections.abc.Callable` or `None`
         The method to wrap.
     metadata : `collections.abc.MutableMapping`, optional
         Metadata to use as override if the instance object attached
         to this timer does not support a ``metadata`` property.
-    logger : `logging.Logger`, optional
+    logger : `logging.Logger` or `lsst.utils.logging.LsstLogAdapter`, optional
         Logger to use when the class containing the decorated method does not
         have a ``log`` property.
     logLevel : `int`, optional
         Log level to use when logging messages. Default is `~logging.DEBUG`.
 
     Notes
     -----
@@ -425,23 +425,23 @@
                 f", delta: {current_delta.to(mem_unit):{mem_fmt}}"
                 f", peak delta: {peak_delta.to(mem_unit):{mem_fmt}}"
             )
         log.log(level, msg, *params, stacklevel=3)
 
 
 @contextmanager
-def profile(filename: str | None, log: logging.Logger | None = None) -> Iterator[cProfile.Profile | None]:
+def profile(filename: str | None, log: LsstLoggers | None = None) -> Iterator[cProfile.Profile | None]:
     """Profile the enclosed code block and save the result to a file.
 
     Parameters
     ----------
     filename : `str` or `None`
         Filename to which to write profile (profiling disabled if `None` or
         empty string).
-    log : `logging.Logger`, optional
+    log : `logging.Logger` or `lsst.utils.logging.LsstLogAdapter`, optional
         Log object for logging the profile operations.
 
     Yields
     ------
     prof : `cProfile.Profile` or `None`
         If profiling is enabled, the context manager returns the
         `cProfile.Profile` object (otherwise it returns `None`),
```

### Comparing `lsst-utils-26.2024.900/python/lsst/utils/usage.py` & `lsst_utils-27.0.0rc1/python/lsst/utils/usage.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.900/python/lsst/utils/wrappers.py` & `lsst_utils-27.0.0rc1/python/lsst/utils/wrappers.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.900/python/lsst_utils.egg-info/PKG-INFO` & `lsst_utils-27.0.0rc1/python/lsst_utils.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-utils
-Version: 26.2024.900
+Version: 27.0.0rc1
 Summary: Utility functions from Rubin Observatory Data Management for the Legacy Survey of Space and Time (LSST).
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/lsst/utils
 Keywords: lsst
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst-utils-26.2024.900/python/lsst_utils.egg-info/SOURCES.txt` & `lsst_utils-27.0.0rc1/python/lsst_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.900/tests/test_classes.py` & `lsst_utils-27.0.0rc1/tests/test_classes.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.900/tests/test_db_auth.py` & `lsst_utils-27.0.0rc1/tests/test_db_auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -229,27 +229,27 @@
 
         auth = DbAuth(
             authList=[dict(url="postgresql://host.example.com/my_database", username="foo", password="bar")]
         )
         self.assertEqual(
             auth.getUrl("postgresql://user@host.example.com:5432/my_database"),
             "postgresql://user:bar@host.example.com:5432/my_database",
-        ),
+        )
         self.assertEqual(
             auth.getUrl("postgresql://user@host.example.com/my_database"),
             "postgresql://user:bar@host.example.com/my_database",
-        ),
+        )
         self.assertEqual(
             auth.getUrl("postgresql://host.example.com/my_database"),
             "postgresql://foo:bar@host.example.com/my_database",
-        ),
+        )
         self.assertEqual(
             auth.getUrl("postgresql://host.example.com:5432/my_database"),
             "postgresql://foo:bar@host.example.com:5432/my_database",
-        ),
+        )
 
         filePath = os.path.join(TESTDIR, "db-auth.yaml")
         os.chmod(filePath, 0o600)
         auth = DbAuth(filePath)
         self.assertEqual(
             auth.getUrl("postgresql://user@host.example.com:5432/my_database"),
             "postgresql://user:test1@host.example.com:5432/my_database",
```

### Comparing `lsst-utils-26.2024.900/tests/test_decorators.py` & `lsst_utils-27.0.0rc1/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.900/tests/test_deprecated.py` & `lsst_utils-27.0.0rc1/tests/test_deprecated.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.900/tests/test_doImport.py` & `lsst_utils-27.0.0rc1/tests/test_doImport.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.900/tests/test_ellipsis.py` & `lsst_utils-27.0.0rc1/tests/test_ellipsis.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.900/tests/test_executables.py` & `lsst_utils-27.0.0rc1/tests/test_executables.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.900/tests/test_getPackageDir.py` & `lsst_utils-27.0.0rc1/tests/test_getPackageDir.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.900/tests/test_getTempFilePath.py` & `lsst_utils-27.0.0rc1/tests/test_getTempFilePath.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.900/tests/test_import.py` & `lsst_utils-27.0.0rc1/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.900/tests/test_inheritDoc.py` & `lsst_utils-27.0.0rc1/tests/test_inheritDoc.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.900/tests/test_introspection.py` & `lsst_utils-27.0.0rc1/tests/test_introspection.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.900/tests/test_iteration.py` & `lsst_utils-27.0.0rc1/tests/test_iteration.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.900/tests/test_logging.py` & `lsst_utils-27.0.0rc1/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.900/tests/test_ordering.py` & `lsst_utils-27.0.0rc1/tests/test_ordering.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.900/tests/test_packages.py` & `lsst_utils-27.0.0rc1/tests/test_packages.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.900/tests/test_plotting_limits.py` & `lsst_utils-27.0.0rc1/tests/test_plotting_limits.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.900/tests/test_threads.py` & `lsst_utils-27.0.0rc1/tests/test_threads.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.900/tests/test_timer.py` & `lsst_utils-27.0.0rc1/tests/test_timer.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.900/tests/test_usage.py` & `lsst_utils-27.0.0rc1/tests/test_usage.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.900/tests/test_utils.py` & `lsst_utils-27.0.0rc1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.900/tests/test_wrappers.py` & `lsst_utils-27.0.0rc1/tests/test_wrappers.py`

 * *Files identical despite different names*

