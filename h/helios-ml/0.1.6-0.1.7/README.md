# Comparing `tmp/helios_ml-0.1.6.tar.gz` & `tmp/helios_ml-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helios_ml-0.1.6.tar", last modified: Fri Apr 26 22:59:01 2024, max compression
+gzip compressed data, was "helios_ml-0.1.7.tar", last modified: Wed May  1 19:54:10 2024, max compression
```

## Comparing `helios_ml-0.1.6.tar` & `helios_ml-0.1.7.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:59:01.313719 helios_ml-0.1.6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:59:01.293719 helios_ml-0.1.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:59:01.297719 helios_ml-0.1.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-26 22:58:24.000000 helios_ml-0.1.6/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-26 22:58:24.000000 helios_ml-0.1.6/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-26 22:58:24.000000 helios_ml-0.1.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-26 22:58:24.000000 helios_ml-0.1.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-26 22:58:24.000000 helios_ml-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-04-26 22:59:01.313719 helios_ml-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5351 2024-04-26 22:58:24.000000 helios_ml-0.1.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:59:01.293719 helios_ml-0.1.6/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:59:01.297719 helios_ml-0.1.6/data/logo/
--rw-r--r--   0 runner    (1001) docker     (127)    20058 2024-04-26 22:58:24.000000 helios_ml-0.1.6/data/logo/logo-background.png
--rw-r--r--   0 runner    (1001) docker     (127)    14627 2024-04-26 22:58:24.000000 helios_ml-0.1.6/data/logo/logo-transparent.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:59:01.293719 helios_ml-0.1.6/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:59:01.297719 helios_ml-0.1.6/examples/cifar10/
--rw-r--r--   0 runner    (1001) docker     (127)    11404 2024-04-26 22:58:24.000000 helios_ml-0.1.6/examples/cifar10/cifar10.py
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-04-26 22:58:24.000000 helios_ml-0.1.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:59:01.301719 helios_ml-0.1.6/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-26 22:58:24.000000 helios_ml-0.1.6/requirements/ci.txt
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-26 22:58:24.000000 helios_ml-0.1.6/requirements/default.txt
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-26 22:58:24.000000 helios_ml-0.1.6/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 22:59:01.313719 helios_ml-0.1.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:59:01.297719 helios_ml-0.1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:59:01.301719 helios_ml-0.1.6/src/helios/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-26 22:58:24.000000 helios_ml-0.1.6/src/helios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-26 22:58:24.000000 helios_ml-0.1.6/src/helios/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:59:01.301719 helios_ml-0.1.6/src/helios/core/
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-26 22:58:24.000000 helios_ml-0.1.6/src/helios/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-26 22:58:24.000000 helios_ml-0.1.6/src/helios/core/cuda.py
--rw-r--r--   0 runner    (1001) docker     (127)     5408 2024-04-26 22:58:24.000000 helios_ml-0.1.6/src/helios/core/distributed.py
--rw-r--r--   0 runner    (1001) docker     (127)    17255 2024-04-26 22:58:24.000000 helios_ml-0.1.6/src/helios/core/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     4342 2024-04-26 22:58:24.000000 helios_ml-0.1.6/src/helios/core/rng.py
--rw-r--r--   0 runner    (1001) docker     (127)    13539 2024-04-26 22:58:24.000000 helios_ml-0.1.6/src/helios/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:59:01.301719 helios_ml-0.1.6/src/helios/data/
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-26 22:58:24.000000 helios_ml-0.1.6/src/helios/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12644 2024-04-26 22:58:24.000000 helios_ml-0.1.6/src/helios/data/datamodule.py
--rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-04-26 22:58:24.000000 helios_ml-0.1.6/src/helios/data/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)     7733 2024-04-26 22:58:24.000000 helios_ml-0.1.6/src/helios/data/samplers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-04-26 22:58:24.000000 helios_ml-0.1.6/src/helios/data/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:59:01.301719 helios_ml-0.1.6/src/helios/losses/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-26 22:58:24.000000 helios_ml-0.1.6/src/helios/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-26 22:58:24.000000 helios_ml-0.1.6/src/helios/losses/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-26 22:58:24.000000 helios_ml-0.1.6/src/helios/losses/weighted_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:59:01.301719 helios_ml-0.1.6/src/helios/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-26 22:58:24.000000 helios_ml-0.1.6/src/helios/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13882 2024-04-26 22:58:24.000000 helios_ml-0.1.6/src/helios/metrics/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)     7376 2024-04-26 22:58:24.000000 helios_ml-0.1.6/src/helios/metrics/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:59:01.305719 helios_ml-0.1.6/src/helios/model/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-26 22:58:24.000000 helios_ml-0.1.6/src/helios/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13012 2024-04-26 22:58:24.000000 helios_ml-0.1.6/src/helios/model/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-26 22:58:24.000000 helios_ml-0.1.6/src/helios/model/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:59:01.305719 helios_ml-0.1.6/src/helios/nn/
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-26 22:58:24.000000 helios_ml-0.1.6/src/helios/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-04-26 22:58:24.000000 helios_ml-0.1.6/src/helios/nn/swa_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-26 22:58:24.000000 helios_ml-0.1.6/src/helios/nn/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-26 22:58:24.000000 helios_ml-0.1.6/src/helios/onnx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:59:01.305719 helios_ml-0.1.6/src/helios/optim/
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-26 22:58:24.000000 helios_ml-0.1.6/src/helios/optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-26 22:58:24.000000 helios_ml-0.1.6/src/helios/optim/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 22:58:24.000000 helios_ml-0.1.6/src/helios/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:59:01.305719 helios_ml-0.1.6/src/helios/scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-26 22:58:24.000000 helios_ml-0.1.6/src/helios/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-04-26 22:58:24.000000 helios_ml-0.1.6/src/helios/scheduler/schedulers.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-26 22:58:24.000000 helios_ml-0.1.6/src/helios/scheduler/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    36997 2024-04-26 22:58:24.000000 helios_ml-0.1.6/src/helios/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:59:01.309719 helios_ml-0.1.6/src/helios_ml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-04-26 22:59:01.000000 helios_ml-0.1.6/src/helios_ml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-26 22:59:01.000000 helios_ml-0.1.6/src/helios_ml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 22:59:01.000000 helios_ml-0.1.6/src/helios_ml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-26 22:59:01.000000 helios_ml-0.1.6/src/helios_ml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-26 22:59:01.000000 helios_ml-0.1.6/src/helios_ml.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:59:01.309719 helios_ml-0.1.6/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 22:58:24.000000 helios_ml-0.1.6/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-04-26 22:58:24.000000 helios_ml-0.1.6/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:59:01.309719 helios_ml-0.1.6/test/registry_test/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-26 22:58:24.000000 helios_ml-0.1.6/test/registry_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-26 22:58:24.000000 helios_ml-0.1.6/test/registry_test/extra.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-26 22:58:24.000000 helios_ml-0.1.6/test/registry_test/foo.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-26 22:58:24.000000 helios_ml-0.1.6/test/registry_test/func_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:59:01.309719 helios_ml-0.1.6/test/registry_test/nested/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 22:58:24.000000 helios_ml-0.1.6/test/registry_test/nested/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-26 22:58:24.000000 helios_ml-0.1.6/test/registry_test/nested/bar.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-26 22:58:24.000000 helios_ml-0.1.6/test/registry_test/nested/extra.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 22:58:24.000000 helios_ml-0.1.6/test/registry_test/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-04-26 22:58:24.000000 helios_ml-0.1.6/test/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     7923 2024-04-26 22:58:24.000000 helios_ml-0.1.6/test/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-26 22:58:24.000000 helios_ml-0.1.6/test/test_losses.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-26 22:58:24.000000 helios_ml-0.1.6/test/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-04-26 22:58:24.000000 helios_ml-0.1.6/test/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-26 22:58:24.000000 helios_ml-0.1.6/test/test_nn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-26 22:58:24.000000 helios_ml-0.1.6/test/test_onnx.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-26 22:58:24.000000 helios_ml-0.1.6/test/test_optim.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-26 22:58:24.000000 helios_ml-0.1.6/test/test_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)    11800 2024-04-26 22:58:24.000000 helios_ml-0.1.6/test/test_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:59:01.309719 helios_ml-0.1.6/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-26 22:58:24.000000 helios_ml-0.1.6/tools/generate_requirements.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:54:10.419554 helios_ml-0.1.7/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:54:10.403554 helios_ml-0.1.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:54:10.407554 helios_ml-0.1.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-01 19:53:38.000000 helios_ml-0.1.7/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-01 19:53:38.000000 helios_ml-0.1.7/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-01 19:53:38.000000 helios_ml-0.1.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-01 19:53:38.000000 helios_ml-0.1.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-01 19:53:38.000000 helios_ml-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-05-01 19:54:10.419554 helios_ml-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5351 2024-05-01 19:53:38.000000 helios_ml-0.1.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:54:10.403554 helios_ml-0.1.7/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:54:10.407554 helios_ml-0.1.7/data/logo/
+-rw-r--r--   0 runner    (1001) docker     (127)    20058 2024-05-01 19:53:38.000000 helios_ml-0.1.7/data/logo/logo-background.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14627 2024-05-01 19:53:38.000000 helios_ml-0.1.7/data/logo/logo-transparent.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:54:10.403554 helios_ml-0.1.7/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:54:10.407554 helios_ml-0.1.7/examples/cifar10/
+-rw-r--r--   0 runner    (1001) docker     (127)    11404 2024-05-01 19:53:38.000000 helios_ml-0.1.7/examples/cifar10/cifar10.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-05-01 19:53:38.000000 helios_ml-0.1.7/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:54:10.407554 helios_ml-0.1.7/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-01 19:53:38.000000 helios_ml-0.1.7/requirements/ci.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-01 19:53:38.000000 helios_ml-0.1.7/requirements/default.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-01 19:53:38.000000 helios_ml-0.1.7/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 19:54:10.419554 helios_ml-0.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:54:10.403554 helios_ml-0.1.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:54:10.407554 helios_ml-0.1.7/src/helios/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:54:10.407554 helios_ml-0.1.7/src/helios/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/core/cuda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7242 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/core/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17255 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/core/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4342 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/core/rng.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13539 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:54:10.411554 helios_ml-0.1.7/src/helios/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12644 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/data/datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/data/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7733 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/data/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/data/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:54:10.411554 helios_ml-0.1.7/src/helios/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/losses/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/losses/weighted_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:54:10.411554 helios_ml-0.1.7/src/helios/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13882 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/metrics/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7376 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/metrics/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:54:10.411554 helios_ml-0.1.7/src/helios/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13012 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/model/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/model/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:54:10.411554 helios_ml-0.1.7/src/helios/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/nn/swa_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/nn/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/onnx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:54:10.411554 helios_ml-0.1.7/src/helios/optim/
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/optim/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:54:10.411554 helios_ml-0.1.7/src/helios/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/scheduler/schedulers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/scheduler/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35609 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:54:10.415554 helios_ml-0.1.7/src/helios_ml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-05-01 19:54:10.000000 helios_ml-0.1.7/src/helios_ml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-01 19:54:10.000000 helios_ml-0.1.7/src/helios_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 19:54:10.000000 helios_ml-0.1.7/src/helios_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-01 19:54:10.000000 helios_ml-0.1.7/src/helios_ml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-01 19:54:10.000000 helios_ml-0.1.7/src/helios_ml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:54:10.415554 helios_ml-0.1.7/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 19:53:38.000000 helios_ml-0.1.7/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-05-01 19:53:38.000000 helios_ml-0.1.7/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:54:10.415554 helios_ml-0.1.7/test/registry_test/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-01 19:53:38.000000 helios_ml-0.1.7/test/registry_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-01 19:53:38.000000 helios_ml-0.1.7/test/registry_test/extra.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-01 19:53:38.000000 helios_ml-0.1.7/test/registry_test/foo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-01 19:53:38.000000 helios_ml-0.1.7/test/registry_test/func_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:54:10.415554 helios_ml-0.1.7/test/registry_test/nested/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 19:53:38.000000 helios_ml-0.1.7/test/registry_test/nested/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-01 19:53:38.000000 helios_ml-0.1.7/test/registry_test/nested/bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-01 19:53:38.000000 helios_ml-0.1.7/test/registry_test/nested/extra.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 19:53:38.000000 helios_ml-0.1.7/test/registry_test/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-05-01 19:53:38.000000 helios_ml-0.1.7/test/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7923 2024-05-01 19:53:38.000000 helios_ml-0.1.7/test/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-01 19:53:38.000000 helios_ml-0.1.7/test/test_losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-01 19:53:38.000000 helios_ml-0.1.7/test/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-05-01 19:53:38.000000 helios_ml-0.1.7/test/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-01 19:53:38.000000 helios_ml-0.1.7/test/test_nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-01 19:53:38.000000 helios_ml-0.1.7/test/test_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-01 19:53:38.000000 helios_ml-0.1.7/test/test_optim.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-01 19:53:38.000000 helios_ml-0.1.7/test/test_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11800 2024-05-01 19:53:38.000000 helios_ml-0.1.7/test/test_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:54:10.415554 helios_ml-0.1.7/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-01 19:53:38.000000 helios_ml-0.1.7/tools/generate_requirements.py
```

### Comparing `helios_ml-0.1.6/.github/workflows/publish.yml` & `helios_ml-0.1.7/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.6/.github/workflows/tests.yml` & `helios_ml-0.1.7/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.6/.pre-commit-config.yaml` & `helios_ml-0.1.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.6/LICENSE` & `helios_ml-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.6/PKG-INFO` & `helios_ml-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helios-ml
-Version: 0.1.6
+Version: 0.1.7
 Summary: A light-weight system for training AI networks using PyTorch
 Author-email: "Mauricio A. Rovira Galvez" <maroviragalvez@outlook.com>
 License: BSD-3-Clause
 Project-URL: homepage, https://github.com/marovira/helios-ml
 Project-URL: source, https://github.com/marovira/helios-ml
 Project-URL: issues, https://github.com/marovira/helios-ml/issues
 Project-URL: release notes, https://github.com/marovira/helios-ml/releases
