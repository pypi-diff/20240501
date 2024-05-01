# Comparing `tmp/astro-metadata-translator-26.2024.900.tar.gz` & `tmp/astro_metadata_translator-27.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro-metadata-translator-26.2024.900.tar", last modified: Thu Feb 29 10:20:49 2024, max compression
+gzip compressed data, was "astro_metadata_translator-27.0.0rc1.tar", last modified: Wed May  1 21:17:09 2024, max compression
```

## Comparing `astro-metadata-translator-26.2024.900.tar` & `astro_metadata_translator-27.0.0rc1.tar`

### file list

```diff
@@ -1,92 +1,102 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:49.200474 astro-metadata-translator-26.2024.900/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-02-29 10:20:49.200474 astro-metadata-translator-26.2024.900/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:49.184474 astro-metadata-translator-26.2024.900/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:49.188474 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:49.188474 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/bin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13335 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/bin/translateheader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/bin/writeindex.py
--rw-r--r--   0 runner    (1001) docker     (127)     5407 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/bin/writesidecar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:49.192474 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7357 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/cli/astrometadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:49.184474 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/corrections/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:49.196474 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/corrections/HSC/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00042600.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00120200.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00120400.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00120600.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00120800.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00121000.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00121200.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00121400.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00121600.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00121800.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00122000.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00122800.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00123000.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00123200.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00123800.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00124000.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00124200.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00124400.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00124600.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00124800.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00186800.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00187000.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00187200.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00187400.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00187600.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00188000.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00188200.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     9750 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/file_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    18951 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/headers.py
--rw-r--r--   0 runner    (1001) docker     (127)    14677 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/indexing.py
--rw-r--r--   0 runner    (1001) docker     (127)     8303 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/observationGroup.py
--rw-r--r--   0 runner    (1001) docker     (127)    27129 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/observationInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)    12878 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/properties.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:49.196474 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/serialize/
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/serialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/serialize/fits.py
--rw-r--r--   0 runner    (1001) docker     (127)    11827 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    50088 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/translator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:49.196474 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/translators/
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/translators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14863 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/translators/decam.py
--rw-r--r--   0 runner    (1001) docker     (127)     7029 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/translators/fits.py
--rw-r--r--   0 runner    (1001) docker     (127)     6569 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/translators/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8205 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/translators/hsc.py
--rw-r--r--   0 runner    (1001) docker     (127)     9926 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/translators/megaprime.py
--rw-r--r--   0 runner    (1001) docker     (127)     9013 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/translators/sdss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/translators/subaru.py
--rw-r--r--   0 runner    (1001) docker     (127)     8413 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/translators/suprimecam.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-29 10:20:49.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:49.200474 astro-metadata-translator-26.2024.900/python/astro_metadata_translator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-02-29 10:20:49.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-02-29 10:20:49.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 10:20:49.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-02-29 10:20:49.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-29 10:20:49.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-29 10:20:49.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 10:20:49.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-02-29 10:20:49.200474 astro-metadata-translator-26.2024.900/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:49.200474 astro-metadata-translator-26.2024.900/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/tests/test_basics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4417 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/tests/test_cfht.py
--rw-r--r--   0 runner    (1001) docker     (127)     7401 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/tests/test_decam.py
--rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/tests/test_extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/tests/test_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    17115 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/tests/test_headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/tests/test_indexing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/tests/test_sdss.py
--rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/tests/test_shadowing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6904 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/tests/test_subaru.py
--rw-r--r--   0 runner    (1001) docker     (127)     6382 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/tests/test_translate_header.py
--rw-r--r--   0 runner    (1001) docker     (127)     9387 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/tests/test_translation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:17:09.851095 astro_metadata_translator-27.0.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-05-01 21:17:09.851095 astro_metadata_translator-27.0.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:17:09.835095 astro_metadata_translator-27.0.0rc1/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:17:09.839095 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:17:09.843095 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8644 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/bin/translate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4220 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/bin/writeindex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5427 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/bin/writesidecar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:17:09.843095 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7659 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/cli/astrometadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:17:09.835095 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/corrections/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:17:09.843095 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/corrections/CFHT/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/corrections/CFHT/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:17:09.843095 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/corrections/DECam/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/corrections/DECam/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:17:09.847095 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/corrections/HSC/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00042600.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00120200.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00120400.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00120600.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00120800.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00121000.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00121200.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00121400.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00121600.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00121800.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00122000.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00122800.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00123000.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00123200.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00123800.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00124000.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00124200.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00124400.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00124600.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00124800.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00186800.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00187000.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00187200.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00187400.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00187600.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00188000.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00188200.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/corrections/HSC/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:17:09.847095 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/corrections/SDSS/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/corrections/SDSS/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:17:09.847095 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/corrections/SuprimeCam/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/corrections/SuprimeCam/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9443 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/file_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18944 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14533 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/indexing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8647 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/observationGroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27452 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/observationInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18320 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:17:09.847095 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/serialize/
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/serialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/serialize/fits.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12647 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55373 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/translator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:17:09.847095 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/translators/
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/translators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16414 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/translators/decam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7028 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/translators/fits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6557 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/translators/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8529 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/translators/hsc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10567 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/translators/megaprime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9013 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/translators/sdss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/translators/subaru.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8413 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/translators/suprimecam.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-01 21:17:09.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:17:09.851095 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-05-01 21:17:09.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-05-01 21:17:09.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 21:17:09.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-01 21:17:09.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-01 21:17:09.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-01 21:17:09.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 21:17:09.000000 astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-01 21:17:09.851095 astro_metadata_translator-27.0.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:17:09.851095 astro_metadata_translator-27.0.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/tests/test_basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4532 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/tests/test_cfht.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7524 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/tests/test_decam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/tests/test_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/tests/test_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17115 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/tests/test_headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8249 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/tests/test_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/tests/test_sdss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/tests/test_shadowing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7019 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/tests/test_subaru.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6896 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/tests/test_translate_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10022 2024-05-01 21:16:59.000000 astro_metadata_translator-27.0.0rc1/tests/test_translation.py
```

### Comparing `astro-metadata-translator-26.2024.900/LICENSE` & `astro_metadata_translator-27.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `astro-metadata-translator-26.2024.900/PKG-INFO` & `astro_metadata_translator-27.0.0rc1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 Metadata-Version: 2.1
 Name: astro-metadata-translator
-Version: 26.2024.900
+Version: 27.0.0rc1
 Summary: A translator for astronomical metadata.
-Home-page: https://github.com/lsst/astro_metadata_translator
-Author: Rubin Observatory Data Management
-Author-email: dm-admin@lists.lsst.org
+Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
+Project-URL: Homepage, https://github.com/lsst/astro_metadata_translator
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering :: Astronomy
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: astropy>=3.0.5
 Requires-Dist: pyyaml>=3.13
 Requires-Dist: click>=8
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
 
 # astro_metadata_translator
 
 [![pypi](https://img.shields.io/pypi/v/astro-metadata-translator.svg)](https://pypi.org/project/astro-metadata-translator/)
 [![codecov](https://codecov.io/gh/lsst/astro_metadata_translator/branch/main/graph/badge.svg?token=0HtEHdoYDF)](https://codecov.io/gh/lsst/astro_metadata_translator)
 
 Observation metadata handling infrastructure
```

### Comparing `astro-metadata-translator-26.2024.900/README.md` & `astro_metadata_translator-27.0.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `astro-metadata-translator-26.2024.900/python/astro_metadata_translator/__init__.py` & `astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/__init__.py`

 * *Files identical despite different names*

### Comparing `astro-metadata-translator-26.2024.900/python/astro_metadata_translator/bin/writeindex.py` & `astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/bin/writeindex.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,20 +7,19 @@
 # for details of code ownership.
 #
 # Use of this source code is governed by a 3-clause BSD-style
 # license that can be found in the LICENSE file.
 
 from __future__ import annotations
 
-__all__ = "write_index_files"
+__all__ = ["write_index_files"]
 
 import json
 import logging
 import os
-import sys
 from collections.abc import MutableMapping, Sequence
 from typing import IO
 
 from ..file_helpers import find_files
 from ..indexing import index_files
 
 log = logging.getLogger(__name__)
@@ -29,16 +28,15 @@
 def write_index_files(
     files: Sequence[str],
     regex: str,
     hdrnum: int,
     print_trace: bool,
     content_mode: str = "translated",
     outpath: str | None = None,
-    outstream: IO = sys.stdout,
-    errstream: IO = sys.stderr,
+    outstream: IO | None = None,
 ) -> tuple[list[str], list[str]]:
     """Process each file and create JSON index file.
 
     The index file will have common information in the toplevel.
     There is then a ``__DIFF__`` key that is a dictionary with file
     names as keys and per-file differences as the values in a dict.
 
@@ -56,25 +54,23 @@
         If there is an error reading the file and this parameter is `True`,
         a full traceback of the exception will be reported. If `False` prints
         a one line summary of the error condition.
     content_mode : `str`
         Form of data to write in index file. Options are:
         ``translated`` (default) to write ObservationInfo to the index;
         ``metadata`` to write native metadata headers to the index.
-        The index file is called ``_index.json``
+        The index file is called ``_index.json``.
     outpath : `str`, optional
         If specified a single index file will be written to this location
         combining all the information from all files. If `None`, the default,
         and index file will be written to each directory in which files
         are found.
     outstream : `io.StringIO`, optional
-        Output stream to use for standard messages. Defaults to `sys.stdout`.
-    errstream : `io.StringIO`, optional
-        Stream to send messages that would normally be sent to standard
-        error. Defaults to `sys.stderr`.
+        Output stream to use for standard messages. Defaults to `None` which
+        uses the default output stream. Defaults to `sys.stdout`.
 
     Returns
     -------
     okay : `list` of `str`
         All the files that were processed successfully.
     failed : `list` of `str`
         All the files that could not be processed.
@@ -100,15 +96,20 @@
             files_per_directory.setdefault(head, []).append(tail)
     else:
         files_per_directory["."] = list(found_files)
 
     # Extract translated metadata for each file in each directory
     for directory, files_in_dir in files_per_directory.items():
         output, this_okay, this_failed = index_files(
-            files_in_dir, directory, hdrnum, print_trace, content_mode, outstream, errstream
+            files_in_dir,
+            directory,
+            hdrnum,
+            print_trace,
+            content_mode,
+            outstream,
         )
 
         failed.extend(this_failed)
         okay.extend(this_okay)
 
         # Write the index file
         if outpath is None:
```

### Comparing `astro-metadata-translator-26.2024.900/python/astro_metadata_translator/bin/writesidecar.py` & `astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/bin/writesidecar.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,27 +9,40 @@
 # Use of this source code is governed by a 3-clause BSD-style
 # license that can be found in the LICENSE file.
 
 from __future__ import annotations
 
 __all__ = ("write_sidecar_files", "write_sidecar_file")
 
+import logging
 import os
-import sys
 import traceback
 from collections.abc import Sequence
 from typing import IO
 
 from ..file_helpers import find_files, read_file_info
 
+log = logging.getLogger(__name__)
+
 
 def _split_ext(file: str) -> tuple[str, str]:
     """Split the extension from the file name and return it and the root.
 
-    Special case handling of .gz and other compression extensions.
+    Parameters
+    ----------
+    file : `str`
+        The file name to examine.
+
+    Returns
+    -------
+    root : `str`
+        The root of the file name.
+    ext : `str`
+        The file extension. There is special case handling of .gz and other
+        compression extensions.
     """
     special = {".gz", ".bz2", ".xz", ".fz"}
 
     root, ext = os.path.splitext(file)
 
     if ext in special:
         root, second_ext = os.path.splitext(root)
@@ -39,16 +52,15 @@
 
 
 def write_sidecar_file(
     file: str,
     hdrnum: int,
     content_mode: str,
     print_trace: bool,
-    outstream: IO = sys.stdout,
-    errstream: IO = sys.stderr,
+    outstream: IO | None = None,
 ) -> bool:
     """Write JSON summary to sidecar file.
 
     Parameters
     ----------
     file : `str`
         The file from which the header is to be read.
@@ -61,18 +73,16 @@
         ``translated`` to write the translated ObservationInfo.
     print_trace : `bool`
         If there is an error reading the file and this parameter is `True`,
         a full traceback of the exception will be reported. If `False` prints
         a one line summary of the error condition. If `None` the exception
         will be allowed.
     outstream : `io.StringIO`, optional
