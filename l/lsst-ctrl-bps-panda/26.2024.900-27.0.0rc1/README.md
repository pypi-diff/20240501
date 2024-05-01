# Comparing `tmp/lsst-ctrl-bps-panda-26.2024.900.tar.gz` & `tmp/lsst_ctrl_bps_panda-27.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsst-ctrl-bps-panda-26.2024.900.tar", last modified: Thu Feb 29 10:20:28 2024, max compression
+gzip compressed data, was "lsst_ctrl_bps_panda-27.0.0rc1.tar", last modified: Wed May  1 21:16:39 2024, max compression
```

## Comparing `lsst-ctrl-bps-panda-26.2024.900.tar` & `lsst_ctrl_bps_panda-27.0.0rc1.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:28.417526 lsst-ctrl-bps-panda-26.2024.900/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-02-29 10:20:19.000000 lsst-ctrl-bps-panda-26.2024.900/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-02-29 10:20:19.000000 lsst-ctrl-bps-panda-26.2024.900/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-02-29 10:20:28.417526 lsst-ctrl-bps-panda-26.2024.900/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-02-29 10:20:19.000000 lsst-ctrl-bps-panda-26.2024.900/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-02-29 10:20:19.000000 lsst-ctrl-bps-panda-26.2024.900/bsd_license.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-29 10:20:19.000000 lsst-ctrl-bps-panda-26.2024.900/gpl-v3.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-02-29 10:20:19.000000 lsst-ctrl-bps-panda-26.2024.900/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:28.409526 lsst-ctrl-bps-panda-26.2024.900/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:28.409526 lsst-ctrl-bps-panda-26.2024.900/python/lsst/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:28.409526 lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:28.409526 lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:28.413526 lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-02-29 10:20:19.000000 lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:28.413526 lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:19.000000 lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:28.413526 lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/cli/cmd/
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-02-29 10:20:19.000000 lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/cli/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-02-29 10:20:19.000000 lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/cli/cmd/panda_auth_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-02-29 10:20:19.000000 lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/cli/panda_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-02-29 10:20:19.000000 lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/cmd_line_embedder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:28.413526 lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/conf_example/
--rw-r--r--   0 runner    (1001) docker     (127)     5855 2024-02-29 10:20:19.000000 lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/conf_example/example_panda_SLAC.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-02-29 10:20:19.000000 lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/conf_example/pipelines_check_idf.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-02-29 10:20:19.000000 lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/conf_example/test_idf.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-02-29 10:20:19.000000 lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/conf_example/test_sdf.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-02-29 10:20:19.000000 lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/conf_example/test_usdf.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-02-29 10:20:19.000000 lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:28.413526 lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/edgenode/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:19.000000 lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/edgenode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6052 2024-02-29 10:20:19.000000 lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/edgenode/cmd_line_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-02-29 10:20:19.000000 lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/panda_auth_drivers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-02-29 10:20:19.000000 lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/panda_auth_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15176 2024-02-29 10:20:19.000000 lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/panda_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    23468 2024-02-29 10:20:19.000000 lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-29 10:20:28.000000 lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:28.417526 lsst-ctrl-bps-panda-26.2024.900/python/lsst_ctrl_bps_panda.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-02-29 10:20:28.000000 lsst-ctrl-bps-panda-26.2024.900/python/lsst_ctrl_bps_panda.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-02-29 10:20:28.000000 lsst-ctrl-bps-panda-26.2024.900/python/lsst_ctrl_bps_panda.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 10:20:28.000000 lsst-ctrl-bps-panda-26.2024.900/python/lsst_ctrl_bps_panda.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-02-29 10:20:28.000000 lsst-ctrl-bps-panda-26.2024.900/python/lsst_ctrl_bps_panda.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-29 10:20:28.000000 lsst-ctrl-bps-panda-26.2024.900/python/lsst_ctrl_bps_panda.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 10:20:28.000000 lsst-ctrl-bps-panda-26.2024.900/python/lsst_ctrl_bps_panda.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-02-29 10:20:28.417526 lsst-ctrl-bps-panda-26.2024.900/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:28.413526 lsst-ctrl-bps-panda-26.2024.900/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-02-29 10:20:19.000000 lsst-ctrl-bps-panda-26.2024.900/tests/test_cmd_line_embedder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-02-29 10:20:19.000000 lsst-ctrl-bps-panda-26.2024.900/tests/test_panda_auth_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-02-29 10:20:19.000000 lsst-ctrl-bps-panda-26.2024.900/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:39.604740 lsst_ctrl_bps_panda-27.0.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-01 21:16:33.000000 lsst_ctrl_bps_panda-27.0.0rc1/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-01 21:16:33.000000 lsst_ctrl_bps_panda-27.0.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-01 21:16:39.604740 lsst_ctrl_bps_panda-27.0.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-01 21:16:33.000000 lsst_ctrl_bps_panda-27.0.0rc1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-01 21:16:33.000000 lsst_ctrl_bps_panda-27.0.0rc1/bsd_license.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-01 21:16:33.000000 lsst_ctrl_bps_panda-27.0.0rc1/gpl-v3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-05-01 21:16:33.000000 lsst_ctrl_bps_panda-27.0.0rc1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:39.596740 lsst_ctrl_bps_panda-27.0.0rc1/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:39.596740 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:39.596740 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:39.596740 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:39.600740 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-01 21:16:33.000000 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:39.600740 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:33.000000 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:39.600740 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/cli/cmd/
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-01 21:16:33.000000 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/cli/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-05-01 21:16:33.000000 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/cli/cmd/panda_auth_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-05-01 21:16:33.000000 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/cli/panda_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-05-01 21:16:33.000000 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/cmd_line_embedder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:39.600740 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/conf_example/
+-rw-r--r--   0 runner    (1001) docker     (127)     5855 2024-05-01 21:16:33.000000 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/conf_example/example_panda_SLAC.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-01 21:16:33.000000 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/conf_example/pipelines_check_idf.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-01 21:16:33.000000 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/conf_example/test_idf.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-01 21:16:33.000000 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/conf_example/test_sdf.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-01 21:16:33.000000 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/conf_example/test_usdf.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-01 21:16:33.000000 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:39.600740 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/edgenode/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:33.000000 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/edgenode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5139 2024-05-01 21:16:33.000000 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/edgenode/build_cmd_line_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6052 2024-05-01 21:16:33.000000 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/edgenode/cmd_line_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-05-01 21:16:33.000000 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/panda_auth_drivers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-05-01 21:16:33.000000 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/panda_auth_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16267 2024-05-01 21:16:33.000000 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/panda_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28165 2024-05-01 21:16:33.000000 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-01 21:16:39.000000 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:39.604740 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst_ctrl_bps_panda.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-01 21:16:39.000000 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst_ctrl_bps_panda.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-01 21:16:39.000000 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst_ctrl_bps_panda.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 21:16:39.000000 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst_ctrl_bps_panda.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-01 21:16:39.000000 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst_ctrl_bps_panda.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-01 21:16:39.000000 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst_ctrl_bps_panda.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 21:16:39.000000 lsst_ctrl_bps_panda-27.0.0rc1/python/lsst_ctrl_bps_panda.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-01 21:16:39.604740 lsst_ctrl_bps_panda-27.0.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:39.604740 lsst_ctrl_bps_panda-27.0.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-05-01 21:16:33.000000 lsst_ctrl_bps_panda-27.0.0rc1/tests/test_cmd_line_embedder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-05-01 21:16:33.000000 lsst_ctrl_bps_panda-27.0.0rc1/tests/test_panda_auth_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-05-01 21:16:33.000000 lsst_ctrl_bps_panda-27.0.0rc1/tests/test_utils.py
```

### Comparing `lsst-ctrl-bps-panda-26.2024.900/PKG-INFO` & `lsst_ctrl_bps_panda-27.0.0rc1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-ctrl-bps-panda
-Version: 26.2024.900
+Version: 27.0.0rc1
 Summary: PanDA plugin for lsst-ctrl-bps.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/lsst/ctrl_bps_panda
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst-ctrl-bps-panda-26.2024.900/README.rst` & `lsst_ctrl_bps_panda-27.0.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-panda-26.2024.900/bsd_license.txt` & `lsst_ctrl_bps_panda-27.0.0rc1/bsd_license.txt`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-panda-26.2024.900/gpl-v3.0.txt` & `lsst_ctrl_bps_panda-27.0.0rc1/gpl-v3.0.txt`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-panda-26.2024.900/pyproject.toml` & `lsst_ctrl_bps_panda-27.0.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/__init__.py` & `lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/cli/cmd/__init__.py` & `lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/cli/cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/cli/cmd/panda_auth_commands.py` & `lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/cli/cmd/panda_auth_commands.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/cli/panda_auth.py` & `lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/cli/panda_auth.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/cmd_line_embedder.py` & `lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/cmd_line_embedder.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/conf_example/example_panda_SLAC.yaml` & `lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/conf_example/example_panda_SLAC.yaml`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/conf_example/pipelines_check_idf.yaml` & `lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/conf_example/pipelines_check_idf.yaml`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/constants.py` & `lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/constants.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/edgenode/cmd_line_decoder.py` & `lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/edgenode/cmd_line_decoder.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/panda_auth_drivers.py` & `lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/panda_auth_drivers.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/panda_auth_utils.py` & `lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/panda_auth_utils.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/panda_service.py` & `lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/panda_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 from idds.workflowv2.workflow import Workflow as IDDS_client_workflow
 from lsst.ctrl.bps import BaseWmsService, BaseWmsWorkflow, WmsRunReport, WmsStates
 from lsst.ctrl.bps.panda.constants import PANDA_DEFAULT_MAX_COPY_WORKERS
 from lsst.ctrl.bps.panda.utils import (
     add_final_idds_work,
     add_idds_work,
     copy_files_for_distribution,
+    create_idds_build_workflow,
     get_idds_client,
     get_idds_result,
 )
 
 _LOG = logging.getLogger(__name__)
 
 