```

### Comparing `helios_ml-0.1.6/README.rst` & `helios_ml-0.1.7/README.rst`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.6/data/logo/logo-background.png` & `helios_ml-0.1.7/data/logo/logo-background.png`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.6/data/logo/logo-transparent.png` & `helios_ml-0.1.7/data/logo/logo-transparent.png`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.6/examples/cifar10/cifar10.py` & `helios_ml-0.1.7/examples/cifar10/cifar10.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.6/pyproject.toml` & `helios_ml-0.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.6/src/helios/core/__init__.py` & `helios_ml-0.1.7/src/helios/core/__init__.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.6/src/helios/core/cuda.py` & `helios_ml-0.1.7/src/helios/core/cuda.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.6/src/helios/core/logging.py` & `helios_ml-0.1.7/src/helios/core/logging.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.6/src/helios/core/rng.py` & `helios_ml-0.1.7/src/helios/core/rng.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.6/src/helios/core/utils.py` & `helios_ml-0.1.7/src/helios/core/utils.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.6/src/helios/data/__init__.py` & `helios_ml-0.1.7/src/helios/data/__init__.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.6/src/helios/data/datamodule.py` & `helios_ml-0.1.7/src/helios/data/datamodule.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.6/src/helios/data/functional.py` & `helios_ml-0.1.7/src/helios/data/functional.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.6/src/helios/data/samplers.py` & `helios_ml-0.1.7/src/helios/data/samplers.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.6/src/helios/data/transforms.py` & `helios_ml-0.1.7/src/helios/data/transforms.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.6/src/helios/losses/utils.py` & `helios_ml-0.1.7/src/helios/losses/utils.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.6/src/helios/losses/weighted_loss.py` & `helios_ml-0.1.7/src/helios/losses/weighted_loss.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.6/src/helios/metrics/functional.py` & `helios_ml-0.1.7/src/helios/metrics/functional.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.6/src/helios/metrics/metrics.py` & `helios_ml-0.1.7/src/helios/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.6/src/helios/model/model.py` & `helios_ml-0.1.7/src/helios/model/model.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.6/src/helios/model/utils.py` & `helios_ml-0.1.7/src/helios/model/utils.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.6/src/helios/nn/swa_utils.py` & `helios_ml-0.1.7/src/helios/nn/swa_utils.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.6/src/helios/nn/utils.py` & `helios_ml-0.1.7/src/helios/nn/utils.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.6/src/helios/onnx.py` & `helios_ml-0.1.7/src/helios/onnx.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.6/src/helios/optim/utils.py` & `helios_ml-0.1.7/src/helios/optim/utils.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.6/src/helios/scheduler/schedulers.py` & `helios_ml-0.1.7/src/helios/scheduler/schedulers.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.6/src/helios/scheduler/utils.py` & `helios_ml-0.1.7/src/helios/scheduler/utils.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.6/src/helios/trainer.py` & `helios_ml-0.1.7/src/helios/trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import os
 import pathlib
 import re
 import time
 import typing
 
 import torch
-import torch.distributed as td
 import torch.multiprocessing as mp
 import torch.utils.data as tud
 import tqdm
 
 import helios.model as hlm
 from helios import core, data
 from helios.core import distributed as dist
@@ -223,15 +222,14 @@
         import_prefix: str = "",
     ):
         """Create the trainer."""
         self._model: hlm.Model | None = None
         self._datamodule: data.DataModule | None = None
         self._local_rank: int = 0
         self._rank: int = 0
-        self._callbacks: dict[str, typing.Callable] = {}
 
         self._use_cpu: bool = False
         self._device: torch.device | None = None
         self._map_loc: str | dict[str, str] = ""
         self._gpu_ids: list[int] = [] if gpus is None else gpus
         self._active_gpu: int = 0
         self._is_distributed: bool = False
@@ -305,36 +303,14 @@
         self._rank = r
 
     @property
     def gpu_ids(self) -> list[int]:
         """Return the list of GPU IDs to use for training."""
         return self._gpu_ids
 
-    @property
-    def callbacks(self) -> dict[str, typing.Callable]:
-        """Return the table of callbacks."""
-        return self._callbacks
-
-    def register_callback(self, name: str, callback: typing.Callable) -> None:
-        """
-        Register a callback.
-
-        Callbacks are used to inject additional code or behaviour into the training code.
-        You may call these at any time through the trainer instance that is attached to
-        the datamodule and the model.
-
-        Args:
-            name (str): the name of the callback.
-            callback (typing.Callable): the callback to register.
-        """
-        if name in self._callbacks:
-            raise KeyError(f"error: {name} has already been registered as a callback")
-
-        self._callbacks[name] = callback
-
     def fit(self, model: hlm.Model, datamodule: data.DataModule) -> None:
         """
         Run the full training routine.
 
         Args:
             model (pym.Model): the model to run on.
             datamodule (data.DataModule): the datamodule to use.
@@ -431,16 +407,15 @@
 
         self.model.on_training_end()
 
         logging.flush_default_loggers()
         logging.close_default_loggers()
 
         # If we're distributed, ensure that all processes are caught up before we exit.
-        if self._is_distributed:
-            td.barrier()
+        dist.safe_barrier()
 
     def _test(self) -> None:
         """
         Test the model.
 
         This will ensure everything gets correctly initialised and run the testing loop on
         the dataset.
@@ -494,16 +469,15 @@
                     self.model.on_testing_batch_start(idx)
                     self.model.test_step(batch, idx)
                     self.model.on_testing_batch_end(idx)
                     pbar.update()
 
             self.model.on_testing_end()
 
-        if self._is_distributed:
-            td.barrier()
+        dist.safe_barrier()
 
     def _configure_env(self) -> None:
         """
         Configure the training environment.
 
         This will seed the RNGs as well as setup any CUDA state (if using). It will also
         set all of the registries provided the source root is not None. This is to prevent
@@ -563,32 +537,32 @@
 
     def _print_header(
         self, chkpt_path: pathlib.Path | None, for_training: bool = True
     ) -> None:
         """Print the Helios header with system info to the logs."""
         root_logger = logging.get_root_logger()
 
-        self._print(core.get_env_info_str())
+        dist.global_print(core.get_env_info_str())
 
         if for_training:
             if chkpt_path is not None:
                 msg = f"Resuming training from checkpoint {str(chkpt_path)}"
                 root_logger.info(msg)
-                self._print(f"{msg}\n")
+                dist.global_print(f"{msg}\n")
             else:
                 root_logger.info(core.get_env_info_str())
         else:
             root_logger.info(core.get_env_info_str())
             msg = (
                 f"Testing using checkpoint {str(chkpt_path)}"
                 if chkpt_path is not None
                 else "Testing from loaded model"
             )
             root_logger.info(msg)
-            self._print(f"{msg}\n")
+            dist.global_print(f"{msg}\n")
 
     def _validate_flags(self):
         """Ensure that all the settings and flags are valid."""
         if isinstance(self._total_steps, float) and self._total_steps != float("inf"):
             raise ValueError(
                 "error: expected 'total_steps' to be of type 'int' or 'infinity', but "
                 f"received {self._total_steps}"
@@ -797,22 +771,22 @@
                 break
             root_logger.info(f"Starting epoch {epoch + 1}")
             sampler.set_epoch(epoch)
             epoch_start = time.time()
 
             iter_timer.start()
             for batch in dataloader:
+                state.global_iteration += 1
                 if state.global_iteration % accumulation_steps == 0:
                     state.current_iteration += 1
                     state.running_iter += 1
                     current_iteration_changed = True
                 else:
                     current_iteration_changed = False
 
-                state.global_iteration += 1
                 if state.current_iteration > total_steps:
                     training_done = True
                     break
 
                 self.model.on_training_batch_start(state)
                 self.model.train_step(batch, state)
                 iter_timer.record()
@@ -849,25 +823,27 @@
                     save_freq is not None
                     and state.current_iteration % save_freq == 0
                     and self.rank == 0
                     and current_iteration_changed
                 ):
                     self._save_checkpoint(state)
 
+                if (
+                    early_stop_cycles is not None
+                    and state.early_stop_count >= early_stop_cycles
+                ):
+                    training_done = True
+                    break
+
             state.dataset_iter = 0
             state.global_epoch += 1
 
             root_logger.info(
                 f"Epoch {epoch + 1} completed in {time.time() - epoch_start:.2f}s"
             )
-            if (
-                early_stop_cycles is not None
-                and state.early_stop_count >= early_stop_cycles
-            ):
-                training_done = True
 
     def _train_on_epoch(self, state: TrainingState) -> None:
         """
         Run the main loop for epoch-based training.
 
         Args:
             state (TrainingState): the training state.
@@ -1012,24 +988,8 @@
                     # loop runs faster than the refresh rate of the progress bar.
                     if not pbar.update():
                         pbar.refresh()
 
             self.model.train()
             self.model.on_validation_end(val_cycle)
 
-        if self._is_distributed:
-            td.barrier()
-
-    def _print(self, *args: typing.Any, **kwargs: typing.Any) -> None:
-        """
-        Wrap Python's print function for distributed training.
-
-        Specifically, this function will ensure that only rank 0 prints messages to the
-        screen. All other ranks will do nothing.
-
-        Args:
-            args: named arguments for print.
-            kwargs: keyword arguments for print.
-        """
-        if self.rank != 0:
-            return
-        print(*args, **kwargs)
+        dist.safe_barrier()
```

