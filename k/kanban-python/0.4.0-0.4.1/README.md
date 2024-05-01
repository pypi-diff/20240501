# Comparing `tmp/kanban-python-0.4.0.tar.gz` & `tmp/kanban_python-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kanban-python-0.4.0.tar", last modified: Mon Jan 22 21:37:29 2024, max compression
+gzip compressed data, was "kanban_python-0.4.1.tar", last modified: Wed May  1 06:59:47 2024, max compression
```

## Comparing `kanban-python-0.4.0.tar` & `kanban_python-0.4.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 21:37:29.476559 kanban-python-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-01-22 21:37:02.000000 kanban-python-0.4.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 21:37:29.464559 kanban-python-0.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 21:37:29.468559 kanban-python-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     4523 2024-01-22 21:37:02.000000 kanban-python-0.4.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-01-22 21:37:02.000000 kanban-python-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-01-22 21:37:02.000000 kanban-python-0.4.0/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-01-22 21:37:02.000000 kanban-python-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-01-22 21:37:02.000000 kanban-python-0.4.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-01-22 21:37:02.000000 kanban-python-0.4.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-01-22 21:37:02.000000 kanban-python-0.4.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    13555 2024-01-22 21:37:02.000000 kanban-python-0.4.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-01-22 21:37:02.000000 kanban-python-0.4.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10488 2024-01-22 21:37:29.476559 kanban-python-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9623 2024-01-22 21:37:02.000000 kanban-python-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 21:37:29.468559 kanban-python-0.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-01-22 21:37:02.000000 kanban-python-0.4.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 21:37:29.468559 kanban-python-0.4.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-01-22 21:37:02.000000 kanban-python-0.4.0/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-01-22 21:37:02.000000 kanban-python-0.4.0/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-01-22 21:37:02.000000 kanban-python-0.4.0/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)    10042 2024-01-22 21:37:02.000000 kanban-python-0.4.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-01-22 21:37:02.000000 kanban-python-0.4.0/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-01-22 21:37:02.000000 kanban-python-0.4.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-01-22 21:37:02.000000 kanban-python-0.4.0/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-01-22 21:37:02.000000 kanban-python-0.4.0/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-01-22 21:37:02.000000 kanban-python-0.4.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 21:37:29.472559 kanban-python-0.4.0/images/
--rw-r--r--   0 runner    (1001) docker     (127)    32001 2024-01-22 21:37:02.000000 kanban-python-0.4.0/images/image_config.PNG
--rw-r--r--   0 runner    (1001) docker     (127)    69734 2024-01-22 21:37:02.000000 kanban-python-0.4.0/images/image_header.PNG
--rw-r--r--   0 runner    (1001) docker     (127)    70516 2024-01-22 21:37:02.000000 kanban-python-0.4.0/images/image_kanban.PNG
--rw-r--r--   0 runner    (1001) docker     (127)    15944 2024-01-22 21:37:02.000000 kanban-python-0.4.0/images/image_kanban_change.PNG
--rw-r--r--   0 runner    (1001) docker     (127)    74491 2024-01-22 21:37:02.000000 kanban-python-0.4.0/images/image_kanban_configure.PNG
--rw-r--r--   0 runner    (1001) docker     (127)    21483 2024-01-22 21:37:02.000000 kanban-python-0.4.0/images/image_kanban_init.PNG
--rw-r--r--   0 runner    (1001) docker     (127)    22831 2024-01-22 21:37:02.000000 kanban-python-0.4.0/images/image_kanban_report.PNG
--rw-r--r--   0 runner    (1001) docker     (127)    31262 2024-01-22 21:37:02.000000 kanban-python-0.4.0/images/image_kanban_report_document.PNG
--rw-r--r--   0 runner    (1001) docker     (127)    11146 2024-01-22 21:37:02.000000 kanban-python-0.4.0/images/image_scan_table.PNG
--rw-r--r--   0 runner    (1001) docker     (127)    19685 2024-01-22 21:37:02.000000 kanban-python-0.4.0/images/image_scan_view.PNG
--rw-r--r--   0 runner    (1001) docker     (127)    14884 2024-01-22 21:37:02.000000 kanban-python-0.4.0/images/image_task_example.PNG
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-01-22 21:37:02.000000 kanban-python-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-01-22 21:37:29.476559 kanban-python-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-01-22 21:37:02.000000 kanban-python-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 21:37:29.464559 kanban-python-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 21:37:29.472559 kanban-python-0.4.0/src/kanban_python/
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-01-22 21:37:02.000000 kanban-python-0.4.0/src/kanban_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-01-22 21:37:02.000000 kanban-python-0.4.0/src/kanban_python/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-01-22 21:37:02.000000 kanban-python-0.4.0/src/kanban_python/cli_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-01-22 21:37:02.000000 kanban-python-0.4.0/src/kanban_python/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-01-22 21:37:02.000000 kanban-python-0.4.0/src/kanban_python/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    10525 2024-01-22 21:37:02.000000 kanban-python-0.4.0/src/kanban_python/controls.py
--rw-r--r--   0 runner    (1001) docker     (127)    17357 2024-01-22 21:37:02.000000 kanban-python-0.4.0/src/kanban_python/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     8681 2024-01-22 21:37:02.000000 kanban-python-0.4.0/src/kanban_python/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 21:37:29.476559 kanban-python-0.4.0/src/kanban_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10488 2024-01-22 21:37:29.000000 kanban-python-0.4.0/src/kanban_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-01-22 21:37:29.000000 kanban-python-0.4.0/src/kanban_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-22 21:37:29.000000 kanban-python-0.4.0/src/kanban_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-01-22 21:37:29.000000 kanban-python-0.4.0/src/kanban_python.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-22 21:37:29.000000 kanban-python-0.4.0/src/kanban_python.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-01-22 21:37:29.000000 kanban-python-0.4.0/src/kanban_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-01-22 21:37:29.000000 kanban-python-0.4.0/src/kanban_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 21:37:29.476559 kanban-python-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-01-22 21:37:02.000000 kanban-python-0.4.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4060 2024-01-22 21:37:02.000000 kanban-python-0.4.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-01-22 21:37:02.000000 kanban-python-0.4.0/tests/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     7740 2024-01-22 21:37:02.000000 kanban-python-0.4.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-01-22 21:37:02.000000 kanban-python-0.4.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:59:47.481195 kanban_python-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-01 06:59:21.000000 kanban_python-0.4.1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:59:47.469195 kanban_python-0.4.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:59:47.473195 kanban_python-0.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     4523 2024-05-01 06:59:21.000000 kanban_python-0.4.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-01 06:59:21.000000 kanban_python-0.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-01 06:59:21.000000 kanban_python-0.4.1/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-01 06:59:21.000000 kanban_python-0.4.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-01 06:59:21.000000 kanban_python-0.4.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-01 06:59:21.000000 kanban_python-0.4.1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-05-01 06:59:21.000000 kanban_python-0.4.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13555 2024-05-01 06:59:21.000000 kanban_python-0.4.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-01 06:59:21.000000 kanban_python-0.4.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10488 2024-05-01 06:59:47.481195 kanban_python-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9623 2024-05-01 06:59:21.000000 kanban_python-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:59:47.473195 kanban_python-0.4.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-01 06:59:21.000000 kanban_python-0.4.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:59:47.477195 kanban_python-0.4.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-01 06:59:21.000000 kanban_python-0.4.1/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-01 06:59:21.000000 kanban_python-0.4.1/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-01 06:59:21.000000 kanban_python-0.4.1/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10042 2024-05-01 06:59:21.000000 kanban_python-0.4.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-01 06:59:21.000000 kanban_python-0.4.1/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-01 06:59:21.000000 kanban_python-0.4.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-01 06:59:21.000000 kanban_python-0.4.1/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-01 06:59:21.000000 kanban_python-0.4.1/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-01 06:59:21.000000 kanban_python-0.4.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:59:47.477195 kanban_python-0.4.1/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    32001 2024-05-01 06:59:21.000000 kanban_python-0.4.1/images/image_config.PNG
+-rw-r--r--   0 runner    (1001) docker     (127)    69734 2024-05-01 06:59:21.000000 kanban_python-0.4.1/images/image_header.PNG
+-rw-r--r--   0 runner    (1001) docker     (127)    70516 2024-05-01 06:59:21.000000 kanban_python-0.4.1/images/image_kanban.PNG
+-rw-r--r--   0 runner    (1001) docker     (127)    15944 2024-05-01 06:59:21.000000 kanban_python-0.4.1/images/image_kanban_change.PNG
+-rw-r--r--   0 runner    (1001) docker     (127)    74491 2024-05-01 06:59:21.000000 kanban_python-0.4.1/images/image_kanban_configure.PNG
+-rw-r--r--   0 runner    (1001) docker     (127)    21483 2024-05-01 06:59:21.000000 kanban_python-0.4.1/images/image_kanban_init.PNG
+-rw-r--r--   0 runner    (1001) docker     (127)    22831 2024-05-01 06:59:21.000000 kanban_python-0.4.1/images/image_kanban_report.PNG
+-rw-r--r--   0 runner    (1001) docker     (127)    31262 2024-05-01 06:59:21.000000 kanban_python-0.4.1/images/image_kanban_report_document.PNG
+-rw-r--r--   0 runner    (1001) docker     (127)    11146 2024-05-01 06:59:21.000000 kanban_python-0.4.1/images/image_scan_table.PNG
+-rw-r--r--   0 runner    (1001) docker     (127)    19685 2024-05-01 06:59:21.000000 kanban_python-0.4.1/images/image_scan_view.PNG
+-rw-r--r--   0 runner    (1001) docker     (127)    14884 2024-05-01 06:59:21.000000 kanban_python-0.4.1/images/image_task_example.PNG
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-01 06:59:21.000000 kanban_python-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-01 06:59:47.481195 kanban_python-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-01 06:59:21.000000 kanban_python-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:59:47.469195 kanban_python-0.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:59:47.481195 kanban_python-0.4.1/src/kanban_python/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-01 06:59:21.000000 kanban_python-0.4.1/src/kanban_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-05-01 06:59:21.000000 kanban_python-0.4.1/src/kanban_python/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-01 06:59:21.000000 kanban_python-0.4.1/src/kanban_python/cli_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-05-01 06:59:21.000000 kanban_python-0.4.1/src/kanban_python/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-01 06:59:21.000000 kanban_python-0.4.1/src/kanban_python/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10525 2024-05-01 06:59:21.000000 kanban_python-0.4.1/src/kanban_python/controls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17357 2024-05-01 06:59:21.000000 kanban_python-0.4.1/src/kanban_python/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8681 2024-05-01 06:59:21.000000 kanban_python-0.4.1/src/kanban_python/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:59:47.481195 kanban_python-0.4.1/src/kanban_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10488 2024-05-01 06:59:47.000000 kanban_python-0.4.1/src/kanban_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-01 06:59:47.000000 kanban_python-0.4.1/src/kanban_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 06:59:47.000000 kanban_python-0.4.1/src/kanban_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-01 06:59:47.000000 kanban_python-0.4.1/src/kanban_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 06:59:47.000000 kanban_python-0.4.1/src/kanban_python.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-01 06:59:47.000000 kanban_python-0.4.1/src/kanban_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-01 06:59:47.000000 kanban_python-0.4.1/src/kanban_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:59:47.481195 kanban_python-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-01 06:59:21.000000 kanban_python-0.4.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4060 2024-05-01 06:59:21.000000 kanban_python-0.4.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-01 06:59:21.000000 kanban_python-0.4.1/tests/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7740 2024-05-01 06:59:21.000000 kanban_python-0.4.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-05-01 06:59:21.000000 kanban_python-0.4.1/tox.ini
```

### Comparing `kanban-python-0.4.0/.coveragerc` & `kanban_python-0.4.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `kanban-python-0.4.0/.github/workflows/ci.yml` & `kanban_python-0.4.1/.github/workflows/ci.yml`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
           retention-days: 1
 
   test:
     needs: prepare
     strategy:
       matrix:
         python:
-        - "3.7"  # oldest Python supported by PSF
+        - "3.8"  # oldest Python supported by PSF
         - "3.11"  # newest Python that is stable
         platform:
         - ubuntu-latest
         - macos-latest
         - windows-latest
     runs-on: ${{ matrix.platform }}
     steps:
```

### Comparing `kanban-python-0.4.0/.gitignore` & `kanban_python-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `kanban-python-0.4.0/.pre-commit-config.yaml` & `kanban_python-0.4.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kanban-python-0.4.0/.readthedocs.yml` & `kanban_python-0.4.1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `kanban-python-0.4.0/CHANGELOG.md` & `kanban_python-0.4.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # Changelog
 
+## Version 0.4.1
+- Update minimum python version in ci test
+
+## Version 0.4.0
+- Update Docs with pipx link
+
 ## Version 0.3.10
 - Fix datetime for test for dict creation
 - Amount of completed task to tasks of current year in report
 
 ## Version 0.3.9
 - Add `from __future__ import annotations` to controls.py to not error on Union TypeHint if python version is <=3.9
```

### Comparing `kanban-python-0.4.0/CONTRIBUTING.md` & `kanban_python-0.4.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `kanban-python-0.4.0/LICENSE.txt` & `kanban_python-0.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kanban-python-0.4.0/PKG-INFO` & `kanban_python-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kanban-python
-Version: 0.4.0
+Version: 0.4.1
 Summary: Terminal Kanban App written in Python
 Home-page: https://github.com/Zaloog/kanban-python
 Author: Zaloog
 Author-email: gramslars@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/Zaloog/kanban-python
 Project-URL: Tracker, https://github.com/Zaloog/kanban-python/issues
```