-        Output stream to use for standard messages. Defaults to `sys.stdout`.
-    errstream : `io.StringIO`, optional
-        Stream to send messages that would normally be sent to standard
-        error. Defaults to `sys.stderr`.
+        Output stream to use for standard messages. Defaults to `None` which
+        uses the default output stream.
 
     Returns
     -------
     success : `bool`
         `True` if the file was handled successfully, `False` if the file
         could not be processed.
     """
@@ -84,26 +94,26 @@
         json_str = read_file_info(
             file,
             hdrnum,
             content_mode=content_mode,
             content_type="json",
             print_trace=print_trace,
             outstream=outstream,
-            errstream=errstream,
         )
         if json_str is None:
             return False
 
         # Calculate sidecar file name derived from this file.
         # Match the ButlerURI behavior in that .fits.gz should be replaced
         # with .json, and not resulting in .fits.json.
         root, ext = _split_ext(file)
         newfile = root + ".json"
         with open(newfile, "w") as fd:
             print(json_str, file=fd)
+        log.debug("Writing sidecar file %s", newfile)
 
     except Exception as e:
         if print_trace is None:
             raise e
         if print_trace:
             traceback.print_exc(file=outstream)
         else:
@@ -114,55 +124,53 @@
 
 def write_sidecar_files(
     files: Sequence[str],
     regex: str,
     hdrnum: int,
     content_mode: str,
     print_trace: bool,
-    outstream: IO = sys.stdout,
-    errstream: IO = sys.stderr,
+    outstream: IO | None = None,
 ) -> tuple[list[str], list[str]]:
     """Process each file and create sidecar file.
 
     Parameters
     ----------
     files : iterable of `str`
         The files or directories from which the headers are to be read.
     regex : `str`
         Regular expression string used to filter files when a directory is
         scanned.
     hdrnum : `int`
         The HDU number to read. The primary header is always read and
+        merged with the header from this HDU.
     content_mode : `str`
         Content mode to use when writing JSON to sidecar. Options are:
         ``metadata`` to write the unmodified header;
         ``translated`` to write the translated ObservationInfo.
     print_trace : `bool`
         If there is an error reading the file and this parameter is `True`,
         a full traceback of the exception will be reported. If `False` prints
         a one line summary of the error condition.
     outstream : `io.StringIO`, optional
-        Output stream to use for standard messages. Defaults to `sys.stdout`.
-    errstream : `io.StringIO`, optional
-        Stream to send messages that would normally be sent to standard
-        error. Defaults to `sys.stderr`.
+        Output stream to use for standard messages. Defaults to `None` which
+        uses the default output stream.
 
     Returns
     -------
     okay : `list` of `str`
         All the files that were processed successfully.
     failed : `list` of `str`
         All the files that could not be processed.
     """
     found_files = find_files(files, regex)
 
     # Process each file
     failed = []
     okay = []
     for path in sorted(found_files):
-        isok = write_sidecar_file(path, hdrnum, content_mode, print_trace, outstream, errstream)
+        isok = write_sidecar_file(path, hdrnum, content_mode, print_trace, outstream)
         if isok:
             okay.append(path)
         else:
             failed.append(path)
 
     return okay, failed
```

### Comparing `astro-metadata-translator-26.2024.900/python/astro_metadata_translator/cli/astrometadata.py` & `astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/cli/astrometadata.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,21 +16,23 @@
 import importlib
 import logging
 import os
 from collections.abc import Sequence
 
 import click
 
-from ..bin.translateheader import process_files as translate_header
+from ..bin.translate import translate_or_dump_headers
 from ..bin.writeindex import write_index_files
 from ..bin.writesidecar import write_sidecar_files
 
 # Default regex for finding data files
 re_default = r"\.fit[s]?\b"
 
+log = logging.getLogger("astro_metadata_translator")
+
 PACKAGES_VAR = "METADATA_TRANSLATORS"
 
 hdrnum_option = click.option(
     "-n",
     "--hdrnum",
     default=-1,
     help="HDU number to read. If the HDU can not be found, a warning is issued but"
@@ -91,15 +93,15 @@
         packages_set.update(new_packages)
 
     # Process import requests
     for m in packages_set:
         try:
             importlib.import_module(m)
         except (ImportError, ModuleNotFoundError):
-            logging.warn("Failed to import translator module: %s", m)
+            log.warning("Failed to import translator module: %s", m)
 
 
 @main.command(help="Translate metadata in supplied files and report.")
 @click.argument("files", nargs=-1)
 @click.option(
     "-q",
     "--quiet/--no-quiet",
@@ -122,15 +124,15 @@
     ctx: click.Context, files: Sequence[str], quiet: bool, hdrnum: int, mode: str, regex: str
 ) -> None:
     """Translate a header."""
     # For quiet mode we want to translate everything but report nothing.
     if quiet:
         mode = "none"
 
-    okay, failed = translate_header(files, regex, hdrnum, ctx.obj["TRACEBACK"], output_mode=mode)
+    okay, failed = translate_or_dump_headers(files, regex, hdrnum, ctx.obj["TRACEBACK"], output_mode=mode)
 
     if failed:
         click.echo("Files with failed translations:", err=True)
         for f in failed:
             click.echo(f"\t{f}", err=True)
 
     if not okay:
@@ -151,15 +153,15 @@
     " 'yamlnative' is as for 'yaml' but dumps the native (astropy vs PropertyList) native form."
     " 'yamlfixed' is as for 'fixed' but dumps the native (astropy vs PropertyList) native form.",
 )
 @regex_option
 @click.pass_context
 def dump(ctx: click.Context, files: Sequence[str], hdrnum: int, mode: str, regex: str) -> None:
     """Dump a header."""
-    okay, failed = translate_header(files, regex, hdrnum, ctx.obj["TRACEBACK"], output_mode=mode)
+    okay, failed = translate_or_dump_headers(files, regex, hdrnum, ctx.obj["TRACEBACK"], output_mode=mode)
 
     if failed:
         click.echo("Files with failed header extraction:", err=True)
         for f in failed:
             click.echo(f"\t{f}", err=True)
 
     if not okay:
@@ -178,16 +180,22 @@
     okay, failed = write_sidecar_files(files, regex, hdrnum, content, ctx.obj["TRACEBACK"])
 
     if failed:
         click.echo("Files with failed header extraction:", err=True)
         for f in failed:
             click.echo(f"\t{f}", err=True)
 
+    if not okay and not failed:
+        # No files found at all.
+        click.echo("Found no files matching regex.")
+        raise click.exceptions.Exit(1)
+
     if not okay:
         # Good status if anything was returned in okay
+        click.echo(f"No files processed successfully. Found {len(failed)}.", err=True)
         raise click.exceptions.Exit(1)
 
 
 @main.command(help="Write JSON index file for entire directory.")
 @click.argument("files", nargs=-1)
 @hdrnum_option
 @regex_option
```

### Comparing `astro-metadata-translator-26.2024.900/python/astro_metadata_translator/file_helpers.py` & `astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/file_helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,32 +5,37 @@
 # (http://www.lsst.org).
 # See the LICENSE file at the top-level directory of this distribution
 # for details of code ownership.
 #
 # Use of this source code is governed by a 3-clause BSD-style
 # license that can be found in the LICENSE file.
 
-"""Support functions for script implementations."""
+"""Support functions for script implementations.
+
+These functions should not be treated as part of the public API.
+"""
 
 from __future__ import annotations
 
 __all__ = ("find_files", "read_basic_metadata_from_file", "read_file_info")
 
 import json
+import logging
 import os
 import re
-import sys
 import traceback
 from collections.abc import Iterable, MutableMapping
 from typing import IO, Any
 
 from .headers import merge_headers
 from .observationInfo import ObservationInfo
 from .tests import read_test_file
 
+log = logging.getLogger(__name__)
+
 # Prefer afw over Astropy
 try:
     import lsst.daf.base  # noqa: F401 need PropertyBase for readMetadata
     from lsst.afw.fits import FitsError, readMetadata
 
     def _read_fits_metadata(file: str, hdu: int, can_raise: bool = False) -> MutableMapping[str, Any] | None:
         """Read a FITS header using afw.
@@ -116,32 +121,29 @@
         else:
             found_files.append(file)
 
     return found_files
 
 
 def read_basic_metadata_from_file(
-    file: str, hdrnum: int, errstream: IO = sys.stderr, can_raise: bool = True
+    file: str, hdrnum: int, can_raise: bool = True
 ) -> MutableMapping[str, Any] | None:
     """Read a raw header from a file, merging if necessary.
 
     Parameters
     ----------
     file : `str`
         Name of file to read. Can be FITS, YAML or JSON. YAML or JSON must be
         a simple top-level dict.
     hdrnum : `int`
         Header number to read. Only relevant for FITS. If greater than 1
         it will be merged with the primary header. If a negative number is
         given the second header, if present, will be merged with the primary
         header. If there is only a primary header a negative number behaves
         identically to specifying 0 for the HDU number.
-    errstream : `io.StringIO`, optional
-        Stream to send messages that would normally be sent to standard
-        error. Defaults to `sys.stderr`. Only used if exceptions are disabled.
     can_raise : `bool`, optional
         Indicate whether the function can raise an exception (default)
         or should return `None` on error. Can still raise if an unexpected
         error is encountered.
 
     Returns
     -------
@@ -161,40 +163,39 @@
                 raise e
         if hdrnum != 0:
             # YAML can't have HDUs so skip merging below
             hdrnum = 0
     else:
         md = _read_fits_metadata(file, 0, can_raise=can_raise)
     if md is None:
-        print(f"Unable to open file {file}", file=errstream)
+        log.warning("Unable to open file %s", file)
         return None
     if hdrnum < 0:
         if "EXTEND" in md and md["EXTEND"]:
             hdrnum = 1
     if hdrnum > 0:
         # Allow this to fail
         mdn = _read_fits_metadata(file, int(hdrnum), can_raise=False)
         # Astropy does not allow append mode since it does not
         # convert lists to multiple cards. Overwrite for now
         if mdn is not None:
             md = merge_headers([md, mdn], mode="overwrite")
         else:
-            print(f"HDU {hdrnum} was not found in file {file}. Ignoring request.", file=errstream)
+            log.warning("HDU %d was not found in file %s. Ignoring request.", hdrnum, file)
 
     return md
 
 
 def read_file_info(
     file: str,
     hdrnum: int,
     print_trace: bool | None = None,
     content_mode: str = "translated",
     content_type: str = "simple",
-    outstream: IO = sys.stdout,
-    errstream: IO = sys.stderr,
+    outstream: IO | None = None,
 ) -> str | MutableMapping[str, Any] | ObservationInfo | None:
     """Read information from file.
 
     Parameters
     ----------
     file : `str`
         The file from which the header is to be read.
@@ -211,19 +212,17 @@
         metadata headers; ``translated`` to return the output from metadata
         translation.
     content_type : `str`, optional
         Form of content to be returned. Can be either ``json`` to return a
         JSON string, ``simple`` to always return a `dict`, or ``native`` to
         return either a `dict` (for ``metadata``) or `.ObservationInfo` for
         ``translated``.
-    outstream : `io.StringIO`, optional
-        Output stream to use for standard messages. Defaults to `sys.stdout`.
-    errstream : `io.StringIO`, optional
-        Stream to send messages that would normally be sent to standard
-        error. Defaults to `sys.stderr`.
+    outstream : `io.StringIO` or `None`, optional
+        Output stream to use for standard messages. Defaults to `None` which
+        uses the default output stream.
 
     Returns
     -------
     simple : `dict` of `str` or `.ObservationInfo`
         The return value of `.ObservationInfo.to_simple`. Returns `None`
         if there was a problem and ``print_trace`` is not `None`.
     """
@@ -231,17 +230,15 @@
         raise ValueError(f"Unrecognized content mode request: {content_mode}")
 
     if content_type not in ("native", "simple", "json"):
         raise ValueError(f"Unrecognized content type request {content_type}")
 
     try:
         # Calculate the JSON from the file
-        md = read_basic_metadata_from_file(
-            file, hdrnum, errstream=errstream, can_raise=True if print_trace is None else False
-        )
+        md = read_basic_metadata_from_file(file, hdrnum, can_raise=True if print_trace is None else False)
         if md is None:
             return None
         if content_mode == "metadata":
             # Do not fix the header
             if content_type == "json":
                 # Add a key to tell the reader whether this is md or translated
                 md["__CONTENT__"] = content_mode
```

### Comparing `astro-metadata-translator-26.2024.900/python/astro_metadata_translator/headers.py` & `astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/headers.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,21 +13,21 @@
 
 from __future__ import annotations
 
 __all__ = ("merge_headers", "fix_header")
 
 import copy
 import datetime
-import importlib.resources as resources
 import itertools
 import logging
 import os
 import posixpath
 from collections import Counter
 from collections.abc import Mapping, MutableMapping, Sequence
+from importlib import resources
 from typing import IO, Any
 
 import yaml
 
 from .translator import MetadataTranslator
 from .translators import FitsTranslator
 
@@ -265,15 +265,15 @@
 
 def _read_yaml(fh: IO[bytes], msg: str) -> Mapping[str, Any] | None:
     """Read YAML from file descriptor.
 
     Parameters
     ----------
     fh : `io.IOBase`
-        Open file handle containing the YAML stream
+        Open file handle containing the YAML stream.
     msg : `str`
         Text to include in log file when referring to this stream. Examples
         could be "file something.yaml" or "resource module:resource".
 
     Returns
     -------
     parsed : `dict` or `None`
```

### Comparing `astro-metadata-translator-26.2024.900/python/astro_metadata_translator/indexing.py` & `astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/indexing.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,14 @@
     "process_sidecar_data",
 )
 
 import collections.abc
 import json
 import logging
 import os
-import sys
 from collections.abc import MutableMapping, Sequence
 from copy import deepcopy
 from typing import IO, Any, Literal, overload
 
 from .file_helpers import read_file_info
 from .headers import merge_headers
 from .observationGroup import ObservationGroup
