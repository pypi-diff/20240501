# Comparing `tmp/holospy-0.2.tar.gz` & `tmp/holospy-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "holospy-0.2.tar", last modified: Thu Apr  4 16:03:10 2024, max compression
+gzip compressed data, was "holospy-0.3.tar", last modified: Wed May  1 17:28:53 2024, max compression
```

## Comparing `holospy-0.2.tar` & `holospy-0.3.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:03:09.995966 holospy-0.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:03:09.983966 holospy-0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:03:09.983966 holospy-0.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-04 16:02:58.000000 holospy-0.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-04 16:02:58.000000 holospy-0.2/.github/ISSUE_TEMPLATE/custom.md
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-04 16:02:58.000000 holospy-0.2/.github/ISSUE_TEMPLATE/feature_request.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     1238 2024-04-04 16:02:58.000000 holospy-0.2/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-04 16:02:58.000000 holospy-0.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:03:09.983966 holospy-0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-04 16:02:58.000000 holospy-0.2/.github/workflows/doc.yml
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-04 16:02:58.000000 holospy-0.2/.github/workflows/package_and_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-04 16:02:58.000000 holospy-0.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-04 16:02:58.000000 holospy-0.2/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-04 16:02:58.000000 holospy-0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-04 16:02:58.000000 holospy-0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-04 16:02:58.000000 holospy-0.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-04-04 16:02:58.000000 holospy-0.2/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-04-04 16:02:58.000000 holospy-0.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    35155 2024-04-04 16:02:58.000000 holospy-0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    43725 2024-04-04 16:03:09.995966 holospy-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-04 16:02:58.000000 holospy-0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:03:09.987966 holospy-0.2/doc/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-04 16:02:58.000000 holospy-0.2/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:03:09.987966 holospy-0.2/doc/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    21844 2024-04-04 16:02:58.000000 holospy-0.2/doc/_static/holospy-banner-dark.svg
--rw-r--r--   0 runner    (1001) docker     (127)    21771 2024-04-04 16:02:58.000000 holospy-0.2/doc/_static/holospy-banner-light.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-04-04 16:02:58.000000 holospy-0.2/doc/_static/holospy-icon.svg
--rw-r--r--   0 runner    (1001) docker     (127)   103104 2024-04-04 16:02:58.000000 holospy-0.2/doc/_static/holospy.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:03:09.987966 holospy-0.2/doc/api/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-04 16:02:58.000000 holospy-0.2/doc/api/data.rst
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-04 16:02:58.000000 holospy-0.2/doc/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-04 16:02:58.000000 holospy-0.2/doc/api/reconstruct.rst
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-04 16:02:58.000000 holospy-0.2/doc/api/signals.rst
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-04 16:02:58.000000 holospy-0.2/doc/api/tools.rst
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-04 16:02:58.000000 holospy-0.2/doc/changes.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-04-04 16:02:58.000000 holospy-0.2/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-04 16:02:58.000000 holospy-0.2/doc/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-04 16:02:58.000000 holospy-0.2/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-04-04 16:02:58.000000 holospy-0.2/doc/intro.rst
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-04 16:02:58.000000 holospy-0.2/doc/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:03:09.987966 holospy-0.2/doc/user_guide/
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-04 16:02:58.000000 holospy-0.2/doc/user_guide/bibliography.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8639 2024-04-04 16:02:58.000000 holospy-0.2/doc/user_guide/electron_holography.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:03:09.987966 holospy-0.2/doc/user_guide/images/
--rw-r--r--   0 runner    (1001) docker     (127)    61567 2024-04-04 16:02:58.000000 holospy-0.2/doc/user_guide/images/holography_argand_diagram.png
--rw-r--r--   0 runner    (1001) docker     (127)   128508 2024-04-04 16:02:58.000000 holospy-0.2/doc/user_guide/images/holography_unwrapped_phase.png
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-04 16:02:58.000000 holospy-0.2/doc/user_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-04-04 16:02:58.000000 holospy-0.2/doc/user_guide/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-04-04 16:02:58.000000 holospy-0.2/doc/user_guide/metadata_structure.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:03:09.987966 holospy-0.2/holospy/
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-04 16:02:58.000000 holospy-0.2/holospy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-04 16:02:58.000000 holospy-0.2/holospy/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:03:09.995966 holospy-0.2/holospy/data/
--rw-r--r--   0 runner    (1001) docker     (127)  1358560 2024-04-04 16:02:58.000000 holospy-0.2/holospy/data/00_ref_Vbp_130V_0V_bin2_crop.hdf5
--rw-r--r--   0 runner    (1001) docker     (127)  1353256 2024-04-04 16:02:58.000000 holospy-0.2/holospy/data/01_holo_Vbp_130V_0V_bin2_crop.hdf5
--rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-04-04 16:02:58.000000 holospy-0.2/holospy/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-04 16:02:58.000000 holospy-0.2/holospy/hyperspy_extension.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     7643 2024-04-04 16:02:58.000000 holospy-0.2/holospy/reconstruct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:03:09.995966 holospy-0.2/holospy/signals/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-04 16:02:58.000000 holospy-0.2/holospy/signals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34208 2024-04-04 16:02:58.000000 holospy-0.2/holospy/signals/hologram_image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:03:09.995966 holospy-0.2/holospy/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 16:02:58.000000 holospy-0.2/holospy/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:03:09.995966 holospy-0.2/holospy/tests/signals/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 16:02:58.000000 holospy-0.2/holospy/tests/signals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12594 2024-04-04 16:02:58.000000 holospy-0.2/holospy/tests/signals/test_hologram_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     5888 2024-04-04 16:02:58.000000 holospy-0.2/holospy/tests/signals/test_hologram_image_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-04 16:02:58.000000 holospy-0.2/holospy/tests/test_non-uniform_not-implemented.py
--rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-04-04 16:02:58.000000 holospy-0.2/holospy/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:03:09.995966 holospy-0.2/holospy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    43725 2024-04-04 16:03:09.000000 holospy-0.2/holospy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-04 16:03:09.000000 holospy-0.2/holospy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 16:03:09.000000 holospy-0.2/holospy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-04 16:03:09.000000 holospy-0.2/holospy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-04 16:03:09.000000 holospy-0.2/holospy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-04 16:03:09.000000 holospy-0.2/holospy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-04 16:02:58.000000 holospy-0.2/prepare_release.py
--rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-04-04 16:02:58.000000 holospy-0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-04 16:02:58.000000 holospy-0.2/releasing_guide.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 16:03:09.995966 holospy-0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:03:09.995966 holospy-0.2/upcoming_changes/
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-04 16:02:58.000000 holospy-0.2/upcoming_changes/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:28:53.482468 holospy-0.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:28:53.470468 holospy-0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:28:53.470468 holospy-0.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-01 17:28:41.000000 holospy-0.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-01 17:28:41.000000 holospy-0.3/.github/ISSUE_TEMPLATE/custom.md
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-01 17:28:41.000000 holospy-0.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1238 2024-05-01 17:28:41.000000 holospy-0.3/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-01 17:28:41.000000 holospy-0.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:28:53.470468 holospy-0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-01 17:28:41.000000 holospy-0.3/.github/workflows/doc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-01 17:28:41.000000 holospy-0.3/.github/workflows/package_and_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-01 17:28:41.000000 holospy-0.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-01 17:28:41.000000 holospy-0.3/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-01 17:28:41.000000 holospy-0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-01 17:28:41.000000 holospy-0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-01 17:28:41.000000 holospy-0.3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-05-01 17:28:41.000000 holospy-0.3/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-05-01 17:28:41.000000 holospy-0.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35155 2024-05-01 17:28:41.000000 holospy-0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    44475 2024-05-01 17:28:53.482468 holospy-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-05-01 17:28:41.000000 holospy-0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:28:53.470468 holospy-0.3/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-01 17:28:41.000000 holospy-0.3/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:28:53.470468 holospy-0.3/doc/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    21844 2024-05-01 17:28:41.000000 holospy-0.3/doc/_static/holospy-banner-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    21771 2024-05-01 17:28:41.000000 holospy-0.3/doc/_static/holospy-banner-light.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-05-01 17:28:41.000000 holospy-0.3/doc/_static/holospy-icon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   103104 2024-05-01 17:28:41.000000 holospy-0.3/doc/_static/holospy.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:28:53.474469 holospy-0.3/doc/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-01 17:28:41.000000 holospy-0.3/doc/api/data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-01 17:28:41.000000 holospy-0.3/doc/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-01 17:28:41.000000 holospy-0.3/doc/api/reconstruct.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-01 17:28:41.000000 holospy-0.3/doc/api/signals.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-01 17:28:41.000000 holospy-0.3/doc/api/tools.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-01 17:28:41.000000 holospy-0.3/doc/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4122 2024-05-01 17:28:41.000000 holospy-0.3/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-01 17:28:41.000000 holospy-0.3/doc/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-01 17:28:41.000000 holospy-0.3/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-05-01 17:28:41.000000 holospy-0.3/doc/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-01 17:28:41.000000 holospy-0.3/doc/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:28:53.474469 holospy-0.3/doc/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-01 17:28:41.000000 holospy-0.3/doc/user_guide/bibliography.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8639 2024-05-01 17:28:41.000000 holospy-0.3/doc/user_guide/electron_holography.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:28:53.474469 holospy-0.3/doc/user_guide/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    61567 2024-05-01 17:28:41.000000 holospy-0.3/doc/user_guide/images/holography_argand_diagram.png
+-rw-r--r--   0 runner    (1001) docker     (127)   128508 2024-05-01 17:28:41.000000 holospy-0.3/doc/user_guide/images/holography_unwrapped_phase.png
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-01 17:28:41.000000 holospy-0.3/doc/user_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-05-01 17:28:41.000000 holospy-0.3/doc/user_guide/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-01 17:28:41.000000 holospy-0.3/doc/user_guide/metadata_structure.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:28:53.474469 holospy-0.3/holospy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-05-01 17:28:41.000000 holospy-0.3/holospy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-01 17:28:41.000000 holospy-0.3/holospy/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:28:53.478469 holospy-0.3/holospy/data/
+-rw-r--r--   0 runner    (1001) docker     (127)  1358560 2024-05-01 17:28:41.000000 holospy-0.3/holospy/data/00_ref_Vbp_130V_0V_bin2_crop.hdf5
+-rw-r--r--   0 runner    (1001) docker     (127)  1353256 2024-05-01 17:28:41.000000 holospy-0.3/holospy/data/01_holo_Vbp_130V_0V_bin2_crop.hdf5
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-05-01 17:28:41.000000 holospy-0.3/holospy/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-01 17:28:41.000000 holospy-0.3/holospy/hyperspy_extension.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     7644 2024-05-01 17:28:41.000000 holospy-0.3/holospy/reconstruct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:28:53.478469 holospy-0.3/holospy/signals/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-01 17:28:41.000000 holospy-0.3/holospy/signals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34721 2024-05-01 17:28:41.000000 holospy-0.3/holospy/signals/hologram_image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:28:53.482468 holospy-0.3/holospy/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 17:28:41.000000 holospy-0.3/holospy/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:28:53.482468 holospy-0.3/holospy/tests/signals/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 17:28:41.000000 holospy-0.3/holospy/tests/signals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12961 2024-05-01 17:28:41.000000 holospy-0.3/holospy/tests/signals/test_hologram_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5886 2024-05-01 17:28:41.000000 holospy-0.3/holospy/tests/signals/test_hologram_image_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-01 17:28:41.000000 holospy-0.3/holospy/tests/test_non-uniform_not-implemented.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-05-01 17:28:41.000000 holospy-0.3/holospy/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:28:53.482468 holospy-0.3/holospy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    44475 2024-05-01 17:28:53.000000 holospy-0.3/holospy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-01 17:28:53.000000 holospy-0.3/holospy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 17:28:53.000000 holospy-0.3/holospy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-01 17:28:53.000000 holospy-0.3/holospy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-01 17:28:53.000000 holospy-0.3/holospy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-01 17:28:53.000000 holospy-0.3/holospy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-01 17:28:41.000000 holospy-0.3/prepare_release.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-05-01 17:28:41.000000 holospy-0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-01 17:28:41.000000 holospy-0.3/releasing_guide.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 17:28:53.482468 holospy-0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:28:53.482468 holospy-0.3/upcoming_changes/
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-01 17:28:41.000000 holospy-0.3/upcoming_changes/README.rst
```

### Comparing `holospy-0.2/.github/ISSUE_TEMPLATE/bug_report.md` & `holospy-0.3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `holospy-0.2/.github/PULL_REQUEST_TEMPLATE.md` & `holospy-0.3/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `holospy-0.2/.github/dependabot.yml` & `holospy-0.3/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `holospy-0.2/.github/workflows/doc.yml` & `holospy-0.3/.github/workflows/doc.yml`

 * *Files identical despite different names*

