# Comparing `tmp/daxa-0.0.4.tar.gz` & `tmp/daxa-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daxa-0.0.4.tar", last modified: Thu Apr 25 22:15:24 2024, max compression
+gzip compressed data, was "daxa-0.0.5.tar", last modified: Wed May  1 14:36:30 2024, max compression
```

## Comparing `daxa-0.0.4.tar` & `daxa-0.0.5.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:15:24.632090 daxa-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-25 22:15:20.000000 daxa-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-25 22:15:20.000000 daxa-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5499 2024-04-25 22:15:24.632090 daxa-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-04-25 22:15:20.000000 daxa-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:15:24.620090 daxa-0.0.4/daxa/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-25 22:15:20.000000 daxa-0.0.4/daxa/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:15:24.620090 daxa-0.0.4/daxa/archive/
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-25 22:15:20.000000 daxa-0.0.4/daxa/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-25 22:15:20.000000 daxa-0.0.4/daxa/archive/assemble.py
--rw-r--r--   0 runner    (1001) docker     (127)   117934 2024-04-25 22:15:20.000000 daxa-0.0.4/daxa/archive/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4411 2024-04-25 22:15:20.000000 daxa-0.0.4/daxa/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    12477 2024-04-25 22:15:20.000000 daxa-0.0.4/daxa/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:15:24.624090 daxa-0.0.4/daxa/files/
--rw-r--r--   0 runner    (1001) docker     (127)    19204 2024-04-25 22:15:20.000000 daxa-0.0.4/daxa/files/browse_extract.pl
--rw-r--r--   0 runner    (1001) docker     (127)   128218 2024-04-25 22:15:20.000000 daxa-0.0.4/daxa/files/daxa-high-resolution-color-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)   147370 2024-04-25 22:15:20.000000 daxa-0.0.4/daxa/files/daxa-high-resolution-logo-black-on-transparent-background.png
--rw-r--r--   0 runner    (1001) docker     (127)   108001 2024-04-25 22:15:20.000000 daxa-0.0.4/daxa/files/daxa-high-resolution-logo-black-on-white-background.png
--rw-r--r--   0 runner    (1001) docker     (127)   558372 2024-04-25 22:15:20.000000 daxa-0.0.4/daxa/files/erass_de_dr1_info.csv
--rw-r--r--   0 runner    (1001) docker     (127)    35542 2024-04-25 22:15:20.000000 daxa-0.0.4/daxa/files/erosita_calpv_info.csv
--rw-r--r--   0 runner    (1001) docker     (127)    21704 2024-04-25 22:15:20.000000 daxa-0.0.4/daxa/files/sas_errors.csv
--rw-r--r--   0 runner    (1001) docker     (127)    15345 2024-04-25 22:15:20.000000 daxa-0.0.4/daxa/files/sas_warnings.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-25 22:15:20.000000 daxa-0.0.4/daxa/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:15:24.628090 daxa-0.0.4/daxa/mission/
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-25 22:15:20.000000 daxa-0.0.4/daxa/mission/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36759 2024-04-25 22:15:20.000000 daxa-0.0.4/daxa/mission/asca.py
--rw-r--r--   0 runner    (1001) docker     (127)   145563 2024-04-25 22:15:20.000000 daxa-0.0.4/daxa/mission/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    40513 2024-04-25 22:15:20.000000 daxa-0.0.4/daxa/mission/chandra.py
--rw-r--r--   0 runner    (1001) docker     (127)    91659 2024-04-25 22:15:20.000000 daxa-0.0.4/daxa/mission/erosita.py
--rw-r--r--   0 runner    (1001) docker     (127)    40077 2024-04-25 22:15:20.000000 daxa-0.0.4/daxa/mission/integral.py
--rw-r--r--   0 runner    (1001) docker     (127)    34928 2024-04-25 22:15:20.000000 daxa-0.0.4/daxa/mission/nustar.py
--rw-r--r--   0 runner    (1001) docker     (127)    64315 2024-04-25 22:15:20.000000 daxa-0.0.4/daxa/mission/rosat.py
--rw-r--r--   0 runner    (1001) docker     (127)    33896 2024-04-25 22:15:20.000000 daxa-0.0.4/daxa/mission/suzaku.py
--rw-r--r--   0 runner    (1001) docker     (127)    37595 2024-04-25 22:15:20.000000 daxa-0.0.4/daxa/mission/swift.py
--rw-r--r--   0 runner    (1001) docker     (127)    30621 2024-04-25 22:15:20.000000 daxa-0.0.4/daxa/mission/xmm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:15:24.628090 daxa-0.0.4/daxa/process/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-25 22:15:20.000000 daxa-0.0.4/daxa/process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6576 2024-04-25 22:15:20.000000 daxa-0.0.4/daxa/process/_backend_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     6214 2024-04-25 22:15:20.000000 daxa-0.0.4/daxa/process/_cleanup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:15:24.632090 daxa-0.0.4/daxa/process/erosita/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-25 22:15:20.000000 daxa-0.0.4/daxa/process/erosita/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19365 2024-04-25 22:15:20.000000 daxa-0.0.4/daxa/process/erosita/_common.py
--rw-r--r--   0 runner    (1001) docker     (127)    13072 2024-04-25 22:15:20.000000 daxa-0.0.4/daxa/process/erosita/assemble.py
--rw-r--r--   0 runner    (1001) docker     (127)    19531 2024-04-25 22:15:20.000000 daxa-0.0.4/daxa/process/erosita/clean.py
--rw-r--r--   0 runner    (1001) docker     (127)     5998 2024-04-25 22:15:20.000000 daxa-0.0.4/daxa/process/erosita/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:15:24.632090 daxa-0.0.4/daxa/process/general/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-25 22:15:20.000000 daxa-0.0.4/daxa/process/general/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20667 2024-04-25 22:15:20.000000 daxa-0.0.4/daxa/process/general/preprocessed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-04-25 22:15:20.000000 daxa-0.0.4/daxa/process/general/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     8394 2024-04-25 22:15:20.000000 daxa-0.0.4/daxa/process/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:15:24.632090 daxa-0.0.4/daxa/process/xmm/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-25 22:15:20.000000 daxa-0.0.4/daxa/process/xmm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22497 2024-04-25 22:15:20.000000 daxa-0.0.4/daxa/process/xmm/_common.py
--rw-r--r--   0 runner    (1001) docker     (127)    80965 2024-04-25 22:15:20.000000 daxa-0.0.4/daxa/process/xmm/assemble.py
--rw-r--r--   0 runner    (1001) docker     (127)    10859 2024-04-25 22:15:20.000000 daxa-0.0.4/daxa/process/xmm/check.py
--rw-r--r--   0 runner    (1001) docker     (127)    24297 2024-04-25 22:15:20.000000 daxa-0.0.4/daxa/process/xmm/clean.py
--rw-r--r--   0 runner    (1001) docker     (127)    16510 2024-04-25 22:15:20.000000 daxa-0.0.4/daxa/process/xmm/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)    24888 2024-04-25 22:15:20.000000 daxa-0.0.4/daxa/process/xmm/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:15:24.632090 daxa-0.0.4/daxa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5499 2024-04-25 22:15:24.000000 daxa-0.0.4/daxa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-25 22:15:24.000000 daxa-0.0.4/daxa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 22:15:24.000000 daxa-0.0.4/daxa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-25 22:15:24.000000 daxa-0.0.4/daxa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-25 22:15:24.000000 daxa-0.0.4/daxa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 22:15:24.632090 daxa-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-25 22:15:22.000000 daxa-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:36:30.986342 daxa-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-01 14:36:24.000000 daxa-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-01 14:36:24.000000 daxa-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6347 2024-05-01 14:36:30.986342 daxa-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5613 2024-05-01 14:36:24.000000 daxa-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:36:30.974342 daxa-0.0.5/daxa/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-01 14:36:24.000000 daxa-0.0.5/daxa/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:36:30.974342 daxa-0.0.5/daxa/archive/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-01 14:36:24.000000 daxa-0.0.5/daxa/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-01 14:36:24.000000 daxa-0.0.5/daxa/archive/assemble.py
+-rw-r--r--   0 runner    (1001) docker     (127)   117934 2024-05-01 14:36:24.000000 daxa-0.0.5/daxa/archive/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4411 2024-05-01 14:36:24.000000 daxa-0.0.5/daxa/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12477 2024-05-01 14:36:24.000000 daxa-0.0.5/daxa/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:36:30.978342 daxa-0.0.5/daxa/files/
+-rw-r--r--   0 runner    (1001) docker     (127)    19204 2024-05-01 14:36:24.000000 daxa-0.0.5/daxa/files/browse_extract.pl
+-rw-r--r--   0 runner    (1001) docker     (127)   128218 2024-05-01 14:36:24.000000 daxa-0.0.5/daxa/files/daxa-high-resolution-color-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)   147370 2024-05-01 14:36:24.000000 daxa-0.0.5/daxa/files/daxa-high-resolution-logo-black-on-transparent-background.png
+-rw-r--r--   0 runner    (1001) docker     (127)   108001 2024-05-01 14:36:24.000000 daxa-0.0.5/daxa/files/daxa-high-resolution-logo-black-on-white-background.png
+-rw-r--r--   0 runner    (1001) docker     (127)   558372 2024-05-01 14:36:24.000000 daxa-0.0.5/daxa/files/erass_de_dr1_info.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    35542 2024-05-01 14:36:24.000000 daxa-0.0.5/daxa/files/erosita_calpv_info.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    21704 2024-05-01 14:36:24.000000 daxa-0.0.5/daxa/files/sas_errors.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    15345 2024-05-01 14:36:24.000000 daxa-0.0.5/daxa/files/sas_warnings.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-01 14:36:24.000000 daxa-0.0.5/daxa/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:36:30.982342 daxa-0.0.5/daxa/mission/
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-01 14:36:24.000000 daxa-0.0.5/daxa/mission/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36759 2024-05-01 14:36:24.000000 daxa-0.0.5/daxa/mission/asca.py
+-rw-r--r--   0 runner    (1001) docker     (127)   145563 2024-05-01 14:36:24.000000 daxa-0.0.5/daxa/mission/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40513 2024-05-01 14:36:24.000000 daxa-0.0.5/daxa/mission/chandra.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91659 2024-05-01 14:36:24.000000 daxa-0.0.5/daxa/mission/erosita.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40077 2024-05-01 14:36:24.000000 daxa-0.0.5/daxa/mission/integral.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34928 2024-05-01 14:36:24.000000 daxa-0.0.5/daxa/mission/nustar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64315 2024-05-01 14:36:24.000000 daxa-0.0.5/daxa/mission/rosat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33896 2024-05-01 14:36:24.000000 daxa-0.0.5/daxa/mission/suzaku.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37595 2024-05-01 14:36:24.000000 daxa-0.0.5/daxa/mission/swift.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30621 2024-05-01 14:36:24.000000 daxa-0.0.5/daxa/mission/xmm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:36:30.982342 daxa-0.0.5/daxa/process/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-01 14:36:24.000000 daxa-0.0.5/daxa/process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6576 2024-05-01 14:36:24.000000 daxa-0.0.5/daxa/process/_backend_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6214 2024-05-01 14:36:24.000000 daxa-0.0.5/daxa/process/_cleanup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:36:30.982342 daxa-0.0.5/daxa/process/erosita/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-01 14:36:24.000000 daxa-0.0.5/daxa/process/erosita/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19365 2024-05-01 14:36:24.000000 daxa-0.0.5/daxa/process/erosita/_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13072 2024-05-01 14:36:24.000000 daxa-0.0.5/daxa/process/erosita/assemble.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19531 2024-05-01 14:36:24.000000 daxa-0.0.5/daxa/process/erosita/clean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5998 2024-05-01 14:36:24.000000 daxa-0.0.5/daxa/process/erosita/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:36:30.982342 daxa-0.0.5/daxa/process/general/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-01 14:36:24.000000 daxa-0.0.5/daxa/process/general/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20667 2024-05-01 14:36:24.000000 daxa-0.0.5/daxa/process/general/preprocessed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-05-01 14:36:24.000000 daxa-0.0.5/daxa/process/general/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8394 2024-05-01 14:36:24.000000 daxa-0.0.5/daxa/process/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:36:30.986342 daxa-0.0.5/daxa/process/xmm/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-01 14:36:24.000000 daxa-0.0.5/daxa/process/xmm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22497 2024-05-01 14:36:24.000000 daxa-0.0.5/daxa/process/xmm/_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80965 2024-05-01 14:36:24.000000 daxa-0.0.5/daxa/process/xmm/assemble.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10859 2024-05-01 14:36:24.000000 daxa-0.0.5/daxa/process/xmm/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24297 2024-05-01 14:36:24.000000 daxa-0.0.5/daxa/process/xmm/clean.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16510 2024-05-01 14:36:24.000000 daxa-0.0.5/daxa/process/xmm/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24888 2024-05-01 14:36:24.000000 daxa-0.0.5/daxa/process/xmm/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:36:30.986342 daxa-0.0.5/daxa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6347 2024-05-01 14:36:30.000000 daxa-0.0.5/daxa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-01 14:36:30.000000 daxa-0.0.5/daxa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 14:36:30.000000 daxa-0.0.5/daxa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-01 14:36:30.000000 daxa-0.0.5/daxa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-01 14:36:30.000000 daxa-0.0.5/daxa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 14:36:30.986342 daxa-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-05-01 14:36:28.000000 daxa-0.0.5/setup.py
```

### Comparing `daxa-0.0.4/LICENSE` & `daxa-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `daxa-0.0.4/PKG-INFO` & `daxa-0.0.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daxa
-Version: 0.0.4
+Version: 0.0.5
 Summary: Democratising Astronomy X-ray Archives (DAXA) is an easy-to-use Python module which enables the simple processing and reduction of archives of X-ray telescope observations.
 Home-page: https://github.com/DavidT3/DAXA
 Author: David J Turner
 Author-email: turne540@msu.edu
 License: BSD 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -40,18 +40,45 @@
 identify what archival data might be available for a set of objects you wish to study. It is also possible to place
 no filters on the desired observations, and as such process every observation available for a set of missions. 
 
 Documentation is available on ReadTheDocs, and [can be found here](https://daxa.readthedocs.io), or
 accessed by clicking on the documentation build status at the top of the README. The source for the documentation can
 be found in the 'docs' directory in this repository.
 
+# Installing DAXA
+
+We **strongly recommend** that you make use of Python virtual environments, or (even better) Conda/Mamba virtual environments when installing DAXA.
+
+DAXA is available on the popular Python Package Index (PyPI), and can be installed like this:
+
+```
+pip install daxa
+```
+
+You can also fetch the current working version from the git repository, and install it (this method has replaced 'python setup.py install'):
+
+```
+git clone https://github.com/DavidT3/DAXA
+cd DAXA
+python -m pip install .
+```
+
+Alternatively you could use the 'editable' option (this has replaced running setup.py and passing 'develop') so that any changes you pull from the remote repository are reflected without having to reinstall DAXA.
+
+```
+git clone https://github.com/DavidT3/DAXA
+cd DAXA
+python -m pip install --editable .
+```
+
 # Which missions are supported?
 
-**_DAXA is still in an early stage of development, and as such the list of supported telescopes is currently
-limited. Support for more telescopes is either currently under development or being actively planned._** 
+_DAXA is still in a relatively early stage of development, and as such the support for local re-processing is 
+limited; however, support for the acquisition and use of pre-processed data is implemented for a wide selection 
+of telescopes:_ 
 
 * XMM-Newton Pointed
 * eROSITA Commissioning
 * eROSITA All-Sky Survey DR1 (German Half)
 * **_[Under Development - data acquisition implemented]_** NuSTAR
 * **_[Under Development - data acquisition implemented]_** Chandra
 * **_[Under Development - RASS/pointed data acquisition implemented]_** ROSAT
```