### Comparing `helios_ml-0.1.6/src/helios_ml.egg-info/PKG-INFO` & `helios_ml-0.1.7/src/helios_ml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helios-ml
-Version: 0.1.6
+Version: 0.1.7
 Summary: A light-weight system for training AI networks using PyTorch
 Author-email: "Mauricio A. Rovira Galvez" <maroviragalvez@outlook.com>
 License: BSD-3-Clause
 Project-URL: homepage, https://github.com/marovira/helios-ml
 Project-URL: source, https://github.com/marovira/helios-ml
 Project-URL: issues, https://github.com/marovira/helios-ml/issues
 Project-URL: release notes, https://github.com/marovira/helios-ml/releases
```

### Comparing `helios_ml-0.1.6/src/helios_ml.egg-info/SOURCES.txt` & `helios_ml-0.1.7/src/helios_ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.6/test/conftest.py` & `helios_ml-0.1.7/test/conftest.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.6/test/test_core.py` & `helios_ml-0.1.7/test/test_core.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.6/test/test_data.py` & `helios_ml-0.1.7/test/test_data.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.6/test/test_losses.py` & `helios_ml-0.1.7/test/test_losses.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.6/test/test_metrics.py` & `helios_ml-0.1.7/test/test_metrics.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.6/test/test_model.py` & `helios_ml-0.1.7/test/test_model.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.6/test/test_nn.py` & `helios_ml-0.1.7/test/test_nn.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.6/test/test_onnx.py` & `helios_ml-0.1.7/test/test_onnx.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.6/test/test_trainer.py` & `helios_ml-0.1.7/test/test_trainer.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.6/tools/generate_requirements.py` & `helios_ml-0.1.7/tools/generate_requirements.py`

 * *Files identical despite different names*

