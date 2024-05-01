# Comparing `tmp/scikit-ued-2.1.8.tar.gz` & `tmp/scikit-ued-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit-ued-2.1.8.tar", last modified: Sun Jul  3 23:35:28 2022, max compression
+gzip compressed data, was "scikit-ued-2.1.9.tar", last modified: Thu Aug  4 16:21:45 2022, max compression
```

## Comparing `scikit-ued-2.1.8.tar` & `scikit-ued-2.1.9.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-03 23:35:28.774663 scikit-ued-2.1.8/
--rw-r--r--   0 runner     (501) staff       (20)     6666 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/CHANGELOG.rst
--rw-r--r--   0 runner     (501) staff       (20)    35148 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/LICENSE.txt
--rw-r--r--   0 runner     (501) staff       (20)      314 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)     5075 2022-07-03 23:35:28.774837 scikit-ued-2.1.8/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     3896 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/README.md
--rw-r--r--   0 runner     (501) staff       (20)       74 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/dev-requirements.txt
--rw-r--r--   0 runner     (501) staff       (20)      205 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/requirements.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-03 23:35:28.700376 scikit-ued-2.1.8/scikit_ued.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     5075 2022-07-03 23:35:28.000000 scikit-ued-2.1.8/scikit_ued.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     2874 2022-07-03 23:35:28.000000 scikit-ued-2.1.8/scikit_ued.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2022-07-03 23:35:28.000000 scikit-ued-2.1.8/scikit_ued.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)       47 2022-07-03 23:35:28.000000 scikit-ued-2.1.8/scikit_ued.egg-info/entry_points.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2022-07-03 23:31:08.000000 scikit-ued-2.1.8/scikit_ued.egg-info/not-zip-safe
--rw-r--r--   0 runner     (501) staff       (20)      174 2022-07-03 23:35:28.000000 scikit-ued-2.1.8/scikit_ued.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)        6 2022-07-03 23:35:28.000000 scikit-ued-2.1.8/scikit_ued.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)      108 2022-07-03 23:35:28.775515 scikit-ued-2.1.8/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)     3116 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-03 23:35:28.708810 scikit-ued-2.1.8/skued/
--rw-r--r--   0 runner     (501) staff       (20)     1928 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1577 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/__main__.py
--rw-r--r--   0 runner     (501) staff       (20)     8392 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/affine.py
--rw-r--r--   0 runner     (501) staff       (20)     5310 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/array_utils.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-03 23:35:28.710809 scikit-ued-2.1.8/skued/baseline/
--rw-r--r--   0 runner     (501) staff       (20)      337 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/baseline/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    17075 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/baseline/algorithms.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-03 23:35:28.714639 scikit-ued-2.1.8/skued/baseline/data/
--rw-r--r--   0 runner     (501) staff       (20)     2565 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/baseline/data/qshift1.npz
--rw-r--r--   0 runner     (501) staff       (20)     2837 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/baseline/data/qshift2.npz
--rw-r--r--   0 runner     (501) staff       (20)     2973 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/baseline/data/qshift3.npz
--rw-r--r--   0 runner     (501) staff       (20)     3109 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/baseline/data/qshift4.npz
--rw-r--r--   0 runner     (501) staff       (20)     2359 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/baseline/data/qshift5.npz
--rw-r--r--   0 runner     (501) staff       (20)     4238 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/baseline/data/qshift6.npz
--rw-r--r--   0 runner     (501) staff       (20)    13764 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/baseline/dtcwt.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-03 23:35:28.720602 scikit-ued-2.1.8/skued/baseline/tests/
--rw-r--r--   0 runner     (501) staff       (20)       24 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/baseline/tests/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     5269 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/baseline/tests/test_algorithms.py
--rw-r--r--   0 runner     (501) staff       (20)     4496 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/baseline/tests/test_dtcwt.py
--rw-r--r--   0 runner     (501) staff       (20)     2643 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/eproperties.py
--rw-r--r--   0 runner     (501) staff       (20)     1083 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/fft.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-03 23:35:28.728766 scikit-ued-2.1.8/skued/image/
--rw-r--r--   0 runner     (501) staff       (20)      456 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/image/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4291 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/image/alignment.py
--rw-r--r--   0 runner     (501) staff       (20)     6873 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/image/calibration.py
--rw-r--r--   0 runner     (501) staff       (20)     4165 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/image/center.py
--rw-r--r--   0 runner     (501) staff       (20)     3636 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/image/indexing.py
--rw-r--r--   0 runner     (501) staff       (20)     7764 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/image/metrics.py
--rw-r--r--   0 runner     (501) staff       (20)     3364 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/image/powder.py
--rw-r--r--   0 runner     (501) staff       (20)     5026 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/image/symmetry.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-03 23:35:28.733341 scikit-ued-2.1.8/skued/image/tests/
--rw-r--r--   0 runner     (501) staff       (20)       24 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/image/tests/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     3347 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/image/tests/test_alignment.py
--rw-r--r--   0 runner     (501) staff       (20)     3282 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/image/tests/test_calibration.py
--rw-r--r--   0 runner     (501) staff       (20)     4120 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/image/tests/test_center.py
--rw-r--r--   0 runner     (501) staff       (20)     1421 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/image/tests/test_indexing.py
--rw-r--r--   0 runner     (501) staff       (20)     5118 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/image/tests/test_metrics.py
--rw-r--r--   0 runner     (501) staff       (20)     4922 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/image/tests/test_powder.py
--rw-r--r--   0 runner     (501) staff       (20)     5658 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/image/tests/test_symmetry.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-03 23:35:28.736012 scikit-ued-2.1.8/skued/io/
--rw-r--r--   0 runner     (501) staff       (20)      286 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/io/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     3125 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/io/diffshow.py
--rw-r--r--   0 runner     (501) staff       (20)    22632 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/io/dm.py
--rw-r--r--   0 runner     (501) staff       (20)     1248 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/io/io.py
--rw-r--r--   0 runner     (501) staff       (20)     4221 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/io/merlin.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-03 23:35:28.736801 scikit-ued-2.1.8/skued/io/tests/
--rw-r--r--   0 runner     (501) staff       (20)        0 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/io/tests/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-03 23:35:28.748916 scikit-ued-2.1.8/skued/io/tests/data/
--rw-r--r--   0 runner     (501) staff       (20)   675364 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/io/tests/data/bismuth.dm3
--rw-r--r--   0 runner     (501) staff       (20)   682800 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/io/tests/data/bismuth.dm4
--rw-r--r--   0 runner     (501) staff       (20)      770 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/io/tests/data/png_test.png
--rw-r--r--   0 runner     (501) staff       (20)   131456 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/io/tests/data/test.mib
--rw-r--r--   0 runner     (501) staff       (20)   593280 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/io/tests/data/test_multi.mib
--rw-r--r--   0 runner     (501) staff       (20)     3376 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/io/tests/test_io.py
--rw-r--r--   0 runner     (501) staff       (20)     1793 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/patterson.py
--rw-r--r--   0 runner     (501) staff       (20)     4538 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/plot_utils.py
--rw-r--r--   0 runner     (501) staff       (20)     5548 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/potential_map.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-03 23:35:28.761196 scikit-ued-2.1.8/skued/simulation/
--rw-r--r--   0 runner     (501) staff       (20)      201 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/simulation/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-03 23:35:28.761638 scikit-ued-2.1.8/skued/simulation/data/
--rw-r--r--   0 runner     (501) staff       (20)    45935 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/simulation/data/aspherical.yaml
--rw-r--r--   0 runner     (501) staff       (20)     4408 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/simulation/form_factors.py
--rw-r--r--   0 runner     (501) staff       (20)     3904 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/simulation/kinematic.py
--rw-r--r--   0 runner     (501) staff       (20)     4655 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/simulation/potential.py
--rw-r--r--   0 runner     (501) staff       (20)     1397 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/simulation/powdersim.py
--rw-r--r--   0 runner     (501) staff       (20)    42606 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/simulation/scattering_params.py
--rw-r--r--   0 runner     (501) staff       (20)     2274 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/simulation/structure_factors.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-03 23:35:28.764135 scikit-ued-2.1.8/skued/simulation/tests/
--rw-r--r--   0 runner     (501) staff       (20)       24 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/simulation/tests/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1786 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/simulation/tests/test_kinematic.py
--rw-r--r--   0 runner     (501) staff       (20)     1883 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/simulation/tests/test_potential.py
--rw-r--r--   0 runner     (501) staff       (20)      992 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/simulation/tests/test_powdersim.py
--rw-r--r--   0 runner     (501) staff       (20)     1405 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/simulation/tests/test_structure_factors.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-03 23:35:28.768661 scikit-ued-2.1.8/skued/tests/
--rw-r--r--   0 runner     (501) staff       (20)       24 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/tests/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     5732 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/tests/test_affine.py
--rw-r--r--   0 runner     (501) staff       (20)     3946 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/tests/test_array_utils.py
--rw-r--r--   0 runner     (501) staff       (20)     1753 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/tests/test_eproperties.py
--rw-r--r--   0 runner     (501) staff       (20)      509 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/tests/test_patterson.py
--rw-r--r--   0 runner     (501) staff       (20)     1682 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/tests/test_plot_utils.py
--rw-r--r--   0 runner     (501) staff       (20)     3907 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/tests/test_potential_map.py
--rw-r--r--   0 runner     (501) staff       (20)      768 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/tests/test_thin_films.py
--rw-r--r--   0 runner     (501) staff       (20)     1865 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/tests/test_voigt.py
--rw-r--r--   0 runner     (501) staff       (20)     2474 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/thin_films.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-03 23:35:28.771479 scikit-ued-2.1.8/skued/time_series/
--rw-r--r--   0 runner     (501) staff       (20)      519 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/time_series/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     6008 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/time_series/fitting.py
--rw-r--r--   0 runner     (501) staff       (20)     2657 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/time_series/nfft_routines.py
--rw-r--r--   0 runner     (501) staff       (20)      567 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/time_series/robust.py
--rw-r--r--   0 runner     (501) staff       (20)    11496 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/time_series/selections.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-03 23:35:28.774178 scikit-ued-2.1.8/skued/time_series/tests/
--rw-r--r--   0 runner     (501) staff       (20)        0 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/time_series/tests/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     6251 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/time_series/tests/test_fitting.py
--rw-r--r--   0 runner     (501) staff       (20)      666 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/time_series/tests/test_nfft.py
--rw-r--r--   0 runner     (501) staff       (20)      939 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/time_series/tests/test_robust.py
--rw-r--r--   0 runner     (501) staff       (20)     2853 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/time_series/tests/test_selections.py
--rw-r--r--   0 runner     (501) staff       (20)     3121 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/time_series/tests/test_time_zero.py
--rw-r--r--   0 runner     (501) staff       (20)     4378 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/time_series/time_zero.py
--rw-r--r--   0 runner     (501) staff       (20)      997 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/utils.py
--rw-r--r--   0 runner     (501) staff       (20)     6651 2022-07-03 23:29:31.000000 scikit-ued-2.1.8/skued/voigt.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-04 16:21:45.228227 scikit-ued-2.1.9/
+-rw-r--r--   0 runner     (501) staff       (20)     6729 2022-08-04 16:13:57.000000 scikit-ued-2.1.9/CHANGELOG.rst
+-rw-r--r--   0 runner     (501) staff       (20)    35148 2022-08-04 16:13:57.000000 scikit-ued-2.1.9/LICENSE.txt
+-rw-r--r--   0 runner     (501) staff       (20)      314 2022-08-04 16:13:57.000000 scikit-ued-2.1.9/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)     5075 2022-08-04 16:21:45.228424 scikit-ued-2.1.9/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     3896 2022-08-04 16:13:57.000000 scikit-ued-2.1.9/README.md
+-rw-r--r--   0 runner     (501) staff       (20)       74 2022-08-04 16:13:57.000000 scikit-ued-2.1.9/dev-requirements.txt
+-rw-r--r--   0 runner     (501) staff       (20)      205 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/requirements.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-04 16:21:45.156436 scikit-ued-2.1.9/scikit_ued.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     5075 2022-08-04 16:21:45.000000 scikit-ued-2.1.9/scikit_ued.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     2874 2022-08-04 16:21:45.000000 scikit-ued-2.1.9/scikit_ued.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2022-08-04 16:21:45.000000 scikit-ued-2.1.9/scikit_ued.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)       47 2022-08-04 16:21:45.000000 scikit-ued-2.1.9/scikit_ued.egg-info/entry_points.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2022-08-04 16:16:21.000000 scikit-ued-2.1.9/scikit_ued.egg-info/not-zip-safe
+-rw-r--r--   0 runner     (501) staff       (20)      183 2022-08-04 16:21:45.000000 scikit-ued-2.1.9/scikit_ued.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)        6 2022-08-04 16:21:45.000000 scikit-ued-2.1.9/scikit_ued.egg-info/top_level.txt
+-rw-r--r--   0 runner     (501) staff       (20)      108 2022-08-04 16:21:45.229864 scikit-ued-2.1.9/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)     3125 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-04 16:21:45.163077 scikit-ued-2.1.9/skued/
+-rw-r--r--   0 runner     (501) staff       (20)     1928 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1577 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/__main__.py
+-rw-r--r--   0 runner     (501) staff       (20)     8392 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/affine.py
+-rw-r--r--   0 runner     (501) staff       (20)     5310 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/array_utils.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-04 16:21:45.165187 scikit-ued-2.1.9/skued/baseline/
+-rw-r--r--   0 runner     (501) staff       (20)      337 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/baseline/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    17075 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/baseline/algorithms.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-04 16:21:45.173716 scikit-ued-2.1.9/skued/baseline/data/
+-rw-r--r--   0 runner     (501) staff       (20)     2565 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/baseline/data/qshift1.npz
+-rw-r--r--   0 runner     (501) staff       (20)     2837 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/baseline/data/qshift2.npz
+-rw-r--r--   0 runner     (501) staff       (20)     2973 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/baseline/data/qshift3.npz
+-rw-r--r--   0 runner     (501) staff       (20)     3109 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/baseline/data/qshift4.npz
+-rw-r--r--   0 runner     (501) staff       (20)     2359 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/baseline/data/qshift5.npz
+-rw-r--r--   0 runner     (501) staff       (20)     4238 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/baseline/data/qshift6.npz
+-rw-r--r--   0 runner     (501) staff       (20)    13764 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/baseline/dtcwt.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-04 16:21:45.175686 scikit-ued-2.1.9/skued/baseline/tests/
+-rw-r--r--   0 runner     (501) staff       (20)       24 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/baseline/tests/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     5269 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/baseline/tests/test_algorithms.py
+-rw-r--r--   0 runner     (501) staff       (20)     4496 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/baseline/tests/test_dtcwt.py
+-rw-r--r--   0 runner     (501) staff       (20)     2643 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/eproperties.py
+-rw-r--r--   0 runner     (501) staff       (20)     1083 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/fft.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-04 16:21:45.180388 scikit-ued-2.1.9/skued/image/
+-rw-r--r--   0 runner     (501) staff       (20)      456 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/image/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4291 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/image/alignment.py
+-rw-r--r--   0 runner     (501) staff       (20)     6873 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/image/calibration.py
+-rw-r--r--   0 runner     (501) staff       (20)     4165 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/image/center.py
+-rw-r--r--   0 runner     (501) staff       (20)     3636 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/image/indexing.py
+-rw-r--r--   0 runner     (501) staff       (20)     7764 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/image/metrics.py
+-rw-r--r--   0 runner     (501) staff       (20)     3364 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/image/powder.py
+-rw-r--r--   0 runner     (501) staff       (20)     5026 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/image/symmetry.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-04 16:21:45.184810 scikit-ued-2.1.9/skued/image/tests/
+-rw-r--r--   0 runner     (501) staff       (20)       24 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/image/tests/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     3347 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/image/tests/test_alignment.py
+-rw-r--r--   0 runner     (501) staff       (20)     3282 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/image/tests/test_calibration.py
+-rw-r--r--   0 runner     (501) staff       (20)     4120 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/image/tests/test_center.py
+-rw-r--r--   0 runner     (501) staff       (20)     1421 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/image/tests/test_indexing.py
+-rw-r--r--   0 runner     (501) staff       (20)     5118 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/image/tests/test_metrics.py
+-rw-r--r--   0 runner     (501) staff       (20)     4922 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/image/tests/test_powder.py
+-rw-r--r--   0 runner     (501) staff       (20)     5658 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/image/tests/test_symmetry.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-04 16:21:45.188589 scikit-ued-2.1.9/skued/io/
+-rw-r--r--   0 runner     (501) staff       (20)      286 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/io/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     3129 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/io/diffshow.py
+-rw-r--r--   0 runner     (501) staff       (20)    22632 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/io/dm.py
+-rw-r--r--   0 runner     (501) staff       (20)     1248 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/io/io.py
+-rw-r--r--   0 runner     (501) staff       (20)     4221 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/io/merlin.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-04 16:21:45.189481 scikit-ued-2.1.9/skued/io/tests/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/io/tests/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-04 16:21:45.196603 scikit-ued-2.1.9/skued/io/tests/data/
+-rw-r--r--   0 runner     (501) staff       (20)   675364 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/io/tests/data/bismuth.dm3
+-rw-r--r--   0 runner     (501) staff       (20)   682800 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/io/tests/data/bismuth.dm4
+-rw-r--r--   0 runner     (501) staff       (20)      770 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/io/tests/data/png_test.png
+-rw-r--r--   0 runner     (501) staff       (20)   131456 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/io/tests/data/test.mib
+-rw-r--r--   0 runner     (501) staff       (20)   593280 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/io/tests/data/test_multi.mib
+-rw-r--r--   0 runner     (501) staff       (20)     3376 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/io/tests/test_io.py
+-rw-r--r--   0 runner     (501) staff       (20)     1793 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/patterson.py
+-rw-r--r--   0 runner     (501) staff       (20)     4538 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/plot_utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     5548 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/potential_map.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-04 16:21:45.204520 scikit-ued-2.1.9/skued/simulation/
+-rw-r--r--   0 runner     (501) staff       (20)      201 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/simulation/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-04 16:21:45.207279 scikit-ued-2.1.9/skued/simulation/data/
+-rw-r--r--   0 runner     (501) staff       (20)    45935 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/simulation/data/aspherical.yaml
+-rw-r--r--   0 runner     (501) staff       (20)     4408 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/simulation/form_factors.py
+-rw-r--r--   0 runner     (501) staff       (20)     3904 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/simulation/kinematic.py
+-rw-r--r--   0 runner     (501) staff       (20)     4655 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/simulation/potential.py
+-rw-r--r--   0 runner     (501) staff       (20)     1397 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/simulation/powdersim.py
+-rw-r--r--   0 runner     (501) staff       (20)    42606 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/simulation/scattering_params.py
+-rw-r--r--   0 runner     (501) staff       (20)     2274 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/simulation/structure_factors.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-04 16:21:45.212645 scikit-ued-2.1.9/skued/simulation/tests/
+-rw-r--r--   0 runner     (501) staff       (20)       24 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/simulation/tests/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1786 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/simulation/tests/test_kinematic.py
+-rw-r--r--   0 runner     (501) staff       (20)     1883 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/simulation/tests/test_potential.py
+-rw-r--r--   0 runner     (501) staff       (20)      992 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/simulation/tests/test_powdersim.py
+-rw-r--r--   0 runner     (501) staff       (20)     1405 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/simulation/tests/test_structure_factors.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-04 16:21:45.219079 scikit-ued-2.1.9/skued/tests/
+-rw-r--r--   0 runner     (501) staff       (20)       24 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/tests/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     5732 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/tests/test_affine.py
+-rw-r--r--   0 runner     (501) staff       (20)     3946 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/tests/test_array_utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     1753 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/tests/test_eproperties.py
+-rw-r--r--   0 runner     (501) staff       (20)      509 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/tests/test_patterson.py
+-rw-r--r--   0 runner     (501) staff       (20)     1682 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/tests/test_plot_utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     3907 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/tests/test_potential_map.py
+-rw-r--r--   0 runner     (501) staff       (20)      768 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/tests/test_thin_films.py
+-rw-r--r--   0 runner     (501) staff       (20)     1865 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/tests/test_voigt.py
+-rw-r--r--   0 runner     (501) staff       (20)     2474 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/thin_films.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-04 16:21:45.222714 scikit-ued-2.1.9/skued/time_series/
+-rw-r--r--   0 runner     (501) staff       (20)      519 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/time_series/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     6008 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/time_series/fitting.py
+-rw-r--r--   0 runner     (501) staff       (20)     2657 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/time_series/nfft_routines.py
+-rw-r--r--   0 runner     (501) staff       (20)      567 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/time_series/robust.py
+-rw-r--r--   0 runner     (501) staff       (20)    11496 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/time_series/selections.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-04 16:21:45.227543 scikit-ued-2.1.9/skued/time_series/tests/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/time_series/tests/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     6251 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/time_series/tests/test_fitting.py
+-rw-r--r--   0 runner     (501) staff       (20)      666 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/time_series/tests/test_nfft.py
+-rw-r--r--   0 runner     (501) staff       (20)      939 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/time_series/tests/test_robust.py
+-rw-r--r--   0 runner     (501) staff       (20)     2853 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/time_series/tests/test_selections.py
+-rw-r--r--   0 runner     (501) staff       (20)     3121 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/time_series/tests/test_time_zero.py
+-rw-r--r--   0 runner     (501) staff       (20)     4378 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/time_series/time_zero.py
+-rw-r--r--   0 runner     (501) staff       (20)      997 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     6651 2022-08-04 16:13:58.000000 scikit-ued-2.1.9/skued/voigt.py
```

### Comparing `scikit-ued-2.1.8/CHANGELOG.rst` & `scikit-ued-2.1.9/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Changelog
 =========
 