### Comparing `holospy-0.2/.github/workflows/release.yml` & `holospy-0.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `holospy-0.2/.github/workflows/tests.yml` & `holospy-0.3/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `holospy-0.2/.readthedocs.yaml` & `holospy-0.3/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `holospy-0.2/CHANGES.rst` & `holospy-0.3/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,30 @@
 Changelog entries for the development version are available at
 https://holospy.readthedocs.io/en/latest/changes.html
 
 .. towncrier-draft-entries:: |release| [UNRELEASED]
 
 .. towncrier release notes start
 
+0.3 (2024-05-02)
+================
+
+Improved Documentation
+----------------------
+
+- Fix DOI and add more badges to readme file. (`#34 <https://github.com/hyperspy/holospy/issues/34>`_)
+
+
+Maintenance
+-----------
+
+- Use ``pint.get_application_registry`` instead of HyperSpy private API to get the handle of the ``pint.UnitRegistry``. (`#35 <https://github.com/hyperspy/holospy/issues/35>`_)
+- Add/enable more ruff rules: isort, pyflakes, pycodestyle. (`#37 <https://github.com/hyperspy/holospy/issues/37>`_)
+
+
 0.2 (2024-04-04)
 ================
 
 Deprecations
 ------------
 
 - The positional arguments ``holo_data`` and ``holo_sampling`` of :func:`~.reconstruct.reconstruct` have been renamed to ``data`` and ``sampling``, respectively. (`#26 <https://github.com/hyperspy/holospy/issues/26>`_)
