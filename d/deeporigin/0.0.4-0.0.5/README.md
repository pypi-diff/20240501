# Comparing `tmp/deeporigin-0.0.4.tar.gz` & `tmp/deeporigin-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deeporigin-0.0.4.tar", last modified: Mon Apr 29 13:57:08 2024, max compression
+gzip compressed data, was "deeporigin-0.0.5.tar", last modified: Wed May  1 15:12:26 2024, max compression
```

## Comparing `deeporigin-0.0.4.tar` & `deeporigin-0.0.5.tar`

### file list

```diff
@@ -1,66 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:57:08.388641 deeporigin-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-29 13:57:03.000000 deeporigin-0.0.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-29 13:57:03.000000 deeporigin-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-29 13:57:08.388641 deeporigin-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-29 13:57:03.000000 deeporigin-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:57:08.388641 deeporigin-0.0.4/deeporigin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-29 13:57:08.000000 deeporigin-0.0.4/deeporigin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-29 13:57:08.000000 deeporigin-0.0.4/deeporigin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 13:57:08.000000 deeporigin-0.0.4/deeporigin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-29 13:57:08.000000 deeporigin-0.0.4/deeporigin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-29 13:57:08.000000 deeporigin-0.0.4/deeporigin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-29 13:57:08.000000 deeporigin-0.0.4/deeporigin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-29 13:57:03.000000 deeporigin-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 13:57:08.388641 deeporigin-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:57:08.380641 deeporigin-0.0.4/src/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-29 13:57:05.000000 deeporigin-0.0.4/src/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:57:08.380641 deeporigin-0.0.4/src/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/cli/context.py
--rw-r--r--   0 runner    (1001) docker     (127)    11909 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/cli/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    14212 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/cli/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:57:08.380641 deeporigin-0.0.4/src/config/
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/config/default.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/do_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/feature_flags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:57:08.380641 deeporigin-0.0.4/src/managed_data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/managed_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8487 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/managed_data/_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    15869 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/managed_data/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     9305 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/managed_data/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/managed_data/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:57:08.380641 deeporigin-0.0.4/src/variables/
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/variables/base_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    20324 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/variables/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:57:08.384641 deeporigin-0.0.4/src/variables/types/
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/variables/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/variables/types/anthropic_api_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    11608 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/variables/types/aws_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     9728 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/variables/types/env_var.py
--rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/variables/types/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     8402 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/variables/types/git_http_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/variables/types/gurobi_license_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/variables/types/mosek_license_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/variables/types/open_ai_api_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     5606 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/variables/types/private_gpg_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/variables/types/private_ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/variables/types/secret_env_var.py
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/variables/types/secret_env_var_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/variables/types/secret_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/variables/types/secret_file_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/variables/types/xpress_license_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:57:08.388641 deeporigin-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-04-29 13:57:03.000000 deeporigin-0.0.4/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-29 13:57:03.000000 deeporigin-0.0.4/tests/test_cli_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5850 2024-04-29 13:57:03.000000 deeporigin-0.0.4/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9024 2024-04-29 13:57:03.000000 deeporigin-0.0.4/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-04-29 13:57:03.000000 deeporigin-0.0.4/tests/test_feature_flags.py
--rw-r--r--   0 runner    (1001) docker     (127)    10328 2024-04-29 13:57:03.000000 deeporigin-0.0.4/tests/test_managed_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    90063 2024-04-29 13:57:03.000000 deeporigin-0.0.4/tests/test_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:12:26.922603 deeporigin-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-01 15:12:23.000000 deeporigin-0.0.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-01 15:12:23.000000 deeporigin-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-01 15:12:26.922603 deeporigin-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-01 15:12:23.000000 deeporigin-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:12:26.922603 deeporigin-0.0.5/deeporigin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-01 15:12:26.000000 deeporigin-0.0.5/deeporigin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-01 15:12:26.000000 deeporigin-0.0.5/deeporigin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 15:12:26.000000 deeporigin-0.0.5/deeporigin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-01 15:12:26.000000 deeporigin-0.0.5/deeporigin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-01 15:12:26.000000 deeporigin-0.0.5/deeporigin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-01 15:12:26.000000 deeporigin-0.0.5/deeporigin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-01 15:12:23.000000 deeporigin-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 15:12:26.922603 deeporigin-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:12:26.914602 deeporigin-0.0.5/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-01 15:12:24.000000 deeporigin-0.0.5/src/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:12:26.914602 deeporigin-0.0.5/src/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/cli/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/cli/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11909 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/cli/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14212 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/cli/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:12:26.914602 deeporigin-0.0.5/src/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/config/default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5195 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/do_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/feature_flags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:12:26.914602 deeporigin-0.0.5/src/managed_data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/managed_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8487 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/managed_data/_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15869 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/managed_data/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9305 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/managed_data/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/managed_data/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:12:26.918603 deeporigin-0.0.5/src/variables/
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/variables/base_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20324 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/variables/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:12:26.918603 deeporigin-0.0.5/src/variables/types/
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/variables/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/variables/types/anthropic_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11608 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/variables/types/aws_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9728 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/variables/types/env_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/variables/types/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8402 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/variables/types/git_http_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/variables/types/gurobi_license_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/variables/types/mosek_license_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/variables/types/open_ai_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5606 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/variables/types/private_gpg_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/variables/types/private_ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/variables/types/secret_env_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/variables/types/secret_env_var_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/variables/types/secret_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/variables/types/secret_file_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/variables/types/xpress_license_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:12:26.918603 deeporigin-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-01 15:12:23.000000 deeporigin-0.0.5/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-01 15:12:23.000000 deeporigin-0.0.5/tests/test_cli_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5850 2024-05-01 15:12:23.000000 deeporigin-0.0.5/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9024 2024-05-01 15:12:23.000000 deeporigin-0.0.5/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-01 15:12:23.000000 deeporigin-0.0.5/tests/test_feature_flags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10328 2024-05-01 15:12:23.000000 deeporigin-0.0.5/tests/test_managed_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    90063 2024-05-01 15:12:23.000000 deeporigin-0.0.5/tests/test_variables.py
```

### Comparing `deeporigin-0.0.4/LICENSE.txt` & `deeporigin-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.4/PKG-INFO` & `deeporigin-0.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deeporigin
-Version: 0.0.4
+Version: 0.0.5
 Summary: Command line tool and Python client for working with Deep Origin
 Author-email: Deep Origin <support@deeporigin.com>
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Utilities
```

### Comparing `deeporigin-0.0.4/README.md` & `deeporigin-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.4/deeporigin.egg-info/PKG-INFO` & `deeporigin-0.0.5/deeporigin.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deeporigin
-Version: 0.0.4
+Version: 0.0.5
 Summary: Command line tool and Python client for working with Deep Origin
 Author-email: Deep Origin <support@deeporigin.com>
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Utilities
```

### Comparing `deeporigin-0.0.4/deeporigin.egg-info/SOURCES.txt` & `deeporigin-0.0.5/deeporigin.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 src/context.py
 src/do_api.py
 src/exceptions.py
 src/feature_flags.py
 src/utils.py
 src/warnings.py
 src/cli/__init__.py
