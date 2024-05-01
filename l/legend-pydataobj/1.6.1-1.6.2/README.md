# Comparing `tmp/legend_pydataobj-1.6.1.tar.gz` & `tmp/legend_pydataobj-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "legend_pydataobj-1.6.1.tar", last modified: Mon Apr 22 14:08:14 2024, max compression
+gzip compressed data, was "legend_pydataobj-1.6.2.tar", last modified: Wed May  1 12:28:06 2024, max compression
```

## Comparing `legend_pydataobj-1.6.1.tar` & `legend_pydataobj-1.6.2.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:08:14.968011 legend_pydataobj-1.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    44355 2024-04-22 14:08:14.968011 legend_pydataobj-1.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 14:08:14.968011 legend_pydataobj-1.6.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:08:14.948011 legend_pydataobj-1.6.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:08:14.964011 legend_pydataobj-1.6.1/src/legend_pydataobj.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    44355 2024-04-22 14:08:14.000000 legend_pydataobj-1.6.1/src/legend_pydataobj.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-04-22 14:08:14.000000 legend_pydataobj-1.6.1/src/legend_pydataobj.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 14:08:14.000000 legend_pydataobj-1.6.1/src/legend_pydataobj.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-22 14:08:14.000000 legend_pydataobj-1.6.1/src/legend_pydataobj.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 14:08:14.000000 legend_pydataobj-1.6.1/src/legend_pydataobj.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-22 14:08:14.000000 legend_pydataobj-1.6.1/src/legend_pydataobj.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-22 14:08:14.000000 legend_pydataobj-1.6.1/src/legend_pydataobj.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:08:14.952011 legend_pydataobj-1.6.1/src/lgdo/
--rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/src/lgdo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-22 14:08:14.000000 legend_pydataobj-1.6.1/src/lgdo/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     8018 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/src/lgdo/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:08:14.956011 legend_pydataobj-1.6.1/src/lgdo/compression/
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/src/lgdo/compression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/src/lgdo/compression/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/src/lgdo/compression/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)    24015 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/src/lgdo/compression/radware.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/src/lgdo/compression/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15127 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/src/lgdo/compression/varlen.py
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/src/lgdo/lgdo_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:08:14.956011 legend_pydataobj-1.6.1/src/lgdo/lh5/
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/src/lgdo/lh5/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:08:14.956011 legend_pydataobj-1.6.1/src/lgdo/lh5/_serializers/
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/src/lgdo/lh5/_serializers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:08:14.956011 legend_pydataobj-1.6.1/src/lgdo/lh5/_serializers/read/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/src/lgdo/lh5/_serializers/read/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/src/lgdo/lh5/_serializers/read/array.py
--rw-r--r--   0 runner    (1001) docker     (127)    12066 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/src/lgdo/lh5/_serializers/read/composite.py
--rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/src/lgdo/lh5/_serializers/read/encoded.py
--rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/src/lgdo/lh5/_serializers/read/ndarray.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/src/lgdo/lh5/_serializers/read/scalar.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/src/lgdo/lh5/_serializers/read/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6665 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/src/lgdo/lh5/_serializers/read/vector_of_vectors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:08:14.960011 legend_pydataobj-1.6.1/src/lgdo/lh5/_serializers/write/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/src/lgdo/lh5/_serializers/write/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/src/lgdo/lh5/_serializers/write/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     8460 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/src/lgdo/lh5/_serializers/write/composite.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/src/lgdo/lh5/_serializers/write/scalar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/src/lgdo/lh5/_serializers/write/vector_of_vectors.py
--rw-r--r--   0 runner    (1001) docker     (127)    10780 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/src/lgdo/lh5/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/src/lgdo/lh5/datatype.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/src/lgdo/lh5/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    12369 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/src/lgdo/lh5/iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6670 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/src/lgdo/lh5/store.py
--rw-r--r--   0 runner    (1001) docker     (127)     8386 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/src/lgdo/lh5/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/src/lgdo/lh5/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8483 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/src/lgdo/lh5_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/src/lgdo/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:08:14.960011 legend_pydataobj-1.6.1/src/lgdo/types/
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/src/lgdo/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6537 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/src/lgdo/types/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/src/lgdo/types/arrayofequalsizedarrays.py
--rw-r--r--   0 runner    (1001) docker     (127)    15293 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/src/lgdo/types/encoded.py
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/src/lgdo/types/fixedsizearray.py
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/src/lgdo/types/lgdo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/src/lgdo/types/scalar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/src/lgdo/types/struct.py
--rw-r--r--   0 runner    (1001) docker     (127)    17153 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/src/lgdo/types/table.py
--rw-r--r--   0 runner    (1001) docker     (127)    24503 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/src/lgdo/types/vectorofvectors.py
--rw-r--r--   0 runner    (1001) docker     (127)    10302 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/src/lgdo/types/vovutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9901 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/src/lgdo/types/waveformtable.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/src/lgdo/units.py
--rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/src/lgdo/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:08:14.960011 legend_pydataobj-1.6.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:08:14.960011 legend_pydataobj-1.6.1/tests/compression/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/tests/compression/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:08:14.964011 legend_pydataobj-1.6.1/tests/compression/sigcompress/
--rw-r--r--   0 runner    (1001) docker     (127)    23516 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/tests/compression/sigcompress/LDQTA_r117_20200110T105115Z_cal_geds_raw-0.dat
--rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/tests/compression/sigcompress/special-wf-clipped.dat
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/tests/compression/test_compression.py
--rw-r--r--   0 runner    (1001) docker     (127)    48214 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/tests/compression/test_radware_sigcompress.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/tests/compression/test_str2wfcodec.py
--rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/tests/compression/test_uleb128_zigzag_diff.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:08:14.964011 legend_pydataobj-1.6.1/tests/lh5/
--rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/tests/lh5/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/tests/lh5/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/tests/lh5/test_lh5_datatype.py
--rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/tests/lh5/test_lh5_iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)    14501 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/tests/lh5/test_lh5_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/tests/lh5/test_lh5_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/tests/lh5/test_lh5_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14032 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/tests/lh5/test_lh5_write.py
--rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/tests/test_lgdo_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:08:14.964011 legend_pydataobj-1.6.1/tests/types/
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/tests/types/test_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/tests/types/test_arrayofequalsizedarrays.py
--rw-r--r--   0 runner    (1001) docker     (127)     8134 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/tests/types/test_encoded.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/tests/types/test_fixedsizearray.py
--rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/tests/types/test_representations.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/tests/types/test_scalar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/tests/types/test_struct.py
--rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/tests/types/test_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/tests/types/test_table_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)    12028 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/tests/types/test_vectorofvectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/tests/types/test_vovutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-04-22 14:08:10.000000 legend_pydataobj-1.6.1/tests/types/test_waveformtable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:28:06.532618 legend_pydataobj-1.6.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    44355 2024-05-01 12:28:06.532618 legend_pydataobj-1.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 12:28:06.532618 legend_pydataobj-1.6.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:28:06.516618 legend_pydataobj-1.6.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:28:06.532618 legend_pydataobj-1.6.2/src/legend_pydataobj.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    44355 2024-05-01 12:28:06.000000 legend_pydataobj-1.6.2/src/legend_pydataobj.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-01 12:28:06.000000 legend_pydataobj-1.6.2/src/legend_pydataobj.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 12:28:06.000000 legend_pydataobj-1.6.2/src/legend_pydataobj.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-01 12:28:06.000000 legend_pydataobj-1.6.2/src/legend_pydataobj.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 12:28:06.000000 legend_pydataobj-1.6.2/src/legend_pydataobj.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-01 12:28:06.000000 legend_pydataobj-1.6.2/src/legend_pydataobj.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-01 12:28:06.000000 legend_pydataobj-1.6.2/src/legend_pydataobj.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:28:06.520618 legend_pydataobj-1.6.2/src/lgdo/
+-rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-01 12:28:06.000000 legend_pydataobj-1.6.2/src/lgdo/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8018 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:28:06.520618 legend_pydataobj-1.6.2/src/lgdo/compression/
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/compression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/compression/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/compression/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24015 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/compression/radware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/compression/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15127 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/compression/varlen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/lgdo_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:28:06.524618 legend_pydataobj-1.6.2/src/lgdo/lh5/
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/lh5/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:28:06.524618 legend_pydataobj-1.6.2/src/lgdo/lh5/_serializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/lh5/_serializers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:28:06.524618 legend_pydataobj-1.6.2/src/lgdo/lh5/_serializers/read/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/lh5/_serializers/read/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/lh5/_serializers/read/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12066 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/lh5/_serializers/read/composite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/lh5/_serializers/read/encoded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/lh5/_serializers/read/ndarray.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/lh5/_serializers/read/scalar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/lh5/_serializers/read/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6665 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/lh5/_serializers/read/vector_of_vectors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:28:06.524618 legend_pydataobj-1.6.2/src/lgdo/lh5/_serializers/write/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/lh5/_serializers/write/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/lh5/_serializers/write/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8460 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/lh5/_serializers/write/composite.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/lh5/_serializers/write/scalar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/lh5/_serializers/write/vector_of_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10780 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/lh5/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/lh5/datatype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/lh5/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12369 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/lh5/iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6670 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/lh5/store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8386 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/lh5/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/lh5/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8483 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/lh5_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:28:06.528618 legend_pydataobj-1.6.2/src/lgdo/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6537 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/types/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/types/arrayofequalsizedarrays.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15293 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/types/encoded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/types/fixedsizearray.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/types/lgdo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/types/scalar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/types/struct.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17153 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/types/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24503 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/types/vectorofvectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10302 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/types/vovutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9901 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/types/waveformtable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/src/lgdo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:28:06.528618 legend_pydataobj-1.6.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:28:06.528618 legend_pydataobj-1.6.2/tests/compression/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/tests/compression/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:28:06.528618 legend_pydataobj-1.6.2/tests/compression/sigcompress/
+-rw-r--r--   0 runner    (1001) docker     (127)    23516 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/tests/compression/sigcompress/LDQTA_r117_20200110T105115Z_cal_geds_raw-0.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/tests/compression/sigcompress/special-wf-clipped.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/tests/compression/test_compression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48214 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/tests/compression/test_radware_sigcompress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/tests/compression/test_str2wfcodec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/tests/compression/test_uleb128_zigzag_diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:28:06.528618 legend_pydataobj-1.6.2/tests/lh5/
+-rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/tests/lh5/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/tests/lh5/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/tests/lh5/test_lh5_datatype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/tests/lh5/test_lh5_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14711 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/tests/lh5/test_lh5_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/tests/lh5/test_lh5_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/tests/lh5/test_lh5_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14032 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/tests/lh5/test_lh5_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/tests/test_lgdo_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:28:06.532618 legend_pydataobj-1.6.2/tests/types/
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/tests/types/test_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/tests/types/test_arrayofequalsizedarrays.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8134 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/tests/types/test_encoded.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/tests/types/test_fixedsizearray.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/tests/types/test_representations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/tests/types/test_scalar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/tests/types/test_struct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/tests/types/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/tests/types/test_table_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12028 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/tests/types/test_vectorofvectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/tests/types/test_vovutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-05-01 12:28:02.000000 legend_pydataobj-1.6.2/tests/types/test_waveformtable.py
```

### Comparing `legend_pydataobj-1.6.1/LICENSE` & `legend_pydataobj-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/PKG-INFO` & `legend_pydataobj-1.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: legend_pydataobj
-Version: 1.6.1
+Version: 1.6.2
 Summary: LEGEND Python Data Objects
 Author: The LEGEND Collaboration
 Maintainer: The LEGEND Collaboration
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `legend_pydataobj-1.6.1/README.md` & `legend_pydataobj-1.6.2/README.md`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/pyproject.toml` & `legend_pydataobj-1.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/src/legend_pydataobj.egg-info/PKG-INFO` & `legend_pydataobj-1.6.2/src/legend_pydataobj.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: legend_pydataobj
-Version: 1.6.1
+Version: 1.6.2
 Summary: LEGEND Python Data Objects
 Author: The LEGEND Collaboration
 Maintainer: The LEGEND Collaboration
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `legend_pydataobj-1.6.1/src/legend_pydataobj.egg-info/SOURCES.txt` & `legend_pydataobj-1.6.2/src/legend_pydataobj.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/src/lgdo/__init__.py` & `legend_pydataobj-1.6.2/src/lgdo/__init__.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/src/lgdo/cli.py` & `legend_pydataobj-1.6.2/src/lgdo/cli.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/src/lgdo/compression/__init__.py` & `legend_pydataobj-1.6.2/src/lgdo/compression/__init__.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/src/lgdo/compression/base.py` & `legend_pydataobj-1.6.2/src/lgdo/compression/base.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/src/lgdo/compression/generic.py` & `legend_pydataobj-1.6.2/src/lgdo/compression/generic.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/src/lgdo/compression/radware.py` & `legend_pydataobj-1.6.2/src/lgdo/compression/radware.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/src/lgdo/compression/utils.py` & `legend_pydataobj-1.6.2/src/lgdo/compression/utils.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/src/lgdo/compression/varlen.py` & `legend_pydataobj-1.6.2/src/lgdo/compression/varlen.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/src/lgdo/lgdo_utils.py` & `legend_pydataobj-1.6.2/src/lgdo/lgdo_utils.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/src/lgdo/lh5/__init__.py` & `legend_pydataobj-1.6.2/src/lgdo/lh5/__init__.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/src/lgdo/lh5/_serializers/__init__.py` & `legend_pydataobj-1.6.2/src/lgdo/lh5/_serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/src/lgdo/lh5/_serializers/read/array.py` & `legend_pydataobj-1.6.2/src/lgdo/lh5/_serializers/read/array.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/src/lgdo/lh5/_serializers/read/composite.py` & `legend_pydataobj-1.6.2/src/lgdo/lh5/_serializers/read/composite.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/src/lgdo/lh5/_serializers/read/encoded.py` & `legend_pydataobj-1.6.2/src/lgdo/lh5/_serializers/read/encoded.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/src/lgdo/lh5/_serializers/read/ndarray.py` & `legend_pydataobj-1.6.2/src/lgdo/lh5/_serializers/read/ndarray.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/src/lgdo/lh5/_serializers/read/scalar.py` & `legend_pydataobj-1.6.2/src/lgdo/lh5/_serializers/read/scalar.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/src/lgdo/lh5/_serializers/read/vector_of_vectors.py` & `legend_pydataobj-1.6.2/src/lgdo/lh5/_serializers/read/vector_of_vectors.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/src/lgdo/lh5/_serializers/write/array.py` & `legend_pydataobj-1.6.2/src/lgdo/lh5/_serializers/write/array.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import numpy as np
 
 from .... import types
 from ...exceptions import LH5EncodeError
 
 log = logging.getLogger(__name__)
 
-DEFAULT_HDF5_SETTINGS: dict[str, ...] = {"shuffle": True, "compression": "gzip"}
+DEFAULT_HDF5_SETTINGS: dict[str, ...] = {"shuffle": True, "compression": "lzf"}
 
 
 def _h5_write_array(
     obj,
     name,
     lh5_file,
     group="/",
```