+Release 2.1.9
+-------------
+
+* Updated bounds on `pyqtgraph`.
+
 Release 2.1.8
 -------------
 
 * Added explicit testing with python 3.10.
 * Cleaned up unused imports.
 * Updated some modules which were using deprecated code.
```

### Comparing `scikit-ued-2.1.8/LICENSE.txt` & `scikit-ued-2.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/PKG-INFO` & `scikit-ued-2.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-ued
-Version: 2.1.8
+Version: 2.1.9
 Summary: Collection of algorithms and functions for ultrafast electron scattering
 Home-page: http://scikit-ued.readthedocs.io
 Author: Laurent P. René de Cotret
 Author-email: laurent.renedecotret@mail.mcgill.ca
 Maintainer: Laurent P. René de Cotret
 Maintainer-email: laurent.renedecotret@mail.mcgill.ca
 License: GPLv3
```

### Comparing `scikit-ued-2.1.8/README.md` & `scikit-ued-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/scikit_ued.egg-info/PKG-INFO` & `scikit-ued-2.1.9/scikit_ued.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-ued
-Version: 2.1.8
+Version: 2.1.9
 Summary: Collection of algorithms and functions for ultrafast electron scattering
 Home-page: http://scikit-ued.readthedocs.io
 Author: Laurent P. René de Cotret
 Author-email: laurent.renedecotret@mail.mcgill.ca
 Maintainer: Laurent P. René de Cotret
 Maintainer-email: laurent.renedecotret@mail.mcgill.ca
 License: GPLv3