@@ -44,16 +43,15 @@
 
 def index_files(
     files: Sequence[str],
     root: str | None,
     hdrnum: int,
     print_trace: bool,
     content: str,
-    outstream: IO = sys.stdout,
-    errstream: IO = sys.stderr,
+    outstream: IO | None = None,
 ) -> tuple[MutableMapping[str, str | MutableMapping[str, Any]], list[str], list[str]]:
     """Create an index from the supplied files.
 
     No file is written. The Python structure returned is suitable
     for writing.
 
     Parameters
@@ -63,29 +61,28 @@
         in a single directory but all content will be indexed into a single
         index.
     root : `str`
         Directory root that can be combined with each file (if the supplied)
         file is relative. Will be ignored if `None`.
     hdrnum : `int`
         The HDU number to read. The primary header is always read and
+        merged with the header from this HDU.
     print_trace : `bool`
         If there is an error reading the file and this parameter is `True`,
         a full traceback of the exception will be reported. If `False` prints
         a one line summary of the error condition. If `None` the exception
         will be allowed.
     content : `str`
         Form of data to write in index file. Options are:
         ``translated`` (default) to write ObservationInfo to the index;
         ``metadata`` to write native metadata headers to the index.
-        The index file is called ``{mode}_index.json``
+        The index file is called ``{mode}_index.json``.
     outstream : `io.StringIO`, optional
-        Output stream to use for standard messages. Defaults to `sys.stdout`.
-    errstream : `io.StringIO`, optional
-        Stream to send messages that would normally be sent to standard
-        error. Defaults to `sys.stderr`.
+        Output stream to use for standard messages. Defaults to `None` which
+        uses the default output stream.
 
     Returns
     -------
     file_index : `dict` of [`str`, `dict`]
         The headers in form suitable for writing to an index. The keys will
         be ``__COMMON__`` for shared content, ``__CONTENT_`` to record the
         content mode used to construct the index, and paths to the files. The
@@ -105,15 +102,15 @@
 
     content_by_file: MutableMapping[str, MutableMapping[str, Any]] = {}  # Mapping of path to file content
     for file in sorted(files):
         if root is not None:
             path = os.path.join(root, file)
         else:
             path = file
-        simple = read_file_info(path, hdrnum, print_trace, content, "simple", outstream, errstream)
+        simple = read_file_info(path, hdrnum, print_trace, content, "simple", outstream)
         if simple is None:
             failed.append(path)
             continue
         else:
             okay.append(path)
 
         # Store the information indexed by the filename within dir
@@ -187,25 +184,23 @@
 
 
 @overload
 def read_index(
     path: str,
     *,
     force_dict: Literal[True],
-) -> MutableMapping[str, MutableMapping[str, Any] | ObservationInfo]:
-    ...
+) -> MutableMapping[str, MutableMapping[str, Any] | ObservationInfo]: ...
 
 
 @overload
 def read_index(
     path: str,
     *,
     force_dict: Literal[False],
-) -> ObservationGroup | MutableMapping[str, MutableMapping[str, Any] | ObservationInfo]:
-    ...
+) -> ObservationGroup | MutableMapping[str, MutableMapping[str, Any] | ObservationInfo]: ...
 
 
 def read_index(
     path: str, force_dict: bool = False
 ) -> ObservationGroup | MutableMapping[str, MutableMapping[str, Any] | ObservationInfo]:
     """Read an index file.
 
@@ -237,33 +232,30 @@
 
 @overload
 def process_index_data(
     content: MutableMapping[str, Any],
     *,
     force_metadata: Literal[True],
     force_dict: Literal[False],
-) -> MutableMapping[str, Any]:
-    ...
+) -> MutableMapping[str, Any]: ...
 
 
 @overload
 def process_index_data(
     content: MutableMapping[str, Any],
     *,
     force_metadata: Literal[False],
     force_dict: Literal[True],
-) -> MutableMapping[str, MutableMapping[str, Any] | ObservationInfo]:
-    ...
+) -> MutableMapping[str, MutableMapping[str, Any] | ObservationInfo]: ...
 
 
 @overload
 def process_index_data(
     content: MutableMapping[str, Any], *, force_metadata: bool = False, force_dict: bool = False
-) -> ObservationGroup | MutableMapping[str, MutableMapping[str, Any] | ObservationInfo]:
-    ...
+) -> ObservationGroup | MutableMapping[str, MutableMapping[str, Any] | ObservationInfo]: ...
 
 
 def process_index_data(
     content: MutableMapping[str, Any], *, force_metadata: bool = False, force_dict: bool = False
 ) -> ObservationGroup | MutableMapping[str, MutableMapping[str, Any] | ObservationInfo]:
     """Process the content read from a JSON index file.
 
@@ -279,22 +271,22 @@
     force_dict : `bool`, optional
         If `True` the structure returned will always be a dict keyed
         by filename.
 
     Returns
     -------
     index : `.ObservationGroup` or `dict` of [`str`, `dict`]
-       If the index file referred to `.ObservationInfo` this will return
-       an `.ObservationGroup`, otherwise a `dict` will be returned with the
-       keys being paths to files and the values being the keys and values
-       stored in the index (with common information merged in). This
-       can be overridden using the ``force_metadata`` parameter. If
-       ``force_dict`` is `True` a `dict` will be returned with filename
-       keys even if the index file refers to `.ObservationInfo` (the values
-       will be `.ObservationInfo` unless ``force_metadata`` is `True`).
+        If the index file referred to `.ObservationInfo` this will return
+        an `.ObservationGroup`, otherwise a `dict` will be returned with the
+        keys being paths to files and the values being the keys and values
+        stored in the index (with common information merged in). This
+        can be overridden using the ``force_metadata`` parameter. If
+        ``force_dict`` is `True` a `dict` will be returned with filename
+        keys even if the index file refers to `.ObservationInfo` (the values
+        will be `.ObservationInfo` unless ``force_metadata`` is `True`).
 
     Notes
     -----
     File keys will be relative to the location of the index file.
     """
     if COMMON_KEY not in content:
         raise ValueError(f"No '{COMMON_KEY}' key found in dict. Does not look like an index data structure.")
@@ -359,30 +351,27 @@
 
     return process_sidecar_data(content)
 
 
 @overload
 def process_sidecar_data(
     content: MutableMapping[str, Any],
-) -> ObservationInfo | MutableMapping[str, Any]:
-    ...
+) -> ObservationInfo | MutableMapping[str, Any]: ...
 
 
 @overload
 def process_sidecar_data(
     content: MutableMapping[str, Any], force_metadata: Literal[True]
-) -> MutableMapping[str, Any]:
-    ...
+) -> MutableMapping[str, Any]: ...
 
 
 @overload
 def process_sidecar_data(
     content: MutableMapping[str, Any], force_metadata: Literal[False]
-) -> ObservationInfo | MutableMapping[str, Any]:
-    ...
+) -> ObservationInfo | MutableMapping[str, Any]: ...
 
 
 def process_sidecar_data(
     content: MutableMapping[str, Any], force_metadata: bool = False
 ) -> ObservationInfo | MutableMapping[str, Any]:
     """Process the content read from a JSON sidecar file.
```

### Comparing `astro-metadata-translator-26.2024.900/python/astro_metadata_translator/observationGroup.py` & `astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/observationGroup.py`

 * *Files 3% similar despite different names*

```diff
@@ -122,30 +122,41 @@
     def __iter__(self) -> Iterator[ObservationInfo]:
         return iter(self._members)
 
     def __eq__(self, other: Any) -> bool:
         """Check equality with another group.
 
         Compare equal if all the members are equal in the same order.
+
+        Parameters
+        ----------
+        other : `typing.Any`
+            Thing to compare with current group.
         """
         if not isinstance(other, ObservationGroup):
             return NotImplemented
 
         for info1, info2 in zip(self, other):
             if info1 != info2:
                 return False
         return True
 
     def __setitem__(  # type: ignore
         self, index: int, value: ObservationInfo | MutableMapping[str, Any]
     ) -> None:
         """Store item in group.
 
-        Item must be an `ObservationInfo` or something that can be passed
-        to an `ObservationInfo` constructor.
+        Parameters
+        ----------
+        index : `int`
+            Index to use to store the item.
+        value : `ObservationInfo` or `~collections.abc.MutableMapping`
+            Information to store in group. Item must be an `ObservationInfo`
+            or something that can be passed to an `ObservationInfo`
+            constructor.
         """
         value = self._coerce_value(value)
         self._members[index] = value
         self._sorted = None
 
     def insert(self, index: int, value: ObservationInfo | MutableMapping[str, Any]) -> None:
         value = self._coerce_value(value)
@@ -200,15 +211,15 @@
 
     def property_values(self, property: str) -> set[Any]:
         """Return a set of values associated with the specified property.
 
         Parameters
         ----------
         property : `str`
-            Property of an `ObservationInfo`
+            Property of an `ObservationInfo`.
 
         Returns
         -------
         values : `set`
             All the distinct values for that property within this group.
         """
         return {getattr(obs_info, property) for obs_info in self}
```

### Comparing `astro-metadata-translator-26.2024.900/python/astro_metadata_translator/observationInfo.py` & `astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/observationInfo.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,14 +133,15 @@
         altaz_begin: astropy.coordinates.AltAz
         science_program: str
         observation_counter: int
         observation_reason: str
         observation_type: str
         observation_id: str
         observing_day: int
+        observing_day_offset: astropy.time.TimeDelta | None
         group_counter_start: int
         group_counter_end: int
         has_simulated_content: bool
 
     def __init__(
         self,
         header: MutableMapping[str, Any] | None,
@@ -306,14 +307,21 @@
 
     def __setattr__(self, name: str, value: Any) -> Any:
         """Set attribute.
 
         This provides read-only protection for the extension properties. The
         core set of properties have read-only protection via the use of the
         python ``property``.
+
+        Parameters
+        ----------
+        name : `str`
+            Name of attribute to set.
+        value : `typing.Any`
+            Value to set it to.
         """
         if hasattr(self, "extensions") and name.startswith("ext_") and name[4:] in self.extensions:
             raise AttributeError(f"Attribute {name} is read-only")
         return super().__setattr__(name, value)
 
     @classmethod
     def _is_property_ok(cls, definition: PropertyDefinition, value: Any) -> bool:
@@ -396,14 +404,19 @@
 
         return result
 
     def __eq__(self, other: Any) -> bool:
         """Check equality with another object.
 
         Compares equal if standard properties are equal.
+
+        Parameters
+        ----------
+        other : `typing.Any`
+            Thing to compare with.
         """
         if not isinstance(other, ObservationInfo):
             return NotImplemented
 
         # Compare simplified forms.
         # Cannot compare directly because nan will not equate as equal
         # whereas they should be equal for our purposes
@@ -539,15 +552,15 @@
     def from_simple(cls, simple: MutableMapping[str, Any]) -> ObservationInfo:
         """Convert the entity returned by `to_simple` back into an
         `ObservationInfo`.
 
         Parameters
         ----------
         simple : `dict` [`str`, `~typing.Any`]
-            The dict returned by `to_simple()`
+            The dict returned by `to_simple()`.
 
         Returns
         -------
         obsinfo : `ObservationInfo`
             New object constructed from the dict.
 
         Notes
```

### Comparing `astro-metadata-translator-26.2024.900/python/astro_metadata_translator/properties.py` & `astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/properties.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 """Properties calculated by this package.
 
 Defines all properties in one place so that both `ObservationInfo` and
 `MetadataTranslator` can use them.  In particular, the translator
 base class can use knowledge of these properties to predefine translation
 stubs with documentation attached, and `ObservationInfo` can automatically
 define the getter methods.
-
 """
 from __future__ import annotations
 
 __all__ = (
     "PropertyDefinition",
     "PROPERTIES",
 )
@@ -54,15 +53,28 @@
         The geocentric location as three floats in meters.
     """
     geocentric = location.to_geocentric()
     return tuple(c.to_value(astropy.units.m) for c in geocentric)
 
 
 def simple_to_earthlocation(simple: tuple[float, ...], **kwargs: Any) -> astropy.coordinates.EarthLocation:
-    """Convert simple form back to EarthLocation."""
+    """Convert simple form back to EarthLocation.
+
+    Parameters
+    ----------
+    simple : `tuple` [`float`, ...]
+        The geocentric location as three floats in meters.
+    **kwargs : `typing.Any`
+        Keyword arguments. Currently not used.
+
+    Returns
+    -------
+    loc : `astropy.coordinates.EarthLocation`
+        The location on the Earth.
+    """
     return astropy.coordinates.EarthLocation.from_geocentric(*simple, unit=astropy.units.m)
 
 
 def datetime_to_simple(datetime: astropy.time.Time) -> tuple[float, float]:
     """Convert Time to tuple.
 
     Parameters