@@ -59,39 +60,60 @@
         _LOG.debug("out_prefix = '%s'", out_prefix)
         workflow = PandaBpsWmsWorkflow.from_generic_workflow(
             config, generic_workflow, out_prefix, f"{self.__class__.__module__}.{self.__class__.__name__}"
         )
         workflow.write(out_prefix)
         return workflow
 
-    def submit(self, workflow):
-        _, max_copy_workers = self.config.search(
-            "maxCopyWorkers", opt={"default": PANDA_DEFAULT_MAX_COPY_WORKERS}
-        )
-        # Docstring inherited from BaseWmsService.submit.
-        file_distribution_uri = self.config["fileDistributionEndPoint"]
-        lsst_temp = "LSST_RUN_TEMP_SPACE"
-        if lsst_temp in file_distribution_uri and lsst_temp not in os.environ:
-            file_distribution_uri = self.config["fileDistributionEndPointDefault"]
-
-        copy_files_for_distribution(workflow.files_to_pre_stage, file_distribution_uri, max_copy_workers)
-
-        idds_client = get_idds_client(self.config)
-        ret = idds_client.submit(workflow.idds_client_workflow, username=None, use_dataset_name=False)
-        _LOG.debug("iDDS client manager submit returned = %s", ret)
-
-        # Check submission success
-        status, result, error = get_idds_result(ret)
-        if status:
-            request_id = int(result)
+    def submit(self, workflow, **kwargs):
+        config = kwargs["config"] if "config" in kwargs else None
+        remote_build = kwargs["remote_build"] if "remote_build" in kwargs else None
+
+        if config and remote_build:
+            _LOG.info("remote build")
+
+            idds_build_workflow = create_idds_build_workflow(**kwargs)
+            idds_client = get_idds_client(self.config)
+            ret = idds_client.submit_build(idds_build_workflow, username=None, use_dataset_name=False)
+            _LOG.debug("iDDS client manager submit returned = %s", ret)
+
+            # Check submission success
+            status, result, error = get_idds_result(ret)
+            if status:
+                request_id = int(result)
+            else:
+                raise RuntimeError(f"Error submitting to PanDA service: {error}")
+
+            _LOG.info("Submitted into iDDs with request id=%s", request_id)
+            idds_build_workflow.run_id = request_id
+            return idds_build_workflow
         else:
