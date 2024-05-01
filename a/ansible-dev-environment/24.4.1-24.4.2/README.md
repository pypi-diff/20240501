# Comparing `tmp/ansible_dev_environment-24.4.1.tar.gz` & `tmp/ansible_dev_environment-24.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible_dev_environment-24.4.1.tar", last modified: Mon Apr 29 23:03:54 2024, max compression
+gzip compressed data, was "ansible_dev_environment-24.4.2.tar", last modified: Wed May  1 16:24:46 2024, max compression
```

## Comparing `ansible_dev_environment-24.4.1.tar` & `ansible_dev_environment-24.4.2.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:03:54.177497 ansible_dev_environment-24.4.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:03:54.165497 ansible_dev_environment-24.4.1/.config/
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/.config/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/.config/dictionary.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/.config/requirements-dev.in
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/.config/requirements-docs.in
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/.config/requirements-test.in
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/.config/requirements.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:03:54.169497 ansible_dev_environment-24.4.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:03:54.169497 ansible_dev_environment-24.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/.github/workflows/ack.yml
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/.github/workflows/push.yml
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/.readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:03:54.169497 ansible_dev_environment-24.4.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-04-29 23:03:54.177497 ansible_dev_environment-24.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/cspell.config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:03:54.169497 ansible_dev_environment-24.4.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)    14492 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 23:03:54.177497 ansible_dev_environment-24.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:03:54.161497 ansible_dev_environment-24.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:03:54.169497 ansible_dev_environment-24.4.1/src/ansible_dev_environment/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/src/ansible_dev_environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/src/ansible_dev_environment/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-29 23:03:54.000000 ansible_dev_environment-24.4.1/src/ansible_dev_environment/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7412 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/src/ansible_dev_environment/arg_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/src/ansible_dev_environment/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     6222 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/src/ansible_dev_environment/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     6078 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/src/ansible_dev_environment/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9645 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/src/ansible_dev_environment/output.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:03:54.173497 ansible_dev_environment-24.4.1/src/ansible_dev_environment/subcommands/
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/src/ansible_dev_environment/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8161 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/src/ansible_dev_environment/subcommands/checker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/src/ansible_dev_environment/subcommands/inspector.py
--rw-r--r--   0 runner    (1001) docker     (127)    18398 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/src/ansible_dev_environment/subcommands/installer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/src/ansible_dev_environment/subcommands/lister.py
--rw-r--r--   0 runner    (1001) docker     (127)     6055 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/src/ansible_dev_environment/subcommands/treemaker.py
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/src/ansible_dev_environment/subcommands/uninstaller.py
--rw-r--r--   0 runner    (1001) docker     (127)     5555 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/src/ansible_dev_environment/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)    14630 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/src/ansible_dev_environment/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:03:54.177497 ansible_dev_environment-24.4.1/src/ansible_dev_environment.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-04-29 23:03:54.000000 ansible_dev_environment-24.4.1/src/ansible_dev_environment.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-29 23:03:54.000000 ansible_dev_environment-24.4.1/src/ansible_dev_environment.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 23:03:54.000000 ansible_dev_environment-24.4.1/src/ansible_dev_environment.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-29 23:03:54.000000 ansible_dev_environment-24.4.1/src/ansible_dev_environment.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-29 23:03:54.000000 ansible_dev_environment-24.4.1/src/ansible_dev_environment.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-29 23:03:54.000000 ansible_dev_environment-24.4.1/src/ansible_dev_environment.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:03:54.173497 ansible_dev_environment-24.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:03:54.173497 ansible_dev_environment-24.4.1/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/tests/fixtures/galaxy.yml
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/tests/fixtures/requirements.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:03:54.173497 ansible_dev_environment-24.4.1/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/tests/integration/test_basic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:03:54.177497 ansible_dev_environment-24.4.1/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/tests/unit/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/tests/unit/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/tests/unit/test_installer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/tests/unit/test_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:24:46.544136 ansible_dev_environment-24.4.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:24:46.532136 ansible_dev_environment-24.4.2/.config/
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-01 16:24:34.000000 ansible_dev_environment-24.4.2/.config/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-01 16:24:34.000000 ansible_dev_environment-24.4.2/.config/dictionary.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-01 16:24:34.000000 ansible_dev_environment-24.4.2/.config/requirements-dev.in
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-01 16:24:34.000000 ansible_dev_environment-24.4.2/.config/requirements-docs.in
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-01 16:24:34.000000 ansible_dev_environment-24.4.2/.config/requirements-test.in
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 16:24:34.000000 ansible_dev_environment-24.4.2/.config/requirements.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:24:46.536136 ansible_dev_environment-24.4.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-01 16:24:34.000000 ansible_dev_environment-24.4.2/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-01 16:24:34.000000 ansible_dev_environment-24.4.2/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-01 16:24:34.000000 ansible_dev_environment-24.4.2/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-01 16:24:34.000000 ansible_dev_environment-24.4.2/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:24:46.536136 ansible_dev_environment-24.4.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-01 16:24:34.000000 ansible_dev_environment-24.4.2/.github/workflows/ack.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-01 16:24:34.000000 ansible_dev_environment-24.4.2/.github/workflows/push.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-01 16:24:34.000000 ansible_dev_environment-24.4.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-05-01 16:24:34.000000 ansible_dev_environment-24.4.2/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-05-01 16:24:34.000000 ansible_dev_environment-24.4.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-05-01 16:24:34.000000 ansible_dev_environment-24.4.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-01 16:24:34.000000 ansible_dev_environment-24.4.2/.readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:24:46.536136 ansible_dev_environment-24.4.2/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-01 16:24:34.000000 ansible_dev_environment-24.4.2/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-01 16:24:34.000000 ansible_dev_environment-24.4.2/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-01 16:24:34.000000 ansible_dev_environment-24.4.2/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-01 16:24:34.000000 ansible_dev_environment-24.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-05-01 16:24:46.544136 ansible_dev_environment-24.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-05-01 16:24:34.000000 ansible_dev_environment-24.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-01 16:24:34.000000 ansible_dev_environment-24.4.2/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-01 16:24:34.000000 ansible_dev_environment-24.4.2/cspell.config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:24:46.536136 ansible_dev_environment-24.4.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-01 16:24:34.000000 ansible_dev_environment-24.4.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-05-01 16:24:34.000000 ansible_dev_environment-24.4.2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    14492 2024-05-01 16:24:34.000000 ansible_dev_environment-24.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 16:24:46.544136 ansible_dev_environment-24.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:24:46.528136 ansible_dev_environment-24.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:24:46.536136 ansible_dev_environment-24.4.2/src/ansible_dev_environment/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-01 16:24:34.000000 ansible_dev_environment-24.4.2/src/ansible_dev_environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-01 16:24:34.000000 ansible_dev_environment-24.4.2/src/ansible_dev_environment/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-01 16:24:46.000000 ansible_dev_environment-24.4.2/src/ansible_dev_environment/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7412 2024-05-01 16:24:34.000000 ansible_dev_environment-24.4.2/src/ansible_dev_environment/arg_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-05-01 16:24:34.000000 ansible_dev_environment-24.4.2/src/ansible_dev_environment/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6222 2024-05-01 16:24:34.000000 ansible_dev_environment-24.4.2/src/ansible_dev_environment/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7071 2024-05-01 16:24:34.000000 ansible_dev_environment-24.4.2/src/ansible_dev_environment/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9645 2024-05-01 16:24:34.000000 ansible_dev_environment-24.4.2/src/ansible_dev_environment/output.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:24:46.540136 ansible_dev_environment-24.4.2/src/ansible_dev_environment/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-01 16:24:34.000000 ansible_dev_environment-24.4.2/src/ansible_dev_environment/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8161 2024-05-01 16:24:34.000000 ansible_dev_environment-24.4.2/src/ansible_dev_environment/subcommands/checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-01 16:24:34.000000 ansible_dev_environment-24.4.2/src/ansible_dev_environment/subcommands/inspector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18318 2024-05-01 16:24:34.000000 ansible_dev_environment-24.4.2/src/ansible_dev_environment/subcommands/installer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-05-01 16:24:34.000000 ansible_dev_environment-24.4.2/src/ansible_dev_environment/subcommands/lister.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6055 2024-05-01 16:24:34.000000 ansible_dev_environment-24.4.2/src/ansible_dev_environment/subcommands/treemaker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-05-01 16:24:34.000000 ansible_dev_environment-24.4.2/src/ansible_dev_environment/subcommands/uninstaller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5555 2024-05-01 16:24:34.000000 ansible_dev_environment-24.4.2/src/ansible_dev_environment/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14630 2024-05-01 16:24:34.000000 ansible_dev_environment-24.4.2/src/ansible_dev_environment/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:24:46.544136 ansible_dev_environment-24.4.2/src/ansible_dev_environment.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-05-01 16:24:46.000000 ansible_dev_environment-24.4.2/src/ansible_dev_environment.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-01 16:24:46.000000 ansible_dev_environment-24.4.2/src/ansible_dev_environment.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 16:24:46.000000 ansible_dev_environment-24.4.2/src/ansible_dev_environment.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-01 16:24:46.000000 ansible_dev_environment-24.4.2/src/ansible_dev_environment.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-01 16:24:46.000000 ansible_dev_environment-24.4.2/src/ansible_dev_environment.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-01 16:24:46.000000 ansible_dev_environment-24.4.2/src/ansible_dev_environment.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:24:46.540136 ansible_dev_environment-24.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-01 16:24:34.000000 ansible_dev_environment-24.4.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:24:46.540136 ansible_dev_environment-24.4.2/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-01 16:24:34.000000 ansible_dev_environment-24.4.2/tests/fixtures/galaxy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-01 16:24:34.000000 ansible_dev_environment-24.4.2/tests/fixtures/requirements.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:24:46.540136 ansible_dev_environment-24.4.2/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-01 16:24:34.000000 ansible_dev_environment-24.4.2/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-05-01 16:24:34.000000 ansible_dev_environment-24.4.2/tests/integration/test_basic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:24:46.544136 ansible_dev_environment-24.4.2/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-01 16:24:34.000000 ansible_dev_environment-24.4.2/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-01 16:24:34.000000 ansible_dev_environment-24.4.2/tests/unit/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6155 2024-05-01 16:24:34.000000 ansible_dev_environment-24.4.2/tests/unit/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-05-01 16:24:34.000000 ansible_dev_environment-24.4.2/tests/unit/test_installer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-05-01 16:24:34.000000 ansible_dev_environment-24.4.2/tests/unit/test_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-05-01 16:24:34.000000 ansible_dev_environment-24.4.2/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-01 16:24:34.000000 ansible_dev_environment-24.4.2/tox.ini
```

### Comparing `ansible_dev_environment-24.4.1/.config/constraints.txt` & `ansible_dev_environment-24.4.2/.config/constraints.txt`

 * *Files identical despite different names*

### Comparing `ansible_dev_environment-24.4.1/.github/workflows/ack.yml` & `ansible_dev_environment-24.4.2/.github/workflows/ack.yml`

 * *Files identical despite different names*

### Comparing `ansible_dev_environment-24.4.1/.github/workflows/release.yml` & `ansible_dev_environment-24.4.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `ansible_dev_environment-24.4.1/.github/workflows/tox.yml` & `ansible_dev_environment-24.4.2/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `ansible_dev_environment-24.4.1/.gitignore` & `ansible_dev_environment-24.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ansible_dev_environment-24.4.1/.pre-commit-config.yaml` & `ansible_dev_environment-24.4.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ansible_dev_environment-24.4.1/.vscode/launch.json` & `ansible_dev_environment-24.4.2/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `ansible_dev_environment-24.4.1/.vscode/settings.json` & `ansible_dev_environment-24.4.2/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `ansible_dev_environment-24.4.1/LICENSE` & `ansible_dev_environment-24.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible_dev_environment-24.4.1/PKG-INFO` & `ansible_dev_environment-24.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-dev-environment
-Version: 24.4.1
+Version: 24.4.2
 Summary: A pip-like ansible collection installer.
 Author-email: "Bradley A. Thornton" <bthornto@redhat.com>
 Maintainer-email: Bradley Thornton <bthornto@redhat.com>
 License: GPL-3.0-only
 Project-URL: changelog, https://github.com/ansible/ansible-dev-environment/releases
 Project-URL: documentation, https://ansible.readthedocs.io/projects/dev-environment/
 Project-URL: homepage, https://github.com/ansible/ansible-dev-environment