@@ -76,101 +88,316 @@
         The two MJDs in TAI.
     """
     tai = datetime.tai
     return (tai.jd1, tai.jd2)
 
 
 def simple_to_datetime(simple: tuple[float, float], **kwargs: Any) -> astropy.time.Time:
-    """Convert simple form back to astropy.time.Time."""
+    """Convert simple form back to `astropy.time.Time`.
+
+    Parameters
+    ----------
+    simple : `tuple` [`float`, `float`]
+        The time represented by two MJDs.
+    **kwargs : `typing.Any`
+        Keyword arguments. Currently not used.
+
+    Returns
+    -------
+    t : `astropy.time.Time`
+        An astropy time object.
+    """
     return astropy.time.Time(*simple, format="jd", scale="tai")
 
 
 def exptime_to_simple(exptime: astropy.units.Quantity) -> float:
-    """Convert exposure time Quantity to seconds."""
+    """Convert exposure time Quantity to seconds.
+
+    Parameters
+    ----------
+    exptime : `astropy.units.Quantity`
+        The exposure time as a quantity.
+
+    Returns
+    -------
+    e : `float`
+        Exposure time in seconds.
+    """
     return exptime.to_value(astropy.units.s)
 
 
 def simple_to_exptime(simple: float, **kwargs: Any) -> astropy.units.Quantity:
-    """Convert simple form back to Quantity."""
+    """Convert simple form back to Quantity.
+
+    Parameters
+    ----------
+    simple : `float`
+        Exposure time in seconds.
+    **kwargs : `typing.Any`
+        Keyword arguments. Currently not used.
+
+    Returns
+    -------
+    q : `astropy.units.Quantity`
+        The exposure time as a quantity.
+    """
     return simple * astropy.units.s
 
 
 def angle_to_simple(angle: astropy.coordinates.Angle) -> float:
-    """Convert Angle to degrees."""
+    """Convert Angle to degrees.
+
+    Parameters
+    ----------
+    angle : `astropy.coordinates.Angle`
+        The angle.
+
+    Returns
+    -------
+    a : `float`
+        The angle in degrees.
+    """
     return angle.to_value(astropy.units.deg)
 
 
 def simple_to_angle(simple: float, **kwargs: Any) -> astropy.coordinates.Angle:
-    """Convert degrees to Angle."""
+    """Convert degrees to Angle.
+
+    Parameters
+    ----------
+    simple : `float`
+        The angle in degrees.
+    **kwargs : `typing.Any`
+        Keyword arguments. Currently not used.
+
+    Returns
+    -------
+    a : `astropy.coordinates.Angle`
+        The angle as an object.
+    """
     return astropy.coordinates.Angle(simple * astropy.units.deg)
 
 
 def focusz_to_simple(focusz: astropy.units.Quantity) -> float:
-    """Convert focusz to meters."""
+    """Convert focusz to meters.
+
+    Parameters
+    ----------
+    focusz : `astropy.units.Quantity`
+        The z-focus as a quantity.
+
+    Returns
+    -------
+    f : `float`
+        The z-focus in meters.
+    """
     return focusz.to_value(astropy.units.m)
 
 
 def simple_to_focusz(simple: float, **kwargs: Any) -> astropy.units.Quantity:
-    """Convert simple form back to Quantity."""
+    """Convert simple form back to Quantity.
+
+    Parameters
+    ----------
+    simple : `float`
+        The z-focus in meters.
+    **kwargs : `typing.Any`
+        Keyword arguments. Currently not used.
+
+    Returns
+    -------
+    q : `astropy.units.Quantity`
+        The z-focus as a quantity.
+    """
     return simple * astropy.units.m
 
 
 def temperature_to_simple(temp: astropy.units.Quantity) -> float:
-    """Convert temperature to kelvin."""
+    """Convert temperature to kelvin.
+
+    Parameters
+    ----------
+    temp : `astropy.units.Quantity`
+        The temperature as a quantity.
+
+    Returns
+    -------
+    t : `float`
+        The temperature in kelvin.
+    """
     return temp.to(astropy.units.K, equivalencies=astropy.units.temperature()).to_value()
 
 
 def simple_to_temperature(simple: float, **kwargs: Any) -> astropy.units.Quantity:
-    """Convert scalar kelvin value back to quantity."""
+    """Convert scalar kelvin value back to quantity.
+
+    Parameters
+    ----------
+    simple : `float`
+        Temperature as a float in units of kelvin.
+    **kwargs : `typing.Any`
+        Keyword arguments. Currently not used.
+
+    Returns
+    -------
+    q : `astropy.units.Quantity`
+        The temperature as a quantity.
+    """
     return simple * astropy.units.K
 
 
 def pressure_to_simple(press: astropy.units.Quantity) -> float:
-    """Convert pressure Quantity to hPa."""
+    """Convert pressure Quantity to hPa.
+
+    Parameters
+    ----------
+    press : `astropy.units.Quantity`
+        The pressure as a quantity.
+
+    Returns
+    -------
+    hpa : `float`
+        The pressure in units of hPa.
+    """
     return press.to_value(astropy.units.hPa)
 
 
 def simple_to_pressure(simple: float, **kwargs: Any) -> astropy.units.Quantity:
-    """Convert the pressure scalar back to Quantity."""
+    """Convert the pressure scalar back to Quantity.
+
+    Parameters
+    ----------
+    simple : `float`
+        Pressure in units of hPa.
+    **kwargs : `typing.Any`
+        Keyword arguments. Currently not used.
+
+    Returns
+    -------
+    q : `astropy.units.Quantity`
+        The pressure as a quantity.
+    """
     return simple * astropy.units.hPa
 
 
 def skycoord_to_simple(skycoord: astropy.coordinates.SkyCoord) -> tuple[float, float]:
-    """Convert SkyCoord to ICRS RA/Dec tuple."""
+    """Convert SkyCoord to ICRS RA/Dec tuple.
+
+    Parameters
+    ----------
+    skycoord : `astropy.coordinates.SkyCoord`
+        Sky coordinates in astropy form.
+
+    Returns
+    -------
+    simple : `tuple` [`float`, `float`]
+        Sky coordinates as a tuple of two floats in units of degrees.
+    """
     icrs = skycoord.icrs
     return (icrs.ra.to_value(astropy.units.deg), icrs.dec.to_value(astropy.units.deg))
 
 
 def simple_to_skycoord(simple: tuple[float, float], **kwargs: Any) -> astropy.coordinates.SkyCoord:
-    """Convert ICRS tuple to SkyCoord."""
+    """Convert ICRS tuple to SkyCoord.
+
+    Parameters
+    ----------
+    simple : `tuple` [`float`, `float`]
+        Sky coordinates in degrees.
+    **kwargs : `typing.Any`
+        Keyword arguments. Currently not used.
+
+    Returns
+    -------
+    skycoord : `astropy.coordinates.SkyCoord`
+        The sky coordinates in astropy form.
+    """
     return astropy.coordinates.SkyCoord(*simple, unit=astropy.units.deg)
 
 
 def altaz_to_simple(altaz: astropy.coordinates.AltAz) -> tuple[float, float]:
     """Convert AltAz to Alt/Az tuple.
 
     Do not include obstime or location in simplification. It is assumed
     that those will be present from other properties.
+
+    Parameters
+    ----------
+    altaz : `astropy.coordinates.AltAz`
+        The alt/az in astropy form.
+
+    Returns
+    -------
+    simple : `tuple` [`float`, `float`]
+        The Alt/Az as a tuple of two floats representing the position in
+        units of degrees.
     """
     return (altaz.az.to_value(astropy.units.deg), altaz.alt.to_value(astropy.units.deg))
 
 
 def simple_to_altaz(simple: tuple[float, float], **kwargs: Any) -> astropy.coordinates.AltAz:
     """Convert simple altaz tuple to AltAz.
 
-    Will look for location and datetime_begin in kwargs.
+    Parameters
+    ----------
+    simple : `tuple` [`float`, `float`]
+        Altitude and elevation in degrees.
+    **kwargs : `dict`
+        Additional information. Must contain ``location`` and
+        ``datetime_begin``.
+
+    Returns
+    -------
+    altaz : `astropy.coordinates.AltAz`
+        The altaz in astropy form.
     """
     location = kwargs.get("location")
     obstime = kwargs.get("datetime_begin")
 
     return astropy.coordinates.AltAz(
         simple[0] * astropy.units.deg, simple[1] * astropy.units.deg, obstime=obstime, location=location
     )
 
 
+def timedelta_to_simple(delta: astropy.time.TimeDelta) -> int:
+    """Convert a TimeDelta to integer seconds.
+
+    This property does not need to support floating point seconds.
+
+    Parameters
+    ----------
+    delta : `astropy.time.TimeDelta`
+        The time offset.
+
+    Returns
+    -------
+    sec : `int`
+        Offset in integer seconds.
+    """
+    return round(delta.to_value("s"))
+
+
+def simple_to_timedelta(simple: int, **kwargs: Any) -> astropy.time.TimeDelta:
+    """Convert integer seconds to a `~astropy.time.TimeDelta`.
+
+    Parameters
+    ----------
+    simple : `int`
+        The offset in integer seconds.
+    **kwargs : `dict`
+        Additional information. Unused.
+
+    Returns
+    -------
+    delta : `astropy.time.TimeDelta`
+        The delta object.
+    """
+    return astropy.time.TimeDelta(simple, format="sec", scale="tai")
+
+
 @dataclass
 class PropertyDefinition:
     """Definition of an instrumental property."""
 
     doc: str
     """Docstring for the property."""
 
@@ -342,14 +569,24 @@
         "Label to use to associate this exposure with others (can be related to 'exposure_id').",
         "str",
         str,
     ),
     "observing_day": PropertyDefinition(
         "Integer in YYYYMMDD format corresponding to the day of observation.", "int", int
     ),
+    "observing_day_offset": PropertyDefinition(
+        (
+            "Offset to subtract from an observation date when calculating the observing day. "
+            "Conversely, the offset to add to an observing day when calculating the time span of a day."
+        ),
+        "astropy.time.TimeDelta",
+        astropy.time.TimeDelta,
+        timedelta_to_simple,
+        simple_to_timedelta,
+    ),
     "observation_counter": PropertyDefinition(
         (
             "Counter of this observation. Can be counter within observing_day or a global counter. "
             "Likely to be observatory specific."
         ),
         "int",
         int,
@@ -371,8 +608,15 @@
         "Depending on the instrument the relevant group may be "
         "visit_id or exposure_group.",
         "int",
         int,
         None,
         None,
     ),
+    "can_see_sky": PropertyDefinition(
+        "True if the observation is looking at sky, False if it is definitely"
+        " not looking at the sky. None indicates that it is not known whether"
+        " sky could be seen.",
+        "bool",
+        bool,
+    ),
 }
```

### Comparing `astro-metadata-translator-26.2024.900/python/astro_metadata_translator/serialize/fits.py` & `astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/serialize/fits.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 def dates_to_fits(date_begin: astropy.time.Time, date_end: astropy.time.Time) -> dict[str, Any]:
     """Convert two dates into FITS form.
 
     Parameters
     ----------
     date_begin : `astropy.time.Time`
         Date representing the beginning of the observation.
-    date_end  : `astropy.time.Time`
+    date_end : `astropy.time.Time`
         Date representing the end of the observation.
 
     Returns
     -------
     cards : `dict` of `str` to `str` or `float`
         Header card keys and values following the FITS standard.
         If neither date is defined this may be empty.
```

### Comparing `astro-metadata-translator-26.2024.900/python/astro_metadata_translator/tests.py` & `astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/tests.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from collections.abc import MutableMapping
 from typing import TYPE_CHECKING, Any, NoReturn
 
 import astropy.units as u
 import astropy.utils.exceptions
 import yaml
 from astropy.io.fits import Header
+from astropy.io.fits.verify import VerifyWarning
 from astropy.time import Time
 
 from astro_metadata_translator import ObservationInfo
 
 # PropertyList is optional
 try:
     import lsst.daf.base as daf_base
@@ -42,15 +43,28 @@
 except AttributeError:
     Loader = yaml.Loader
 
 
 # Define a YAML loader for lsst.daf.base.PropertySet serializations that
 # we can use if daf_base is not available.
 def pl_constructor(loader: yaml.Loader, node: yaml.SequenceNode) -> Any:
-    """Construct an OrderedDict from a YAML file containing a PropertyList."""
+    """Construct an OrderedDict from a YAML file containing a PropertyList.
+
+    Parameters
+    ----------
+    loader : `yaml.Loader`
+        Instance used to load YAML file.
+    node : `yaml.SequenceNode`
+        Node to examine.
+
+    Yields
+    ------
+    pl : `dict`
+        Contents of PropertyList as a dict.
+    """
     pl: dict[str, Any] = {}
     yield pl
     state = loader.construct_sequence(node, deep=True)
     for key, dtype, value, comment in state:
         if dtype == "Double":
             pl[key] = float(value)
         elif dtype == "Int":
@@ -68,15 +82,15 @@
 def read_test_file(filename: str, dir: str | None = None) -> MutableMapping[str, Any]:
     """Read the named test file relative to the location of this helper.
 
     Parameters
     ----------
     filename : `str`
         Name of file in the data directory.
-    dir : `str`, optional.
+    dir : `str`, optional
         Directory from which to read file. Current directory used if none
         specified.
 
     Returns
     -------
     header : `dict`-like
         Header read from file.
@@ -147,23 +161,28 @@
             Max difference between header airmass and derived airmass.
 
         Raises
         ------
         AssertionError
             Inconsistencies found.
         """
-        self.assertIsNotNone(obsinfo.tracking_radec)
-        self.assertIsNotNone(obsinfo.altaz_begin)
+        self.assertIsNotNone(obsinfo.tracking_radec, msg="Checking tracking_radec is defined")
+        self.assertIsNotNone(obsinfo.altaz_begin, msg="Checking AltAz is defined")
 
         # Is airmass from header close to airmass from AltAz headers?
         # In most cases there is uncertainty over whether the elevation
         # and airmass in the header are for the start, end, or middle
         # of the observation.  Sometimes the AltAz is from the start
         # but the airmass is from the middle so accuracy is not certain.