### Comparing `kanban-python-0.4.0/README.md` & `kanban_python-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `kanban-python-0.4.0/docs/Makefile` & `kanban_python-0.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `kanban-python-0.4.0/docs/conf.py` & `kanban_python-0.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `kanban-python-0.4.0/docs/index.md` & `kanban_python-0.4.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `kanban-python-0.4.0/images/image_config.PNG` & `kanban_python-0.4.1/images/image_config.PNG`

 * *Files identical despite different names*

### Comparing `kanban-python-0.4.0/images/image_header.PNG` & `kanban_python-0.4.1/images/image_header.PNG`

 * *Files identical despite different names*

### Comparing `kanban-python-0.4.0/images/image_kanban.PNG` & `kanban_python-0.4.1/images/image_kanban.PNG`

 * *Files identical despite different names*

### Comparing `kanban-python-0.4.0/images/image_kanban_change.PNG` & `kanban_python-0.4.1/images/image_kanban_change.PNG`

 * *Files identical despite different names*

### Comparing `kanban-python-0.4.0/images/image_kanban_configure.PNG` & `kanban_python-0.4.1/images/image_kanban_configure.PNG`

 * *Files identical despite different names*

### Comparing `kanban-python-0.4.0/images/image_kanban_init.PNG` & `kanban_python-0.4.1/images/image_kanban_init.PNG`

 * *Files identical despite different names*