```

### Comparing `ansible_dev_environment-24.4.1/README.md` & `ansible_dev_environment-24.4.2/README.md`

 * *Files identical despite different names*

### Comparing `ansible_dev_environment-24.4.1/cspell.config.yaml` & `ansible_dev_environment-24.4.2/cspell.config.yaml`

 * *Files identical despite different names*

### Comparing `ansible_dev_environment-24.4.1/docs/index.md` & `ansible_dev_environment-24.4.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `ansible_dev_environment-24.4.1/mkdocs.yml` & `ansible_dev_environment-24.4.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ansible_dev_environment-24.4.1/pyproject.toml` & `ansible_dev_environment-24.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansible_dev_environment-24.4.1/src/ansible_dev_environment/arg_parser.py` & `ansible_dev_environment-24.4.2/src/ansible_dev_environment/arg_parser.py`

 * *Files identical despite different names*

### Comparing `ansible_dev_environment-24.4.1/src/ansible_dev_environment/cli.py` & `ansible_dev_environment-24.4.2/src/ansible_dev_environment/cli.py`

 * *Files identical despite different names*

### Comparing `ansible_dev_environment-24.4.1/src/ansible_dev_environment/collection.py` & `ansible_dev_environment-24.4.2/src/ansible_dev_environment/collection.py`

 * *Files identical despite different names*