```

### Comparing `holospy-0.2/CONTRIBUTING.rst` & `holospy-0.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `holospy-0.2/LICENSE` & `holospy-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `holospy-0.2/PKG-INFO` & `holospy-0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: holospy
-Version: 0.2
+Version: 0.3
 Summary: Analysis of (off-axis) electron holography data with HyperSpy.
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -695,14 +695,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: hyperspy>=2.0rc0
 Requires-Dist: numpy>=1.20.0
+Requires-Dist: pint>=0.10
 Requires-Dist: scipy>=1.5.0
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-cov; extra == "tests"
 Requires-Dist: setuptools-scm; extra == "tests"
 Provides-Extra: doc
 Requires-Dist: numpydoc; extra == "doc"
@@ -714,19 +715,25 @@
 Requires-Dist: towncrier; extra == "doc"
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: holospy[doc]; extra == "dev"
 Requires-Dist: holospy[tests]; extra == "dev"
 
 
+[![Docs](https://readthedocs.org/projects/holospy/badge/?version=latest)](https://holospy.readthedocs.io/en/latest/?badge=latest)
 [![Tests](https://github.com/hyperspy/holospy/actions/workflows/tests.yml/badge.svg)](https://github.com/hyperspy/holospy/actions/workflows/tests.yml)
 [![codecov](https://codecov.io/gh/hyperspy/holospy/graph/badge.svg?token=XB1QDTXQ86)](https://codecov.io/gh/hyperspy/holospy)
-[![Docs](https://readthedocs.org/projects/holospy/badge/?version=latest)](https://holospy.readthedocs.io/en/latest/?badge=latest)
+[![CodeQL](https://github.com/hyperspy/holospy/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/hyperspy/holospy/actions/workflows/github-code-scanning/codeql)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/hyperspy/holospy/main.svg)](https://results.pre-commit.ci/latest/github/hyperspy/holospy/main)
+
+[![Python Version](https://img.shields.io/pypi/pyversions/holospy.svg?style=flat)](https://pypi.python.org/pypi/holospy)
+[![PyPi Version](http://img.shields.io/pypi/v/holospy.svg?style=flat)](https://pypi.python.org/pypi/holospy)
+[![Anaconda Version](https://anaconda.org/conda-forge/holospy/badges/version.svg)](https://anaconda.org/conda-forge/holospy)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
-[![DOI](https://zenodo.org/badge/2233998.svg)](https://zenodo.org/badge/latestdoi/2233998)
+[![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.10137993.svg)](https://doi.org/10.5281/zenodo.10137993)
 
 **HoloSpy** is a Python package extending the functionality for multi-dimensional
 data analysis provided by the [HyperSpy](https://hyperspy.org) library. It is
 aimed at helping with the analysis of (off-axis) electron holography data.
 
 Go to the documentation for instructions on how to install HoloSpy and start an
 analysis: [Read the docs](https://holospy.readthedocs.io).
```

### Comparing `holospy-0.2/README.md` & `holospy-0.3/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 
+[![Docs](https://readthedocs.org/projects/holospy/badge/?version=latest)](https://holospy.readthedocs.io/en/latest/?badge=latest)
 [![Tests](https://github.com/hyperspy/holospy/actions/workflows/tests.yml/badge.svg)](https://github.com/hyperspy/holospy/actions/workflows/tests.yml)
 [![codecov](https://codecov.io/gh/hyperspy/holospy/graph/badge.svg?token=XB1QDTXQ86)](https://codecov.io/gh/hyperspy/holospy)
-[![Docs](https://readthedocs.org/projects/holospy/badge/?version=latest)](https://holospy.readthedocs.io/en/latest/?badge=latest)
+[![CodeQL](https://github.com/hyperspy/holospy/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/hyperspy/holospy/actions/workflows/github-code-scanning/codeql)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/hyperspy/holospy/main.svg)](https://results.pre-commit.ci/latest/github/hyperspy/holospy/main)
+
+[![Python Version](https://img.shields.io/pypi/pyversions/holospy.svg?style=flat)](https://pypi.python.org/pypi/holospy)
+[![PyPi Version](http://img.shields.io/pypi/v/holospy.svg?style=flat)](https://pypi.python.org/pypi/holospy)
+[![Anaconda Version](https://anaconda.org/conda-forge/holospy/badges/version.svg)](https://anaconda.org/conda-forge/holospy)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
-[![DOI](https://zenodo.org/badge/2233998.svg)](https://zenodo.org/badge/latestdoi/2233998)
+[![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.10137993.svg)](https://doi.org/10.5281/zenodo.10137993)
 
 **HoloSpy** is a Python package extending the functionality for multi-dimensional
 data analysis provided by the [HyperSpy](https://hyperspy.org) library. It is
 aimed at helping with the analysis of (off-axis) electron holography data.
 
 Go to the documentation for instructions on how to install HoloSpy and start an
 analysis: [Read the docs](https://holospy.readthedocs.io).
```

### Comparing `holospy-0.2/doc/Makefile` & `holospy-0.3/doc/Makefile`

 * *Files identical despite different names*

### Comparing `holospy-0.2/doc/_static/holospy-banner-dark.svg` & `holospy-0.3/doc/_static/holospy-banner-dark.svg`

 * *Files identical despite different names*

### Comparing `holospy-0.2/doc/_static/holospy-banner-light.svg` & `holospy-0.3/doc/_static/holospy-banner-light.svg`

 * *Files identical despite different names*

### Comparing `holospy-0.2/doc/_static/holospy-icon.svg` & `holospy-0.3/doc/_static/holospy-icon.svg`

 * *Files identical despite different names*

### Comparing `holospy-0.2/doc/_static/holospy.ico` & `holospy-0.3/doc/_static/holospy.ico`

 * *Files identical despite different names*

### Comparing `holospy-0.2/doc/conf.py` & `holospy-0.3/doc/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 #
 # import os
 # import sys
 # sys.path.insert(0, os.path.abspath('.'))
 
 import hyperspy.api as hs
 
-
 # Set logging level to `ERROR` to avoid exspy warning in documentation
 hs.set_log_level("ERROR")
 
 
 # -- Project information -----------------------------------------------------
 
 project = "HoloSpy"
```

### Comparing `holospy-0.2/doc/intro.rst` & `holospy-0.3/doc/intro.rst`

 * *Files identical despite different names*

### Comparing `holospy-0.2/doc/make.bat` & `holospy-0.3/doc/make.bat`

 * *Files identical despite different names*

### Comparing `holospy-0.2/doc/user_guide/bibliography.rst` & `holospy-0.3/doc/user_guide/bibliography.rst`

 * *Files identical despite different names*

### Comparing `holospy-0.2/doc/user_guide/electron_holography.rst` & `holospy-0.3/doc/user_guide/electron_holography.rst`

 * *Files identical despite different names*

### Comparing `holospy-0.2/doc/user_guide/images/holography_argand_diagram.png` & `holospy-0.3/doc/user_guide/images/holography_argand_diagram.png`

 * *Files identical despite different names*

### Comparing `holospy-0.2/doc/user_guide/images/holography_unwrapped_phase.png` & `holospy-0.3/doc/user_guide/images/holography_unwrapped_phase.png`

 * *Files identical despite different names*

### Comparing `holospy-0.2/doc/user_guide/installation.rst` & `holospy-0.3/doc/user_guide/installation.rst`

 * *Files identical despite different names*

### Comparing `holospy-0.2/doc/user_guide/metadata_structure.rst` & `holospy-0.3/doc/user_guide/metadata_structure.rst`

 * *Files identical despite different names*

### Comparing `holospy-0.2/holospy/__init__.py` & `holospy-0.3/holospy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,16 +15,15 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with HyperSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
 
 from importlib.metadata import version
 from pathlib import Path
 
-from . import data, signals, reconstruct, tools
-
+from . import data, reconstruct, signals, tools
 
 __version__ = version("holospy")
 
 # For development version, `setuptools_scm` will be used at build time
 # to get the dev version, in case of missing vcs information (git archive,
 # shallow repository), the fallback version defined in pyproject.toml will
 # be used
```

### Comparing `holospy-0.2/holospy/conftest.py` & `holospy-0.3/holospy/conftest.py`

 * *Files identical despite different names*

### Comparing `holospy-0.2/holospy/data/00_ref_Vbp_130V_0V_bin2_crop.hdf5` & `holospy-0.3/holospy/data/00_ref_Vbp_130V_0V_bin2_crop.hdf5`

 * *Files identical despite different names*

### Comparing `holospy-0.2/holospy/data/01_holo_Vbp_130V_0V_bin2_crop.hdf5` & `holospy-0.3/holospy/data/01_holo_Vbp_130V_0V_bin2_crop.hdf5`

 * *Files identical despite different names*

### Comparing `holospy-0.2/holospy/data/__init__.py` & `holospy-0.3/holospy/data/__init__.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with HyperSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
 
-from pathlib import Path
 import warnings
+from pathlib import Path
 
 import hyperspy.api as hs
 
 __all__ = [
     "Fe_needle_hologram",
     "Fe_needle_reference_hologram",
 ]
```

### Comparing `holospy-0.2/holospy/reconstruct.py` & `holospy-0.3/holospy/reconstruct.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,19 +12,20 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with HyperSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
 
-import numpy as np
-from scipy.fftpack import fft2, ifft2, fftshift
-import matplotlib.pyplot as plt
 import logging
 
+import matplotlib.pyplot as plt
+import numpy as np
+from scipy.fftpack import fft2, fftshift, ifft2
+
 _logger = logging.getLogger(__name__)
 
 
 def estimate_sideband_position(
     data, sampling, central_band_mask_radius=None, sb="lower", high_cf=True
 ):
     """
```

### Comparing `holospy-0.2/holospy/signals/__init__.py` & `holospy-0.3/holospy/signals/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 LazyHologramImage
     For holography data processed lazily
 
 """
 
 from .hologram_image import HologramImage, LazyHologramImage
 
-
 __all__ = [
     "HologramImage",
     "LazyHologramImage",
 ]
 
 
 def __dir__():
```

### Comparing `holospy-0.2/holospy/signals/hologram_image.py` & `holospy-0.3/holospy/signals/hologram_image.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,40 +12,53 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with HyperSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
 
+import importlib
 import logging
 from collections import OrderedDict
-import scipy.constants as constants
+
+import hyperspy.api as hs
 import numpy as np
+import scipy.constants as constants
 from dask.array import Array as daArray
+from hyperspy._signals.lazy import LazySignal
+from hyperspy.docstrings.signal import (
+    LAZYSIGNAL_DOC,
+    NUM_WORKERS_ARG,
+    SHOW_PROGRESSBAR_ARG,
+)
 from pint import UndefinedUnitError
 
-from hyperspy.api_nogui import _ureg
-from hyperspy._signals.signal2d import Signal2D
-from hyperspy.signal import BaseSignal
-from hyperspy._signals.signal1d import Signal1D
-from hyperspy._signals.lazy import LazySignal
 from holospy.reconstruct import (
-    reconstruct,
     estimate_sideband_position,
     estimate_sideband_size,
+    reconstruct,
 )
 from holospy.tools import (
     calculate_carrier_frequency,
     estimate_fringe_contrast_fourier,
 )
-from hyperspy.docstrings.signal import (
-    SHOW_PROGRESSBAR_ARG,
-    NUM_WORKERS_ARG,
-    LAZYSIGNAL_DOC,
-)
+
+if importlib.util.find_spec("hyperspy.api_nogui") is None:
+    # Considering the usage of the UnitRegistry in holospy,
+    # sharing the same UnitRegistry in holospy is not necessary
+    # because there is no operations between quantities defined in
+    # hyperspy and holospy but this is good practise and
+    # can be used as a reference
+    import pint
+
+    _ureg = pint.get_application_registry()
+
+else:
+    # Before hyperspy migrate to use pint default global UnitRegistry
+    from hyperspy.api_nogui import _ureg
 
 _logger = logging.getLogger(__name__)
 
 
 def _first_nav_pixel_data(s):
     return s._data_aligned_with_axes[(0,) * s.axes_manager.navigation_dimension]
 
@@ -66,21 +79,21 @@
         else:
             sb_position = reference.estimate_sideband_position(
                 sb=sb, high_cf=high_cf, num_workers=num_workers
             )
 
     else:
         if (
-            isinstance(sb_position, BaseSignal)
+            isinstance(sb_position, hs.signals.BaseSignal)
             and not sb_position._signal_dimension == 1
         ):
             raise ValueError("sb_position dimension has to be 1.")
 
-        if not isinstance(sb_position, Signal1D):
-            sb_position = Signal1D(sb_position)
+        if not isinstance(sb_position, hs.signals.Signal1D):
+            sb_position = hs.signals.Signal1D(sb_position)
             if isinstance(sb_position.data, daArray):
                 sb_position = sb_position.as_lazy()
 
         if not sb_position.axes_manager.signal_size == 2:
             raise ValueError("sb_position should to have signal size of 2.")
 
     if sb_position.axes_manager.navigation_size != s.axes_manager.navigation_size:
@@ -103,20 +116,20 @@
         if reference is None:
             sb_size = s.estimate_sideband_size(sb_position, num_workers=num_workers)
         else:
             sb_size = reference.estimate_sideband_size(
                 sb_position, num_workers=num_workers
             )
     else:
-        if not isinstance(sb_size, BaseSignal):
+        if not isinstance(sb_size, hs.signals.BaseSignal):
             if isinstance(sb_size, (np.ndarray, daArray)) and sb_size.size > 1:
                 # transpose if np.array of multiple instances
-                sb_size = BaseSignal(sb_size).T
+                sb_size = hs.signals.BaseSignal(sb_size).T
             else:
-                sb_size = BaseSignal(sb_size)
+                sb_size = hs.signals.BaseSignal(sb_size)
             if isinstance(sb_size.data, daArray):
                 sb_size = sb_size.as_lazy()
     if sb_size.axes_manager.navigation_size != s.axes_manager.navigation_size:
         if sb_size.axes_manager.navigation_size:
             raise ValueError(
                 "Sideband size dimensions do not match "
                 "neither reference nor hologram dimensions."
@@ -146,15 +159,15 @@
     """
 
     axes = signal.axes_manager.signal_axes
 
     return signal.std(axes) / signal.mean(axes)
 
 
-class HologramImage(Signal2D):
+class HologramImage(hs.signals.Signal2D):
     """Signal class for holograms acquired via off-axis electron holography."""
 
     _signal_type = "hologram"
 
     def set_microscope_parameters(
         self, beam_energy=None, biprism_voltage=None, tilt_stage=None
     ):
@@ -408,15 +421,15 @@
             if not axis.is_uniform:
                 raise NotImplementedError(
                     "This operation is not yet implemented for non-uniform energy axes."
                 )
 
         # Parsing reference:
         if not isinstance(reference, HologramImage):
-            if isinstance(reference, Signal2D):
+            if isinstance(reference, hs.signals.Signal2D):
                 if (
                     not reference.axes_manager.navigation_shape
                     == self.axes_manager.navigation_shape
                     and reference.axes_manager.navigation_size
                 ):
                     raise ValueError(
                         "The navigation dimensions of object and"
@@ -476,22 +489,22 @@
             num_workers=num_workers,
         )
 
         # Standard edge smoothness of sideband aperture 5% of sb_size
         if sb_smoothness is None:
             sb_smoothness = sb_size * 0.05
         else:
-            if not isinstance(sb_smoothness, BaseSignal):
+            if not isinstance(sb_smoothness, hs.signals.BaseSignal):
                 if (
                     isinstance(sb_smoothness, (np.ndarray, daArray))
                     and sb_smoothness.size > 1
                 ):
-                    sb_smoothness = BaseSignal(sb_smoothness).T
+                    sb_smoothness = hs.signals.BaseSignal(sb_smoothness).T
                 else:
-                    sb_smoothness = BaseSignal(sb_smoothness)
+                    sb_smoothness = hs.signals.BaseSignal(sb_smoothness)
                 if isinstance(sb_smoothness.data, daArray):
                     sb_smoothness = sb_smoothness.as_lazy()
 
         if (
             sb_smoothness.axes_manager.navigation_size
             != self.axes_manager.navigation_size
         ):
```

### Comparing `holospy-0.2/holospy/tests/signals/test_hologram_image.py` & `holospy-0.3/holospy/tests/signals/test_hologram_image.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,22 +14,22 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with HyperSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
 
 import gc
 
+import hyperspy.api as hs
 import matplotlib.pyplot as plt
 import numpy as np
 import pytest
+from hyperspy.decorators import lazifyTestClass
 from scipy.interpolate import RectBivariateSpline
 
-import hyperspy.api as hs
-from holospy.signals.hologram_image import HologramImage
-from hyperspy.decorators import lazifyTestClass
+from holospy.signals.hologram_image import HologramImage, _ureg
 
 # Set parameters outside the tests
 img_size = 256
 IMG_SIZE3X = 128
 IMG_SIZE3Y = 64
 FRINGE_DIRECTION = -np.pi / 6
 FRINGE_SPACING = 5.23
@@ -326,7 +326,16 @@
         holo_image3.reconstruct_phase(sb_size=sb_size_mismatched)
     with pytest.raises(ValueError):
         holo_image3.reconstruct_phase(sb_smoothness=sb_smoothness_mismatched)
 
     #   e. Beam energy is not assigned, while 'mrad' units selected
     with pytest.raises(AttributeError):
         holo_image3.reconstruct_phase(sb_size=40, sb_unit="mrad")
+
+
+def test_pint_unit_registry():
+    # Check that holospy and hyperspy share the same UnitRegistry
+    s = hs.signals.Signal1D(np.arange(10))
+    # this will not work if the UnitRegistry are not the same
+    s.axes_manager[0].scale_as_quantity = "2.5 µm"
+    s.axes_manager[0].scale_as_quantity += 2e-6 * _ureg.meter
+    assert s.axes_manager[0].scale == 4.5
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `holospy-0.2/holospy/tests/signals/test_hologram_image_statistics.py` & `holospy-0.3/holospy/tests/signals/test_hologram_image_statistics.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,23 +13,21 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with HyperSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
 
 
+import hyperspy.api as hs
 import numpy as np
 import pytest
 import scipy.constants as constants
 
-import hyperspy.api as hs
-
 import holospy as holo
 
-
 # Set parameters outside the tests
 img_size = 256
 IMG_SIZE3X = 128
 IMG_SIZE3Y = 64
 FRINGE_DIRECTION = -np.pi / 6
 FRINGE_SPACING = 5.23
 FRINGE_DIRECTION3 = np.pi / 3
```

### Comparing `holospy-0.2/holospy/tests/test_non-uniform_not-implemented.py` & `holospy-0.3/holospy/tests/test_non-uniform_not-implemented.py`

 * *Files identical despite different names*

### Comparing `holospy-0.2/holospy/tools.py` & `holospy-0.3/holospy/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,17 +12,18 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with HyperSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
 
+import logging
+
 import numpy as np
 from scipy.fftpack import fft2
-import logging
 
 _logger = logging.getLogger(__name__)
 
 
 def calculate_carrier_frequency(data, sb_position, scale):
     """
     Calculates fringe carrier frequency of a hologram
```

### Comparing `holospy-0.2/holospy.egg-info/PKG-INFO` & `holospy-0.3/holospy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: holospy
-Version: 0.2
+Version: 0.3
 Summary: Analysis of (off-axis) electron holography data with HyperSpy.
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -695,14 +695,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: hyperspy>=2.0rc0
 Requires-Dist: numpy>=1.20.0
+Requires-Dist: pint>=0.10
 Requires-Dist: scipy>=1.5.0
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-cov; extra == "tests"
 Requires-Dist: setuptools-scm; extra == "tests"
 Provides-Extra: doc
 Requires-Dist: numpydoc; extra == "doc"
@@ -714,19 +715,25 @@
 Requires-Dist: towncrier; extra == "doc"
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: holospy[doc]; extra == "dev"
 Requires-Dist: holospy[tests]; extra == "dev"
 
 
+[![Docs](https://readthedocs.org/projects/holospy/badge/?version=latest)](https://holospy.readthedocs.io/en/latest/?badge=latest)
 [![Tests](https://github.com/hyperspy/holospy/actions/workflows/tests.yml/badge.svg)](https://github.com/hyperspy/holospy/actions/workflows/tests.yml)
 [![codecov](https://codecov.io/gh/hyperspy/holospy/graph/badge.svg?token=XB1QDTXQ86)](https://codecov.io/gh/hyperspy/holospy)
-[![Docs](https://readthedocs.org/projects/holospy/badge/?version=latest)](https://holospy.readthedocs.io/en/latest/?badge=latest)
+[![CodeQL](https://github.com/hyperspy/holospy/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/hyperspy/holospy/actions/workflows/github-code-scanning/codeql)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/hyperspy/holospy/main.svg)](https://results.pre-commit.ci/latest/github/hyperspy/holospy/main)
+
+[![Python Version](https://img.shields.io/pypi/pyversions/holospy.svg?style=flat)](https://pypi.python.org/pypi/holospy)
+[![PyPi Version](http://img.shields.io/pypi/v/holospy.svg?style=flat)](https://pypi.python.org/pypi/holospy)
+[![Anaconda Version](https://anaconda.org/conda-forge/holospy/badges/version.svg)](https://anaconda.org/conda-forge/holospy)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
-[![DOI](https://zenodo.org/badge/2233998.svg)](https://zenodo.org/badge/latestdoi/2233998)
+[![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.10137993.svg)](https://doi.org/10.5281/zenodo.10137993)
 
 **HoloSpy** is a Python package extending the functionality for multi-dimensional
 data analysis provided by the [HyperSpy](https://hyperspy.org) library. It is
 aimed at helping with the analysis of (off-axis) electron holography data.
 
 Go to the documentation for instructions on how to install HoloSpy and start an
 analysis: [Read the docs](https://holospy.readthedocs.io).
```

### Comparing `holospy-0.2/holospy.egg-info/SOURCES.txt` & `holospy-0.3/holospy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `holospy-0.2/prepare_release.py` & `holospy-0.3/prepare_release.py`

 * *Files identical despite different names*

### Comparing `holospy-0.2/pyproject.toml` & `holospy-0.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -32,14 +32,15 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
   "hyperspy>=2.0rc0",
   "numpy>=1.20.0",
+  "pint>=0.10",
   "scipy>=1.5.0",
 ]
 dynamic = ["version"]
 
 [project.entry-points."hyperspy.extensions"]
 holospy = "holospy"
 
@@ -87,27 +88,42 @@
 #  "-ra",  # Display summary: "all except passes"
 addopts = "-ra"
 minversion = "6.0"
 testpaths = [
   "holospy/tests",
 ]
 
+[tool.ruff.lint]
+select = [
+    # Pyflakes
+    "F",
+    # Pycodestyle
+    "E",
+    "W",
+    # isort
+    "I"
+]
+# Rely on the formatter to define line-length
+# and avoid conflicting lint rules
+# https://docs.astral.sh/ruff/formatter/#conflicting-lint-rules
+extend-ignore = ["E501"]
+
 [tool.setuptools.packages.find]
 include = ["holospy*"]
 
 [tool.setuptools.package-data]
 "*" = [
   "*hdf5",
   "*.yaml"
   ]
 
 [tool.setuptools_scm]
 # Presence enables setuptools_scm, the version will be determine at build time from git
 # The version will be updated by the `prepare_release.py` script
-fallback_version = "0.3.dev0"
+fallback_version = "0.4.dev0"
 
 [tool.towncrier]
 directory = "upcoming_changes/"
 filename = "CHANGES.rst"
 issue_format = "`#{issue} <https://github.com/hyperspy/holospy/issues/{issue}>`_"
 title_format = "{version} ({project_date})"
 package_dir = "holospy"
```

### Comparing `holospy-0.2/releasing_guide.md` & `holospy-0.3/releasing_guide.md`

 * *Files identical despite different names*

### Comparing `holospy-0.2/upcoming_changes/README.rst` & `holospy-0.3/upcoming_changes/README.rst`

 * *Files identical despite different names*