### Comparing `legend_pydataobj-1.6.1/src/lgdo/lh5/_serializers/write/composite.py` & `legend_pydataobj-1.6.2/src/lgdo/lh5/_serializers/write/composite.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/src/lgdo/lh5/_serializers/write/scalar.py` & `legend_pydataobj-1.6.2/src/lgdo/lh5/_serializers/write/scalar.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/src/lgdo/lh5/_serializers/write/vector_of_vectors.py` & `legend_pydataobj-1.6.2/src/lgdo/lh5/_serializers/write/vector_of_vectors.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/src/lgdo/lh5/core.py` & `legend_pydataobj-1.6.2/src/lgdo/lh5/core.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/src/lgdo/lh5/datatype.py` & `legend_pydataobj-1.6.2/src/lgdo/lh5/datatype.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,17 +12,17 @@
         (lgdo.VectorOfEncodedVectors, r"^array<1>\{encoded_array<1>\{.+\}\}$"),
         (
             lgdo.ArrayOfEncodedEqualSizedArrays,
             r"^array_of_encoded_equalsized_arrays<1,1>\{.+\}$",
         ),
         (lgdo.Struct, r"^struct\{.*\}$"),
         (lgdo.Table, r"^table\{.*\}$"),
-        (lgdo.FixedSizeArray, r"^fixedsize_array<1>\{.+\}$"),
+        (lgdo.FixedSizeArray, r"^fixedsize_array<\d+>\{.+\}$"),
         (lgdo.ArrayOfEqualSizedArrays, r"^array_of_equalsized_arrays<1,1>\{.+\}$"),