### Comparing `kanban-python-0.4.0/images/image_kanban_report.PNG` & `kanban_python-0.4.1/images/image_kanban_report.PNG`

 * *Files identical despite different names*

### Comparing `kanban-python-0.4.0/images/image_kanban_report_document.PNG` & `kanban_python-0.4.1/images/image_kanban_report_document.PNG`

 * *Files identical despite different names*

### Comparing `kanban-python-0.4.0/images/image_scan_table.PNG` & `kanban_python-0.4.1/images/image_scan_table.PNG`

 * *Files identical despite different names*

### Comparing `kanban-python-0.4.0/images/image_scan_view.PNG` & `kanban_python-0.4.1/images/image_scan_view.PNG`

 * *Files identical despite different names*

### Comparing `kanban-python-0.4.0/images/image_task_example.PNG` & `kanban_python-0.4.1/images/image_task_example.PNG`

 * *Files identical despite different names*

### Comparing `kanban-python-0.4.0/setup.cfg` & `kanban_python-0.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `kanban-python-0.4.0/setup.py` & `kanban_python-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `kanban-python-0.4.0/src/kanban_python/__init__.py` & `kanban_python-0.4.1/src/kanban_python/__init__.py`

 * *Files identical despite different names*

### Comparing `kanban-python-0.4.0/src/kanban_python/app.py` & `kanban_python-0.4.1/src/kanban_python/app.py`

 * *Files identical despite different names*

### Comparing `kanban-python-0.4.0/src/kanban_python/cli_parser.py` & `kanban_python-0.4.1/src/kanban_python/cli_parser.py`

 * *Files identical despite different names*

### Comparing `kanban-python-0.4.0/src/kanban_python/config.py` & `kanban_python-0.4.1/src/kanban_python/config.py`

 * *Files identical despite different names*

### Comparing `kanban-python-0.4.0/src/kanban_python/constants.py` & `kanban_python-0.4.1/src/kanban_python/constants.py`

 * *Files identical despite different names*

### Comparing `kanban-python-0.4.0/src/kanban_python/controls.py` & `kanban_python-0.4.1/src/kanban_python/controls.py`

 * *Files identical despite different names*

### Comparing `kanban-python-0.4.0/src/kanban_python/interface.py` & `kanban_python-0.4.1/src/kanban_python/interface.py`

 * *Files identical despite different names*

### Comparing `kanban-python-0.4.0/src/kanban_python/utils.py` & `kanban_python-0.4.1/src/kanban_python/utils.py`

 * *Files identical despite different names*

### Comparing `kanban-python-0.4.0/src/kanban_python.egg-info/PKG-INFO` & `kanban_python-0.4.1/src/kanban_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kanban-python
-Version: 0.4.0
+Version: 0.4.1
 Summary: Terminal Kanban App written in Python
 Home-page: https://github.com/Zaloog/kanban-python
 Author: Zaloog
 Author-email: gramslars@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/Zaloog/kanban-python
 Project-URL: Tracker, https://github.com/Zaloog/kanban-python/issues
```

### Comparing `kanban-python-0.4.0/src/kanban_python.egg-info/SOURCES.txt` & `kanban_python-0.4.1/src/kanban_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kanban-python-0.4.0/tests/conftest.py` & `kanban_python-0.4.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `kanban-python-0.4.0/tests/test_config.py` & `kanban_python-0.4.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `kanban-python-0.4.0/tests/test_interface.py` & `kanban_python-0.4.1/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `kanban-python-0.4.0/tests/test_utils.py` & `kanban_python-0.4.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `kanban-python-0.4.0/tox.ini` & `kanban_python-0.4.1/tox.ini`

 * *Files identical despite different names*