### Comparing `ansible_dev_environment-24.4.1/src/ansible_dev_environment/config.py` & `ansible_dev_environment-24.4.2/src/ansible_dev_environment/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Constants, for now, for ansible-dev-environment."""
 
 from __future__ import annotations
 
 import json
 import os
+import shutil
 import subprocess
 import sys
 
 from pathlib import Path
 from typing import TYPE_CHECKING
 
 from .utils import subprocess_run
@@ -97,14 +98,39 @@
         return self.venv / "bin"
 
     @property
     def interpreter(self: Config) -> Path:
         """Return the current interpreter."""
         return Path(sys.executable)
 
+    @property
+    def galaxy_bin(self: Config) -> Path | None:
+        """Find the ansible galaxy command.
+
+        Prefer the venv over the system package over the PATH.
+        """
+        within_venv = self.venv_bindir / "ansible-galaxy"
+        if within_venv.exists():
+            msg = f"Found ansible-galaxy in virtual environment: {within_venv}"
+            self._output.debug(msg)
+            return within_venv
+        system_pkg = self.site_pkg_path / "bin" / "ansible-galaxy"
+        if system_pkg.exists():
+            msg = f"Found ansible-galaxy in system packages: {system_pkg}"
+            self._output.debug(msg)
+            return system_pkg
+        last_resort = shutil.which("ansible-galaxy")
+        if last_resort:
+            msg = f"Found ansible-galaxy in PATH: {last_resort}"
+            self._output.debug(msg)
+            return Path(last_resort)
+        msg = "Failed to find ansible-galaxy."
+        self._output.critical(msg)
+        return None
+
     def _set_interpreter(
         self: Config,
     ) -> None:
         """Set the interpreter."""
         if not self.venv.exists():
             if self._create_venv:
                 msg = f"Creating virtual environment: {self.venv}"