-        (lgdo.Array, r"^array<1>\{.+\}$"),
+        (lgdo.Array, r"^array<\d+>\{.+\}$"),
     ]
 )
 """Mapping between LGDO types and regular expression defining the corresponding datatype string"""
 
 
 def datatype(expr: str) -> type:
     """Return the LGDO type corresponding to a datatype string."""
```

### Comparing `legend_pydataobj-1.6.1/src/lgdo/lh5/exceptions.py` & `legend_pydataobj-1.6.2/src/lgdo/lh5/exceptions.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/src/lgdo/lh5/iterator.py` & `legend_pydataobj-1.6.2/src/lgdo/lh5/iterator.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/src/lgdo/lh5/store.py` & `legend_pydataobj-1.6.2/src/lgdo/lh5/store.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/src/lgdo/lh5/tools.py` & `legend_pydataobj-1.6.2/src/lgdo/lh5/tools.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/src/lgdo/lh5/utils.py` & `legend_pydataobj-1.6.2/src/lgdo/lh5/utils.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/src/lgdo/lh5_store.py` & `legend_pydataobj-1.6.2/src/lgdo/lh5_store.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/src/lgdo/logging.py` & `legend_pydataobj-1.6.2/src/lgdo/logging.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/src/lgdo/types/__init__.py` & `legend_pydataobj-1.6.2/src/lgdo/types/__init__.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/src/lgdo/types/array.py` & `legend_pydataobj-1.6.2/src/lgdo/types/array.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/src/lgdo/types/arrayofequalsizedarrays.py` & `legend_pydataobj-1.6.2/src/lgdo/types/arrayofequalsizedarrays.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/src/lgdo/types/encoded.py` & `legend_pydataobj-1.6.2/src/lgdo/types/encoded.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/src/lgdo/types/fixedsizearray.py` & `legend_pydataobj-1.6.2/src/lgdo/types/fixedsizearray.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/src/lgdo/types/lgdo.py` & `legend_pydataobj-1.6.2/src/lgdo/types/lgdo.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/src/lgdo/types/scalar.py` & `legend_pydataobj-1.6.2/src/lgdo/types/scalar.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/src/lgdo/types/struct.py` & `legend_pydataobj-1.6.2/src/lgdo/types/struct.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/src/lgdo/types/table.py` & `legend_pydataobj-1.6.2/src/lgdo/types/table.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/src/lgdo/types/vectorofvectors.py` & `legend_pydataobj-1.6.2/src/lgdo/types/vectorofvectors.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/src/lgdo/types/vovutils.py` & `legend_pydataobj-1.6.2/src/lgdo/types/vovutils.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/src/lgdo/types/waveformtable.py` & `legend_pydataobj-1.6.2/src/lgdo/types/waveformtable.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/src/lgdo/utils.py` & `legend_pydataobj-1.6.2/src/lgdo/utils.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/tests/compression/sigcompress/LDQTA_r117_20200110T105115Z_cal_geds_raw-0.dat` & `legend_pydataobj-1.6.2/tests/compression/sigcompress/LDQTA_r117_20200110T105115Z_cal_geds_raw-0.dat`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/tests/compression/sigcompress/special-wf-clipped.dat` & `legend_pydataobj-1.6.2/tests/compression/sigcompress/special-wf-clipped.dat`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/tests/compression/test_compression.py` & `legend_pydataobj-1.6.2/tests/compression/test_compression.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/tests/compression/test_radware_sigcompress.py` & `legend_pydataobj-1.6.2/tests/compression/test_radware_sigcompress.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/tests/compression/test_str2wfcodec.py` & `legend_pydataobj-1.6.2/tests/compression/test_str2wfcodec.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/tests/compression/test_uleb128_zigzag_diff.py` & `legend_pydataobj-1.6.2/tests/compression/test_uleb128_zigzag_diff.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/tests/conftest.py` & `legend_pydataobj-1.6.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/tests/lh5/conftest.py` & `legend_pydataobj-1.6.2/tests/lh5/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 @pytest.fixture(scope="module")
 def lh5_file(tmptestdir):
     store = lh5.LH5Store()
 
     struct = lgdo.Struct()
     struct.add_field("scalar", lgdo.Scalar(value=10, attrs={"sth": 1}))
     struct.add_field("array", types.Array(nda=np.array([1, 2, 3, 4, 5])))