-            raise RuntimeError(f"Error submitting to PanDA service: {error}")
+            _, max_copy_workers = self.config.search(
+                "maxCopyWorkers", opt={"default": PANDA_DEFAULT_MAX_COPY_WORKERS}
+            )
+            # Docstring inherited from BaseWmsService.submit.
+            file_distribution_uri = self.config["fileDistributionEndPoint"]
+            lsst_temp = "LSST_RUN_TEMP_SPACE"
+            if lsst_temp in file_distribution_uri and lsst_temp not in os.environ:
+                file_distribution_uri = self.config["fileDistributionEndPointDefault"]
+            copy_files_for_distribution(workflow.files_to_pre_stage, file_distribution_uri, max_copy_workers)
+
+            idds_client = get_idds_client(self.config)
+            ret = idds_client.submit(workflow.idds_client_workflow, username=None, use_dataset_name=False)
+            _LOG.debug("iDDS client manager submit returned = %s", ret)
+
+            # Check submission success
+            status, result, error = get_idds_result(ret)
+            if status:
+                request_id = int(result)
+            else:
+                raise RuntimeError(f"Error submitting to PanDA service: {error}")
 
-        _LOG.info("Submitted into iDDs with request id=%s", request_id)
-        workflow.run_id = request_id
+            _LOG.info("Submitted into iDDs with request id=%s", request_id)
+            workflow.run_id = request_id
 
     def restart(self, wms_workflow_id):
         # Docstring inherited from BaseWmsService.restart.
         idds_client = get_idds_client(self.config)
         ret = idds_client.retry(request_id=wms_workflow_id)
         _LOG.debug("Restart PanDA workflow returned = %s", ret)
