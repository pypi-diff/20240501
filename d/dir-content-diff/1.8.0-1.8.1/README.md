# Comparing `tmp/dir-content-diff-1.8.0.tar.gz` & `tmp/dir_content_diff-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dir-content-diff-1.8.0.tar", last modified: Mon Apr  8 10:27:51 2024, max compression
+gzip compressed data, was "dir_content_diff-1.8.1.tar", last modified: Wed May  1 07:43:37 2024, max compression
```

## Comparing `dir-content-diff-1.8.0.tar` & `dir_content_diff-1.8.1.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:27:51.801595 dir-content-diff-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/.auto-changelog
--rw-r--r--   0 runner    (1001) docker     (127)    11016 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/.auto-changelog-template.hbs
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/.codespellignorelines
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/.codespellrc
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/.copier-answers.yml
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/.coveragerc_py38
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:27:51.793594 dir-content-diff-1.8.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:27:51.793594 dir-content-diff-1.8.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/.github/ISSUE_TEMPLATE/bug_report.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/.github/ISSUE_TEMPLATE/feature_request.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/.github/ISSUE_TEMPLATE/how_to_use.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:27:51.793594 dir-content-diff-1.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/.github/workflows/commitlint.yml
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/.github/workflows/publish-sdist.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/.github/workflows/run-tox.yml
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/.gitreview
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     7672 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11354 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9494 2024-04-08 10:27:51.801595 dir-content-diff-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7468 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/commitlint.config.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:27:51.797595 dir-content-diff-1.8.0/dir_content_diff/
--rw-r--r--   0 runner    (1001) docker     (127)    14436 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/dir_content_diff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21897 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/dir_content_diff/base_comparators.py
--rw-r--r--   0 runner    (1001) docker     (127)     7375 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/dir_content_diff/pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/dir_content_diff/pytest_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/dir_content_diff/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:27:51.801595 dir-content-diff-1.8.0/dir_content_diff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9494 2024-04-08 10:27:51.000000 dir-content-diff-1.8.0/dir_content_diff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-08 10:27:51.000000 dir-content-diff-1.8.0/dir_content_diff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 10:27:51.000000 dir-content-diff-1.8.0/dir_content_diff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-08 10:27:51.000000 dir-content-diff-1.8.0/dir_content_diff.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-08 10:27:51.000000 dir-content-diff-1.8.0/dir_content_diff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-08 10:27:51.000000 dir-content-diff-1.8.0/dir_content_diff.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:27:51.797595 dir-content-diff-1.8.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:27:51.797595 dir-content-diff-1.8.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/docs/source/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/docs/source/api_ref.rst
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/docs/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/docs/source/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/package.json
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 10:27:51.801595 dir-content-diff-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:27:51.801595 dir-content-diff-1.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8397 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/tests/generate_test_files.py
--rw-r--r--   0 runner    (1001) docker     (127)    42632 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    18589 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/tests/test_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/tests/test_pytest_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-08 10:27:44.000000 dir-content-diff-1.8.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 07:43:37.164259 dir_content_diff-1.8.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-01 07:43:30.000000 dir_content_diff-1.8.1/.auto-changelog
+-rw-r--r--   0 runner    (1001) docker     (127)    11016 2024-05-01 07:43:30.000000 dir_content_diff-1.8.1/.auto-changelog-template.hbs
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 07:43:30.000000 dir_content_diff-1.8.1/.codespellignorelines
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-01 07:43:30.000000 dir_content_diff-1.8.1/.codespellrc
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-01 07:43:30.000000 dir_content_diff-1.8.1/.copier-answers.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-01 07:43:30.000000 dir_content_diff-1.8.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-01 07:43:30.000000 dir_content_diff-1.8.1/.coveragerc_py38
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-01 07:43:30.000000 dir_content_diff-1.8.1/.flake8
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-01 07:43:30.000000 dir_content_diff-1.8.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 07:43:37.156259 dir_content_diff-1.8.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 07:43:37.156259 dir_content_diff-1.8.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-05-01 07:43:30.000000 dir_content_diff-1.8.1/.github/ISSUE_TEMPLATE/bug_report.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-01 07:43:30.000000 dir_content_diff-1.8.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-01 07:43:30.000000 dir_content_diff-1.8.1/.github/ISSUE_TEMPLATE/feature_request.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-05-01 07:43:30.000000 dir_content_diff-1.8.1/.github/ISSUE_TEMPLATE/how_to_use.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-01 07:43:30.000000 dir_content_diff-1.8.1/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-01 07:43:30.000000 dir_content_diff-1.8.1/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 07:43:37.156259 dir_content_diff-1.8.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-01 07:43:30.000000 dir_content_diff-1.8.1/.github/workflows/commitlint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-01 07:43:30.000000 dir_content_diff-1.8.1/.github/workflows/publish-sdist.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-05-01 07:43:30.000000 dir_content_diff-1.8.1/.github/workflows/run-tox.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-01 07:43:30.000000 dir_content_diff-1.8.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-01 07:43:30.000000 dir_content_diff-1.8.1/.gitreview
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-01 07:43:30.000000 dir_content_diff-1.8.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-01 07:43:30.000000 dir_content_diff-1.8.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-01 07:43:30.000000 dir_content_diff-1.8.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-01 07:43:30.000000 dir_content_diff-1.8.1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7914 2024-05-01 07:43:30.000000 dir_content_diff-1.8.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-05-01 07:43:30.000000 dir_content_diff-1.8.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11354 2024-05-01 07:43:30.000000 dir_content_diff-1.8.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-01 07:43:30.000000 dir_content_diff-1.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9540 2024-05-01 07:43:37.164259 dir_content_diff-1.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7468 2024-05-01 07:43:30.000000 dir_content_diff-1.8.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-01 07:43:30.000000 dir_content_diff-1.8.1/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-05-01 07:43:30.000000 dir_content_diff-1.8.1/commitlint.config.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 07:43:37.156259 dir_content_diff-1.8.1/dir_content_diff/
+-rw-r--r--   0 runner    (1001) docker     (127)    14436 2024-05-01 07:43:30.000000 dir_content_diff-1.8.1/dir_content_diff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21897 2024-05-01 07:43:30.000000 dir_content_diff-1.8.1/dir_content_diff/base_comparators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7375 2024-05-01 07:43:30.000000 dir_content_diff-1.8.1/dir_content_diff/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-05-01 07:43:30.000000 dir_content_diff-1.8.1/dir_content_diff/pytest_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-05-01 07:43:30.000000 dir_content_diff-1.8.1/dir_content_diff/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 07:43:37.160259 dir_content_diff-1.8.1/dir_content_diff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9540 2024-05-01 07:43:37.000000 dir_content_diff-1.8.1/dir_content_diff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-01 07:43:37.000000 dir_content_diff-1.8.1/dir_content_diff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 07:43:37.000000 dir_content_diff-1.8.1/dir_content_diff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-01 07:43:37.000000 dir_content_diff-1.8.1/dir_content_diff.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-01 07:43:37.000000 dir_content_diff-1.8.1/dir_content_diff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-01 07:43:37.000000 dir_content_diff-1.8.1/dir_content_diff.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 07:43:37.156259 dir_content_diff-1.8.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-01 07:43:30.000000 dir_content_diff-1.8.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 07:43:37.160259 dir_content_diff-1.8.1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-01 07:43:30.000000 dir_content_diff-1.8.1/docs/source/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-01 07:43:30.000000 dir_content_diff-1.8.1/docs/source/api_ref.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-01 07:43:30.000000 dir_content_diff-1.8.1/docs/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-01 07:43:30.000000 dir_content_diff-1.8.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-01 07:43:30.000000 dir_content_diff-1.8.1/docs/source/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-01 07:43:30.000000 dir_content_diff-1.8.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-01 07:43:30.000000 dir_content_diff-1.8.1/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-01 07:43:30.000000 dir_content_diff-1.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 07:43:37.164259 dir_content_diff-1.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-01 07:43:30.000000 dir_content_diff-1.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 07:43:37.160259 dir_content_diff-1.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-01 07:43:30.000000 dir_content_diff-1.8.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8397 2024-05-01 07:43:30.000000 dir_content_diff-1.8.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-05-01 07:43:30.000000 dir_content_diff-1.8.1/tests/generate_test_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42632 2024-05-01 07:43:30.000000 dir_content_diff-1.8.1/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18589 2024-05-01 07:43:30.000000 dir_content_diff-1.8.1/tests/test_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-05-01 07:43:30.000000 dir_content_diff-1.8.1/tests/test_pytest_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-01 07:43:30.000000 dir_content_diff-1.8.1/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-05-01 07:43:30.000000 dir_content_diff-1.8.1/tox.ini
```

### Comparing `dir-content-diff-1.8.0/.auto-changelog` & `dir_content_diff-1.8.1/.auto-changelog`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.8.0/.auto-changelog-template.hbs` & `dir_content_diff-1.8.1/.auto-changelog-template.hbs`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.8.0/.copier-answers.yml` & `dir_content_diff-1.8.1/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.8.0/.github/ISSUE_TEMPLATE/bug_report.yaml` & `dir_content_diff-1.8.1/.github/ISSUE_TEMPLATE/bug_report.yaml`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.8.0/.github/ISSUE_TEMPLATE/feature_request.yaml` & `dir_content_diff-1.8.1/.github/ISSUE_TEMPLATE/feature_request.yaml`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.8.0/.github/ISSUE_TEMPLATE/how_to_use.yaml` & `dir_content_diff-1.8.1/.github/ISSUE_TEMPLATE/how_to_use.yaml`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.8.0/.github/dependabot.yml` & `dir_content_diff-1.8.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.8.0/.github/pull_request_template.md` & `dir_content_diff-1.8.1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.8.0/.github/workflows/commitlint.yml` & `dir_content_diff-1.8.1/.github/workflows/commitlint.yml`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.8.0/.github/workflows/publish-sdist.yml` & `dir_content_diff-1.8.1/.github/workflows/publish-sdist.yml`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.8.0/.github/workflows/run-tox.yml` & `dir_content_diff-1.8.1/.github/workflows/run-tox.yml`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.8.0/.pre-commit-config.yaml` & `dir_content_diff-1.8.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.8.0/.pylintrc` & `dir_content_diff-1.8.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.8.0/CHANGELOG.md` & `dir_content_diff-1.8.1/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # Changelog
 