```

### Comparing `ansible_dev_environment-24.4.1/src/ansible_dev_environment/output.py` & `ansible_dev_environment-24.4.2/src/ansible_dev_environment/output.py`

 * *Files identical despite different names*

### Comparing `ansible_dev_environment-24.4.1/src/ansible_dev_environment/subcommands/checker.py` & `ansible_dev_environment-24.4.2/src/ansible_dev_environment/subcommands/checker.py`

 * *Files identical despite different names*

### Comparing `ansible_dev_environment-24.4.1/src/ansible_dev_environment/subcommands/inspector.py` & `ansible_dev_environment-24.4.2/src/ansible_dev_environment/subcommands/inspector.py`

 * *Files identical despite different names*

### Comparing `ansible_dev_environment-24.4.1/src/ansible_dev_environment/subcommands/installer.py` & `ansible_dev_environment-24.4.2/src/ansible_dev_environment/subcommands/installer.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,15 +133,15 @@
                 self._output.debug(msg)
                 if collection.site_pkg_path.is_symlink():
                     collection.site_pkg_path.unlink()
                 else:
                     shutil.rmtree(collection.site_pkg_path)
 
         command = (
-            f"{self._config.venv_bindir / 'ansible-galaxy'} collection"
+            f"{self._config.galaxy_bin} collection"
             f" install {collections_str}"
             f" -p {self._config.site_pkg_path}"
             " --force"
         )
         env = {
             "ANSIBLE_GALAXY_COLLECTIONS_PATH_WARNING": str(self._config.args.verbose),
         }