+src/cli/auth.py
 src/cli/context.py
 src/cli/data.py
 src/cli/variables.py
 src/config/__init__.py
 src/config/default.yml
 src/managed_data/__init__.py
 src/managed_data/_api.py
```

### Comparing `deeporigin-0.0.4/pyproject.toml` & `deeporigin-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.4/src/cli/__init__.py` & `deeporigin-0.0.5/src/cli/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import cement
 import termcolor
 
 from .. import __version__
 from ..exceptions import DeepOriginException
 from ..warnings import DeepOriginWarning
+from .auth import CONTROLLERS as AUTH_CONTROLLERS
 from .context import CONTROLLERS as CONTEXT_CONTROLLERS
 from .data import CONTROLLERS as DATA_CONTROLLERS
 from .variables import CONTROLLERS as VARIABLE_CONTROLLERS
 
 __all__ = ["main", "App"]
 
 
@@ -47,14 +48,15 @@
         label = "deep-origin"
         base_controller = "base"
         handlers = (
             [BaseController]
             + VARIABLE_CONTROLLERS
             + CONTEXT_CONTROLLERS
             + DATA_CONTROLLERS
+            + AUTH_CONTROLLERS
         )
 
 
 def except_hook(built_in_except_hook, type, value, tb):
     if issubclass(type, DeepOriginException):
         sys.stderr.write(termcolor.colored(value, "red") + "\n")
     else:
