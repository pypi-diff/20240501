# Comparing `tmp/voltorb-0.0.0.tar.gz` & `tmp/voltorb-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voltorb-0.0.0.tar", last modified: Wed May  1 08:10:55 2024, max compression
+gzip compressed data, was "voltorb-0.1.0.tar", last modified: Wed May  1 09:21:46 2024, max compression
```

## Comparing `voltorb-0.0.0.tar` & `voltorb-0.1.0.tar`

### file list

```diff
@@ -1,12 +1,53 @@
-drwxr-xr-x   0 avianello   (503) staff       (20)        0 2024-05-01 08:10:55.977023 voltorb-0.0.0/
--rw-r--r--   0 avianello   (503) staff       (20)      162 2024-05-01 08:10:55.976552 voltorb-0.0.0/PKG-INFO
--rw-r--r--   0 avianello   (503) staff       (20)      286 2024-05-01 08:08:12.000000 voltorb-0.0.0/pyproject.toml
--rw-r--r--   0 avianello   (503) staff       (20)       38 2024-05-01 08:10:55.977153 voltorb-0.0.0/setup.cfg
-drwxr-xr-x   0 avianello   (503) staff       (20)        0 2024-05-01 08:10:55.972350 voltorb-0.0.0/src/
-drwxr-xr-x   0 avianello   (503) staff       (20)        0 2024-05-01 08:10:55.973123 voltorb-0.0.0/src/voltorb/
--rw-r--r--   0 avianello   (503) staff       (20)        0 2024-05-01 08:08:05.000000 voltorb-0.0.0/src/voltorb/__init__.py
-drwxr-xr-x   0 avianello   (503) staff       (20)        0 2024-05-01 08:10:55.975986 voltorb-0.0.0/src/voltorb.egg-info/
--rw-r--r--   0 avianello   (503) staff       (20)      162 2024-05-01 08:10:55.000000 voltorb-0.0.0/src/voltorb.egg-info/PKG-INFO
--rw-r--r--   0 avianello   (503) staff       (20)      178 2024-05-01 08:10:55.000000 voltorb-0.0.0/src/voltorb.egg-info/SOURCES.txt
--rw-r--r--   0 avianello   (503) staff       (20)        1 2024-05-01 08:10:55.000000 voltorb-0.0.0/src/voltorb.egg-info/dependency_links.txt
--rw-r--r--   0 avianello   (503) staff       (20)        8 2024-05-01 08:10:55.000000 voltorb-0.0.0/src/voltorb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:21:46.558860 voltorb-0.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:21:46.554860 voltorb-0.1.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-01 09:21:33.000000 voltorb-0.1.0/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:21:46.554860 voltorb-0.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-05-01 09:21:33.000000 voltorb-0.1.0/.github/workflows/core.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-05-01 09:21:33.000000 voltorb-0.1.0/.github/workflows/deploy-package.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-01 09:21:33.000000 voltorb-0.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-05-01 09:21:33.000000 voltorb-0.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-01 09:21:33.000000 voltorb-0.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6715 2024-05-01 09:21:46.558860 voltorb-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5658 2024-05-01 09:21:33.000000 voltorb-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-01 09:21:33.000000 voltorb-0.1.0/check_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-05-01 09:21:33.000000 voltorb-0.1.0/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-05-01 09:21:33.000000 voltorb-0.1.0/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-05-01 09:21:33.000000 voltorb-0.1.0/plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-01 09:21:33.000000 voltorb-0.1.0/pylock.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4146 2024-05-01 09:21:33.000000 voltorb-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 09:21:46.558860 voltorb-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:21:46.550860 voltorb-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:21:46.554860 voltorb-0.1.0/src/voltorb/
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-01 09:21:33.000000 voltorb-0.1.0/src/voltorb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-01 09:21:33.000000 voltorb-0.1.0/src/voltorb/_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-01 09:21:46.000000 voltorb-0.1.0/src/voltorb/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21023 2024-05-01 09:21:33.000000 voltorb-0.1.0/src/voltorb/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-01 09:21:33.000000 voltorb-0.1.0/src/voltorb/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-01 09:21:33.000000 voltorb-0.1.0/src/voltorb/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-05-01 09:21:33.000000 voltorb-0.1.0/src/voltorb/middlewares.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-05-01 09:21:33.000000 voltorb-0.1.0/src/voltorb/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-05-01 09:21:33.000000 voltorb-0.1.0/src/voltorb/serde.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-01 09:21:33.000000 voltorb-0.1.0/src/voltorb/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:21:46.558860 voltorb-0.1.0/src/voltorb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6715 2024-05-01 09:21:46.000000 voltorb-0.1.0/src/voltorb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-01 09:21:46.000000 voltorb-0.1.0/src/voltorb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 09:21:46.000000 voltorb-0.1.0/src/voltorb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-01 09:21:46.000000 voltorb-0.1.0/src/voltorb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-01 09:21:46.000000 voltorb-0.1.0/src/voltorb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:21:46.558860 voltorb-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 09:21:33.000000 voltorb-0.1.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:21:46.558860 voltorb-0.1.0/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 09:21:33.000000 voltorb-0.1.0/tests/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5928 2024-05-01 09:21:33.000000 voltorb-0.1.0/tests/api/test_carbon_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-01 09:21:33.000000 voltorb-0.1.0/tests/api/test_health.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-05-01 09:21:33.000000 voltorb-0.1.0/tests/api/test_marginal_carbon_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10384 2024-05-01 09:21:33.000000 voltorb-0.1.0/tests/api/test_power_breakdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-05-01 09:21:33.000000 voltorb-0.1.0/tests/api/test_power_consumption_breakdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-01 09:21:33.000000 voltorb-0.1.0/tests/api/test_power_production_breakdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-01 09:21:33.000000 voltorb-0.1.0/tests/api/test_updated_since.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-01 09:21:33.000000 voltorb-0.1.0/tests/api/test_zones.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-01 09:21:33.000000 voltorb-0.1.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-01 09:21:33.000000 voltorb-0.1.0/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-01 09:21:33.000000 voltorb-0.1.0/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-05-01 09:21:33.000000 voltorb-0.1.0/tests/test_middlewares.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-01 09:21:33.000000 voltorb-0.1.0/tests/test_public_api.py
```