```

### Comparing `scikit-ued-2.1.8/scikit_ued.egg-info/SOURCES.txt` & `scikit-ued-2.1.9/scikit_ued.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/setup.py` & `scikit-ued-2.1.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         download_url=DOWNLOAD_URL,
         version=VERSION,
         author=AUTHOR,
         author_email=AUTHOR_EMAIL,
         maintainer=AUTHOR,
         maintainer_email=AUTHOR_EMAIL,
         install_requires=REQUIREMENTS,
-        extras_require={"diffshow": ["pyqtgraph", "PyQt5"]},
+        extras_require={"diffshow": ["pyqtgraph>=0.12,<1", "PyQt5"]},
         keywords="ultrafast electron scattering",
         project_urls={
             "Documentation": "https://scikit-ued.readthedocs.io/",
             "Source": "https://github.com/LaurentRDC/scikit-ued",
         },
         python_requires=">=3.7",
         packages=PACKAGES,
```

### Comparing `scikit-ued-2.1.8/skued/__init__.py` & `scikit-ued-2.1.9/skued/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 __author__ = "Laurent P. René de Cotret"
 __email__ = "laurent.renedecotret@mail.mcgill.ca"
 __license__ = "GPLv3"
-__version__ = "2.1.8"
+__version__ = "2.1.9"
 
 from .affine import (
     affine_map,
     change_basis_mesh,
     change_of_basis,
     is_basis,
     is_rotation_matrix,
```

### Comparing `scikit-ued-2.1.8/skued/__main__.py` & `scikit-ued-2.1.9/skued/__main__.py`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/affine.py` & `scikit-ued-2.1.9/skued/affine.py`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/array_utils.py` & `scikit-ued-2.1.9/skued/array_utils.py`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/baseline/algorithms.py` & `scikit-ued-2.1.9/skued/baseline/algorithms.py`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/baseline/data/qshift1.npz` & `scikit-ued-2.1.9/skued/baseline/data/qshift1.npz`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/baseline/data/qshift2.npz` & `scikit-ued-2.1.9/skued/baseline/data/qshift2.npz`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/baseline/data/qshift3.npz` & `scikit-ued-2.1.9/skued/baseline/data/qshift3.npz`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/baseline/data/qshift4.npz` & `scikit-ued-2.1.9/skued/baseline/data/qshift4.npz`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/baseline/data/qshift5.npz` & `scikit-ued-2.1.9/skued/baseline/data/qshift5.npz`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/baseline/data/qshift6.npz` & `scikit-ued-2.1.9/skued/baseline/data/qshift6.npz`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/baseline/dtcwt.py` & `scikit-ued-2.1.9/skued/baseline/dtcwt.py`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/baseline/tests/test_algorithms.py` & `scikit-ued-2.1.9/skued/baseline/tests/test_algorithms.py`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/baseline/tests/test_dtcwt.py` & `scikit-ued-2.1.9/skued/baseline/tests/test_dtcwt.py`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/eproperties.py` & `scikit-ued-2.1.9/skued/eproperties.py`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/fft.py` & `scikit-ued-2.1.9/skued/fft.py`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/image/alignment.py` & `scikit-ued-2.1.9/skued/image/alignment.py`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/image/calibration.py` & `scikit-ued-2.1.9/skued/image/calibration.py`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/image/center.py` & `scikit-ued-2.1.9/skued/image/center.py`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/image/indexing.py` & `scikit-ued-2.1.9/skued/image/indexing.py`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/image/metrics.py` & `scikit-ued-2.1.9/skued/image/metrics.py`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/image/powder.py` & `scikit-ued-2.1.9/skued/image/powder.py`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/image/symmetry.py` & `scikit-ued-2.1.9/skued/image/symmetry.py`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/image/tests/test_alignment.py` & `scikit-ued-2.1.9/skued/image/tests/test_alignment.py`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/image/tests/test_calibration.py` & `scikit-ued-2.1.9/skued/image/tests/test_calibration.py`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/image/tests/test_center.py` & `scikit-ued-2.1.9/skued/image/tests/test_center.py`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/image/tests/test_indexing.py` & `scikit-ued-2.1.9/skued/image/tests/test_indexing.py`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/image/tests/test_metrics.py` & `scikit-ued-2.1.9/skued/image/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/image/tests/test_powder.py` & `scikit-ued-2.1.9/skued/image/tests/test_powder.py`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/image/tests/test_symmetry.py` & `scikit-ued-2.1.9/skued/image/tests/test_symmetry.py`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/io/diffshow.py` & `scikit-ued-2.1.9/skued/io/diffshow.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     WITH_PYQTGRAPH = True
 
 
 # This is weird, but PyQtGraph is an optional dependency
 # Therefore, we cannot define this class unless PyQtGraph is importable
 if WITH_PYQTGRAPH:
 
-    class Diffshow(pg.QtGui.QWidget):
+    class Diffshow(pg.QtWidgets.QWidget):
         """
         Widget containing a main viewer, plus some cursor information.
 
         Parameters
         ----------
         image : ndarray
         """
```

### Comparing `scikit-ued-2.1.8/skued/io/dm.py` & `scikit-ued-2.1.9/skued/io/dm.py`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/io/io.py` & `scikit-ued-2.1.9/skued/io/io.py`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/io/merlin.py` & `scikit-ued-2.1.9/skued/io/merlin.py`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/io/tests/data/bismuth.dm3` & `scikit-ued-2.1.9/skued/io/tests/data/bismuth.dm3`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/io/tests/data/bismuth.dm4` & `scikit-ued-2.1.9/skued/io/tests/data/bismuth.dm4`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/io/tests/data/png_test.png` & `scikit-ued-2.1.9/skued/io/tests/data/png_test.png`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/io/tests/data/test.mib` & `scikit-ued-2.1.9/skued/io/tests/data/test.mib`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/io/tests/data/test_multi.mib` & `scikit-ued-2.1.9/skued/io/tests/data/test_multi.mib`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/io/tests/test_io.py` & `scikit-ued-2.1.9/skued/io/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/patterson.py` & `scikit-ued-2.1.9/skued/patterson.py`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/plot_utils.py` & `scikit-ued-2.1.9/skued/plot_utils.py`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/potential_map.py` & `scikit-ued-2.1.9/skued/potential_map.py`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/simulation/data/aspherical.yaml` & `scikit-ued-2.1.9/skued/simulation/data/aspherical.yaml`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/simulation/form_factors.py` & `scikit-ued-2.1.9/skued/simulation/form_factors.py`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/simulation/kinematic.py` & `scikit-ued-2.1.9/skued/simulation/kinematic.py`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/simulation/potential.py` & `scikit-ued-2.1.9/skued/simulation/potential.py`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/simulation/powdersim.py` & `scikit-ued-2.1.9/skued/simulation/powdersim.py`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/simulation/scattering_params.py` & `scikit-ued-2.1.9/skued/simulation/scattering_params.py`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/simulation/structure_factors.py` & `scikit-ued-2.1.9/skued/simulation/structure_factors.py`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/simulation/tests/test_kinematic.py` & `scikit-ued-2.1.9/skued/simulation/tests/test_kinematic.py`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/simulation/tests/test_potential.py` & `scikit-ued-2.1.9/skued/simulation/tests/test_potential.py`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/simulation/tests/test_powdersim.py` & `scikit-ued-2.1.9/skued/simulation/tests/test_powdersim.py`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/simulation/tests/test_structure_factors.py` & `scikit-ued-2.1.9/skued/simulation/tests/test_structure_factors.py`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/tests/test_affine.py` & `scikit-ued-2.1.9/skued/tests/test_affine.py`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/tests/test_array_utils.py` & `scikit-ued-2.1.9/skued/tests/test_array_utils.py`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/tests/test_eproperties.py` & `scikit-ued-2.1.9/skued/tests/test_eproperties.py`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/tests/test_plot_utils.py` & `scikit-ued-2.1.9/skued/tests/test_plot_utils.py`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/tests/test_potential_map.py` & `scikit-ued-2.1.9/skued/tests/test_potential_map.py`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/tests/test_thin_films.py` & `scikit-ued-2.1.9/skued/tests/test_thin_films.py`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/tests/test_voigt.py` & `scikit-ued-2.1.9/skued/tests/test_voigt.py`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/thin_films.py` & `scikit-ued-2.1.9/skued/thin_films.py`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/time_series/__init__.py` & `scikit-ued-2.1.9/skued/time_series/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/time_series/fitting.py` & `scikit-ued-2.1.9/skued/time_series/fitting.py`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/time_series/nfft_routines.py` & `scikit-ued-2.1.9/skued/time_series/nfft_routines.py`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/time_series/robust.py` & `scikit-ued-2.1.9/skued/time_series/robust.py`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/time_series/selections.py` & `scikit-ued-2.1.9/skued/time_series/selections.py`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/time_series/tests/test_fitting.py` & `scikit-ued-2.1.9/skued/time_series/tests/test_fitting.py`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/time_series/tests/test_nfft.py` & `scikit-ued-2.1.9/skued/time_series/tests/test_nfft.py`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/time_series/tests/test_robust.py` & `scikit-ued-2.1.9/skued/time_series/tests/test_robust.py`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/time_series/tests/test_selections.py` & `scikit-ued-2.1.9/skued/time_series/tests/test_selections.py`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/time_series/tests/test_time_zero.py` & `scikit-ued-2.1.9/skued/time_series/tests/test_time_zero.py`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/time_series/time_zero.py` & `scikit-ued-2.1.9/skued/time_series/time_zero.py`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/utils.py` & `scikit-ued-2.1.9/skued/utils.py`

 * *Files identical despite different names*

### Comparing `scikit-ued-2.1.8/skued/voigt.py` & `scikit-ued-2.1.9/skued/voigt.py`

 * *Files identical despite different names*