```

### Comparing `lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/utils.py` & `lsst_ctrl_bps_panda-27.0.0rc1/python/lsst/ctrl/bps/panda/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -35,19 +35,22 @@
     "add_decoder_prefix",
 ]
 
 import binascii
 import concurrent.futures
 import logging
 import os
+import tarfile
+import uuid
 
 import idds.common.utils as idds_utils
 import pandaclient.idds_api
 from idds.doma.workflowv2.domapandawork import DomaPanDAWork
 from idds.workflowv2.workflow import AndCondition
+from idds.workflowv2.workflow import Workflow as IDDS_client_workflow
 from lsst.ctrl.bps import BpsConfig, GenericWorkflow, GenericWorkflowJob
 from lsst.ctrl.bps.panda.cmd_line_embedder import CommandLineEmbedder
 from lsst.ctrl.bps.panda.constants import (
     PANDA_DEFAULT_CLOUD,
     PANDA_DEFAULT_CORE_COUNT,
     PANDA_DEFAULT_MAX_ATTEMPTS,
     PANDA_DEFAULT_MAX_JOBS_PER_TASK,
@@ -599,7 +602,116 @@
                     }
                 )
             pseudo_filename = job_to_pseudo_filename[job_name]
             work.dependency_map.append({"name": pseudo_filename, "dependencies": deps})
         _LOG.info("Successfully recovered.")
 
     return files_to_pre_stage, dag_sink_work, task_count