### Comparing `daxa-0.0.4/README.md` & `daxa-0.0.5/daxa.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: daxa
+Version: 0.0.5
+Summary: Democratising Astronomy X-ray Archives (DAXA) is an easy-to-use Python module which enables the simple processing and reduction of archives of X-ray telescope observations.
+Home-page: https://github.com/DavidT3/DAXA
+Author: David J Turner
+Author-email: turne540@msu.edu
+License: BSD 3
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy==1.24.4
+Requires-Dist: astroquery==0.4.7
+Requires-Dist: pandas==2.0.3
+Requires-Dist: astropy==5.2.2
+Requires-Dist: packaging==21.3
+Requires-Dist: tqdm==4.66.2
+Requires-Dist: exceptiongroup==1.0.4
+Requires-Dist: scipy==1.10.1
+Requires-Dist: tabulate==0.9.0
+Requires-Dist: unlzw3==0.2.2
+
 <p align="center">
     <img src="https://raw.githubusercontent.com/DavidT3/DAXA/master/daxa/files/daxa-high-resolution-logo-black-on-white-background.png" width="500">
 </p>
 
 [![Documentation Status](https://readthedocs.org/projects/daxa/badge/?version=latest)](https://daxa.readthedocs.io/en/latest/?badge=latest)
 
 # What is Democratising Archival X-ray Astronomy (DAXA)?
@@ -18,18 +40,45 @@
 identify what archival data might be available for a set of objects you wish to study. It is also possible to place
 no filters on the desired observations, and as such process every observation available for a set of missions. 
 
 Documentation is available on ReadTheDocs, and [can be found here](https://daxa.readthedocs.io), or
 accessed by clicking on the documentation build status at the top of the README. The source for the documentation can
 be found in the 'docs' directory in this repository.
 
+# Installing DAXA
+
+We **strongly recommend** that you make use of Python virtual environments, or (even better) Conda/Mamba virtual environments when installing DAXA.
+
+DAXA is available on the popular Python Package Index (PyPI), and can be installed like this:
+
+```
+pip install daxa
+```
+
+You can also fetch the current working version from the git repository, and install it (this method has replaced 'python setup.py install'):
+
+```
+git clone https://github.com/DavidT3/DAXA
+cd DAXA
+python -m pip install .
+```
+
+Alternatively you could use the 'editable' option (this has replaced running setup.py and passing 'develop') so that any changes you pull from the remote repository are reflected without having to reinstall DAXA.
+
+```
+git clone https://github.com/DavidT3/DAXA
+cd DAXA
+python -m pip install --editable .
+```
+
 # Which missions are supported?
 
-**_DAXA is still in an early stage of development, and as such the list of supported telescopes is currently
-limited. Support for more telescopes is either currently under development or being actively planned._** 
+_DAXA is still in a relatively early stage of development, and as such the support for local re-processing is 
+limited; however, support for the acquisition and use of pre-processed data is implemented for a wide selection 
+of telescopes:_ 
 
 * XMM-Newton Pointed
 * eROSITA Commissioning
 * eROSITA All-Sky Survey DR1 (German Half)
 * **_[Under Development - data acquisition implemented]_** NuSTAR
 * **_[Under Development - data acquisition implemented]_** Chandra
 * **_[Under Development - RASS/pointed data acquisition implemented]_** ROSAT
```

### Comparing `daxa-0.0.4/daxa/archive/base.py` & `daxa-0.0.5/daxa/archive/base.py`

 * *Files identical despite different names*

### Comparing `daxa-0.0.4/daxa/config.py` & `daxa-0.0.5/daxa/config.py`

 * *Files identical despite different names*

### Comparing `daxa-0.0.4/daxa/exceptions.py` & `daxa-0.0.5/daxa/exceptions.py`

 * *Files identical despite different names*

### Comparing `daxa-0.0.4/daxa/files/browse_extract.pl` & `daxa-0.0.5/daxa/files/browse_extract.pl`

 * *Files identical despite different names*

### Comparing `daxa-0.0.4/daxa/files/daxa-high-resolution-color-logo.png` & `daxa-0.0.5/daxa/files/daxa-high-resolution-color-logo.png`

 * *Files identical despite different names*

### Comparing `daxa-0.0.4/daxa/files/daxa-high-resolution-logo-black-on-transparent-background.png` & `daxa-0.0.5/daxa/files/daxa-high-resolution-logo-black-on-transparent-background.png`

 * *Files identical despite different names*

### Comparing `daxa-0.0.4/daxa/files/daxa-high-resolution-logo-black-on-white-background.png` & `daxa-0.0.5/daxa/files/daxa-high-resolution-logo-black-on-white-background.png`

 * *Files identical despite different names*

### Comparing `daxa-0.0.4/daxa/files/erass_de_dr1_info.csv` & `daxa-0.0.5/daxa/files/erass_de_dr1_info.csv`

 * *Files identical despite different names*

### Comparing `daxa-0.0.4/daxa/files/erosita_calpv_info.csv` & `daxa-0.0.5/daxa/files/erosita_calpv_info.csv`

 * *Files identical despite different names*

### Comparing `daxa-0.0.4/daxa/files/sas_errors.csv` & `daxa-0.0.5/daxa/files/sas_errors.csv`

 * *Files identical despite different names*

### Comparing `daxa-0.0.4/daxa/files/sas_warnings.csv` & `daxa-0.0.5/daxa/files/sas_warnings.csv`

 * *Files identical despite different names*

### Comparing `daxa-0.0.4/daxa/misc.py` & `daxa-0.0.5/daxa/misc.py`

 * *Files identical despite different names*

### Comparing `daxa-0.0.4/daxa/mission/__init__.py` & `daxa-0.0.5/daxa/mission/__init__.py`

 * *Files identical despite different names*

### Comparing `daxa-0.0.4/daxa/mission/asca.py` & `daxa-0.0.5/daxa/mission/asca.py`

 * *Files identical despite different names*

### Comparing `daxa-0.0.4/daxa/mission/base.py` & `daxa-0.0.5/daxa/mission/base.py`

 * *Files identical despite different names*

### Comparing `daxa-0.0.4/daxa/mission/chandra.py` & `daxa-0.0.5/daxa/mission/chandra.py`

 * *Files identical despite different names*

### Comparing `daxa-0.0.4/daxa/mission/erosita.py` & `daxa-0.0.5/daxa/mission/erosita.py`

 * *Files identical despite different names*

### Comparing `daxa-0.0.4/daxa/mission/integral.py` & `daxa-0.0.5/daxa/mission/integral.py`

 * *Files identical despite different names*

### Comparing `daxa-0.0.4/daxa/mission/nustar.py` & `daxa-0.0.5/daxa/mission/nustar.py`

 * *Files identical despite different names*

### Comparing `daxa-0.0.4/daxa/mission/rosat.py` & `daxa-0.0.5/daxa/mission/rosat.py`

 * *Files identical despite different names*

### Comparing `daxa-0.0.4/daxa/mission/suzaku.py` & `daxa-0.0.5/daxa/mission/suzaku.py`

 * *Files identical despite different names*

### Comparing `daxa-0.0.4/daxa/mission/swift.py` & `daxa-0.0.5/daxa/mission/swift.py`

 * *Files identical despite different names*

### Comparing `daxa-0.0.4/daxa/mission/xmm.py` & `daxa-0.0.5/daxa/mission/xmm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #  This code is a part of the Democratising Archival X-ray Astronomy (DAXA) module.
-#  Last modified by David J Turner (turne540@msu.edu) 24/04/2024, 13:58. Copyright (c) The Contributors
+#  Last modified by David J Turner (turne540@msu.edu) 01/05/2024, 10:25. Copyright (c) The Contributors
 import os.path
 import tarfile
 from datetime import datetime
 from multiprocessing import Pool
 from typing import List, Union, Any
 from warnings import warn
 
@@ -181,15 +181,15 @@
         into a Pandas dataframe and stored.
         """
         # First of all I want to know how many entries there are in the 'all observations' table, because I need to
         #  specify the number of rows to select in my ADQL (Astronomical Data Query Language) command for reasons
         #  I'll explain in a second
         count_tab = AQXMMNewton.query_xsa_tap('select count(observation_id) from xsa.v_all_observations')
         # Then I round up to the nearest 1000, probably unnecessary but oh well
-        num_obs = np.ceil(count_tab['count'].tolist()[0] / 1000).astype(int) * 1000
+        num_obs = np.ceil(count_tab['COUNT'].tolist()[0] / 1000).astype(int) * 1000
         # Now I have to be a bit cheesy - If I used select * (which is what I would normally do in an SQL-derived
         #  language to grab every row) it actually only returns the top 2000. I think that * is replaced with TOP 2000
         #  before the query is sent to the server. However if I specify a TOP N, where N is greater than 2000, then it
         #  works as intended. I hope this is a stable behaviour!
         # TODO Might want to grab footprint_fov, stc_s at some point
         obs_info = AQXMMNewton.query_xsa_tap("select TOP {} ra, dec, observation_id, start_utc, with_science, "
                                              "duration, proprietary_end_date, revolution "
```

### Comparing `daxa-0.0.4/daxa/process/_backend_check.py` & `daxa-0.0.5/daxa/process/_backend_check.py`

 * *Files identical despite different names*

### Comparing `daxa-0.0.4/daxa/process/_cleanup.py` & `daxa-0.0.5/daxa/process/_cleanup.py`

 * *Files identical despite different names*

### Comparing `daxa-0.0.4/daxa/process/erosita/_common.py` & `daxa-0.0.5/daxa/process/erosita/_common.py`

 * *Files identical despite different names*

### Comparing `daxa-0.0.4/daxa/process/erosita/assemble.py` & `daxa-0.0.5/daxa/process/erosita/assemble.py`

 * *Files identical despite different names*

### Comparing `daxa-0.0.4/daxa/process/erosita/clean.py` & `daxa-0.0.5/daxa/process/erosita/clean.py`

 * *Files identical despite different names*

### Comparing `daxa-0.0.4/daxa/process/erosita/setup.py` & `daxa-0.0.5/daxa/process/erosita/setup.py`

 * *Files identical despite different names*

### Comparing `daxa-0.0.4/daxa/process/general/preprocessed.py` & `daxa-0.0.5/daxa/process/general/preprocessed.py`

 * *Files identical despite different names*

### Comparing `daxa-0.0.4/daxa/process/general/setup.py` & `daxa-0.0.5/daxa/process/general/setup.py`

 * *Files identical despite different names*

### Comparing `daxa-0.0.4/daxa/process/simple.py` & `daxa-0.0.5/daxa/process/simple.py`

 * *Files identical despite different names*

### Comparing `daxa-0.0.4/daxa/process/xmm/_common.py` & `daxa-0.0.5/daxa/process/xmm/_common.py`

 * *Files identical despite different names*

### Comparing `daxa-0.0.4/daxa/process/xmm/assemble.py` & `daxa-0.0.5/daxa/process/xmm/assemble.py`

 * *Files identical despite different names*

### Comparing `daxa-0.0.4/daxa/process/xmm/check.py` & `daxa-0.0.5/daxa/process/xmm/check.py`

 * *Files identical despite different names*

### Comparing `daxa-0.0.4/daxa/process/xmm/clean.py` & `daxa-0.0.5/daxa/process/xmm/clean.py`

 * *Files identical despite different names*

### Comparing `daxa-0.0.4/daxa/process/xmm/generate.py` & `daxa-0.0.5/daxa/process/xmm/generate.py`

 * *Files identical despite different names*

### Comparing `daxa-0.0.4/daxa/process/xmm/setup.py` & `daxa-0.0.5/daxa/process/xmm/setup.py`

 * *Files identical despite different names*

### Comparing `daxa-0.0.4/daxa.egg-info/PKG-INFO` & `daxa-0.0.5/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: daxa
-Version: 0.0.4
-Summary: Democratising Astronomy X-ray Archives (DAXA) is an easy-to-use Python module which enables the simple processing and reduction of archives of X-ray telescope observations.
-Home-page: https://github.com/DavidT3/DAXA
-Author: David J Turner
-Author-email: turne540@msu.edu
-License: BSD 3
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy==1.24.4
-Requires-Dist: astroquery==0.4.7
-Requires-Dist: pandas==2.0.3
-Requires-Dist: astropy==5.2.2
-Requires-Dist: packaging==21.3
-Requires-Dist: tqdm==4.66.2
-Requires-Dist: exceptiongroup==1.0.4
-Requires-Dist: scipy==1.10.1
-Requires-Dist: tabulate==0.9.0
-Requires-Dist: unlzw3==0.2.2
-
 <p align="center">
     <img src="https://raw.githubusercontent.com/DavidT3/DAXA/master/daxa/files/daxa-high-resolution-logo-black-on-white-background.png" width="500">
 </p>
 
 [![Documentation Status](https://readthedocs.org/projects/daxa/badge/?version=latest)](https://daxa.readthedocs.io/en/latest/?badge=latest)
 
 # What is Democratising Archival X-ray Astronomy (DAXA)?
@@ -40,18 +18,45 @@
 identify what archival data might be available for a set of objects you wish to study. It is also possible to place
 no filters on the desired observations, and as such process every observation available for a set of missions. 
 
 Documentation is available on ReadTheDocs, and [can be found here](https://daxa.readthedocs.io), or
 accessed by clicking on the documentation build status at the top of the README. The source for the documentation can
 be found in the 'docs' directory in this repository.
 
+# Installing DAXA
+
+We **strongly recommend** that you make use of Python virtual environments, or (even better) Conda/Mamba virtual environments when installing DAXA.
+
+DAXA is available on the popular Python Package Index (PyPI), and can be installed like this:
+
+```
+pip install daxa
+```
+
+You can also fetch the current working version from the git repository, and install it (this method has replaced 'python setup.py install'):
+
+```
+git clone https://github.com/DavidT3/DAXA
+cd DAXA
+python -m pip install .
+```
+
+Alternatively you could use the 'editable' option (this has replaced running setup.py and passing 'develop') so that any changes you pull from the remote repository are reflected without having to reinstall DAXA.
+
+```
+git clone https://github.com/DavidT3/DAXA
+cd DAXA
+python -m pip install --editable .
+```
+
 # Which missions are supported?
 
-**_DAXA is still in an early stage of development, and as such the list of supported telescopes is currently
-limited. Support for more telescopes is either currently under development or being actively planned._** 
+_DAXA is still in a relatively early stage of development, and as such the support for local re-processing is 
+limited; however, support for the acquisition and use of pre-processed data is implemented for a wide selection 
+of telescopes:_ 
 
 * XMM-Newton Pointed
 * eROSITA Commissioning
 * eROSITA All-Sky Survey DR1 (German Half)
 * **_[Under Development - data acquisition implemented]_** NuSTAR
 * **_[Under Development - data acquisition implemented]_** Chandra
 * **_[Under Development - RASS/pointed data acquisition implemented]_** ROSAT
```

### Comparing `daxa-0.0.4/daxa.egg-info/SOURCES.txt` & `daxa-0.0.5/daxa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `daxa-0.0.4/setup.py` & `daxa-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Uses the README as the long description
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='daxa',
-    version='v0.0.4',
+    version='v0.0.5',
     packages=find_packages(),
     url='https://github.com/DavidT3/DAXA',
     license='BSD 3',
     author='David J Turner',
     author_email='turne540@msu.edu',
     description='Democratising Astronomy X-ray Archives (DAXA) is an easy-to-use Python module which enables '
                 'the simple processing and reduction of archives of X-ray telescope observations.',
```