-        self.assertAlmostEqual(obsinfo.altaz_begin.secz.to_value(), obsinfo.boresight_airmass, delta=amdelta)
+        self.assertAlmostEqual(
+            obsinfo.altaz_begin.secz.to_value(),
+            obsinfo.boresight_airmass,
+            delta=amdelta,
+            msg="Checking airmass is consistent",
+        )
 
         # Is AltAz from headers close to AltAz from RA/Dec headers?
         # Can trigger warnings from Astropy if date is in future
         with warnings.catch_warnings():
             warnings.simplefilter("ignore", category=astropy.utils.exceptions.AstropyWarning)
             sep = obsinfo.altaz_begin.separation(obsinfo.tracking_radec.altaz)
         self.assertLess(sep.to_value(unit="arcmin"), max_sep, msg="AltAz inconsistent with RA/Dec")
@@ -187,15 +206,15 @@
             Optional directory from which to read ``file``.
         check_wcs : `bool`, optional
             Check the consistency of the RA/Dec and AltAz values.
         wcs_params : `dict`, optional
             Parameters to pass to `assertCoordinatesConsistent`.
         check_altaz : `bool`, optional
             Check that an alt/az value has been calculated.
-        kwargs : `dict`
+        **kwargs : `dict`
             Keys matching `ObservationInfo` properties with values
             to be tested.
 
         Raises
         ------
         AssertionError
             A value in the ObservationInfo derived from the file is
@@ -204,16 +223,21 @@
         header = read_test_file(file, dir=dir)
 
         # DM-30093: Astropy Header does not always behave dict-like
         astropy_header = Header()
         for key, val in header.items():
             values = val if isinstance(val, list) else [val]
             for v in values:
-                # appending ensures *all* duplicated keys are also preserved
-                astropy_header.append((key, v))
+                # Appending ensures *all* duplicated keys are also preserved.
+                # astropy.io.fits complains about long keywords rather than
+                # letting us say "thank you for using the standard to let
+                # us write this header" so we need to catch the warnings.
+                with warnings.catch_warnings():
+                    warnings.simplefilter("ignore", category=VerifyWarning)
+                    astropy_header.append((key, v))
 
         for hdr in (header, astropy_header):
             try:
                 self.assertObservationInfo(
                     header,
                     filename=file,
                     check_wcs=check_wcs,
@@ -247,15 +271,15 @@
             Check the consistency of the RA/Dec and AltAz values.  Checks
             are automatically disabled if the translated header does
             not appear to be "science".
         wcs_params : `dict`, optional
             Parameters to pass to `assertCoordinatesConsistent`.
         check_altaz : `bool`, optional
             Check that an alt/az value has been calculated.
-        kwargs : `dict`
+        **kwargs : `dict`
             Keys matching `ObservationInfo` properties with values
             to be tested.
 
         Raises
         ------
         AssertionError
             A value in the ObservationInfo derived from the file is
```

### Comparing `astro-metadata-translator-26.2024.900/python/astro_metadata_translator/translator.py` & `astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/translator.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,28 +15,29 @@
 
 __all__ = ("MetadataTranslator", "StubTranslator", "cache_translation")
 
 import importlib
 import inspect
 import logging
 import math
+import numbers
 import warnings
 from abc import abstractmethod
 from collections.abc import Callable, Iterable, Iterator, Mapping, MutableMapping, Sequence
 from typing import TYPE_CHECKING, Any, ClassVar
 
 import astropy.io.fits.card
+import astropy.time
 import astropy.units as u
 from astropy.coordinates import Angle
 
 from .properties import PROPERTIES, PropertyDefinition
 
 if TYPE_CHECKING:
     import astropy.coordinates
-    import astropy.time
 
 log = logging.getLogger(__name__)
 
 # Location of the root of the corrections resource files
 CORRECTIONS_RESOURCE_ROOT = "corrections"
 
 """Cache of version strings indexed by class."""
@@ -136,14 +137,24 @@
     way as the standard set, except that their names will everywhere be
     prefixed with ``ext_``.
 
     Each property is indexed by name (`str`), with a corresponding
     `PropertyDefinition`.
     """
 
+    _sky_observation_types: tuple[str, ...] = ("science", "object")
+    """Observation types that correspond to an observation where the detector
+    can see sky photons.  This is used by the default implementation of
+    ``can_see_sky`` determination."""
+
+    _non_sky_observation_types: tuple[str, ...] = ("bias", "dark")
+    """Observation types that correspond to an observation where the detector
+    can not see sky photons.  This is used by the default implementation of
+    ``can_see_sky`` determination."""
+
     # Static typing requires that we define the standard dynamic properties
     # statically.
     if TYPE_CHECKING:
         to_telescope: ClassVar[Callable[[MetadataTranslator], str]]
         to_instrument: ClassVar[Callable[[MetadataTranslator], str]]
         to_location: ClassVar[Callable[[MetadataTranslator], astropy.coordinates.EarthLocation]]
         to_exposure_id: ClassVar[Callable[[MetadataTranslator], int]]
@@ -391,14 +402,19 @@
         provide a full ``to_property()`` translation method the mapping can be
         defined in a class variable named ``_constMap``.  Similarly, for
         one-to-one trivial mappings from a header to a property,
         ``_trivialMap`` can be defined.  Trivial mappings are a dict mapping a
         generic property to either a header keyword, or a tuple consisting of
         the header keyword and a dict containing key value pairs suitable for
         the `MetadataTranslator.quantity_from_card` method.
+
+        Parameters
+        ----------
+        **kwargs : `dict`
+            Arbitrary parameters passed to parent class.
         """
         super().__init_subclass__(**kwargs)
 
         # Only register classes with declared names
         if hasattr(cls, "name") and cls.name is not None:
             if cls.name in MetadataTranslator.translators:
                 log.warning(
@@ -440,15 +456,15 @@
         cls.all_properties = dict(PROPERTIES)
         cls.all_properties.update(cls.extensions)
 
         # Go through the trival mappings for this class and create
         # corresponding translator methods
         for property_key, header_key in trivial_map.items():
             kwargs = {}
-            if type(header_key) == tuple:
+            if type(header_key) is tuple:
                 kwargs = header_key[1]
                 header_key = header_key[0]
             translator = cls._make_trivial_mapping(property_key, header_key, **kwargs)
             method = f"to_{property_key}"
             translator.__name__ = f"{method}_trivial_in_{cls.__name__}"
             setattr(cls, method, cache_translation(translator, method=method))
             if property_key not in properties:
@@ -560,19 +576,19 @@
         file_msg = ""
         if filename is not None:
             file_msg = f" from {filename}"
         for name, trans in cls.translators.items():
             if trans.can_translate(header, filename=filename):
                 log.debug("Using translation class %s%s", name, file_msg)
                 return trans
-        else:
-            raise ValueError(
-                f"None of the registered translation classes {list(cls.translators.keys())}"
-                f" understood this header{file_msg}"
-            )
+
+        raise ValueError(
+            f"None of the registered translation classes {list(cls.translators.keys())}"
+            f" understood this header{file_msg}"
+        )
 
     @classmethod
     def translator_version(cls) -> str:
         """Return the version string for this translator class.
 
         Returns
         -------
@@ -698,15 +714,15 @@
         return self._log_prefix_cache
 
     def _used_these_cards(self, *args: str) -> None:
         """Indicate that the supplied cards have been used for translation.
 
         Parameters
         ----------
-        args : sequence of `str`
+        *args : sequence of `str`
             Keywords used to process a translation.
         """
         self._used_cards.update(set(args))
 
     def cards_used(self) -> frozenset[str]:
         """Cards used during metadata extraction.
 
@@ -1015,33 +1031,125 @@
             The reason for this observation.
         """
         obstype = self.to_observation_type()
         if obstype == "science":
             return "science"
         return "unknown"
 
+    @classmethod
+    def observing_date_to_offset(cls, observing_date: astropy.time.Time) -> astropy.time.TimeDelta | None:
+        """Calculate the observing day offset to apply for a given observation.
+
+        In some cases the definition of the observing day offset has changed
+        during the lifetime of the instrument. For example lab data might
+        have a different offset to that when the instrument is on the
+        telescope.
+
+        Parameters
+        ----------
+        observing_date : `astropy.time.Time`
+            The observation date.
+
+        Returns
+        -------
+        offset : `astropy.time.TimeDelta` or `None`
+            The offset to apply when calculating the observing day for a
+            specific time of observation. `None` implies the offset
+            is not known for that date.
+        """
+        return None
+
+    @classmethod
+    def observing_date_to_observing_day(
+        cls, observing_date: astropy.time.Time, offset: astropy.time.TimeDelta | int | None
+    ) -> int:
+        """Return the YYYYMMDD integer corresponding to the observing day.
+
+        The offset is subtracted from the time of observation before
+        calculating the year, month and day.
+
+        Parameters
+        ----------
+        observing_date : `astropy.time.Time`
+            The observation date.
+        offset : `astropy.time.TimeDelta` | `numbers.Real` | None
+            The offset to subtract from the observing date when calculating
+            the observing day. If a plain number is given it is taken to be
+            in units of seconds. If `None` no offset is applied.
+
+        Returns
+        -------
+        day : `int`
+            The observing day as an integer of form YYYYMMDD.
+
+        Notes
+        -----
+        For example, if the offset is +12 hours both 2023-07-06T13:00 and
+        2023-07-07T11:00 will return an observing day of 20230706 because
+        the observing day goes from 2023-07-06T12:00 to 2023-07-07T12:00.
+        """
+        observing_date = observing_date.tai
+        if offset:
+            if isinstance(offset, numbers.Real):
+                offset = astropy.time.TimeDelta(offset, format="sec", scale="tai")
+            observing_date -= offset
+        return int(observing_date.strftime("%Y%m%d"))
+
+    @cache_translation
+    def to_observing_day_offset(self) -> astropy.time.TimeDelta | None:
+        """Return the offset required to calculate observing day.
+
+        Base class implementation returns `None`.
+
+        Returns
+        -------
+        offset : `astropy.time.TimeDelta` or `None`
+            The offset to apply. Returns `None` if the offset is not defined.
+
+        Notes
+        -----
+        This offset must be subtracted from a time of observation to calculate
+        the observing day. This offset must be added to the YYYYMMDDT00:00
+        observing day to calculate the time span coverage of the observing day.
+        """
+        datetime_begin = self.to_datetime_begin()
+        if datetime_begin is None:
+            return None
+        return self.observing_date_to_offset(datetime_begin)
+
     @cache_translation
     def to_observing_day(self) -> int:
         """Return the YYYYMMDD integer corresponding to the observing day.
 
         Base class implementation uses the TAI date of the start of the
-        observation.
+        observation corrected by the observing day offset. If that offset
+        is `None` no offset will be applied.
+
+        The offset is subtracted from the time of observation before
+        calculating the year, month and day.
 
         Returns
         -------
         day : `int`
             The observing day as an integer of form YYYYMMDD. If the header
             is broken and is unable to obtain a date of observation, ``0``
             is returned and the assumption is made that the problem will
             be caught elsewhere.
+
+        Notes
+        -----
+        For example, if the offset is +12 hours both 2023-07-06T13:00 and
+        2023-07-07T11:00 will return an observing day of 20230706 because
+        the observing day goes from 2023-07-06T12:00 to 2023-07-07T12:00.
         """
         datetime_begin = self.to_datetime_begin()
         if datetime_begin is None:
             return 0
-        return int(datetime_begin.tai.strftime("%Y%m%d"))
+        offset = self.to_observing_day_offset()
+        return self.observing_date_to_observing_day(datetime_begin.tai, offset)
 
     @cache_translation
     def to_observation_counter(self) -> int:
         """Return an integer corresponding to how this observation relates
         to other observations.
 
         Base class implementation returns ``0`` to indicate that it is not
@@ -1116,18 +1224,47 @@
         """Return a default defocal distance of 0.0 mm if there is no
         keyword for defocal distance in the header. The default
         keyword for defocal distance is ``FOCUSZ``.
 
         Returns
         -------
         focus_z: `astropy.units.Quantity`
-            The defocal distance from header or the 0.0mm default
+            The defocal distance from header or the 0.0mm default.
         """
         return 0.0 * u.mm
 
+    @cache_translation
+    def to_can_see_sky(self) -> bool | None:
+        """Return whether the observation can see the sky or not.
+
+        Returns
+        -------
+        can_see_sky : `bool` or `None`
+            `True` if the detector is receiving photons from the sky.
+            `False` if the sky is not visible to the detector.
+            `None` if the metadata translator does not know one way or the
+            other.
+
+        Notes
+        -----
+        The base class translator uses a simple heuristic of returning
+        `True` if the observation type is "science" or "object" and `False`
+        if the observation type is "bias" or "dark". For all other cases it
+        will return `None`.
+        """
+        obs_type = self.to_observation_type()
+        if obs_type is not None:
+            obs_type = obs_type.lower()
+
+        if obs_type in self._sky_observation_types:
+            return True
+        if obs_type in self._non_sky_observation_types:
+            return False
+        return None
+
     @classmethod
     def determine_translatable_headers(
         cls, filename: str, primary: MutableMapping[str, Any] | None = None
     ) -> Iterator[MutableMapping[str, Any]]:
         """Given a file return all the headers usable for metadata translation.
 
         This method can optionally be given a header from the file.  This
@@ -1263,29 +1400,28 @@
     """Translator where all the translations are stubbed out and issue
     warnings.
 
     This translator can be used as a base class whilst developing a new
     translator.  It allows testing to proceed without being required to fully
     define all translation methods.  Once complete the class should be
     removed from the inheritance tree.
-
     """
 
     pass
 
 
 def _make_forwarded_stub_translator_method(
-    cls: type[MetadataTranslator], property: str, doc: str, return_typedoc: str, return_type: type
+    cls_: type[MetadataTranslator], property: str, doc: str, return_typedoc: str, return_type: type
 ) -> Callable:
     """Create a stub translation method for this property that calls the
     base method and catches `NotImplementedError`.
 
     Parameters
     ----------
-    cls : `type`
+    cls_ : `type`
         Class to use when referencing `super()`.  This would usually be
         `StubTranslator`.
     property : `str`
         Name of the translator for property to be created.
     doc : `str`
         Description of the property.
     return_typedoc : `str`
@@ -1297,15 +1433,15 @@
     -------
     m : `~collections.abc.Callable`
         Stub translator method for this property.
     """
     method = f"to_{property}"
 
     def to_stub(self: MetadataTranslator) -> Any:
-        parent = getattr(super(cls, self), method, None)
+        parent = getattr(super(cls_, self), method, None)
         try:
             if parent is not None:
                 return parent()
         except NotImplementedError:
             pass
 
         warnings.warn(
```

### Comparing `astro-metadata-translator-26.2024.900/python/astro_metadata_translator/translators/__init__.py` & `astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/translators/__init__.py`

 * *Files identical despite different names*

### Comparing `astro-metadata-translator-26.2024.900/python/astro_metadata_translator/translators/decam.py` & `astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/translators/decam.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,25 +17,25 @@
 
 import logging
 import posixpath
 import re
 from collections.abc import Iterator, Mapping, MutableMapping
 from typing import TYPE_CHECKING, Any
 
+import astropy.time
 import astropy.units as u
 from astropy.coordinates import Angle, EarthLocation
 from astropy.io import fits
 
 from ..translator import CORRECTIONS_RESOURCE_ROOT, cache_translation
 from .fits import FitsTranslator
 from .helpers import altaz_from_degree_headers, is_non_science, tracking_from_degree_headers
 
 if TYPE_CHECKING:
     import astropy.coordinates
-    import astropy.time
 
 log = logging.getLogger(__name__)
 
 
 class DecamTranslator(FitsTranslator):
     """Metadata translator for DECam standard headers."""
 
@@ -71,14 +71,23 @@
         "relative_humidity": ("HUMIDITY", dict(default=40.0, minimum=0, maximum=100.0)),
         "temperature": ("OUTTEMP", dict(unit=u.deg_C, default=10.0, minimum=-10.0, maximum=40.0)),
         # Header says torr but seems to be mbar. Use hPa unit
         # which is the SI equivalent of mbar.
         "pressure": ("PRESSURE", dict(unit=u.hPa, default=771.611, minimum=700.0, maximum=850.0)),
     }
 
+    # DECam has no formal concept of an observing day. To ensure that
+    # observations from a single night all have the same observing_day, adopt
+    # the same offset used by the Vera Rubin Observatory of 12 hours.
+    _observing_day_offset = astropy.time.TimeDelta(12 * 3600, format="sec", scale="tai")
+
+    # List from Frank Valdes (2024-03-21).
+    _sky_observation_types: tuple[str, ...] = ("science", "object", "standard", "sky flat")
+    _non_sky_observation_types: tuple[str, ...] = ("zero", "dark", "dome flat")
+
     # Unique detector names are currently not used but are read directly from
     # header.
     # The detector_group could be N or S with detector_name corresponding
     # to the number in that group.
     detector_names = {
         1: "S29",
         2: "S30",
@@ -212,14 +221,24 @@
         return datetime_end
 
     def _translate_from_calib_id(self, field: str) -> str:
         """Fetch the ID from the CALIB_ID header.
 
         Calibration products made with constructCalibs have some metadata
         saved in its FITS header CALIB_ID.
+
+        Parameters
+        ----------
+        field : `str`
+            Field to extract from the ``CALIB_ID`` header.
+
+        Returns
+        -------
+        value : `str`
+            The value extracted from the calibration header for that field.
         """
         data = self._header["CALIB_ID"]
         match = re.search(r".*%s=(\S+)" % field, data)
         if not match:
             raise RuntimeError(f"Header CALIB_ID with value '{data}' has not field '{field}'")
         self._used_these_cards("CALIB_ID")
         return match.groups()[0]
@@ -432,7 +451,27 @@
 
                 header = hdu.header
                 if "CCDNUM" not in header:  # Primary does not have CCDNUM
                     continue
                 if header["CCDNUM"] > 62:  # ignore guide CCDs
                     continue
                 yield merge_headers([primary_hdr, header], mode="overwrite")
+
+    @classmethod
+    def observing_date_to_offset(cls, observing_date: astropy.time.Time) -> astropy.time.TimeDelta | None:
+        """Return the offset to use when calculating the observing day.
+
+        Parameters
+        ----------
+        observing_date : `astropy.time.Time`
+            The date of the observation. Unused.
+
+        Returns
+        -------
+        offset : `astropy.time.TimeDelta`
+            The offset to apply. The offset is always 12 hours. DECam has
+            no defined observing day concept in its headers. To ensure that
+            observations from a single night all have the same observing_day,
+            adopt the same offset used by the Vera Rubin Observatory of
+            12 hours.
+        """
+        return cls._observing_day_offset
```

### Comparing `astro-metadata-translator-26.2024.900/python/astro_metadata_translator/translators/fits.py` & `astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/translators/fits.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 
     Understands:
 
     - DATE-OBS/MJD-OBS or DATE-BEG/MJD-BEG (-BEG is preferred).
     - INSTRUME
     - TELESCOP
     - OBSGEO-[X,Y,Z]
-
     """
 
     # Direct translation from header key to standard form
     _trivial_map: dict[str, str | list[str] | tuple[Any, ...]] = dict(
         instrument="INSTRUME",
         telescope="TELESCOP",
     )
```

### Comparing `astro-metadata-translator-26.2024.900/python/astro_metadata_translator/translators/helpers.py` & `astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/translators/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 They are written as free functions.  Some of them are written
 as if they are methods of `MetadataTranslator`, allowing them to be attached
 to translator classes that need them.  These methods have full access to
 the translator methods.
 
 Other functions are pure helpers that can be imported and used to help
 translation classes without using `MetadataTranslator` properties.
-
 """
 
 from __future__ import annotations
 
 __all__ = (
     "to_location_via_telescope_name",
     "is_non_science",
@@ -63,15 +62,14 @@
     Raises
     ------
     KeyError
         Is a science observation.
     """
     if self.to_observation_type() == "science":
         raise KeyError(f"{self._log_prefix}: Header represents science observation and can not default")
-    return
 
 
 def altitude_from_zenith_distance(zd: astropy.units.Quantity) -> astropy.units.Quantity:
     """Convert zenith distance to altitude.
 
     Parameters
     ----------
```

### Comparing `astro-metadata-translator-26.2024.900/python/astro_metadata_translator/translators/hsc.py` & `astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/translators/hsc.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,14 +46,26 @@
     """Hard wire HSC even though modern headers call it Hyper Suprime-Cam"""
 
     _trivial_map = {
         "detector_serial": "T_CCDSN",
     }
     """One-to-one mappings"""
 
+    # List from Hisanori Furusawa (2024-03-25).
+    _sky_observation_types: tuple[str, ...] = (
+        "science",
+        "object",
+        "standard_star",
+        "skyflat",
+        "focus",
+        "focusing",
+        "exp",
+    )
+    _non_sky_observation_types: tuple[str, ...] = ("dark", "bias", "agexp", "domeflat")
+
     # Zero point for HSC dates: 2012-01-01  51544 -> 2000-01-01
     _DAY0 = 55927
 
     # CCD index mapping for commissioning run 2
     _CCD_MAP_COMMISSIONING_2 = {
         112: 106,
         107: 105,
```

### Comparing `astro-metadata-translator-26.2024.900/python/astro_metadata_translator/translators/megaprime.py` & `astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/translators/megaprime.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,25 +16,25 @@
 __all__ = ("MegaPrimeTranslator",)
 
 import posixpath
 import re
 from collections.abc import Iterator, MutableMapping
 from typing import TYPE_CHECKING, Any
 
+import astropy.time
 import astropy.units as u
 from astropy.coordinates import Angle, EarthLocation
 from astropy.io import fits
 
 from ..translator import CORRECTIONS_RESOURCE_ROOT, cache_translation
 from .fits import FitsTranslator
 from .helpers import altaz_from_degree_headers, tracking_from_degree_headers
 
 if TYPE_CHECKING:
     import astropy.coordinates
-    import astropy.time
     import astropy.units
 
 
 class MegaPrimeTranslator(FitsTranslator):
     """Metadata translator for CFHT MegaPrime standard headers."""
 
     name = "MegaPrime"
@@ -42,14 +42,16 @@
 
     supported_instrument = "MegaPrime"
     """Supports the MegaPrime instrument."""
 
     default_resource_root = posixpath.join(CORRECTIONS_RESOURCE_ROOT, "CFHT")
     """Default resource path root to use to locate header correction files."""
 
+    _observing_day_offset = astropy.time.TimeDelta(0, format="sec", scale="tai")
+
     # CFHT Megacam has no rotator, and the instrument angle on sky is set to
     # +Y=N, +X=W which we define as a 0 degree rotation.
     _const_map = {
         "boresight_rotation_angle": Angle(0 * u.deg),
         "boresight_rotation_coord": "sky",
         "detector_group": None,
     }
@@ -183,16 +185,16 @@
     @cache_translation
     def to_pressure(self) -> astropy.units.Quantity:
         # Docstring will be inherited. Property defined in properties.py
         # Can be either AIRPRESS in Pa or PRESSURE in mbar
         for key, unit in (("PRESSURE", u.hPa), ("AIRPRESS", u.Pa)):
             if self.is_key_ok(key):
                 return self.quantity_from_card(key, unit)
-        else:
-            raise KeyError(f"{self._log_prefix}: Could not find pressure keywords in header")
+
+        raise KeyError(f"{self._log_prefix}: Could not find pressure keywords in header")
 
     @cache_translation
     def to_observation_counter(self) -> int:
         """Return the lifetime exposure number.
 
         Returns
         -------
@@ -258,7 +260,24 @@
                 # COMPRESSED_IMAGE but the EXTVER as the detector number.
                 if hdu.name == "COMPRESSED_IMAGE":
                     header = hdu.header
 
                     # Astropy strips EXTNAME so put it back for the translator
                     header["EXTNAME"] = f"ccd{hdu.ver:02d}"
                     yield header
+
+    @classmethod
+    def observing_date_to_offset(cls, observing_date: astropy.time.Time) -> astropy.time.TimeDelta | None:
+        """Return the offset to use when calculating the observing day.
+
+        Parameters
+        ----------
+        observing_date : `astropy.time.Time`
+            The date of the observation. Unused.
+
+        Returns
+        -------
+        offset : `astropy.time.TimeDelta`
+            The offset to apply. The offset is always 0 seconds. In Hawaii
+            UTC rollover is at 2pm local time.
+        """
+        return cls._observing_day_offset
```

### Comparing `astro-metadata-translator-26.2024.900/python/astro_metadata_translator/translators/sdss.py` & `astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/translators/sdss.py`

 * *Files identical despite different names*

### Comparing `astro-metadata-translator-26.2024.900/python/astro_metadata_translator/translators/subaru.py` & `astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/translators/subaru.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,23 +11,26 @@
 
 """Metadata translation code for Subaru telescope."""
 
 from __future__ import annotations
 
 __all__ = ("SubaruTranslator",)
 
+import astropy.time
 from astropy.coordinates import EarthLocation
 
 from ..translator import cache_translation
 from .fits import FitsTranslator
 
 
 class SubaruTranslator(FitsTranslator):
     """Metadata translator for Subaru telescope headers."""
 
+    _observing_day_offset = astropy.time.TimeDelta(0, format="sec", scale="tai")
+
     @cache_translation
     def to_location(self) -> EarthLocation:
         """Return the location of the Subaru telescope on Mauna Kea.
 
         Hardcodes the location and does not look at any headers.
 
         Returns
@@ -43,7 +46,24 @@
 
         Returns
         -------
         sequence : `int`
             The observation counter.
         """
         return self.to_exposure_id()
+
+    @classmethod
+    def observing_date_to_offset(cls, observing_date: astropy.time.Time) -> astropy.time.TimeDelta | None:
+        """Return the offset to use when calculating the observing day.
+
+        Parameters
+        ----------
+        observing_date : `astropy.time.Time`
+            The date of the observation. Unused.
+
+        Returns
+        -------
+        offset : `astropy.time.TimeDelta`
+            The offset to apply. The offset is always 0 seconds. In Hawaii
+            UTC rollover is at 2pm local time.
+        """
+        return cls._observing_day_offset
```

### Comparing `astro-metadata-translator-26.2024.900/python/astro_metadata_translator/translators/suprimecam.py` & `astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator/translators/suprimecam.py`

 * *Files identical despite different names*

### Comparing `astro-metadata-translator-26.2024.900/python/astro_metadata_translator.egg-info/PKG-INFO` & `astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 Metadata-Version: 2.1
 Name: astro-metadata-translator
-Version: 26.2024.900
+Version: 27.0.0rc1
 Summary: A translator for astronomical metadata.
-Home-page: https://github.com/lsst/astro_metadata_translator
-Author: Rubin Observatory Data Management
-Author-email: dm-admin@lists.lsst.org
+Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
+Project-URL: Homepage, https://github.com/lsst/astro_metadata_translator
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering :: Astronomy
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: astropy>=3.0.5
 Requires-Dist: pyyaml>=3.13
 Requires-Dist: click>=8
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
 
 # astro_metadata_translator
 
 [![pypi](https://img.shields.io/pypi/v/astro-metadata-translator.svg)](https://pypi.org/project/astro-metadata-translator/)
 [![codecov](https://codecov.io/gh/lsst/astro_metadata_translator/branch/main/graph/badge.svg?token=0HtEHdoYDF)](https://codecov.io/gh/lsst/astro_metadata_translator)
 
 Observation metadata handling infrastructure
```

### Comparing `astro-metadata-translator-26.2024.900/python/astro_metadata_translator.egg-info/SOURCES.txt` & `astro_metadata_translator-27.0.0rc1/python/astro_metadata_translator.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -19,19 +19,21 @@
 python/astro_metadata_translator.egg-info/SOURCES.txt
 python/astro_metadata_translator.egg-info/dependency_links.txt
 python/astro_metadata_translator.egg-info/entry_points.txt
 python/astro_metadata_translator.egg-info/requires.txt
 python/astro_metadata_translator.egg-info/top_level.txt
 python/astro_metadata_translator.egg-info/zip-safe
 python/astro_metadata_translator/bin/__init__.py
-python/astro_metadata_translator/bin/translateheader.py
+python/astro_metadata_translator/bin/translate.py
 python/astro_metadata_translator/bin/writeindex.py
 python/astro_metadata_translator/bin/writesidecar.py
 python/astro_metadata_translator/cli/__init__.py
 python/astro_metadata_translator/cli/astrometadata.py
+python/astro_metadata_translator/corrections/CFHT/README.md
+python/astro_metadata_translator/corrections/DECam/README.md
 python/astro_metadata_translator/corrections/HSC/HSC-HSCA00042600.yaml
 python/astro_metadata_translator/corrections/HSC/HSC-HSCA00120200.yaml
 python/astro_metadata_translator/corrections/HSC/HSC-HSCA00120400.yaml
 python/astro_metadata_translator/corrections/HSC/HSC-HSCA00120600.yaml
 python/astro_metadata_translator/corrections/HSC/HSC-HSCA00120800.yaml
 python/astro_metadata_translator/corrections/HSC/HSC-HSCA00121000.yaml
 python/astro_metadata_translator/corrections/HSC/HSC-HSCA00121200.yaml
@@ -51,27 +53,31 @@
 python/astro_metadata_translator/corrections/HSC/HSC-HSCA00186800.yaml
 python/astro_metadata_translator/corrections/HSC/HSC-HSCA00187000.yaml
 python/astro_metadata_translator/corrections/HSC/HSC-HSCA00187200.yaml
 python/astro_metadata_translator/corrections/HSC/HSC-HSCA00187400.yaml
 python/astro_metadata_translator/corrections/HSC/HSC-HSCA00187600.yaml
 python/astro_metadata_translator/corrections/HSC/HSC-HSCA00188000.yaml
 python/astro_metadata_translator/corrections/HSC/HSC-HSCA00188200.yaml
+python/astro_metadata_translator/corrections/HSC/README.md
+python/astro_metadata_translator/corrections/SDSS/README.md
+python/astro_metadata_translator/corrections/SuprimeCam/README.md
 python/astro_metadata_translator/serialize/__init__.py
 python/astro_metadata_translator/serialize/fits.py
 python/astro_metadata_translator/translators/__init__.py
 python/astro_metadata_translator/translators/decam.py
 python/astro_metadata_translator/translators/fits.py
 python/astro_metadata_translator/translators/helpers.py
 python/astro_metadata_translator/translators/hsc.py
 python/astro_metadata_translator/translators/megaprime.py
 python/astro_metadata_translator/translators/sdss.py
 python/astro_metadata_translator/translators/subaru.py
 python/astro_metadata_translator/translators/suprimecam.py
 tests/test_basics.py
 tests/test_cfht.py
+tests/test_cli.py
 tests/test_decam.py
 tests/test_extensions.py
 tests/test_groups.py
 tests/test_headers.py
 tests/test_indexing.py
 tests/test_sdss.py
 tests/test_shadowing.py
```

### Comparing `astro-metadata-translator-26.2024.900/tests/test_basics.py` & `astro_metadata_translator-27.0.0rc1/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `astro-metadata-translator-26.2024.900/tests/test_cfht.py` & `astro_metadata_translator-27.0.0rc1/tests/test_cfht.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 #
 # Use of this source code is governed by a 3-clause BSD-style
 # license that can be found in the LICENSE file.
 
 import os.path
 import unittest
 
+import astropy.time
 import astropy.units as u
 
 from astro_metadata_translator import ObservationInfo
 from astro_metadata_translator.tests import MetadataAssertHelper, read_test_file
 
 TESTDIR = os.path.abspath(os.path.dirname(__file__))
 
@@ -49,14 +50,15 @@
                     has_simulated_content=False,
                     object="w2.+2+2",
                     observation_counter=1038843,
                     observation_id="1038843",
                     observation_type="science",
                     observation_reason="science",
                     observing_day=20081101,
+                    observing_day_offset=astropy.time.TimeDelta(0, format="sec", scale="tai"),
                     physical_filter="i.MP9702",
                     pressure=617.65 * u.hPa,
                     relative_humidity=39.77,
                     science_program="08BL05",
                     temperature=0.9 * u.deg_C,
                     visit_id=1038843,
                 ),
```

### Comparing `astro-metadata-translator-26.2024.900/tests/test_decam.py` & `astro_metadata_translator-27.0.0rc1/tests/test_decam.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 #
 # Use of this source code is governed by a 3-clause BSD-style
 # license that can be found in the LICENSE file.
 
 import os.path
 import unittest
 
+import astropy.time
 import astropy.units as u
 
 from astro_metadata_translator.tests import MetadataAssertHelper
 
 TESTDIR = os.path.abspath(os.path.dirname(__file__))
 
 
@@ -47,15 +48,15 @@
                     group_counter_start=229388,
                     has_simulated_content=False,
                     object="DES supernova hex SN-S1 tiling 22",
                     observation_counter=229388,
                     observation_id="ct4m20130901t060255",
                     observation_type="science",
                     observation_reason="science",
-                    observing_day=20130901,
+                    observing_day=20130831,
                     physical_filter="z DECam SDSS c0004 9260.0 1520.0",
                     pressure=779.0 * u.hPa,
                     relative_humidity=23.0,
                     science_program="2012B-0001",
                     temperature=11.9 * u.deg_C,
                     visit_id=229388,
                     wcs_params=dict(max_sep=1.5),
@@ -84,14 +85,15 @@
                     has_simulated_content=False,
                     object="postflats-BIAS",
                     observation_counter=160496,
                     observation_id="ct4m20121211t220632",
                     observation_type="zero",
                     observation_reason="unknown",
                     observing_day=20121211,
+                    observing_day_offset=astropy.time.TimeDelta(12 * 3600, format="sec", scale="tai"),
                     physical_filter="solid plate 0.0 0.0",  # corrected value
                     pressure=777.0 * u.hPa,
                     relative_humidity=38.0,
                     science_program="2012B-0416",
                     temperature=17.0 * u.deg_C,
                     visit_id=160496,
                     wcs_params=dict(max_sep=1.5),
@@ -119,15 +121,15 @@
                     group_counter_start=412037,
                     has_simulated_content=False,
                     object="Blind15A_03",
                     observation_counter=412037,
                     observation_id="ct4m20150220t004721",
                     observation_type="science",
                     observation_reason="science",
-                    observing_day=20150220,
+                    observing_day=20150219,
                     physical_filter="g",
                     pressure=777.0 * u.hPa,
                     relative_humidity=76.0,
                     science_program="2015A-0608",
                     temperature=9.0 * u.deg_C,
                     visit_id=412037,
                     wcs_params=dict(max_sep=5.0),
@@ -155,15 +157,15 @@
                     group_counter_start=845291,
                     has_simulated_content=False,
                     object="",
                     observation_counter=845291,
                     observation_id="ct4m20190402t050618",
                     observation_type="science",
                     observation_reason="science",
-                    observing_day=20190402,
+                    observing_day=20190401,
                     physical_filter="VR DECam c0007 6300.0 2600.0",
                     pressure=779.0 * u.hPa,
                     relative_humidity=38.0,
                     science_program="2019A-0337",
                     temperature=15.1 * u.deg_C,
                     visit_id=845291,
                     wcs_params=dict(max_sep=5.0),
```

### Comparing `astro-metadata-translator-26.2024.900/tests/test_extensions.py` & `astro_metadata_translator-27.0.0rc1/tests/test_extensions.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,15 +49,21 @@
         self.header = dict(INSTRUME="dummy")
         # The test translator is incomplete so it will issue warnings
         # about missing translations. Catch them.
         with self.assertWarns(UserWarning):
             self.obsinfo = ObservationInfo(self.header)
 
     def assert_observation_info(self, obsinfo):
-        """Check that the `ObservationInfo` is as expected."""
+        """Check that the `ObservationInfo` is as expected.
+
+        Parameters
+        ----------
+        obsinfo : `ObservationInfo`
+            Information to check.
+        """
         self.assertIsInstance(obsinfo, ObservationInfo)
         self.assertEqual(obsinfo.ext_foo, FOO)
         self.assertEqual(obsinfo.ext_number, NUMBER)
 
     def test_basic(self):
         """Test construction of extended ObservationInfo."""
         # Behaves like the original
```

### Comparing `astro-metadata-translator-26.2024.900/tests/test_groups.py` & `astro_metadata_translator-27.0.0rc1/tests/test_groups.py`

 * *Files identical despite different names*

### Comparing `astro-metadata-translator-26.2024.900/tests/test_headers.py` & `astro_metadata_translator-27.0.0rc1/tests/test_headers.py`

 * *Files identical despite different names*

### Comparing `astro-metadata-translator-26.2024.900/tests/test_indexing.py` & `astro_metadata_translator-27.0.0rc1/tests/test_indexing.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 # for details of code ownership.
 #
 # Use of this source code is governed by a 3-clause BSD-style
 # license that can be found in the LICENSE file.
 
 import io
 import json
+import logging
 import os
 import tempfile
 import unittest
 
 from astro_metadata_translator import ObservationGroup, ObservationInfo
 from astro_metadata_translator.file_helpers import read_file_info
 from astro_metadata_translator.indexing import (
@@ -141,43 +142,41 @@
 
         with self.assertRaises(ValueError):
             read_file_info(file, 1, None, "unknown")
 
         with self.assertRaises(FileNotFoundError):
             read_file_info("notthere.not", 1)
 
-        with io.StringIO() as err:
-            info = read_file_info("notthere.not", 1, print_trace=False, errstream=err)
-            err.seek(0)
-            self.assertEqual(err.readlines()[0], "Unable to open file notthere.not\n")
+        with self.assertLogs(level=logging.WARNING) as cm:
+            info = read_file_info("notthere.not", 1, print_trace=False)
+
+        self.assertIn("Unable to open file notthere.not", "\n".join(cm.output))
 
         # Now read a file that can not be translated and should trigger
         # different errors
         bad_file = os.path.join(TESTDATA, "corrections", "SCUBA_test-20000101_00002.yaml")
 
         with self.assertLogs(level="DEBUG") as cm:
             with self.assertRaises(ValueError):
                 read_file_info(bad_file, 1)
         self.assertIn("Unable to determine translator class", "\n".join(cm.output))
 
         with io.StringIO() as out:
-            with io.StringIO() as err:
-                info = read_file_info(bad_file, 1, print_trace=False, errstream=err, outstream=out)
-                out.seek(0)
-                lines = out.readlines()
-                self.assertEqual(len(lines), 1)
-                self.assertIn("ValueError", lines[0])
+            info = read_file_info(bad_file, 1, print_trace=False, outstream=out)
+            out.seek(0)
+            lines = out.readlines()
+            self.assertEqual(len(lines), 1)
+            self.assertIn("ValueError", lines[0])
 
         with io.StringIO() as out:
-            with io.StringIO() as err:
-                info = read_file_info(bad_file, 1, print_trace=True, errstream=err, outstream=out)
-                out.seek(0)
-                lines = out.readlines()
-                self.assertGreater(len(lines), 4)
-                self.assertIn("ValueError", lines[-1])
+            info = read_file_info(bad_file, 1, print_trace=True, outstream=out)
+            out.seek(0)
+            lines = out.readlines()
+            self.assertGreater(len(lines), 4)
+            self.assertIn("ValueError", lines[-1])
 
         # A sidecar file that is not a dict.
         not_dict = os.path.join(TESTDATA, "bad-sidecar.json")
         with self.assertRaises(ValueError):
             read_sidecar(not_dict)
 
         with self.assertRaises(ValueError):
```

### Comparing `astro-metadata-translator-26.2024.900/tests/test_sdss.py` & `astro_metadata_translator-27.0.0rc1/tests/test_sdss.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,14 +47,15 @@
                     has_simulated_content=False,
                     object="82 S",
                     observation_counter=0,
                     observation_id="6377 4 g 407",
                     observation_type="science",
                     observation_reason="science",
                     observing_day=20060920,
+                    observing_day_offset=None,
                     physical_filter="g",
                     pressure=None,
                     relative_humidity=None,
                     science_program="82 S",
                     temperature=None,
                     visit_id=6377,
                     wcs_params=dict(max_sep=10.0),
```

### Comparing `astro-metadata-translator-26.2024.900/tests/test_shadowing.py` & `astro_metadata_translator-27.0.0rc1/tests/test_shadowing.py`

 * *Files identical despite different names*

### Comparing `astro-metadata-translator-26.2024.900/tests/test_subaru.py` & `astro_metadata_translator-27.0.0rc1/tests/test_subaru.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 #
 # Use of this source code is governed by a 3-clause BSD-style
 # license that can be found in the LICENSE file.
 
 import os.path
 import unittest
 
+import astropy.time
 import astropy.units as u
 
 from astro_metadata_translator import merge_headers
 from astro_metadata_translator.tests import MetadataAssertHelper, read_test_file
 
 TESTDIR = os.path.abspath(os.path.dirname(__file__))
 
@@ -48,14 +49,15 @@
                     has_simulated_content=False,
                     object="STRIPE82L",
                     observation_counter=904024,
                     observation_id="HSCA90402400",
                     observation_type="science",
                     observation_reason="science",
                     observing_day=20131102,
+                    observing_day_offset=astropy.time.TimeDelta(0, format="sec", scale="tai"),
                     physical_filter="HSC-I",
                     pressure=621.7 * u.hPa,
                     relative_humidity=33.1,
                     science_program="o13015",
                     temperature=272.35 * u.K,
                     visit_id=904024,
                 ),
```

### Comparing `astro-metadata-translator-26.2024.900/tests/test_translate_header.py` & `astro_metadata_translator-27.0.0rc1/tests/test_translate_header.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,25 +6,26 @@
 # See the LICENSE file at the top-level directory of this distribution
 # for details of code ownership.
 #
 # Use of this source code is governed by a 3-clause BSD-style
 # license that can be found in the LICENSE file.
 
 import io
+import logging
 import os.path
 import unittest
 
-from astro_metadata_translator.bin.translateheader import process_files
+from astro_metadata_translator.bin.translate import translate_or_dump_headers
 
 TESTDIR = os.path.abspath(os.path.dirname(__file__))
 TESTDATA = os.path.join(TESTDIR, "data")
 
 
 class TestTranslateHeader(unittest.TestCase):
-    """Test that the translate_header CLI logic works."""
+    """Test that the astrometadata translate and dump logic works."""
 
     def _readlines(self, stream):
         """Return the lines written to the stream.
 
         Parameters
         ----------
         stream : `io.StringIO`
@@ -37,135 +38,144 @@
         """
         stream.seek(0)
         return [ll.rstrip() for ll in stream.readlines()]
 
     def test_translate_header(self):
         """Translate some header files."""
         with io.StringIO() as out:
-            with io.StringIO() as err:
-                okay, failed = process_files(
+            with self.assertLogs(level=logging.INFO) as cm:
+                okay, failed = translate_or_dump_headers(
                     [TESTDATA],
                     r"^fitsheader.*yaml$",
                     0,
                     False,
                     outstream=out,
-                    errstream=err,
                     output_mode="none",
                 )
-                self.assertEqual(self._readlines(out), [])
-                lines = self._readlines(err)
-                self.assertEqual(len(lines), 10)
-                self.assertTrue(lines[0].startswith("Analyzing"), f"Line: '{lines[0]}'")
+            self.assertEqual(self._readlines(out), [])
+            lines = [r.getMessage() for r in cm.records]
+            self.assertEqual(len(lines), 10)
+            self.assertTrue(lines[0].startswith("Analyzing"), f"Line: '{lines[0]}'")
 
         self.assertEqual(len(okay), 10)
         self.assertEqual(len(failed), 0)
 
     def test_translate_header_table(self):
         """Translate some header files with table output."""
         with io.StringIO() as out:
-            with io.StringIO() as err:
-                okay, failed = process_files(
-                    [TESTDATA], r"^fitsheader.*yaml$", 0, False, outstream=out, errstream=err
+            with self.assertLogs(level=logging.WARNING) as cm:
+                logging.getLogger().warning("False warning")
+                okay, failed = translate_or_dump_headers(
+                    [TESTDATA],
+                    r"^fitsheader.*yaml$",
+                    0,
+                    False,
+                    outstream=out,
                 )
                 output = self._readlines(out)
                 self.assertTrue(output[0].startswith("ObsId"))
                 self.assertTrue(output[1].startswith("-------"))
                 self.assertEqual(len(output), 12)
-                errlines = self._readlines(err)
-                self.assertEqual(len(errlines), 0)
+                self.assertEqual(len(cm.output), 1)  # Should only have the warning this test made.
 
         self.assertEqual(len(okay), 10)
         self.assertEqual(len(failed), 0)
 
     def test_translate_header_fails(self):
         """Translate some header files that fail."""
         with io.StringIO() as out:
-            with io.StringIO() as err:
-                okay, failed = process_files(
-                    [TESTDATA], r"^.*yaml$", 0, False, outstream=out, errstream=err, output_mode="none"
-                )
-
-                lines = self._readlines(out)
-                self.assertEqual(len(lines), len(failed))
-                self.assertTrue(lines[0].startswith("Failure processing"), f"Line: '{lines[0]}'")
-                self.assertIn("not a mapping", lines[0], f"Line: '{lines[0]}'")
-
-                lines = self._readlines(err)
-                self.assertEqual(len(lines), 13)
-                self.assertTrue(lines[0].startswith("Analyzing"), f"Line: '{lines[0]}'")
-
-        self.assertEqual(len(okay), 10)
-        self.assertEqual(len(failed), 3)
+            with self.assertLogs(level=logging.INFO) as cm:
+                okay, failed = translate_or_dump_headers(
+                    [TESTDATA], r"^.*yaml$", 0, False, outstream=out, output_mode="none"
+                )
+
+            out_lines = self._readlines(out)
+            self.assertEqual(len(out_lines), len(failed))
+            self.assertTrue(out_lines[0].startswith("Failure processing"), f"Line: '{out_lines[0]}'")
+            self.assertIn("not a mapping", out_lines[0], f"Line: '{out_lines[0]}'")
+
+            err_lines = [r.getMessage() for r in cm.records]
+            self.assertEqual(len(err_lines), 13)  # The number of files analyzed
+            self.assertTrue(err_lines[0].startswith("Analyzing"), f"Line: '{err_lines[0]}'")
+
+        # Form message to issue if the test fails.
+        newline = "\n"  # f-string can not accept \ in string.
+        msg = f"""Converted successfully:
+{newline.join(okay)}
+Failed conversions:
+{newline.join(failed)}
+Standard output:
+{newline.join(out_lines)}
+"""
+        self.assertEqual((len(okay), len(failed)), (10, 3), msg=msg)
 
     def test_translate_header_traceback(self):
         """Translate some header files that fail and trigger traceback."""
         with io.StringIO() as out:
-            with io.StringIO() as err:
-                okay, failed = process_files(
-                    [TESTDATA], r"^.*yaml$", 0, True, outstream=out, errstream=err, output_mode="none"
+            with self.assertLogs(level=logging.INFO) as cm:
+                okay, failed = translate_or_dump_headers(
+                    [TESTDATA], r"^.*yaml$", 0, True, outstream=out, output_mode="none"
                 )
 
-                lines = self._readlines(out)
-                self.assertGreaterEqual(len(lines), 22, "\n".join(lines))
-                self.assertTrue(lines[0].startswith("Traceback"), f"Line '{lines[0]}'")
-
-                lines = self._readlines(err)
-                self.assertGreaterEqual(len(lines), 13, "\n".join(lines))
-                self.assertTrue(lines[0].startswith("Analyzing"), f"Line: '{lines[0]}'")
+            lines = self._readlines(out)
+            self.assertGreaterEqual(len(lines), 22, "\n".join(lines))
+            self.assertTrue(lines[0].startswith("Traceback"), f"Line '{lines[0]}'")
+
+            lines = [r.getMessage() for r in cm.records]
+            self.assertGreaterEqual(len(lines), 13, "\n".join(lines))
+            self.assertTrue(lines[0].startswith("Analyzing"), f"Line: '{lines[0]}'")
 
         self.assertEqual(len(okay), 10)
         self.assertEqual(len(failed), 3)
 
     def test_translate_header_dump(self):
         """Check that a header is dumped."""
         with io.StringIO() as out:
-            with io.StringIO() as err:
-                okay, failed = process_files(
+            with self.assertLogs(level=logging.INFO) as cm:
+                okay, failed = translate_or_dump_headers(
                     [os.path.join(TESTDATA, "fitsheader-decam.yaml")],
                     r"^fitsheader.*yaml$",
                     0,
                     False,
                     outstream=out,
-                    errstream=err,
                     output_mode="yaml",
                 )
 
-                lines = self._readlines(out)
-                # Look for a DECam header in the output
-                header = "\n".join(lines)
-                self.assertIn("DTINSTRU", header)
-
-                lines = self._readlines(err)
-                self.assertEqual(len(lines), 1)
-                self.assertTrue(lines[0], "Analyzing tests/data/fitsheader-decam.yaml...")
+            lines = self._readlines(out)
+            # Look for a DECam header in the output
+            header = "\n".join(lines)
+            self.assertIn("DTINSTRU", header)
+
+            lines = [r.getMessage() for r in cm.records]
+            self.assertEqual(len(lines), 1)
+            self.assertTrue(lines[0], "Analyzing tests/data/fitsheader-decam.yaml...")
 
         self.assertEqual(len(okay), 1)
         self.assertEqual(len(failed), 0)
 
     def test_translate_header_loud(self):
         """Check that ObservationInfo content is displayed."""
         with io.StringIO() as out:
-            with io.StringIO() as err:
-                okay, failed = process_files(
+            with self.assertLogs(level=logging.INFO) as cm:
+                okay, failed = translate_or_dump_headers(
                     [os.path.join(TESTDATA, "fitsheader-decam.yaml")],
                     r"^fitsheader.*yaml$",
                     0,
                     False,
                     outstream=out,
-                    errstream=err,
                     output_mode="verbose",
                 )
 
-                lines = self._readlines(out)
-                # Look for the translated DECam header in the output
-                self.assertEqual(lines[2], "datetime_begin: 2013-09-01T06:02:55.754")
-
-                lines = self._readlines(err)
-                self.assertEqual(len(lines), 1)
-                self.assertTrue(lines[0], "Analyzing tests/data/fitsheader-decam.yaml...")
+            lines = self._readlines(out)
+            # Look for the translated DECam header in the output
+            self.assertEqual(lines[2], "datetime_begin: 2013-09-01T06:02:55.754")
+
+            lines = [r.getMessage() for r in cm.records]
+            self.assertEqual(len(lines), 1)
+            self.assertTrue(lines[0], "Analyzing tests/data/fitsheader-decam.yaml...")
 
         self.assertEqual(len(okay), 1)
         self.assertEqual(len(failed), 0)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `astro-metadata-translator-26.2024.900/tests/test_translation.py` & `astro_metadata_translator-27.0.0rc1/tests/test_translation.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Use of this source code is governed by a 3-clause BSD-style
 # license that can be found in the LICENSE file.
 
 import os.path
 import unittest
 
-from astropy.time import Time
+from astropy.time import Time, TimeDelta
 
 from astro_metadata_translator import FitsTranslator, ObservationInfo, StubTranslator
 
 TESTDIR = os.path.abspath(os.path.dirname(__file__))
 
 
 class InstrumentTestTranslator(FitsTranslator, StubTranslator):
@@ -241,10 +241,22 @@
                     ObservationInfo(
                         header,
                         translator_class=InstrumentTestTranslator,
                         pedantic=False,
                         required={"boresight_airmass"},
                     )
 
+    def test_observing_date(self):
+        """Test the observing_date class methods."""
+        date1 = Time("2023-07-06T13:00", format="isot", scale="tai")
+        day_obs = StubTranslator.observing_date_to_observing_day(date1, 12 * 3600)
+        self.assertEqual(day_obs, 20230706)
+
+        date2 = Time("2023-07-07T11:00", format="isot", scale="tai")
+        day_obs = StubTranslator.observing_date_to_observing_day(date2, TimeDelta("0.5d", scale="tai"))
+        self.assertEqual(day_obs, 20230706)
+        day_obs = StubTranslator.observing_date_to_observing_day(date2, 1.0)
+        self.assertEqual(day_obs, 20230707)
+
 
 if __name__ == "__main__":
     unittest.main()
```