@@ -187,15 +187,15 @@
                 self._output.debug(msg)
                 if cpath.is_symlink():
                     cpath.unlink()
                 else:
                     shutil.rmtree(cpath)
 
         command = (
-            f"{self._config.venv_bindir / 'ansible-galaxy'} collection"
+            f"{self._config.galaxy_bin} collection"
             f" install -r {self._config.args.requirement}"
             f" -p {self._config.site_pkg_path}"
             " --force"
         )
         work = "Install collections from requirements file"
         try:
             proc = subprocess_run(
@@ -355,15 +355,15 @@
         self._copy_repo_files(
             local_repo_path=collection.path,
             destination_path=collection.build_dir,
         )
 
         command = (
             f"cd {collection.build_dir} &&"
-            f" {self._config.venv_bindir / 'ansible-galaxy'} collection build"
+            f" {self._config.galaxy_bin} collection build"
             f" --output-path {collection.build_dir}"
             " --force"
         )
 
         msg = "Running ansible-galaxy to build collection."
         self._output.debug(msg)
 
@@ -408,15 +408,15 @@
         ]
         for info_dir in info_dirs:
             msg = f"Removing installed {info_dir}"
             self._output.debug(msg)
             shutil.rmtree(info_dir)
 
         command = (
-            f"{self._config.venv_bindir / 'ansible-galaxy'} collection"
+            f"{self._config.galaxy_bin} collection"
             f" install {tarball} -p {self._config.site_pkg_path}"
             " --force"
         )
         env = {
             "ANSIBLE_GALAXY_COLLECTIONS_PATH_WARNING": str(self._config.args.verbose),
         }
         msg = "Running ansible-galaxy to install a local collection and it's dependencies."
```

### Comparing `ansible_dev_environment-24.4.1/src/ansible_dev_environment/subcommands/lister.py` & `ansible_dev_environment-24.4.2/src/ansible_dev_environment/subcommands/lister.py`

 * *Files identical despite different names*

### Comparing `ansible_dev_environment-24.4.1/src/ansible_dev_environment/subcommands/treemaker.py` & `ansible_dev_environment-24.4.2/src/ansible_dev_environment/subcommands/treemaker.py`

 * *Files identical despite different names*

### Comparing `ansible_dev_environment-24.4.1/src/ansible_dev_environment/subcommands/uninstaller.py` & `ansible_dev_environment-24.4.2/src/ansible_dev_environment/subcommands/uninstaller.py`

 * *Files identical despite different names*

### Comparing `ansible_dev_environment-24.4.1/src/ansible_dev_environment/tree.py` & `ansible_dev_environment-24.4.2/src/ansible_dev_environment/tree.py`

 * *Files identical despite different names*

### Comparing `ansible_dev_environment-24.4.1/src/ansible_dev_environment/utils.py` & `ansible_dev_environment-24.4.2/src/ansible_dev_environment/utils.py`

 * *Files identical despite different names*

### Comparing `ansible_dev_environment-24.4.1/src/ansible_dev_environment.egg-info/PKG-INFO` & `ansible_dev_environment-24.4.2/src/ansible_dev_environment.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-dev-environment
-Version: 24.4.1
+Version: 24.4.2
 Summary: A pip-like ansible collection installer.
 Author-email: "Bradley A. Thornton" <bthornto@redhat.com>
 Maintainer-email: Bradley Thornton <bthornto@redhat.com>
 License: GPL-3.0-only
 Project-URL: changelog, https://github.com/ansible/ansible-dev-environment/releases
 Project-URL: documentation, https://ansible.readthedocs.io/projects/dev-environment/
 Project-URL: homepage, https://github.com/ansible/ansible-dev-environment
```

### Comparing `ansible_dev_environment-24.4.1/src/ansible_dev_environment.egg-info/SOURCES.txt` & `ansible_dev_environment-24.4.2/src/ansible_dev_environment.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ansible_dev_environment-24.4.1/tests/integration/test_basic.py` & `ansible_dev_environment-24.4.2/tests/integration/test_basic.py`

 * *Files identical despite different names*

### Comparing `ansible_dev_environment-24.4.1/tests/unit/conftest.py` & `ansible_dev_environment-24.4.2/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `ansible_dev_environment-24.4.1/tests/unit/test_installer.py` & `ansible_dev_environment-24.4.2/tests/unit/test_installer.py`

 * *Files identical despite different names*

### Comparing `ansible_dev_environment-24.4.1/tests/unit/test_tree.py` & `ansible_dev_environment-24.4.2/tests/unit/test_tree.py`

 * *Files identical despite different names*

### Comparing `ansible_dev_environment-24.4.1/tests/unit/test_utils.py` & `ansible_dev_environment-24.4.2/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `ansible_dev_environment-24.4.1/tox.ini` & `ansible_dev_environment-24.4.2/tox.ini`

 * *Files identical despite different names*