+    struct.add_field("array2d", types.Array(shape=(23, 56), fill_val=69, dtype=int))
     struct.add_field(
         "aoesa",
         types.ArrayOfEqualSizedArrays(shape=(5, 5), dtype=np.float32, fill_val=42),
     )
     struct.add_field(
         "vov",
         types.VectorOfVectors(
```

### Comparing `legend_pydataobj-1.6.1/tests/lh5/test_core.py` & `legend_pydataobj-1.6.2/tests/lh5/test_core.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/tests/lh5/test_lh5_datatype.py` & `legend_pydataobj-1.6.2/tests/lh5/test_lh5_datatype.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/tests/lh5/test_lh5_iterator.py` & `legend_pydataobj-1.6.2/tests/lh5/test_lh5_iterator.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/tests/lh5/test_lh5_store.py` & `legend_pydataobj-1.6.2/tests/lh5/test_lh5_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,14 +80,18 @@
     assert n_rows == 3
     with h5py.File(lh5_file) as h5f:
         assert (
             h5f["/data/struct/array"].compression
             is DEFAULT_HDF5_SETTINGS["compression"]
         )
 
+    lh5_obj, n_rows = store.read("/data/struct_full/array2d", lh5_file)
+    assert isinstance(lh5_obj, types.Array)
+    assert lh5_obj == types.Array(shape=(23, 56), fill_val=69, dtype=int)
+
 
 def test_read_array_slice(lh5_file):
     store = lh5.LH5Store()
     lh5_obj, n_rows = store.read(
         "/data/struct_full/array", lh5_file, start_row=1, n_rows=3
     )
     assert isinstance(lh5_obj, types.Array)
@@ -347,14 +351,15 @@
 
     lh5_obj, n_rows = store.read(
         "/data/struct_full", lh5_file, field_mask={"vov": False, "voev": False}
     )
     assert sorted(lh5_obj.keys()) == [
         "aoesa",
         "array",
+        "array2d",
         "empty_struct",
         "scalar",
         "table",
         "vov3d",
         "wftable",
         "wftable_enc",
     ]
```

### Comparing `legend_pydataobj-1.6.1/tests/lh5/test_lh5_tools.py` & `legend_pydataobj-1.6.2/tests/lh5/test_lh5_tools.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/tests/lh5/test_lh5_utils.py` & `legend_pydataobj-1.6.2/tests/lh5/test_lh5_utils.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/tests/lh5/test_lh5_write.py` & `legend_pydataobj-1.6.2/tests/lh5/test_lh5_write.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/tests/test_cli.py` & `legend_pydataobj-1.6.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/tests/types/test_array.py` & `legend_pydataobj-1.6.2/tests/types/test_array.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/tests/types/test_arrayofequalsizedarrays.py` & `legend_pydataobj-1.6.2/tests/types/test_arrayofequalsizedarrays.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/tests/types/test_encoded.py` & `legend_pydataobj-1.6.2/tests/types/test_encoded.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/tests/types/test_fixedsizearray.py` & `legend_pydataobj-1.6.2/tests/types/test_fixedsizearray.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/tests/types/test_representations.py` & `legend_pydataobj-1.6.2/tests/types/test_representations.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/tests/types/test_scalar.py` & `legend_pydataobj-1.6.2/tests/types/test_scalar.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/tests/types/test_struct.py` & `legend_pydataobj-1.6.2/tests/types/test_struct.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/tests/types/test_table.py` & `legend_pydataobj-1.6.2/tests/types/test_table.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/tests/types/test_table_eval.py` & `legend_pydataobj-1.6.2/tests/types/test_table_eval.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/tests/types/test_vectorofvectors.py` & `legend_pydataobj-1.6.2/tests/types/test_vectorofvectors.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/tests/types/test_vovutils.py` & `legend_pydataobj-1.6.2/tests/types/test_vovutils.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.6.1/tests/types/test_waveformtable.py` & `legend_pydataobj-1.6.2/tests/types/test_waveformtable.py`

 * *Files identical despite different names*