+
+
+def create_archive_file(submit_path, archive_filename, files):
+    if not archive_filename.startswith("/"):
+        archive_filename = os.path.join(submit_path, archive_filename)
+
+    with tarfile.open(archive_filename, "w:gz", dereference=True) as tar:
+        for local_file in files:
+            base_name = os.path.basename(local_file)
+            tar.add(local_file, arcname=os.path.basename(base_name))
+    return archive_filename
+
+
+def copy_files_to_pandacache(filename):
+    from pandaclient import Client
+
+    attempt = 0
+    max_attempts = 3
+    done = False
+    while attempt < max_attempts and not done:
+        status, out = Client.putFile(filename, True)
+        if status == 0:
+            done = True
+    print(f"copy_files_to_pandacache: status: {status}, out: {out}")
+    if out.startswith("NewFileName:"):
+        # found the same input sandbox to reuse
+        filename = out.split(":")[-1]
+    elif out != "True":
+        print(out)
+        return None
+
+    filename = os.path.basename(filename)
+    cache_path = os.path.join(os.environ["PANDACACHE_URL"], "cache")
+    filename = os.path.join(cache_path, filename)
+    return filename
+
+
+def get_task_parameter(config, remote_build, key):
+    search_opt = {"replaceVars": True, "expandEnvVars": False, "replaceEnvVars": False, "required": False}
+    _, value = remote_build.search(key, search_opt)
+    if not value:
+        _, value = config.search(key, search_opt)
+    return value
+
+
+def create_idds_build_workflow(**kwargs):
+    config = kwargs["config"] if "config" in kwargs else None
+    remote_build = kwargs["remote_build"] if "remote_build" in kwargs else None
+    config_file = kwargs["config_file"] if "config_file" in kwargs else None
+    config_file_base = os.path.basename(config_file) if config_file else None
+    compute_site = kwargs["compute_site"] if "compute_site" in kwargs else None
+    _, files = remote_build.search("files", opt={"default": []})
+    submit_path = config["submitPath"]
+    files.append(config_file)
+    archive_filename = "jobO.%s.tar.gz" % str(uuid.uuid4())
+    archive_filename = create_archive_file(submit_path, archive_filename, files)
+    _LOG.info("archive file name: %s" % archive_filename)
+    remote_filename = copy_files_to_pandacache(archive_filename)
+    _LOG.info("pandacache file: %s" % remote_filename)
+
+    _LOG.info(type(remote_build))
+    search_opt = {"replaceVars": True, "expandEnvVars": False, "replaceEnvVars": False, "required": False}
+    cvals = {"LSST_VERSION": get_task_parameter(config, remote_build, "LSST_VERSION")}
+    cvals["custom_lsst_setup"] = get_task_parameter(config, remote_build, "custom_lsst_setup")
+    search_opt["curvals"] = cvals
+    _, executable = remote_build.search("runnerCommand", opt=search_opt)
+    executable = executable.replace("_download_cmd_line_", remote_filename)
+    executable = executable.replace("_build_cmd_line_", config_file_base)
+    executable = executable.replace("_compute_site_", compute_site or "")
+
+    task_cloud = get_task_parameter(config, remote_build, "computeCloud")
+    task_site = get_task_parameter(config, remote_build, "computeSite")
+    task_queue = get_task_parameter(config, remote_build, "queue")
+    task_rss = get_task_parameter(config, remote_build, "requestMemory")
+    nretries = get_task_parameter(config, remote_build, "numberOfRetries")
+    _LOG.info("requestMemory: %s", task_rss)
+    _LOG.info("Site: %s", task_site)
+    # _LOG.info("executable: %s", executable)
+    # TODO: fill other parameters based on config
+    build_work = DomaPanDAWork(
+        executable=executable,
+        task_type="lsst_build",
+        primary_input_collection={"scope": "pseudo_dataset", "name": "pseudo_input_collection#1"},
+        output_collections=[{"scope": "pseudo_dataset", "name": "pseudo_output_collection#1"}],
+        log_collections=[],
+        dependency_map=None,
+        task_name="build_task",
+        task_queue=task_queue,
+        encode_command_line=True,
+        prodSourceLabel="managed",
+        task_log={
+            "dataset": "PandaJob_#{pandaid}/",
+            "destination": "local",
+            "param_type": "log",
+            "token": "local",
+            "type": "template",
+            "value": "log.tgz",
+        },
+        task_rss=task_rss if task_rss else PANDA_DEFAULT_RSS,
+        task_cloud=task_cloud,
+        task_site=task_site,
+        maxattempt=nretries if nretries > 0 else PANDA_DEFAULT_MAX_ATTEMPTS,
+    )
+
+    workflow = IDDS_client_workflow()
+
+    workflow.add_work(build_work)
+    workflow.name = config["bps_defined"]["uniqProcName"]
+    return workflow
```

### Comparing `lsst-ctrl-bps-panda-26.2024.900/python/lsst_ctrl_bps_panda.egg-info/PKG-INFO` & `lsst_ctrl_bps_panda-27.0.0rc1/python/lsst_ctrl_bps_panda.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-ctrl-bps-panda
-Version: 26.2024.900
+Version: 27.0.0rc1
 Summary: PanDA plugin for lsst-ctrl-bps.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/lsst/ctrl_bps_panda
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst-ctrl-bps-panda-26.2024.900/python/lsst_ctrl_bps_panda.egg-info/SOURCES.txt` & `lsst_ctrl_bps_panda-27.0.0rc1/python/lsst_ctrl_bps_panda.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 python/lsst/ctrl/bps/panda/cli/cmd/panda_auth_commands.py
 python/lsst/ctrl/bps/panda/conf_example/example_panda_SLAC.yaml
 python/lsst/ctrl/bps/panda/conf_example/pipelines_check_idf.yaml
 python/lsst/ctrl/bps/panda/conf_example/test_idf.yaml
 python/lsst/ctrl/bps/panda/conf_example/test_sdf.yaml
 python/lsst/ctrl/bps/panda/conf_example/test_usdf.yaml
 python/lsst/ctrl/bps/panda/edgenode/__init__.py
+python/lsst/ctrl/bps/panda/edgenode/build_cmd_line_decoder.py
 python/lsst/ctrl/bps/panda/edgenode/cmd_line_decoder.py
 python/lsst_ctrl_bps_panda.egg-info/PKG-INFO
 python/lsst_ctrl_bps_panda.egg-info/SOURCES.txt
 python/lsst_ctrl_bps_panda.egg-info/dependency_links.txt
 python/lsst_ctrl_bps_panda.egg-info/requires.txt
 python/lsst_ctrl_bps_panda.egg-info/top_level.txt
 python/lsst_ctrl_bps_panda.egg-info/zip-safe
```

### Comparing `lsst-ctrl-bps-panda-26.2024.900/tests/test_cmd_line_embedder.py` & `lsst_ctrl_bps_panda-27.0.0rc1/tests/test_cmd_line_embedder.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-panda-26.2024.900/tests/test_panda_auth_utils.py` & `lsst_ctrl_bps_panda-27.0.0rc1/tests/test_panda_auth_utils.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-panda-26.2024.900/tests/test_utils.py` & `lsst_ctrl_bps_panda-27.0.0rc1/tests/test_utils.py`

 * *Files identical despite different names*