```

### Comparing `deeporigin-0.0.4/src/cli/context.py` & `deeporigin-0.0.5/src/cli/context.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.4/src/cli/data.py` & `deeporigin-0.0.5/src/cli/data.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.4/src/cli/variables.py` & `deeporigin-0.0.5/src/cli/variables.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.4/src/config/__init__.py` & `deeporigin-0.0.5/src/config/__init__.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.4/src/config/default.yml` & `deeporigin-0.0.5/src/config/default.yml`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.4/src/context.py` & `deeporigin-0.0.5/src/context.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.4/src/do_api.py` & `deeporigin-0.0.5/src/do_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import functools
 import json
 import os
 import time
+from urllib.parse import urljoin
 
 import requests
 
 from .config import get_value as get_config
 from .exceptions import DeepOriginException
 
 __all__ = [
@@ -15,33 +16,36 @@
     "remove_cached_do_api_tokens",
     "sign_into_do_platform",
     "refresh_access_to_do_platform",
 ]
 
 
 @functools.cache
-def get_do_api_tokens() -> tuple[str, str]:
+def get_do_api_tokens(verbose: bool = False) -> tuple[str, str]:
     """Get a token for accessing the Deep Origin API
 
     If the user already has a token, refresh it. If not, sign into the Deep Origin platform.
     Then cache the new or refreshed token.
 
     Returns:
         :obj:`tuple`: API access and refresh tokens
     """
     config = get_config()
 
     if os.path.isfile(config.api_tokens_filename):
+        if verbose:
+            print("Refreshing existing tokens...")
         tokens = read_cached_do_api_tokens()
         refresh_token = tokens["refresh"]
 
         access_token = refresh_access_to_do_platform(refresh_token)
 
     else:
-        print("No cached file, signing in...")
+        if verbose:
+            print("No cached tokens. Signing into Deep Origin...")
         access_token, refresh_token = sign_into_do_platform()
 
     return access_token, refresh_token
 
 
 def cache_do_api_tokens(access_token: str, refresh_token: str) -> None:
     """Save access and refresh tokens to a local file, for example, to
@@ -85,15 +89,15 @@
     Returns:
         :obj:`tuple`: API access token, API refresh token
     """
 
     config = get_config()
 
     # Get a link for the user to sign into the Deep Origin platform
-    endpoint = f"{config.auth_domain}{config.auth_device_code_endpoint}"
+    endpoint = urljoin(config.auth_domain, config.auth_device_code_endpoint)
     body = {
         "client_id": config.auth_client_id,
         "scope": "offline_access",
         "audience": config.auth_audience,
     }
 
     response = requests.post(endpoint, json=body)
@@ -111,15 +115,15 @@
             f"navigate your browser to \n\n{verification_url}\n\n"
             f'and verify the confirmation code is "{user_code}", '
             'and click the "Confirm" button.'
         )
     )
 
     # Wait for the user to sign into the Deep Origin platform
-    endpoint = f"{config.auth_domain}{config.auth_token_endpoint}"
+    endpoint = urljoin(config.auth_domain, config.auth_token_endpoint)
     body = {
         "grant_type": config.auth_grant_type,
         "device_code": device_code,
         "client_id": config.auth_client_id,
     }
     while True:
         response = requests.post(endpoint, json=body)
@@ -148,15 +152,15 @@
         api_refresh_token (:obj:`str`): API refresh token
 
     Returns:
         :obj:`str`: new API access token
     """
     config = get_config()
 
-    endpoint = f"{config.auth_domain}{config.auth_token_endpoint}"
+    endpoint = urljoin(config.auth_domain, config.auth_token_endpoint)
     body = {
         "grant_type": "refresh_token",
         "client_id": config.auth_client_id,
         "client_secret": config.auth_client_secret,
         "refresh_token": api_refresh_token,
     }
     response = requests.post(endpoint, json=body)
```

### Comparing `deeporigin-0.0.4/src/feature_flags.py` & `deeporigin-0.0.5/src/feature_flags.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.4/src/managed_data/_api.py` & `deeporigin-0.0.5/src/managed_data/_api.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.4/src/managed_data/api.py` & `deeporigin-0.0.5/src/managed_data/api.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.4/src/managed_data/client.py` & `deeporigin-0.0.5/src/managed_data/client.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.4/src/managed_data/schema.py` & `deeporigin-0.0.5/src/managed_data/schema.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.4/src/utils.py` & `deeporigin-0.0.5/src/utils.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.4/src/variables/base_type.py` & `deeporigin-0.0.5/src/variables/base_type.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.4/src/variables/core.py` & `deeporigin-0.0.5/src/variables/core.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.4/src/variables/types/__init__.py` & `deeporigin-0.0.5/src/variables/types/__init__.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.4/src/variables/types/aws_profile.py` & `deeporigin-0.0.5/src/variables/types/aws_profile.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.4/src/variables/types/env_var.py` & `deeporigin-0.0.5/src/variables/types/env_var.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.4/src/variables/types/file.py` & `deeporigin-0.0.5/src/variables/types/file.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.4/src/variables/types/git_http_credentials.py` & `deeporigin-0.0.5/src/variables/types/git_http_credentials.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.4/src/variables/types/private_gpg_key.py` & `deeporigin-0.0.5/src/variables/types/private_gpg_key.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.4/src/variables/types/private_ssh_key.py` & `deeporigin-0.0.5/src/variables/types/private_ssh_key.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.4/src/variables/types/secret_env_var_value.py` & `deeporigin-0.0.5/src/variables/types/secret_env_var_value.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.4/src/variables/types/secret_file_value.py` & `deeporigin-0.0.5/src/variables/types/secret_file_value.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.4/src/variables/types/xpress_license_file.py` & `deeporigin-0.0.5/src/variables/types/xpress_license_file.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.4/tests/test_cli.py` & `deeporigin-0.0.5/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.4/tests/test_cli_data.py` & `deeporigin-0.0.5/tests/test_cli_data.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.4/tests/test_config.py` & `deeporigin-0.0.5/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.4/tests/test_context.py` & `deeporigin-0.0.5/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.4/tests/test_feature_flags.py` & `deeporigin-0.0.5/tests/test_feature_flags.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.4/tests/test_managed_data.py` & `deeporigin-0.0.5/tests/test_managed_data.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.4/tests/test_variables.py` & `deeporigin-0.0.5/tests/test_variables.py`

 * *Files identical despite different names*