+## [1.8.1](https://github.com/BlueBrain/dir-content-diff/compare/1.8.0..1.8.1)
+
+> 26 April 2024
+
+### Build
+
+- Freeze docutils version to be compatible with m2r2 (Adrien Berchet - [#58](https://github.com/BlueBrain/dir-content-diff/pull/58))
+
 ## [1.8.0](https://github.com/BlueBrain/dir-content-diff/compare/1.7.0..1.8.0)
 
 > 8 April 2024
 
 ### New Features
 
 - Add new comparators for Feather, Parquet and Stata files (Adrien Berchet - [#56](https://github.com/BlueBrain/dir-content-diff/pull/56))
```

### Comparing `dir-content-diff-1.8.0/CONTRIBUTING.md` & `dir_content_diff-1.8.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.8.0/LICENSE.txt` & `dir_content_diff-1.8.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.8.0/PKG-INFO` & `dir_content_diff-1.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dir-content-diff
-Version: 1.8.0
+Version: 1.8.1
 Summary: Simple tool to compare directory contents.
 Home-page: https://dir-content-diff.readthedocs.io
 Author: Blue Brain Project, EPFL
 License: Apache License 2.0
 Project-URL: Tracker, https://github.com/BlueBrain/dir-content-diff/issues
 Project-URL: Source, https://github.com/BlueBrain/dir-content-diff
 Classifier: Development Status :: 4 - Beta
@@ -27,14 +27,15 @@
 Requires-Dist: jsonpath-ng>=1.5
 Requires-Dist: PyYaml>=6
 Provides-Extra: pandas
 Requires-Dist: pandas>=1.4; extra == "pandas"
 Requires-Dist: pyarrow>=11; extra == "pandas"
 Requires-Dist: tables>=3.7; extra == "pandas"
 Provides-Extra: docs
+Requires-Dist: docutils<0.21; extra == "docs"
 Requires-Dist: m2r2; extra == "docs"
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-bluebrain-theme; extra == "docs"
 Requires-Dist: pandas>=1.4; extra == "docs"
 Requires-Dist: pyarrow>=11; extra == "docs"
 Requires-Dist: tables>=3.7; extra == "docs"
 Provides-Extra: test
```

### Comparing `dir-content-diff-1.8.0/README.md` & `dir_content_diff-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.8.0/commitlint.config.js` & `dir_content_diff-1.8.1/commitlint.config.js`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.8.0/dir_content_diff/__init__.py` & `dir_content_diff-1.8.1/dir_content_diff/__init__.py`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.8.0/dir_content_diff/base_comparators.py` & `dir_content_diff-1.8.1/dir_content_diff/base_comparators.py`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.8.0/dir_content_diff/pandas.py` & `dir_content_diff-1.8.1/dir_content_diff/pandas.py`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.8.0/dir_content_diff/pytest_plugin.py` & `dir_content_diff-1.8.1/dir_content_diff/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.8.0/dir_content_diff/util.py` & `dir_content_diff-1.8.1/dir_content_diff/util.py`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.8.0/dir_content_diff.egg-info/PKG-INFO` & `dir_content_diff-1.8.1/dir_content_diff.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dir-content-diff
-Version: 1.8.0
+Version: 1.8.1
 Summary: Simple tool to compare directory contents.
 Home-page: https://dir-content-diff.readthedocs.io
 Author: Blue Brain Project, EPFL
 License: Apache License 2.0
 Project-URL: Tracker, https://github.com/BlueBrain/dir-content-diff/issues
 Project-URL: Source, https://github.com/BlueBrain/dir-content-diff
 Classifier: Development Status :: 4 - Beta
@@ -27,14 +27,15 @@
 Requires-Dist: jsonpath-ng>=1.5
 Requires-Dist: PyYaml>=6
 Provides-Extra: pandas
 Requires-Dist: pandas>=1.4; extra == "pandas"
 Requires-Dist: pyarrow>=11; extra == "pandas"
 Requires-Dist: tables>=3.7; extra == "pandas"
 Provides-Extra: docs
+Requires-Dist: docutils<0.21; extra == "docs"
 Requires-Dist: m2r2; extra == "docs"
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-bluebrain-theme; extra == "docs"
 Requires-Dist: pandas>=1.4; extra == "docs"
 Requires-Dist: pyarrow>=11; extra == "docs"
 Requires-Dist: tables>=3.7; extra == "docs"
 Provides-Extra: test
```

### Comparing `dir-content-diff-1.8.0/dir_content_diff.egg-info/SOURCES.txt` & `dir_content_diff-1.8.1/dir_content_diff.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.8.0/docs/Makefile` & `dir_content_diff-1.8.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.8.0/docs/source/conf.py` & `dir_content_diff-1.8.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.8.0/package.json` & `dir_content_diff-1.8.1/package.json`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.8.0/pyproject.toml` & `dir_content_diff-1.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.8.0/setup.py` & `dir_content_diff-1.8.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     "dicttoxml>=1.7.12",
     "diff_pdf_visually>=1.7",
     "jsonpath-ng>=1.5",
     "PyYaml>=6",
 ]
 
 doc_reqs = [
+    "docutils<0.21",  # Temporary fix for m2r2
     "m2r2",
     "sphinx",
     "sphinx-bluebrain-theme",
 ]
 
 pandas_reqs = [
     "pandas>=1.4",
```

### Comparing `dir-content-diff-1.8.0/tests/conftest.py` & `dir_content_diff-1.8.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.8.0/tests/generate_test_files.py` & `dir_content_diff-1.8.1/tests/generate_test_files.py`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.8.0/tests/test_base.py` & `dir_content_diff-1.8.1/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.8.0/tests/test_pandas.py` & `dir_content_diff-1.8.1/tests/test_pandas.py`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.8.0/tests/test_pytest_plugin.py` & `dir_content_diff-1.8.1/tests/test_pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.8.0/tox.ini` & `dir_content_diff-1.8.1/tox.ini`

 * *Files identical despite different names*

